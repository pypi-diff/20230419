# Comparing `tmp/sqlalchemy-spanner-1.4.0.tar.gz` & `tmp/sqlalchemy-spanner-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-spanner-1.4.0.tar", last modified: Mon Apr 10 05:40:20 2023, max compression
+gzip compressed data, was "sqlalchemy-spanner-1.5.0.tar", last modified: Wed Apr 19 07:47:15 2023, max compression
```

## Comparing `sqlalchemy-spanner-1.4.0.tar` & `sqlalchemy-spanner-1.5.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-10 05:40:20.883465 sqlalchemy-spanner-1.4.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/LICENSE
--rw-r--r--   0 root         (0)     1003    17665 2023-04-10 05:40:20.883465 sqlalchemy-spanner-1.4.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    17292 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-10 05:40:20.879465 sqlalchemy-spanner-1.4.0/google/
--rw-rw-r--   0 root         (0)     1003      747 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-10 05:40:20.879465 sqlalchemy-spanner-1.4.0/google/cloud/
--rw-rw-r--   0 root         (0)     1003      747 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-10 05:40:20.883465 sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/
--rw-rw-r--   0 root         (0)     1003      651 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/__init__.py
--rw-rw-r--   0 root         (0)     1003     1988 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py
--rw-rw-r--   0 root         (0)     1003      792 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/provision.py
--rw-rw-r--   0 root         (0)     1003     2675 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/requirements.py
--rw-rw-r--   0 root         (0)     1003    35544 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/sqlalchemy_spanner.py
--rw-rw-r--   0 root         (0)     1003      261 2023-04-10 05:40:20.887465 sqlalchemy-spanner-1.4.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2431 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-10 05:40:20.883465 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/
--rw-r--r--   0 root         (0)     1003    17665 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      720 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       87 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/entry_points.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      155 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-10 05:40:20.883465 sqlalchemy-spanner-1.4.0/test/
--rw-rw-r--   0 root         (0)     1003    66314 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/test/test_suite_13.py
--rw-rw-r--   0 root         (0)     1003    75361 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/test/test_suite_14.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 07:47:15.121830 sqlalchemy-spanner-1.5.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/LICENSE
+-rw-r--r--   0 root         (0)     1003    17665 2023-04-19 07:47:15.121830 sqlalchemy-spanner-1.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003    17292 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 07:47:15.117831 sqlalchemy-spanner-1.5.0/google/
+-rw-rw-r--   0 root         (0)     1003      747 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 07:47:15.117831 sqlalchemy-spanner-1.5.0/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      747 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 07:47:15.117831 sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/
+-rw-rw-r--   0 root         (0)     1003      651 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1988 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py
+-rw-rw-r--   0 root         (0)     1003      792 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/provision.py
+-rw-rw-r--   0 root         (0)     1003     3140 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/requirements.py
+-rw-rw-r--   0 root         (0)     1003    49547 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/sqlalchemy_spanner.py
+-rw-rw-r--   0 root         (0)     1003      261 2023-04-19 07:47:15.121830 sqlalchemy-spanner-1.5.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2431 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 07:47:15.121830 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/
+-rw-r--r--   0 root         (0)     1003    17665 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      742 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       87 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      155 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 07:47:15.121830 sqlalchemy-spanner-1.5.0/test/
+-rw-rw-r--   0 root         (0)     1003    68740 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/test/test_suite_13.py
+-rw-rw-r--   0 root         (0)     1003    81211 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/test/test_suite_14.py
+-rw-rw-r--   0 root         (0)     1003   102613 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/test/test_suite_20.py
```

### Comparing `sqlalchemy-spanner-1.4.0/LICENSE` & `sqlalchemy-spanner-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.4.0/PKG-INFO` & `sqlalchemy-spanner-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-spanner
-Version: 1.4.0
+Version: 1.5.0
 Summary: SQLAlchemy dialect integrated into Cloud Spanner database
 Home-page: https://github.com/cloudspannerecosystem/python-spanner-sqlalchemy
 Author: Google LLC
 Author-email: cloud-spanner-developers@googlegroups.com
 Classifier: Intended Audience :: Developers
 Provides-Extra: tracing
 License-File: LICENSE
```

### Comparing `sqlalchemy-spanner-1.4.0/README.rst` & `sqlalchemy-spanner-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.4.0/google/__init__.py` & `sqlalchemy-spanner-1.5.0/google/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.4.0/google/cloud/__init__.py` & `sqlalchemy-spanner-1.5.0/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/__init__.py` & `sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py` & `sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/provision.py` & `sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/provision.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/requirements.py` & `sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/requirements.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from sqlalchemy.testing import exclusions
 from sqlalchemy.testing.requirements import SuiteRequirements
+from sqlalchemy.testing.exclusions import against, only_on
 
 
 class Requirements(SuiteRequirements):  # pragma: no cover
     @property
     def json_type(self):
         return exclusions.open()
 
@@ -42,14 +43,23 @@
         return exclusions.open()
 
     @property
     def schema_reflection(self):
         return exclusions.open()
 
     @property
+    def array_type(self):
+        return only_on([lambda config: against(config, "postgresql")])
+
+    @property
+    def uuid_data_type(self):
+        """Return databases that support the UUID datatype."""
+        return only_on(("postgresql >= 8.3", "mariadb >= 10.7.0"))
+
+    @property
     def implicitly_named_constraints(self):
         return exclusions.open()
 
     @property
     def autocommit(self):
         return exclusions.open()
 
@@ -95,7 +105,12 @@
         return {"default": "SERIALIZABLE", "supported": ["SERIALIZABLE", "AUTOCOMMIT"]}
 
     @property
     def precision_numerics_enotation_large(self):
         """target backend supports Decimal() objects using E notation
         to represent very large values."""
         return exclusions.open()
+
+    @property
+    def views(self):
+        """Target database must support VIEWs."""
+        return exclusions.open()
```

### Comparing `sqlalchemy-spanner-1.4.0/setup.py` & `sqlalchemy-spanner-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/PKG-INFO` & `sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-spanner
-Version: 1.4.0
+Version: 1.5.0
 Summary: SQLAlchemy dialect integrated into Cloud Spanner database
 Home-page: https://github.com/cloudspannerecosystem/python-spanner-sqlalchemy
 Author: Google LLC
 Author-email: cloud-spanner-developers@googlegroups.com
 Classifier: Intended Audience :: Developers
 Provides-Extra: tracing
 License-File: LICENSE
```

### Comparing `sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/SOURCES.txt` & `sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 sqlalchemy_spanner.egg-info/dependency_links.txt
 sqlalchemy_spanner.egg-info/entry_points.txt
 sqlalchemy_spanner.egg-info/namespace_packages.txt
 sqlalchemy_spanner.egg-info/not-zip-safe
 sqlalchemy_spanner.egg-info/requires.txt
 sqlalchemy_spanner.egg-info/top_level.txt
 test/test_suite_13.py
-test/test_suite_14.py
+test/test_suite_14.py
+test/test_suite_20.py
```

### Comparing `sqlalchemy-spanner-1.4.0/test/test_suite_13.py` & `sqlalchemy-spanner-1.5.0/test/test_suite_13.py`

 * *Files 2% similar despite different names*

```diff
@@ -523,14 +523,42 @@
     """
 
     pass
 
 
 class ComponentReflectionTest(_ComponentReflectionTest):
     @classmethod
+    def define_views(cls, metadata, schema):
+        table_info = {
+            "users": ["user_id", "test1", "test2"],
+            "email_addresses": ["address_id", "remote_user_id", "email_address"],
+        }
+        if testing.requires.self_referential_foreign_keys.enabled:
+            table_info["users"] = table_info["users"] + ["parent_user_id"]
+        for table_name in ("users", "email_addresses"):
+            fullname = table_name
+            if schema:
+                fullname = "%s.%s" % (schema, table_name)
+            view_name = fullname + "_v"
+            columns = ""
+            for column in table_info[table_name]:
+                stmt = table_name + "." + column + " AS " + column
+                if columns:
+                    columns = columns + ", " + stmt
+                else:
+                    columns = stmt
+            query = f"""CREATE VIEW {view_name}
+                SQL SECURITY INVOKER
+                AS SELECT {columns}
+                FROM {fullname}"""
+
+            event.listen(metadata, "after_create", DDL(query))
+            event.listen(metadata, "before_drop", DDL("DROP VIEW %s" % view_name))
+
+    @classmethod
     def define_reflected_tables(cls, metadata, schema):
         if schema:
             schema_prefix = schema + "."
         else:
             schema_prefix = ""
 
         if testing.requires.self_referential_foreign_keys.enabled:
@@ -661,19 +689,32 @@
                     test_needs_fk=True,
                 )
 
                 if testing.requires.indexes_with_ascdesc.enabled:
                     sqlalchemy.Index("noncol_idx_nopk", noncol_idx_test_nopk.c.q.desc())
                     sqlalchemy.Index("noncol_idx_pk", noncol_idx_test_pk.c.q.desc())
 
-        if testing.requires.view_column_reflection.enabled:
+        if testing.requires.view_column_reflection.enabled and not bool(
+            os.environ.get("SPANNER_EMULATOR_HOST")
+        ):
             cls.define_views(metadata, schema)
         if not schema and testing.requires.temp_table_reflection.enabled:
             cls.define_temp_tables(metadata)
 
+    def _test_get_columns(self, schema=None, table_type="table"):
+        if table_type == "view" and bool(os.environ.get("SPANNER_EMULATOR_HOST")):
+            pytest.skip("View tables not supported on emulator")
+        super()._test_get_columns(schema, table_type)
+
+    @testing.provide_metadata
+    def _test_get_view_definition(self, schema=None):
+        if bool(os.environ.get("SPANNER_EMULATOR_HOST")):
+            pytest.skip("View tables not supported on emulator")
+        super()._test_get_view_definition(schema)
+
     @classmethod
     def define_temp_tables(cls, metadata):
         """
         SPANNER OVERRIDE:
 
         In Cloud Spanner unique indexes are used instead of directly
         creating unique constraints. Overriding the test to replace
@@ -854,15 +895,15 @@
             "remote_table",
             "remote_table_2",
         ]
         meta = self.metadata
 
         insp = inspect(meta.bind)
 
-        if table_type == "view":
+        if table_type == "view" and not bool(os.environ.get("SPANNER_EMULATOR_HOST")):
             table_names = insp.get_view_names(schema)
             table_names.sort()
             answer = ["email_addresses_v", "users_v"]
             eq_(sorted(table_names), answer)
         else:
             if order_by:
                 tables = [
@@ -917,22 +958,22 @@
     @testing.requires.table_reflection
     def test_array_reflection(self):
         """Check array columns reflection."""
         orig_meta = self.metadata
 
         str_array = ARRAY(String(16))
         int_array = ARRAY(Integer)
-        Table(
+        arrays_test = Table(
             "arrays_test",
             orig_meta,
             Column("id", Integer, primary_key=True),
             Column("str_array", str_array),
             Column("int_array", int_array),
         )
-        orig_meta.create_all()
+        arrays_test.create(create_engine(get_db_url()))
 
         # autoload the table and check its columns reflection
         tab = Table("arrays_test", orig_meta, autoload=True)
         col_types = [col.type for col in tab.columns]
         for type_ in (
             str_array,
             int_array,
@@ -965,14 +1006,30 @@
         insp = inspect(meta.bind)
         foreign_keys = insp.get_foreign_keys(self.tables.tb2.name)
         eq_(len(foreign_keys), 1)
         fkey1 = foreign_keys[0]
         eq_(set(fkey1.get("referred_columns")), {"name", "id", "attr"})
         eq_(set(fkey1.get("constrained_columns")), {"pname", "pid", "pattr"})
 
+    @testing.requires.primary_key_constraint_reflection
+    def test_pk_column_order(self, connection):
+        """
+        SPANNER OVERRIDE:
+        Emultor doesn't support returning pk sorted by ordinal value
+        of columns.
+        """
+        insp = inspect(connection)
+        primary_key = insp.get_pk_constraint(self.tables.tb1.name)
+        exp = (
+            ["id", "name", "attr"]
+            if bool(os.environ.get("SPANNER_EMULATOR_HOST"))
+            else ["name", "id", "attr"]
+        )
+        eq_(primary_key.get("constrained_columns"), exp)
+
 
 class RowFetchTest(_RowFetchTest):
     def test_row_w_scalar_select(self):
         """
         SPANNER OVERRIDE:
 
         Cloud Spanner returns a DatetimeWithNanoseconds() for date
```

### Comparing `sqlalchemy-spanner-1.4.0/test/test_suite_14.py` & `sqlalchemy-spanner-1.5.0/test/test_suite_14.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,4588 +124,4953 @@
 000007b0: 656d 792e 7479 7065 7320 696d 706f 7274  emy.types import
 000007c0: 2054 6578 740a 6672 6f6d 2073 716c 616c   Text.from sqlal
 000007d0: 6368 656d 792e 7465 7374 696e 6720 696d  chemy.testing im
 000007e0: 706f 7274 2072 6571 7569 7265 730a 6672  port requires.fr
 000007f0: 6f6d 2073 716c 616c 6368 656d 792e 7465  om sqlalchemy.te
 00000800: 7374 696e 6720 696d 706f 7274 2069 735f  sting import is_
 00000810: 7472 7565 0a66 726f 6d20 7371 6c61 6c63  true.from sqlalc
-00000820: 6865 6d79 2e74 6573 7469 6e67 2e66 6978  hemy.testing.fix
-00000830: 7475 7265 7320 696d 706f 7274 2028 0a20  tures import (. 
-00000840: 2020 2043 6f6d 7075 7465 6452 6566 6c65     ComputedRefle
-00000850: 6374 696f 6e46 6978 7475 7265 5465 7374  ctionFixtureTest
-00000860: 2061 7320 5f43 6f6d 7075 7465 6452 6566   as _ComputedRef
-00000870: 6c65 6374 696f 6e46 6978 7475 7265 5465  lectionFixtureTe
-00000880: 7374 2c0a 290a 0a66 726f 6d20 676f 6f67  st,.)..from goog
-00000890: 6c65 2e61 7069 5f63 6f72 652e 6461 7465  le.api_core.date
-000008a0: 7469 6d65 5f68 656c 7065 7273 2069 6d70  time_helpers imp
-000008b0: 6f72 7420 4461 7465 7469 6d65 5769 7468  ort DatetimeWith
-000008c0: 4e61 6e6f 7365 636f 6e64 730a 0a66 726f  Nanoseconds..fro
-000008d0: 6d20 676f 6f67 6c65 2e63 6c6f 7564 2069  m google.cloud i
-000008e0: 6d70 6f72 7420 7370 616e 6e65 725f 6462  mport spanner_db
-000008f0: 6170 690a 0a66 726f 6d20 7371 6c61 6c63  api..from sqlalc
-00000900: 6865 6d79 2e74 6573 7469 6e67 2e73 7569  hemy.testing.sui
-00000910: 7465 2e74 6573 745f 6374 6520 696d 706f  te.test_cte impo
-00000920: 7274 202a 2020 2320 6e6f 7161 3a20 4634  rt *  # noqa: F4
-00000930: 3031 2c20 4634 3033 0a66 726f 6d20 7371  01, F403.from sq
-00000940: 6c61 6c63 6865 6d79 2e74 6573 7469 6e67  lalchemy.testing
-00000950: 2e73 7569 7465 2e74 6573 745f 6464 6c20  .suite.test_ddl 
-00000960: 696d 706f 7274 202a 2020 2320 6e6f 7161  import *  # noqa
-00000970: 3a20 4634 3031 2c20 4634 3033 0a66 726f  : F401, F403.fro
-00000980: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
-00000990: 7469 6e67 2e73 7569 7465 2e74 6573 745f  ting.suite.test_
-000009a0: 6469 616c 6563 7420 696d 706f 7274 202a  dialect import *
-000009b0: 2020 2320 6e6f 7161 3a20 4634 3031 2c20    # noqa: F401, 
-000009c0: 4634 3033 0a66 726f 6d20 7371 6c61 6c63  F403.from sqlalc
-000009d0: 6865 6d79 2e74 6573 7469 6e67 2e73 7569  hemy.testing.sui
-000009e0: 7465 2e74 6573 745f 696e 7365 7274 2069  te.test_insert i
-000009f0: 6d70 6f72 7420 2a20 2023 206e 6f71 613a  mport *  # noqa:
-00000a00: 2046 3430 312c 2046 3430 330a 6672 6f6d   F401, F403.from
-00000a10: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
-00000a20: 696e 672e 7375 6974 652e 7465 7374 5f72  ing.suite.test_r
-00000a30: 6566 6c65 6374 696f 6e20 696d 706f 7274  eflection import
-00000a40: 202a 2020 2320 6e6f 7161 3a20 4634 3031   *  # noqa: F401
-00000a50: 2c20 4634 3033 0a66 726f 6d20 7371 6c61  , F403.from sqla
-00000a60: 6c63 6865 6d79 2e74 6573 7469 6e67 2e73  lchemy.testing.s
-00000a70: 7569 7465 2e74 6573 745f 7265 7375 6c74  uite.test_result
-00000a80: 7320 696d 706f 7274 202a 2020 2320 6e6f  s import *  # no
-00000a90: 7161 3a20 4634 3031 2c20 4634 3033 0a66  qa: F401, F403.f
-00000aa0: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
-00000ab0: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
-00000ac0: 745f 7365 6c65 6374 2069 6d70 6f72 7420  t_select import 
-00000ad0: 2a20 2023 206e 6f71 613a 2046 3430 312c  *  # noqa: F401,
-00000ae0: 2046 3430 330a 6672 6f6d 2073 716c 616c   F403.from sqlal
-00000af0: 6368 656d 792e 7465 7374 696e 672e 7375  chemy.testing.su
-00000b00: 6974 652e 7465 7374 5f73 6571 7565 6e63  ite.test_sequenc
-00000b10: 6520 696d 706f 7274 202a 2020 2320 6e6f  e import *  # no
-00000b20: 7161 3a20 4634 3031 2c20 4634 3033 0a66  qa: F401, F403.f
-00000b30: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
-00000b40: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
-00000b50: 745f 7570 6461 7465 5f64 656c 6574 6520  t_update_delete 
-00000b60: 696d 706f 7274 202a 2020 2320 6e6f 7161  import *  # noqa
-00000b70: 3a20 4634 3031 2c20 4634 3033 0a66 726f  : F401, F403.fro
-00000b80: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
-00000b90: 7469 6e67 2e73 7569 7465 2e74 6573 745f  ting.suite.test_
-00000ba0: 6374 6520 696d 706f 7274 2043 5445 5465  cte import CTETe
-00000bb0: 7374 2061 7320 5f43 5445 5465 7374 0a66  st as _CTETest.f
-00000bc0: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
-00000bd0: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
-00000be0: 745f 6464 6c20 696d 706f 7274 2054 6162  t_ddl import Tab
-00000bf0: 6c65 4444 4c54 6573 7420 6173 205f 5461  leDDLTest as _Ta
-00000c00: 626c 6544 444c 5465 7374 0a66 726f 6d20  bleDDLTest.from 
-00000c10: 7371 6c61 6c63 6865 6d79 2e74 6573 7469  sqlalchemy.testi
-00000c20: 6e67 2e73 7569 7465 2e74 6573 745f 6464  ng.suite.test_dd
-00000c30: 6c20 696d 706f 7274 2028 0a20 2020 2046  l import (.    F
-00000c40: 7574 7572 6554 6162 6c65 4444 4c54 6573  utureTableDDLTes
-00000c50: 7420 6173 205f 4675 7475 7265 5461 626c  t as _FutureTabl
-00000c60: 6544 444c 5465 7374 2c0a 2020 2020 4c6f  eDDLTest,.    Lo
-00000c70: 6e67 4e61 6d65 426c 6f77 6f75 7454 6573  ngNameBlowoutTes
-00000c80: 7420 6173 205f 4c6f 6e67 4e61 6d65 426c  t as _LongNameBl
-00000c90: 6f77 6f75 7454 6573 742c 0a29 0a66 726f  owoutTest,.).fro
-00000ca0: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
-00000cb0: 7469 6e67 2e73 7569 7465 2e74 6573 745f  ting.suite.test_
-00000cc0: 7570 6461 7465 5f64 656c 6574 6520 696d  update_delete im
-00000cd0: 706f 7274 2028 0a20 2020 2053 696d 706c  port (.    Simpl
-00000ce0: 6555 7064 6174 6544 656c 6574 6554 6573  eUpdateDeleteTes
-00000cf0: 7420 6173 205f 5369 6d70 6c65 5570 6461  t as _SimpleUpda
-00000d00: 7465 4465 6c65 7465 5465 7374 2c0a 290a  teDeleteTest,.).
-00000d10: 6672 6f6d 2073 716c 616c 6368 656d 792e  from sqlalchemy.
-00000d20: 7465 7374 696e 672e 7375 6974 652e 7465  testing.suite.te
-00000d30: 7374 5f64 6961 6c65 6374 2069 6d70 6f72  st_dialect impor
-00000d40: 7420 280a 2020 2020 4469 6666 6963 756c  t (.    Difficul
-00000d50: 7450 6172 616d 6574 6572 7354 6573 7420  tParametersTest 
-00000d60: 6173 205f 4469 6666 6963 756c 7450 6172  as _DifficultPar
-00000d70: 616d 6574 6572 7354 6573 742c 0a20 2020  ametersTest,.   
-00000d80: 2045 7363 6170 696e 6754 6573 7420 6173   EscapingTest as
-00000d90: 205f 4573 6361 7069 6e67 5465 7374 2c0a   _EscapingTest,.
-00000da0: 290a 6672 6f6d 2073 716c 616c 6368 656d  ).from sqlalchem
-00000db0: 792e 7465 7374 696e 672e 7375 6974 652e  y.testing.suite.
-00000dc0: 7465 7374 5f69 6e73 6572 7420 696d 706f  test_insert impo
-00000dd0: 7274 2028 0a20 2020 2049 6e73 6572 7442  rt (.    InsertB
-00000de0: 6568 6176 696f 7254 6573 7420 6173 205f  ehaviorTest as _
-00000df0: 496e 7365 7274 4265 6861 7669 6f72 5465  InsertBehaviorTe
-00000e00: 7374 2c0a 290a 6672 6f6d 2073 716c 616c  st,.).from sqlal
-00000e10: 6368 656d 792e 7465 7374 696e 672e 7375  chemy.testing.su
-00000e20: 6974 652e 7465 7374 5f73 656c 6563 7420  ite.test_select 
-00000e30: 696d 706f 7274 2028 2020 2320 6e6f 7161  import (  # noqa
-00000e40: 3a20 4634 3031 2c20 4634 3033 0a20 2020  : F401, F403.   
-00000e50: 2043 6f6d 706f 756e 6453 656c 6563 7454   CompoundSelectT
-00000e60: 6573 7420 6173 205f 436f 6d70 6f75 6e64  est as _Compound
-00000e70: 5365 6c65 6374 5465 7374 2c0a 2020 2020  SelectTest,.    
-00000e80: 4578 6973 7473 5465 7374 2061 7320 5f45  ExistsTest as _E
-00000e90: 7869 7374 7354 6573 742c 0a20 2020 2046  xistsTest,.    F
-00000ea0: 6574 6368 4c69 6d69 744f 6666 7365 7454  etchLimitOffsetT
-00000eb0: 6573 7420 6173 205f 4665 7463 684c 696d  est as _FetchLim
-00000ec0: 6974 4f66 6673 6574 5465 7374 2c0a 2020  itOffsetTest,.  
-00000ed0: 2020 4964 656e 7469 7479 4175 746f 696e    IdentityAutoin
-00000ee0: 6372 656d 656e 7454 6573 7420 6173 205f  crementTest as _
-00000ef0: 4964 656e 7469 7479 4175 746f 696e 6372  IdentityAutoincr
-00000f00: 656d 656e 7454 6573 742c 0a20 2020 2049  ementTest,.    I
-00000f10: 734f 7249 734e 6f74 4469 7374 696e 6374  sOrIsNotDistinct
-00000f20: 4672 6f6d 5465 7374 2061 7320 5f49 734f  FromTest as _IsO
-00000f30: 7249 734e 6f74 4469 7374 696e 6374 4672  rIsNotDistinctFr
-00000f40: 6f6d 5465 7374 2c0a 2020 2020 4c69 6b65  omTest,.    Like
-00000f50: 4675 6e63 7469 6f6e 7354 6573 7420 6173  FunctionsTest as
-00000f60: 205f 4c69 6b65 4675 6e63 7469 6f6e 7354   _LikeFunctionsT
-00000f70: 6573 742c 0a20 2020 204f 7264 6572 4279  est,.    OrderBy
-00000f80: 4c61 6265 6c54 6573 7420 6173 205f 4f72  LabelTest as _Or
-00000f90: 6465 7242 794c 6162 656c 5465 7374 2c0a  derByLabelTest,.
-00000fa0: 2020 2020 506f 7374 436f 6d70 696c 6550      PostCompileP
-00000fb0: 6172 616d 7354 6573 7420 6173 205f 506f  aramsTest as _Po
-00000fc0: 7374 436f 6d70 696c 6550 6172 616d 7354  stCompileParamsT
-00000fd0: 6573 742c 0a29 0a66 726f 6d20 7371 6c61  est,.).from sqla
-00000fe0: 6c63 6865 6d79 2e74 6573 7469 6e67 2e73  lchemy.testing.s
-00000ff0: 7569 7465 2e74 6573 745f 7265 666c 6563  uite.test_reflec
-00001000: 7469 6f6e 2069 6d70 6f72 7420 280a 2020  tion import (.  
-00001010: 2020 436f 6d70 6f6e 656e 7452 6566 6c65    ComponentRefle
-00001020: 6374 696f 6e54 6573 7445 7874 7261 2061  ctionTestExtra a
-00001030: 7320 5f43 6f6d 706f 6e65 6e74 5265 666c  s _ComponentRefl
-00001040: 6563 7469 6f6e 5465 7374 4578 7472 612c  ectionTestExtra,
-00001050: 0a20 2020 2051 756f 7465 644e 616d 6541  .    QuotedNameA
-00001060: 7267 756d 656e 7454 6573 7420 6173 205f  rgumentTest as _
-00001070: 5175 6f74 6564 4e61 6d65 4172 6775 6d65  QuotedNameArgume
-00001080: 6e74 5465 7374 2c0a 2020 2020 436f 6d70  ntTest,.    Comp
-00001090: 6f6e 656e 7452 6566 6c65 6374 696f 6e54  onentReflectionT
-000010a0: 6573 7420 6173 205f 436f 6d70 6f6e 656e  est as _Componen
-000010b0: 7452 6566 6c65 6374 696f 6e54 6573 742c  tReflectionTest,
-000010c0: 0a20 2020 2043 6f6d 706f 7369 7465 4b65  .    CompositeKe
-000010d0: 7952 6566 6c65 6374 696f 6e54 6573 7420  yReflectionTest 
-000010e0: 6173 205f 436f 6d70 6f73 6974 654b 6579  as _CompositeKey
-000010f0: 5265 666c 6563 7469 6f6e 5465 7374 2c0a  ReflectionTest,.
-00001100: 2020 2020 436f 6d70 7574 6564 5265 666c      ComputedRefl
-00001110: 6563 7469 6f6e 5465 7374 2061 7320 5f43  ectionTest as _C
-00001120: 6f6d 7075 7465 6452 6566 6c65 6374 696f  omputedReflectio
-00001130: 6e54 6573 742c 0a20 2020 2048 6173 496e  nTest,.    HasIn
-00001140: 6465 7854 6573 7420 6173 205f 4861 7349  dexTest as _HasI
-00001150: 6e64 6578 5465 7374 2c0a 2020 2020 4861  ndexTest,.    Ha
-00001160: 7354 6162 6c65 5465 7374 2061 7320 5f48  sTableTest as _H
-00001170: 6173 5461 626c 6554 6573 742c 0a29 0a66  asTableTest,.).f
-00001180: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
-00001190: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
-000011a0: 745f 7265 7375 6c74 7320 696d 706f 7274  t_results import
-000011b0: 2052 6f77 4665 7463 6854 6573 7420 6173   RowFetchTest as
-000011c0: 205f 526f 7746 6574 6368 5465 7374 0a66   _RowFetchTest.f
-000011d0: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
-000011e0: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
-000011f0: 745f 7479 7065 7320 696d 706f 7274 2028  t_types import (
-00001200: 2020 2320 6e6f 7161 3a20 4634 3031 2c20    # noqa: F401, 
-00001210: 4634 3033 0a20 2020 2042 6f6f 6c65 616e  F403.    Boolean
-00001220: 5465 7374 2061 7320 5f42 6f6f 6c65 616e  Test as _Boolean
-00001230: 5465 7374 2c0a 2020 2020 4461 7465 5465  Test,.    DateTe
-00001240: 7374 2061 7320 5f44 6174 6554 6573 742c  st as _DateTest,
-00001250: 0a20 2020 205f 4461 7465 4669 7874 7572  .    _DateFixtur
-00001260: 6520 6173 205f 5f44 6174 6546 6978 7475  e as __DateFixtu
-00001270: 7265 2c0a 2020 2020 4461 7465 5469 6d65  re,.    DateTime
-00001280: 4869 7374 6f72 6963 5465 7374 2c0a 2020  HistoricTest,.  
-00001290: 2020 4461 7465 5469 6d65 436f 6572 6365    DateTimeCoerce
-000012a0: 6454 6f44 6174 6554 696d 6554 6573 7420  dToDateTimeTest 
-000012b0: 6173 205f 4461 7465 5469 6d65 436f 6572  as _DateTimeCoer
-000012c0: 6365 6454 6f44 6174 6554 696d 6554 6573  cedToDateTimeTes
-000012d0: 742c 0a20 2020 2044 6174 6554 696d 654d  t,.    DateTimeM
-000012e0: 6963 726f 7365 636f 6e64 7354 6573 7420  icrosecondsTest 
-000012f0: 6173 205f 4461 7465 5469 6d65 4d69 6372  as _DateTimeMicr
-00001300: 6f73 6563 6f6e 6473 5465 7374 2c0a 2020  osecondsTest,.  
-00001310: 2020 4461 7465 5469 6d65 5465 7374 2061    DateTimeTest a
-00001320: 7320 5f44 6174 6554 696d 6554 6573 742c  s _DateTimeTest,
-00001330: 0a20 2020 2049 6e74 6567 6572 5465 7374  .    IntegerTest
-00001340: 2061 7320 5f49 6e74 6567 6572 5465 7374   as _IntegerTest
-00001350: 2c0a 2020 2020 4a53 4f4e 5465 7374 2061  ,.    JSONTest a
-00001360: 7320 5f4a 534f 4e54 6573 742c 0a20 2020  s _JSONTest,.   
-00001370: 205f 4c69 7465 7261 6c52 6f75 6e64 5472   _LiteralRoundTr
-00001380: 6970 4669 7874 7572 652c 0a20 2020 204e  ipFixture,.    N
-00001390: 756d 6572 6963 5465 7374 2061 7320 5f4e  umericTest as _N
-000013a0: 756d 6572 6963 5465 7374 2c0a 2020 2020  umericTest,.    
-000013b0: 5374 7269 6e67 5465 7374 2061 7320 5f53  StringTest as _S
-000013c0: 7472 696e 6754 6573 742c 0a20 2020 2054  tringTest,.    T
-000013d0: 6578 7454 6573 7420 6173 205f 5465 7874  extTest as _Text
-000013e0: 5465 7374 2c0a 2020 2020 5469 6d65 5465  Test,.    TimeTe
-000013f0: 7374 2061 7320 5f54 696d 6554 6573 742c  st as _TimeTest,
-00001400: 0a20 2020 2054 696d 654d 6963 726f 7365  .    TimeMicrose
-00001410: 636f 6e64 7354 6573 7420 6173 205f 5469  condsTest as _Ti
-00001420: 6d65 4d69 6372 6f73 6563 6f6e 6473 5465  meMicrosecondsTe
-00001430: 7374 2c0a 2020 2020 5469 6d65 7374 616d  st,.    Timestam
-00001440: 704d 6963 726f 7365 636f 6e64 7354 6573  pMicrosecondsTes
-00001450: 742c 0a20 2020 2055 6e69 636f 6465 5661  t,.    UnicodeVa
-00001460: 7263 6861 7254 6573 7420 6173 205f 556e  rcharTest as _Un
-00001470: 6963 6f64 6556 6172 6368 6172 5465 7374  icodeVarcharTest
-00001480: 2c0a 2020 2020 556e 6963 6f64 6554 6578  ,.    UnicodeTex
-00001490: 7454 6573 7420 6173 205f 556e 6963 6f64  tTest as _Unicod
-000014a0: 6554 6578 7454 6573 742c 0a20 2020 205f  eTextTest,.    _
-000014b0: 556e 6963 6f64 6546 6978 7475 7265 2061  UnicodeFixture a
-000014c0: 7320 5f5f 556e 6963 6f64 6546 6978 7475  s __UnicodeFixtu
-000014d0: 7265 2c0a 290a 6672 6f6d 2074 6573 742e  re,.).from test.
-000014e0: 5f68 656c 7065 7273 2069 6d70 6f72 7420  _helpers import 
-000014f0: 6765 745f 6462 5f75 726c 2c20 6765 745f  get_db_url, get_
-00001500: 7072 6f6a 6563 740a 0a63 6f6e 6669 672e  project..config.
-00001510: 7465 7374 5f73 6368 656d 6120 3d20 2222  test_schema = ""
-00001520: 0a0a 0a63 6c61 7373 2042 6f6f 6c65 616e  ...class Boolean
-00001530: 5465 7374 285f 426f 6f6c 6561 6e54 6573  Test(_BooleanTes
-00001540: 7429 3a0a 2020 2020 4070 7974 6573 742e  t):.    @pytest.
-00001550: 6d61 726b 2e73 6b69 7028 0a20 2020 2020  mark.skip(.     
-00001560: 2020 2022 5468 6520 6f72 6967 696e 616c     "The original
-00001570: 2074 6573 7420 6361 7365 2077 6173 2073   test case was s
-00001580: 706c 6974 2069 6e74 6f20 3220 7061 7274  plit into 2 part
-00001590: 733a 2022 0a20 2020 2020 2020 2022 7465  s: ".        "te
-000015a0: 7374 5f72 656e 6465 725f 6c69 7465 7261  st_render_litera
-000015b0: 6c5f 626f 6f6c 5f74 7275 6520 616e 6420  l_bool_true and 
-000015c0: 7465 7374 5f72 656e 6465 725f 6c69 7465  test_render_lite
-000015d0: 7261 6c5f 626f 6f6c 5f66 616c 7365 220a  ral_bool_false".
-000015e0: 2020 2020 290a 2020 2020 6465 6620 7465      ).    def te
-000015f0: 7374 5f72 656e 6465 725f 6c69 7465 7261  st_render_litera
-00001600: 6c5f 626f 6f6c 2873 656c 6629 3a0a 2020  l_bool(self):.  
-00001610: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00001620: 6465 6620 7465 7374 5f72 656e 6465 725f  def test_render_
-00001630: 6c69 7465 7261 6c5f 626f 6f6c 5f74 7275  literal_bool_tru
-00001640: 6528 7365 6c66 2c20 6c69 7465 7261 6c5f  e(self, literal_
-00001650: 726f 756e 645f 7472 6970 293a 0a20 2020  round_trip):.   
-00001660: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00001670: 2053 5041 4e4e 4552 204f 5645 5252 4944   SPANNER OVERRID
-00001680: 453a 0a0a 2020 2020 2020 2020 436c 6f75  E:..        Clou
-00001690: 6420 5370 616e 6e65 7220 7375 7070 6f72  d Spanner suppor
-000016a0: 7473 2074 6162 6c65 7320 7769 7468 2061  ts tables with a
-000016b0: 6e20 656d 7074 7920 7072 696d 6172 7920  n empty primary 
-000016c0: 6b65 792c 2062 7574 0a20 2020 2020 2020  key, but.       
-000016d0: 206f 6e6c 7920 6120 7369 6e67 6c65 2072   only a single r
-000016e0: 6f77 2063 616e 2062 6520 696e 7365 7274  ow can be insert
-000016f0: 6564 2069 6e74 6f20 7375 6368 2061 2074  ed into such a t
-00001700: 6162 6c65 202d 0a20 2020 2020 2020 2066  able -.        f
-00001710: 6f6c 6c6f 7769 6e67 2069 6e73 6572 7469  ollowing inserti
-00001720: 6f6e 7320 7769 6c6c 2066 6169 6c20 7769  ons will fail wi
-00001730: 7468 2060 526f 7720 5b5d 2061 6c72 6561  th `Row [] alrea
-00001740: 6479 2065 7869 7374 7322 2e0a 2020 2020  dy exists"..    
-00001750: 2020 2020 4f76 6572 7269 6469 6e67 2074      Overriding t
-00001760: 6865 2074 6573 7420 746f 2061 766f 6964  he test to avoid
-00001770: 2074 6865 2073 616d 6520 6661 696c 7572   the same failur
-00001780: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00001790: 2020 2020 2020 206c 6974 6572 616c 5f72         literal_r
-000017a0: 6f75 6e64 5f74 7269 7028 426f 6f6c 6561  ound_trip(Boolea
-000017b0: 6e28 292c 205b 5472 7565 5d2c 205b 5472  n(), [True], [Tr
-000017c0: 7565 5d29 0a0a 2020 2020 6465 6620 7465  ue])..    def te
-000017d0: 7374 5f72 656e 6465 725f 6c69 7465 7261  st_render_litera
-000017e0: 6c5f 626f 6f6c 5f66 616c 7365 2873 656c  l_bool_false(sel
-000017f0: 662c 206c 6974 6572 616c 5f72 6f75 6e64  f, literal_round
-00001800: 5f74 7269 7029 3a0a 2020 2020 2020 2020  _trip):.        
-00001810: 2222 220a 2020 2020 2020 2020 5350 414e  """.        SPAN
-00001820: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
-00001830: 2020 2020 2020 2043 6c6f 7564 2053 7061         Cloud Spa
-00001840: 6e6e 6572 2073 7570 706f 7274 7320 7461  nner supports ta
-00001850: 626c 6573 2077 6974 6820 616e 2065 6d70  bles with an emp
-00001860: 7479 2070 7269 6d61 7279 206b 6579 2c20  ty primary key, 
-00001870: 6275 740a 2020 2020 2020 2020 6f6e 6c79  but.        only
-00001880: 2061 2073 696e 676c 6520 726f 7720 6361   a single row ca
-00001890: 6e20 6265 2069 6e73 6572 7465 6420 696e  n be inserted in
-000018a0: 746f 2073 7563 6820 6120 7461 626c 6520  to such a table 
-000018b0: 2d0a 2020 2020 2020 2020 666f 6c6c 6f77  -.        follow
-000018c0: 696e 6720 696e 7365 7274 696f 6e73 2077  ing insertions w
-000018d0: 696c 6c20 6661 696c 2077 6974 6820 6052  ill fail with `R
-000018e0: 6f77 205b 5d20 616c 7265 6164 7920 6578  ow [] already ex
-000018f0: 6973 7473 222e 0a20 2020 2020 2020 204f  ists"..        O
-00001900: 7665 7272 6964 696e 6720 7468 6520 7465  verriding the te
-00001910: 7374 2074 6f20 6176 6f69 6420 7468 6520  st to avoid the 
-00001920: 7361 6d65 2066 6169 6c75 7265 2e0a 2020  same failure..  
-00001930: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00001940: 2020 6c69 7465 7261 6c5f 726f 756e 645f    literal_round_
-00001950: 7472 6970 2842 6f6f 6c65 616e 2829 2c20  trip(Boolean(), 
-00001960: 5b46 616c 7365 5d2c 205b 4661 6c73 655d  [False], [False]
-00001970: 290a 0a20 2020 2040 7079 7465 7374 2e6d  )..    @pytest.m
-00001980: 6172 6b2e 736b 6970 2822 4e6f 7420 7375  ark.skip("Not su
-00001990: 7070 6f72 7465 6420 6279 2043 6c6f 7564  pported by Cloud
-000019a0: 2053 7061 6e6e 6572 2229 0a20 2020 2064   Spanner").    d
-000019b0: 6566 2074 6573 745f 7768 6572 6563 6c61  ef test_wherecla
-000019c0: 7573 6528 7365 6c66 293a 0a20 2020 2020  use(self):.     
-000019d0: 2020 2070 6173 730a 0a0a 636c 6173 7320     pass...class 
-000019e0: 436f 6d70 6f6e 656e 7452 6566 6c65 6374  ComponentReflect
-000019f0: 696f 6e54 6573 7445 7874 7261 285f 436f  ionTestExtra(_Co
-00001a00: 6d70 6f6e 656e 7452 6566 6c65 6374 696f  mponentReflectio
-00001a10: 6e54 6573 7445 7874 7261 293a 0a20 2020  nTestExtra):.   
-00001a20: 2040 7465 7374 696e 672e 7265 7175 6972   @testing.requir
-00001a30: 6573 2e74 6162 6c65 5f72 6566 6c65 6374  es.table_reflect
-00001a40: 696f 6e0a 2020 2020 6465 6620 7465 7374  ion.    def test
-00001a50: 5f6e 756c 6c61 626c 655f 7265 666c 6563  _nullable_reflec
-00001a60: 7469 6f6e 2873 656c 662c 2063 6f6e 6e65  tion(self, conne
-00001a70: 6374 696f 6e2c 206d 6574 6164 6174 6129  ction, metadata)
-00001a80: 3a0a 2020 2020 2020 2020 7420 3d20 5461  :.        t = Ta
-00001a90: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
-00001aa0: 2022 7422 2c0a 2020 2020 2020 2020 2020   "t",.          
-00001ab0: 2020 6d65 7461 6461 7461 2c0a 2020 2020    metadata,.    
-00001ac0: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-00001ad0: 6122 2c20 496e 7465 6765 722c 206e 756c  a", Integer, nul
-00001ae0: 6c61 626c 653d 5472 7565 292c 0a20 2020  lable=True),.   
-00001af0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00001b00: 2262 222c 2049 6e74 6567 6572 2c20 6e75  "b", Integer, nu
-00001b10: 6c6c 6162 6c65 3d46 616c 7365 292c 0a20  llable=False),. 
-00001b20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00001b30: 2074 2e63 7265 6174 6528 636f 6e6e 6563   t.create(connec
-00001b40: 7469 6f6e 290a 2020 2020 2020 2020 636f  tion).        co
-00001b50: 6e6e 6563 7469 6f6e 2e63 6f6e 6e65 6374  nnection.connect
-00001b60: 696f 6e2e 636f 6d6d 6974 2829 0a20 2020  ion.commit().   
-00001b70: 2020 2020 2065 715f 280a 2020 2020 2020       eq_(.      
-00001b80: 2020 2020 2020 6469 6374 280a 2020 2020        dict(.    
-00001b90: 2020 2020 2020 2020 2020 2020 2863 6f6c              (col
-00001ba0: 5b22 6e61 6d65 225d 2c20 636f 6c5b 226e  ["name"], col["n
-00001bb0: 756c 6c61 626c 6522 5d29 0a20 2020 2020  ullable"]).     
-00001bc0: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-00001bd0: 6f6c 2069 6e20 696e 7370 6563 7428 636f  ol in inspect(co
-00001be0: 6e6e 6563 7469 6f6e 292e 6765 745f 636f  nnection).get_co
-00001bf0: 6c75 6d6e 7328 2274 2229 0a20 2020 2020  lumns("t").     
-00001c00: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-00001c10: 2020 2020 2020 7b22 6122 3a20 5472 7565        {"a": True
-00001c20: 2c20 2262 223a 2046 616c 7365 7d2c 0a20  , "b": False},. 
-00001c30: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-00001c40: 6620 5f74 7970 655f 726f 756e 645f 7472  f _type_round_tr
-00001c50: 6970 2873 656c 662c 2063 6f6e 6e65 6374  ip(self, connect
-00001c60: 696f 6e2c 206d 6574 6164 6174 612c 202a  ion, metadata, *
-00001c70: 7479 7065 7329 3a0a 2020 2020 2020 2020  types):.        
-00001c80: 7420 3d20 5461 626c 6528 0a20 2020 2020  t = Table(.     
-00001c90: 2020 2020 2020 2022 7422 2c20 6d65 7461         "t", meta
-00001ca0: 6461 7461 2c20 2a5b 436f 6c75 6d6e 2822  data, *[Column("
-00001cb0: 7425 6422 2025 2069 2c20 7479 7065 5f29  t%d" % i, type_)
-00001cc0: 2066 6f72 2069 2c20 7479 7065 5f20 696e   for i, type_ in
-00001cd0: 2065 6e75 6d65 7261 7465 2874 7970 6573   enumerate(types
-00001ce0: 295d 0a20 2020 2020 2020 2029 0a20 2020  )].        ).   
-00001cf0: 2020 2020 2074 2e63 7265 6174 6528 636f       t.create(co
-00001d00: 6e6e 6563 7469 6f6e 290a 2020 2020 2020  nnection).      
-00001d10: 2020 636f 6e6e 6563 7469 6f6e 2e63 6f6e    connection.con
-00001d20: 6e65 6374 696f 6e2e 636f 6d6d 6974 2829  nection.commit()
-00001d30: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00001d40: 205b 635b 2274 7970 6522 5d20 666f 7220   [c["type"] for 
-00001d50: 6320 696e 2069 6e73 7065 6374 2863 6f6e  c in inspect(con
-00001d60: 6e65 6374 696f 6e29 2e67 6574 5f63 6f6c  nection).get_col
-00001d70: 756d 6e73 2822 7422 295d 0a0a 2020 2020  umns("t")]..    
-00001d80: 4074 6573 7469 6e67 2e72 6571 7569 7265  @testing.require
-00001d90: 732e 7461 626c 655f 7265 666c 6563 7469  s.table_reflecti
-00001da0: 6f6e 0a20 2020 2064 6566 2074 6573 745f  on.    def test_
-00001db0: 6e75 6d65 7269 635f 7265 666c 6563 7469  numeric_reflecti
-00001dc0: 6f6e 2873 656c 662c 2063 6f6e 6e65 6374  on(self, connect
-00001dd0: 696f 6e2c 206d 6574 6164 6174 6129 3a0a  ion, metadata):.
-00001de0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00001df0: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
-00001e00: 5249 4445 3a0a 0a20 2020 2020 2020 2053  RIDE:..        S
-00001e10: 7061 6e6e 6572 2064 6566 696e 6573 204e  panner defines N
-00001e20: 554d 4552 4943 2074 7970 6520 7769 7468  UMERIC type with
-00001e30: 2074 6865 2063 6f6e 7374 616e 7420 7072   the constant pr
-00001e40: 6563 6973 696f 6e3d 3338 0a20 2020 2020  ecision=38.     
-00001e50: 2020 2061 6e64 2073 6361 6c65 3d39 2e20     and scale=9. 
-00001e60: 4f76 6572 7269 6469 6e67 2074 6865 2074  Overriding the t
-00001e70: 6573 7420 746f 2063 6865 636b 2069 6620  est to check if 
-00001e80: 7468 6520 4e55 4d45 5249 430a 2020 2020  the NUMERIC.    
-00001e90: 2020 2020 636f 6c75 6d6e 2069 7320 7375      column is su
-00001ea0: 6363 6573 7366 756c 6c79 2063 7265 6174  ccessfully creat
-00001eb0: 6564 2061 6e64 2068 6173 2064 696d 656e  ed and has dimen
-00001ec0: 7369 6f6e 730a 2020 2020 2020 2020 636f  sions.        co
-00001ed0: 7272 6563 7420 666f 7220 436c 6f75 6420  rrect for Cloud 
-00001ee0: 5370 616e 6e65 722e 0a20 2020 2020 2020  Spanner..       
-00001ef0: 2022 2222 0a20 2020 2020 2020 2066 6f72   """.        for
-00001f00: 2074 7970 2069 6e20 7365 6c66 2e5f 7479   typ in self._ty
-00001f10: 7065 5f72 6f75 6e64 5f74 7269 7028 636f  pe_round_trip(co
-00001f20: 6e6e 6563 7469 6f6e 2c20 6d65 7461 6461  nnection, metada
-00001f30: 7461 2c20 4e75 6d65 7269 6328 3138 2c20  ta, Numeric(18, 
-00001f40: 3529 293a 0a20 2020 2020 2020 2020 2020  5)):.           
-00001f50: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
-00001f60: 6365 2874 7970 2c20 4e75 6d65 7269 6329  ce(typ, Numeric)
-00001f70: 0a20 2020 2020 2020 2020 2020 2065 715f  .            eq_
-00001f80: 2874 7970 2e70 7265 6369 7369 6f6e 2c20  (typ.precision, 
-00001f90: 3338 290a 2020 2020 2020 2020 2020 2020  38).            
-00001fa0: 6571 5f28 7479 702e 7363 616c 652c 2039  eq_(typ.scale, 9
-00001fb0: 290a 0a20 2020 2040 7465 7374 696e 672e  )..    @testing.
-00001fc0: 7265 7175 6972 6573 2e74 6162 6c65 5f72  requires.table_r
-00001fd0: 6566 6c65 6374 696f 6e0a 2020 2020 6465  eflection.    de
-00001fe0: 6620 7465 7374 5f62 696e 6172 795f 7265  f test_binary_re
-00001ff0: 666c 6563 7469 6f6e 2873 656c 662c 2063  flection(self, c
-00002000: 6f6e 6e65 6374 696f 6e2c 206d 6574 6164  onnection, metad
-00002010: 6174 6129 3a0a 2020 2020 2020 2020 2222  ata):.        ""
-00002020: 220a 2020 2020 2020 2020 4368 6563 6b20  ".        Check 
-00002030: 7468 6174 2061 2042 5954 4553 2063 6f6c  that a BYTES col
-00002040: 756d 6e20 7769 7468 2061 6e20 6578 706c  umn with an expl
-00002050: 6963 6974 6c79 0a20 2020 2020 2020 2073  icitly.        s
-00002060: 6574 2073 697a 6520 6973 2063 6f72 7265  et size is corre
-00002070: 6374 6c79 2072 6566 6c65 6374 6564 2e0a  ctly reflected..
-00002080: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00002090: 2020 2020 666f 7220 7479 7020 696e 2073      for typ in s
-000020a0: 656c 662e 5f74 7970 655f 726f 756e 645f  elf._type_round_
-000020b0: 7472 6970 2863 6f6e 6e65 6374 696f 6e2c  trip(connection,
-000020c0: 206d 6574 6164 6174 612c 204c 6172 6765   metadata, Large
-000020d0: 4269 6e61 7279 2832 3029 293a 0a20 2020  Binary(20)):.   
-000020e0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-000020f0: 6973 696e 7374 616e 6365 2874 7970 2c20  isinstance(typ, 
-00002100: 4c61 7267 6542 696e 6172 7929 0a20 2020  LargeBinary).   
-00002110: 2020 2020 2020 2020 2065 715f 2874 7970           eq_(typ
-00002120: 2e6c 656e 6774 682c 2032 3029 0a0a 0a63  .length, 20)...c
-00002130: 6c61 7373 2043 6f6d 706f 6e65 6e74 5265  lass ComponentRe
-00002140: 666c 6563 7469 6f6e 5465 7374 285f 436f  flectionTest(_Co
-00002150: 6d70 6f6e 656e 7452 6566 6c65 6374 696f  mponentReflectio
-00002160: 6e54 6573 7429 3a0a 2020 2020 4063 6c61  nTest):.    @cla
-00002170: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-00002180: 2064 6566 696e 655f 7461 626c 6573 2863   define_tables(c
-00002190: 6c73 2c20 6d65 7461 6461 7461 293a 0a20  ls, metadata):. 
-000021a0: 2020 2020 2020 2063 6c73 2e64 6566 696e         cls.defin
-000021b0: 655f 7265 666c 6563 7465 645f 7461 626c  e_reflected_tabl
-000021c0: 6573 286d 6574 6164 6174 612c 204e 6f6e  es(metadata, Non
-000021d0: 6529 0a0a 2020 2020 4063 6c61 7373 6d65  e)..    @classme
-000021e0: 7468 6f64 0a20 2020 2064 6566 2064 6566  thod.    def def
-000021f0: 696e 655f 7265 666c 6563 7465 645f 7461  ine_reflected_ta
-00002200: 626c 6573 2863 6c73 2c20 6d65 7461 6461  bles(cls, metada
-00002210: 7461 2c20 7363 6865 6d61 293a 0a20 2020  ta, schema):.   
-00002220: 2020 2020 2069 6620 7363 6865 6d61 3a0a       if schema:.
-00002230: 2020 2020 2020 2020 2020 2020 7363 6865              sche
-00002240: 6d61 5f70 7265 6669 7820 3d20 7363 6865  ma_prefix = sche
-00002250: 6d61 202b 2022 2e22 0a20 2020 2020 2020  ma + ".".       
-00002260: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00002270: 2020 2073 6368 656d 615f 7072 6566 6978     schema_prefix
-00002280: 203d 2022 220a 0a20 2020 2020 2020 2069   = ""..        i
-00002290: 6620 7465 7374 696e 672e 7265 7175 6972  f testing.requir
-000022a0: 6573 2e73 656c 665f 7265 6665 7265 6e74  es.self_referent
-000022b0: 6961 6c5f 666f 7265 6967 6e5f 6b65 7973  ial_foreign_keys
-000022c0: 2e65 6e61 626c 6564 3a0a 2020 2020 2020  .enabled:.      
-000022d0: 2020 2020 2020 7573 6572 7320 3d20 5461        users = Ta
-000022e0: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
-000022f0: 2020 2020 2022 7573 6572 7322 2c0a 2020       "users",.  
-00002300: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00002310: 7461 6461 7461 2c0a 2020 2020 2020 2020  tadata,.        
-00002320: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-00002330: 7573 6572 5f69 6422 2c20 7371 6c61 6c63  user_id", sqlalc
-00002340: 6865 6d79 2e49 4e54 2c20 7072 696d 6172  hemy.INT, primar
-00002350: 795f 6b65 793d 5472 7565 292c 0a20 2020  y_key=True),.   
-00002360: 2020 2020 2020 2020 2020 2020 2043 6f6c               Col
-00002370: 756d 6e28 2274 6573 7431 222c 2073 716c  umn("test1", sql
-00002380: 616c 6368 656d 792e 4348 4152 2835 292c  alchemy.CHAR(5),
-00002390: 206e 756c 6c61 626c 653d 4661 6c73 6529   nullable=False)
-000023a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000023b0: 2020 436f 6c75 6d6e 2822 7465 7374 3222    Column("test2"
-000023c0: 2c20 7371 6c61 6c63 6865 6d79 2e46 6c6f  , sqlalchemy.Flo
-000023d0: 6174 2835 292c 206e 756c 6c61 626c 653d  at(5), nullable=
-000023e0: 4661 6c73 6529 2c0a 2020 2020 2020 2020  False),.        
-000023f0: 2020 2020 2020 2020 436f 6c75 6d6e 280a          Column(.
-00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002410: 2020 2020 2270 6172 656e 745f 7573 6572      "parent_user
-00002420: 5f69 6422 2c0a 2020 2020 2020 2020 2020  _id",.          
-00002430: 2020 2020 2020 2020 2020 7371 6c61 6c63            sqlalc
-00002440: 6865 6d79 2e49 6e74 6567 6572 2c0a 2020  hemy.Integer,.  
-00002450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002460: 2020 7371 6c61 6c63 6865 6d79 2e46 6f72    sqlalchemy.For
-00002470: 6569 676e 4b65 7928 0a20 2020 2020 2020  eignKey(.       
-00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002490: 2022 2573 7573 6572 732e 7573 6572 5f69   "%susers.user_i
-000024a0: 6422 2025 2073 6368 656d 615f 7072 6566  d" % schema_pref
-000024b0: 6978 2c20 6e61 6d65 3d22 7573 6572 5f69  ix, name="user_i
-000024c0: 645f 666b 220a 2020 2020 2020 2020 2020  d_fk".          
-000024d0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-000024e0: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
-000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002500: 7363 6865 6d61 3d73 6368 656d 612c 0a20  schema=schema,. 
-00002510: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00002520: 6573 745f 6e65 6564 735f 666b 3d54 7275  est_needs_fk=Tru
-00002530: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
-00002540: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00002550: 2020 2020 2020 2020 2020 2075 7365 7273             users
-00002560: 203d 2054 6162 6c65 280a 2020 2020 2020   = Table(.      
-00002570: 2020 2020 2020 2020 2020 2275 7365 7273            "users
-00002580: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002590: 2020 206d 6574 6164 6174 612c 0a20 2020     metadata,.   
-000025a0: 2020 2020 2020 2020 2020 2020 2043 6f6c               Col
-000025b0: 756d 6e28 2275 7365 725f 6964 222c 2073  umn("user_id", s
-000025c0: 716c 616c 6368 656d 792e 494e 542c 2070  qlalchemy.INT, p
-000025d0: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
-000025e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000025f0: 2020 436f 6c75 6d6e 2822 7465 7374 3122    Column("test1"
-00002600: 2c20 7371 6c61 6c63 6865 6d79 2e43 4841  , sqlalchemy.CHA
-00002610: 5228 3529 2c20 6e75 6c6c 6162 6c65 3d46  R(5), nullable=F
-00002620: 616c 7365 292c 0a20 2020 2020 2020 2020  alse),.         
-00002630: 2020 2020 2020 2043 6f6c 756d 6e28 2274         Column("t
-00002640: 6573 7432 222c 2073 716c 616c 6368 656d  est2", sqlalchem
-00002650: 792e 466c 6f61 7428 3529 2c20 6e75 6c6c  y.Float(5), null
-00002660: 6162 6c65 3d46 616c 7365 292c 0a20 2020  able=False),.   
-00002670: 2020 2020 2020 2020 2020 2020 2073 6368               sch
-00002680: 656d 613d 7363 6865 6d61 2c0a 2020 2020  ema=schema,.    
-00002690: 2020 2020 2020 2020 2020 2020 7465 7374              test
-000026a0: 5f6e 6565 6473 5f66 6b3d 5472 7565 2c0a  _needs_fk=True,.
-000026b0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-000026c0: 2020 2020 2020 2054 6162 6c65 280a 2020         Table(.  
-000026d0: 2020 2020 2020 2020 2020 2264 696e 6761            "dinga
-000026e0: 6c69 6e67 7322 2c0a 2020 2020 2020 2020  lings",.        
-000026f0: 2020 2020 6d65 7461 6461 7461 2c0a 2020      metadata,.  
-00002700: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-00002710: 2822 6469 6e67 616c 696e 675f 6964 222c  ("dingaling_id",
-00002720: 2073 716c 616c 6368 656d 792e 496e 7465   sqlalchemy.Inte
-00002730: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
-00002740: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
-00002750: 2020 2020 436f 6c75 6d6e 280a 2020 2020      Column(.    
-00002760: 2020 2020 2020 2020 2020 2020 2261 6464              "add
-00002770: 7265 7373 5f69 6422 2c0a 2020 2020 2020  ress_id",.      
-00002780: 2020 2020 2020 2020 2020 7371 6c61 6c63            sqlalc
-00002790: 6865 6d79 2e49 6e74 6567 6572 2c0a 2020  hemy.Integer,.  
-000027a0: 2020 2020 2020 2020 2020 2020 2020 7371                sq
-000027b0: 6c61 6c63 6865 6d79 2e46 6f72 6569 676e  lalchemy.Foreign
-000027c0: 4b65 7928 2225 7365 6d61 696c 5f61 6464  Key("%semail_add
-000027d0: 7265 7373 6573 2e61 6464 7265 7373 5f69  resses.address_i
-000027e0: 6422 2025 2073 6368 656d 615f 7072 6566  d" % schema_pref
-000027f0: 6978 292c 0a20 2020 2020 2020 2020 2020  ix),.           
-00002800: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00002810: 436f 6c75 6d6e 2822 6461 7461 222c 2073  Column("data", s
-00002820: 716c 616c 6368 656d 792e 5374 7269 6e67  qlalchemy.String
-00002830: 2833 3029 292c 0a20 2020 2020 2020 2020  (30)),.         
-00002840: 2020 2073 6368 656d 613d 7363 6865 6d61     schema=schema
-00002850: 2c0a 2020 2020 2020 2020 2020 2020 7465  ,.            te
-00002860: 7374 5f6e 6565 6473 5f66 6b3d 5472 7565  st_needs_fk=True
-00002870: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00002880: 2020 2020 5461 626c 6528 0a20 2020 2020      Table(.     
-00002890: 2020 2020 2020 2022 656d 6169 6c5f 6164         "email_ad
-000028a0: 6472 6573 7365 7322 2c0a 2020 2020 2020  dresses",.      
-000028b0: 2020 2020 2020 6d65 7461 6461 7461 2c0a        metadata,.
-000028c0: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
-000028d0: 6d6e 2822 6164 6472 6573 735f 6964 222c  mn("address_id",
-000028e0: 2073 716c 616c 6368 656d 792e 496e 7465   sqlalchemy.Inte
-000028f0: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
-00002900: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
-00002910: 2020 2020 436f 6c75 6d6e 280a 2020 2020      Column(.    
-00002920: 2020 2020 2020 2020 2020 2020 2272 656d              "rem
-00002930: 6f74 655f 7573 6572 5f69 6422 2c0a 2020  ote_user_id",.  
-00002940: 2020 2020 2020 2020 2020 2020 2020 7371                sq
-00002950: 6c61 6c63 6865 6d79 2e49 6e74 6567 6572  lalchemy.Integer
-00002960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002970: 2020 7371 6c61 6c63 6865 6d79 2e46 6f72    sqlalchemy.For
-00002980: 6569 676e 4b65 7928 7573 6572 732e 632e  eignKey(users.c.
-00002990: 7573 6572 5f69 6429 2c0a 2020 2020 2020  user_id),.      
-000029a0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-000029b0: 2020 2020 2043 6f6c 756d 6e28 2265 6d61       Column("ema
-000029c0: 696c 5f61 6464 7265 7373 222c 2073 716c  il_address", sql
-000029d0: 616c 6368 656d 792e 5374 7269 6e67 2832  alchemy.String(2
-000029e0: 3029 292c 0a20 2020 2020 2020 2020 2020  0)),.           
-000029f0: 2073 716c 616c 6368 656d 792e 5072 696d   sqlalchemy.Prim
-00002a00: 6172 794b 6579 436f 6e73 7472 6169 6e74  aryKeyConstraint
-00002a10: 2822 6164 6472 6573 735f 6964 222c 206e  ("address_id", n
-00002a20: 616d 653d 2265 6d61 696c 5f61 645f 706b  ame="email_ad_pk
-00002a30: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-00002a40: 7363 6865 6d61 3d73 6368 656d 612c 0a20  schema=schema,. 
-00002a50: 2020 2020 2020 2020 2020 2074 6573 745f             test_
-00002a60: 6e65 6564 735f 666b 3d54 7275 652c 0a20  needs_fk=True,. 
-00002a70: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00002a80: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
-00002a90: 2020 2020 2263 6f6d 6d65 6e74 5f74 6573      "comment_tes
-00002aa0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00002ab0: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
-00002ac0: 2020 2020 2020 436f 6c75 6d6e 2822 6964        Column("id
-00002ad0: 222c 2073 716c 616c 6368 656d 792e 496e  ", sqlalchemy.In
-00002ae0: 7465 6765 722c 2070 7269 6d61 7279 5f6b  teger, primary_k
-00002af0: 6579 3d54 7275 652c 2063 6f6d 6d65 6e74  ey=True, comment
-00002b00: 3d22 6964 2063 6f6d 6d65 6e74 2229 2c0a  ="id comment"),.
-00002b10: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
-00002b20: 6d6e 2822 6461 7461 222c 2073 716c 616c  mn("data", sqlal
-00002b30: 6368 656d 792e 5374 7269 6e67 2832 3029  chemy.String(20)
-00002b40: 2c20 636f 6d6d 656e 743d 2264 6174 6120  , comment="data 
-00002b50: 2520 636f 6d6d 656e 7422 292c 0a20 2020  % comment"),.   
-00002b60: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00002b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002b80: 2022 6432 222c 0a20 2020 2020 2020 2020   "d2",.         
-00002b90: 2020 2020 2020 2073 716c 616c 6368 656d         sqlalchem
-00002ba0: 792e 5374 7269 6e67 2832 3029 2c0a 2020  y.String(20),.  
-00002bb0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00002bc0: 6d6d 656e 743d 7222 2222 436f 6d6d 656e  mment=r"""Commen
-00002bd0: 7420 7479 7065 7320 7479 7065 2073 7065  t types type spe
-00002be0: 6564 696c 7920 2720 2220 5c20 2727 2046  edily ' " \ '' F
-00002bf0: 756e 2122 2222 2c0a 2020 2020 2020 2020  un!""",.        
-00002c00: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-00002c10: 2020 2073 6368 656d 613d 7363 6865 6d61     schema=schema
-00002c20: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
-00002c30: 6d6d 656e 743d 7222 2222 7468 6520 7465  mment=r"""the te
-00002c40: 7374 2025 2027 2022 205c 2074 6162 6c65  st % ' " \ table
-00002c50: 2063 6f6d 6d65 6e74 2222 222c 0a20 2020   comment""",.   
-00002c60: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00002c70: 6966 2074 6573 7469 6e67 2e72 6571 7569  if testing.requi
-00002c80: 7265 732e 6372 6f73 735f 7363 6865 6d61  res.cross_schema
-00002c90: 5f66 6b5f 7265 666c 6563 7469 6f6e 2e65  _fk_reflection.e
-00002ca0: 6e61 626c 6564 3a0a 2020 2020 2020 2020  nabled:.        
-00002cb0: 2020 2020 6966 2073 6368 656d 6120 6973      if schema is
-00002cc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00002cd0: 2020 2020 2020 2054 6162 6c65 280a 2020         Table(.  
-00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cf0: 2020 226c 6f63 616c 5f74 6162 6c65 222c    "local_table",
-00002d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002d10: 2020 2020 206d 6574 6164 6174 612c 0a20       metadata,. 
-00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d30: 2020 2043 6f6c 756d 6e28 2269 6422 2c20     Column("id", 
-00002d40: 7371 6c61 6c63 6865 6d79 2e49 6e74 6567  sqlalchemy.Integ
-00002d50: 6572 2c20 7072 696d 6172 795f 6b65 793d  er, primary_key=
-00002d60: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-00002d70: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
-00002d80: 6e28 2264 6174 6122 2c20 7371 6c61 6c63  n("data", sqlalc
-00002d90: 6865 6d79 2e53 7472 696e 6728 3230 2929  hemy.String(20))
-00002da0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002db0: 2020 2020 2020 436f 6c75 6d6e 280a 2020        Column(.  
-00002dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dd0: 2020 2020 2020 2272 656d 6f74 655f 6964        "remote_id
-00002de0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002df0: 2020 2020 2020 2020 2020 2046 6f72 6569             Forei
-00002e00: 676e 4b65 7928 2225 732e 7265 6d6f 7465  gnKey("%s.remote
-00002e10: 5f74 6162 6c65 5f32 2e69 6422 2025 2074  _table_2.id" % t
-00002e20: 6573 7469 6e67 2e63 6f6e 6669 672e 7465  esting.config.te
-00002e30: 7374 5f73 6368 656d 6129 2c0a 2020 2020  st_schema),.    
-00002e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e50: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00002e60: 2020 2020 2020 2074 6573 745f 6e65 6564         test_need
-00002e70: 735f 666b 3d54 7275 652c 0a20 2020 2020  s_fk=True,.     
-00002e80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002e90: 6368 656d 613d 636f 6e66 6967 2e64 622e  chema=config.db.
-00002ea0: 6469 616c 6563 742e 6465 6661 756c 745f  dialect.default_
-00002eb0: 7363 6865 6d61 5f6e 616d 652c 0a20 2020  schema_name,.   
-00002ec0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00002ed0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00002ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ef0: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
-00002f00: 2020 2020 2020 2020 2020 2020 2272 656d              "rem
-00002f10: 6f74 655f 7461 626c 6522 2c0a 2020 2020  ote_table",.    
-00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f30: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
-00002f40: 2020 2020 2020 2020 2020 2020 2020 436f                Co
-00002f50: 6c75 6d6e 2822 6964 222c 2073 716c 616c  lumn("id", sqlal
-00002f60: 6368 656d 792e 496e 7465 6765 722c 2070  chemy.Integer, p
-00002f70: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
-00002f80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002f90: 2020 2020 2020 436f 6c75 6d6e 280a 2020        Column(.  
-00002fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fb0: 2020 2020 2020 226c 6f63 616c 5f69 6422        "local_id"
-00002fc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002fd0: 2020 2020 2020 2020 2020 466f 7265 6967            Foreig
-00002fe0: 6e4b 6579 280a 2020 2020 2020 2020 2020  nKey(.          
-00002ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003000: 2020 2225 732e 6c6f 6361 6c5f 7461 626c    "%s.local_tabl
-00003010: 652e 6964 2220 2520 636f 6e66 6967 2e64  e.id" % config.d
-00003020: 622e 6469 616c 6563 742e 6465 6661 756c  b.dialect.defaul
-00003030: 745f 7363 6865 6d61 5f6e 616d 650a 2020  t_schema_name.  
-00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003050: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-00003060: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
-00003070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003080: 2020 2020 436f 6c75 6d6e 2822 6461 7461      Column("data
-00003090: 222c 2073 716c 616c 6368 656d 792e 5374  ", sqlalchemy.St
-000030a0: 7269 6e67 2832 3029 292c 0a20 2020 2020  ring(20)),.     
-000030b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000030c0: 6368 656d 613d 7363 6865 6d61 2c0a 2020  chema=schema,.  
-000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030e0: 2020 7465 7374 5f6e 6565 6473 5f66 6b3d    test_needs_fk=
-000030f0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00003100: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00003110: 2020 2020 2020 2020 5461 626c 6528 0a20          Table(. 
-00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003130: 2020 2022 7265 6d6f 7465 5f74 6162 6c65     "remote_table
-00003140: 5f32 222c 0a20 2020 2020 2020 2020 2020  _2",.           
-00003150: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
-00003160: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-00003170: 2020 2020 2020 2043 6f6c 756d 6e28 2269         Column("i
-00003180: 6422 2c20 7371 6c61 6c63 6865 6d79 2e49  d", sqlalchemy.I
-00003190: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
-000031a0: 6b65 793d 5472 7565 292c 0a20 2020 2020  key=True),.     
-000031b0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
-000031c0: 6f6c 756d 6e28 2264 6174 6122 2c20 7371  olumn("data", sq
-000031d0: 6c61 6c63 6865 6d79 2e53 7472 696e 6728  lalchemy.String(
-000031e0: 3230 2929 2c0a 2020 2020 2020 2020 2020  20)),.          
-000031f0: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
-00003200: 3d73 6368 656d 612c 0a20 2020 2020 2020  =schema,.       
-00003210: 2020 2020 2020 2020 2020 2020 2074 6573               tes
-00003220: 745f 6e65 6564 735f 666b 3d54 7275 652c  t_needs_fk=True,
-00003230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003240: 2029 0a0a 2020 2020 2020 2020 6966 2074   )..        if t
-00003250: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
-00003260: 696e 6465 785f 7265 666c 6563 7469 6f6e  index_reflection
-00003270: 2e65 6e61 626c 6564 3a0a 2020 2020 2020  .enabled:.      
-00003280: 2020 2020 2020 636c 732e 6465 6669 6e65        cls.define
-00003290: 5f69 6e64 6578 286d 6574 6164 6174 612c  _index(metadata,
-000032a0: 2075 7365 7273 290a 0a20 2020 2020 2020   users)..       
-000032b0: 2020 2020 2069 6620 6e6f 7420 7363 6865       if not sche
-000032c0: 6d61 3a0a 2020 2020 2020 2020 2020 2020  ma:.            
-000032d0: 2020 2020 2320 7465 7374 5f6e 6565 6473      # test_needs
-000032e0: 5f66 6b20 6973 2061 7420 7468 6520 6d6f  _fk is at the mo
-000032f0: 6d65 6e74 2074 6f20 666f 7263 6520 4d79  ment to force My
-00003300: 5351 4c20 496e 6e6f 4442 0a20 2020 2020  SQL InnoDB.     
-00003310: 2020 2020 2020 2020 2020 206e 6f6e 636f             nonco
-00003320: 6c5f 6964 785f 7465 7374 5f6e 6f70 6b20  l_idx_test_nopk 
-00003330: 3d20 5461 626c 6528 0a20 2020 2020 2020  = Table(.       
-00003340: 2020 2020 2020 2020 2020 2020 2022 6e6f               "no
-00003350: 6e63 6f6c 5f69 6478 5f74 6573 745f 6e6f  ncol_idx_test_no
-00003360: 706b 222c 0a20 2020 2020 2020 2020 2020  pk",.           
-00003370: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
-00003380: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-00003390: 2020 2020 2020 2043 6f6c 756d 6e28 2269         Column("i
-000033a0: 6422 2c20 7371 6c61 6c63 6865 6d79 2e49  d", sqlalchemy.I
-000033b0: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
-000033c0: 6b65 793d 5472 7565 292c 0a20 2020 2020  key=True),.     
-000033d0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
-000033e0: 6f6c 756d 6e28 2271 222c 2073 716c 616c  olumn("q", sqlal
-000033f0: 6368 656d 792e 5374 7269 6e67 2835 2929  chemy.String(5))
-00003400: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003410: 2020 2020 2020 7465 7374 5f6e 6565 6473        test_needs
-00003420: 5f66 6b3d 5472 7565 2c0a 2020 2020 2020  _fk=True,.      
-00003430: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00003440: 7465 6e64 5f65 7869 7374 696e 673d 5472  tend_existing=Tr
-00003450: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00003460: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-00003470: 2020 2020 2020 206e 6f6e 636f 6c5f 6964         noncol_id
-00003480: 785f 7465 7374 5f70 6b20 3d20 5461 626c  x_test_pk = Tabl
-00003490: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-000034a0: 2020 2020 2020 2022 6e6f 6e63 6f6c 5f69         "noncol_i
-000034b0: 6478 5f74 6573 745f 706b 222c 0a20 2020  dx_test_pk",.   
-000034c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034d0: 206d 6574 6164 6174 612c 0a20 2020 2020   metadata,.     
-000034e0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
-000034f0: 6f6c 756d 6e28 2269 6422 2c20 7371 6c61  olumn("id", sqla
-00003500: 6c63 6865 6d79 2e49 6e74 6567 6572 2c20  lchemy.Integer, 
-00003510: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
-00003520: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00003530: 2020 2020 2020 2043 6f6c 756d 6e28 2271         Column("q
-00003540: 222c 2073 716c 616c 6368 656d 792e 5374  ", sqlalchemy.St
-00003550: 7269 6e67 2835 2929 2c0a 2020 2020 2020  ring(5)),.      
-00003560: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00003570: 7374 5f6e 6565 6473 5f66 6b3d 5472 7565  st_needs_fk=True
-00003580: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003590: 2020 2020 2020 6578 7465 6e64 5f65 7869        extend_exi
-000035a0: 7374 696e 673d 5472 7565 2c0a 2020 2020  sting=True,.    
-000035b0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-000035c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000035d0: 6620 7465 7374 696e 672e 7265 7175 6972  f testing.requir
-000035e0: 6573 2e69 6e64 6578 6573 5f77 6974 685f  es.indexes_with_
-000035f0: 6173 6364 6573 632e 656e 6162 6c65 643a  ascdesc.enabled:
-00003600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003610: 2020 2020 2073 716c 616c 6368 656d 792e       sqlalchemy.
-00003620: 496e 6465 7828 226e 6f6e 636f 6c5f 6964  Index("noncol_id
-00003630: 785f 6e6f 706b 222c 206e 6f6e 636f 6c5f  x_nopk", noncol_
-00003640: 6964 785f 7465 7374 5f6e 6f70 6b2e 632e  idx_test_nopk.c.
-00003650: 712e 6465 7363 2829 290a 2020 2020 2020  q.desc()).      
-00003660: 2020 2020 2020 2020 2020 2020 2020 7371                sq
-00003670: 6c61 6c63 6865 6d79 2e49 6e64 6578 2822  lalchemy.Index("
-00003680: 6e6f 6e63 6f6c 5f69 6478 5f70 6b22 2c20  noncol_idx_pk", 
-00003690: 6e6f 6e63 6f6c 5f69 6478 5f74 6573 745f  noncol_idx_test_
-000036a0: 706b 2e63 2e71 2e64 6573 6328 2929 0a0a  pk.c.q.desc())..
-000036b0: 2020 2020 2020 2020 6966 2074 6573 7469          if testi
-000036c0: 6e67 2e72 6571 7569 7265 732e 7669 6577  ng.requires.view
-000036d0: 5f63 6f6c 756d 6e5f 7265 666c 6563 7469  _column_reflecti
-000036e0: 6f6e 2e65 6e61 626c 6564 3a0a 2020 2020  on.enabled:.    
-000036f0: 2020 2020 2020 2020 636c 732e 6465 6669          cls.defi
-00003700: 6e65 5f76 6965 7773 286d 6574 6164 6174  ne_views(metadat
-00003710: 612c 2073 6368 656d 6129 0a0a 2020 2020  a, schema)..    
-00003720: 4074 6573 7469 6e67 2e63 6f6d 6269 6e61  @testing.combina
-00003730: 7469 6f6e 7328 2846 616c 7365 2c29 2c20  tions((False,), 
-00003740: 6172 676e 616d 6573 3d22 7573 655f 7363  argnames="use_sc
-00003750: 6865 6d61 2229 0a20 2020 2040 7465 7374  hema").    @test
-00003760: 696e 672e 7265 7175 6972 6573 2e66 6f72  ing.requires.for
-00003770: 6569 676e 5f6b 6579 5f63 6f6e 7374 7261  eign_key_constra
-00003780: 696e 745f 7265 666c 6563 7469 6f6e 0a20  int_reflection. 
-00003790: 2020 2064 6566 2074 6573 745f 6765 745f     def test_get_
-000037a0: 666f 7265 6967 6e5f 6b65 7973 2873 656c  foreign_keys(sel
-000037b0: 662c 2063 6f6e 6e65 6374 696f 6e2c 2075  f, connection, u
-000037c0: 7365 5f73 6368 656d 6129 3a0a 2020 2020  se_schema):.    
-000037d0: 2020 2020 6966 2075 7365 5f73 6368 656d      if use_schem
-000037e0: 613a 0a20 2020 2020 2020 2020 2020 2073  a:.            s
-000037f0: 6368 656d 6120 3d20 636f 6e66 6967 2e74  chema = config.t
-00003800: 6573 745f 7363 6865 6d61 0a20 2020 2020  est_schema.     
-00003810: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00003820: 2020 2020 2073 6368 656d 6120 3d20 4e6f       schema = No
-00003830: 6e65 0a0a 2020 2020 2020 2020 7573 6572  ne..        user
-00003840: 732c 2061 6464 7265 7373 6573 203d 2028  s, addresses = (
-00003850: 7365 6c66 2e74 6162 6c65 732e 7573 6572  self.tables.user
-00003860: 732c 2073 656c 662e 7461 626c 6573 2e65  s, self.tables.e
-00003870: 6d61 696c 5f61 6464 7265 7373 6573 290a  mail_addresses).
-00003880: 2020 2020 2020 2020 696e 7370 203d 2069          insp = i
-00003890: 6e73 7065 6374 2863 6f6e 6e65 6374 696f  nspect(connectio
-000038a0: 6e29 0a20 2020 2020 2020 2065 7870 6563  n).        expec
-000038b0: 7465 645f 7363 6865 6d61 203d 2073 6368  ted_schema = sch
-000038c0: 656d 610a 2020 2020 2020 2020 2320 7573  ema.        # us
-000038d0: 6572 730a 0a20 2020 2020 2020 2069 6620  ers..        if 
-000038e0: 7465 7374 696e 672e 7265 7175 6972 6573  testing.requires
-000038f0: 2e73 656c 665f 7265 6665 7265 6e74 6961  .self_referentia
-00003900: 6c5f 666f 7265 6967 6e5f 6b65 7973 2e65  l_foreign_keys.e
-00003910: 6e61 626c 6564 3a0a 2020 2020 2020 2020  nabled:.        
-00003920: 2020 2020 7573 6572 735f 666b 6579 7320      users_fkeys 
-00003930: 3d20 696e 7370 2e67 6574 5f66 6f72 6569  = insp.get_forei
-00003940: 676e 5f6b 6579 7328 7573 6572 732e 6e61  gn_keys(users.na
-00003950: 6d65 2c20 7363 6865 6d61 3d73 6368 656d  me, schema=schem
-00003960: 6129 0a20 2020 2020 2020 2020 2020 2066  a).            f
-00003970: 6b65 7931 203d 2075 7365 7273 5f66 6b65  key1 = users_fke
-00003980: 7973 5b30 5d0a 0a20 2020 2020 2020 2020  ys[0]..         
-00003990: 2020 2077 6974 6820 7465 7374 696e 672e     with testing.
-000039a0: 7265 7175 6972 6573 2e6e 616d 6564 5f63  requires.named_c
-000039b0: 6f6e 7374 7261 696e 7473 2e66 6169 6c5f  onstraints.fail_
-000039c0: 6966 2829 3a0a 2020 2020 2020 2020 2020  if():.          
-000039d0: 2020 2020 2020 6571 5f28 666b 6579 315b        eq_(fkey1[
-000039e0: 226e 616d 6522 5d2c 2022 7573 6572 5f69  "name"], "user_i
-000039f0: 645f 666b 2229 0a0a 2020 2020 2020 2020  d_fk")..        
-00003a00: 2020 2020 6571 5f28 666b 6579 315b 2272      eq_(fkey1["r
-00003a10: 6566 6572 7265 645f 7363 6865 6d61 225d  eferred_schema"]
-00003a20: 2c20 6578 7065 6374 6564 5f73 6368 656d  , expected_schem
-00003a30: 6129 0a20 2020 2020 2020 2020 2020 2065  a).            e
-00003a40: 715f 2866 6b65 7931 5b22 7265 6665 7272  q_(fkey1["referr
-00003a50: 6564 5f74 6162 6c65 225d 2c20 7573 6572  ed_table"], user
-00003a60: 732e 6e61 6d65 290a 2020 2020 2020 2020  s.name).        
-00003a70: 2020 2020 6571 5f28 666b 6579 315b 2272      eq_(fkey1["r
-00003a80: 6566 6572 7265 645f 636f 6c75 6d6e 7322  eferred_columns"
-00003a90: 5d2c 205b 2275 7365 725f 6964 225d 290a  ], ["user_id"]).
-00003aa0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00003ab0: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
-00003ac0: 7365 6c66 5f72 6566 6572 656e 7469 616c  self_referential
-00003ad0: 5f66 6f72 6569 676e 5f6b 6579 732e 656e  _foreign_keys.en
-00003ae0: 6162 6c65 643a 0a20 2020 2020 2020 2020  abled:.         
-00003af0: 2020 2020 2020 2065 715f 2866 6b65 7931         eq_(fkey1
-00003b00: 5b22 636f 6e73 7472 6169 6e65 645f 636f  ["constrained_co
-00003b10: 6c75 6d6e 7322 5d2c 205b 2270 6172 656e  lumns"], ["paren
-00003b20: 745f 7573 6572 5f69 6422 5d29 0a0a 2020  t_user_id"])..  
-00003b30: 2020 2020 2020 2320 6164 6472 6573 7365        # addresse
-00003b40: 730a 2020 2020 2020 2020 6164 6472 5f66  s.        addr_f
-00003b50: 6b65 7973 203d 2069 6e73 702e 6765 745f  keys = insp.get_
-00003b60: 666f 7265 6967 6e5f 6b65 7973 2861 6464  foreign_keys(add
-00003b70: 7265 7373 6573 2e6e 616d 652c 2073 6368  resses.name, sch
-00003b80: 656d 613d 7363 6865 6d61 290a 2020 2020  ema=schema).    
-00003b90: 2020 2020 666b 6579 3120 3d20 6164 6472      fkey1 = addr
-00003ba0: 5f66 6b65 7973 5b30 5d0a 0a20 2020 2020  _fkeys[0]..     
-00003bb0: 2020 2077 6974 6820 7465 7374 696e 672e     with testing.
-00003bc0: 7265 7175 6972 6573 2e69 6d70 6c69 6369  requires.implici
-00003bd0: 746c 795f 6e61 6d65 645f 636f 6e73 7472  tly_named_constr
-00003be0: 6169 6e74 732e 6661 696c 5f69 6628 293a  aints.fail_if():
-00003bf0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003c00: 662e 6173 7365 7274 5f28 666b 6579 315b  f.assert_(fkey1[
-00003c10: 226e 616d 6522 5d20 6973 206e 6f74 204e  "name"] is not N
-00003c20: 6f6e 6529 0a0a 2020 2020 2020 2020 6571  one)..        eq
-00003c30: 5f28 666b 6579 315b 2272 6566 6572 7265  _(fkey1["referre
-00003c40: 645f 7363 6865 6d61 225d 2c20 6578 7065  d_schema"], expe
-00003c50: 6374 6564 5f73 6368 656d 6129 0a20 2020  cted_schema).   
-00003c60: 2020 2020 2065 715f 2866 6b65 7931 5b22       eq_(fkey1["
-00003c70: 7265 6665 7272 6564 5f74 6162 6c65 225d  referred_table"]
-00003c80: 2c20 7573 6572 732e 6e61 6d65 290a 2020  , users.name).  
-00003c90: 2020 2020 2020 6571 5f28 666b 6579 315b        eq_(fkey1[
-00003ca0: 2272 6566 6572 7265 645f 636f 6c75 6d6e  "referred_column
-00003cb0: 7322 5d2c 205b 2275 7365 725f 6964 225d  s"], ["user_id"]
-00003cc0: 290a 2020 2020 2020 2020 6571 5f28 666b  ).        eq_(fk
-00003cd0: 6579 315b 2263 6f6e 7374 7261 696e 6564  ey1["constrained
-00003ce0: 5f63 6f6c 756d 6e73 225d 2c20 5b22 7265  _columns"], ["re
-00003cf0: 6d6f 7465 5f75 7365 725f 6964 225d 290a  mote_user_id"]).
-00003d00: 0a20 2020 2040 7465 7374 696e 672e 7265  .    @testing.re
-00003d10: 7175 6972 6573 2e66 6f72 6569 676e 5f6b  quires.foreign_k
-00003d20: 6579 5f63 6f6e 7374 7261 696e 745f 7265  ey_constraint_re
-00003d30: 666c 6563 7469 6f6e 0a20 2020 2040 7465  flection.    @te
-00003d40: 7374 696e 672e 636f 6d62 696e 6174 696f  sting.combinatio
-00003d50: 6e73 280a 2020 2020 2020 2020 284e 6f6e  ns(.        (Non
-00003d60: 652c 2054 7275 652c 2046 616c 7365 2c20  e, True, False, 
-00003d70: 4661 6c73 6529 2c0a 2020 2020 2020 2020  False),.        
-00003d80: 284e 6f6e 652c 2054 7275 652c 2046 616c  (None, True, Fal
-00003d90: 7365 2c20 5472 7565 2c20 7465 7374 696e  se, True, testin
-00003da0: 672e 7265 7175 6972 6573 2e73 6368 656d  g.requires.schem
-00003db0: 6173 292c 0a20 2020 2020 2020 2028 2266  as),.        ("f
-00003dc0: 6f72 6569 676e 5f6b 6579 222c 2054 7275  oreign_key", Tru
-00003dd0: 652c 2046 616c 7365 2c20 4661 6c73 6529  e, False, False)
-00003de0: 2c0a 2020 2020 2020 2020 284e 6f6e 652c  ,.        (None,
-00003df0: 2046 616c 7365 2c20 4661 6c73 652c 2046   False, False, F
-00003e00: 616c 7365 292c 0a20 2020 2020 2020 2028  alse),.        (
-00003e10: 4e6f 6e65 2c20 4661 6c73 652c 2046 616c  None, False, Fal
-00003e20: 7365 2c20 5472 7565 2c20 7465 7374 696e  se, True, testin
-00003e30: 672e 7265 7175 6972 6573 2e73 6368 656d  g.requires.schem
-00003e40: 6173 292c 0a20 2020 2020 2020 2028 4e6f  as),.        (No
-00003e50: 6e65 2c20 5472 7565 2c20 4661 6c73 652c  ne, True, False,
-00003e60: 2046 616c 7365 292c 0a20 2020 2020 2020   False),.       
-00003e70: 2028 4e6f 6e65 2c20 5472 7565 2c20 4661   (None, True, Fa
-00003e80: 6c73 652c 2054 7275 652c 2074 6573 7469  lse, True, testi
-00003e90: 6e67 2e72 6571 7569 7265 732e 7363 6865  ng.requires.sche
-00003ea0: 6d61 7329 2c0a 2020 2020 2020 2020 6172  mas),.        ar
-00003eb0: 676e 616d 6573 3d22 6f72 6465 725f 6279  gnames="order_by
-00003ec0: 2c69 6e63 6c75 6465 5f70 6c61 696e 2c69  ,include_plain,i
-00003ed0: 6e63 6c75 6465 5f76 6965 7773 2c75 7365  nclude_views,use
-00003ee0: 5f73 6368 656d 6122 2c0a 2020 2020 290a  _schema",.    ).
-00003ef0: 2020 2020 6465 6620 7465 7374 5f67 6574      def test_get
-00003f00: 5f74 6162 6c65 5f6e 616d 6573 280a 2020  _table_names(.  
-00003f10: 2020 2020 2020 7365 6c66 2c20 636f 6e6e        self, conn
-00003f20: 6563 7469 6f6e 2c20 6f72 6465 725f 6279  ection, order_by
-00003f30: 2c20 696e 636c 7564 655f 706c 6169 6e2c  , include_plain,
-00003f40: 2069 6e63 6c75 6465 5f76 6965 7773 2c20   include_views, 
-00003f50: 7573 655f 7363 6865 6d61 0a20 2020 2029  use_schema.    )
-00003f60: 3a0a 0a20 2020 2020 2020 2069 6620 7573  :..        if us
-00003f70: 655f 7363 6865 6d61 3a0a 2020 2020 2020  e_schema:.      
-00003f80: 2020 2020 2020 7363 6865 6d61 203d 2063        schema = c
-00003f90: 6f6e 6669 672e 7465 7374 5f73 6368 656d  onfig.test_schem
-00003fa0: 610a 2020 2020 2020 2020 656c 7365 3a0a  a.        else:.
-00003fb0: 2020 2020 2020 2020 2020 2020 7363 6865              sche
-00003fc0: 6d61 203d 204e 6f6e 650a 0a20 2020 2020  ma = None..     
-00003fd0: 2020 205f 6967 6e6f 7265 5f74 6162 6c65     _ignore_table
-00003fe0: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
-00003ff0: 2020 2261 6363 6f75 6e74 222c 0a20 2020    "account",.   
-00004000: 2020 2020 2020 2020 2022 616c 656d 6269           "alembi
-00004010: 635f 7665 7273 696f 6e22 2c0a 2020 2020  c_version",.    
-00004020: 2020 2020 2020 2020 2262 7974 6573 5f74          "bytes_t
-00004030: 6162 6c65 222c 0a20 2020 2020 2020 2020  able",.         
-00004040: 2020 2022 636f 6d6d 656e 745f 7465 7374     "comment_test
-00004050: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00004060: 6461 7465 5f74 6162 6c65 222c 0a20 2020  date_table",.   
-00004070: 2020 2020 2020 2020 2022 6e6f 6e63 6f6c           "noncol
-00004080: 5f69 6478 5f74 6573 745f 706b 222c 0a20  _idx_test_pk",. 
-00004090: 2020 2020 2020 2020 2020 2022 6e6f 6e63             "nonc
-000040a0: 6f6c 5f69 6478 5f74 6573 745f 6e6f 706b  ol_idx_test_nopk
-000040b0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-000040c0: 6c6f 6361 6c5f 7461 626c 6522 2c0a 2020  local_table",.  
-000040d0: 2020 2020 2020 2020 2020 2272 656d 6f74            "remot
-000040e0: 655f 7461 626c 6522 2c0a 2020 2020 2020  e_table",.      
-000040f0: 2020 2020 2020 2272 656d 6f74 655f 7461        "remote_ta
-00004100: 626c 655f 3222 2c0a 2020 2020 2020 2020  ble_2",.        
-00004110: 2020 2020 2274 6578 745f 7461 626c 6522      "text_table"
-00004120: 2c0a 2020 2020 2020 2020 2020 2020 2275  ,.            "u
-00004130: 7365 725f 746d 7022 2c0a 2020 2020 2020  ser_tmp",.      
-00004140: 2020 5d0a 0a20 2020 2020 2020 2069 6e73    ]..        ins
-00004150: 7020 3d20 696e 7370 6563 7428 636f 6e6e  p = inspect(conn
-00004160: 6563 7469 6f6e 290a 0a20 2020 2020 2020  ection)..       
-00004170: 2069 6620 696e 636c 7564 655f 7669 6577   if include_view
-00004180: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
-00004190: 6162 6c65 5f6e 616d 6573 203d 2069 6e73  able_names = ins
-000041a0: 702e 6765 745f 7669 6577 5f6e 616d 6573  p.get_view_names
-000041b0: 2873 6368 656d 6129 0a20 2020 2020 2020  (schema).       
-000041c0: 2020 2020 2074 6162 6c65 5f6e 616d 6573       table_names
-000041d0: 2e73 6f72 7428 290a 2020 2020 2020 2020  .sort().        
-000041e0: 2020 2020 616e 7377 6572 203d 205b 2265      answer = ["e
-000041f0: 6d61 696c 5f61 6464 7265 7373 6573 5f76  mail_addresses_v
-00004200: 222c 2022 7573 6572 735f 7622 5d0a 2020  ", "users_v"].  
-00004210: 2020 2020 2020 2020 2020 6571 5f28 736f            eq_(so
-00004220: 7274 6564 2874 6162 6c65 5f6e 616d 6573  rted(table_names
-00004230: 292c 2061 6e73 7765 7229 0a0a 2020 2020  ), answer)..    
-00004240: 2020 2020 6966 2069 6e63 6c75 6465 5f70      if include_p
-00004250: 6c61 696e 3a0a 2020 2020 2020 2020 2020  lain:.          
-00004260: 2020 6966 206f 7264 6572 5f62 793a 0a20    if order_by:. 
-00004270: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00004280: 6162 6c65 7320 3d20 5b0a 2020 2020 2020  ables = [.      
-00004290: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000042a0: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
-000042b0: 2020 2020 2020 2020 2066 6f72 2072 6563           for rec
-000042c0: 2069 6e20 696e 7370 2e67 6574 5f73 6f72   in insp.get_sor
-000042d0: 7465 645f 7461 626c 655f 616e 645f 666b  ted_table_and_fk
-000042e0: 635f 6e61 6d65 7328 7363 6865 6d61 290a  c_names(schema).
-000042f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004300: 2020 2020 6966 2072 6563 5b30 5d0a 2020      if rec[0].  
-00004310: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-00004320: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00004330: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004340: 2020 7461 626c 6573 203d 2069 6e73 702e    tables = insp.
-00004350: 6765 745f 7461 626c 655f 6e61 6d65 7328  get_table_names(
-00004360: 7363 6865 6d61 290a 2020 2020 2020 2020  schema).        
-00004370: 2020 2020 7461 626c 655f 6e61 6d65 7320      table_names 
-00004380: 3d20 5b74 2066 6f72 2074 2069 6e20 7461  = [t for t in ta
-00004390: 626c 6573 2069 6620 7420 6e6f 7420 696e  bles if t not in
-000043a0: 205f 6967 6e6f 7265 5f74 6162 6c65 735d   _ignore_tables]
-000043b0: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000043c0: 206f 7264 6572 5f62 7920 3d3d 2022 666f   order_by == "fo
-000043d0: 7265 6967 6e5f 6b65 7922 3a0a 2020 2020  reign_key":.    
-000043e0: 2020 2020 2020 2020 2020 2020 616e 7377              answ
-000043f0: 6572 203d 205b 2275 7365 7273 222c 2022  er = ["users", "
-00004400: 656d 6169 6c5f 6164 6472 6573 7365 7322  email_addresses"
-00004410: 2c20 2264 696e 6761 6c69 6e67 7322 5d0a  , "dingalings"].
-00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004430: 6571 5f28 7461 626c 655f 6e61 6d65 732c  eq_(table_names,
-00004440: 2061 6e73 7765 7229 0a20 2020 2020 2020   answer).       
-00004450: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00004460: 2020 2020 2020 2020 2020 2061 6e73 7765             answe
-00004470: 7220 3d20 5b22 6469 6e67 616c 696e 6773  r = ["dingalings
-00004480: 222c 2022 656d 6169 6c5f 6164 6472 6573  ", "email_addres
-00004490: 7365 7322 2c20 2275 7365 7273 225d 0a20  ses", "users"]. 
-000044a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000044b0: 715f 2873 6f72 7465 6428 7461 626c 655f  q_(sorted(table_
-000044c0: 6e61 6d65 7329 2c20 616e 7377 6572 290a  names), answer).
-000044d0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-000044e0: 640a 2020 2020 6465 6620 6465 6669 6e65  d.    def define
-000044f0: 5f74 656d 705f 7461 626c 6573 2863 6c73  _temp_tables(cls
-00004500: 2c20 6d65 7461 6461 7461 293a 0a20 2020  , metadata):.   
-00004510: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00004520: 2053 5041 4e4e 4552 204f 5645 5252 4944   SPANNER OVERRID
-00004530: 453a 0a0a 2020 2020 2020 2020 496e 2043  E:..        In C
-00004540: 6c6f 7564 2053 7061 6e6e 6572 2075 6e69  loud Spanner uni
-00004550: 7175 6520 696e 6465 7865 7320 6172 6520  que indexes are 
-00004560: 7573 6564 2069 6e73 7465 6164 206f 6620  used instead of 
-00004570: 6469 7265 6374 6c79 0a20 2020 2020 2020  directly.       
-00004580: 2063 7265 6174 696e 6720 756e 6971 7565   creating unique
-00004590: 2063 6f6e 7374 7261 696e 7473 2e20 4f76   constraints. Ov
-000045a0: 6572 7269 6469 6e67 2074 6865 2074 6573  erriding the tes
-000045b0: 7420 746f 2072 6570 6c61 6365 0a20 2020  t to replace.   
-000045c0: 2020 2020 2063 6f6e 7374 7261 696e 7473       constraints
-000045d0: 2077 6974 6820 696e 6465 7865 7320 696e   with indexes in
-000045e0: 2074 6573 7469 6e67 2064 6174 612e 0a20   testing data.. 
-000045f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00004600: 2020 206b 7720 3d20 7465 6d70 5f74 6162     kw = temp_tab
-00004610: 6c65 5f6b 6579 776f 7264 5f61 7267 7328  le_keyword_args(
-00004620: 636f 6e66 6967 2c20 636f 6e66 6967 2e64  config, config.d
-00004630: 6229 0a20 2020 2020 2020 2075 7365 725f  b).        user_
-00004640: 746d 7020 3d20 5461 626c 6528 0a20 2020  tmp = Table(.   
-00004650: 2020 2020 2020 2020 2022 7573 6572 5f74           "user_t
-00004660: 6d70 222c 0a20 2020 2020 2020 2020 2020  mp",.           
-00004670: 206d 6574 6164 6174 612c 0a20 2020 2020   metadata,.     
-00004680: 2020 2020 2020 2043 6f6c 756d 6e28 2269         Column("i
-00004690: 6422 2c20 7371 6c61 6c63 6865 6d79 2e49  d", sqlalchemy.I
-000046a0: 4e54 2c20 7072 696d 6172 795f 6b65 793d  NT, primary_key=
-000046b0: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-000046c0: 2020 2043 6f6c 756d 6e28 226e 616d 6522     Column("name"
-000046d0: 2c20 7371 6c61 6c63 6865 6d79 2e56 4152  , sqlalchemy.VAR
-000046e0: 4348 4152 2835 3029 292c 0a20 2020 2020  CHAR(50)),.     
-000046f0: 2020 2020 2020 2043 6f6c 756d 6e28 2266         Column("f
-00004700: 6f6f 222c 2073 716c 616c 6368 656d 792e  oo", sqlalchemy.
-00004710: 494e 5429 2c0a 2020 2020 2020 2020 2020  INT),.          
-00004720: 2020 7371 6c61 6c63 6865 6d79 2e49 6e64    sqlalchemy.Ind
-00004730: 6578 2822 7573 6572 5f74 6d70 5f75 7122  ex("user_tmp_uq"
-00004740: 2c20 226e 616d 6522 2c20 756e 6971 7565  , "name", unique
-00004750: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
-00004760: 2020 2020 7371 6c61 6c63 6865 6d79 2e49      sqlalchemy.I
-00004770: 6e64 6578 2822 7573 6572 5f74 6d70 5f69  ndex("user_tmp_i
-00004780: 7822 2c20 2266 6f6f 2229 2c0a 2020 2020  x", "foo"),.    
-00004790: 2020 2020 2020 2020 6578 7465 6e64 5f65          extend_e
-000047a0: 7869 7374 696e 673d 5472 7565 2c0a 2020  xisting=True,.  
-000047b0: 2020 2020 2020 2020 2020 2a2a 6b77 2c0a            **kw,.
-000047c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000047d0: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
-000047e0: 2020 2074 6573 7469 6e67 2e72 6571 7569     testing.requi
-000047f0: 7265 732e 7669 6577 5f72 6566 6c65 6374  res.view_reflect
-00004800: 696f 6e2e 656e 6162 6c65 640a 2020 2020  ion.enabled.    
-00004810: 2020 2020 2020 2020 616e 6420 7465 7374          and test
-00004820: 696e 672e 7265 7175 6972 6573 2e74 656d  ing.requires.tem
-00004830: 706f 7261 7279 5f76 6965 7773 2e65 6e61  porary_views.ena
-00004840: 626c 6564 0a20 2020 2020 2020 2029 3a0a  bled.        ):.
-00004850: 2020 2020 2020 2020 2020 2020 6576 656e              even
-00004860: 742e 6c69 7374 656e 280a 2020 2020 2020  t.listen(.      
-00004870: 2020 2020 2020 2020 2020 7573 6572 5f74            user_t
-00004880: 6d70 2c0a 2020 2020 2020 2020 2020 2020  mp,.            
-00004890: 2020 2020 2261 6674 6572 5f63 7265 6174      "after_creat
-000048a0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-000048b0: 2020 2020 4444 4c28 2263 7265 6174 6520      DDL("create 
-000048c0: 7465 6d70 6f72 6172 7920 7669 6577 2075  temporary view u
-000048d0: 7365 725f 746d 705f 7620 6173 2022 2022  ser_tmp_v as " "
-000048e0: 7365 6c65 6374 202a 2066 726f 6d20 7573  select * from us
-000048f0: 6572 5f74 6d70 2229 2c0a 2020 2020 2020  er_tmp"),.      
-00004900: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00004910: 2020 2020 6576 656e 742e 6c69 7374 656e      event.listen
-00004920: 2875 7365 725f 746d 702c 2022 6265 666f  (user_tmp, "befo
-00004930: 7265 5f64 726f 7022 2c20 4444 4c28 2264  re_drop", DDL("d
-00004940: 726f 7020 7669 6577 2075 7365 725f 746d  rop view user_tm
-00004950: 705f 7622 2929 0a0a 2020 2020 4074 6573  p_v"))..    @tes
-00004960: 7469 6e67 2e70 726f 7669 6465 5f6d 6574  ting.provide_met
-00004970: 6164 6174 610a 2020 2020 6465 6620 7465  adata.    def te
-00004980: 7374 5f72 6566 6c65 6374 5f73 7472 696e  st_reflect_strin
-00004990: 675f 636f 6c75 6d6e 5f6d 6178 5f6c 656e  g_column_max_len
-000049a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000049b0: 2222 220a 2020 2020 2020 2020 5350 414e  """.        SPAN
-000049c0: 4e45 5220 5350 4543 4946 4943 2054 4553  NER SPECIFIC TES
-000049d0: 543a 0a0a 2020 2020 2020 2020 496e 2053  T:..        In S
-000049e0: 7061 6e6e 6572 2063 6f6c 756d 6e20 6f66  panner column of
-000049f0: 2074 6865 2053 5452 494e 4720 7479 7065   the STRING type
-00004a00: 2063 616e 2062 650a 2020 2020 2020 2020   can be.        
-00004a10: 6372 6561 7465 6420 7769 7468 2073 697a  created with siz
-00004a20: 6520 6465 6669 6e65 6420 6173 204d 4158  e defined as MAX
-00004a30: 2e20 5468 6520 7465 7374 0a20 2020 2020  . The test.     
-00004a40: 2020 2063 6865 636b 7320 7468 6174 2073     checks that s
-00004a50: 7563 6820 6120 636f 6c75 6d6e 2069 7320  uch a column is 
-00004a60: 636f 7272 6563 746c 7920 7265 666c 6563  correctly reflec
-00004a70: 7465 642e 0a20 2020 2020 2020 2022 2222  ted..        """
-00004a80: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
-00004a90: 6120 3d20 4d65 7461 4461 7461 2873 656c  a = MetaData(sel
-00004aa0: 662e 6269 6e64 290a 2020 2020 2020 2020  f.bind).        
-00004ab0: 5461 626c 6528 2274 6578 745f 7461 626c  Table("text_tabl
-00004ac0: 6522 2c20 6d65 7461 6461 7461 2c20 436f  e", metadata, Co
-00004ad0: 6c75 6d6e 2822 5465 7374 436f 6c75 6d6e  lumn("TestColumn
-00004ae0: 222c 2054 6578 742c 206e 756c 6c61 626c  ", Text, nullabl
-00004af0: 653d 4661 6c73 6529 290a 2020 2020 2020  e=False)).      
-00004b00: 2020 6d65 7461 6461 7461 2e63 7265 6174    metadata.creat
-00004b10: 655f 616c 6c28 290a 0a20 2020 2020 2020  e_all()..       
-00004b20: 2054 6162 6c65 2822 7465 7874 5f74 6162   Table("text_tab
-00004b30: 6c65 222c 206d 6574 6164 6174 612c 2061  le", metadata, a
-00004b40: 7574 6f6c 6f61 643d 5472 7565 290a 0a20  utoload=True).. 
-00004b50: 2020 2064 6566 2074 6573 745f 7265 666c     def test_refl
-00004b60: 6563 745f 6279 7465 735f 636f 6c75 6d6e  ect_bytes_column
-00004b70: 5f6d 6178 5f6c 656e 2873 656c 6629 3a0a  _max_len(self):.
-00004b80: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00004b90: 2020 2020 5350 414e 4e45 5220 5350 4543      SPANNER SPEC
-00004ba0: 4946 4943 2054 4553 543a 0a0a 2020 2020  IFIC TEST:..    
-00004bb0: 2020 2020 496e 2053 7061 6e6e 6572 2063      In Spanner c
-00004bc0: 6f6c 756d 6e20 6f66 2074 6865 2042 5954  olumn of the BYT
-00004bd0: 4553 2074 7970 6520 6361 6e20 6265 0a20  ES type can be. 
-00004be0: 2020 2020 2020 2063 7265 6174 6564 2077         created w
-00004bf0: 6974 6820 7369 7a65 2064 6566 696e 6564  ith size defined
-00004c00: 2061 7320 4d41 582e 2054 6865 2074 6573   as MAX. The tes
-00004c10: 740a 2020 2020 2020 2020 6368 6563 6b73  t.        checks
-00004c20: 2074 6861 7420 7375 6368 2061 2063 6f6c   that such a col
-00004c30: 756d 6e20 6973 2063 6f72 7265 6374 6c79  umn is correctly
-00004c40: 2072 6566 6c65 6374 6564 2e0a 2020 2020   reflected..    
-00004c50: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00004c60: 6d65 7461 6461 7461 203d 204d 6574 6144  metadata = MetaD
-00004c70: 6174 6128 7365 6c66 2e62 696e 6429 0a20  ata(self.bind). 
-00004c80: 2020 2020 2020 2054 6162 6c65 280a 2020         Table(.  
-00004c90: 2020 2020 2020 2020 2020 2262 7974 6573            "bytes
-00004ca0: 5f74 6162 6c65 222c 0a20 2020 2020 2020  _table",.       
-00004cb0: 2020 2020 206d 6574 6164 6174 612c 0a20       metadata,. 
-00004cc0: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
-00004cd0: 6e28 2254 6573 7443 6f6c 756d 6e22 2c20  n("TestColumn", 
-00004ce0: 4c61 7267 6542 696e 6172 792c 206e 756c  LargeBinary, nul
-00004cf0: 6c61 626c 653d 4661 6c73 6529 2c0a 2020  lable=False),.  
-00004d00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00004d10: 6d65 7461 6461 7461 2e63 7265 6174 655f  metadata.create_
-00004d20: 616c 6c28 290a 0a20 2020 2020 2020 2054  all()..        T
-00004d30: 6162 6c65 2822 6279 7465 735f 7461 626c  able("bytes_tabl
-00004d40: 6522 2c20 6d65 7461 6461 7461 2c20 6175  e", metadata, au
-00004d50: 746f 6c6f 6164 3d54 7275 6529 0a0a 2020  toload=True)..  
-00004d60: 2020 4074 6573 7469 6e67 2e63 6f6d 6269    @testing.combi
-00004d70: 6e61 7469 6f6e 7328 0a20 2020 2020 2020  nations(.       
-00004d80: 2028 5472 7565 2c20 7465 7374 696e 672e   (True, testing.
-00004d90: 7265 7175 6972 6573 2e73 6368 656d 6173  requires.schemas
-00004da0: 292c 2028 4661 6c73 652c 292c 2061 7267  ), (False,), arg
-00004db0: 6e61 6d65 733d 2275 7365 5f73 6368 656d  names="use_schem
-00004dc0: 6122 0a20 2020 2029 0a20 2020 2040 7465  a".    ).    @te
-00004dd0: 7374 696e 672e 7265 7175 6972 6573 2e75  sting.requires.u
-00004de0: 6e69 7175 655f 636f 6e73 7472 6169 6e74  nique_constraint
-00004df0: 5f72 6566 6c65 6374 696f 6e0a 2020 2020  _reflection.    
-00004e00: 6465 6620 7465 7374 5f67 6574 5f75 6e69  def test_get_uni
-00004e10: 7175 655f 636f 6e73 7472 6169 6e74 7328  que_constraints(
-00004e20: 7365 6c66 2c20 6d65 7461 6461 7461 2c20  self, metadata, 
-00004e30: 636f 6e6e 6563 7469 6f6e 2c20 7573 655f  connection, use_
-00004e40: 7363 6865 6d61 293a 0a20 2020 2020 2020  schema):.       
-00004e50: 2023 2053 514c 6974 6520 6469 616c 6563   # SQLite dialec
-00004e60: 7420 6e65 6564 7320 746f 2070 6172 7365  t needs to parse
-00004e70: 2074 6865 206e 616d 6573 206f 6620 7468   the names of th
-00004e80: 6520 636f 6e73 7472 6169 6e74 730a 2020  e constraints.  
-00004e90: 2020 2020 2020 2320 7365 7061 7261 7465        # separate
-00004ea0: 6c79 2066 726f 6d20 7768 6174 2069 7420  ly from what it 
-00004eb0: 6765 7473 2066 726f 6d20 5052 4147 4d41  gets from PRAGMA
-00004ec0: 2069 6e64 6578 5f6c 6973 7428 292c 2061   index_list(), a
-00004ed0: 6e64 0a20 2020 2020 2020 2023 2074 6865  nd.        # the
-00004ee0: 6e20 6d61 7463 6865 7320 7468 656d 2075  n matches them u
-00004ef0: 702e 2020 736f 2073 616d 6520 7365 7420  p.  so same set 
-00004f00: 6f66 2063 6f6c 756d 6e5f 6e61 6d65 7320  of column_names 
-00004f10: 696e 2074 776f 0a20 2020 2020 2020 2023  in two.        #
-00004f20: 2063 6f6e 7374 7261 696e 7473 2077 696c   constraints wil
-00004f30: 6c20 636f 6e66 7573 6520 6974 2e20 2020  l confuse it.   
-00004f40: 2050 6572 6861 7073 2077 6520 7368 6f75   Perhaps we shou
-00004f50: 6c64 206e 6f20 6c6f 6e67 6572 0a20 2020  ld no longer.   
-00004f60: 2020 2020 2023 2062 6f74 6865 7220 7769       # bother wi
-00004f70: 7468 2069 6e64 6578 5f6c 6973 7428 2920  th index_list() 
-00004f80: 6865 7265 2073 696e 6365 2077 6520 6861  here since we ha
-00004f90: 7665 2074 6865 2077 686f 6c65 0a20 2020  ve the whole.   
-00004fa0: 2020 2020 2023 2043 5245 4154 4520 5441       # CREATE TA
-00004fb0: 424c 453f 0a0a 2020 2020 2020 2020 6966  BLE?..        if
-00004fc0: 2075 7365 5f73 6368 656d 613a 0a20 2020   use_schema:.   
-00004fd0: 2020 2020 2020 2020 2073 6368 656d 6120           schema 
-00004fe0: 3d20 636f 6e66 6967 2e74 6573 745f 7363  = config.test_sc
-00004ff0: 6865 6d61 0a20 2020 2020 2020 2065 6c73  hema.        els
-00005000: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00005010: 6368 656d 6120 3d20 4e6f 6e65 0a20 2020  chema = None.   
-00005020: 2020 2020 2075 6e69 7175 6573 203d 2073       uniques = s
-00005030: 6f72 7465 6428 0a20 2020 2020 2020 2020  orted(.         
-00005040: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-00005050: 2020 2020 207b 226e 616d 6522 3a20 2275       {"name": "u
-00005060: 6e69 7175 655f 6122 2c20 2263 6f6c 756d  nique_a", "colum
-00005070: 6e5f 6e61 6d65 7322 3a20 5b22 6122 5d7d  n_names": ["a"]}
-00005080: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005090: 2020 7b22 6e61 6d65 223a 2022 756e 6971    {"name": "uniq
-000050a0: 7565 5f61 5f62 5f63 222c 2022 636f 6c75  ue_a_b_c", "colu
-000050b0: 6d6e 5f6e 616d 6573 223a 205b 2261 222c  mn_names": ["a",
-000050c0: 2022 6222 2c20 2263 225d 7d2c 0a20 2020   "b", "c"]},.   
-000050d0: 2020 2020 2020 2020 2020 2020 207b 226e               {"n
-000050e0: 616d 6522 3a20 2275 6e69 7175 655f 635f  ame": "unique_c_
-000050f0: 615f 6222 2c20 2263 6f6c 756d 6e5f 6e61  a_b", "column_na
-00005100: 6d65 7322 3a20 5b22 6322 2c20 2261 222c  mes": ["c", "a",
-00005110: 2022 6222 5d7d 2c0a 2020 2020 2020 2020   "b"]},.        
-00005120: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
-00005130: 2022 756e 6971 7565 5f61 7363 5f6b 6579   "unique_asc_key
-00005140: 222c 2022 636f 6c75 6d6e 5f6e 616d 6573  ", "column_names
-00005150: 223a 205b 2261 7363 222c 2022 6b65 7922  ": ["asc", "key"
-00005160: 5d7d 2c0a 2020 2020 2020 2020 2020 2020  ]},.            
-00005170: 2020 2020 7b22 6e61 6d65 223a 2022 692e      {"name": "i.
-00005180: 6861 7665 2e64 6f74 7322 2c20 2263 6f6c  have.dots", "col
-00005190: 756d 6e5f 6e61 6d65 7322 3a20 5b22 6222  umn_names": ["b"
-000051a0: 5d7d 2c0a 2020 2020 2020 2020 2020 2020  ]},.            
-000051b0: 2020 2020 7b22 6e61 6d65 223a 2022 6920      {"name": "i 
-000051c0: 6861 7665 2073 7061 6365 7322 2c20 2263  have spaces", "c
-000051d0: 6f6c 756d 6e5f 6e61 6d65 7322 3a20 5b22  olumn_names": ["
-000051e0: 6322 5d7d 2c0a 2020 2020 2020 2020 2020  c"]},.          
-000051f0: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
-00005200: 206b 6579 3d6f 7065 7261 746f 722e 6974   key=operator.it
-00005210: 656d 6765 7474 6572 2822 6e61 6d65 2229  emgetter("name")
-00005220: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00005230: 2020 2020 7461 626c 6520 3d20 5461 626c      table = Tabl
-00005240: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
-00005250: 7465 7374 7462 6c22 2c0a 2020 2020 2020  testtbl",.      
-00005260: 2020 2020 2020 6d65 7461 6461 7461 2c0a        metadata,.
-00005270: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
-00005280: 6d6e 2822 6964 222c 2073 716c 616c 6368  mn("id", sqlalch
-00005290: 656d 792e 494e 542c 2070 7269 6d61 7279  emy.INT, primary
-000052a0: 5f6b 6579 3d54 7275 6529 2c0a 2020 2020  _key=True),.    
-000052b0: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-000052c0: 6122 2c20 5374 7269 6e67 2832 3029 292c  a", String(20)),
-000052d0: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-000052e0: 756d 6e28 2262 222c 2053 7472 696e 6728  umn("b", String(
-000052f0: 3330 2929 2c0a 2020 2020 2020 2020 2020  30)),.          
-00005300: 2020 436f 6c75 6d6e 2822 6322 2c20 496e    Column("c", In
-00005310: 7465 6765 7229 2c0a 2020 2020 2020 2020  teger),.        
-00005320: 2020 2020 2320 7265 7365 7276 6564 2069      # reserved i
-00005330: 6465 6e74 6966 6965 7273 0a20 2020 2020  dentifiers.     
-00005340: 2020 2020 2020 2043 6f6c 756d 6e28 2261         Column("a
-00005350: 7363 222c 2053 7472 696e 6728 3330 2929  sc", String(30))
-00005360: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
-00005370: 6c75 6d6e 2822 6b65 7922 2c20 5374 7269  lumn("key", Stri
-00005380: 6e67 2833 3029 292c 0a20 2020 2020 2020  ng(30)),.       
-00005390: 2020 2020 2073 716c 616c 6368 656d 792e       sqlalchemy.
-000053a0: 496e 6465 7828 2275 6e69 7175 655f 6122  Index("unique_a"
-000053b0: 2c20 2261 222c 2075 6e69 7175 653d 5472  , "a", unique=Tr
-000053c0: 7565 292c 0a20 2020 2020 2020 2020 2020  ue),.           
-000053d0: 2073 716c 616c 6368 656d 792e 496e 6465   sqlalchemy.Inde
-000053e0: 7828 2275 6e69 7175 655f 615f 625f 6322  x("unique_a_b_c"
-000053f0: 2c20 2261 222c 2022 6222 2c20 2263 222c  , "a", "b", "c",
-00005400: 2075 6e69 7175 653d 5472 7565 292c 0a20   unique=True),. 
-00005410: 2020 2020 2020 2020 2020 2073 716c 616c             sqlal
-00005420: 6368 656d 792e 496e 6465 7828 2275 6e69  chemy.Index("uni
-00005430: 7175 655f 635f 615f 6222 2c20 2263 222c  que_c_a_b", "c",
-00005440: 2022 6122 2c20 2262 222c 2075 6e69 7175   "a", "b", uniqu
-00005450: 653d 5472 7565 292c 0a20 2020 2020 2020  e=True),.       
-00005460: 2020 2020 2073 716c 616c 6368 656d 792e       sqlalchemy.
-00005470: 496e 6465 7828 2275 6e69 7175 655f 6173  Index("unique_as
-00005480: 635f 6b65 7922 2c20 2261 7363 222c 2022  c_key", "asc", "
-00005490: 6b65 7922 2c20 756e 6971 7565 3d54 7275  key", unique=Tru
-000054a0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-000054b0: 7363 6865 6d61 3d73 6368 656d 612c 0a20  schema=schema,. 
-000054c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000054d0: 2074 6162 6c65 2e63 7265 6174 6528 636f   table.create(co
-000054e0: 6e6e 6563 7469 6f6e 290a 2020 2020 2020  nnection).      
-000054f0: 2020 636f 6e6e 6563 7469 6f6e 2e63 6f6e    connection.con
-00005500: 6e65 6374 696f 6e2e 636f 6d6d 6974 2829  nection.commit()
-00005510: 0a0a 2020 2020 2020 2020 696e 7370 6563  ..        inspec
-00005520: 746f 7220 3d20 696e 7370 6563 7428 636f  tor = inspect(co
-00005530: 6e6e 6563 7469 6f6e 290a 2020 2020 2020  nnection).      
-00005540: 2020 7265 666c 6563 7465 6420 3d20 736f    reflected = so
-00005550: 7274 6564 280a 2020 2020 2020 2020 2020  rted(.          
-00005560: 2020 696e 7370 6563 746f 722e 6765 745f    inspector.get_
-00005570: 756e 6971 7565 5f63 6f6e 7374 7261 696e  unique_constrain
-00005580: 7473 2822 7465 7374 7462 6c22 2c20 7363  ts("testtbl", sc
-00005590: 6865 6d61 3d73 6368 656d 6129 2c0a 2020  hema=schema),.  
-000055a0: 2020 2020 2020 2020 2020 6b65 793d 6f70            key=op
-000055b0: 6572 6174 6f72 2e69 7465 6d67 6574 7465  erator.itemgette
-000055c0: 7228 226e 616d 6522 292c 0a20 2020 2020  r("name"),.     
-000055d0: 2020 2029 0a0a 2020 2020 2020 2020 6e61     )..        na
-000055e0: 6d65 735f 7468 6174 5f64 7570 6c69 6361  mes_that_duplica
-000055f0: 7465 5f69 6e64 6578 203d 2073 6574 2829  te_index = set()
-00005600: 0a0a 2020 2020 2020 2020 666f 7220 6f72  ..        for or
-00005610: 6967 2c20 7265 666c 2069 6e20 7a69 7028  ig, refl in zip(
-00005620: 756e 6971 7565 732c 2072 6566 6c65 6374  uniques, reflect
-00005630: 6564 293a 0a20 2020 2020 2020 2020 2020  ed):.           
-00005640: 2023 2044 6966 6665 7265 6e74 2064 6961   # Different dia
-00005650: 6c65 6374 7320 6861 6e64 6c65 2064 7570  lects handle dup
-00005660: 6c69 6361 7465 2069 6e64 6578 2061 6e64  licate index and
-00005670: 2063 6f6e 7374 7261 696e 7473 0a20 2020   constraints.   
-00005680: 2020 2020 2020 2020 2023 2064 6966 6665           # diffe
-00005690: 7265 6e74 6c79 2c20 736f 2069 676e 6f72  rently, so ignor
-000056a0: 6520 7468 6973 2066 6c61 670a 2020 2020  e this flag.    
-000056b0: 2020 2020 2020 2020 6475 7065 203d 2072          dupe = r
-000056c0: 6566 6c2e 706f 7028 2264 7570 6c69 6361  efl.pop("duplica
-000056d0: 7465 735f 696e 6465 7822 2c20 4e6f 6e65  tes_index", None
-000056e0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-000056f0: 2064 7570 653a 0a20 2020 2020 2020 2020   dupe:.         
-00005700: 2020 2020 2020 206e 616d 6573 5f74 6861         names_tha
-00005710: 745f 6475 706c 6963 6174 655f 696e 6465  t_duplicate_inde
-00005720: 782e 6164 6428 6475 7065 290a 2020 2020  x.add(dupe).    
-00005730: 2020 2020 2020 2020 6571 5f28 6f72 6967          eq_(orig
-00005740: 2c20 7265 666c 290a 0a20 2020 2020 2020  , refl)..       
-00005750: 2072 6566 6c65 6374 6564 5f6d 6574 6164   reflected_metad
-00005760: 6174 6120 3d20 4d65 7461 4461 7461 2829  ata = MetaData()
-00005770: 0a20 2020 2020 2020 2072 6566 6c65 6374  .        reflect
-00005780: 6564 203d 2054 6162 6c65 280a 2020 2020  ed = Table(.    
-00005790: 2020 2020 2020 2020 2274 6573 7474 626c          "testtbl
-000057a0: 222c 0a20 2020 2020 2020 2020 2020 2072  ",.            r
-000057b0: 6566 6c65 6374 6564 5f6d 6574 6164 6174  eflected_metadat
-000057c0: 612c 0a20 2020 2020 2020 2020 2020 2061  a,.            a
-000057d0: 7574 6f6c 6f61 645f 7769 7468 3d63 6f6e  utoload_with=con
-000057e0: 6e65 6374 696f 6e2c 0a20 2020 2020 2020  nection,.       
-000057f0: 2020 2020 2073 6368 656d 613d 7363 6865       schema=sche
-00005800: 6d61 2c0a 2020 2020 2020 2020 290a 0a20  ma,.        ).. 
-00005810: 2020 2020 2020 2023 2074 6573 7420 2264         # test "d
-00005820: 6564 7570 6c69 6361 7465 7320 666f 7220  eduplicates for 
-00005830: 696e 6465 7822 206c 6f67 6963 2e20 2020  index" logic.   
-00005840: 4d79 5351 4c20 616e 6420 4f72 6163 6c65  MySQL and Oracle
-00005850: 0a20 2020 2020 2020 2023 2022 756e 6971  .        # "uniq
-00005860: 7565 2063 6f6e 7374 7261 696e 7473 2220  ue constraints" 
-00005870: 6172 6520 6163 7475 616c 6c79 2075 6e69  are actually uni
-00005880: 7175 6520 696e 6465 7865 7320 2877 6974  que indexes (wit
-00005890: 6820 706f 7373 6962 6c65 0a20 2020 2020  h possible.     
-000058a0: 2020 2023 2065 7863 6570 7469 6f6e 206f     # exception o
-000058b0: 6620 6120 756e 6971 7565 2074 6861 7420  f a unique that 
-000058c0: 6973 2061 2064 7570 6520 6f66 2061 6e6f  is a dupe of ano
-000058d0: 7468 6572 206f 6e65 2069 6e20 7468 6520  ther one in the 
-000058e0: 6361 7365 0a20 2020 2020 2020 2023 206f  case.        # o
-000058f0: 6620 4f72 6163 6c65 292e 2020 6d61 6b65  f Oracle).  make
-00005900: 2073 7572 6520 2320 7468 6579 2061 7265   sure # they are
-00005910: 6e27 7420 6475 706c 6963 6174 6564 2e0a  n't duplicated..
-00005920: 2020 2020 2020 2020 6964 785f 6e61 6d65          idx_name
-00005930: 7320 3d20 7365 7428 5b69 6478 2e6e 616d  s = set([idx.nam
-00005940: 6520 666f 7220 6964 7820 696e 2072 6566  e for idx in ref
-00005950: 6c65 6374 6564 2e69 6e64 6578 6573 5d29  lected.indexes])
-00005960: 0a20 2020 2020 2020 2075 715f 6e61 6d65  .        uq_name
-00005970: 7320 3d20 7365 7428 0a20 2020 2020 2020  s = set(.       
-00005980: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-00005990: 2020 2020 2020 2075 712e 6e61 6d65 0a20         uq.name. 
-000059a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000059b0: 6f72 2075 7120 696e 2072 6566 6c65 6374  or uq in reflect
-000059c0: 6564 2e63 6f6e 7374 7261 696e 7473 0a20  ed.constraints. 
-000059d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000059e0: 6620 6973 696e 7374 616e 6365 2875 712c  f isinstance(uq,
-000059f0: 2073 716c 616c 6368 656d 792e 556e 6971   sqlalchemy.Uniq
-00005a00: 7565 436f 6e73 7472 6169 6e74 290a 2020  ueConstraint).  
-00005a10: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-00005a20: 2020 2020 292e 6469 6666 6572 656e 6365      ).difference
-00005a30: 285b 2275 6e69 7175 655f 635f 615f 6222  (["unique_c_a_b"
-00005a40: 5d29 0a0a 2020 2020 2020 2020 6173 7365  ])..        asse
-00005a50: 7274 206e 6f74 2069 6478 5f6e 616d 6573  rt not idx_names
-00005a60: 2e69 6e74 6572 7365 6374 696f 6e28 7571  .intersection(uq
-00005a70: 5f6e 616d 6573 290a 2020 2020 2020 2020  _names).        
-00005a80: 6966 206e 616d 6573 5f74 6861 745f 6475  if names_that_du
-00005a90: 706c 6963 6174 655f 696e 6465 783a 0a20  plicate_index:. 
-00005aa0: 2020 2020 2020 2020 2020 2065 715f 286e             eq_(n
-00005ab0: 616d 6573 5f74 6861 745f 6475 706c 6963  ames_that_duplic
-00005ac0: 6174 655f 696e 6465 782c 2069 6478 5f6e  ate_index, idx_n
-00005ad0: 616d 6573 290a 2020 2020 2020 2020 2020  ames).          
-00005ae0: 2020 6571 5f28 7571 5f6e 616d 6573 2c20    eq_(uq_names, 
-00005af0: 7365 7428 2929 0a0a 2020 2020 4074 6573  set())..    @tes
-00005b00: 7469 6e67 2e70 726f 7669 6465 5f6d 6574  ting.provide_met
-00005b10: 6164 6174 610a 2020 2020 6465 6620 7465  adata.    def te
-00005b20: 7374 5f75 6e69 7175 655f 636f 6e73 7472  st_unique_constr
-00005b30: 6169 6e74 5f72 6169 7365 7328 7365 6c66  aint_raises(self
-00005b40: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00005b50: 2020 2020 2020 2043 6865 636b 696e 6720         Checking 
-00005b60: 7468 6174 2075 6e69 7175 6520 636f 6e73  that unique cons
-00005b70: 7472 6169 6e74 2063 7265 6174 696f 6e0a  traint creation.
-00005b80: 2020 2020 2020 2020 6661 696c 7320 6475          fails du
-00005b90: 6520 746f 2061 2050 726f 6772 616d 6d69  e to a Programmi
-00005ba0: 6e67 4572 726f 722e 0a20 2020 2020 2020  ngError..       
-00005bb0: 2022 2222 0a20 2020 2020 2020 206d 6574   """.        met
-00005bc0: 6164 6174 6120 3d20 4d65 7461 4461 7461  adata = MetaData
-00005bd0: 2873 656c 662e 6269 6e64 290a 2020 2020  (self.bind).    
-00005be0: 2020 2020 5461 626c 6528 0a20 2020 2020      Table(.     
-00005bf0: 2020 2020 2020 2022 7573 6572 5f74 6d70         "user_tmp
-00005c00: 5f66 6169 6c75 7265 222c 0a20 2020 2020  _failure",.     
-00005c10: 2020 2020 2020 206d 6574 6164 6174 612c         metadata,
-00005c20: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-00005c30: 756d 6e28 2269 6422 2c20 7371 6c61 6c63  umn("id", sqlalc
-00005c40: 6865 6d79 2e49 4e54 2c20 7072 696d 6172  hemy.INT, primar
-00005c50: 795f 6b65 793d 5472 7565 292c 0a20 2020  y_key=True),.   
-00005c60: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00005c70: 226e 616d 6522 2c20 7371 6c61 6c63 6865  "name", sqlalche
-00005c80: 6d79 2e56 4152 4348 4152 2835 3029 292c  my.VARCHAR(50)),
-00005c90: 0a20 2020 2020 2020 2020 2020 2073 716c  .            sql
-00005ca0: 616c 6368 656d 792e 556e 6971 7565 436f  alchemy.UniqueCo
-00005cb0: 6e73 7472 6169 6e74 2822 6e61 6d65 222c  nstraint("name",
-00005cc0: 206e 616d 653d 2275 7365 725f 746d 705f   name="user_tmp_
-00005cd0: 7571 2229 2c0a 2020 2020 2020 2020 290a  uq"),.        ).
-00005ce0: 0a20 2020 2020 2020 2077 6974 6820 7079  .        with py
-00005cf0: 7465 7374 2e72 6169 7365 7328 7370 616e  test.raises(span
-00005d00: 6e65 725f 6462 6170 692e 6578 6365 7074  ner_dbapi.except
-00005d10: 696f 6e73 2e50 726f 6772 616d 6d69 6e67  ions.Programming
-00005d20: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-00005d30: 2020 2020 6d65 7461 6461 7461 2e63 7265      metadata.cre
-00005d40: 6174 655f 616c 6c28 290a 0a20 2020 2040  ate_all()..    @
-00005d50: 7465 7374 696e 672e 7072 6f76 6964 655f  testing.provide_
-00005d60: 6d65 7461 6461 7461 0a20 2020 2064 6566  metadata.    def
-00005d70: 205f 7465 7374 5f67 6574 5f74 6162 6c65   _test_get_table
-00005d80: 5f6e 616d 6573 2873 656c 662c 2073 6368  _names(self, sch
-00005d90: 656d 613d 4e6f 6e65 2c20 7461 626c 655f  ema=None, table_
-00005da0: 7479 7065 3d22 7461 626c 6522 2c20 6f72  type="table", or
-00005db0: 6465 725f 6279 3d4e 6f6e 6529 3a0a 2020  der_by=None):.  
-00005dc0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00005dd0: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
-00005de0: 4445 3a0a 0a20 2020 2020 2020 2053 7061  DE:..        Spa
-00005df0: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
-00005e00: 706f 7274 2074 656d 706f 7261 7279 2074  port temporary t
-00005e10: 6162 6c65 732c 2073 6f20 7265 616c 2074  ables, so real t
-00005e20: 6162 6c65 7320 6172 650a 2020 2020 2020  ables are.      
-00005e30: 2020 7573 6564 2066 6f72 2074 6573 7469    used for testi
-00005e40: 6e67 2e20 4173 2074 6865 206f 7269 6769  ng. As the origi
-00005e50: 6e61 6c20 7465 7374 2065 7870 6563 7473  nal test expects
-00005e60: 206f 6e6c 7920 7265 616c 0a20 2020 2020   only real.     
-00005e70: 2020 2074 6162 6c65 7320 746f 2062 6520     tables to be 
-00005e80: 7265 6164 2c20 616e 6420 696e 2053 7061  read, and in Spa
-00005e90: 6e6e 6572 2061 6c6c 2074 6865 2074 6162  nner all the tab
-00005ea0: 6c65 7320 6172 6520 7265 616c 2c0a 2020  les are real,.  
-00005eb0: 2020 2020 2020 6578 7065 6374 6564 2072        expected r
-00005ec0: 6573 756c 7473 206f 7665 7272 6964 6520  esults override 
-00005ed0: 6973 2072 6571 7569 7265 642e 0a20 2020  is required..   
-00005ee0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00005ef0: 205f 6967 6e6f 7265 5f74 6162 6c65 7320   _ignore_tables 
-00005f00: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-00005f10: 2263 6f6d 6d65 6e74 5f74 6573 7422 2c0a  "comment_test",.
-00005f20: 2020 2020 2020 2020 2020 2020 226e 6f6e              "non
-00005f30: 636f 6c5f 6964 785f 7465 7374 5f70 6b22  col_idx_test_pk"
-00005f40: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
-00005f50: 6f6e 636f 6c5f 6964 785f 7465 7374 5f6e  oncol_idx_test_n
-00005f60: 6f70 6b22 2c0a 2020 2020 2020 2020 2020  opk",.          
-00005f70: 2020 226c 6f63 616c 5f74 6162 6c65 222c    "local_table",
-00005f80: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
-00005f90: 6d6f 7465 5f74 6162 6c65 222c 0a20 2020  mote_table",.   
-00005fa0: 2020 2020 2020 2020 2022 7265 6d6f 7465           "remote
-00005fb0: 5f74 6162 6c65 5f32 222c 0a20 2020 2020  _table_2",.     
-00005fc0: 2020 205d 0a20 2020 2020 2020 206d 6574     ].        met
-00005fd0: 6120 3d20 7365 6c66 2e6d 6574 6164 6174  a = self.metadat
-00005fe0: 610a 0a20 2020 2020 2020 2069 6e73 7020  a..        insp 
-00005ff0: 3d20 696e 7370 6563 7428 6d65 7461 2e62  = inspect(meta.b
-00006000: 696e 6429 0a0a 2020 2020 2020 2020 6966  ind)..        if
-00006010: 2074 6162 6c65 5f74 7970 6520 3d3d 2022   table_type == "
-00006020: 7669 6577 223a 0a20 2020 2020 2020 2020  view":.         
-00006030: 2020 2074 6162 6c65 5f6e 616d 6573 203d     table_names =
-00006040: 2069 6e73 702e 6765 745f 7669 6577 5f6e   insp.get_view_n
-00006050: 616d 6573 2873 6368 656d 6129 0a20 2020  ames(schema).   
-00006060: 2020 2020 2020 2020 2074 6162 6c65 5f6e           table_n
-00006070: 616d 6573 2e73 6f72 7428 290a 2020 2020  ames.sort().    
-00006080: 2020 2020 2020 2020 616e 7377 6572 203d          answer =
-00006090: 205b 2265 6d61 696c 5f61 6464 7265 7373   ["email_address
-000060a0: 6573 5f76 222c 2022 7573 6572 735f 7622  es_v", "users_v"
-000060b0: 5d0a 2020 2020 2020 2020 2020 2020 6571  ].            eq
-000060c0: 5f28 736f 7274 6564 2874 6162 6c65 5f6e  _(sorted(table_n
-000060d0: 616d 6573 292c 2061 6e73 7765 7229 0a20  ames), answer). 
-000060e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000060f0: 2020 2020 2020 2020 2069 6620 6f72 6465           if orde
-00006100: 725f 6279 3a0a 2020 2020 2020 2020 2020  r_by:.          
-00006110: 2020 2020 2020 7461 626c 6573 203d 205b        tables = [
-00006120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006130: 2020 2020 2072 6563 5b30 5d0a 2020 2020       rec[0].    
-00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006150: 666f 7220 7265 6320 696e 2069 6e73 702e  for rec in insp.
-00006160: 6765 745f 736f 7274 6564 5f74 6162 6c65  get_sorted_table
-00006170: 5f61 6e64 5f66 6b63 5f6e 616d 6573 2873  _and_fkc_names(s
-00006180: 6368 656d 6129 0a20 2020 2020 2020 2020  chema).         
-00006190: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-000061a0: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
-000061b0: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
-000061c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000061d0: 2020 2020 2020 2020 2074 6162 6c65 7320           tables 
-000061e0: 3d20 696e 7370 2e67 6574 5f74 6162 6c65  = insp.get_table
-000061f0: 5f6e 616d 6573 2873 6368 656d 6129 0a20  _names(schema). 
-00006200: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-00006210: 5f6e 616d 6573 203d 205b 7420 666f 7220  _names = [t for 
-00006220: 7420 696e 2074 6162 6c65 7320 6966 2074  t in tables if t
-00006230: 206e 6f74 2069 6e20 5f69 676e 6f72 655f   not in _ignore_
-00006240: 7461 626c 6573 5d0a 0a20 2020 2020 2020  tables]..       
-00006250: 2020 2020 2069 6620 6f72 6465 725f 6279       if order_by
-00006260: 203d 3d20 2266 6f72 6569 676e 5f6b 6579   == "foreign_key
-00006270: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00006280: 2020 2061 6e73 7765 7220 3d20 7b22 6469     answer = {"di
-00006290: 6e67 616c 696e 6773 222c 2022 656d 6169  ngalings", "emai
-000062a0: 6c5f 6164 6472 6573 7365 7322 2c20 2275  l_addresses", "u
-000062b0: 7365 725f 746d 7022 2c20 2275 7365 7273  ser_tmp", "users
-000062c0: 227d 0a20 2020 2020 2020 2020 2020 2020  "}.             
-000062d0: 2020 2065 715f 2873 6574 2874 6162 6c65     eq_(set(table
-000062e0: 5f6e 616d 6573 292c 2061 6e73 7765 7229  _names), answer)
-000062f0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00006300: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00006310: 2020 2061 6e73 7765 7220 3d20 5b22 6469     answer = ["di
-00006320: 6e67 616c 696e 6773 222c 2022 656d 6169  ngalings", "emai
-00006330: 6c5f 6164 6472 6573 7365 7322 2c20 2275  l_addresses", "u
-00006340: 7365 725f 746d 7022 2c20 2275 7365 7273  ser_tmp", "users
-00006350: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-00006360: 2020 2065 715f 2873 6f72 7465 6428 7461     eq_(sorted(ta
-00006370: 626c 655f 6e61 6d65 7329 2c20 616e 7377  ble_names), answ
-00006380: 6572 290a 0a20 2020 2040 7079 7465 7374  er)..    @pytest
-00006390: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
-000063a0: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
-000063b0: 6f72 7420 7465 6d70 6f72 6172 7920 7461  ort temporary ta
-000063c0: 626c 6573 2229 0a20 2020 2064 6566 2074  bles").    def t
-000063d0: 6573 745f 6765 745f 7465 6d70 5f74 6162  est_get_temp_tab
-000063e0: 6c65 5f69 6e64 6578 6573 2873 656c 6629  le_indexes(self)
-000063f0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-00006400: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00006410: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
-00006420: 6f65 736e 2774 2073 7570 706f 7274 2074  oesn't support t
-00006430: 656d 706f 7261 7279 2074 6162 6c65 7322  emporary tables"
-00006440: 290a 2020 2020 6465 6620 7465 7374 5f67  ).    def test_g
-00006450: 6574 5f74 656d 705f 7461 626c 655f 756e  et_temp_table_un
-00006460: 6971 7565 5f63 6f6e 7374 7261 696e 7473  ique_constraints
-00006470: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00006480: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
-00006490: 742e 6d61 726b 2e73 6b69 7028 2253 7061  t.mark.skip("Spa
-000064a0: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
-000064b0: 706f 7274 2074 656d 706f 7261 7279 2074  port temporary t
-000064c0: 6162 6c65 7322 290a 2020 2020 6465 6620  ables").    def 
-000064d0: 7465 7374 5f67 6574 5f74 656d 705f 7461  test_get_temp_ta
-000064e0: 626c 655f 636f 6c75 6d6e 7328 7365 6c66  ble_columns(self
-000064f0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-00006500: 0a20 2020 2064 6566 205f 6173 7365 7274  .    def _assert
-00006510: 5f69 6e73 705f 696e 6465 7865 7328 7365  _insp_indexes(se
-00006520: 6c66 2c20 696e 6465 7865 732c 2065 7870  lf, indexes, exp
-00006530: 6563 7465 645f 696e 6465 7865 7329 3a0a  ected_indexes):.
-00006540: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-00006550: 5f69 6e64 6578 6573 2e73 6f72 7428 6b65  _indexes.sort(ke
-00006560: 793d 6c61 6d62 6461 2069 7465 6d3a 2069  y=lambda item: i
-00006570: 7465 6d5b 226e 616d 6522 5d29 0a0a 2020  tem["name"])..  
-00006580: 2020 2020 2020 696e 6465 785f 6e61 6d65        index_name
-00006590: 7320 3d20 5b64 5b22 6e61 6d65 225d 2066  s = [d["name"] f
-000065a0: 6f72 2064 2069 6e20 696e 6465 7865 735d  or d in indexes]
-000065b0: 0a20 2020 2020 2020 2065 7870 5f69 6e64  .        exp_ind
-000065c0: 6578 5f6e 616d 6573 203d 205b 645b 226e  ex_names = [d["n
-000065d0: 616d 6522 5d20 666f 7220 6420 696e 2065  ame"] for d in e
-000065e0: 7870 6563 7465 645f 696e 6465 7865 735d  xpected_indexes]
-000065f0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00006600: 736f 7274 6564 2869 6e64 6578 5f6e 616d  sorted(index_nam
-00006610: 6573 2920 3d3d 2073 6f72 7465 6428 6578  es) == sorted(ex
-00006620: 705f 696e 6465 785f 6e61 6d65 7329 0a0a  p_index_names)..
-00006630: 0a63 6c61 7373 2043 6f6d 706f 7369 7465  .class Composite
-00006640: 4b65 7952 6566 6c65 6374 696f 6e54 6573  KeyReflectionTes
-00006650: 7428 5f43 6f6d 706f 7369 7465 4b65 7952  t(_CompositeKeyR
-00006660: 6566 6c65 6374 696f 6e54 6573 7429 3a0a  eflectionTest):.
-00006670: 2020 2020 4074 6573 7469 6e67 2e72 6571      @testing.req
-00006680: 7569 7265 732e 666f 7265 6967 6e5f 6b65  uires.foreign_ke
-00006690: 795f 636f 6e73 7472 6169 6e74 5f72 6566  y_constraint_ref
-000066a0: 6c65 6374 696f 6e0a 2020 2020 6465 6620  lection.    def 
-000066b0: 7465 7374 5f66 6b5f 636f 6c75 6d6e 5f6f  test_fk_column_o
-000066c0: 7264 6572 2873 656c 6629 3a0a 2020 2020  rder(self):.    
-000066d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000066e0: 5350 414e 4e45 5220 4f56 4552 5249 4445  SPANNER OVERRIDE
-000066f0: 3a0a 0a20 2020 2020 2020 2053 7061 6e6e  :..        Spann
-00006700: 6572 2063 6f6c 756d 6e20 7573 6167 6520  er column usage 
-00006710: 7265 666c 6563 7469 6f6e 2064 6f65 736e  reflection doesn
-00006720: 2774 2073 7570 706f 7274 2064 6574 6572  't support deter
-00006730: 6d65 6e69 7374 6963 0a20 2020 2020 2020  menistic.       
-00006740: 206f 7264 6572 696e 672e 204f 7665 7272   ordering. Overr
-00006750: 6964 696e 6720 7468 6520 7465 7374 2074  iding the test t
-00006760: 6f20 6368 6563 6b20 7468 6174 2063 6f6c  o check that col
-00006770: 756d 6e73 2061 7265 0a20 2020 2020 2020  umns are.       
-00006780: 2072 6566 6c65 6374 6564 2063 6f72 7265   reflected corre
-00006790: 6374 6c79 2c20 7769 7468 6f75 7420 636f  ctly, without co
-000067a0: 6e73 6964 6572 696e 6720 7468 6569 7220  nsidering their 
-000067b0: 6f72 6465 722e 0a20 2020 2020 2020 2022  order..        "
-000067c0: 2222 0a20 2020 2020 2020 2023 2074 6573  "".        # tes
-000067d0: 7420 666f 7220 6973 7375 6520 2335 3636  t for issue #566
-000067e0: 310a 2020 2020 2020 2020 696e 7370 203d  1.        insp =
-000067f0: 2069 6e73 7065 6374 2873 656c 662e 6269   inspect(self.bi
-00006800: 6e64 290a 2020 2020 2020 2020 666f 7265  nd).        fore
-00006810: 6967 6e5f 6b65 7973 203d 2069 6e73 702e  ign_keys = insp.
-00006820: 6765 745f 666f 7265 6967 6e5f 6b65 7973  get_foreign_keys
-00006830: 2873 656c 662e 7461 626c 6573 2e74 6232  (self.tables.tb2
-00006840: 2e6e 616d 6529 0a20 2020 2020 2020 2065  .name).        e
-00006850: 715f 286c 656e 2866 6f72 6569 676e 5f6b  q_(len(foreign_k
-00006860: 6579 7329 2c20 3129 0a20 2020 2020 2020  eys), 1).       
-00006870: 2066 6b65 7931 203d 2066 6f72 6569 676e   fkey1 = foreign
-00006880: 5f6b 6579 735b 305d 0a20 2020 2020 2020  _keys[0].       
-00006890: 2065 715f 2873 6574 2866 6b65 7931 2e67   eq_(set(fkey1.g
-000068a0: 6574 2822 7265 6665 7272 6564 5f63 6f6c  et("referred_col
-000068b0: 756d 6e73 2229 292c 207b 226e 616d 6522  umns")), {"name"
-000068c0: 2c20 2269 6422 2c20 2261 7474 7222 7d29  , "id", "attr"})
-000068d0: 0a20 2020 2020 2020 2065 715f 2873 6574  .        eq_(set
-000068e0: 2866 6b65 7931 2e67 6574 2822 636f 6e73  (fkey1.get("cons
-000068f0: 7472 6169 6e65 645f 636f 6c75 6d6e 7322  trained_columns"
-00006900: 2929 2c20 7b22 706e 616d 6522 2c20 2270  )), {"pname", "p
-00006910: 6964 222c 2022 7061 7474 7222 7d29 0a0a  id", "pattr"})..
-00006920: 0a40 7079 7465 7374 2e6d 6172 6b2e 736b  .@pytest.mark.sk
-00006930: 6970 2822 5370 616e 6e65 7220 646f 6573  ip("Spanner does
-00006940: 6e27 7420 7375 7070 6f72 7420 7175 6f74  n't support quot
-00006950: 6573 2069 6e20 7461 626c 6520 6e61 6d65  es in table name
-00006960: 732e 2229 0a63 6c61 7373 2051 756f 7465  s.").class Quote
-00006970: 644e 616d 6541 7267 756d 656e 7454 6573  dNameArgumentTes
-00006980: 7428 5f51 756f 7465 644e 616d 6541 7267  t(_QuotedNameArg
-00006990: 756d 656e 7454 6573 7429 3a0a 2020 2020  umentTest):.    
-000069a0: 7061 7373 0a0a 0a63 6c61 7373 205f 4461  pass...class _Da
-000069b0: 7465 4669 7874 7572 6528 5f5f 4461 7465  teFixture(__Date
-000069c0: 4669 7874 7572 6529 3a0a 2020 2020 636f  Fixture):.    co
-000069d0: 6d70 6172 6520 3d20 4e6f 6e65 0a0a 2020  mpare = None..  
-000069e0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-000069f0: 2020 2064 6566 2064 6566 696e 655f 7461     def define_ta
-00006a00: 626c 6573 2863 6c73 2c20 6d65 7461 6461  bles(cls, metada
-00006a10: 7461 293a 0a20 2020 2020 2020 2022 2222  ta):.        """
-00006a20: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
-00006a30: 204f 5645 5252 4944 453a 0a0a 2020 2020   OVERRIDE:..    
-00006a40: 2020 2020 436c 6f75 6420 5370 616e 6e65      Cloud Spanne
-00006a50: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
-00006a60: 7420 6175 746f 2069 6e63 7265 6d65 6e74  t auto increment
-00006a70: 696e 6720 6964 7320 6665 6174 7572 652c  ing ids feature,
-00006a80: 0a20 2020 2020 2020 2077 6869 6368 2069  .        which i
-00006a90: 7320 7573 6564 2062 7920 7468 6520 6f72  s used by the or
-00006aa0: 6967 696e 616c 2074 6573 742e 204f 7665  iginal test. Ove
-00006ab0: 7272 6964 696e 6720 7468 6520 7465 7374  rriding the test
-00006ac0: 2064 6174 610a 2020 2020 2020 2020 6372   data.        cr
-00006ad0: 6561 7469 6f6e 206d 6574 686f 6420 746f  eation method to
-00006ae0: 2064 6973 6162 6c65 2061 7574 6f69 6e63   disable autoinc
-00006af0: 7265 6d65 6e74 2061 6e64 206d 616b 6520  rement and make 
-00006b00: 6964 2063 6f6c 756d 6e0a 2020 2020 2020  id column.      
-00006b10: 2020 6e75 6c6c 6162 6c65 2e0a 2020 2020    nullable..    
-00006b20: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00006b30: 2063 6c61 7373 2044 6563 6f72 6174 6564   class Decorated
-00006b40: 2873 716c 616c 6368 656d 792e 5479 7065  (sqlalchemy.Type
-00006b50: 4465 636f 7261 746f 7229 3a0a 2020 2020  Decorator):.    
-00006b60: 2020 2020 2020 2020 696d 706c 203d 2063          impl = c
-00006b70: 6c73 2e64 6174 6174 7970 650a 2020 2020  ls.datatype.    
-00006b80: 2020 2020 2020 2020 6361 6368 655f 6f6b          cache_ok
-00006b90: 203d 2054 7275 650a 0a20 2020 2020 2020   = True..       
-00006ba0: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
-00006bb0: 2020 2020 2264 6174 655f 7461 626c 6522      "date_table"
-00006bc0: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
-00006bd0: 7461 6461 7461 2c0a 2020 2020 2020 2020  tadata,.        
-00006be0: 2020 2020 436f 6c75 6d6e 2822 6964 222c      Column("id",
-00006bf0: 2049 6e74 6567 6572 2c20 7072 696d 6172   Integer, primar
-00006c00: 795f 6b65 793d 5472 7565 2c20 6e75 6c6c  y_key=True, null
-00006c10: 6162 6c65 3d54 7275 6529 2c0a 2020 2020  able=True),.    
-00006c20: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-00006c30: 6461 7465 5f64 6174 6122 2c20 636c 732e  date_data", cls.
-00006c40: 6461 7461 7479 7065 292c 0a20 2020 2020  datatype),.     
-00006c50: 2020 2020 2020 2043 6f6c 756d 6e28 2264         Column("d
-00006c60: 6563 6f72 6174 6564 5f64 6174 655f 6461  ecorated_date_da
-00006c70: 7461 222c 2044 6563 6f72 6174 6564 292c  ta", Decorated),
-00006c80: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
-00006c90: 7373 2044 6174 6554 6573 7428 5f44 6174  ss DateTest(_Dat
-00006ca0: 6554 6573 7429 3a0a 2020 2020 2222 220a  eTest):.    """.
-00006cb0: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
-00006cc0: 5249 4445 3a0a 0a20 2020 2044 6174 6554  RIDE:..    DateT
-00006cd0: 6573 7420 7465 7374 7320 7573 6564 2073  est tests used s
-00006ce0: 616d 6520 636c 6173 7320 6d65 7468 6f64  ame class method
-00006cf0: 2074 6f20 6372 6561 7465 2074 6162 6c65   to create table
-00006d00: 2c20 736f 2074 6f20 6176 6f69 6420 7468  , so to avoid th
-00006d10: 6f73 6520 6661 696c 7572 6573 0a20 2020  ose failures.   
-00006d20: 2061 6e64 206d 6169 6e74 6169 6e20 4452   and maintain DR
-00006d30: 5920 636f 6e63 6570 7420 6a75 7374 2069  Y concept just i
-00006d40: 6e68 6572 6974 2074 6865 2063 6c61 7373  nherit the class
-00006d50: 2074 6f20 7275 6e20 7465 7374 7320 7375   to run tests su
-00006d60: 6363 6573 7366 756c 6c79 2e0a 2020 2020  ccessfully..    
-00006d70: 2222 220a 0a20 2020 2040 7079 7465 7374  """..    @pytest
-00006d80: 2e6d 6172 6b2e 736b 6970 6966 280a 2020  .mark.skipif(.  
-00006d90: 2020 2020 2020 626f 6f6c 286f 732e 656e        bool(os.en
-00006da0: 7669 726f 6e2e 6765 7428 2253 5041 4e4e  viron.get("SPANN
-00006db0: 4552 5f45 4d55 4c41 544f 525f 484f 5354  ER_EMULATOR_HOST
-00006dc0: 2229 292c 2072 6561 736f 6e3d 2253 6b69  ")), reason="Ski
-00006dd0: 7070 6564 206f 6e20 656d 756c 6174 6f72  pped on emulator
-00006de0: 220a 2020 2020 290a 2020 2020 6465 6620  ".    ).    def 
-00006df0: 7465 7374 5f6e 756c 6c5f 626f 756e 645f  test_null_bound_
-00006e00: 636f 6d70 6172 6973 6f6e 2873 656c 6629  comparison(self)
-00006e10: 3a0a 2020 2020 2020 2020 7375 7065 7228  :.        super(
-00006e20: 292e 7465 7374 5f6e 756c 6c5f 626f 756e  ).test_null_boun
-00006e30: 645f 636f 6d70 6172 6973 6f6e 2829 0a0a  d_comparison()..
-00006e40: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00006e50: 2e73 6b69 7069 6628 0a20 2020 2020 2020  .skipif(.       
-00006e60: 2062 6f6f 6c28 6f73 2e65 6e76 6972 6f6e   bool(os.environ
-00006e70: 2e67 6574 2822 5350 414e 4e45 525f 454d  .get("SPANNER_EM
-00006e80: 554c 4154 4f52 5f48 4f53 5422 2929 2c20  ULATOR_HOST")), 
-00006e90: 7265 6173 6f6e 3d22 536b 6970 7065 6420  reason="Skipped 
-00006ea0: 6f6e 2065 6d75 6c61 746f 7222 0a20 2020  on emulator".   
-00006eb0: 2029 0a20 2020 2064 6566 2074 6573 745f   ).    def test_
-00006ec0: 6e75 6c6c 2873 656c 662c 2063 6f6e 6e65  null(self, conne
-00006ed0: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
-00006ee0: 7375 7065 7228 292e 7465 7374 5f6e 756c  super().test_nul
-00006ef0: 6c28 636f 6e6e 6563 7469 6f6e 290a 0a0a  l(connection)...
-00006f00: 636c 6173 7320 4354 4554 6573 7428 5f43  class CTETest(_C
-00006f10: 5445 5465 7374 293a 0a20 2020 2040 636c  TETest):.    @cl
-00006f20: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-00006f30: 6620 6465 6669 6e65 5f74 6162 6c65 7328  f define_tables(
-00006f40: 636c 732c 206d 6574 6164 6174 6129 3a0a  cls, metadata):.
-00006f50: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00006f60: 2020 2020 5468 6520 6f72 6967 696e 616c      The original
-00006f70: 206d 6574 686f 6420 6372 6561 7465 7320   method creates 
-00006f80: 6120 666f 7265 6967 6e20 6b65 7920 7769  a foreign key wi
-00006f90: 7468 6f75 7420 6120 6e61 6d65 2c0a 2020  thout a name,.  
-00006fa0: 2020 2020 2020 7768 6963 6820 6361 7573        which caus
-00006fb0: 6573 2074 726f 7562 6c65 7320 6f6e 2074  es troubles on t
-00006fc0: 6573 7420 636c 6561 6e75 702e 204f 7665  est cleanup. Ove
-00006fd0: 7272 6964 696e 6720 7468 650a 2020 2020  rriding the.    
-00006fe0: 2020 2020 6d65 7468 6f64 2074 6f20 6578      method to ex
-00006ff0: 706c 6963 6974 6c79 2073 6574 2061 2066  plicitly set a f
-00007000: 6f72 6569 676e 206b 6579 206e 616d 652e  oreign key name.
-00007010: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00007020: 2020 2020 2054 6162 6c65 280a 2020 2020       Table(.    
-00007030: 2020 2020 2020 2020 2273 6f6d 655f 7461          "some_ta
-00007040: 626c 6522 2c0a 2020 2020 2020 2020 2020  ble",.          
-00007050: 2020 6d65 7461 6461 7461 2c0a 2020 2020    metadata,.    
-00007060: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-00007070: 6964 222c 2049 6e74 6567 6572 2c20 7072  id", Integer, pr
-00007080: 696d 6172 795f 6b65 793d 5472 7565 292c  imary_key=True),
-00007090: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-000070a0: 756d 6e28 2264 6174 6122 2c20 5374 7269  umn("data", Stri
-000070b0: 6e67 2835 3029 292c 0a20 2020 2020 2020  ng(50)),.       
-000070c0: 2020 2020 2043 6f6c 756d 6e28 2270 6172       Column("par
-000070d0: 656e 745f 6964 222c 2046 6f72 6569 676e  ent_id", Foreign
-000070e0: 4b65 7928 2273 6f6d 655f 7461 626c 652e  Key("some_table.
-000070f0: 6964 222c 206e 616d 653d 2266 6b5f 736f  id", name="fk_so
-00007100: 6d65 5f74 6162 6c65 2229 292c 0a20 2020  me_table")),.   
-00007110: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00007120: 5461 626c 6528 0a20 2020 2020 2020 2020  Table(.         
-00007130: 2020 2022 736f 6d65 5f6f 7468 6572 5f74     "some_other_t
-00007140: 6162 6c65 222c 0a20 2020 2020 2020 2020  able",.         
-00007150: 2020 206d 6574 6164 6174 612c 0a20 2020     metadata,.   
-00007160: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00007170: 2269 6422 2c20 496e 7465 6765 722c 2070  "id", Integer, p
-00007180: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
-00007190: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
-000071a0: 6c75 6d6e 2822 6461 7461 222c 2053 7472  lumn("data", Str
-000071b0: 696e 6728 3530 2929 2c0a 2020 2020 2020  ing(50)),.      
-000071c0: 2020 2020 2020 436f 6c75 6d6e 2822 7061        Column("pa
-000071d0: 7265 6e74 5f69 6422 2c20 496e 7465 6765  rent_id", Intege
-000071e0: 7229 2c0a 2020 2020 2020 2020 290a 0a20  r),.        ).. 
-000071f0: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-00007200: 736b 6970 2822 494e 5345 5254 2066 726f  skip("INSERT fro
-00007210: 6d20 5749 5448 2073 7562 7175 6572 7920  m WITH subquery 
-00007220: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
-00007230: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
-00007240: 696e 7365 7274 5f66 726f 6d5f 7365 6c65  insert_from_sele
-00007250: 6374 5f72 6f75 6e64 5f74 7269 7028 7365  ct_round_trip(se
-00007260: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00007270: 0a20 2020 2020 2020 2054 6865 2074 6573  .        The tes
-00007280: 7420 6368 6563 6b73 2069 6620 616e 2049  t checks if an I
-00007290: 4e53 4552 5420 6361 6e20 6265 2064 6f6e  NSERT can be don
-000072a0: 6520 6672 6f6d 2061 2063 7465 2c20 6c69  e from a cte, li
-000072b0: 6b65 3a0a 0a20 2020 2020 2020 2057 4954  ke:..        WIT
-000072c0: 4820 736f 6d65 5f63 7465 2041 5320 282e  H some_cte AS (.
-000072d0: 2e2e 290a 2020 2020 2020 2020 494e 5345  ..).        INSE
-000072e0: 5254 2049 4e54 4f20 736f 6d65 5f6f 7468  RT INTO some_oth
-000072f0: 6572 5f74 6162 6c65 2028 2e2e 2e20 5345  er_table (... SE
-00007300: 4c45 4354 202a 2046 524f 4d20 736f 6d65  LECT * FROM some
-00007310: 5f63 7465 290a 0a20 2020 2020 2020 2053  _cte)..        S
-00007320: 7563 6820 7175 6572 6965 7320 6172 6520  uch queries are 
-00007330: 6e6f 7420 7375 7070 6f72 7465 6420 6279  not supported by
-00007340: 2053 7061 6e6e 6572 2e0a 2020 2020 2020   Spanner..      
-00007350: 2020 2222 220a 2020 2020 2020 2020 7061    """.        pa
-00007360: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
-00007370: 6d61 726b 2e73 6b69 7028 2244 454c 4554  mark.skip("DELET
-00007380: 4520 6672 6f6d 2057 4954 4820 7375 6271  E from WITH subq
-00007390: 7565 7279 2069 7320 6e6f 7420 7375 7070  uery is not supp
-000073a0: 6f72 7465 6422 290a 2020 2020 6465 6620  orted").    def 
-000073b0: 7465 7374 5f64 656c 6574 655f 7363 616c  test_delete_scal
-000073c0: 6172 5f73 7562 715f 726f 756e 645f 7472  ar_subq_round_tr
-000073d0: 6970 2873 656c 6629 3a0a 2020 2020 2020  ip(self):.      
-000073e0: 2020 2222 220a 2020 2020 2020 2020 5468    """.        Th
-000073f0: 6520 7465 7374 2063 6865 636b 7320 6966  e test checks if
-00007400: 2061 2044 454c 4554 4520 6361 6e20 6265   a DELETE can be
-00007410: 2064 6f6e 6520 6672 6f6d 2061 2063 7465   done from a cte
-00007420: 2c20 6c69 6b65 3a0a 0a20 2020 2020 2020  , like:..       
-00007430: 2057 4954 4820 736f 6d65 5f63 7465 2041   WITH some_cte A
-00007440: 5320 282e 2e2e 290a 2020 2020 2020 2020  S (...).        
-00007450: 4445 4c45 5445 2046 524f 4d20 736f 6d65  DELETE FROM some
-00007460: 5f6f 7468 6572 5f74 6162 6c65 2028 2e2e  _other_table (..
-00007470: 2e20 5345 4c45 4354 202a 2046 524f 4d20  . SELECT * FROM 
-00007480: 736f 6d65 5f63 7465 290a 0a20 2020 2020  some_cte)..     
-00007490: 2020 2053 7563 6820 7175 6572 6965 7320     Such queries 
-000074a0: 6172 6520 6e6f 7420 7375 7070 6f72 7465  are not supporte
-000074b0: 6420 6279 2053 7061 6e6e 6572 2e0a 2020  d by Spanner..  
-000074c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000074d0: 2020 7061 7373 0a0a 2020 2020 4070 7974    pass..    @pyt
-000074e0: 6573 742e 6d61 726b 2e73 6b69 7028 2244  est.mark.skip("D
-000074f0: 454c 4554 4520 6672 6f6d 2057 4954 4820  ELETE from WITH 
-00007500: 7375 6271 7565 7279 2069 7320 6e6f 7420  subquery is not 
-00007510: 7375 7070 6f72 7465 6422 290a 2020 2020  supported").    
-00007520: 6465 6620 7465 7374 5f64 656c 6574 655f  def test_delete_
-00007530: 6672 6f6d 5f72 6f75 6e64 5f74 7269 7028  from_round_trip(
-00007540: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00007550: 2222 0a20 2020 2020 2020 2054 6865 2074  "".        The t
-00007560: 6573 7420 6368 6563 6b73 2069 6620 6120  est checks if a 
-00007570: 4445 4c45 5445 2063 616e 2062 6520 646f  DELETE can be do
-00007580: 6e65 2066 726f 6d20 6120 6374 652c 206c  ne from a cte, l
-00007590: 696b 653a 0a0a 2020 2020 2020 2020 5749  ike:..        WI
-000075a0: 5448 2073 6f6d 655f 6374 6520 4153 2028  TH some_cte AS (
-000075b0: 2e2e 2e29 0a20 2020 2020 2020 2044 454c  ...).        DEL
-000075c0: 4554 4520 4652 4f4d 2073 6f6d 655f 6f74  ETE FROM some_ot
-000075d0: 6865 725f 7461 626c 6520 282e 2e2e 2053  her_table (... S
-000075e0: 454c 4543 5420 2a20 4652 4f4d 2073 6f6d  ELECT * FROM som
-000075f0: 655f 6374 6529 0a0a 2020 2020 2020 2020  e_cte)..        
-00007600: 5375 6368 2071 7565 7269 6573 2061 7265  Such queries are
-00007610: 206e 6f74 2073 7570 706f 7274 6564 2062   not supported b
-00007620: 7920 5370 616e 6e65 722e 0a20 2020 2020  y Spanner..     
-00007630: 2020 2022 2222 0a20 2020 2020 2020 2070     """.        p
-00007640: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
-00007650: 2e6d 6172 6b2e 736b 6970 2822 5550 4441  .mark.skip("UPDA
-00007660: 5445 2066 726f 6d20 5749 5448 2073 7562  TE from WITH sub
-00007670: 7175 6572 7920 6973 206e 6f74 2073 7570  query is not sup
-00007680: 706f 7274 6564 2229 0a20 2020 2064 6566  ported").    def
-00007690: 2074 6573 745f 7570 6461 7465 5f66 726f   test_update_fro
-000076a0: 6d5f 726f 756e 645f 7472 6970 2873 656c  m_round_trip(sel
-000076b0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-000076c0: 2020 2020 2020 2020 5468 6520 7465 7374          The test
-000076d0: 2063 6865 636b 7320 6966 2061 6e20 5550   checks if an UP
-000076e0: 4441 5445 2063 616e 2062 6520 646f 6e65  DATE can be done
-000076f0: 2066 726f 6d20 6120 6374 652c 206c 696b   from a cte, lik
-00007700: 653a 0a0a 2020 2020 2020 2020 5749 5448  e:..        WITH
-00007710: 2073 6f6d 655f 6374 6520 4153 2028 2e2e   some_cte AS (..
-00007720: 2e29 0a20 2020 2020 2020 2055 5044 4154  .).        UPDAT
-00007730: 4520 736f 6d65 5f6f 7468 6572 5f74 6162  E some_other_tab
-00007740: 6c65 0a20 2020 2020 2020 2053 4554 2028  le.        SET (
-00007750: 2e2e 2e20 5345 4c45 4354 202a 2046 524f  ... SELECT * FRO
-00007760: 4d20 736f 6d65 5f63 7465 290a 0a20 2020  M some_cte)..   
-00007770: 2020 2020 2053 7563 6820 7175 6572 6965       Such querie
-00007780: 7320 6172 6520 6e6f 7420 7375 7070 6f72  s are not suppor
-00007790: 7465 6420 6279 2053 7061 6e6e 6572 2e0a  ted by Spanner..
-000077a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000077b0: 2020 2020 7061 7373 0a0a 2020 2020 4070      pass..    @p
-000077c0: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
-000077d0: 2257 4954 4820 5245 4355 5253 4956 4520  "WITH RECURSIVE 
-000077e0: 7375 6271 7565 7269 6573 2061 7265 206e  subqueries are n
-000077f0: 6f74 2073 7570 706f 7274 6564 2229 0a20  ot supported"). 
-00007800: 2020 2064 6566 2074 6573 745f 7365 6c65     def test_sele
-00007810: 6374 5f72 6563 7572 7369 7665 5f72 6f75  ct_recursive_rou
-00007820: 6e64 5f74 7269 7028 7365 6c66 293a 0a20  nd_trip(self):. 
-00007830: 2020 2020 2020 2070 6173 730a 0a0a 636c         pass...cl
-00007840: 6173 7320 4461 7465 5469 6d65 4d69 6372  ass DateTimeMicr
-00007850: 6f73 6563 6f6e 6473 5465 7374 285f 4461  osecondsTest(_Da
-00007860: 7465 5469 6d65 4d69 6372 6f73 6563 6f6e  teTimeMicrosecon
-00007870: 6473 5465 7374 2c20 4461 7465 5465 7374  dsTest, DateTest
-00007880: 293a 0a20 2020 2040 7079 7465 7374 2e6d  ):.    @pytest.m
-00007890: 6172 6b2e 736b 6970 2822 5370 616e 6e65  ark.skip("Spanne
-000078a0: 7220 6461 7465 7320 6172 6520 7469 6d65  r dates are time
-000078b0: 207a 6f6e 6520 696e 6465 7065 6e64 656e   zone independen
-000078c0: 7422 290a 2020 2020 6465 6620 7465 7374  t").    def test
-000078d0: 5f73 656c 6563 745f 6469 7265 6374 2873  _select_direct(s
-000078e0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-000078f0: 7373 0a0a 2020 2020 6465 6620 7465 7374  ss..    def test
-00007900: 5f72 6f75 6e64 5f74 7269 7028 7365 6c66  _round_trip(self
-00007910: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00007920: 2020 2020 2020 2053 5041 4e4e 4552 204f         SPANNER O
-00007930: 5645 5252 4944 453a 0a0a 2020 2020 2020  VERRIDE:..      
-00007940: 2020 5370 616e 6e65 7220 636f 6e76 6572    Spanner conver
-00007950: 7473 2074 696d 6573 7461 6d70 2069 6e74  ts timestamp int
-00007960: 6f20 6025 592d 256d 2d25 6454 2548 3a25  o `%Y-%m-%dT%H:%
-00007970: 4d3a 2553 2e25 665a 6020 666f 726d 6174  M:%S.%fZ` format
-00007980: 2c20 736f 2074 6f20 6176 6f69 640a 2020  , so to avoid.  
-00007990: 2020 2020 2020 6173 7365 7274 2066 6169        assert fai
-000079a0: 6c75 7265 7320 636f 6e76 6572 7420 6461  lures convert da
-000079b0: 7465 7469 6d65 2069 6e70 7574 2074 6f20  tetime input to 
-000079c0: 7468 6520 6465 7369 7265 2074 696d 6573  the desire times
-000079d0: 7461 6d70 2066 6f72 6d61 742e 0a20 2020  tamp format..   
-000079e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000079f0: 2064 6174 655f 7461 626c 6520 3d20 7365   date_table = se
-00007a00: 6c66 2e74 6162 6c65 732e 6461 7465 5f74  lf.tables.date_t
-00007a10: 6162 6c65 0a20 2020 2020 2020 2063 6f6e  able.        con
-00007a20: 6669 672e 6462 2e65 7865 6375 7465 2864  fig.db.execute(d
-00007a30: 6174 655f 7461 626c 652e 696e 7365 7274  ate_table.insert
-00007a40: 2829 2c20 7b22 6461 7465 5f64 6174 6122  (), {"date_data"
-00007a50: 3a20 7365 6c66 2e64 6174 612c 2022 6964  : self.data, "id
-00007a60: 223a 2032 3530 7d29 0a0a 2020 2020 2020  ": 250})..      
-00007a70: 2020 726f 7720 3d20 636f 6e66 6967 2e64    row = config.d
-00007a80: 622e 6578 6563 7574 6528 7365 6c65 6374  b.execute(select
-00007a90: 285b 6461 7465 5f74 6162 6c65 2e63 2e64  ([date_table.c.d
-00007aa0: 6174 655f 6461 7461 5d29 292e 6669 7273  ate_data])).firs
-00007ab0: 7428 290a 2020 2020 2020 2020 636f 6d70  t().        comp
-00007ac0: 6172 6520 3d20 7365 6c66 2e63 6f6d 7061  are = self.compa
-00007ad0: 7265 206f 7220 7365 6c66 2e64 6174 610a  re or self.data.
-00007ae0: 2020 2020 2020 2020 636f 6d70 6172 6520          compare 
-00007af0: 3d20 636f 6d70 6172 652e 7374 7266 7469  = compare.strfti
-00007b00: 6d65 2822 2559 2d25 6d2d 2564 5425 483a  me("%Y-%m-%dT%H:
-00007b10: 254d 3a25 532e 2566 5a22 290a 2020 2020  %M:%S.%fZ").    
-00007b20: 2020 2020 6571 5f28 726f 775b 305d 2e72      eq_(row[0].r
-00007b30: 6663 3333 3339 2829 2c20 636f 6d70 6172  fc3339(), compar
-00007b40: 6529 0a20 2020 2020 2020 2061 7373 6572  e).        asser
-00007b50: 7420 6973 696e 7374 616e 6365 2872 6f77  t isinstance(row
-00007b60: 5b30 5d2c 2044 6174 6574 696d 6557 6974  [0], DatetimeWit
-00007b70: 684e 616e 6f73 6563 6f6e 6473 290a 0a20  hNanoseconds).. 
-00007b80: 2020 2064 6566 2074 6573 745f 726f 756e     def test_roun
-00007b90: 645f 7472 6970 5f64 6563 6f72 6174 6564  d_trip_decorated
-00007ba0: 2873 656c 662c 2063 6f6e 6e65 6374 696f  (self, connectio
-00007bb0: 6e29 3a0a 2020 2020 2020 2020 2222 220a  n):.        """.
-00007bc0: 2020 2020 2020 2020 5350 414e 4e45 5220          SPANNER 
-00007bd0: 4f56 4552 5249 4445 3a0a 0a20 2020 2020  OVERRIDE:..     
-00007be0: 2020 2053 7061 6e6e 6572 2063 6f6e 7665     Spanner conve
-00007bf0: 7274 7320 7469 6d65 7374 616d 7020 696e  rts timestamp in
-00007c00: 746f 2060 2559 2d25 6d2d 2564 5425 483a  to `%Y-%m-%dT%H:
-00007c10: 254d 3a25 532e 2566 5a60 2066 6f72 6d61  %M:%S.%fZ` forma
-00007c20: 742c 2073 6f20 746f 2061 766f 6964 0a20  t, so to avoid. 
-00007c30: 2020 2020 2020 2061 7373 6572 7420 6661         assert fa
-00007c40: 696c 7572 6573 2063 6f6e 7665 7274 2064  ilures convert d
-00007c50: 6174 6574 696d 6520 696e 7075 7420 746f  atetime input to
-00007c60: 2074 6865 2064 6573 6972 6520 7469 6d65   the desire time
-00007c70: 7374 616d 7020 666f 726d 6174 2e0a 2020  stamp format..  
-00007c80: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00007c90: 2020 6461 7465 5f74 6162 6c65 203d 2073    date_table = s
-00007ca0: 656c 662e 7461 626c 6573 2e64 6174 655f  elf.tables.date_
-00007cb0: 7461 626c 650a 0a20 2020 2020 2020 2063  table..        c
-00007cc0: 6f6e 6e65 6374 696f 6e2e 6578 6563 7574  onnection.execut
-00007cd0: 6528 0a20 2020 2020 2020 2020 2020 2064  e(.            d
-00007ce0: 6174 655f 7461 626c 652e 696e 7365 7274  ate_table.insert
-00007cf0: 2829 2c20 7b22 6964 223a 2031 2c20 2264  (), {"id": 1, "d
-00007d00: 6563 6f72 6174 6564 5f64 6174 655f 6461  ecorated_date_da
-00007d10: 7461 223a 2073 656c 662e 6461 7461 7d0a  ta": self.data}.
-00007d20: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00007d30: 2020 2072 6f77 203d 2063 6f6e 6e65 6374     row = connect
-00007d40: 696f 6e2e 6578 6563 7574 6528 7365 6c65  ion.execute(sele
-00007d50: 6374 2864 6174 655f 7461 626c 652e 632e  ct(date_table.c.
-00007d60: 6465 636f 7261 7465 645f 6461 7465 5f64  decorated_date_d
-00007d70: 6174 6129 292e 6669 7273 7428 290a 0a20  ata)).first().. 
-00007d80: 2020 2020 2020 2063 6f6d 7061 7265 203d         compare =
-00007d90: 2073 656c 662e 636f 6d70 6172 6520 6f72   self.compare or
-00007da0: 2073 656c 662e 6461 7461 0a20 2020 2020   self.data.     
-00007db0: 2020 2063 6f6d 7061 7265 203d 2063 6f6d     compare = com
-00007dc0: 7061 7265 2e73 7472 6674 696d 6528 2225  pare.strftime("%
-00007dd0: 592d 256d 2d25 6454 2548 3a25 4d3a 2553  Y-%m-%dT%H:%M:%S
-00007de0: 2e25 665a 2229 0a20 2020 2020 2020 2065  .%fZ").        e
-00007df0: 715f 2872 6f77 5b30 5d2e 7266 6333 3333  q_(row[0].rfc333
-00007e00: 3928 292c 2063 6f6d 7061 7265 290a 2020  9(), compare).  
-00007e10: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
-00007e20: 6e73 7461 6e63 6528 726f 775b 305d 2c20  nstance(row[0], 
-00007e30: 4461 7465 7469 6d65 5769 7468 4e61 6e6f  DatetimeWithNano
-00007e40: 7365 636f 6e64 7329 0a0a 2020 2020 4070  seconds)..    @p
-00007e50: 7974 6573 742e 6d61 726b 2e73 6b69 7069  ytest.mark.skipi
-00007e60: 6628 0a20 2020 2020 2020 2062 6f6f 6c28  f(.        bool(
-00007e70: 6f73 2e65 6e76 6972 6f6e 2e67 6574 2822  os.environ.get("
-00007e80: 5350 414e 4e45 525f 454d 554c 4154 4f52  SPANNER_EMULATOR
-00007e90: 5f48 4f53 5422 2929 2c20 7265 6173 6f6e  _HOST")), reason
-00007ea0: 3d22 536b 6970 7065 6420 6f6e 2065 6d75  ="Skipped on emu
-00007eb0: 6c61 746f 7222 0a20 2020 2029 0a20 2020  lator".    ).   
-00007ec0: 2064 6566 2074 6573 745f 6e75 6c6c 5f62   def test_null_b
-00007ed0: 6f75 6e64 5f63 6f6d 7061 7269 736f 6e28  ound_comparison(
-00007ee0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-00007ef0: 7570 6572 2829 2e74 6573 745f 6e75 6c6c  uper().test_null
-00007f00: 5f62 6f75 6e64 5f63 6f6d 7061 7269 736f  _bound_compariso
-00007f10: 6e28 290a 0a20 2020 2040 7079 7465 7374  n()..    @pytest
-00007f20: 2e6d 6172 6b2e 736b 6970 6966 280a 2020  .mark.skipif(.  
-00007f30: 2020 2020 2020 626f 6f6c 286f 732e 656e        bool(os.en
-00007f40: 7669 726f 6e2e 6765 7428 2253 5041 4e4e  viron.get("SPANN
-00007f50: 4552 5f45 4d55 4c41 544f 525f 484f 5354  ER_EMULATOR_HOST
-00007f60: 2229 292c 2072 6561 736f 6e3d 2253 6b69  ")), reason="Ski
-00007f70: 7070 6564 206f 6e20 656d 756c 6174 6f72  pped on emulator
-00007f80: 220a 2020 2020 290a 2020 2020 6465 6620  ".    ).    def 
-00007f90: 7465 7374 5f6e 756c 6c28 7365 6c66 2c20  test_null(self, 
-00007fa0: 636f 6e6e 6563 7469 6f6e 293a 0a20 2020  connection):.   
-00007fb0: 2020 2020 2073 7570 6572 2829 2e74 6573       super().tes
-00007fc0: 745f 6e75 6c6c 2863 6f6e 6e65 6374 696f  t_null(connectio
-00007fd0: 6e29 0a0a 0a63 6c61 7373 2044 6174 6554  n)...class DateT
-00007fe0: 696d 6554 6573 7428 5f44 6174 6554 696d  imeTest(_DateTim
-00007ff0: 6554 6573 742c 2044 6174 6554 696d 654d  eTest, DateTimeM
-00008000: 6963 726f 7365 636f 6e64 7354 6573 7429  icrosecondsTest)
-00008010: 3a0a 2020 2020 2222 220a 2020 2020 5350  :.    """.    SP
-00008020: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
-00008030: 0a20 2020 2044 6174 6554 696d 6554 6573  .    DateTimeTes
-00008040: 7420 7465 7374 7320 6861 7665 2074 6865  t tests have the
-00008050: 2073 616d 6520 6661 696c 7572 6573 2073   same failures s
-00008060: 616d 6520 6173 2044 6174 6554 696d 654d  ame as DateTimeM
-00008070: 6963 726f 7365 636f 6e64 7354 6573 7420  icrosecondsTest 
-00008080: 7465 7374 732c 0a20 2020 2073 6f20 746f  tests,.    so to
-00008090: 2061 766f 6964 2074 686f 7365 2066 6169   avoid those fai
-000080a0: 6c75 7265 7320 616e 6420 6d61 696e 7461  lures and mainta
-000080b0: 696e 2044 5259 2063 6f6e 6365 7074 206a  in DRY concept j
-000080c0: 7573 7420 696e 6865 7269 7420 7468 6520  ust inherit the 
-000080d0: 636c 6173 7320 746f 2072 756e 0a20 2020  class to run.   
-000080e0: 2074 6573 7473 2073 7563 6365 7373 6675   tests successfu
-000080f0: 6c6c 792e 0a20 2020 2022 2222 0a0a 2020  lly..    """..  
-00008100: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-00008110: 6b69 7069 6628 0a20 2020 2020 2020 2062  kipif(.        b
-00008120: 6f6f 6c28 6f73 2e65 6e76 6972 6f6e 2e67  ool(os.environ.g
-00008130: 6574 2822 5350 414e 4e45 525f 454d 554c  et("SPANNER_EMUL
-00008140: 4154 4f52 5f48 4f53 5422 2929 2c20 7265  ATOR_HOST")), re
-00008150: 6173 6f6e 3d22 536b 6970 7065 6420 6f6e  ason="Skipped on
-00008160: 2065 6d75 6c61 746f 7222 0a20 2020 2029   emulator".    )
-00008170: 0a20 2020 2064 6566 2074 6573 745f 6e75  .    def test_nu
-00008180: 6c6c 5f62 6f75 6e64 5f63 6f6d 7061 7269  ll_bound_compari
-00008190: 736f 6e28 7365 6c66 293a 0a20 2020 2020  son(self):.     
-000081a0: 2020 2073 7570 6572 2829 2e74 6573 745f     super().test_
-000081b0: 6e75 6c6c 5f62 6f75 6e64 5f63 6f6d 7061  null_bound_compa
-000081c0: 7269 736f 6e28 290a 0a20 2020 2040 7079  rison()..    @py
-000081d0: 7465 7374 2e6d 6172 6b2e 736b 6970 6966  test.mark.skipif
-000081e0: 280a 2020 2020 2020 2020 626f 6f6c 286f  (.        bool(o
-000081f0: 732e 656e 7669 726f 6e2e 6765 7428 2253  s.environ.get("S
-00008200: 5041 4e4e 4552 5f45 4d55 4c41 544f 525f  PANNER_EMULATOR_
-00008210: 484f 5354 2229 292c 2072 6561 736f 6e3d  HOST")), reason=
-00008220: 2253 6b69 7070 6564 206f 6e20 656d 756c  "Skipped on emul
-00008230: 6174 6f72 220a 2020 2020 290a 2020 2020  ator".    ).    
-00008240: 6465 6620 7465 7374 5f6e 756c 6c28 7365  def test_null(se
-00008250: 6c66 2c20 636f 6e6e 6563 7469 6f6e 293a  lf, connection):
-00008260: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00008270: 2e74 6573 745f 6e75 6c6c 2863 6f6e 6e65  .test_null(conne
-00008280: 6374 696f 6e29 0a0a 2020 2020 4070 7974  ction)..    @pyt
-00008290: 6573 742e 6d61 726b 2e73 6b69 7028 2253  est.mark.skip("S
-000082a0: 7061 6e6e 6572 2064 6174 6573 2061 7265  panner dates are
-000082b0: 2074 696d 6520 7a6f 6e65 2069 6e64 6570   time zone indep
-000082c0: 656e 6465 6e74 2229 0a20 2020 2064 6566  endent").    def
-000082d0: 2074 6573 745f 7365 6c65 6374 5f64 6972   test_select_dir
-000082e0: 6563 7428 7365 6c66 293a 0a20 2020 2020  ect(self):.     
-000082f0: 2020 2070 6173 730a 0a0a 4070 7974 6573     pass...@pytes
-00008300: 742e 6d61 726b 2e73 6b69 7028 224e 6f74  t.mark.skip("Not
-00008310: 2073 7570 706f 7274 6564 2062 7920 5370   supported by Sp
-00008320: 616e 6e65 7222 290a 636c 6173 7320 4469  anner").class Di
-00008330: 6666 6963 756c 7450 6172 616d 6574 6572  fficultParameter
-00008340: 7354 6573 7428 5f44 6966 6669 6375 6c74  sTest(_Difficult
-00008350: 5061 7261 6d65 7465 7273 5465 7374 293a  ParametersTest):
-00008360: 0a20 2020 2070 6173 730a 0a0a 636c 6173  .    pass...clas
-00008370: 7320 4665 7463 684c 696d 6974 4f66 6673  s FetchLimitOffs
-00008380: 6574 5465 7374 285f 4665 7463 684c 696d  etTest(_FetchLim
-00008390: 6974 4f66 6673 6574 5465 7374 293a 0a20  itOffsetTest):. 
-000083a0: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-000083b0: 736b 6970 2822 5370 616e 6e65 7220 646f  skip("Spanner do
-000083c0: 6573 6e27 7420 7375 7070 6f72 7420 636f  esn't support co
-000083d0: 6d70 6f73 6974 6520 4c49 4d49 5420 616e  mposite LIMIT an
-000083e0: 6420 4f46 4653 4554 2063 6c61 7573 6573  d OFFSET clauses
-000083f0: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
-00008400: 6578 7072 5f6c 696d 6974 2873 656c 662c  expr_limit(self,
-00008410: 2063 6f6e 6e65 6374 696f 6e29 3a0a 2020   connection):.  
-00008420: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00008430: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
-00008440: 7028 2253 7061 6e6e 6572 2064 6f65 736e  p("Spanner doesn
-00008450: 2774 2073 7570 706f 7274 2063 6f6d 706f  't support compo
-00008460: 7369 7465 204c 494d 4954 2061 6e64 204f  site LIMIT and O
-00008470: 4646 5345 5420 636c 6175 7365 7322 290a  FFSET clauses").
-00008480: 2020 2020 6465 6620 7465 7374 5f65 7870      def test_exp
-00008490: 725f 6f66 6673 6574 2873 656c 662c 2063  r_offset(self, c
-000084a0: 6f6e 6e65 6374 696f 6e29 3a0a 2020 2020  onnection):.    
-000084b0: 2020 2020 7061 7373 0a0a 2020 2020 4070      pass..    @p
-000084c0: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
-000084d0: 2253 7061 6e6e 6572 2064 6f65 736e 2774  "Spanner doesn't
-000084e0: 2073 7570 706f 7274 2063 6f6d 706f 7369   support composi
-000084f0: 7465 204c 494d 4954 2061 6e64 204f 4646  te LIMIT and OFF
-00008500: 5345 5420 636c 6175 7365 7322 290a 2020  SET clauses").  
-00008510: 2020 6465 6620 7465 7374 5f65 7870 725f    def test_expr_
-00008520: 6c69 6d69 745f 6f66 6673 6574 2873 656c  limit_offset(sel
-00008530: 662c 2063 6f6e 6e65 6374 696f 6e29 3a0a  f, connection):.
-00008540: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00008550: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-00008560: 6b69 7028 2253 7061 6e6e 6572 2064 6f65  kip("Spanner doe
-00008570: 736e 2774 2073 7570 706f 7274 2063 6f6d  sn't support com
-00008580: 706f 7369 7465 204c 494d 4954 2061 6e64  posite LIMIT and
-00008590: 204f 4646 5345 5420 636c 6175 7365 7322   OFFSET clauses"
-000085a0: 290a 2020 2020 6465 6620 7465 7374 5f65  ).    def test_e
-000085b0: 7870 725f 6c69 6d69 745f 7369 6d70 6c65  xpr_limit_simple
-000085c0: 5f6f 6666 7365 7428 7365 6c66 2c20 636f  _offset(self, co
-000085d0: 6e6e 6563 7469 6f6e 293a 0a20 2020 2020  nnection):.     
-000085e0: 2020 2070 6173 730a 0a20 2020 2040 7079     pass..    @py
-000085f0: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
-00008600: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
-00008610: 7375 7070 6f72 7420 636f 6d70 6f73 6974  support composit
-00008620: 6520 4c49 4d49 5420 616e 6420 4f46 4653  e LIMIT and OFFS
-00008630: 4554 2063 6c61 7573 6573 2229 0a20 2020  ET clauses").   
-00008640: 2064 6566 2074 6573 745f 7369 6d70 6c65   def test_simple
-00008650: 5f6c 696d 6974 5f65 7870 725f 6f66 6673  _limit_expr_offs
-00008660: 6574 2873 656c 662c 2063 6f6e 6e65 6374  et(self, connect
-00008670: 696f 6e29 3a0a 2020 2020 2020 2020 7061  ion):.        pa
-00008680: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
-00008690: 6d61 726b 2e73 6b69 7028 2253 7061 6e6e  mark.skip("Spann
-000086a0: 6572 2064 6f65 736e 2774 2073 7570 706f  er doesn't suppo
-000086b0: 7274 2063 6f6d 706f 7369 7465 204c 494d  rt composite LIM
-000086c0: 4954 2061 6e64 204f 4646 5345 5420 636c  IT and OFFSET cl
-000086d0: 6175 7365 7322 290a 2020 2020 6465 6620  auses").    def 
-000086e0: 7465 7374 5f62 6f75 6e64 5f6f 6666 7365  test_bound_offse
-000086f0: 7428 7365 6c66 2c20 636f 6e6e 6563 7469  t(self, connecti
-00008700: 6f6e 293a 0a20 2020 2020 2020 2070 6173  on):.        pas
-00008710: 730a 0a20 2020 2064 6566 2074 6573 745f  s..    def test_
-00008720: 6c69 6d69 745f 7265 6e64 6572 5f6d 756c  limit_render_mul
-00008730: 7469 706c 655f 7469 6d65 7328 7365 6c66  tiple_times(self
-00008740: 2c20 636f 6e6e 6563 7469 6f6e 293a 0a20  , connection):. 
-00008750: 2020 2020 2020 2074 6162 6c65 203d 2073         table = s
-00008760: 656c 662e 7461 626c 6573 2e73 6f6d 655f  elf.tables.some_
-00008770: 7461 626c 650a 2020 2020 2020 2020 7374  table.        st
-00008780: 6d74 203d 2073 656c 6563 7428 7461 626c  mt = select(tabl
-00008790: 652e 632e 6964 292e 6c69 6d69 7428 3129  e.c.id).limit(1)
-000087a0: 2e73 6361 6c61 725f 7375 6271 7565 7279  .scalar_subquery
-000087b0: 2829 0a0a 2020 2020 2020 2020 7520 3d20  ()..        u = 
-000087c0: 756e 696f 6e28 7365 6c65 6374 2873 746d  union(select(stm
-000087d0: 7429 2c20 7365 6c65 6374 2873 746d 7429  t), select(stmt)
-000087e0: 292e 7375 6271 7565 7279 2829 2e73 656c  ).subquery().sel
-000087f0: 6563 7428 290a 0a20 2020 2020 2020 2073  ect()..        s
-00008800: 656c 662e 5f61 7373 6572 745f 7265 7375  elf._assert_resu
-00008810: 6c74 280a 2020 2020 2020 2020 2020 2020  lt(.            
-00008820: 636f 6e6e 6563 7469 6f6e 2c0a 2020 2020  connection,.    
-00008830: 2020 2020 2020 2020 752c 0a20 2020 2020          u,.     
-00008840: 2020 2020 2020 205b 2832 2c29 5d2c 0a20         [(2,)],. 
-00008850: 2020 2020 2020 2029 0a0a 0a40 7079 7465         )...@pyte
-00008860: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
-00008870: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
-00008880: 7070 6f72 7420 6175 746f 696e 6372 656d  pport autoincrem
-00008890: 656e 7422 290a 636c 6173 7320 4964 656e  ent").class Iden
-000088a0: 7469 7479 4175 746f 696e 6372 656d 656e  tityAutoincremen
-000088b0: 7454 6573 7428 5f49 6465 6e74 6974 7941  tTest(_IdentityA
-000088c0: 7574 6f69 6e63 7265 6d65 6e74 5465 7374  utoincrementTest
-000088d0: 293a 0a20 2020 2070 6173 730a 0a0a 636c  ):.    pass...cl
-000088e0: 6173 7320 4573 6361 7069 6e67 5465 7374  ass EscapingTest
-000088f0: 285f 4573 6361 7069 6e67 5465 7374 293a  (_EscapingTest):
-00008900: 0a20 2020 2040 7072 6f76 6964 655f 6d65  .    @provide_me
-00008910: 7461 6461 7461 0a20 2020 2064 6566 2074  tadata.    def t
-00008920: 6573 745f 7065 7263 656e 745f 7369 676e  est_percent_sign
-00008930: 5f72 6f75 6e64 5f74 7269 7028 7365 6c66  _round_trip(self
-00008940: 293a 0a20 2020 2020 2020 2022 2222 5465  ):.        """Te
-00008950: 7374 2074 6861 7420 7468 6520 4442 4150  st that the DBAP
-00008960: 4920 6163 636f 6d6d 6f64 6174 6573 2066  I accommodates f
-00008970: 6f72 2065 7363 6170 6564 202f 206e 6f6e  or escaped / non
-00008980: 6573 6361 7065 640a 2020 2020 2020 2020  escaped.        
-00008990: 7065 7263 656e 7420 7369 676e 7320 696e  percent signs in
-000089a0: 2061 2077 6179 2074 6861 7420 6d61 7463   a way that matc
-000089b0: 6865 7320 7468 6520 636f 6d70 696c 6572  hes the compiler
-000089c0: 0a0a 2020 2020 2020 2020 5350 414e 4e45  ..        SPANNE
-000089d0: 5220 4f56 4552 5249 4445 0a20 2020 2020  R OVERRIDE.     
-000089e0: 2020 2043 6c6f 7564 2053 7061 6e6e 6572     Cloud Spanner
-000089f0: 2073 7570 706f 7274 7320 7461 626c 6573   supports tables
-00008a00: 2077 6974 6820 656d 7074 7920 7072 696d   with empty prim
-00008a10: 6172 7920 6b65 792c 2062 7574 0a20 2020  ary key, but.   
-00008a20: 2020 2020 206f 6e6c 7920 7369 6e67 6c65       only single
-00008a30: 206f 6e65 2072 6f77 2063 616e 2062 6520   one row can be 
-00008a40: 696e 7365 7274 6564 2069 6e74 6f20 7375  inserted into su
-00008a50: 6368 2061 2074 6162 6c65 202d 0a20 2020  ch a table -.   
-00008a60: 2020 2020 2066 6f6c 6c6f 7769 6e67 2069       following i
-00008a70: 6e73 6572 7469 6f6e 7320 7769 6c6c 2066  nsertions will f
-00008a80: 6169 6c20 7769 7468 2060 526f 7720 5b5d  ail with `Row []
-00008a90: 2061 6c72 6561 6479 2065 7869 7374 7322   already exists"
-00008aa0: 2e0a 2020 2020 2020 2020 4f76 6572 7269  ..        Overri
-00008ab0: 6469 6e67 2074 6865 2074 6573 7420 746f  ding the test to
-00008ac0: 2061 766f 6964 2074 6865 2073 616d 6520   avoid the same 
-00008ad0: 6661 696c 7572 652e 0a20 2020 2020 2020  failure..       
-00008ae0: 2022 2222 0a20 2020 2020 2020 206d 203d   """.        m =
-00008af0: 2073 656c 662e 6d65 7461 6461 7461 0a20   self.metadata. 
-00008b00: 2020 2020 2020 2074 203d 2054 6162 6c65         t = Table
-00008b10: 2822 7422 2c20 6d2c 2043 6f6c 756d 6e28  ("t", m, Column(
-00008b20: 2264 6174 6122 2c20 5374 7269 6e67 2835  "data", String(5
-00008b30: 3029 2929 0a20 2020 2020 2020 2074 2e63  0))).        t.c
-00008b40: 7265 6174 6528 636f 6e66 6967 2e64 6229  reate(config.db)
-00008b50: 0a20 2020 2020 2020 2077 6974 6820 636f  .        with co
-00008b60: 6e66 6967 2e64 622e 6265 6769 6e28 2920  nfig.db.begin() 
-00008b70: 6173 2063 6f6e 6e3a 0a20 2020 2020 2020  as conn:.       
-00008b80: 2020 2020 2063 6f6e 6e2e 6578 6563 7574       conn.execut
-00008b90: 6528 742e 696e 7365 7274 2829 2c20 6469  e(t.insert(), di
-00008ba0: 6374 2864 6174 613d 2273 6f6d 6520 2520  ct(data="some % 
-00008bb0: 7661 6c75 6522 2929 0a0a 2020 2020 2020  value"))..      
-00008bc0: 2020 2020 2020 6571 5f28 0a20 2020 2020        eq_(.     
-00008bd0: 2020 2020 2020 2020 2020 2063 6f6e 6e2e             conn.
-00008be0: 7363 616c 6172 280a 2020 2020 2020 2020  scalar(.        
-00008bf0: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
-00008c00: 6374 285b 742e 632e 6461 7461 5d29 2e77  ct([t.c.data]).w
-00008c10: 6865 7265 280a 2020 2020 2020 2020 2020  here(.          
-00008c20: 2020 2020 2020 2020 2020 2020 2020 742e                t.
-00008c30: 632e 6461 7461 203d 3d20 6c69 7465 7261  c.data == litera
-00008c40: 6c5f 636f 6c75 6d6e 2822 2773 6f6d 6520  l_column("'some 
-00008c50: 2520 7661 6c75 6527 2229 0a20 2020 2020  % value'").     
-00008c60: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00008c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008c80: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00008c90: 2020 2020 2273 6f6d 6520 2520 7661 6c75      "some % valu
-00008ca0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00008cb0: 290a 0a20 2020 2020 2020 2020 2020 2063  )..            c
-00008cc0: 6f6e 6e2e 6578 6563 7574 6528 742e 6465  onn.execute(t.de
-00008cd0: 6c65 7465 2829 290a 2020 2020 2020 2020  lete()).        
-00008ce0: 2020 2020 636f 6e6e 2e65 7865 6375 7465      conn.execute
-00008cf0: 2874 2e69 6e73 6572 7428 292c 2064 6963  (t.insert(), dic
-00008d00: 7428 6461 7461 3d22 736f 6d65 2025 2520  t(data="some %% 
-00008d10: 6f74 6865 7220 7661 6c75 6522 2929 0a20  other value")). 
-00008d20: 2020 2020 2020 2020 2020 2065 715f 280a             eq_(.
-00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d40: 636f 6e6e 2e73 6361 6c61 7228 0a20 2020  conn.scalar(.   
-00008d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d60: 2073 656c 6563 7428 5b74 2e63 2e64 6174   select([t.c.dat
-00008d70: 615d 292e 7768 6572 6528 0a20 2020 2020  a]).where(.     
-00008d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d90: 2020 2074 2e63 2e64 6174 6120 3d3d 206c     t.c.data == l
-00008da0: 6974 6572 616c 5f63 6f6c 756d 6e28 2227  iteral_column("'
-00008db0: 736f 6d65 2025 2520 6f74 6865 7220 7661  some %% other va
-00008dc0: 6c75 6527 2229 0a20 2020 2020 2020 2020  lue'").         
-00008dd0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00008de0: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
-00008df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e00: 2273 6f6d 6520 2525 206f 7468 6572 2076  "some %% other v
-00008e10: 616c 7565 222c 0a20 2020 2020 2020 2020  alue",.         
-00008e20: 2020 2029 0a0a 0a63 6c61 7373 2045 7869     )...class Exi
-00008e30: 7374 7354 6573 7428 5f45 7869 7374 7354  stsTest(_ExistsT
-00008e40: 6573 7429 3a0a 2020 2020 6465 6620 7465  est):.    def te
-00008e50: 7374 5f73 656c 6563 745f 6578 6973 7473  st_select_exists
-00008e60: 2873 656c 662c 2063 6f6e 6e65 6374 696f  (self, connectio
-00008e70: 6e29 3a0a 2020 2020 2020 2020 2222 220a  n):.        """.
-00008e80: 2020 2020 2020 2020 5350 414e 4e45 5220          SPANNER 
-00008e90: 4f56 4552 5249 4445 3a0a 0a20 2020 2020  OVERRIDE:..     
-00008ea0: 2020 2054 6865 206f 7269 6769 6e61 6c20     The original 
-00008eb0: 7465 7374 2069 7320 7472 7969 6e67 2074  test is trying t
-00008ec0: 6f20 6578 6563 7574 6520 6120 7175 6572  o execute a quer
-00008ed0: 7920 6c69 6b65 3a0a 0a20 2020 2020 2020  y like:..       
-00008ee0: 2053 454c 4543 5420 2e2e 2e0a 2020 2020   SELECT ....    
-00008ef0: 2020 2020 5748 4552 4520 4558 4953 5453      WHERE EXISTS
-00008f00: 2028 5345 4c45 4354 202e 2e2e 290a 0a20   (SELECT ...).. 
-00008f10: 2020 2020 2020 2053 454c 4543 5420 5748         SELECT WH
-00008f20: 4552 4520 7769 7468 6f75 7420 4652 4f4d  ERE without FROM
-00008f30: 2063 6c61 7573 6520 6973 206e 6f74 2073   clause is not s
-00008f40: 7570 706f 7274 6564 2062 7920 5370 616e  upported by Span
-00008f50: 6e65 722e 0a20 2020 2020 2020 2052 6577  ner..        Rew
-00008f60: 7269 7469 6e67 2074 6865 2074 6573 7420  riting the test 
-00008f70: 746f 2066 6f72 6365 2069 7420 746f 2067  to force it to g
-00008f80: 656e 6572 6174 6520 6120 7175 6572 7920  enerate a query 
-00008f90: 6c69 6b65 3a0a 0a20 2020 2020 2020 2053  like:..        S
-00008fa0: 454c 4543 5420 4558 4953 5453 2028 5345  ELECT EXISTS (SE
-00008fb0: 4c45 4354 202e 2e2e 290a 2020 2020 2020  LECT ...).      
-00008fc0: 2020 2222 220a 2020 2020 2020 2020 7374    """.        st
-00008fd0: 7566 6620 3d20 7365 6c66 2e74 6162 6c65  uff = self.table
-00008fe0: 732e 7374 7566 660a 2020 2020 2020 2020  s.stuff.        
-00008ff0: 6571 5f28 0a20 2020 2020 2020 2020 2020  eq_(.           
-00009000: 2063 6f6e 6e65 6374 696f 6e2e 6578 6563   connection.exec
-00009010: 7574 6528 0a20 2020 2020 2020 2020 2020  ute(.           
-00009020: 2020 2020 2073 656c 6563 7428 2865 7869       select((exi
-00009030: 7374 7328 292e 7768 6572 6528 7374 7566  sts().where(stuf
-00009040: 662e 632e 6461 7461 203d 3d20 2273 6f6d  f.c.data == "som
-00009050: 6520 6461 7461 2229 2c29 290a 2020 2020  e data"),)).    
-00009060: 2020 2020 2020 2020 292e 6665 7463 6861          ).fetcha
-00009070: 6c6c 2829 2c0a 2020 2020 2020 2020 2020  ll(),.          
-00009080: 2020 5b28 5472 7565 2c29 5d2c 0a20 2020    [(True,)],.   
-00009090: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-000090a0: 7465 7374 5f73 656c 6563 745f 6578 6973  test_select_exis
-000090b0: 7473 5f66 616c 7365 2873 656c 662c 2063  ts_false(self, c
-000090c0: 6f6e 6e65 6374 696f 6e29 3a0a 2020 2020  onnection):.    
-000090d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000090e0: 5350 414e 4e45 5220 4f56 4552 5249 4445  SPANNER OVERRIDE
-000090f0: 3a0a 0a20 2020 2020 2020 2054 6865 206f  :..        The o
-00009100: 7269 6769 6e61 6c20 7465 7374 2069 7320  riginal test is 
-00009110: 7472 7969 6e67 2074 6f20 6578 6563 7574  trying to execut
-00009120: 6520 6120 7175 6572 7920 6c69 6b65 3a0a  e a query like:.
-00009130: 0a20 2020 2020 2020 2053 454c 4543 5420  .        SELECT 
-00009140: 2e2e 2e0a 2020 2020 2020 2020 5748 4552  ....        WHER
-00009150: 4520 4558 4953 5453 2028 5345 4c45 4354  E EXISTS (SELECT
-00009160: 202e 2e2e 290a 0a20 2020 2020 2020 2053   ...)..        S
-00009170: 454c 4543 5420 5748 4552 4520 7769 7468  ELECT WHERE with
-00009180: 6f75 7420 4652 4f4d 2063 6c61 7573 6520  out FROM clause 
-00009190: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
-000091a0: 2062 7920 5370 616e 6e65 722e 0a20 2020   by Spanner..   
-000091b0: 2020 2020 2052 6577 7269 7469 6e67 2074       Rewriting t
-000091c0: 6865 2074 6573 7420 746f 2066 6f72 6365  he test to force
-000091d0: 2069 7420 746f 2067 656e 6572 6174 6520   it to generate 
-000091e0: 6120 7175 6572 7920 6c69 6b65 3a0a 0a20  a query like:.. 
-000091f0: 2020 2020 2020 2053 454c 4543 5420 4558         SELECT EX
-00009200: 4953 5453 2028 5345 4c45 4354 202e 2e2e  ISTS (SELECT ...
-00009210: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
-00009220: 2020 2020 2020 7374 7566 6620 3d20 7365        stuff = se
-00009230: 6c66 2e74 6162 6c65 732e 7374 7566 660a  lf.tables.stuff.
-00009240: 2020 2020 2020 2020 6571 5f28 0a20 2020          eq_(.   
-00009250: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
-00009260: 696f 6e2e 6578 6563 7574 6528 0a20 2020  ion.execute(.   
-00009270: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00009280: 6563 7428 2865 7869 7374 7328 292e 7768  ect((exists().wh
-00009290: 6572 6528 7374 7566 662e 632e 6461 7461  ere(stuff.c.data
-000092a0: 203d 3d20 226e 6f20 6461 7461 2229 2c29   == "no data"),)
-000092b0: 290a 2020 2020 2020 2020 2020 2020 292e  ).            ).
-000092c0: 6665 7463 6861 6c6c 2829 2c0a 2020 2020  fetchall(),.    
-000092d0: 2020 2020 2020 2020 5b28 4661 6c73 652c          [(False,
-000092e0: 295d 2c0a 2020 2020 2020 2020 290a 0a0a  )],.        )...
-000092f0: 636c 6173 7320 5461 626c 6544 444c 5465  class TableDDLTe
-00009300: 7374 285f 5461 626c 6544 444c 5465 7374  st(_TableDDLTest
-00009310: 293a 0a20 2020 2040 7079 7465 7374 2e6d  ):.    @pytest.m
-00009320: 6172 6b2e 736b 6970 280a 2020 2020 2020  ark.skip(.      
-00009330: 2020 2253 7061 6e6e 6572 2074 6162 6c65    "Spanner table
-00009340: 206e 616d 6520 6d75 7374 2073 7461 7274   name must start
-00009350: 2077 6974 6820 616e 2075 7070 6572 6361   with an upperca
-00009360: 7365 206f 7220 6c6f 7765 7263 6173 6520  se or lowercase 
-00009370: 6c65 7474 6572 220a 2020 2020 290a 2020  letter".    ).  
-00009380: 2020 6465 6620 7465 7374 5f75 6e64 6572    def test_under
-00009390: 7363 6f72 655f 6e61 6d65 7328 7365 6c66  score_names(self
-000093a0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-000093b0: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-000093c0: 6b2e 736b 6970 2822 5461 626c 6520 6e61  k.skip("Table na
-000093d0: 6d65 7320 696e 6375 6469 6e67 2073 6368  mes incuding sch
-000093e0: 656d 6173 2061 7265 206e 6f74 2073 7570  emas are not sup
-000093f0: 706f 7274 6564 2062 7920 5370 616e 6e65  ported by Spanne
-00009400: 7222 290a 2020 2020 6465 6620 7465 7374  r").    def test
-00009410: 5f63 7265 6174 655f 7461 626c 655f 7363  _create_table_sc
-00009420: 6865 6d61 2873 656c 6629 3a0a 2020 2020  hema(self):.    
-00009430: 2020 2020 7061 7373 0a0a 0a63 6c61 7373      pass...class
-00009440: 2046 7574 7572 6554 6162 6c65 4444 4c54   FutureTableDDLT
-00009450: 6573 7428 5f46 7574 7572 6554 6162 6c65  est(_FutureTable
-00009460: 4444 4c54 6573 7429 3a0a 2020 2020 4070  DDLTest):.    @p
-00009470: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
-00009480: 2254 6162 6c65 206e 616d 6573 2069 6e63  "Table names inc
-00009490: 7564 696e 6720 7363 6865 6d61 7320 6172  uding schemas ar
-000094a0: 6520 6e6f 7420 7375 7070 6f72 7465 6420  e not supported 
-000094b0: 6279 2053 7061 6e6e 6572 2229 0a20 2020  by Spanner").   
-000094c0: 2064 6566 2074 6573 745f 6372 6561 7465   def test_create
-000094d0: 5f74 6162 6c65 5f73 6368 656d 6128 7365  _table_schema(se
-000094e0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-000094f0: 730a 0a20 2020 2040 7079 7465 7374 2e6d  s..    @pytest.m
-00009500: 6172 6b2e 736b 6970 280a 2020 2020 2020  ark.skip(.      
-00009510: 2020 2253 7061 6e6e 6572 2074 6162 6c65    "Spanner table
-00009520: 206e 616d 6520 6d75 7374 2073 7461 7274   name must start
-00009530: 2077 6974 6820 616e 2075 7070 6572 6361   with an upperca
-00009540: 7365 206f 7220 6c6f 7765 7263 6173 6520  se or lowercase 
-00009550: 6c65 7474 6572 220a 2020 2020 290a 2020  letter".    ).  
-00009560: 2020 6465 6620 7465 7374 5f75 6e64 6572    def test_under
-00009570: 7363 6f72 655f 6e61 6d65 7328 7365 6c66  score_names(self
-00009580: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-00009590: 0a0a 4070 7974 6573 742e 6d61 726b 2e73  ..@pytest.mark.s
-000095a0: 6b69 7028 224d 6178 2069 6465 6e74 6966  kip("Max identif
-000095b0: 6965 7220 6c65 6e67 7468 2069 6e20 5370  ier length in Sp
-000095c0: 616e 6e65 7220 6973 2031 3238 2229 0a63  anner is 128").c
-000095d0: 6c61 7373 204c 6f6e 674e 616d 6542 6c6f  lass LongNameBlo
-000095e0: 776f 7574 5465 7374 285f 4c6f 6e67 4e61  woutTest(_LongNa
-000095f0: 6d65 426c 6f77 6f75 7454 6573 7429 3a0a  meBlowoutTest):.
-00009600: 2020 2020 7061 7373 0a0a 0a40 7079 7465      pass...@pyte
-00009610: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
-00009620: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
-00009630: 7070 6f72 7420 5469 6d65 2064 6174 6120  pport Time data 
-00009640: 7479 7065 2e22 290a 636c 6173 7320 5469  type.").class Ti
-00009650: 6d65 5465 7374 7328 5f54 696d 654d 6963  meTests(_TimeMic
-00009660: 726f 7365 636f 6e64 7354 6573 742c 205f  rosecondsTest, _
-00009670: 5469 6d65 5465 7374 293a 0a20 2020 2070  TimeTest):.    p
-00009680: 6173 730a 0a0a 4070 7974 6573 742e 6d61  ass...@pytest.ma
-00009690: 726b 2e73 6b69 7028 2253 7061 6e6e 6572  rk.skip("Spanner
-000096a0: 2064 6f65 736e 2774 2063 6f65 7263 6520   doesn't coerce 
-000096b0: 6461 7465 7320 6672 6f6d 2064 6174 6574  dates from datet
-000096c0: 696d 652e 2229 0a63 6c61 7373 2044 6174  ime.").class Dat
-000096d0: 6554 696d 6543 6f65 7263 6564 546f 4461  eTimeCoercedToDa
-000096e0: 7465 5469 6d65 5465 7374 285f 4461 7465  teTimeTest(_Date
-000096f0: 5469 6d65 436f 6572 6365 6454 6f44 6174  TimeCoercedToDat
-00009700: 6554 696d 6554 6573 7429 3a0a 2020 2020  eTimeTest):.    
-00009710: 7061 7373 0a0a 0a63 6c61 7373 2049 6e74  pass...class Int
-00009720: 6567 6572 5465 7374 285f 496e 7465 6765  egerTest(_Intege
-00009730: 7254 6573 7429 3a0a 2020 2020 4070 726f  rTest):.    @pro
-00009740: 7669 6465 5f6d 6574 6164 6174 610a 2020  vide_metadata.  
-00009750: 2020 6465 6620 5f72 6f75 6e64 5f74 7269    def _round_tri
-00009760: 7028 7365 6c66 2c20 6461 7461 7479 7065  p(self, datatype
-00009770: 2c20 6461 7461 293a 0a20 2020 2020 2020  , data):.       
-00009780: 2022 2222 0a20 2020 2020 2020 2053 5041   """.        SPA
-00009790: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
-000097a0: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
-000097b0: 7468 6520 6865 6c70 6572 206d 6574 686f  the helper metho
-000097c0: 6420 666f 7220 696e 7465 6765 7220 636c  d for integer cl
-000097d0: 6173 7320 7465 7374 7320 7768 6963 6820  ass tests which 
-000097e0: 6372 6561 7465 7320 6120 7461 626c 6520  creates a table 
-000097f0: 616e 640a 2020 2020 2020 2020 7065 7266  and.        perf
-00009800: 6f72 6d73 2061 6e20 696e 7365 7274 206f  orms an insert o
-00009810: 7065 7261 7469 6f6e 2e0a 2020 2020 2020  peration..      
-00009820: 2020 436c 6f75 6420 5370 616e 6e65 7220    Cloud Spanner 
-00009830: 7375 7070 6f72 7473 2074 6162 6c65 7320  supports tables 
-00009840: 7769 7468 2061 6e20 656d 7074 7920 7072  with an empty pr
-00009850: 696d 6172 7920 6b65 792c 2062 7574 206f  imary key, but o
-00009860: 6e6c 7920 6f6e 650a 2020 2020 2020 2020  nly one.        
-00009870: 726f 7720 6361 6e20 6265 2069 6e73 6572  row can be inser
-00009880: 7465 6420 696e 746f 2073 7563 6820 6120  ted into such a 
-00009890: 7461 626c 6520 2d20 666f 6c6c 6f77 696e  table - followin
-000098a0: 6720 696e 7365 7274 696f 6e73 2077 696c  g insertions wil
-000098b0: 6c20 6661 696c 2077 6974 680a 2020 2020  l fail with.    
-000098c0: 2020 2020 6034 3030 2069 6420 6d75 7374      `400 id must
-000098d0: 206e 6f74 2062 6520 4e55 4c4c 2069 6e20   not be NULL in 
-000098e0: 7461 626c 6520 6461 7465 5f74 6162 6c65  table date_table
-000098f0: 602e 0a20 2020 2020 2020 204f 7665 7272  `..        Overr
-00009900: 6964 696e 6720 7468 6520 7465 7374 7320  iding the tests 
-00009910: 616e 6420 6164 6469 6e67 2061 206d 616e  and adding a man
-00009920: 7561 6c20 7072 696d 6172 7920 6b65 7920  ual primary key 
-00009930: 7661 6c75 6520 746f 2061 766f 6964 2074  value to avoid t
-00009940: 6865 2073 616d 650a 2020 2020 2020 2020  he same.        
-00009950: 6661 696c 7572 6573 2e0a 2020 2020 2020  failures..      
-00009960: 2020 2222 220a 2020 2020 2020 2020 6d65    """.        me
-00009970: 7461 6461 7461 203d 2073 656c 662e 6d65  tadata = self.me
-00009980: 7461 6461 7461 0a20 2020 2020 2020 2069  tadata.        i
-00009990: 6e74 5f74 6162 6c65 203d 2054 6162 6c65  nt_table = Table
-000099a0: 280a 2020 2020 2020 2020 2020 2020 2269  (.            "i
-000099b0: 6e74 6567 6572 5f74 6162 6c65 222c 0a20  nteger_table",. 
-000099c0: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-000099d0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-000099e0: 2043 6f6c 756d 6e28 2269 6422 2c20 496e   Column("id", In
-000099f0: 7465 6765 722c 2070 7269 6d61 7279 5f6b  teger, primary_k
-00009a00: 6579 3d54 7275 652c 2074 6573 745f 6e65  ey=True, test_ne
-00009a10: 6564 735f 6175 746f 696e 6372 656d 656e  eds_autoincremen
-00009a20: 743d 5472 7565 292c 0a20 2020 2020 2020  t=True),.       
-00009a30: 2020 2020 2043 6f6c 756d 6e28 2269 6e74       Column("int
-00009a40: 6567 6572 5f64 6174 6122 2c20 6461 7461  eger_data", data
-00009a50: 7479 7065 292c 0a20 2020 2020 2020 2029  type),.        )
-00009a60: 0a0a 2020 2020 2020 2020 6d65 7461 6461  ..        metada
-00009a70: 7461 2e63 7265 6174 655f 616c 6c28 636f  ta.create_all(co
-00009a80: 6e66 6967 2e64 6229 0a0a 2020 2020 2020  nfig.db)..      
-00009a90: 2020 636f 6e66 6967 2e64 622e 6578 6563    config.db.exec
-00009aa0: 7574 6528 696e 745f 7461 626c 652e 696e  ute(int_table.in
-00009ab0: 7365 7274 2829 2c20 7b22 6964 223a 2031  sert(), {"id": 1
-00009ac0: 2c20 2269 6e74 6567 6572 5f64 6174 6122  , "integer_data"
-00009ad0: 3a20 6461 7461 7d29 0a0a 2020 2020 2020  : data})..      
-00009ae0: 2020 726f 7720 3d20 636f 6e66 6967 2e64    row = config.d
-00009af0: 622e 6578 6563 7574 6528 7365 6c65 6374  b.execute(select
-00009b00: 285b 696e 745f 7461 626c 652e 632e 696e  ([int_table.c.in
-00009b10: 7465 6765 725f 6461 7461 5d29 292e 6669  teger_data])).fi
-00009b20: 7273 7428 290a 0a20 2020 2020 2020 2065  rst()..        e
-00009b30: 715f 2872 6f77 2c20 2864 6174 612c 2929  q_(row, (data,))
-00009b40: 0a0a 2020 2020 2020 2020 6966 2075 7469  ..        if uti
-00009b50: 6c2e 7079 336b 3a0a 2020 2020 2020 2020  l.py3k:.        
-00009b60: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
-00009b70: 7461 6e63 6528 726f 775b 305d 2c20 696e  tance(row[0], in
-00009b80: 7429 0a20 2020 2020 2020 2065 6c73 653a  t).        else:
-00009b90: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00009ba0: 6572 7420 6973 696e 7374 616e 6365 2872  ert isinstance(r
-00009bb0: 6f77 5b30 5d2c 2028 6c6f 6e67 2c20 696e  ow[0], (long, in
-00009bc0: 7429 2920 2023 206e 6f71 610a 0a0a 636c  t))  # noqa...cl
-00009bd0: 6173 7320 5f55 6e69 636f 6465 4669 7874  ass _UnicodeFixt
-00009be0: 7572 6528 5f5f 556e 6963 6f64 6546 6978  ure(__UnicodeFix
-00009bf0: 7475 7265 293a 0a20 2020 2040 636c 6173  ture):.    @clas
-00009c00: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-00009c10: 6465 6669 6e65 5f74 6162 6c65 7328 636c  define_tables(cl
-00009c20: 732c 206d 6574 6164 6174 6129 3a0a 2020  s, metadata):.  
-00009c30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00009c40: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
-00009c50: 4445 3a0a 0a20 2020 2020 2020 2043 6c6f  DE:..        Clo
-00009c60: 7564 2053 7061 6e6e 6572 2064 6f65 736e  ud Spanner doesn
-00009c70: 2774 2073 7570 706f 7274 2061 7574 6f20  't support auto 
-00009c80: 696e 6372 656d 656e 7469 6e67 2069 6473  incrementing ids
-00009c90: 2066 6561 7475 7265 2c0a 2020 2020 2020   feature,.      
-00009ca0: 2020 7768 6963 6820 6973 2075 7365 6420    which is used 
-00009cb0: 6279 2074 6865 206f 7269 6769 6e61 6c20  by the original 
-00009cc0: 7465 7374 2e20 4f76 6572 7269 6469 6e67  test. Overriding
-00009cd0: 2074 6865 2074 6573 7420 6461 7461 0a20   the test data. 
-00009ce0: 2020 2020 2020 2063 7265 6174 696f 6e20         creation 
-00009cf0: 6d65 7468 6f64 2074 6f20 6469 7361 626c  method to disabl
-00009d00: 6520 6175 746f 696e 6372 656d 656e 7420  e autoincrement 
-00009d10: 616e 6420 6d61 6b65 2069 6420 636f 6c75  and make id colu
-00009d20: 6d6e 0a20 2020 2020 2020 206e 756c 6c61  mn.        nulla
-00009d30: 626c 652e 0a20 2020 2020 2020 2022 2222  ble..        """
-00009d40: 0a20 2020 2020 2020 2054 6162 6c65 280a  .        Table(.
-00009d50: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
-00009d60: 636f 6465 5f74 6162 6c65 222c 0a20 2020  code_table",.   
-00009d70: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
-00009d80: 612c 0a20 2020 2020 2020 2020 2020 2043  a,.            C
-00009d90: 6f6c 756d 6e28 2269 6422 2c20 496e 7465  olumn("id", Inte
-00009da0: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
-00009db0: 3d54 7275 652c 206e 756c 6c61 626c 653d  =True, nullable=
-00009dc0: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-00009dd0: 2020 2043 6f6c 756d 6e28 2275 6e69 636f     Column("unico
-00009de0: 6465 5f64 6174 6122 2c20 636c 732e 6461  de_data", cls.da
-00009df0: 7461 7479 7065 292c 0a20 2020 2020 2020  tatype),.       
-00009e00: 2029 0a0a 2020 2020 6465 6620 7465 7374   )..    def test
-00009e10: 5f72 6f75 6e64 5f74 7269 705f 6578 6563  _round_trip_exec
-00009e20: 7574 656d 616e 7928 7365 6c66 293a 0a20  utemany(self):. 
-00009e30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00009e40: 2020 2053 5041 4e4e 4552 204f 5645 5252     SPANNER OVERR
-00009e50: 4944 450a 0a20 2020 2020 2020 2043 6c6f  IDE..        Clo
-00009e60: 7564 2053 7061 6e6e 6572 2073 7570 706f  ud Spanner suppo
-00009e70: 7274 7320 7461 626c 6573 2077 6974 6820  rts tables with 
-00009e80: 656d 7074 7920 7072 696d 6172 7920 6b65  empty primary ke
-00009e90: 792c 2062 7574 0a20 2020 2020 2020 206f  y, but.        o
-00009ea0: 6e6c 7920 7369 6e67 6c65 206f 6e65 2072  nly single one r
-00009eb0: 6f77 2063 616e 2062 6520 696e 7365 7274  ow can be insert
-00009ec0: 6564 2069 6e74 6f20 7375 6368 2061 2074  ed into such a t
-00009ed0: 6162 6c65 202d 0a20 2020 2020 2020 2066  able -.        f
-00009ee0: 6f6c 6c6f 7769 6e67 2069 6e73 6572 7469  ollowing inserti
-00009ef0: 6f6e 7320 7769 6c6c 2066 6169 6c20 7769  ons will fail wi
-00009f00: 7468 2060 526f 7720 5b5d 2061 6c72 6561  th `Row [] alrea
-00009f10: 6479 2065 7869 7374 7322 2e0a 2020 2020  dy exists"..    
-00009f20: 2020 2020 4f76 6572 7269 6469 6e67 2074      Overriding t
-00009f30: 6865 2074 6573 7420 746f 2061 766f 6964  he test to avoid
-00009f40: 2074 6865 2073 616d 6520 6661 696c 7572   the same failur
-00009f50: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00009f60: 2020 2020 2020 2075 6e69 636f 6465 5f74         unicode_t
-00009f70: 6162 6c65 203d 2073 656c 662e 7461 626c  able = self.tabl
-00009f80: 6573 2e75 6e69 636f 6465 5f74 6162 6c65  es.unicode_table
-00009f90: 0a0a 2020 2020 2020 2020 636f 6e66 6967  ..        config
-00009fa0: 2e64 622e 6578 6563 7574 6528 0a20 2020  .db.execute(.   
-00009fb0: 2020 2020 2020 2020 2075 6e69 636f 6465           unicode
-00009fc0: 5f74 6162 6c65 2e69 6e73 6572 7428 292c  _table.insert(),
-00009fd0: 0a20 2020 2020 2020 2020 2020 205b 7b22  .            [{"
-00009fe0: 6964 223a 2069 2c20 2275 6e69 636f 6465  id": i, "unicode
-00009ff0: 5f64 6174 6122 3a20 7365 6c66 2e64 6174  _data": self.dat
-0000a000: 617d 2066 6f72 2069 2069 6e20 7261 6e67  a} for i in rang
-0000a010: 6528 3329 5d2c 0a20 2020 2020 2020 2029  e(3)],.        )
-0000a020: 0a0a 2020 2020 2020 2020 726f 7773 203d  ..        rows =
-0000a030: 2063 6f6e 6669 672e 6462 2e65 7865 6375   config.db.execu
-0000a040: 7465 2873 656c 6563 7428 5b75 6e69 636f  te(select([unico
-0000a050: 6465 5f74 6162 6c65 2e63 2e75 6e69 636f  de_table.c.unico
-0000a060: 6465 5f64 6174 615d 2929 2e66 6574 6368  de_data])).fetch
-0000a070: 616c 6c28 290a 2020 2020 2020 2020 6571  all().        eq
-0000a080: 5f28 726f 7773 2c20 5b28 7365 6c66 2e64  _(rows, [(self.d
-0000a090: 6174 612c 2920 666f 7220 6920 696e 2072  ata,) for i in r
-0000a0a0: 616e 6765 2833 295d 290a 2020 2020 2020  ange(3)]).      
-0000a0b0: 2020 666f 7220 726f 7720 696e 2072 6f77    for row in row
-0000a0c0: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
-0000a0d0: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
-0000a0e0: 2872 6f77 5b30 5d2c 2075 7469 6c2e 7465  (row[0], util.te
-0000a0f0: 7874 5f74 7970 6529 0a0a 2020 2020 4070  xt_type)..    @p
-0000a100: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
-0000a110: 2253 7061 6e6e 6572 2064 6f65 736e 2774  "Spanner doesn't
-0000a120: 2073 7570 706f 7274 206e 6f6e 2d61 7363   support non-asc
-0000a130: 6969 2063 6861 7261 6374 6572 7322 290a  ii characters").
-0000a140: 2020 2020 6465 6620 7465 7374 5f6c 6974      def test_lit
-0000a150: 6572 616c 2873 656c 6629 3a0a 2020 2020  eral(self):.    
-0000a160: 2020 2020 7061 7373 0a0a 2020 2020 4070      pass..    @p
-0000a170: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
-0000a180: 2253 7061 6e6e 6572 2064 6f65 736e 2774  "Spanner doesn't
-0000a190: 2073 7570 706f 7274 206e 6f6e 2d61 7363   support non-asc
-0000a1a0: 6969 2063 6861 7261 6374 6572 7322 290a  ii characters").
-0000a1b0: 2020 2020 6465 6620 7465 7374 5f6c 6974      def test_lit
-0000a1c0: 6572 616c 5f6e 6f6e 5f61 7363 6969 2873  eral_non_ascii(s
-0000a1d0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-0000a1e0: 7373 0a0a 0a63 6c61 7373 2055 6e69 636f  ss...class Unico
-0000a1f0: 6465 5661 7263 6861 7254 6573 7428 5f55  deVarcharTest(_U
-0000a200: 6e69 636f 6465 4669 7874 7572 652c 205f  nicodeFixture, _
-0000a210: 556e 6963 6f64 6556 6172 6368 6172 5465  UnicodeVarcharTe
-0000a220: 7374 293a 0a20 2020 2022 2222 0a20 2020  st):.    """.   
-0000a230: 2053 5041 4e4e 4552 204f 5645 5252 4944   SPANNER OVERRID
-0000a240: 453a 0a0a 2020 2020 556e 6963 6f64 6556  E:..    UnicodeV
-0000a250: 6172 6368 6172 5465 7374 2063 6c61 7373  archarTest class
-0000a260: 2069 6e68 6572 6974 7320 7468 6520 5f5f   inherits the __
-0000a270: 556e 6963 6f64 6546 6978 7475 7265 2063  UnicodeFixture c
-0000a280: 6c61 7373 2773 2074 6573 7473 2c0a 2020  lass's tests,.  
-0000a290: 2020 736f 2074 6f20 6176 6f69 6420 7468    so to avoid th
-0000a2a0: 6f73 6520 6661 696c 7572 6573 2061 6e64  ose failures and
-0000a2b0: 206d 6169 6e74 6169 6e20 4452 5920 636f   maintain DRY co
-0000a2c0: 6e63 6570 7420 6a75 7374 2069 6e68 6572  ncept just inher
-0000a2d0: 6974 2074 6865 2063 6c61 7373 2074 6f20  it the class to 
-0000a2e0: 7275 6e0a 2020 2020 7465 7374 7320 7375  run.    tests su
-0000a2f0: 6363 6573 7366 756c 6c79 2e0a 2020 2020  ccessfully..    
-0000a300: 2222 220a 0a20 2020 2070 6173 730a 0a0a  """..    pass...
-0000a310: 636c 6173 7320 556e 6963 6f64 6554 6578  class UnicodeTex
-0000a320: 7454 6573 7428 5f55 6e69 636f 6465 4669  tTest(_UnicodeFi
-0000a330: 7874 7572 652c 205f 556e 6963 6f64 6554  xture, _UnicodeT
-0000a340: 6578 7454 6573 7429 3a0a 2020 2020 2222  extTest):.    ""
-0000a350: 220a 2020 2020 5350 414e 4e45 5220 4f56  ".    SPANNER OV
-0000a360: 4552 5249 4445 3a0a 0a20 2020 2055 6e69  ERRIDE:..    Uni
-0000a370: 636f 6465 5465 7874 5465 7374 2063 6c61  codeTextTest cla
-0000a380: 7373 2069 6e68 6572 6974 7320 7468 6520  ss inherits the 
-0000a390: 5f5f 556e 6963 6f64 6546 6978 7475 7265  __UnicodeFixture
-0000a3a0: 2063 6c61 7373 2773 2074 6573 7473 2c0a   class's tests,.
-0000a3b0: 2020 2020 736f 2074 6f20 6176 6f69 6420      so to avoid 
-0000a3c0: 7468 6f73 6520 6661 696c 7572 6573 2061  those failures a
-0000a3d0: 6e64 206d 6169 6e74 6169 6e20 4452 5920  nd maintain DRY 
-0000a3e0: 636f 6e63 6570 7420 6a75 7374 2069 6e68  concept just inh
-0000a3f0: 6572 6974 2074 6865 2063 6c61 7373 2074  erit the class t
-0000a400: 6f20 7275 6e0a 2020 2020 7465 7374 7320  o run.    tests 
-0000a410: 7375 6363 6573 7366 756c 6c79 2e0a 2020  successfully..  
-0000a420: 2020 2222 220a 0a20 2020 2070 6173 730a    """..    pass.
-0000a430: 0a0a 636c 6173 7320 526f 7746 6574 6368  ..class RowFetch
-0000a440: 5465 7374 285f 526f 7746 6574 6368 5465  Test(_RowFetchTe
-0000a450: 7374 293a 0a20 2020 2064 6566 2074 6573  st):.    def tes
-0000a460: 745f 726f 775f 775f 7363 616c 6172 5f73  t_row_w_scalar_s
-0000a470: 656c 6563 7428 7365 6c66 293a 0a20 2020  elect(self):.   
-0000a480: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000a490: 2053 5041 4e4e 4552 204f 5645 5252 4944   SPANNER OVERRID
-0000a4a0: 453a 0a0a 2020 2020 2020 2020 436c 6f75  E:..        Clou
-0000a4b0: 6420 5370 616e 6e65 7220 7265 7475 726e  d Spanner return
-0000a4c0: 7320 6120 4461 7465 7469 6d65 5769 7468  s a DatetimeWith
-0000a4d0: 4e61 6e6f 7365 636f 6e64 7328 2920 666f  Nanoseconds() fo
-0000a4e0: 7220 6461 7465 0a20 2020 2020 2020 2064  r date.        d
-0000a4f0: 6174 6120 7479 7065 732e 204f 7665 7272  ata types. Overr
-0000a500: 6964 696e 6720 7468 6520 7465 7374 2074  iding the test t
-0000a510: 6f20 7573 6520 6120 4461 7465 7469 6d65  o use a Datetime
-0000a520: 5769 7468 4e61 6e6f 7365 636f 6e64 730a  WithNanoseconds.
-0000a530: 2020 2020 2020 2020 7479 7065 2076 616c          type val
-0000a540: 7565 2061 7320 616e 2065 7870 6563 7465  ue as an expecte
-0000a550: 6420 7265 7375 6c74 2e0a 2020 2020 2020  d result..      
-0000a560: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-0000a570: 0a0a 2020 2020 2020 2020 7465 7374 2074  ..        test t
-0000a580: 6861 7420 6120 7363 616c 6172 2073 656c  hat a scalar sel
-0000a590: 6563 7420 6173 2061 2063 6f6c 756d 6e20  ect as a column 
-0000a5a0: 6973 2072 6574 7572 6e65 6420 6173 2073  is returned as s
-0000a5b0: 7563 680a 2020 2020 2020 2020 616e 6420  uch.        and 
-0000a5c0: 7468 6174 2074 7970 6520 636f 6e76 6572  that type conver
-0000a5d0: 7369 6f6e 2077 6f72 6b73 204f 4b2e 0a0a  sion works OK...
-0000a5e0: 2020 2020 2020 2020 2874 6869 7320 6973          (this is
-0000a5f0: 2068 616c 6620 6120 5351 4c41 6c63 6865   half a SQLAlche
-0000a600: 6d79 2043 6f72 6520 7465 7374 2061 6e64  my Core test and
-0000a610: 2068 616c 6620 746f 2063 6174 6368 2064   half to catch d
-0000a620: 6174 6162 6173 650a 2020 2020 2020 2020  atabase.        
-0000a630: 6261 636b 656e 6473 2074 6861 7420 6d61  backends that ma
-0000a640: 7920 6861 7665 2075 6e75 7375 616c 2062  y have unusual b
-0000a650: 6568 6176 696f 7220 7769 7468 2073 6361  ehavior with sca
-0000a660: 6c61 7220 7365 6c65 6374 732e 290a 2020  lar selects.).  
-0000a670: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000a680: 2020 6461 7465 7461 626c 6520 3d20 7365    datetable = se
-0000a690: 6c66 2e74 6162 6c65 732e 6861 735f 6461  lf.tables.has_da
-0000a6a0: 7465 730a 2020 2020 2020 2020 7320 3d20  tes.        s = 
-0000a6b0: 7365 6c65 6374 285b 6461 7465 7461 626c  select([datetabl
-0000a6c0: 652e 616c 6961 7328 2278 2229 2e63 2e74  e.alias("x").c.t
-0000a6d0: 6f64 6179 5d29 2e73 6361 6c61 725f 7375  oday]).scalar_su
-0000a6e0: 6271 7565 7279 2829 0a20 2020 2020 2020  bquery().       
-0000a6f0: 2073 3220 3d20 7365 6c65 6374 285b 6461   s2 = select([da
-0000a700: 7465 7461 626c 652e 632e 6964 2c20 732e  tetable.c.id, s.
-0000a710: 6c61 6265 6c28 2273 6f6d 656c 6162 656c  label("somelabel
-0000a720: 2229 5d29 0a20 2020 2020 2020 2072 6f77  ")]).        row
-0000a730: 203d 2063 6f6e 6669 672e 6462 2e65 7865   = config.db.exe
-0000a740: 6375 7465 2873 3229 2e66 6972 7374 2829  cute(s2).first()
-0000a750: 0a0a 2020 2020 2020 2020 6571 5f28 0a20  ..        eq_(. 
-0000a760: 2020 2020 2020 2020 2020 2072 6f77 5b22             row["
-0000a770: 736f 6d65 6c61 6265 6c22 5d2c 0a20 2020  somelabel"],.   
-0000a780: 2020 2020 2020 2020 2044 6174 6574 696d           Datetim
-0000a790: 6557 6974 684e 616e 6f73 6563 6f6e 6473  eWithNanoseconds
-0000a7a0: 2832 3030 362c 2035 2c20 3132 2c20 3132  (2006, 5, 12, 12
-0000a7b0: 2c20 302c 2030 2c20 747a 696e 666f 3d74  , 0, 0, tzinfo=t
-0000a7c0: 696d 657a 6f6e 652e 7574 6329 2c0a 2020  imezone.utc),.  
-0000a7d0: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
-0000a7e0: 496e 7365 7274 4265 6861 7669 6f72 5465  InsertBehaviorTe
-0000a7f0: 7374 285f 496e 7365 7274 4265 6861 7669  st(_InsertBehavi
-0000a800: 6f72 5465 7374 293a 0a20 2020 2040 7079  orTest):.    @py
-0000a810: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
-0000a820: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
-0000a830: 7375 7070 6f72 7420 656d 7074 7920 696e  support empty in
-0000a840: 7365 7274 7322 290a 2020 2020 6465 6620  serts").    def 
-0000a850: 7465 7374 5f65 6d70 7479 5f69 6e73 6572  test_empty_inser
-0000a860: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
-0000a870: 2070 6173 730a 0a20 2020 2040 7079 7465   pass..    @pyte
-0000a880: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
-0000a890: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
-0000a8a0: 7070 6f72 7420 656d 7074 7920 696e 7365  pport empty inse
-0000a8b0: 7274 7322 290a 2020 2020 6465 6620 7465  rts").    def te
-0000a8c0: 7374 5f65 6d70 7479 5f69 6e73 6572 745f  st_empty_insert_
-0000a8d0: 6d75 6c74 6970 6c65 2873 656c 6629 3a0a  multiple(self):.
-0000a8e0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-0000a8f0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-0000a900: 6b69 7028 2253 7061 6e6e 6572 2064 6f65  kip("Spanner doe
-0000a910: 736e 2774 2073 7570 706f 7274 2061 7574  sn't support aut
-0000a920: 6f20 696e 6372 656d 656e 7422 290a 2020  o increment").  
-0000a930: 2020 6465 6620 7465 7374 5f69 6e73 6572    def test_inser
-0000a940: 745f 6672 6f6d 5f73 656c 6563 745f 6175  t_from_select_au
-0000a950: 746f 696e 6328 7365 6c66 293a 0a20 2020  toinc(self):.   
-0000a960: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-0000a970: 6566 2074 6573 745f 6175 746f 636c 6f73  ef test_autoclos
-0000a980: 655f 6f6e 5f69 6e73 6572 7428 7365 6c66  e_on_insert(self
-0000a990: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000a9a0: 2020 2020 2020 2053 5041 4e4e 4552 204f         SPANNER O
-0000a9b0: 5645 5252 4944 453a 0a0a 2020 2020 2020  VERRIDE:..      
-0000a9c0: 2020 436c 6f75 6420 5370 616e 6e65 7220    Cloud Spanner 
-0000a9d0: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
-0000a9e0: 7461 626c 6573 2077 6974 6820 616e 2061  tables with an a
-0000a9f0: 7574 6f20 696e 6372 656d 656e 7420 7072  uto increment pr
-0000aa00: 696d 6172 7920 6b65 792c 0a20 2020 2020  imary key,.     
-0000aa10: 2020 2066 6f6c 6c6f 7769 6e67 2069 6e73     following ins
-0000aa20: 6572 7469 6f6e 7320 7769 6c6c 2066 6169  ertions will fai
-0000aa30: 6c20 7769 7468 2060 3430 3020 6964 206d  l with `400 id m
-0000aa40: 7573 7420 6e6f 7420 6265 204e 554c 4c20  ust not be NULL 
-0000aa50: 696e 2074 6162 6c65 0a20 2020 2020 2020  in table.       
-0000aa60: 2061 7574 6f69 6e63 5f70 6b60 2e0a 0a20   autoinc_pk`... 
-0000aa70: 2020 2020 2020 204f 7665 7272 6964 696e         Overridin
-0000aa80: 6720 7468 6520 7465 7374 7320 616e 6420  g the tests and 
-0000aa90: 6164 6469 6e67 2061 206d 616e 7561 6c20  adding a manual 
-0000aaa0: 7072 696d 6172 7920 6b65 7920 7661 6c75  primary key valu
-0000aab0: 6520 746f 2061 766f 6964 2074 6865 2073  e to avoid the s
-0000aac0: 616d 650a 2020 2020 2020 2020 6661 696c  ame.        fail
-0000aad0: 7572 6573 2e0a 2020 2020 2020 2020 2222  ures..        ""
-0000aae0: 220a 2020 2020 2020 2020 6966 2063 6f6e  ".        if con
-0000aaf0: 6669 672e 7265 7175 6972 656d 656e 7473  fig.requirements
-0000ab00: 2e72 6574 7572 6e69 6e67 2e65 6e61 626c  .returning.enabl
-0000ab10: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
-0000ab20: 656e 6769 6e65 203d 2065 6e67 696e 6573  engine = engines
-0000ab30: 2e74 6573 7469 6e67 5f65 6e67 696e 6528  .testing_engine(
-0000ab40: 6f70 7469 6f6e 733d 7b22 696d 706c 6963  options={"implic
-0000ab50: 6974 5f72 6574 7572 6e69 6e67 223a 2046  it_returning": F
-0000ab60: 616c 7365 7d29 0a20 2020 2020 2020 2065  alse}).        e
-0000ab70: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000ab80: 2065 6e67 696e 6520 3d20 636f 6e66 6967   engine = config
-0000ab90: 2e64 620a 0a20 2020 2020 2020 2077 6974  .db..        wit
-0000aba0: 6820 656e 6769 6e65 2e62 6567 696e 2829  h engine.begin()
-0000abb0: 2061 7320 636f 6e6e 3a0a 2020 2020 2020   as conn:.      
-0000abc0: 2020 2020 2020 7220 3d20 636f 6e6e 2e65        r = conn.e
-0000abd0: 7865 6375 7465 280a 2020 2020 2020 2020  xecute(.        
-0000abe0: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
-0000abf0: 6c65 732e 6175 746f 696e 635f 706b 2e69  les.autoinc_pk.i
-0000ac00: 6e73 6572 7428 292c 2064 6963 7428 6964  nsert(), dict(id
-0000ac10: 3d31 2c20 6461 7461 3d22 736f 6d65 2064  =1, data="some d
-0000ac20: 6174 6122 290a 2020 2020 2020 2020 2020  ata").          
-0000ac30: 2020 290a 0a20 2020 2020 2020 2061 7373    )..        ass
-0000ac40: 6572 7420 722e 5f73 6f66 745f 636c 6f73  ert r._soft_clos
-0000ac50: 6564 0a20 2020 2020 2020 2061 7373 6572  ed.        asser
-0000ac60: 7420 6e6f 7420 722e 636c 6f73 6564 0a20  t not r.closed. 
-0000ac70: 2020 2020 2020 2061 7373 6572 7420 722e         assert r.
-0000ac80: 6973 5f69 6e73 6572 740a 2020 2020 2020  is_insert.      
-0000ac90: 2020 6173 7365 7274 206e 6f74 2072 2e72    assert not r.r
-0000aca0: 6574 7572 6e73 5f72 6f77 730a 0a0a 636c  eturns_rows...cl
-0000acb0: 6173 7320 4279 7465 7354 6573 7428 5f4c  ass BytesTest(_L
-0000acc0: 6974 6572 616c 526f 756e 6454 7269 7046  iteralRoundTripF
-0000acd0: 6978 7475 7265 2c20 6669 7874 7572 6573  ixture, fixtures
-0000ace0: 2e54 6573 7442 6173 6529 3a0a 2020 2020  .TestBase):.    
-0000acf0: 5f5f 6261 636b 656e 645f 5f20 3d20 5472  __backend__ = Tr
-0000ad00: 7565 0a0a 2020 2020 6465 6620 7465 7374  ue..    def test
-0000ad10: 5f6e 6f6c 656e 6774 685f 6269 6e61 7279  _nolength_binary
-0000ad20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000ad30: 6d65 7461 6461 7461 203d 204d 6574 6144  metadata = MetaD
-0000ad40: 6174 6128 290a 2020 2020 2020 2020 666f  ata().        fo
-0000ad50: 6f20 3d20 5461 626c 6528 2266 6f6f 222c  o = Table("foo",
-0000ad60: 206d 6574 6164 6174 612c 2043 6f6c 756d   metadata, Colum
-0000ad70: 6e28 226f 6e65 222c 204c 6172 6765 4269  n("one", LargeBi
-0000ad80: 6e61 7279 2929 0a0a 2020 2020 2020 2020  nary))..        
-0000ad90: 666f 6f2e 6372 6561 7465 2863 6f6e 6669  foo.create(confi
-0000ada0: 672e 6462 290a 2020 2020 2020 2020 666f  g.db).        fo
-0000adb0: 6f2e 6472 6f70 2863 6f6e 6669 672e 6462  o.drop(config.db
-0000adc0: 290a 0a0a 636c 6173 7320 5374 7269 6e67  )...class String
-0000add0: 5465 7374 285f 5374 7269 6e67 5465 7374  Test(_StringTest
-0000ade0: 293a 0a20 2020 2040 7079 7465 7374 2e6d  ):.    @pytest.m
-0000adf0: 6172 6b2e 736b 6970 2822 5370 616e 6e65  ark.skip("Spanne
-0000ae00: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
-0000ae10: 7420 6e6f 6e2d 6173 6369 6920 6368 6172  t non-ascii char
-0000ae20: 6163 7465 7273 2229 0a20 2020 2064 6566  acters").    def
-0000ae30: 2074 6573 745f 6c69 7465 7261 6c5f 6e6f   test_literal_no
-0000ae40: 6e5f 6173 6369 6928 7365 6c66 293a 0a20  n_ascii(self):. 
-0000ae50: 2020 2020 2020 2070 6173 730a 0a0a 636c         pass...cl
-0000ae60: 6173 7320 5465 7874 5465 7374 285f 5465  ass TextTest(_Te
-0000ae70: 7874 5465 7374 293a 0a20 2020 2040 636c  xtTest):.    @cl
-0000ae80: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-0000ae90: 6620 6465 6669 6e65 5f74 6162 6c65 7328  f define_tables(
-0000aea0: 636c 732c 206d 6574 6164 6174 6129 3a0a  cls, metadata):.
-0000aeb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000aec0: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
-0000aed0: 5249 4445 3a0a 0a20 2020 2020 2020 2043  RIDE:..        C
-0000aee0: 6c6f 7564 2053 7061 6e6e 6572 2064 6f65  loud Spanner doe
-0000aef0: 736e 2774 2073 7570 706f 7274 2061 7574  sn't support aut
-0000af00: 6f20 696e 6372 656d 656e 7469 6e67 2069  o incrementing i
-0000af10: 6473 2066 6561 7475 7265 2c0a 2020 2020  ds feature,.    
-0000af20: 2020 2020 7768 6963 6820 6973 2075 7365      which is use
-0000af30: 6420 6279 2074 6865 206f 7269 6769 6e61  d by the origina
-0000af40: 6c20 7465 7374 2e20 4f76 6572 7269 6469  l test. Overridi
-0000af50: 6e67 2074 6865 2074 6573 7420 6461 7461  ng the test data
-0000af60: 0a20 2020 2020 2020 2063 7265 6174 696f  .        creatio
-0000af70: 6e20 6d65 7468 6f64 2074 6f20 6469 7361  n method to disa
-0000af80: 626c 6520 6175 746f 696e 6372 656d 656e  ble autoincremen
-0000af90: 7420 616e 6420 6d61 6b65 2069 6420 636f  t and make id co
-0000afa0: 6c75 6d6e 0a20 2020 2020 2020 206e 756c  lumn.        nul
-0000afb0: 6c61 626c 652e 0a20 2020 2020 2020 2022  lable..        "
-0000afc0: 2222 0a20 2020 2020 2020 2054 6162 6c65  "".        Table
-0000afd0: 280a 2020 2020 2020 2020 2020 2020 2274  (.            "t
-0000afe0: 6578 745f 7461 626c 6522 2c0a 2020 2020  ext_table",.    
-0000aff0: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-0000b000: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
-0000b010: 6c75 6d6e 2822 6964 222c 2049 6e74 6567  lumn("id", Integ
-0000b020: 6572 2c20 7072 696d 6172 795f 6b65 793d  er, primary_key=
-0000b030: 5472 7565 2c20 6e75 6c6c 6162 6c65 3d54  True, nullable=T
-0000b040: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
-0000b050: 2020 436f 6c75 6d6e 2822 7465 7874 5f64    Column("text_d
-0000b060: 6174 6122 2c20 5465 7874 292c 0a20 2020  ata", Text),.   
-0000b070: 2020 2020 2029 0a0a 2020 2020 4070 7974       )..    @pyt
-0000b080: 6573 742e 6d61 726b 2e73 6b69 7028 2253  est.mark.skip("S
-0000b090: 7061 6e6e 6572 2064 6f65 736e 2774 2073  panner doesn't s
-0000b0a0: 7570 706f 7274 206e 6f6e 2d61 7363 6969  upport non-ascii
-0000b0b0: 2063 6861 7261 6374 6572 7322 290a 2020   characters").  
-0000b0c0: 2020 6465 6620 7465 7374 5f6c 6974 6572    def test_liter
-0000b0d0: 616c 5f6e 6f6e 5f61 7363 6969 2873 656c  al_non_ascii(sel
-0000b0e0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-0000b0f0: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-0000b100: 726b 2e73 6b69 7028 224e 6f74 2073 7570  rk.skip("Not sup
-0000b110: 706f 7274 6564 2062 7920 5370 616e 6e65  ported by Spanne
-0000b120: 7222 290a 2020 2020 6465 6620 7465 7374  r").    def test
-0000b130: 5f74 6578 745f 726f 756e 6474 7269 7028  _text_roundtrip(
-0000b140: 7365 6c66 2c20 636f 6e6e 6563 7469 6f6e  self, connection
-0000b150: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0000b160: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-0000b170: 6b2e 736b 6970 2822 4e6f 7420 7375 7070  k.skip("Not supp
-0000b180: 6f72 7465 6420 6279 2053 7061 6e6e 6572  orted by Spanner
-0000b190: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
-0000b1a0: 7465 7874 5f65 6d70 7479 5f73 7472 696e  text_empty_strin
-0000b1b0: 6773 2873 656c 662c 2063 6f6e 6e65 6374  gs(self, connect
-0000b1c0: 696f 6e29 3a0a 2020 2020 2020 2020 7061  ion):.        pa
-0000b1d0: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
-0000b1e0: 6d61 726b 2e73 6b69 7028 224e 6f74 2073  mark.skip("Not s
-0000b1f0: 7570 706f 7274 6564 2062 7920 5370 616e  upported by Span
-0000b200: 6e65 7222 290a 2020 2020 6465 6620 7465  ner").    def te
-0000b210: 7374 5f74 6578 745f 6e75 6c6c 5f73 7472  st_text_null_str
-0000b220: 696e 6773 2873 656c 662c 2063 6f6e 6e65  ings(self, conne
-0000b230: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
-0000b240: 7061 7373 0a0a 0a63 6c61 7373 204e 756d  pass...class Num
-0000b250: 6572 6963 5465 7374 285f 4e75 6d65 7269  ericTest(_Numeri
-0000b260: 6354 6573 7429 3a0a 2020 2020 4074 6573  cTest):.    @tes
-0000b270: 7469 6e67 2e66 6978 7475 7265 0a20 2020  ting.fixture.   
-0000b280: 2064 6566 2064 6f5f 6e75 6d65 7269 635f   def do_numeric_
-0000b290: 7465 7374 2873 656c 662c 206d 6574 6164  test(self, metad
-0000b2a0: 6174 612c 2063 6f6e 6e65 6374 696f 6e29  ata, connection)
-0000b2b0: 3a0a 2020 2020 2020 2020 4074 6573 7469  :.        @testi
-0000b2c0: 6e67 2e65 6d69 7473 5f77 6172 6e69 6e67  ng.emits_warning
-0000b2d0: 2872 222e 2a64 6f65 7320 5c2a 6e6f 745c  (r".*does \*not\
-0000b2e0: 2a20 7375 7070 6f72 7420 4465 6369 6d61  * support Decima
-0000b2f0: 6c20 6f62 6a65 6374 7320 6e61 7469 7665  l objects native
-0000b300: 6c79 2229 0a20 2020 2020 2020 2064 6566  ly").        def
-0000b310: 2072 756e 2874 7970 655f 2c20 696e 7075   run(type_, inpu
-0000b320: 745f 2c20 6f75 7470 7574 2c20 6669 6c74  t_, output, filt
-0000b330: 6572 5f3d 4e6f 6e65 2c20 6368 6563 6b5f  er_=None, check_
-0000b340: 7363 616c 653d 4661 6c73 6529 3a0a 2020  scale=False):.  
-0000b350: 2020 2020 2020 2020 2020 7420 3d20 5461            t = Ta
+00000820: 6865 6d79 2069 6d70 6f72 7420 7479 7065  hemy import type
+00000830: 7320 6173 2073 716c 5f74 7970 6573 0a66  s as sql_types.f
+00000840: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
+00000850: 6573 7469 6e67 2e66 6978 7475 7265 7320  esting.fixtures 
+00000860: 696d 706f 7274 2028 0a20 2020 2043 6f6d  import (.    Com
+00000870: 7075 7465 6452 6566 6c65 6374 696f 6e46  putedReflectionF
+00000880: 6978 7475 7265 5465 7374 2061 7320 5f43  ixtureTest as _C
+00000890: 6f6d 7075 7465 6452 6566 6c65 6374 696f  omputedReflectio
+000008a0: 6e46 6978 7475 7265 5465 7374 2c0a 290a  nFixtureTest,.).
+000008b0: 0a66 726f 6d20 676f 6f67 6c65 2e61 7069  .from google.api
+000008c0: 5f63 6f72 652e 6461 7465 7469 6d65 5f68  _core.datetime_h
+000008d0: 656c 7065 7273 2069 6d70 6f72 7420 4461  elpers import Da
+000008e0: 7465 7469 6d65 5769 7468 4e61 6e6f 7365  tetimeWithNanose
+000008f0: 636f 6e64 730a 0a66 726f 6d20 676f 6f67  conds..from goog
+00000900: 6c65 2e63 6c6f 7564 2069 6d70 6f72 7420  le.cloud import 
+00000910: 7370 616e 6e65 725f 6462 6170 690a 0a66  spanner_dbapi..f
+00000920: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
+00000930: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
+00000940: 745f 6374 6520 696d 706f 7274 202a 2020  t_cte import *  
+00000950: 2320 6e6f 7161 3a20 4634 3031 2c20 4634  # noqa: F401, F4
+00000960: 3033 0a66 726f 6d20 7371 6c61 6c63 6865  03.from sqlalche
+00000970: 6d79 2e74 6573 7469 6e67 2e73 7569 7465  my.testing.suite
+00000980: 2e74 6573 745f 6464 6c20 696d 706f 7274  .test_ddl import
+00000990: 202a 2020 2320 6e6f 7161 3a20 4634 3031   *  # noqa: F401
+000009a0: 2c20 4634 3033 0a66 726f 6d20 7371 6c61  , F403.from sqla
+000009b0: 6c63 6865 6d79 2e74 6573 7469 6e67 2e73  lchemy.testing.s
+000009c0: 7569 7465 2e74 6573 745f 6469 616c 6563  uite.test_dialec
+000009d0: 7420 696d 706f 7274 202a 2020 2320 6e6f  t import *  # no
+000009e0: 7161 3a20 4634 3031 2c20 4634 3033 0a66  qa: F401, F403.f
+000009f0: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
+00000a00: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
+00000a10: 745f 696e 7365 7274 2069 6d70 6f72 7420  t_insert import 
+00000a20: 2a20 2023 206e 6f71 613a 2046 3430 312c  *  # noqa: F401,
+00000a30: 2046 3430 330a 6672 6f6d 2073 716c 616c   F403.from sqlal
+00000a40: 6368 656d 792e 7465 7374 696e 672e 7375  chemy.testing.su
+00000a50: 6974 652e 7465 7374 5f72 6566 6c65 6374  ite.test_reflect
+00000a60: 696f 6e20 696d 706f 7274 202a 2020 2320  ion import *  # 
+00000a70: 6e6f 7161 3a20 4634 3031 2c20 4634 3033  noqa: F401, F403
+00000a80: 0a66 726f 6d20 7371 6c61 6c63 6865 6d79  .from sqlalchemy
+00000a90: 2e74 6573 7469 6e67 2e73 7569 7465 2e74  .testing.suite.t
+00000aa0: 6573 745f 7265 7375 6c74 7320 696d 706f  est_results impo
+00000ab0: 7274 202a 2020 2320 6e6f 7161 3a20 4634  rt *  # noqa: F4
+00000ac0: 3031 2c20 4634 3033 0a66 726f 6d20 7371  01, F403.from sq
+00000ad0: 6c61 6c63 6865 6d79 2e74 6573 7469 6e67  lalchemy.testing
+00000ae0: 2e73 7569 7465 2e74 6573 745f 7365 6c65  .suite.test_sele
+00000af0: 6374 2069 6d70 6f72 7420 2a20 2023 206e  ct import *  # n
+00000b00: 6f71 613a 2046 3430 312c 2046 3430 330a  oqa: F401, F403.
+00000b10: 6672 6f6d 2073 716c 616c 6368 656d 792e  from sqlalchemy.
+00000b20: 7465 7374 696e 672e 7375 6974 652e 7465  testing.suite.te
+00000b30: 7374 5f73 6571 7565 6e63 6520 696d 706f  st_sequence impo
+00000b40: 7274 202a 2020 2320 6e6f 7161 3a20 4634  rt *  # noqa: F4
+00000b50: 3031 2c20 4634 3033 0a66 726f 6d20 7371  01, F403.from sq
+00000b60: 6c61 6c63 6865 6d79 2e74 6573 7469 6e67  lalchemy.testing
+00000b70: 2e73 7569 7465 2e74 6573 745f 7570 6461  .suite.test_upda
+00000b80: 7465 5f64 656c 6574 6520 696d 706f 7274  te_delete import
+00000b90: 202a 2020 2320 6e6f 7161 3a20 4634 3031   *  # noqa: F401
+00000ba0: 2c20 4634 3033 0a66 726f 6d20 7371 6c61  , F403.from sqla
+00000bb0: 6c63 6865 6d79 2e74 6573 7469 6e67 2e73  lchemy.testing.s
+00000bc0: 7569 7465 2e74 6573 745f 6374 6520 696d  uite.test_cte im
+00000bd0: 706f 7274 2043 5445 5465 7374 2061 7320  port CTETest as 
+00000be0: 5f43 5445 5465 7374 0a66 726f 6d20 7371  _CTETest.from sq
+00000bf0: 6c61 6c63 6865 6d79 2e74 6573 7469 6e67  lalchemy.testing
+00000c00: 2e73 7569 7465 2e74 6573 745f 6464 6c20  .suite.test_ddl 
+00000c10: 696d 706f 7274 2054 6162 6c65 4444 4c54  import TableDDLT
+00000c20: 6573 7420 6173 205f 5461 626c 6544 444c  est as _TableDDL
+00000c30: 5465 7374 0a66 726f 6d20 7371 6c61 6c63  Test.from sqlalc
+00000c40: 6865 6d79 2e74 6573 7469 6e67 2e73 7569  hemy.testing.sui
+00000c50: 7465 2e74 6573 745f 6464 6c20 696d 706f  te.test_ddl impo
+00000c60: 7274 2028 0a20 2020 2046 7574 7572 6554  rt (.    FutureT
+00000c70: 6162 6c65 4444 4c54 6573 7420 6173 205f  ableDDLTest as _
+00000c80: 4675 7475 7265 5461 626c 6544 444c 5465  FutureTableDDLTe
+00000c90: 7374 2c0a 2020 2020 4c6f 6e67 4e61 6d65  st,.    LongName
+00000ca0: 426c 6f77 6f75 7454 6573 7420 6173 205f  BlowoutTest as _
+00000cb0: 4c6f 6e67 4e61 6d65 426c 6f77 6f75 7454  LongNameBlowoutT
+00000cc0: 6573 742c 0a29 0a66 726f 6d20 7371 6c61  est,.).from sqla
+00000cd0: 6c63 6865 6d79 2e74 6573 7469 6e67 2e73  lchemy.testing.s
+00000ce0: 7569 7465 2e74 6573 745f 7570 6461 7465  uite.test_update
+00000cf0: 5f64 656c 6574 6520 696d 706f 7274 2028  _delete import (
+00000d00: 0a20 2020 2053 696d 706c 6555 7064 6174  .    SimpleUpdat
+00000d10: 6544 656c 6574 6554 6573 7420 6173 205f  eDeleteTest as _
+00000d20: 5369 6d70 6c65 5570 6461 7465 4465 6c65  SimpleUpdateDele
+00000d30: 7465 5465 7374 2c0a 290a 6672 6f6d 2073  teTest,.).from s
+00000d40: 716c 616c 6368 656d 792e 7465 7374 696e  qlalchemy.testin
+00000d50: 672e 7375 6974 652e 7465 7374 5f64 6961  g.suite.test_dia
+00000d60: 6c65 6374 2069 6d70 6f72 7420 280a 2020  lect import (.  
+00000d70: 2020 4469 6666 6963 756c 7450 6172 616d    DifficultParam
+00000d80: 6574 6572 7354 6573 7420 6173 205f 4469  etersTest as _Di
+00000d90: 6666 6963 756c 7450 6172 616d 6574 6572  fficultParameter
+00000da0: 7354 6573 742c 0a20 2020 2045 7363 6170  sTest,.    Escap
+00000db0: 696e 6754 6573 7420 6173 205f 4573 6361  ingTest as _Esca
+00000dc0: 7069 6e67 5465 7374 2c0a 290a 6672 6f6d  pingTest,.).from
+00000dd0: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
+00000de0: 696e 672e 7375 6974 652e 7465 7374 5f69  ing.suite.test_i
+00000df0: 6e73 6572 7420 696d 706f 7274 2028 0a20  nsert import (. 
+00000e00: 2020 2049 6e73 6572 7442 6568 6176 696f     InsertBehavio
+00000e10: 7254 6573 7420 6173 205f 496e 7365 7274  rTest as _Insert
+00000e20: 4265 6861 7669 6f72 5465 7374 2c0a 290a  BehaviorTest,.).
+00000e30: 6672 6f6d 2073 716c 616c 6368 656d 792e  from sqlalchemy.
+00000e40: 7465 7374 696e 672e 7375 6974 652e 7465  testing.suite.te
+00000e50: 7374 5f73 656c 6563 7420 696d 706f 7274  st_select import
+00000e60: 2028 2020 2320 6e6f 7161 3a20 4634 3031   (  # noqa: F401
+00000e70: 2c20 4634 3033 0a20 2020 2043 6f6d 706f  , F403.    Compo
+00000e80: 756e 6453 656c 6563 7454 6573 7420 6173  undSelectTest as
+00000e90: 205f 436f 6d70 6f75 6e64 5365 6c65 6374   _CompoundSelect
+00000ea0: 5465 7374 2c0a 2020 2020 4578 6973 7473  Test,.    Exists
+00000eb0: 5465 7374 2061 7320 5f45 7869 7374 7354  Test as _ExistsT
+00000ec0: 6573 742c 0a20 2020 2046 6574 6368 4c69  est,.    FetchLi
+00000ed0: 6d69 744f 6666 7365 7454 6573 7420 6173  mitOffsetTest as
+00000ee0: 205f 4665 7463 684c 696d 6974 4f66 6673   _FetchLimitOffs
+00000ef0: 6574 5465 7374 2c0a 2020 2020 4964 656e  etTest,.    Iden
+00000f00: 7469 7479 4175 746f 696e 6372 656d 656e  tityAutoincremen
+00000f10: 7454 6573 7420 6173 205f 4964 656e 7469  tTest as _Identi
+00000f20: 7479 4175 746f 696e 6372 656d 656e 7454  tyAutoincrementT
+00000f30: 6573 742c 0a20 2020 2049 734f 7249 734e  est,.    IsOrIsN
+00000f40: 6f74 4469 7374 696e 6374 4672 6f6d 5465  otDistinctFromTe
+00000f50: 7374 2061 7320 5f49 734f 7249 734e 6f74  st as _IsOrIsNot
+00000f60: 4469 7374 696e 6374 4672 6f6d 5465 7374  DistinctFromTest
+00000f70: 2c0a 2020 2020 4c69 6b65 4675 6e63 7469  ,.    LikeFuncti
+00000f80: 6f6e 7354 6573 7420 6173 205f 4c69 6b65  onsTest as _Like
+00000f90: 4675 6e63 7469 6f6e 7354 6573 742c 0a20  FunctionsTest,. 
+00000fa0: 2020 204f 7264 6572 4279 4c61 6265 6c54     OrderByLabelT
+00000fb0: 6573 7420 6173 205f 4f72 6465 7242 794c  est as _OrderByL
+00000fc0: 6162 656c 5465 7374 2c0a 2020 2020 506f  abelTest,.    Po
+00000fd0: 7374 436f 6d70 696c 6550 6172 616d 7354  stCompileParamsT
+00000fe0: 6573 7420 6173 205f 506f 7374 436f 6d70  est as _PostComp
+00000ff0: 696c 6550 6172 616d 7354 6573 742c 0a29  ileParamsTest,.)
+00001000: 0a66 726f 6d20 7371 6c61 6c63 6865 6d79  .from sqlalchemy
+00001010: 2e74 6573 7469 6e67 2e73 7569 7465 2e74  .testing.suite.t
+00001020: 6573 745f 7265 666c 6563 7469 6f6e 2069  est_reflection i
+00001030: 6d70 6f72 7420 280a 2020 2020 436f 6d70  mport (.    Comp
+00001040: 6f6e 656e 7452 6566 6c65 6374 696f 6e54  onentReflectionT
+00001050: 6573 7445 7874 7261 2061 7320 5f43 6f6d  estExtra as _Com
+00001060: 706f 6e65 6e74 5265 666c 6563 7469 6f6e  ponentReflection
+00001070: 5465 7374 4578 7472 612c 0a20 2020 2051  TestExtra,.    Q
+00001080: 756f 7465 644e 616d 6541 7267 756d 656e  uotedNameArgumen
+00001090: 7454 6573 7420 6173 205f 5175 6f74 6564  tTest as _Quoted
+000010a0: 4e61 6d65 4172 6775 6d65 6e74 5465 7374  NameArgumentTest
+000010b0: 2c0a 2020 2020 436f 6d70 6f6e 656e 7452  ,.    ComponentR
+000010c0: 6566 6c65 6374 696f 6e54 6573 7420 6173  eflectionTest as
+000010d0: 205f 436f 6d70 6f6e 656e 7452 6566 6c65   _ComponentRefle
+000010e0: 6374 696f 6e54 6573 742c 0a20 2020 2043  ctionTest,.    C
+000010f0: 6f6d 706f 7369 7465 4b65 7952 6566 6c65  ompositeKeyRefle
+00001100: 6374 696f 6e54 6573 7420 6173 205f 436f  ctionTest as _Co
+00001110: 6d70 6f73 6974 654b 6579 5265 666c 6563  mpositeKeyReflec
+00001120: 7469 6f6e 5465 7374 2c0a 2020 2020 436f  tionTest,.    Co
+00001130: 6d70 7574 6564 5265 666c 6563 7469 6f6e  mputedReflection
+00001140: 5465 7374 2061 7320 5f43 6f6d 7075 7465  Test as _Compute
+00001150: 6452 6566 6c65 6374 696f 6e54 6573 742c  dReflectionTest,
+00001160: 0a20 2020 2048 6173 496e 6465 7854 6573  .    HasIndexTes
+00001170: 7420 6173 205f 4861 7349 6e64 6578 5465  t as _HasIndexTe
+00001180: 7374 2c0a 2020 2020 4861 7354 6162 6c65  st,.    HasTable
+00001190: 5465 7374 2061 7320 5f48 6173 5461 626c  Test as _HasTabl
+000011a0: 6554 6573 742c 0a29 0a66 726f 6d20 7371  eTest,.).from sq
+000011b0: 6c61 6c63 6865 6d79 2e74 6573 7469 6e67  lalchemy.testing
+000011c0: 2e73 7569 7465 2e74 6573 745f 7265 7375  .suite.test_resu
+000011d0: 6c74 7320 696d 706f 7274 2052 6f77 4665  lts import RowFe
+000011e0: 7463 6854 6573 7420 6173 205f 526f 7746  tchTest as _RowF
+000011f0: 6574 6368 5465 7374 0a66 726f 6d20 7371  etchTest.from sq
+00001200: 6c61 6c63 6865 6d79 2e74 6573 7469 6e67  lalchemy.testing
+00001210: 2e73 7569 7465 2e74 6573 745f 7479 7065  .suite.test_type
+00001220: 7320 696d 706f 7274 2028 2020 2320 6e6f  s import (  # no
+00001230: 7161 3a20 4634 3031 2c20 4634 3033 0a20  qa: F401, F403. 
+00001240: 2020 2042 6f6f 6c65 616e 5465 7374 2061     BooleanTest a
+00001250: 7320 5f42 6f6f 6c65 616e 5465 7374 2c0a  s _BooleanTest,.
+00001260: 2020 2020 4461 7465 5465 7374 2061 7320      DateTest as 
+00001270: 5f44 6174 6554 6573 742c 0a20 2020 205f  _DateTest,.    _
+00001280: 4461 7465 4669 7874 7572 6520 6173 205f  DateFixture as _
+00001290: 5f44 6174 6546 6978 7475 7265 2c0a 2020  _DateFixture,.  
+000012a0: 2020 4461 7465 5469 6d65 4869 7374 6f72    DateTimeHistor
+000012b0: 6963 5465 7374 2c0a 2020 2020 4461 7465  icTest,.    Date
+000012c0: 5469 6d65 436f 6572 6365 6454 6f44 6174  TimeCoercedToDat
+000012d0: 6554 696d 6554 6573 7420 6173 205f 4461  eTimeTest as _Da
+000012e0: 7465 5469 6d65 436f 6572 6365 6454 6f44  teTimeCoercedToD
+000012f0: 6174 6554 696d 6554 6573 742c 0a20 2020  ateTimeTest,.   
+00001300: 2044 6174 6554 696d 654d 6963 726f 7365   DateTimeMicrose
+00001310: 636f 6e64 7354 6573 7420 6173 205f 4461  condsTest as _Da
+00001320: 7465 5469 6d65 4d69 6372 6f73 6563 6f6e  teTimeMicrosecon
+00001330: 6473 5465 7374 2c0a 2020 2020 4461 7465  dsTest,.    Date
+00001340: 5469 6d65 5465 7374 2061 7320 5f44 6174  TimeTest as _Dat
+00001350: 6554 696d 6554 6573 742c 0a20 2020 2049  eTimeTest,.    I
+00001360: 6e74 6567 6572 5465 7374 2061 7320 5f49  ntegerTest as _I
+00001370: 6e74 6567 6572 5465 7374 2c0a 2020 2020  ntegerTest,.    
+00001380: 4a53 4f4e 5465 7374 2061 7320 5f4a 534f  JSONTest as _JSO
+00001390: 4e54 6573 742c 0a20 2020 205f 4c69 7465  NTest,.    _Lite
+000013a0: 7261 6c52 6f75 6e64 5472 6970 4669 7874  ralRoundTripFixt
+000013b0: 7572 652c 0a20 2020 204e 756d 6572 6963  ure,.    Numeric
+000013c0: 5465 7374 2061 7320 5f4e 756d 6572 6963  Test as _Numeric
+000013d0: 5465 7374 2c0a 2020 2020 5374 7269 6e67  Test,.    String
+000013e0: 5465 7374 2061 7320 5f53 7472 696e 6754  Test as _StringT
+000013f0: 6573 742c 0a20 2020 2054 6578 7454 6573  est,.    TextTes
+00001400: 7420 6173 205f 5465 7874 5465 7374 2c0a  t as _TextTest,.
+00001410: 2020 2020 5469 6d65 5465 7374 2061 7320      TimeTest as 
+00001420: 5f54 696d 6554 6573 742c 0a20 2020 2054  _TimeTest,.    T
+00001430: 696d 654d 6963 726f 7365 636f 6e64 7354  imeMicrosecondsT
+00001440: 6573 7420 6173 205f 5469 6d65 4d69 6372  est as _TimeMicr
+00001450: 6f73 6563 6f6e 6473 5465 7374 2c0a 2020  osecondsTest,.  
+00001460: 2020 5469 6d65 7374 616d 704d 6963 726f    TimestampMicro
+00001470: 7365 636f 6e64 7354 6573 742c 0a20 2020  secondsTest,.   
+00001480: 2055 6e69 636f 6465 5661 7263 6861 7254   UnicodeVarcharT
+00001490: 6573 7420 6173 205f 556e 6963 6f64 6556  est as _UnicodeV
+000014a0: 6172 6368 6172 5465 7374 2c0a 2020 2020  archarTest,.    
+000014b0: 556e 6963 6f64 6554 6578 7454 6573 7420  UnicodeTextTest 
+000014c0: 6173 205f 556e 6963 6f64 6554 6578 7454  as _UnicodeTextT
+000014d0: 6573 742c 0a20 2020 205f 556e 6963 6f64  est,.    _Unicod
+000014e0: 6546 6978 7475 7265 2061 7320 5f5f 556e  eFixture as __Un
+000014f0: 6963 6f64 6546 6978 7475 7265 2c0a 290a  icodeFixture,.).
+00001500: 6672 6f6d 2074 6573 742e 5f68 656c 7065  from test._helpe
+00001510: 7273 2069 6d70 6f72 7420 6765 745f 6462  rs import get_db
+00001520: 5f75 726c 2c20 6765 745f 7072 6f6a 6563  _url, get_projec
+00001530: 740a 0a63 6f6e 6669 672e 7465 7374 5f73  t..config.test_s
+00001540: 6368 656d 6120 3d20 2222 0a0a 0a63 6c61  chema = ""...cla
+00001550: 7373 2042 6f6f 6c65 616e 5465 7374 285f  ss BooleanTest(_
+00001560: 426f 6f6c 6561 6e54 6573 7429 3a0a 2020  BooleanTest):.  
+00001570: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+00001580: 6b69 7028 0a20 2020 2020 2020 2022 5468  kip(.        "Th
+00001590: 6520 6f72 6967 696e 616c 2074 6573 7420  e original test 
+000015a0: 6361 7365 2077 6173 2073 706c 6974 2069  case was split i
+000015b0: 6e74 6f20 3220 7061 7274 733a 2022 0a20  nto 2 parts: ". 
+000015c0: 2020 2020 2020 2022 7465 7374 5f72 656e         "test_ren
+000015d0: 6465 725f 6c69 7465 7261 6c5f 626f 6f6c  der_literal_bool
+000015e0: 5f74 7275 6520 616e 6420 7465 7374 5f72  _true and test_r
+000015f0: 656e 6465 725f 6c69 7465 7261 6c5f 626f  ender_literal_bo
+00001600: 6f6c 5f66 616c 7365 220a 2020 2020 290a  ol_false".    ).
+00001610: 2020 2020 6465 6620 7465 7374 5f72 656e      def test_ren
+00001620: 6465 725f 6c69 7465 7261 6c5f 626f 6f6c  der_literal_bool
+00001630: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00001640: 7061 7373 0a0a 2020 2020 6465 6620 7465  pass..    def te
+00001650: 7374 5f72 656e 6465 725f 6c69 7465 7261  st_render_litera
+00001660: 6c5f 626f 6f6c 5f74 7275 6528 7365 6c66  l_bool_true(self
+00001670: 2c20 6c69 7465 7261 6c5f 726f 756e 645f  , literal_round_
+00001680: 7472 6970 293a 0a20 2020 2020 2020 2022  trip):.        "
+00001690: 2222 0a20 2020 2020 2020 2053 5041 4e4e  "".        SPANN
+000016a0: 4552 204f 5645 5252 4944 453a 0a0a 2020  ER OVERRIDE:..  
+000016b0: 2020 2020 2020 436c 6f75 6420 5370 616e        Cloud Span
+000016c0: 6e65 7220 7375 7070 6f72 7473 2074 6162  ner supports tab
+000016d0: 6c65 7320 7769 7468 2061 6e20 656d 7074  les with an empt
+000016e0: 7920 7072 696d 6172 7920 6b65 792c 2062  y primary key, b
+000016f0: 7574 0a20 2020 2020 2020 206f 6e6c 7920  ut.        only 
+00001700: 6120 7369 6e67 6c65 2072 6f77 2063 616e  a single row can
+00001710: 2062 6520 696e 7365 7274 6564 2069 6e74   be inserted int
+00001720: 6f20 7375 6368 2061 2074 6162 6c65 202d  o such a table -
+00001730: 0a20 2020 2020 2020 2066 6f6c 6c6f 7769  .        followi
+00001740: 6e67 2069 6e73 6572 7469 6f6e 7320 7769  ng insertions wi
+00001750: 6c6c 2066 6169 6c20 7769 7468 2060 526f  ll fail with `Ro
+00001760: 7720 5b5d 2061 6c72 6561 6479 2065 7869  w [] already exi
+00001770: 7374 7322 2e0a 2020 2020 2020 2020 4f76  sts"..        Ov
+00001780: 6572 7269 6469 6e67 2074 6865 2074 6573  erriding the tes
+00001790: 7420 746f 2061 766f 6964 2074 6865 2073  t to avoid the s
+000017a0: 616d 6520 6661 696c 7572 652e 0a20 2020  ame failure..   
+000017b0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000017c0: 206c 6974 6572 616c 5f72 6f75 6e64 5f74   literal_round_t
+000017d0: 7269 7028 426f 6f6c 6561 6e28 292c 205b  rip(Boolean(), [
+000017e0: 5472 7565 5d2c 205b 5472 7565 5d29 0a0a  True], [True])..
+000017f0: 2020 2020 6465 6620 7465 7374 5f72 656e      def test_ren
+00001800: 6465 725f 6c69 7465 7261 6c5f 626f 6f6c  der_literal_bool
+00001810: 5f66 616c 7365 2873 656c 662c 206c 6974  _false(self, lit
+00001820: 6572 616c 5f72 6f75 6e64 5f74 7269 7029  eral_round_trip)
+00001830: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00001840: 2020 2020 2020 5350 414e 4e45 5220 4f56        SPANNER OV
+00001850: 4552 5249 4445 3a0a 0a20 2020 2020 2020  ERRIDE:..       
+00001860: 2043 6c6f 7564 2053 7061 6e6e 6572 2073   Cloud Spanner s
+00001870: 7570 706f 7274 7320 7461 626c 6573 2077  upports tables w
+00001880: 6974 6820 616e 2065 6d70 7479 2070 7269  ith an empty pri
+00001890: 6d61 7279 206b 6579 2c20 6275 740a 2020  mary key, but.  
+000018a0: 2020 2020 2020 6f6e 6c79 2061 2073 696e        only a sin
+000018b0: 676c 6520 726f 7720 6361 6e20 6265 2069  gle row can be i
+000018c0: 6e73 6572 7465 6420 696e 746f 2073 7563  nserted into suc
+000018d0: 6820 6120 7461 626c 6520 2d0a 2020 2020  h a table -.    
+000018e0: 2020 2020 666f 6c6c 6f77 696e 6720 696e      following in
+000018f0: 7365 7274 696f 6e73 2077 696c 6c20 6661  sertions will fa
+00001900: 696c 2077 6974 6820 6052 6f77 205b 5d20  il with `Row [] 
+00001910: 616c 7265 6164 7920 6578 6973 7473 222e  already exists".
+00001920: 0a20 2020 2020 2020 204f 7665 7272 6964  .        Overrid
+00001930: 696e 6720 7468 6520 7465 7374 2074 6f20  ing the test to 
+00001940: 6176 6f69 6420 7468 6520 7361 6d65 2066  avoid the same f
+00001950: 6169 6c75 7265 2e0a 2020 2020 2020 2020  ailure..        
+00001960: 2222 220a 2020 2020 2020 2020 6c69 7465  """.        lite
+00001970: 7261 6c5f 726f 756e 645f 7472 6970 2842  ral_round_trip(B
+00001980: 6f6f 6c65 616e 2829 2c20 5b46 616c 7365  oolean(), [False
+00001990: 5d2c 205b 4661 6c73 655d 290a 0a20 2020  ], [False])..   
+000019a0: 2040 7079 7465 7374 2e6d 6172 6b2e 736b   @pytest.mark.sk
+000019b0: 6970 2822 4e6f 7420 7375 7070 6f72 7465  ip("Not supporte
+000019c0: 6420 6279 2043 6c6f 7564 2053 7061 6e6e  d by Cloud Spann
+000019d0: 6572 2229 0a20 2020 2064 6566 2074 6573  er").    def tes
+000019e0: 745f 7768 6572 6563 6c61 7573 6528 7365  t_whereclause(se
+000019f0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+00001a00: 730a 0a0a 636c 6173 7320 436f 6d70 6f6e  s...class Compon
+00001a10: 656e 7452 6566 6c65 6374 696f 6e54 6573  entReflectionTes
+00001a20: 7445 7874 7261 285f 436f 6d70 6f6e 656e  tExtra(_Componen
+00001a30: 7452 6566 6c65 6374 696f 6e54 6573 7445  tReflectionTestE
+00001a40: 7874 7261 293a 0a20 2020 2040 7465 7374  xtra):.    @test
+00001a50: 696e 672e 7265 7175 6972 6573 2e74 6162  ing.requires.tab
+00001a60: 6c65 5f72 6566 6c65 6374 696f 6e0a 2020  le_reflection.  
+00001a70: 2020 6465 6620 7465 7374 5f6e 756c 6c61    def test_nulla
+00001a80: 626c 655f 7265 666c 6563 7469 6f6e 2873  ble_reflection(s
+00001a90: 656c 662c 2063 6f6e 6e65 6374 696f 6e2c  elf, connection,
+00001aa0: 206d 6574 6164 6174 6129 3a0a 2020 2020   metadata):.    
+00001ab0: 2020 2020 7420 3d20 5461 626c 6528 0a20      t = Table(. 
+00001ac0: 2020 2020 2020 2020 2020 2022 7422 2c0a             "t",.
+00001ad0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+00001ae0: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
+00001af0: 2020 436f 6c75 6d6e 2822 6122 2c20 496e    Column("a", In
+00001b00: 7465 6765 722c 206e 756c 6c61 626c 653d  teger, nullable=
+00001b10: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
+00001b20: 2020 2043 6f6c 756d 6e28 2262 222c 2049     Column("b", I
+00001b30: 6e74 6567 6572 2c20 6e75 6c6c 6162 6c65  nteger, nullable
+00001b40: 3d46 616c 7365 292c 0a20 2020 2020 2020  =False),.       
+00001b50: 2029 0a20 2020 2020 2020 2074 2e63 7265   ).        t.cre
+00001b60: 6174 6528 636f 6e6e 6563 7469 6f6e 290a  ate(connection).
+00001b70: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
+00001b80: 6f6e 2e63 6f6e 6e65 6374 696f 6e2e 636f  on.connection.co
+00001b90: 6d6d 6974 2829 0a20 2020 2020 2020 2065  mmit().        e
+00001ba0: 715f 280a 2020 2020 2020 2020 2020 2020  q_(.            
+00001bb0: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
+00001bc0: 2020 2020 2020 2863 6f6c 5b22 6e61 6d65        (col["name
+00001bd0: 225d 2c20 636f 6c5b 226e 756c 6c61 626c  "], col["nullabl
+00001be0: 6522 5d29 0a20 2020 2020 2020 2020 2020  e"]).           
+00001bf0: 2020 2020 2066 6f72 2063 6f6c 2069 6e20       for col in 
+00001c00: 696e 7370 6563 7428 636f 6e6e 6563 7469  inspect(connecti
+00001c10: 6f6e 292e 6765 745f 636f 6c75 6d6e 7328  on).get_columns(
+00001c20: 2274 2229 0a20 2020 2020 2020 2020 2020  "t").           
+00001c30: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00001c40: 7b22 6122 3a20 5472 7565 2c20 2262 223a  {"a": True, "b":
+00001c50: 2046 616c 7365 7d2c 0a20 2020 2020 2020   False},.       
+00001c60: 2029 0a0a 2020 2020 6465 6620 5f74 7970   )..    def _typ
+00001c70: 655f 726f 756e 645f 7472 6970 2873 656c  e_round_trip(sel
+00001c80: 662c 2063 6f6e 6e65 6374 696f 6e2c 206d  f, connection, m
+00001c90: 6574 6164 6174 612c 202a 7479 7065 7329  etadata, *types)
+00001ca0: 3a0a 2020 2020 2020 2020 7420 3d20 5461  :.        t = Ta
+00001cb0: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
+00001cc0: 2022 7422 2c20 6d65 7461 6461 7461 2c20   "t", metadata, 
+00001cd0: 2a5b 436f 6c75 6d6e 2822 7425 6422 2025  *[Column("t%d" %
+00001ce0: 2069 2c20 7479 7065 5f29 2066 6f72 2069   i, type_) for i
+00001cf0: 2c20 7479 7065 5f20 696e 2065 6e75 6d65  , type_ in enume
+00001d00: 7261 7465 2874 7970 6573 295d 0a20 2020  rate(types)].   
+00001d10: 2020 2020 2029 0a20 2020 2020 2020 2074       ).        t
+00001d20: 2e63 7265 6174 6528 636f 6e6e 6563 7469  .create(connecti
+00001d30: 6f6e 290a 2020 2020 2020 2020 636f 6e6e  on).        conn
+00001d40: 6563 7469 6f6e 2e63 6f6e 6e65 6374 696f  ection.connectio
+00001d50: 6e2e 636f 6d6d 6974 2829 0a0a 2020 2020  n.commit()..    
+00001d60: 2020 2020 7265 7475 726e 205b 635b 2274      return [c["t
+00001d70: 7970 6522 5d20 666f 7220 6320 696e 2069  ype"] for c in i
+00001d80: 6e73 7065 6374 2863 6f6e 6e65 6374 696f  nspect(connectio
+00001d90: 6e29 2e67 6574 5f63 6f6c 756d 6e73 2822  n).get_columns("
+00001da0: 7422 295d 0a0a 2020 2020 4074 6573 7469  t")]..    @testi
+00001db0: 6e67 2e72 6571 7569 7265 732e 7461 626c  ng.requires.tabl
+00001dc0: 655f 7265 666c 6563 7469 6f6e 0a20 2020  e_reflection.   
+00001dd0: 2064 6566 2074 6573 745f 6e75 6d65 7269   def test_numeri
+00001de0: 635f 7265 666c 6563 7469 6f6e 2873 656c  c_reflection(sel
+00001df0: 662c 2063 6f6e 6e65 6374 696f 6e2c 206d  f, connection, m
+00001e00: 6574 6164 6174 6129 3a0a 2020 2020 2020  etadata):.      
+00001e10: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
+00001e20: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
+00001e30: 0a20 2020 2020 2020 2053 7061 6e6e 6572  .        Spanner
+00001e40: 2064 6566 696e 6573 204e 554d 4552 4943   defines NUMERIC
+00001e50: 2074 7970 6520 7769 7468 2074 6865 2063   type with the c
+00001e60: 6f6e 7374 616e 7420 7072 6563 6973 696f  onstant precisio
+00001e70: 6e3d 3338 0a20 2020 2020 2020 2061 6e64  n=38.        and
+00001e80: 2073 6361 6c65 3d39 2e20 4f76 6572 7269   scale=9. Overri
+00001e90: 6469 6e67 2074 6865 2074 6573 7420 746f  ding the test to
+00001ea0: 2063 6865 636b 2069 6620 7468 6520 4e55   check if the NU
+00001eb0: 4d45 5249 430a 2020 2020 2020 2020 636f  MERIC.        co
+00001ec0: 6c75 6d6e 2069 7320 7375 6363 6573 7366  lumn is successf
+00001ed0: 756c 6c79 2063 7265 6174 6564 2061 6e64  ully created and
+00001ee0: 2068 6173 2064 696d 656e 7369 6f6e 730a   has dimensions.
+00001ef0: 2020 2020 2020 2020 636f 7272 6563 7420          correct 
+00001f00: 666f 7220 436c 6f75 6420 5370 616e 6e65  for Cloud Spanne
+00001f10: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
+00001f20: 2020 2020 2020 2066 6f72 2074 7970 2069         for typ i
+00001f30: 6e20 7365 6c66 2e5f 7479 7065 5f72 6f75  n self._type_rou
+00001f40: 6e64 5f74 7269 7028 636f 6e6e 6563 7469  nd_trip(connecti
+00001f50: 6f6e 2c20 6d65 7461 6461 7461 2c20 4e75  on, metadata, Nu
+00001f60: 6d65 7269 6328 3138 2c20 3529 293a 0a20  meric(18, 5)):. 
+00001f70: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00001f80: 7420 6973 696e 7374 616e 6365 2874 7970  t isinstance(typ
+00001f90: 2c20 4e75 6d65 7269 6329 0a20 2020 2020  , Numeric).     
+00001fa0: 2020 2020 2020 2065 715f 2874 7970 2e70         eq_(typ.p
+00001fb0: 7265 6369 7369 6f6e 2c20 3338 290a 2020  recision, 38).  
+00001fc0: 2020 2020 2020 2020 2020 6571 5f28 7479            eq_(ty
+00001fd0: 702e 7363 616c 652c 2039 290a 0a20 2020  p.scale, 9)..   
+00001fe0: 2040 7465 7374 696e 672e 7265 7175 6972   @testing.requir
+00001ff0: 6573 2e74 6162 6c65 5f72 6566 6c65 6374  es.table_reflect
+00002000: 696f 6e0a 2020 2020 6465 6620 7465 7374  ion.    def test
+00002010: 5f62 696e 6172 795f 7265 666c 6563 7469  _binary_reflecti
+00002020: 6f6e 2873 656c 662c 2063 6f6e 6e65 6374  on(self, connect
+00002030: 696f 6e2c 206d 6574 6164 6174 6129 3a0a  ion, metadata):.
+00002040: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00002050: 2020 2020 4368 6563 6b20 7468 6174 2061      Check that a
+00002060: 2042 5954 4553 2063 6f6c 756d 6e20 7769   BYTES column wi
+00002070: 7468 2061 6e20 6578 706c 6963 6974 6c79  th an explicitly
+00002080: 0a20 2020 2020 2020 2073 6574 2073 697a  .        set siz
+00002090: 6520 6973 2063 6f72 7265 6374 6c79 2072  e is correctly r
+000020a0: 6566 6c65 6374 6564 2e0a 2020 2020 2020  eflected..      
+000020b0: 2020 2222 220a 2020 2020 2020 2020 666f    """.        fo
+000020c0: 7220 7479 7020 696e 2073 656c 662e 5f74  r typ in self._t
+000020d0: 7970 655f 726f 756e 645f 7472 6970 2863  ype_round_trip(c
+000020e0: 6f6e 6e65 6374 696f 6e2c 206d 6574 6164  onnection, metad
+000020f0: 6174 612c 204c 6172 6765 4269 6e61 7279  ata, LargeBinary
+00002100: 2832 3029 293a 0a20 2020 2020 2020 2020  (20)):.         
+00002110: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
+00002120: 616e 6365 2874 7970 2c20 4c61 7267 6542  ance(typ, LargeB
+00002130: 696e 6172 7929 0a20 2020 2020 2020 2020  inary).         
+00002140: 2020 2065 715f 2874 7970 2e6c 656e 6774     eq_(typ.lengt
+00002150: 682c 2032 3029 0a0a 0a63 6c61 7373 2043  h, 20)...class C
+00002160: 6f6d 706f 6e65 6e74 5265 666c 6563 7469  omponentReflecti
+00002170: 6f6e 5465 7374 285f 436f 6d70 6f6e 656e  onTest(_Componen
+00002180: 7452 6566 6c65 6374 696f 6e54 6573 7429  tReflectionTest)
+00002190: 3a0a 2020 2020 4063 6c61 7373 6d65 7468  :.    @classmeth
+000021a0: 6f64 0a20 2020 2064 6566 2064 6566 696e  od.    def defin
+000021b0: 655f 7669 6577 7328 636c 732c 206d 6574  e_views(cls, met
+000021c0: 6164 6174 612c 2073 6368 656d 6129 3a0a  adata, schema):.
+000021d0: 2020 2020 2020 2020 7461 626c 655f 696e          table_in
+000021e0: 666f 203d 207b 0a20 2020 2020 2020 2020  fo = {.         
+000021f0: 2020 2022 7573 6572 7322 3a20 5b22 7573     "users": ["us
+00002200: 6572 5f69 6422 2c20 2274 6573 7431 222c  er_id", "test1",
+00002210: 2022 7465 7374 3222 5d2c 0a20 2020 2020   "test2"],.     
+00002220: 2020 2020 2020 2022 656d 6169 6c5f 6164         "email_ad
+00002230: 6472 6573 7365 7322 3a20 5b22 6164 6472  dresses": ["addr
+00002240: 6573 735f 6964 222c 2022 7265 6d6f 7465  ess_id", "remote
+00002250: 5f75 7365 725f 6964 222c 2022 656d 6169  _user_id", "emai
+00002260: 6c5f 6164 6472 6573 7322 5d2c 0a20 2020  l_address"],.   
+00002270: 2020 2020 207d 0a20 2020 2020 2020 2069       }.        i
+00002280: 6620 7465 7374 696e 672e 7265 7175 6972  f testing.requir
+00002290: 6573 2e73 656c 665f 7265 6665 7265 6e74  es.self_referent
+000022a0: 6961 6c5f 666f 7265 6967 6e5f 6b65 7973  ial_foreign_keys
+000022b0: 2e65 6e61 626c 6564 3a0a 2020 2020 2020  .enabled:.      
+000022c0: 2020 2020 2020 7461 626c 655f 696e 666f        table_info
+000022d0: 5b22 7573 6572 7322 5d20 3d20 7461 626c  ["users"] = tabl
+000022e0: 655f 696e 666f 5b22 7573 6572 7322 5d20  e_info["users"] 
+000022f0: 2b20 5b22 7061 7265 6e74 5f75 7365 725f  + ["parent_user_
+00002300: 6964 225d 0a20 2020 2020 2020 2066 6f72  id"].        for
+00002310: 2074 6162 6c65 5f6e 616d 6520 696e 2028   table_name in (
+00002320: 2275 7365 7273 222c 2022 656d 6169 6c5f  "users", "email_
+00002330: 6164 6472 6573 7365 7322 293a 0a20 2020  addresses"):.   
+00002340: 2020 2020 2020 2020 2066 756c 6c6e 616d           fullnam
+00002350: 6520 3d20 7461 626c 655f 6e61 6d65 0a20  e = table_name. 
+00002360: 2020 2020 2020 2020 2020 2069 6620 7363             if sc
+00002370: 6865 6d61 3a0a 2020 2020 2020 2020 2020  hema:.          
+00002380: 2020 2020 2020 6675 6c6c 6e61 6d65 203d        fullname =
+00002390: 2022 2573 2e25 7322 2025 2028 7363 6865   "%s.%s" % (sche
+000023a0: 6d61 2c20 7461 626c 655f 6e61 6d65 290a  ma, table_name).
+000023b0: 2020 2020 2020 2020 2020 2020 7669 6577              view
+000023c0: 5f6e 616d 6520 3d20 6675 6c6c 6e61 6d65  _name = fullname
+000023d0: 202b 2022 5f76 220a 2020 2020 2020 2020   + "_v".        
+000023e0: 2020 2020 636f 6c75 6d6e 7320 3d20 2222      columns = ""
+000023f0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00002400: 2063 6f6c 756d 6e20 696e 2074 6162 6c65   column in table
+00002410: 5f69 6e66 6f5b 7461 626c 655f 6e61 6d65  _info[table_name
+00002420: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00002430: 2020 2073 746d 7420 3d20 7461 626c 655f     stmt = table_
+00002440: 6e61 6d65 202b 2022 2e22 202b 2063 6f6c  name + "." + col
+00002450: 756d 6e20 2b20 2220 4153 2022 202b 2063  umn + " AS " + c
+00002460: 6f6c 756d 6e0a 2020 2020 2020 2020 2020  olumn.          
+00002470: 2020 2020 2020 6966 2063 6f6c 756d 6e73        if columns
+00002480: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002490: 2020 2020 2020 636f 6c75 6d6e 7320 3d20        columns = 
+000024a0: 636f 6c75 6d6e 7320 2b20 222c 2022 202b  columns + ", " +
+000024b0: 2073 746d 740a 2020 2020 2020 2020 2020   stmt.          
+000024c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024e0: 636f 6c75 6d6e 7320 3d20 7374 6d74 0a20  columns = stmt. 
+000024f0: 2020 2020 2020 2020 2020 2071 7565 7279             query
+00002500: 203d 2066 2222 2243 5245 4154 4520 5649   = f"""CREATE VI
+00002510: 4557 207b 7669 6577 5f6e 616d 657d 0a20  EW {view_name}. 
+00002520: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+00002530: 514c 2053 4543 5552 4954 5920 494e 564f  QL SECURITY INVO
+00002540: 4b45 520a 2020 2020 2020 2020 2020 2020  KER.            
+00002550: 2020 2020 4153 2053 454c 4543 5420 7b63      AS SELECT {c
+00002560: 6f6c 756d 6e73 7d0a 2020 2020 2020 2020  olumns}.        
+00002570: 2020 2020 2020 2020 4652 4f4d 207b 6675          FROM {fu
+00002580: 6c6c 6e61 6d65 7d22 2222 0a0a 2020 2020  llname}"""..    
+00002590: 2020 2020 2020 2020 6576 656e 742e 6c69          event.li
+000025a0: 7374 656e 286d 6574 6164 6174 612c 2022  sten(metadata, "
+000025b0: 6166 7465 725f 6372 6561 7465 222c 2044  after_create", D
+000025c0: 444c 2871 7565 7279 2929 0a20 2020 2020  DL(query)).     
+000025d0: 2020 2020 2020 2065 7665 6e74 2e6c 6973         event.lis
+000025e0: 7465 6e28 6d65 7461 6461 7461 2c20 2262  ten(metadata, "b
+000025f0: 6566 6f72 655f 6472 6f70 222c 2044 444c  efore_drop", DDL
+00002600: 2822 4452 4f50 2056 4945 5720 2573 2220  ("DROP VIEW %s" 
+00002610: 2520 7669 6577 5f6e 616d 6529 290a 0a20  % view_name)).. 
+00002620: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00002630: 2020 2020 6465 6620 6465 6669 6e65 5f74      def define_t
+00002640: 6162 6c65 7328 636c 732c 206d 6574 6164  ables(cls, metad
+00002650: 6174 6129 3a0a 2020 2020 2020 2020 636c  ata):.        cl
+00002660: 732e 6465 6669 6e65 5f72 6566 6c65 6374  s.define_reflect
+00002670: 6564 5f74 6162 6c65 7328 6d65 7461 6461  ed_tables(metada
+00002680: 7461 2c20 4e6f 6e65 290a 0a20 2020 2040  ta, None)..    @
+00002690: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+000026a0: 6465 6620 6465 6669 6e65 5f72 6566 6c65  def define_refle
+000026b0: 6374 6564 5f74 6162 6c65 7328 636c 732c  cted_tables(cls,
+000026c0: 206d 6574 6164 6174 612c 2073 6368 656d   metadata, schem
+000026d0: 6129 3a0a 2020 2020 2020 2020 6966 2073  a):.        if s
+000026e0: 6368 656d 613a 0a20 2020 2020 2020 2020  chema:.         
+000026f0: 2020 2073 6368 656d 615f 7072 6566 6978     schema_prefix
+00002700: 203d 2073 6368 656d 6120 2b20 222e 220a   = schema + ".".
+00002710: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00002720: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
+00002730: 5f70 7265 6669 7820 3d20 2222 0a0a 2020  _prefix = ""..  
+00002740: 2020 2020 2020 6966 2074 6573 7469 6e67        if testing
+00002750: 2e72 6571 7569 7265 732e 7365 6c66 5f72  .requires.self_r
+00002760: 6566 6572 656e 7469 616c 5f66 6f72 6569  eferential_forei
+00002770: 676e 5f6b 6579 732e 656e 6162 6c65 643a  gn_keys.enabled:
+00002780: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+00002790: 7273 203d 2054 6162 6c65 280a 2020 2020  rs = Table(.    
+000027a0: 2020 2020 2020 2020 2020 2020 2275 7365              "use
+000027b0: 7273 222c 0a20 2020 2020 2020 2020 2020  rs",.           
+000027c0: 2020 2020 206d 6574 6164 6174 612c 0a20       metadata,. 
+000027d0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+000027e0: 6f6c 756d 6e28 2275 7365 725f 6964 222c  olumn("user_id",
+000027f0: 2073 716c 616c 6368 656d 792e 494e 542c   sqlalchemy.INT,
+00002800: 2070 7269 6d61 7279 5f6b 6579 3d54 7275   primary_key=Tru
+00002810: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+00002820: 2020 2020 436f 6c75 6d6e 2822 7465 7374      Column("test
+00002830: 3122 2c20 7371 6c61 6c63 6865 6d79 2e43  1", sqlalchemy.C
+00002840: 4841 5228 3529 2c20 6e75 6c6c 6162 6c65  HAR(5), nullable
+00002850: 3d46 616c 7365 292c 0a20 2020 2020 2020  =False),.       
+00002860: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00002870: 2274 6573 7432 222c 2073 716c 616c 6368  "test2", sqlalch
+00002880: 656d 792e 466c 6f61 7428 3529 2c20 6e75  emy.Float(5), nu
+00002890: 6c6c 6162 6c65 3d46 616c 7365 292c 0a20  llable=False),. 
+000028a0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+000028b0: 6f6c 756d 6e28 0a20 2020 2020 2020 2020  olumn(.         
+000028c0: 2020 2020 2020 2020 2020 2022 7061 7265             "pare
+000028d0: 6e74 5f75 7365 725f 6964 222c 0a20 2020  nt_user_id",.   
+000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028f0: 2073 716c 616c 6368 656d 792e 496e 7465   sqlalchemy.Inte
+00002900: 6765 722c 0a20 2020 2020 2020 2020 2020  ger,.           
+00002910: 2020 2020 2020 2020 2073 716c 616c 6368           sqlalch
+00002920: 656d 792e 466f 7265 6967 6e4b 6579 280a  emy.ForeignKey(.
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: 2020 2020 2020 2020 2225 7375 7365 7273          "%susers
+00002950: 2e75 7365 725f 6964 2220 2520 7363 6865  .user_id" % sche
+00002960: 6d61 5f70 7265 6669 782c 206e 616d 653d  ma_prefix, name=
+00002970: 2275 7365 725f 6964 5f66 6b22 0a20 2020  "user_id_fk".   
+00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002990: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+000029a0: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+000029b0: 2020 2020 2020 2073 6368 656d 613d 7363         schema=sc
+000029c0: 6865 6d61 2c0a 2020 2020 2020 2020 2020  hema,.          
+000029d0: 2020 2020 2020 7465 7374 5f6e 6565 6473        test_needs
+000029e0: 5f66 6b3d 5472 7565 2c0a 2020 2020 2020  _fk=True,.      
+000029f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00002a00: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00002a10: 2020 7573 6572 7320 3d20 5461 626c 6528    users = Table(
+00002a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a30: 2022 7573 6572 7322 2c0a 2020 2020 2020   "users",.      
+00002a40: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
+00002a50: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+00002a60: 2020 2020 436f 6c75 6d6e 2822 7573 6572      Column("user
+00002a70: 5f69 6422 2c20 7371 6c61 6c63 6865 6d79  _id", sqlalchemy
+00002a80: 2e49 4e54 2c20 7072 696d 6172 795f 6b65  .INT, primary_ke
+00002a90: 793d 5472 7565 292c 0a20 2020 2020 2020  y=True),.       
+00002aa0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00002ab0: 2274 6573 7431 222c 2073 716c 616c 6368  "test1", sqlalch
+00002ac0: 656d 792e 4348 4152 2835 292c 206e 756c  emy.CHAR(5), nul
+00002ad0: 6c61 626c 653d 4661 6c73 6529 2c0a 2020  lable=False),.  
+00002ae0: 2020 2020 2020 2020 2020 2020 2020 436f                Co
+00002af0: 6c75 6d6e 2822 7465 7374 3222 2c20 7371  lumn("test2", sq
+00002b00: 6c61 6c63 6865 6d79 2e46 6c6f 6174 2835  lalchemy.Float(5
+00002b10: 292c 206e 756c 6c61 626c 653d 4661 6c73  ), nullable=Fals
+00002b20: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+00002b30: 2020 2020 7363 6865 6d61 3d73 6368 656d      schema=schem
+00002b40: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+00002b50: 2020 2074 6573 745f 6e65 6564 735f 666b     test_needs_fk
+00002b60: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00002b70: 2020 2029 0a0a 2020 2020 2020 2020 5461     )..        Ta
+00002b80: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
+00002b90: 2022 6469 6e67 616c 696e 6773 222c 0a20   "dingalings",. 
+00002ba0: 2020 2020 2020 2020 2020 206d 6574 6164             metad
+00002bb0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+00002bc0: 2043 6f6c 756d 6e28 2264 696e 6761 6c69   Column("dingali
+00002bd0: 6e67 5f69 6422 2c20 7371 6c61 6c63 6865  ng_id", sqlalche
+00002be0: 6d79 2e49 6e74 6567 6572 2c20 7072 696d  my.Integer, prim
+00002bf0: 6172 795f 6b65 793d 5472 7565 292c 0a20  ary_key=True),. 
+00002c00: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00002c10: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+00002c20: 2020 2022 6164 6472 6573 735f 6964 222c     "address_id",
+00002c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c40: 2073 716c 616c 6368 656d 792e 496e 7465   sqlalchemy.Inte
+00002c50: 6765 722c 0a20 2020 2020 2020 2020 2020  ger,.           
+00002c60: 2020 2020 2073 716c 616c 6368 656d 792e       sqlalchemy.
+00002c70: 466f 7265 6967 6e4b 6579 2822 2573 656d  ForeignKey("%sem
+00002c80: 6169 6c5f 6164 6472 6573 7365 732e 6164  ail_addresses.ad
+00002c90: 6472 6573 735f 6964 2220 2520 7363 6865  dress_id" % sche
+00002ca0: 6d61 5f70 7265 6669 7829 2c0a 2020 2020  ma_prefix),.    
+00002cb0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00002cc0: 2020 2020 2020 2043 6f6c 756d 6e28 2264         Column("d
+00002cd0: 6174 6122 2c20 7371 6c61 6c63 6865 6d79  ata", sqlalchemy
+00002ce0: 2e53 7472 696e 6728 3330 2929 2c0a 2020  .String(30)),.  
+00002cf0: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
+00002d00: 3d73 6368 656d 612c 0a20 2020 2020 2020  =schema,.       
+00002d10: 2020 2020 2074 6573 745f 6e65 6564 735f       test_needs_
+00002d20: 666b 3d54 7275 652c 0a20 2020 2020 2020  fk=True,.       
+00002d30: 2029 0a20 2020 2020 2020 2054 6162 6c65   ).        Table
+00002d40: 280a 2020 2020 2020 2020 2020 2020 2265  (.            "e
+00002d50: 6d61 696c 5f61 6464 7265 7373 6573 222c  mail_addresses",
+00002d60: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+00002d70: 6164 6174 612c 0a20 2020 2020 2020 2020  adata,.         
+00002d80: 2020 2043 6f6c 756d 6e28 2261 6464 7265     Column("addre
+00002d90: 7373 5f69 6422 2c20 7371 6c61 6c63 6865  ss_id", sqlalche
+00002da0: 6d79 2e49 6e74 6567 6572 2c20 7072 696d  my.Integer, prim
+00002db0: 6172 795f 6b65 793d 5472 7565 292c 0a20  ary_key=True),. 
+00002dc0: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00002dd0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+00002de0: 2020 2022 7265 6d6f 7465 5f75 7365 725f     "remote_user_
+00002df0: 6964 222c 0a20 2020 2020 2020 2020 2020  id",.           
+00002e00: 2020 2020 2073 716c 616c 6368 656d 792e       sqlalchemy.
+00002e10: 496e 7465 6765 722c 0a20 2020 2020 2020  Integer,.       
+00002e20: 2020 2020 2020 2020 2073 716c 616c 6368           sqlalch
+00002e30: 656d 792e 466f 7265 6967 6e4b 6579 2875  emy.ForeignKey(u
+00002e40: 7365 7273 2e63 2e75 7365 725f 6964 292c  sers.c.user_id),
+00002e50: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
+00002e60: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
+00002e70: 6d6e 2822 656d 6169 6c5f 6164 6472 6573  mn("email_addres
+00002e80: 7322 2c20 7371 6c61 6c63 6865 6d79 2e53  s", sqlalchemy.S
+00002e90: 7472 696e 6728 3230 2929 2c0a 2020 2020  tring(20)),.    
+00002ea0: 2020 2020 2020 2020 7371 6c61 6c63 6865          sqlalche
+00002eb0: 6d79 2e50 7269 6d61 7279 4b65 7943 6f6e  my.PrimaryKeyCon
+00002ec0: 7374 7261 696e 7428 2261 6464 7265 7373  straint("address
+00002ed0: 5f69 6422 2c20 6e61 6d65 3d22 656d 6169  _id", name="emai
+00002ee0: 6c5f 6164 5f70 6b22 292c 0a20 2020 2020  l_ad_pk"),.     
+00002ef0: 2020 2020 2020 2073 6368 656d 613d 7363         schema=sc
+00002f00: 6865 6d61 2c0a 2020 2020 2020 2020 2020  hema,.          
+00002f10: 2020 7465 7374 5f6e 6565 6473 5f66 6b3d    test_needs_fk=
+00002f20: 5472 7565 2c0a 2020 2020 2020 2020 290a  True,.        ).
+00002f30: 2020 2020 2020 2020 5461 626c 6528 0a20          Table(. 
+00002f40: 2020 2020 2020 2020 2020 2022 636f 6d6d             "comm
+00002f50: 656e 745f 7465 7374 222c 0a20 2020 2020  ent_test",.     
+00002f60: 2020 2020 2020 206d 6574 6164 6174 612c         metadata,
+00002f70: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
+00002f80: 756d 6e28 2269 6422 2c20 7371 6c61 6c63  umn("id", sqlalc
+00002f90: 6865 6d79 2e49 6e74 6567 6572 2c20 7072  hemy.Integer, pr
+00002fa0: 696d 6172 795f 6b65 793d 5472 7565 2c20  imary_key=True, 
+00002fb0: 636f 6d6d 656e 743d 2269 6420 636f 6d6d  comment="id comm
+00002fc0: 656e 7422 292c 0a20 2020 2020 2020 2020  ent"),.         
+00002fd0: 2020 2043 6f6c 756d 6e28 2264 6174 6122     Column("data"
+00002fe0: 2c20 7371 6c61 6c63 6865 6d79 2e53 7472  , sqlalchemy.Str
+00002ff0: 696e 6728 3230 292c 2063 6f6d 6d65 6e74  ing(20), comment
+00003000: 3d22 6461 7461 2025 2063 6f6d 6d65 6e74  ="data % comment
+00003010: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00003020: 436f 6c75 6d6e 280a 2020 2020 2020 2020  Column(.        
+00003030: 2020 2020 2020 2020 2264 3222 2c0a 2020          "d2",.  
+00003040: 2020 2020 2020 2020 2020 2020 2020 7371                sq
+00003050: 6c61 6c63 6865 6d79 2e53 7472 696e 6728  lalchemy.String(
+00003060: 3230 292c 0a20 2020 2020 2020 2020 2020  20),.           
+00003070: 2020 2020 2063 6f6d 6d65 6e74 3d72 2222       comment=r""
+00003080: 2243 6f6d 6d65 6e74 2074 7970 6573 2074  "Comment types t
+00003090: 7970 6520 7370 6565 6469 6c79 2027 2022  ype speedily ' "
+000030a0: 205c 2027 2720 4675 6e21 2222 222c 0a20   \ '' Fun!""",. 
+000030b0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+000030c0: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
+000030d0: 3d73 6368 656d 612c 0a20 2020 2020 2020  =schema,.       
+000030e0: 2020 2020 2063 6f6d 6d65 6e74 3d72 2222       comment=r""
+000030f0: 2274 6865 2074 6573 7420 2520 2720 2220  "the test % ' " 
+00003100: 5c20 7461 626c 6520 636f 6d6d 656e 7422  \ table comment"
+00003110: 2222 2c0a 2020 2020 2020 2020 290a 0a20  "",.        ).. 
+00003120: 2020 2020 2020 2069 6620 7465 7374 696e         if testin
+00003130: 672e 7265 7175 6972 6573 2e63 726f 7373  g.requires.cross
+00003140: 5f73 6368 656d 615f 666b 5f72 6566 6c65  _schema_fk_refle
+00003150: 6374 696f 6e2e 656e 6162 6c65 643a 0a20  ction.enabled:. 
+00003160: 2020 2020 2020 2020 2020 2069 6620 7363             if sc
+00003170: 6865 6d61 2069 7320 4e6f 6e65 3a0a 2020  hema is None:.  
+00003180: 2020 2020 2020 2020 2020 2020 2020 5461                Ta
+00003190: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
+000031a0: 2020 2020 2020 2020 2022 6c6f 6361 6c5f           "local_
+000031b0: 7461 626c 6522 2c0a 2020 2020 2020 2020  table",.        
+000031c0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+000031d0: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
+000031e0: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
+000031f0: 2822 6964 222c 2073 716c 616c 6368 656d  ("id", sqlalchem
+00003200: 792e 496e 7465 6765 722c 2070 7269 6d61  y.Integer, prima
+00003210: 7279 5f6b 6579 3d54 7275 6529 2c0a 2020  ry_key=True),.  
+00003220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003230: 2020 436f 6c75 6d6e 2822 6461 7461 222c    Column("data",
+00003240: 2073 716c 616c 6368 656d 792e 5374 7269   sqlalchemy.Stri
+00003250: 6e67 2832 3029 292c 0a20 2020 2020 2020  ng(20)),.       
+00003260: 2020 2020 2020 2020 2020 2020 2043 6f6c               Col
+00003270: 756d 6e28 0a20 2020 2020 2020 2020 2020  umn(.           
+00003280: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+00003290: 6d6f 7465 5f69 6422 2c0a 2020 2020 2020  mote_id",.      
+000032a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032b0: 2020 466f 7265 6967 6e4b 6579 2822 2573    ForeignKey("%s
+000032c0: 2e72 656d 6f74 655f 7461 626c 655f 322e  .remote_table_2.
+000032d0: 6964 2220 2520 7465 7374 696e 672e 636f  id" % testing.co
+000032e0: 6e66 6967 2e74 6573 745f 7363 6865 6d61  nfig.test_schema
+000032f0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00003300: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00003310: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00003320: 7374 5f6e 6565 6473 5f66 6b3d 5472 7565  st_needs_fk=True
+00003330: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003340: 2020 2020 2020 7363 6865 6d61 3d63 6f6e        schema=con
+00003350: 6669 672e 6462 2e64 6961 6c65 6374 2e64  fig.db.dialect.d
+00003360: 6566 6175 6c74 5f73 6368 656d 615f 6e61  efault_schema_na
+00003370: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00003380: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00003390: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000033a0: 2020 2020 2020 2020 5461 626c 6528 0a20          Table(. 
+000033b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033c0: 2020 2022 7265 6d6f 7465 5f74 6162 6c65     "remote_table
+000033d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000033e0: 2020 2020 2020 206d 6574 6164 6174 612c         metadata,
+000033f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003400: 2020 2020 2043 6f6c 756d 6e28 2269 6422       Column("id"
+00003410: 2c20 7371 6c61 6c63 6865 6d79 2e49 6e74  , sqlalchemy.Int
+00003420: 6567 6572 2c20 7072 696d 6172 795f 6b65  eger, primary_ke
+00003430: 793d 5472 7565 292c 0a20 2020 2020 2020  y=True),.       
+00003440: 2020 2020 2020 2020 2020 2020 2043 6f6c               Col
+00003450: 756d 6e28 0a20 2020 2020 2020 2020 2020  umn(.           
+00003460: 2020 2020 2020 2020 2020 2020 2022 6c6f               "lo
+00003470: 6361 6c5f 6964 222c 0a20 2020 2020 2020  cal_id",.       
+00003480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003490: 2046 6f72 6569 676e 4b65 7928 0a20 2020   ForeignKey(.   
+000034a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034b0: 2020 2020 2020 2020 2022 2573 2e6c 6f63           "%s.loc
+000034c0: 616c 5f74 6162 6c65 2e69 6422 2025 2063  al_table.id" % c
+000034d0: 6f6e 6669 672e 6462 2e64 6961 6c65 6374  onfig.db.dialect
+000034e0: 2e64 6566 6175 6c74 5f73 6368 656d 615f  .default_schema_
+000034f0: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
+00003500: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
+00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003520: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00003530: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00003540: 6e28 2264 6174 6122 2c20 7371 6c61 6c63  n("data", sqlalc
+00003550: 6865 6d79 2e53 7472 696e 6728 3230 2929  hemy.String(20))
+00003560: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003570: 2020 2020 2020 7363 6865 6d61 3d73 6368        schema=sch
+00003580: 656d 612c 0a20 2020 2020 2020 2020 2020  ema,.           
+00003590: 2020 2020 2020 2020 2074 6573 745f 6e65           test_ne
+000035a0: 6564 735f 666b 3d54 7275 652c 0a20 2020  eds_fk=True,.   
+000035b0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+000035c0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+000035d0: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
+000035e0: 2020 2020 2020 2020 2020 2272 656d 6f74            "remot
+000035f0: 655f 7461 626c 655f 3222 2c0a 2020 2020  e_table_2",.    
+00003600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003610: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+00003620: 2020 2020 2020 2020 2020 2020 2020 436f                Co
+00003630: 6c75 6d6e 2822 6964 222c 2073 716c 616c  lumn("id", sqlal
+00003640: 6368 656d 792e 496e 7465 6765 722c 2070  chemy.Integer, p
+00003650: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
+00003660: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003670: 2020 2020 2020 436f 6c75 6d6e 2822 6461        Column("da
+00003680: 7461 222c 2073 716c 616c 6368 656d 792e  ta", sqlalchemy.
+00003690: 5374 7269 6e67 2832 3029 292c 0a20 2020  String(20)),.   
+000036a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036b0: 2073 6368 656d 613d 7363 6865 6d61 2c0a   schema=schema,.
+000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036d0: 2020 2020 7465 7374 5f6e 6565 6473 5f66      test_needs_f
+000036e0: 6b3d 5472 7565 2c0a 2020 2020 2020 2020  k=True,.        
+000036f0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00003700: 2020 2069 6620 7465 7374 696e 672e 7265     if testing.re
+00003710: 7175 6972 6573 2e69 6e64 6578 5f72 6566  quires.index_ref
+00003720: 6c65 6374 696f 6e2e 656e 6162 6c65 643a  lection.enabled:
+00003730: 0a20 2020 2020 2020 2020 2020 2063 6c73  .            cls
+00003740: 2e64 6566 696e 655f 696e 6465 7828 6d65  .define_index(me
+00003750: 7461 6461 7461 2c20 7573 6572 7329 0a0a  tadata, users)..
+00003760: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00003770: 6f74 2073 6368 656d 613a 0a20 2020 2020  ot schema:.     
+00003780: 2020 2020 2020 2020 2020 2023 2074 6573             # tes
+00003790: 745f 6e65 6564 735f 666b 2069 7320 6174  t_needs_fk is at
+000037a0: 2074 6865 206d 6f6d 656e 7420 746f 2066   the moment to f
+000037b0: 6f72 6365 204d 7953 514c 2049 6e6e 6f44  orce MySQL InnoD
+000037c0: 420a 2020 2020 2020 2020 2020 2020 2020  B.              
+000037d0: 2020 6e6f 6e63 6f6c 5f69 6478 5f74 6573    noncol_idx_tes
+000037e0: 745f 6e6f 706b 203d 2054 6162 6c65 280a  t_nopk = Table(.
+000037f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003800: 2020 2020 226e 6f6e 636f 6c5f 6964 785f      "noncol_idx_
+00003810: 7465 7374 5f6e 6f70 6b22 2c0a 2020 2020  test_nopk",.    
+00003820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003830: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+00003840: 2020 2020 2020 2020 2020 2020 2020 436f                Co
+00003850: 6c75 6d6e 2822 6964 222c 2073 716c 616c  lumn("id", sqlal
+00003860: 6368 656d 792e 496e 7465 6765 722c 2070  chemy.Integer, p
+00003870: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
+00003880: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003890: 2020 2020 2020 436f 6c75 6d6e 2822 7122        Column("q"
+000038a0: 2c20 7371 6c61 6c63 6865 6d79 2e53 7472  , sqlalchemy.Str
+000038b0: 696e 6728 3529 292c 0a20 2020 2020 2020  ing(5)),.       
+000038c0: 2020 2020 2020 2020 2020 2020 2074 6573               tes
+000038d0: 745f 6e65 6564 735f 666b 3d54 7275 652c  t_needs_fk=True,
+000038e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000038f0: 2020 2020 2065 7874 656e 645f 6578 6973       extend_exis
+00003900: 7469 6e67 3d54 7275 652c 0a20 2020 2020  ting=True,.     
+00003910: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00003920: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00003930: 6e63 6f6c 5f69 6478 5f74 6573 745f 706b  ncol_idx_test_pk
+00003940: 203d 2054 6162 6c65 280a 2020 2020 2020   = Table(.      
+00003950: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00003960: 6f6e 636f 6c5f 6964 785f 7465 7374 5f70  oncol_idx_test_p
+00003970: 6b22 2c0a 2020 2020 2020 2020 2020 2020  k",.            
+00003980: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
+00003990: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000039a0: 2020 2020 2020 436f 6c75 6d6e 2822 6964        Column("id
+000039b0: 222c 2073 716c 616c 6368 656d 792e 496e  ", sqlalchemy.In
+000039c0: 7465 6765 722c 2070 7269 6d61 7279 5f6b  teger, primary_k
+000039d0: 6579 3d54 7275 6529 2c0a 2020 2020 2020  ey=True),.      
+000039e0: 2020 2020 2020 2020 2020 2020 2020 436f                Co
+000039f0: 6c75 6d6e 2822 7122 2c20 7371 6c61 6c63  lumn("q", sqlalc
+00003a00: 6865 6d79 2e53 7472 696e 6728 3529 292c  hemy.String(5)),
+00003a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003a20: 2020 2020 2074 6573 745f 6e65 6564 735f       test_needs_
+00003a30: 666b 3d54 7275 652c 0a20 2020 2020 2020  fk=True,.       
+00003a40: 2020 2020 2020 2020 2020 2020 2065 7874               ext
+00003a50: 656e 645f 6578 6973 7469 6e67 3d54 7275  end_existing=Tru
+00003a60: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00003a70: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+00003a80: 2020 2020 2020 6966 2074 6573 7469 6e67        if testing
+00003a90: 2e72 6571 7569 7265 732e 696e 6465 7865  .requires.indexe
+00003aa0: 735f 7769 7468 5f61 7363 6465 7363 2e65  s_with_ascdesc.e
+00003ab0: 6e61 626c 6564 3a0a 2020 2020 2020 2020  nabled:.        
+00003ac0: 2020 2020 2020 2020 2020 2020 7371 6c61              sqla
+00003ad0: 6c63 6865 6d79 2e49 6e64 6578 2822 6e6f  lchemy.Index("no
+00003ae0: 6e63 6f6c 5f69 6478 5f6e 6f70 6b22 2c20  ncol_idx_nopk", 
+00003af0: 6e6f 6e63 6f6c 5f69 6478 5f74 6573 745f  noncol_idx_test_
+00003b00: 6e6f 706b 2e63 2e71 2e64 6573 6328 2929  nopk.c.q.desc())
+00003b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003b20: 2020 2020 2073 716c 616c 6368 656d 792e       sqlalchemy.
+00003b30: 496e 6465 7828 226e 6f6e 636f 6c5f 6964  Index("noncol_id
+00003b40: 785f 706b 222c 206e 6f6e 636f 6c5f 6964  x_pk", noncol_id
+00003b50: 785f 7465 7374 5f70 6b2e 632e 712e 6465  x_test_pk.c.q.de
+00003b60: 7363 2829 290a 0a20 2020 2020 2020 2069  sc())..        i
+00003b70: 6620 7465 7374 696e 672e 7265 7175 6972  f testing.requir
+00003b80: 6573 2e76 6965 775f 636f 6c75 6d6e 5f72  es.view_column_r
+00003b90: 6566 6c65 6374 696f 6e2e 656e 6162 6c65  eflection.enable
+00003ba0: 6420 616e 6420 6e6f 7420 626f 6f6c 280a  d and not bool(.
+00003bb0: 2020 2020 2020 2020 2020 2020 6f73 2e65              os.e
+00003bc0: 6e76 6972 6f6e 2e67 6574 2822 5350 414e  nviron.get("SPAN
+00003bd0: 4e45 525f 454d 554c 4154 4f52 5f48 4f53  NER_EMULATOR_HOS
+00003be0: 5422 290a 2020 2020 2020 2020 293a 0a20  T").        ):. 
+00003bf0: 2020 2020 2020 2020 2020 2063 6c73 2e64             cls.d
+00003c00: 6566 696e 655f 7669 6577 7328 6d65 7461  efine_views(meta
+00003c10: 6461 7461 2c20 7363 6865 6d61 290a 0a20  data, schema).. 
+00003c20: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+00003c30: 736b 6970 6966 280a 2020 2020 2020 2020  skipif(.        
+00003c40: 626f 6f6c 286f 732e 656e 7669 726f 6e2e  bool(os.environ.
+00003c50: 6765 7428 2253 5041 4e4e 4552 5f45 4d55  get("SPANNER_EMU
+00003c60: 4c41 544f 525f 484f 5354 2229 292c 2072  LATOR_HOST")), r
+00003c70: 6561 736f 6e3d 2253 6b69 7070 6564 206f  eason="Skipped o
+00003c80: 6e20 656d 756c 6174 6f72 220a 2020 2020  n emulator".    
+00003c90: 290a 2020 2020 4074 6573 7469 6e67 2e72  ).    @testing.r
+00003ca0: 6571 7569 7265 732e 7669 6577 5f72 6566  equires.view_ref
+00003cb0: 6c65 6374 696f 6e0a 2020 2020 4074 6573  lection.    @tes
+00003cc0: 7469 6e67 2e63 6f6d 6269 6e61 7469 6f6e  ting.combination
+00003cd0: 7328 0a20 2020 2020 2020 2028 4661 6c73  s(.        (Fals
+00003ce0: 652c 292c 2028 5472 7565 2c20 7465 7374  e,), (True, test
+00003cf0: 696e 672e 7265 7175 6972 6573 2e73 6368  ing.requires.sch
+00003d00: 656d 6173 292c 2061 7267 6e61 6d65 733d  emas), argnames=
+00003d10: 2275 7365 5f73 6368 656d 6122 0a20 2020  "use_schema".   
+00003d20: 2029 0a20 2020 2064 6566 2074 6573 745f   ).    def test_
+00003d30: 6765 745f 7669 6577 5f64 6566 696e 6974  get_view_definit
+00003d40: 696f 6e28 7365 6c66 2c20 636f 6e6e 6563  ion(self, connec
+00003d50: 7469 6f6e 2c20 7573 655f 7363 6865 6d61  tion, use_schema
+00003d60: 293a 0a20 2020 2020 2020 2069 6620 7573  ):.        if us
+00003d70: 655f 7363 6865 6d61 3a0a 2020 2020 2020  e_schema:.      
+00003d80: 2020 2020 2020 7363 6865 6d61 203d 2063        schema = c
+00003d90: 6f6e 6669 672e 7465 7374 5f73 6368 656d  onfig.test_schem
+00003da0: 610a 2020 2020 2020 2020 656c 7365 3a0a  a.        else:.
+00003db0: 2020 2020 2020 2020 2020 2020 7363 6865              sche
+00003dc0: 6d61 203d 204e 6f6e 650a 2020 2020 2020  ma = None.      
+00003dd0: 2020 7669 6577 5f6e 616d 6531 203d 2022    view_name1 = "
+00003de0: 7573 6572 735f 7622 0a20 2020 2020 2020  users_v".       
+00003df0: 2076 6965 775f 6e61 6d65 3220 3d20 2265   view_name2 = "e
+00003e00: 6d61 696c 5f61 6464 7265 7373 6573 5f76  mail_addresses_v
+00003e10: 220a 2020 2020 2020 2020 696e 7370 203d  ".        insp =
+00003e20: 2069 6e73 7065 6374 2863 6f6e 6e65 6374   inspect(connect
+00003e30: 696f 6e29 0a20 2020 2020 2020 2076 3120  ion).        v1 
+00003e40: 3d20 696e 7370 2e67 6574 5f76 6965 775f  = insp.get_view_
+00003e50: 6465 6669 6e69 7469 6f6e 2876 6965 775f  definition(view_
+00003e60: 6e61 6d65 312c 2073 6368 656d 613d 7363  name1, schema=sc
+00003e70: 6865 6d61 290a 2020 2020 2020 2020 7365  hema).        se
+00003e80: 6c66 2e61 7373 6572 745f 2876 3129 0a20  lf.assert_(v1). 
+00003e90: 2020 2020 2020 2076 3220 3d20 696e 7370         v2 = insp
+00003ea0: 2e67 6574 5f76 6965 775f 6465 6669 6e69  .get_view_defini
+00003eb0: 7469 6f6e 2876 6965 775f 6e61 6d65 322c  tion(view_name2,
+00003ec0: 2073 6368 656d 613d 7363 6865 6d61 290a   schema=schema).
+00003ed0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00003ee0: 6572 745f 2876 3229 0a0a 2020 2020 4074  ert_(v2)..    @t
+00003ef0: 6573 7469 6e67 2e63 6f6d 6269 6e61 7469  esting.combinati
+00003f00: 6f6e 7328 0a20 2020 2020 2020 2028 4661  ons(.        (Fa
+00003f10: 6c73 652c 2046 616c 7365 292c 0a20 2020  lse, False),.   
+00003f20: 2020 2020 2028 4661 6c73 652c 2054 7275       (False, Tru
+00003f30: 652c 2074 6573 7469 6e67 2e72 6571 7569  e, testing.requi
+00003f40: 7265 732e 7363 6865 6d61 7329 2c0a 2020  res.schemas),.  
+00003f50: 2020 2020 2020 2854 7275 652c 2046 616c        (True, Fal
+00003f60: 7365 2c20 7465 7374 696e 672e 7265 7175  se, testing.requ
+00003f70: 6972 6573 2e76 6965 775f 7265 666c 6563  ires.view_reflec
+00003f80: 7469 6f6e 292c 0a20 2020 2020 2020 2028  tion),.        (
+00003f90: 0a20 2020 2020 2020 2020 2020 2054 7275  .            Tru
+00003fa0: 652c 0a20 2020 2020 2020 2020 2020 2054  e,.            T
+00003fb0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00003fc0: 2074 6573 7469 6e67 2e72 6571 7569 7265   testing.require
+00003fd0: 732e 7363 6865 6d61 7320 2b20 7465 7374  s.schemas + test
+00003fe0: 696e 672e 7265 7175 6972 6573 2e76 6965  ing.requires.vie
+00003ff0: 775f 7265 666c 6563 7469 6f6e 2c0a 2020  w_reflection,.  
+00004000: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00004010: 2061 7267 6e61 6d65 733d 2275 7365 5f76   argnames="use_v
+00004020: 6965 7773 2c75 7365 5f73 6368 656d 6122  iews,use_schema"
+00004030: 2c0a 2020 2020 290a 2020 2020 6465 6620  ,.    ).    def 
+00004040: 7465 7374 5f67 6574 5f63 6f6c 756d 6e73  test_get_columns
+00004050: 2873 656c 662c 2063 6f6e 6e65 6374 696f  (self, connectio
+00004060: 6e2c 2075 7365 5f76 6965 7773 2c20 7573  n, use_views, us
+00004070: 655f 7363 6865 6d61 293a 0a20 2020 2020  e_schema):.     
+00004080: 2020 2069 6620 7573 655f 7669 6577 7320     if use_views 
+00004090: 616e 6420 626f 6f6c 286f 732e 656e 7669  and bool(os.envi
+000040a0: 726f 6e2e 6765 7428 2253 5041 4e4e 4552  ron.get("SPANNER
+000040b0: 5f45 4d55 4c41 544f 525f 484f 5354 2229  _EMULATOR_HOST")
+000040c0: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
+000040d0: 7974 6573 742e 736b 6970 2822 536b 6970  ytest.skip("Skip
+000040e0: 7065 6420 6f6e 2065 6d75 6c61 746f 7222  ped on emulator"
+000040f0: 290a 0a20 2020 2020 2020 2073 6368 656d  )..        schem
+00004100: 6120 3d20 4e6f 6e65 0a20 2020 2020 2020  a = None.       
+00004110: 2075 7365 7273 2c20 6164 6472 6573 7365   users, addresse
+00004120: 7320 3d20 2873 656c 662e 7461 626c 6573  s = (self.tables
+00004130: 2e75 7365 7273 2c20 7365 6c66 2e74 6162  .users, self.tab
+00004140: 6c65 732e 656d 6169 6c5f 6164 6472 6573  les.email_addres
+00004150: 7365 7329 0a20 2020 2020 2020 2069 6620  ses).        if 
+00004160: 7573 655f 7669 6577 733a 0a20 2020 2020  use_views:.     
+00004170: 2020 2020 2020 2074 6162 6c65 5f6e 616d         table_nam
+00004180: 6573 203d 205b 2275 7365 7273 5f76 222c  es = ["users_v",
+00004190: 2022 656d 6169 6c5f 6164 6472 6573 7365   "email_addresse
+000041a0: 735f 7622 5d0a 2020 2020 2020 2020 656c  s_v"].        el
+000041b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000041c0: 7461 626c 655f 6e61 6d65 7320 3d20 5b22  table_names = ["
+000041d0: 7573 6572 7322 2c20 2265 6d61 696c 5f61  users", "email_a
+000041e0: 6464 7265 7373 6573 225d 0a0a 2020 2020  ddresses"]..    
+000041f0: 2020 2020 696e 7370 203d 2069 6e73 7065      insp = inspe
+00004200: 6374 2863 6f6e 6e65 6374 696f 6e29 0a20  ct(connection). 
+00004210: 2020 2020 2020 2066 6f72 2074 6162 6c65         for table
+00004220: 5f6e 616d 652c 2074 6162 6c65 2069 6e20  _name, table in 
+00004230: 7a69 7028 7461 626c 655f 6e61 6d65 732c  zip(table_names,
+00004240: 2028 7573 6572 732c 2061 6464 7265 7373   (users, address
+00004250: 6573 2929 3a0a 2020 2020 2020 2020 2020  es)):.          
+00004260: 2020 7363 6865 6d61 5f6e 616d 6520 3d20    schema_name = 
+00004270: 7363 6865 6d61 0a20 2020 2020 2020 2020  schema.         
+00004280: 2020 2063 6f6c 7320 3d20 696e 7370 2e67     cols = insp.g
+00004290: 6574 5f63 6f6c 756d 6e73 2874 6162 6c65  et_columns(table
+000042a0: 5f6e 616d 652c 2073 6368 656d 613d 7363  _name, schema=sc
+000042b0: 6865 6d61 5f6e 616d 6529 0a20 2020 2020  hema_name).     
+000042c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000042d0: 7274 5f28 6c65 6e28 636f 6c73 2920 3e20  rt_(len(cols) > 
+000042e0: 302c 206c 656e 2863 6f6c 7329 290a 0a20  0, len(cols)).. 
+000042f0: 2020 2020 2020 2020 2020 2023 2073 686f             # sho
+00004300: 756c 6420 6265 2069 6e20 6f72 6465 720a  uld be in order.
+00004310: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00004320: 2069 2c20 636f 6c20 696e 2065 6e75 6d65   i, col in enume
+00004330: 7261 7465 2874 6162 6c65 2e63 6f6c 756d  rate(table.colum
+00004340: 6e73 293a 0a20 2020 2020 2020 2020 2020  ns):.           
+00004350: 2020 2020 2065 715f 2863 6f6c 2e6e 616d       eq_(col.nam
+00004360: 652c 2063 6f6c 735b 695d 5b22 6e61 6d65  e, cols[i]["name
+00004370: 225d 290a 2020 2020 2020 2020 2020 2020  "]).            
+00004380: 2020 2020 6374 7970 6520 3d20 636f 6c73      ctype = cols
+00004390: 5b69 5d5b 2274 7970 6522 5d2e 5f5f 636c  [i]["type"].__cl
+000043a0: 6173 735f 5f0a 2020 2020 2020 2020 2020  ass__.          
+000043b0: 2020 2020 2020 6374 7970 655f 6465 6620        ctype_def 
+000043c0: 3d20 636f 6c2e 7479 7065 0a20 2020 2020  = col.type.     
+000043d0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+000043e0: 696e 7374 616e 6365 2863 7479 7065 5f64  instance(ctype_d
+000043f0: 6566 2c20 7371 6c61 6c63 6865 6d79 2e74  ef, sqlalchemy.t
+00004400: 7970 6573 2e54 7970 6545 6e67 696e 6529  ypes.TypeEngine)
+00004410: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004420: 2020 2020 2020 6374 7970 655f 6465 6620        ctype_def 
+00004430: 3d20 6374 7970 655f 6465 662e 5f5f 636c  = ctype_def.__cl
+00004440: 6173 735f 5f0a 0a20 2020 2020 2020 2020  ass__..         
+00004450: 2020 2020 2020 2023 204f 7261 636c 6520         # Oracle 
+00004460: 7265 7475 726e 7320 4461 7465 2066 6f72  returns Date for
+00004470: 2044 6174 6554 696d 652e 0a0a 2020 2020   DateTime...    
+00004480: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00004490: 6573 7469 6e67 2e61 6761 696e 7374 2822  esting.against("
+000044a0: 6f72 6163 6c65 2229 2061 6e64 2063 7479  oracle") and cty
+000044b0: 7065 5f64 6566 2069 6e20 280a 2020 2020  pe_def in (.    
+000044c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044d0: 7371 6c5f 7479 7065 732e 4461 7465 2c0a  sql_types.Date,.
+000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044f0: 2020 2020 7371 6c5f 7479 7065 732e 4461      sql_types.Da
+00004500: 7465 5469 6d65 2c0a 2020 2020 2020 2020  teTime,.        
+00004510: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+00004520: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00004530: 7479 7065 5f64 6566 203d 2073 716c 5f74  type_def = sql_t
+00004540: 7970 6573 2e44 6174 650a 0a20 2020 2020  ypes.Date..     
+00004550: 2020 2020 2020 2020 2020 2023 2061 7373             # ass
+00004560: 6572 7420 7468 6174 2074 6865 2064 6573  ert that the des
+00004570: 6972 6564 2074 7970 6520 616e 6420 7265  ired type and re
+00004580: 7475 726e 2074 7970 6520 7368 6172 650a  turn type share.
+00004590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045a0: 2320 6120 6261 7365 2077 6974 6869 6e20  # a base within 
+000045b0: 6f6e 6520 6f66 2074 6865 2067 656e 6572  one of the gener
+000045c0: 6963 2074 7970 6573 2e0a 0a20 2020 2020  ic types...     
+000045d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000045e0: 6173 7365 7274 5f28 0a20 2020 2020 2020  assert_(.       
+000045f0: 2020 2020 2020 2020 2020 2020 206c 656e               len
+00004600: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00004610: 2020 2020 2020 2020 2020 7365 7428 6374            set(ct
+00004620: 7970 652e 5f5f 6d72 6f5f 5f29 0a20 2020  ype.__mro__).   
+00004630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004640: 2020 2020 202e 696e 7465 7273 6563 7469       .intersecti
+00004650: 6f6e 2863 7479 7065 5f64 6566 2e5f 5f6d  on(ctype_def.__m
+00004660: 726f 5f5f 290a 2020 2020 2020 2020 2020  ro__).          
+00004670: 2020 2020 2020 2020 2020 2020 2020 2e69                .i
+00004680: 6e74 6572 7365 6374 696f 6e28 0a20 2020  ntersection(.   
+00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
+000046b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046c0: 2020 2020 2020 2020 2020 2073 716c 5f74             sql_t
+000046d0: 7970 6573 2e49 6e74 6567 6572 2c0a 2020  ypes.Integer,.  
+000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046f0: 2020 2020 2020 2020 2020 2020 2020 7371                sq
+00004700: 6c5f 7479 7065 732e 4e75 6d65 7269 632c  l_types.Numeric,
+00004710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004730: 2073 716c 5f74 7970 6573 2e44 6174 6554   sql_types.DateT
+00004740: 696d 652c 0a20 2020 2020 2020 2020 2020  ime,.           
+00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004760: 2020 2020 2073 716c 5f74 7970 6573 2e44       sql_types.D
+00004770: 6174 652c 0a20 2020 2020 2020 2020 2020  ate,.           
+00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004790: 2020 2020 2073 716c 5f74 7970 6573 2e54       sql_types.T
+000047a0: 696d 652c 0a20 2020 2020 2020 2020 2020  ime,.           
+000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047c0: 2020 2020 2073 716c 5f74 7970 6573 2e53       sql_types.S
+000047d0: 7472 696e 672c 0a20 2020 2020 2020 2020  tring,.         
+000047e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047f0: 2020 2020 2020 2073 716c 5f74 7970 6573         sql_types
+00004800: 2e5f 4269 6e61 7279 2c0a 2020 2020 2020  ._Binary,.      
+00004810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004820: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00004830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004840: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00004850: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00004860: 2020 2020 2020 2020 2020 2020 3e20 302c              > 0,
+00004870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004880: 2020 2020 2022 2573 2825 7329 2c20 2573       "%s(%s), %s
+00004890: 2825 7329 2220 2520 2863 6f6c 2e6e 616d  (%s)" % (col.nam
+000048a0: 652c 2063 6f6c 2e74 7970 652c 2063 6f6c  e, col.type, col
+000048b0: 735b 695d 5b22 6e61 6d65 225d 2c20 6374  s[i]["name"], ct
+000048c0: 7970 6529 2c0a 2020 2020 2020 2020 2020  ype),.          
+000048d0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+000048e0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000048f0: 636f 6c2e 7072 696d 6172 795f 6b65 793a  col.primary_key:
+00004900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004910: 2020 2020 2061 7373 6572 7420 636f 6c73       assert cols
+00004920: 5b69 5d5b 2264 6566 6175 6c74 225d 2069  [i]["default"] i
+00004930: 7320 4e6f 6e65 0a0a 2020 2020 4074 6573  s None..    @tes
+00004940: 7469 6e67 2e63 6f6d 6269 6e61 7469 6f6e  ting.combination
+00004950: 7328 2846 616c 7365 2c29 2c20 6172 676e  s((False,), argn
+00004960: 616d 6573 3d22 7573 655f 7363 6865 6d61  ames="use_schema
+00004970: 2229 0a20 2020 2040 7465 7374 696e 672e  ").    @testing.
+00004980: 7265 7175 6972 6573 2e66 6f72 6569 676e  requires.foreign
+00004990: 5f6b 6579 5f63 6f6e 7374 7261 696e 745f  _key_constraint_
+000049a0: 7265 666c 6563 7469 6f6e 0a20 2020 2064  reflection.    d
+000049b0: 6566 2074 6573 745f 6765 745f 666f 7265  ef test_get_fore
+000049c0: 6967 6e5f 6b65 7973 2873 656c 662c 2063  ign_keys(self, c
+000049d0: 6f6e 6e65 6374 696f 6e2c 2075 7365 5f73  onnection, use_s
+000049e0: 6368 656d 6129 3a0a 2020 2020 2020 2020  chema):.        
+000049f0: 6966 2075 7365 5f73 6368 656d 613a 0a20  if use_schema:. 
+00004a00: 2020 2020 2020 2020 2020 2073 6368 656d             schem
+00004a10: 6120 3d20 636f 6e66 6967 2e74 6573 745f  a = config.test_
+00004a20: 7363 6865 6d61 0a20 2020 2020 2020 2065  schema.        e
+00004a30: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00004a40: 2073 6368 656d 6120 3d20 4e6f 6e65 0a0a   schema = None..
+00004a50: 2020 2020 2020 2020 7573 6572 732c 2061          users, a
+00004a60: 6464 7265 7373 6573 203d 2028 7365 6c66  ddresses = (self
+00004a70: 2e74 6162 6c65 732e 7573 6572 732c 2073  .tables.users, s
+00004a80: 656c 662e 7461 626c 6573 2e65 6d61 696c  elf.tables.email
+00004a90: 5f61 6464 7265 7373 6573 290a 2020 2020  _addresses).    
+00004aa0: 2020 2020 696e 7370 203d 2069 6e73 7065      insp = inspe
+00004ab0: 6374 2863 6f6e 6e65 6374 696f 6e29 0a20  ct(connection). 
+00004ac0: 2020 2020 2020 2065 7870 6563 7465 645f         expected_
+00004ad0: 7363 6865 6d61 203d 2073 6368 656d 610a  schema = schema.
+00004ae0: 2020 2020 2020 2020 2320 7573 6572 730a          # users.
+00004af0: 0a20 2020 2020 2020 2069 6620 7465 7374  .        if test
+00004b00: 696e 672e 7265 7175 6972 6573 2e73 656c  ing.requires.sel
+00004b10: 665f 7265 6665 7265 6e74 6961 6c5f 666f  f_referential_fo
+00004b20: 7265 6967 6e5f 6b65 7973 2e65 6e61 626c  reign_keys.enabl
+00004b30: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+00004b40: 7573 6572 735f 666b 6579 7320 3d20 696e  users_fkeys = in
+00004b50: 7370 2e67 6574 5f66 6f72 6569 676e 5f6b  sp.get_foreign_k
+00004b60: 6579 7328 7573 6572 732e 6e61 6d65 2c20  eys(users.name, 
+00004b70: 7363 6865 6d61 3d73 6368 656d 6129 0a20  schema=schema). 
+00004b80: 2020 2020 2020 2020 2020 2066 6b65 7931             fkey1
+00004b90: 203d 2075 7365 7273 5f66 6b65 7973 5b30   = users_fkeys[0
+00004ba0: 5d0a 0a20 2020 2020 2020 2020 2020 2077  ]..            w
+00004bb0: 6974 6820 7465 7374 696e 672e 7265 7175  ith testing.requ
+00004bc0: 6972 6573 2e6e 616d 6564 5f63 6f6e 7374  ires.named_const
+00004bd0: 7261 696e 7473 2e66 6169 6c5f 6966 2829  raints.fail_if()
+00004be0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004bf0: 2020 6571 5f28 666b 6579 315b 226e 616d    eq_(fkey1["nam
+00004c00: 6522 5d2c 2022 7573 6572 5f69 645f 666b  e"], "user_id_fk
+00004c10: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
+00004c20: 6571 5f28 666b 6579 315b 2272 6566 6572  eq_(fkey1["refer
+00004c30: 7265 645f 7363 6865 6d61 225d 2c20 6578  red_schema"], ex
+00004c40: 7065 6374 6564 5f73 6368 656d 6129 0a20  pected_schema). 
+00004c50: 2020 2020 2020 2020 2020 2065 715f 2866             eq_(f
+00004c60: 6b65 7931 5b22 7265 6665 7272 6564 5f74  key1["referred_t
+00004c70: 6162 6c65 225d 2c20 7573 6572 732e 6e61  able"], users.na
+00004c80: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+00004c90: 6571 5f28 666b 6579 315b 2272 6566 6572  eq_(fkey1["refer
+00004ca0: 7265 645f 636f 6c75 6d6e 7322 5d2c 205b  red_columns"], [
+00004cb0: 2275 7365 725f 6964 225d 290a 2020 2020  "user_id"]).    
+00004cc0: 2020 2020 2020 2020 6966 2074 6573 7469          if testi
+00004cd0: 6e67 2e72 6571 7569 7265 732e 7365 6c66  ng.requires.self
+00004ce0: 5f72 6566 6572 656e 7469 616c 5f66 6f72  _referential_for
+00004cf0: 6569 676e 5f6b 6579 732e 656e 6162 6c65  eign_keys.enable
+00004d00: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
+00004d10: 2020 2065 715f 2866 6b65 7931 5b22 636f     eq_(fkey1["co
+00004d20: 6e73 7472 6169 6e65 645f 636f 6c75 6d6e  nstrained_column
+00004d30: 7322 5d2c 205b 2270 6172 656e 745f 7573  s"], ["parent_us
+00004d40: 6572 5f69 6422 5d29 0a0a 2020 2020 2020  er_id"])..      
+00004d50: 2020 2320 6164 6472 6573 7365 730a 2020    # addresses.  
+00004d60: 2020 2020 2020 6164 6472 5f66 6b65 7973        addr_fkeys
+00004d70: 203d 2069 6e73 702e 6765 745f 666f 7265   = insp.get_fore
+00004d80: 6967 6e5f 6b65 7973 2861 6464 7265 7373  ign_keys(address
+00004d90: 6573 2e6e 616d 652c 2073 6368 656d 613d  es.name, schema=
+00004da0: 7363 6865 6d61 290a 2020 2020 2020 2020  schema).        
+00004db0: 666b 6579 3120 3d20 6164 6472 5f66 6b65  fkey1 = addr_fke
+00004dc0: 7973 5b30 5d0a 0a20 2020 2020 2020 2077  ys[0]..        w
+00004dd0: 6974 6820 7465 7374 696e 672e 7265 7175  ith testing.requ
+00004de0: 6972 6573 2e69 6d70 6c69 6369 746c 795f  ires.implicitly_
+00004df0: 6e61 6d65 645f 636f 6e73 7472 6169 6e74  named_constraint
+00004e00: 732e 6661 696c 5f69 6628 293a 0a20 2020  s.fail_if():.   
+00004e10: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00004e20: 7365 7274 5f28 666b 6579 315b 226e 616d  sert_(fkey1["nam
+00004e30: 6522 5d20 6973 206e 6f74 204e 6f6e 6529  e"] is not None)
+00004e40: 0a0a 2020 2020 2020 2020 6571 5f28 666b  ..        eq_(fk
+00004e50: 6579 315b 2272 6566 6572 7265 645f 7363  ey1["referred_sc
+00004e60: 6865 6d61 225d 2c20 6578 7065 6374 6564  hema"], expected
+00004e70: 5f73 6368 656d 6129 0a20 2020 2020 2020  _schema).       
+00004e80: 2065 715f 2866 6b65 7931 5b22 7265 6665   eq_(fkey1["refe
+00004e90: 7272 6564 5f74 6162 6c65 225d 2c20 7573  rred_table"], us
+00004ea0: 6572 732e 6e61 6d65 290a 2020 2020 2020  ers.name).      
+00004eb0: 2020 6571 5f28 666b 6579 315b 2272 6566    eq_(fkey1["ref
+00004ec0: 6572 7265 645f 636f 6c75 6d6e 7322 5d2c  erred_columns"],
+00004ed0: 205b 2275 7365 725f 6964 225d 290a 2020   ["user_id"]).  
+00004ee0: 2020 2020 2020 6571 5f28 666b 6579 315b        eq_(fkey1[
+00004ef0: 2263 6f6e 7374 7261 696e 6564 5f63 6f6c  "constrained_col
+00004f00: 756d 6e73 225d 2c20 5b22 7265 6d6f 7465  umns"], ["remote
+00004f10: 5f75 7365 725f 6964 225d 290a 0a20 2020  _user_id"])..   
+00004f20: 2040 7465 7374 696e 672e 7265 7175 6972   @testing.requir
+00004f30: 6573 2e66 6f72 6569 676e 5f6b 6579 5f63  es.foreign_key_c
+00004f40: 6f6e 7374 7261 696e 745f 7265 666c 6563  onstraint_reflec
+00004f50: 7469 6f6e 0a20 2020 2040 7465 7374 696e  tion.    @testin
+00004f60: 672e 636f 6d62 696e 6174 696f 6e73 280a  g.combinations(.
+00004f70: 2020 2020 2020 2020 284e 6f6e 652c 2054          (None, T
+00004f80: 7275 652c 2046 616c 7365 2c20 4661 6c73  rue, False, Fals
+00004f90: 6529 2c0a 2020 2020 2020 2020 284e 6f6e  e),.        (Non
+00004fa0: 652c 2054 7275 652c 2046 616c 7365 2c20  e, True, False, 
+00004fb0: 5472 7565 2c20 7465 7374 696e 672e 7265  True, testing.re
+00004fc0: 7175 6972 6573 2e73 6368 656d 6173 292c  quires.schemas),
+00004fd0: 0a20 2020 2020 2020 2028 2266 6f72 6569  .        ("forei
+00004fe0: 676e 5f6b 6579 222c 2054 7275 652c 2046  gn_key", True, F
+00004ff0: 616c 7365 2c20 4661 6c73 6529 2c0a 2020  alse, False),.  
+00005000: 2020 2020 2020 284e 6f6e 652c 2046 616c        (None, Fal
+00005010: 7365 2c20 4661 6c73 652c 2046 616c 7365  se, False, False
+00005020: 292c 0a20 2020 2020 2020 2028 4e6f 6e65  ),.        (None
+00005030: 2c20 4661 6c73 652c 2046 616c 7365 2c20  , False, False, 
+00005040: 5472 7565 2c20 7465 7374 696e 672e 7265  True, testing.re
+00005050: 7175 6972 6573 2e73 6368 656d 6173 292c  quires.schemas),
+00005060: 0a20 2020 2020 2020 2028 4e6f 6e65 2c20  .        (None, 
+00005070: 5472 7565 2c20 4661 6c73 652c 2046 616c  True, False, Fal
+00005080: 7365 292c 0a20 2020 2020 2020 2028 4e6f  se),.        (No
+00005090: 6e65 2c20 5472 7565 2c20 4661 6c73 652c  ne, True, False,
+000050a0: 2054 7275 652c 2074 6573 7469 6e67 2e72   True, testing.r
+000050b0: 6571 7569 7265 732e 7363 6865 6d61 7329  equires.schemas)
+000050c0: 2c0a 2020 2020 2020 2020 6172 676e 616d  ,.        argnam
+000050d0: 6573 3d22 6f72 6465 725f 6279 2c69 6e63  es="order_by,inc
+000050e0: 6c75 6465 5f70 6c61 696e 2c69 6e63 6c75  lude_plain,inclu
+000050f0: 6465 5f76 6965 7773 2c75 7365 5f73 6368  de_views,use_sch
+00005100: 656d 6122 2c0a 2020 2020 290a 2020 2020  ema",.    ).    
+00005110: 6465 6620 7465 7374 5f67 6574 5f74 6162  def test_get_tab
+00005120: 6c65 5f6e 616d 6573 280a 2020 2020 2020  le_names(.      
+00005130: 2020 7365 6c66 2c20 636f 6e6e 6563 7469    self, connecti
+00005140: 6f6e 2c20 6f72 6465 725f 6279 2c20 696e  on, order_by, in
+00005150: 636c 7564 655f 706c 6169 6e2c 2069 6e63  clude_plain, inc
+00005160: 6c75 6465 5f76 6965 7773 2c20 7573 655f  lude_views, use_
+00005170: 7363 6865 6d61 0a20 2020 2029 3a0a 0a20  schema.    ):.. 
+00005180: 2020 2020 2020 2069 6620 7573 655f 7363         if use_sc
+00005190: 6865 6d61 3a0a 2020 2020 2020 2020 2020  hema:.          
+000051a0: 2020 7363 6865 6d61 203d 2063 6f6e 6669    schema = confi
+000051b0: 672e 7465 7374 5f73 6368 656d 610a 2020  g.test_schema.  
+000051c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000051d0: 2020 2020 2020 2020 7363 6865 6d61 203d          schema =
+000051e0: 204e 6f6e 650a 0a20 2020 2020 2020 205f   None..        _
+000051f0: 6967 6e6f 7265 5f74 6162 6c65 7320 3d20  ignore_tables = 
+00005200: 5b0a 2020 2020 2020 2020 2020 2020 2261  [.            "a
+00005210: 6363 6f75 6e74 222c 0a20 2020 2020 2020  ccount",.       
+00005220: 2020 2020 2022 616c 656d 6269 635f 7665       "alembic_ve
+00005230: 7273 696f 6e22 2c0a 2020 2020 2020 2020  rsion",.        
+00005240: 2020 2020 2262 7974 6573 5f74 6162 6c65      "bytes_table
+00005250: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00005260: 636f 6d6d 656e 745f 7465 7374 222c 0a20  comment_test",. 
+00005270: 2020 2020 2020 2020 2020 2022 6461 7465             "date
+00005280: 5f74 6162 6c65 222c 0a20 2020 2020 2020  _table",.       
+00005290: 2020 2020 2022 6e6f 6e63 6f6c 5f69 6478       "noncol_idx
+000052a0: 5f74 6573 745f 706b 222c 0a20 2020 2020  _test_pk",.     
+000052b0: 2020 2020 2020 2022 6e6f 6e63 6f6c 5f69         "noncol_i
+000052c0: 6478 5f74 6573 745f 6e6f 706b 222c 0a20  dx_test_nopk",. 
+000052d0: 2020 2020 2020 2020 2020 2022 6c6f 6361             "loca
+000052e0: 6c5f 7461 626c 6522 2c0a 2020 2020 2020  l_table",.      
+000052f0: 2020 2020 2020 2272 656d 6f74 655f 7461        "remote_ta
+00005300: 626c 6522 2c0a 2020 2020 2020 2020 2020  ble",.          
+00005310: 2020 2272 656d 6f74 655f 7461 626c 655f    "remote_table_
+00005320: 3222 2c0a 2020 2020 2020 2020 2020 2020  2",.            
+00005330: 2274 6578 745f 7461 626c 6522 2c0a 2020  "text_table",.  
+00005340: 2020 2020 2020 2020 2020 2275 7365 725f            "user_
+00005350: 746d 7022 2c0a 2020 2020 2020 2020 5d0a  tmp",.        ].
+00005360: 0a20 2020 2020 2020 2069 6e73 7020 3d20  .        insp = 
+00005370: 696e 7370 6563 7428 636f 6e6e 6563 7469  inspect(connecti
+00005380: 6f6e 290a 0a20 2020 2020 2020 2069 6620  on)..        if 
+00005390: 696e 636c 7564 655f 7669 6577 733a 0a20  include_views:. 
+000053a0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+000053b0: 5f6e 616d 6573 203d 2069 6e73 702e 6765  _names = insp.ge
+000053c0: 745f 7669 6577 5f6e 616d 6573 2873 6368  t_view_names(sch
+000053d0: 656d 6129 0a20 2020 2020 2020 2020 2020  ema).           
+000053e0: 2074 6162 6c65 5f6e 616d 6573 2e73 6f72   table_names.sor
+000053f0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00005400: 616e 7377 6572 203d 205b 2265 6d61 696c  answer = ["email
+00005410: 5f61 6464 7265 7373 6573 5f76 222c 2022  _addresses_v", "
+00005420: 7573 6572 735f 7622 5d0a 2020 2020 2020  users_v"].      
+00005430: 2020 2020 2020 6571 5f28 736f 7274 6564        eq_(sorted
+00005440: 2874 6162 6c65 5f6e 616d 6573 292c 2061  (table_names), a
+00005450: 6e73 7765 7229 0a0a 2020 2020 2020 2020  nswer)..        
+00005460: 6966 2069 6e63 6c75 6465 5f70 6c61 696e  if include_plain
+00005470: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00005480: 206f 7264 6572 5f62 793a 0a20 2020 2020   order_by:.     
+00005490: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+000054a0: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
+000054b0: 2020 2020 2020 2020 2020 7265 635b 305d            rec[0]
+000054c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000054d0: 2020 2020 2066 6f72 2072 6563 2069 6e20       for rec in 
+000054e0: 696e 7370 2e67 6574 5f73 6f72 7465 645f  insp.get_sorted_
+000054f0: 7461 626c 655f 616e 645f 666b 635f 6e61  table_and_fkc_na
+00005500: 6d65 7328 7363 6865 6d61 290a 2020 2020  mes(schema).    
+00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005520: 6966 2072 6563 5b30 5d0a 2020 2020 2020  if rec[0].      
+00005530: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00005540: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00005550: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+00005560: 626c 6573 203d 2069 6e73 702e 6765 745f  bles = insp.get_
+00005570: 7461 626c 655f 6e61 6d65 7328 7363 6865  table_names(sche
+00005580: 6d61 290a 2020 2020 2020 2020 2020 2020  ma).            
+00005590: 7461 626c 655f 6e61 6d65 7320 3d20 5b74  table_names = [t
+000055a0: 2066 6f72 2074 2069 6e20 7461 626c 6573   for t in tables
+000055b0: 2069 6620 7420 6e6f 7420 696e 205f 6967   if t not in _ig
+000055c0: 6e6f 7265 5f74 6162 6c65 735d 0a0a 2020  nore_tables]..  
+000055d0: 2020 2020 2020 2020 2020 6966 206f 7264            if ord
+000055e0: 6572 5f62 7920 3d3d 2022 666f 7265 6967  er_by == "foreig
+000055f0: 6e5f 6b65 7922 3a0a 2020 2020 2020 2020  n_key":.        
+00005600: 2020 2020 2020 2020 616e 7377 6572 203d          answer =
+00005610: 205b 2275 7365 7273 222c 2022 656d 6169   ["users", "emai
+00005620: 6c5f 6164 6472 6573 7365 7322 2c20 2264  l_addresses", "d
+00005630: 696e 6761 6c69 6e67 7322 5d0a 2020 2020  ingalings"].    
+00005640: 2020 2020 2020 2020 2020 2020 6571 5f28              eq_(
+00005650: 7461 626c 655f 6e61 6d65 732c 2061 6e73  table_names, ans
+00005660: 7765 7229 0a20 2020 2020 2020 2020 2020  wer).           
+00005670: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00005680: 2020 2020 2020 2061 6e73 7765 7220 3d20         answer = 
+00005690: 5b22 6469 6e67 616c 696e 6773 222c 2022  ["dingalings", "
+000056a0: 656d 6169 6c5f 6164 6472 6573 7365 7322  email_addresses"
+000056b0: 2c20 2275 7365 7273 225d 0a20 2020 2020  , "users"].     
+000056c0: 2020 2020 2020 2020 2020 2065 715f 2873             eq_(s
+000056d0: 6f72 7465 6428 7461 626c 655f 6e61 6d65  orted(table_name
+000056e0: 7329 2c20 616e 7377 6572 290a 0a20 2020  s), answer)..   
+000056f0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00005700: 2020 6465 6620 6465 6669 6e65 5f74 656d    def define_tem
+00005710: 705f 7461 626c 6573 2863 6c73 2c20 6d65  p_tables(cls, me
+00005720: 7461 6461 7461 293a 0a20 2020 2020 2020  tadata):.       
+00005730: 2022 2222 0a20 2020 2020 2020 2053 5041   """.        SPA
+00005740: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
+00005750: 2020 2020 2020 2020 496e 2043 6c6f 7564          In Cloud
+00005760: 2053 7061 6e6e 6572 2075 6e69 7175 6520   Spanner unique 
+00005770: 696e 6465 7865 7320 6172 6520 7573 6564  indexes are used
+00005780: 2069 6e73 7465 6164 206f 6620 6469 7265   instead of dire
+00005790: 6374 6c79 0a20 2020 2020 2020 2063 7265  ctly.        cre
+000057a0: 6174 696e 6720 756e 6971 7565 2063 6f6e  ating unique con
+000057b0: 7374 7261 696e 7473 2e20 4f76 6572 7269  straints. Overri
+000057c0: 6469 6e67 2074 6865 2074 6573 7420 746f  ding the test to
+000057d0: 2072 6570 6c61 6365 0a20 2020 2020 2020   replace.       
+000057e0: 2063 6f6e 7374 7261 696e 7473 2077 6974   constraints wit
+000057f0: 6820 696e 6465 7865 7320 696e 2074 6573  h indexes in tes
+00005800: 7469 6e67 2064 6174 612e 0a20 2020 2020  ting data..     
+00005810: 2020 2022 2222 0a20 2020 2020 2020 206b     """.        k
+00005820: 7720 3d20 7465 6d70 5f74 6162 6c65 5f6b  w = temp_table_k
+00005830: 6579 776f 7264 5f61 7267 7328 636f 6e66  eyword_args(conf
+00005840: 6967 2c20 636f 6e66 6967 2e64 6229 0a20  ig, config.db). 
+00005850: 2020 2020 2020 2075 7365 725f 746d 7020         user_tmp 
+00005860: 3d20 5461 626c 6528 0a20 2020 2020 2020  = Table(.       
+00005870: 2020 2020 2022 7573 6572 5f74 6d70 222c       "user_tmp",
+00005880: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+00005890: 6164 6174 612c 0a20 2020 2020 2020 2020  adata,.         
+000058a0: 2020 2043 6f6c 756d 6e28 2269 6422 2c20     Column("id", 
+000058b0: 7371 6c61 6c63 6865 6d79 2e49 4e54 2c20  sqlalchemy.INT, 
+000058c0: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
+000058d0: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
+000058e0: 6f6c 756d 6e28 226e 616d 6522 2c20 7371  olumn("name", sq
+000058f0: 6c61 6c63 6865 6d79 2e56 4152 4348 4152  lalchemy.VARCHAR
+00005900: 2835 3029 292c 0a20 2020 2020 2020 2020  (50)),.         
+00005910: 2020 2043 6f6c 756d 6e28 2266 6f6f 222c     Column("foo",
+00005920: 2073 716c 616c 6368 656d 792e 494e 5429   sqlalchemy.INT)
+00005930: 2c0a 2020 2020 2020 2020 2020 2020 7371  ,.            sq
+00005940: 6c61 6c63 6865 6d79 2e49 6e64 6578 2822  lalchemy.Index("
+00005950: 7573 6572 5f74 6d70 5f75 7122 2c20 226e  user_tmp_uq", "n
+00005960: 616d 6522 2c20 756e 6971 7565 3d54 7275  ame", unique=Tru
+00005970: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+00005980: 7371 6c61 6c63 6865 6d79 2e49 6e64 6578  sqlalchemy.Index
+00005990: 2822 7573 6572 5f74 6d70 5f69 7822 2c20  ("user_tmp_ix", 
+000059a0: 2266 6f6f 2229 2c0a 2020 2020 2020 2020  "foo"),.        
+000059b0: 2020 2020 6578 7465 6e64 5f65 7869 7374      extend_exist
+000059c0: 696e 673d 5472 7565 2c0a 2020 2020 2020  ing=True,.      
+000059d0: 2020 2020 2020 2a2a 6b77 2c0a 2020 2020        **kw,.    
+000059e0: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
+000059f0: 2028 0a20 2020 2020 2020 2020 2020 2074   (.            t
+00005a00: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
+00005a10: 7669 6577 5f72 6566 6c65 6374 696f 6e2e  view_reflection.
+00005a20: 656e 6162 6c65 640a 2020 2020 2020 2020  enabled.        
+00005a30: 2020 2020 616e 6420 7465 7374 696e 672e      and testing.
+00005a40: 7265 7175 6972 6573 2e74 656d 706f 7261  requires.tempora
+00005a50: 7279 5f76 6965 7773 2e65 6e61 626c 6564  ry_views.enabled
+00005a60: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
+00005a70: 2020 2020 2020 2020 6576 656e 742e 6c69          event.li
+00005a80: 7374 656e 280a 2020 2020 2020 2020 2020  sten(.          
+00005a90: 2020 2020 2020 7573 6572 5f74 6d70 2c0a        user_tmp,.
+00005aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ab0: 2261 6674 6572 5f63 7265 6174 6522 2c0a  "after_create",.
+00005ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ad0: 4444 4c28 2263 7265 6174 6520 7465 6d70  DDL("create temp
+00005ae0: 6f72 6172 7920 7669 6577 2075 7365 725f  orary view user_
+00005af0: 746d 705f 7620 6173 2022 2022 7365 6c65  tmp_v as " "sele
+00005b00: 6374 202a 2066 726f 6d20 7573 6572 5f74  ct * from user_t
+00005b10: 6d70 2229 2c0a 2020 2020 2020 2020 2020  mp"),.          
+00005b20: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00005b30: 6576 656e 742e 6c69 7374 656e 2875 7365  event.listen(use
+00005b40: 725f 746d 702c 2022 6265 666f 7265 5f64  r_tmp, "before_d
+00005b50: 726f 7022 2c20 4444 4c28 2264 726f 7020  rop", DDL("drop 
+00005b60: 7669 6577 2075 7365 725f 746d 705f 7622  view user_tmp_v"
+00005b70: 2929 0a0a 2020 2020 4074 6573 7469 6e67  ))..    @testing
+00005b80: 2e70 726f 7669 6465 5f6d 6574 6164 6174  .provide_metadat
+00005b90: 610a 2020 2020 6465 6620 7465 7374 5f72  a.    def test_r
+00005ba0: 6566 6c65 6374 5f73 7472 696e 675f 636f  eflect_string_co
+00005bb0: 6c75 6d6e 5f6d 6178 5f6c 656e 2873 656c  lumn_max_len(sel
+00005bc0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+00005bd0: 2020 2020 2020 2020 5350 414e 4e45 5220          SPANNER 
+00005be0: 5350 4543 4946 4943 2054 4553 543a 0a0a  SPECIFIC TEST:..
+00005bf0: 2020 2020 2020 2020 496e 2053 7061 6e6e          In Spann
+00005c00: 6572 2063 6f6c 756d 6e20 6f66 2074 6865  er column of the
+00005c10: 2053 5452 494e 4720 7479 7065 2063 616e   STRING type can
+00005c20: 2062 650a 2020 2020 2020 2020 6372 6561   be.        crea
+00005c30: 7465 6420 7769 7468 2073 697a 6520 6465  ted with size de
+00005c40: 6669 6e65 6420 6173 204d 4158 2e20 5468  fined as MAX. Th
+00005c50: 6520 7465 7374 0a20 2020 2020 2020 2063  e test.        c
+00005c60: 6865 636b 7320 7468 6174 2073 7563 6820  hecks that such 
+00005c70: 6120 636f 6c75 6d6e 2069 7320 636f 7272  a column is corr
+00005c80: 6563 746c 7920 7265 666c 6563 7465 642e  ectly reflected.
+00005c90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00005ca0: 2020 2020 206d 6574 6164 6174 6120 3d20       metadata = 
+00005cb0: 4d65 7461 4461 7461 2873 656c 662e 6269  MetaData(self.bi
+00005cc0: 6e64 290a 2020 2020 2020 2020 5461 626c  nd).        Tabl
+00005cd0: 6528 2274 6578 745f 7461 626c 6522 2c20  e("text_table", 
+00005ce0: 6d65 7461 6461 7461 2c20 436f 6c75 6d6e  metadata, Column
+00005cf0: 2822 5465 7374 436f 6c75 6d6e 222c 2054  ("TestColumn", T
+00005d00: 6578 742c 206e 756c 6c61 626c 653d 4661  ext, nullable=Fa
+00005d10: 6c73 6529 290a 2020 2020 2020 2020 6d65  lse)).        me
+00005d20: 7461 6461 7461 2e63 7265 6174 655f 616c  tadata.create_al
+00005d30: 6c28 290a 0a20 2020 2020 2020 2054 6162  l()..        Tab
+00005d40: 6c65 2822 7465 7874 5f74 6162 6c65 222c  le("text_table",
+00005d50: 206d 6574 6164 6174 612c 2061 7574 6f6c   metadata, autol
+00005d60: 6f61 643d 5472 7565 290a 0a20 2020 2064  oad=True)..    d
+00005d70: 6566 2074 6573 745f 7265 666c 6563 745f  ef test_reflect_
+00005d80: 6279 7465 735f 636f 6c75 6d6e 5f6d 6178  bytes_column_max
+00005d90: 5f6c 656e 2873 656c 6629 3a0a 2020 2020  _len(self):.    
+00005da0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00005db0: 5350 414e 4e45 5220 5350 4543 4946 4943  SPANNER SPECIFIC
+00005dc0: 2054 4553 543a 0a0a 2020 2020 2020 2020   TEST:..        
+00005dd0: 496e 2053 7061 6e6e 6572 2063 6f6c 756d  In Spanner colum
+00005de0: 6e20 6f66 2074 6865 2042 5954 4553 2074  n of the BYTES t
+00005df0: 7970 6520 6361 6e20 6265 0a20 2020 2020  ype can be.     
+00005e00: 2020 2063 7265 6174 6564 2077 6974 6820     created with 
+00005e10: 7369 7a65 2064 6566 696e 6564 2061 7320  size defined as 
+00005e20: 4d41 582e 2054 6865 2074 6573 740a 2020  MAX. The test.  
+00005e30: 2020 2020 2020 6368 6563 6b73 2074 6861        checks tha
+00005e40: 7420 7375 6368 2061 2063 6f6c 756d 6e20  t such a column 
+00005e50: 6973 2063 6f72 7265 6374 6c79 2072 6566  is correctly ref
+00005e60: 6c65 6374 6564 2e0a 2020 2020 2020 2020  lected..        
+00005e70: 2222 220a 2020 2020 2020 2020 6d65 7461  """.        meta
+00005e80: 6461 7461 203d 204d 6574 6144 6174 6128  data = MetaData(
+00005e90: 7365 6c66 2e62 696e 6429 0a20 2020 2020  self.bind).     
+00005ea0: 2020 2054 6162 6c65 280a 2020 2020 2020     Table(.      
+00005eb0: 2020 2020 2020 2262 7974 6573 5f74 6162        "bytes_tab
+00005ec0: 6c65 222c 0a20 2020 2020 2020 2020 2020  le",.           
+00005ed0: 206d 6574 6164 6174 612c 0a20 2020 2020   metadata,.     
+00005ee0: 2020 2020 2020 2043 6f6c 756d 6e28 2254         Column("T
+00005ef0: 6573 7443 6f6c 756d 6e22 2c20 4c61 7267  estColumn", Larg
+00005f00: 6542 696e 6172 792c 206e 756c 6c61 626c  eBinary, nullabl
+00005f10: 653d 4661 6c73 6529 2c0a 2020 2020 2020  e=False),.      
+00005f20: 2020 290a 2020 2020 2020 2020 6d65 7461    ).        meta
+00005f30: 6461 7461 2e63 7265 6174 655f 616c 6c28  data.create_all(
+00005f40: 290a 0a20 2020 2020 2020 2054 6162 6c65  )..        Table
+00005f50: 2822 6279 7465 735f 7461 626c 6522 2c20  ("bytes_table", 
+00005f60: 6d65 7461 6461 7461 2c20 6175 746f 6c6f  metadata, autolo
+00005f70: 6164 3d54 7275 6529 0a0a 2020 2020 4074  ad=True)..    @t
+00005f80: 6573 7469 6e67 2e63 6f6d 6269 6e61 7469  esting.combinati
+00005f90: 6f6e 7328 0a20 2020 2020 2020 2028 5472  ons(.        (Tr
+00005fa0: 7565 2c20 7465 7374 696e 672e 7265 7175  ue, testing.requ
+00005fb0: 6972 6573 2e73 6368 656d 6173 292c 2028  ires.schemas), (
+00005fc0: 4661 6c73 652c 292c 2061 7267 6e61 6d65  False,), argname
+00005fd0: 733d 2275 7365 5f73 6368 656d 6122 0a20  s="use_schema". 
+00005fe0: 2020 2029 0a20 2020 2040 7465 7374 696e     ).    @testin
+00005ff0: 672e 7265 7175 6972 6573 2e75 6e69 7175  g.requires.uniqu
+00006000: 655f 636f 6e73 7472 6169 6e74 5f72 6566  e_constraint_ref
+00006010: 6c65 6374 696f 6e0a 2020 2020 6465 6620  lection.    def 
+00006020: 7465 7374 5f67 6574 5f75 6e69 7175 655f  test_get_unique_
+00006030: 636f 6e73 7472 6169 6e74 7328 7365 6c66  constraints(self
+00006040: 2c20 6d65 7461 6461 7461 2c20 636f 6e6e  , metadata, conn
+00006050: 6563 7469 6f6e 2c20 7573 655f 7363 6865  ection, use_sche
+00006060: 6d61 293a 0a20 2020 2020 2020 2023 2053  ma):.        # S
+00006070: 514c 6974 6520 6469 616c 6563 7420 6e65  QLite dialect ne
+00006080: 6564 7320 746f 2070 6172 7365 2074 6865  eds to parse the
+00006090: 206e 616d 6573 206f 6620 7468 6520 636f   names of the co
+000060a0: 6e73 7472 6169 6e74 730a 2020 2020 2020  nstraints.      
+000060b0: 2020 2320 7365 7061 7261 7465 6c79 2066    # separately f
+000060c0: 726f 6d20 7768 6174 2069 7420 6765 7473  rom what it gets
+000060d0: 2066 726f 6d20 5052 4147 4d41 2069 6e64   from PRAGMA ind
+000060e0: 6578 5f6c 6973 7428 292c 2061 6e64 0a20  ex_list(), and. 
+000060f0: 2020 2020 2020 2023 2074 6865 6e20 6d61         # then ma
+00006100: 7463 6865 7320 7468 656d 2075 702e 2020  tches them up.  
+00006110: 736f 2073 616d 6520 7365 7420 6f66 2063  so same set of c
+00006120: 6f6c 756d 6e5f 6e61 6d65 7320 696e 2074  olumn_names in t
+00006130: 776f 0a20 2020 2020 2020 2023 2063 6f6e  wo.        # con
+00006140: 7374 7261 696e 7473 2077 696c 6c20 636f  straints will co
+00006150: 6e66 7573 6520 6974 2e20 2020 2050 6572  nfuse it.    Per
+00006160: 6861 7073 2077 6520 7368 6f75 6c64 206e  haps we should n
+00006170: 6f20 6c6f 6e67 6572 0a20 2020 2020 2020  o longer.       
+00006180: 2023 2062 6f74 6865 7220 7769 7468 2069   # bother with i
+00006190: 6e64 6578 5f6c 6973 7428 2920 6865 7265  ndex_list() here
+000061a0: 2073 696e 6365 2077 6520 6861 7665 2074   since we have t
+000061b0: 6865 2077 686f 6c65 0a20 2020 2020 2020  he whole.       
+000061c0: 2023 2043 5245 4154 4520 5441 424c 453f   # CREATE TABLE?
+000061d0: 0a0a 2020 2020 2020 2020 6966 2075 7365  ..        if use
+000061e0: 5f73 6368 656d 613a 0a20 2020 2020 2020  _schema:.       
+000061f0: 2020 2020 2073 6368 656d 6120 3d20 636f       schema = co
+00006200: 6e66 6967 2e74 6573 745f 7363 6865 6d61  nfig.test_schema
+00006210: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00006220: 2020 2020 2020 2020 2020 2073 6368 656d             schem
+00006230: 6120 3d20 4e6f 6e65 0a20 2020 2020 2020  a = None.       
+00006240: 2075 6e69 7175 6573 203d 2073 6f72 7465   uniques = sorte
+00006250: 6428 0a20 2020 2020 2020 2020 2020 205b  d(.            [
+00006260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006270: 207b 226e 616d 6522 3a20 2275 6e69 7175   {"name": "uniqu
+00006280: 655f 6122 2c20 2263 6f6c 756d 6e5f 6e61  e_a", "column_na
+00006290: 6d65 7322 3a20 5b22 6122 5d7d 2c0a 2020  mes": ["a"]},.  
+000062a0: 2020 2020 2020 2020 2020 2020 2020 7b22                {"
+000062b0: 6e61 6d65 223a 2022 756e 6971 7565 5f61  name": "unique_a
+000062c0: 5f62 5f63 222c 2022 636f 6c75 6d6e 5f6e  _b_c", "column_n
+000062d0: 616d 6573 223a 205b 2261 222c 2022 6222  ames": ["a", "b"
+000062e0: 2c20 2263 225d 7d2c 0a20 2020 2020 2020  , "c"]},.       
+000062f0: 2020 2020 2020 2020 207b 226e 616d 6522           {"name"
+00006300: 3a20 2275 6e69 7175 655f 635f 615f 6222  : "unique_c_a_b"
+00006310: 2c20 2263 6f6c 756d 6e5f 6e61 6d65 7322  , "column_names"
+00006320: 3a20 5b22 6322 2c20 2261 222c 2022 6222  : ["c", "a", "b"
+00006330: 5d7d 2c0a 2020 2020 2020 2020 2020 2020  ]},.            
+00006340: 2020 2020 7b22 6e61 6d65 223a 2022 756e      {"name": "un
+00006350: 6971 7565 5f61 7363 5f6b 6579 222c 2022  ique_asc_key", "
+00006360: 636f 6c75 6d6e 5f6e 616d 6573 223a 205b  column_names": [
+00006370: 2261 7363 222c 2022 6b65 7922 5d7d 2c0a  "asc", "key"]},.
+00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006390: 7b22 6e61 6d65 223a 2022 692e 6861 7665  {"name": "i.have
+000063a0: 2e64 6f74 7322 2c20 2263 6f6c 756d 6e5f  .dots", "column_
+000063b0: 6e61 6d65 7322 3a20 5b22 6222 5d7d 2c0a  names": ["b"]},.
+000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063d0: 7b22 6e61 6d65 223a 2022 6920 6861 7665  {"name": "i have
+000063e0: 2073 7061 6365 7322 2c20 2263 6f6c 756d   spaces", "colum
+000063f0: 6e5f 6e61 6d65 7322 3a20 5b22 6322 5d7d  n_names": ["c"]}
+00006400: 2c0a 2020 2020 2020 2020 2020 2020 5d2c  ,.            ],
+00006410: 0a20 2020 2020 2020 2020 2020 206b 6579  .            key
+00006420: 3d6f 7065 7261 746f 722e 6974 656d 6765  =operator.itemge
+00006430: 7474 6572 2822 6e61 6d65 2229 2c0a 2020  tter("name"),.  
+00006440: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00006450: 7461 626c 6520 3d20 5461 626c 6528 0a20  table = Table(. 
+00006460: 2020 2020 2020 2020 2020 2022 7465 7374             "test
+00006470: 7462 6c22 2c0a 2020 2020 2020 2020 2020  tbl",.          
+00006480: 2020 6d65 7461 6461 7461 2c0a 2020 2020    metadata,.    
+00006490: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+000064a0: 6964 222c 2073 716c 616c 6368 656d 792e  id", sqlalchemy.
+000064b0: 494e 542c 2070 7269 6d61 7279 5f6b 6579  INT, primary_key
+000064c0: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
+000064d0: 2020 2020 436f 6c75 6d6e 2822 6122 2c20      Column("a", 
+000064e0: 5374 7269 6e67 2832 3029 292c 0a20 2020  String(20)),.   
+000064f0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00006500: 2262 222c 2053 7472 696e 6728 3330 2929  "b", String(30))
+00006510: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
+00006520: 6c75 6d6e 2822 6322 2c20 496e 7465 6765  lumn("c", Intege
+00006530: 7229 2c0a 2020 2020 2020 2020 2020 2020  r),.            
+00006540: 2320 7265 7365 7276 6564 2069 6465 6e74  # reserved ident
+00006550: 6966 6965 7273 0a20 2020 2020 2020 2020  ifiers.         
+00006560: 2020 2043 6f6c 756d 6e28 2261 7363 222c     Column("asc",
+00006570: 2053 7472 696e 6728 3330 2929 2c0a 2020   String(30)),.  
+00006580: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
+00006590: 2822 6b65 7922 2c20 5374 7269 6e67 2833  ("key", String(3
+000065a0: 3029 292c 0a20 2020 2020 2020 2020 2020  0)),.           
+000065b0: 2073 716c 616c 6368 656d 792e 496e 6465   sqlalchemy.Inde
+000065c0: 7828 2275 6e69 7175 655f 6122 2c20 2261  x("unique_a", "a
+000065d0: 222c 2075 6e69 7175 653d 5472 7565 292c  ", unique=True),
+000065e0: 0a20 2020 2020 2020 2020 2020 2073 716c  .            sql
+000065f0: 616c 6368 656d 792e 496e 6465 7828 2275  alchemy.Index("u
+00006600: 6e69 7175 655f 615f 625f 6322 2c20 2261  nique_a_b_c", "a
+00006610: 222c 2022 6222 2c20 2263 222c 2075 6e69  ", "b", "c", uni
+00006620: 7175 653d 5472 7565 292c 0a20 2020 2020  que=True),.     
+00006630: 2020 2020 2020 2073 716c 616c 6368 656d         sqlalchem
+00006640: 792e 496e 6465 7828 2275 6e69 7175 655f  y.Index("unique_
+00006650: 635f 615f 6222 2c20 2263 222c 2022 6122  c_a_b", "c", "a"
+00006660: 2c20 2262 222c 2075 6e69 7175 653d 5472  , "b", unique=Tr
+00006670: 7565 292c 0a20 2020 2020 2020 2020 2020  ue),.           
+00006680: 2073 716c 616c 6368 656d 792e 496e 6465   sqlalchemy.Inde
+00006690: 7828 2275 6e69 7175 655f 6173 635f 6b65  x("unique_asc_ke
+000066a0: 7922 2c20 2261 7363 222c 2022 6b65 7922  y", "asc", "key"
+000066b0: 2c20 756e 6971 7565 3d54 7275 6529 2c0a  , unique=True),.
+000066c0: 2020 2020 2020 2020 2020 2020 7363 6865              sche
+000066d0: 6d61 3d73 6368 656d 612c 0a20 2020 2020  ma=schema,.     
+000066e0: 2020 2029 0a20 2020 2020 2020 2074 6162     ).        tab
+000066f0: 6c65 2e63 7265 6174 6528 636f 6e6e 6563  le.create(connec
+00006700: 7469 6f6e 290a 2020 2020 2020 2020 636f  tion).        co
+00006710: 6e6e 6563 7469 6f6e 2e63 6f6e 6e65 6374  nnection.connect
+00006720: 696f 6e2e 636f 6d6d 6974 2829 0a0a 2020  ion.commit()..  
+00006730: 2020 2020 2020 696e 7370 6563 746f 7220        inspector 
+00006740: 3d20 696e 7370 6563 7428 636f 6e6e 6563  = inspect(connec
+00006750: 7469 6f6e 290a 2020 2020 2020 2020 7265  tion).        re
+00006760: 666c 6563 7465 6420 3d20 736f 7274 6564  flected = sorted
+00006770: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
+00006780: 7370 6563 746f 722e 6765 745f 756e 6971  spector.get_uniq
+00006790: 7565 5f63 6f6e 7374 7261 696e 7473 2822  ue_constraints("
+000067a0: 7465 7374 7462 6c22 2c20 7363 6865 6d61  testtbl", schema
+000067b0: 3d73 6368 656d 6129 2c0a 2020 2020 2020  =schema),.      
+000067c0: 2020 2020 2020 6b65 793d 6f70 6572 6174        key=operat
+000067d0: 6f72 2e69 7465 6d67 6574 7465 7228 226e  or.itemgetter("n
+000067e0: 616d 6522 292c 0a20 2020 2020 2020 2029  ame"),.        )
+000067f0: 0a0a 2020 2020 2020 2020 6e61 6d65 735f  ..        names_
+00006800: 7468 6174 5f64 7570 6c69 6361 7465 5f69  that_duplicate_i
+00006810: 6e64 6578 203d 2073 6574 2829 0a0a 2020  ndex = set()..  
+00006820: 2020 2020 2020 666f 7220 6f72 6967 2c20        for orig, 
+00006830: 7265 666c 2069 6e20 7a69 7028 756e 6971  refl in zip(uniq
+00006840: 7565 732c 2072 6566 6c65 6374 6564 293a  ues, reflected):
+00006850: 0a20 2020 2020 2020 2020 2020 2023 2044  .            # D
+00006860: 6966 6665 7265 6e74 2064 6961 6c65 6374  ifferent dialect
+00006870: 7320 6861 6e64 6c65 2064 7570 6c69 6361  s handle duplica
+00006880: 7465 2069 6e64 6578 2061 6e64 2063 6f6e  te index and con
+00006890: 7374 7261 696e 7473 0a20 2020 2020 2020  straints.       
+000068a0: 2020 2020 2023 2064 6966 6665 7265 6e74       # different
+000068b0: 6c79 2c20 736f 2069 676e 6f72 6520 7468  ly, so ignore th
+000068c0: 6973 2066 6c61 670a 2020 2020 2020 2020  is flag.        
+000068d0: 2020 2020 6475 7065 203d 2072 6566 6c2e      dupe = refl.
+000068e0: 706f 7028 2264 7570 6c69 6361 7465 735f  pop("duplicates_
+000068f0: 696e 6465 7822 2c20 4e6f 6e65 290a 2020  index", None).  
+00006900: 2020 2020 2020 2020 2020 6966 2064 7570            if dup
+00006910: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00006920: 2020 206e 616d 6573 5f74 6861 745f 6475     names_that_du
+00006930: 706c 6963 6174 655f 696e 6465 782e 6164  plicate_index.ad
+00006940: 6428 6475 7065 290a 2020 2020 2020 2020  d(dupe).        
+00006950: 2020 2020 6571 5f28 6f72 6967 2c20 7265      eq_(orig, re
+00006960: 666c 290a 0a20 2020 2020 2020 2072 6566  fl)..        ref
+00006970: 6c65 6374 6564 5f6d 6574 6164 6174 6120  lected_metadata 
+00006980: 3d20 4d65 7461 4461 7461 2829 0a20 2020  = MetaData().   
+00006990: 2020 2020 2072 6566 6c65 6374 6564 203d       reflected =
+000069a0: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
+000069b0: 2020 2020 2274 6573 7474 626c 222c 0a20      "testtbl",. 
+000069c0: 2020 2020 2020 2020 2020 2072 6566 6c65             refle
+000069d0: 6374 6564 5f6d 6574 6164 6174 612c 0a20  cted_metadata,. 
+000069e0: 2020 2020 2020 2020 2020 2061 7574 6f6c             autol
+000069f0: 6f61 645f 7769 7468 3d63 6f6e 6e65 6374  oad_with=connect
+00006a00: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00006a10: 2073 6368 656d 613d 7363 6865 6d61 2c0a   schema=schema,.
+00006a20: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00006a30: 2020 2023 2074 6573 7420 2264 6564 7570     # test "dedup
+00006a40: 6c69 6361 7465 7320 666f 7220 696e 6465  licates for inde
+00006a50: 7822 206c 6f67 6963 2e20 2020 4d79 5351  x" logic.   MySQ
+00006a60: 4c20 616e 6420 4f72 6163 6c65 0a20 2020  L and Oracle.   
+00006a70: 2020 2020 2023 2022 756e 6971 7565 2063       # "unique c
+00006a80: 6f6e 7374 7261 696e 7473 2220 6172 6520  onstraints" are 
+00006a90: 6163 7475 616c 6c79 2075 6e69 7175 6520  actually unique 
+00006aa0: 696e 6465 7865 7320 2877 6974 6820 706f  indexes (with po
+00006ab0: 7373 6962 6c65 0a20 2020 2020 2020 2023  ssible.        #
+00006ac0: 2065 7863 6570 7469 6f6e 206f 6620 6120   exception of a 
+00006ad0: 756e 6971 7565 2074 6861 7420 6973 2061  unique that is a
+00006ae0: 2064 7570 6520 6f66 2061 6e6f 7468 6572   dupe of another
+00006af0: 206f 6e65 2069 6e20 7468 6520 6361 7365   one in the case
+00006b00: 0a20 2020 2020 2020 2023 206f 6620 4f72  .        # of Or
+00006b10: 6163 6c65 292e 2020 6d61 6b65 2073 7572  acle).  make sur
+00006b20: 6520 2320 7468 6579 2061 7265 6e27 7420  e # they aren't 
+00006b30: 6475 706c 6963 6174 6564 2e0a 2020 2020  duplicated..    
+00006b40: 2020 2020 6964 785f 6e61 6d65 7320 3d20      idx_names = 
+00006b50: 7365 7428 5b69 6478 2e6e 616d 6520 666f  set([idx.name fo
+00006b60: 7220 6964 7820 696e 2072 6566 6c65 6374  r idx in reflect
+00006b70: 6564 2e69 6e64 6578 6573 5d29 0a20 2020  ed.indexes]).   
+00006b80: 2020 2020 2075 715f 6e61 6d65 7320 3d20       uq_names = 
+00006b90: 7365 7428 0a20 2020 2020 2020 2020 2020  set(.           
+00006ba0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00006bb0: 2020 2075 712e 6e61 6d65 0a20 2020 2020     uq.name.     
+00006bc0: 2020 2020 2020 2020 2020 2066 6f72 2075             for u
+00006bd0: 7120 696e 2072 6566 6c65 6374 6564 2e63  q in reflected.c
+00006be0: 6f6e 7374 7261 696e 7473 0a20 2020 2020  onstraints.     
+00006bf0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00006c00: 696e 7374 616e 6365 2875 712c 2073 716c  instance(uq, sql
+00006c10: 616c 6368 656d 792e 556e 6971 7565 436f  alchemy.UniqueCo
+00006c20: 6e73 7472 6169 6e74 290a 2020 2020 2020  nstraint).      
+00006c30: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00006c40: 292e 6469 6666 6572 656e 6365 285b 2275  ).difference(["u
+00006c50: 6e69 7175 655f 635f 615f 6222 5d29 0a0a  nique_c_a_b"])..
+00006c60: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
+00006c70: 6f74 2069 6478 5f6e 616d 6573 2e69 6e74  ot idx_names.int
+00006c80: 6572 7365 6374 696f 6e28 7571 5f6e 616d  ersection(uq_nam
+00006c90: 6573 290a 2020 2020 2020 2020 6966 206e  es).        if n
+00006ca0: 616d 6573 5f74 6861 745f 6475 706c 6963  ames_that_duplic
+00006cb0: 6174 655f 696e 6465 783a 0a20 2020 2020  ate_index:.     
+00006cc0: 2020 2020 2020 2065 715f 286e 616d 6573         eq_(names
+00006cd0: 5f74 6861 745f 6475 706c 6963 6174 655f  _that_duplicate_
+00006ce0: 696e 6465 782c 2069 6478 5f6e 616d 6573  index, idx_names
+00006cf0: 290a 2020 2020 2020 2020 2020 2020 6571  ).            eq
+00006d00: 5f28 7571 5f6e 616d 6573 2c20 7365 7428  _(uq_names, set(
+00006d10: 2929 0a0a 2020 2020 4074 6573 7469 6e67  ))..    @testing
+00006d20: 2e70 726f 7669 6465 5f6d 6574 6164 6174  .provide_metadat
+00006d30: 610a 2020 2020 6465 6620 7465 7374 5f75  a.    def test_u
+00006d40: 6e69 7175 655f 636f 6e73 7472 6169 6e74  nique_constraint
+00006d50: 5f72 6169 7365 7328 7365 6c66 293a 0a20  _raises(self):. 
+00006d60: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006d70: 2020 2043 6865 636b 696e 6720 7468 6174     Checking that
+00006d80: 2075 6e69 7175 6520 636f 6e73 7472 6169   unique constrai
+00006d90: 6e74 2063 7265 6174 696f 6e0a 2020 2020  nt creation.    
+00006da0: 2020 2020 6661 696c 7320 6475 6520 746f      fails due to
+00006db0: 2061 2050 726f 6772 616d 6d69 6e67 4572   a ProgrammingEr
+00006dc0: 726f 722e 0a20 2020 2020 2020 2022 2222  ror..        """
+00006dd0: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
+00006de0: 6120 3d20 4d65 7461 4461 7461 2873 656c  a = MetaData(sel
+00006df0: 662e 6269 6e64 290a 2020 2020 2020 2020  f.bind).        
+00006e00: 5461 626c 6528 0a20 2020 2020 2020 2020  Table(.         
+00006e10: 2020 2022 7573 6572 5f74 6d70 5f66 6169     "user_tmp_fai
+00006e20: 6c75 7265 222c 0a20 2020 2020 2020 2020  lure",.         
+00006e30: 2020 206d 6574 6164 6174 612c 0a20 2020     metadata,.   
+00006e40: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00006e50: 2269 6422 2c20 7371 6c61 6c63 6865 6d79  "id", sqlalchemy
+00006e60: 2e49 4e54 2c20 7072 696d 6172 795f 6b65  .INT, primary_ke
+00006e70: 793d 5472 7565 292c 0a20 2020 2020 2020  y=True),.       
+00006e80: 2020 2020 2043 6f6c 756d 6e28 226e 616d       Column("nam
+00006e90: 6522 2c20 7371 6c61 6c63 6865 6d79 2e56  e", sqlalchemy.V
+00006ea0: 4152 4348 4152 2835 3029 292c 0a20 2020  ARCHAR(50)),.   
+00006eb0: 2020 2020 2020 2020 2073 716c 616c 6368           sqlalch
+00006ec0: 656d 792e 556e 6971 7565 436f 6e73 7472  emy.UniqueConstr
+00006ed0: 6169 6e74 2822 6e61 6d65 222c 206e 616d  aint("name", nam
+00006ee0: 653d 2275 7365 725f 746d 705f 7571 2229  e="user_tmp_uq")
+00006ef0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00006f00: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
+00006f10: 2e72 6169 7365 7328 7370 616e 6e65 725f  .raises(spanner_
+00006f20: 6462 6170 692e 6578 6365 7074 696f 6e73  dbapi.exceptions
+00006f30: 2e50 726f 6772 616d 6d69 6e67 4572 726f  .ProgrammingErro
+00006f40: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00006f50: 6d65 7461 6461 7461 2e63 7265 6174 655f  metadata.create_
+00006f60: 616c 6c28 290a 0a20 2020 2040 7465 7374  all()..    @test
+00006f70: 696e 672e 7072 6f76 6964 655f 6d65 7461  ing.provide_meta
+00006f80: 6461 7461 0a20 2020 2064 6566 205f 7465  data.    def _te
+00006f90: 7374 5f67 6574 5f74 6162 6c65 5f6e 616d  st_get_table_nam
+00006fa0: 6573 2873 656c 662c 2073 6368 656d 613d  es(self, schema=
+00006fb0: 4e6f 6e65 2c20 7461 626c 655f 7479 7065  None, table_type
+00006fc0: 3d22 7461 626c 6522 2c20 6f72 6465 725f  ="table", order_
+00006fd0: 6279 3d4e 6f6e 6529 3a0a 2020 2020 2020  by=None):.      
+00006fe0: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
+00006ff0: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
+00007000: 0a20 2020 2020 2020 2053 7061 6e6e 6572  .        Spanner
+00007010: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
+00007020: 2074 656d 706f 7261 7279 2074 6162 6c65   temporary table
+00007030: 732c 2073 6f20 7265 616c 2074 6162 6c65  s, so real table
+00007040: 7320 6172 650a 2020 2020 2020 2020 7573  s are.        us
+00007050: 6564 2066 6f72 2074 6573 7469 6e67 2e20  ed for testing. 
+00007060: 4173 2074 6865 206f 7269 6769 6e61 6c20  As the original 
+00007070: 7465 7374 2065 7870 6563 7473 206f 6e6c  test expects onl
+00007080: 7920 7265 616c 0a20 2020 2020 2020 2074  y real.        t
+00007090: 6162 6c65 7320 746f 2062 6520 7265 6164  ables to be read
+000070a0: 2c20 616e 6420 696e 2053 7061 6e6e 6572  , and in Spanner
+000070b0: 2061 6c6c 2074 6865 2074 6162 6c65 7320   all the tables 
+000070c0: 6172 6520 7265 616c 2c0a 2020 2020 2020  are real,.      
+000070d0: 2020 6578 7065 6374 6564 2072 6573 756c    expected resul
+000070e0: 7473 206f 7665 7272 6964 6520 6973 2072  ts override is r
+000070f0: 6571 7569 7265 642e 0a20 2020 2020 2020  equired..       
+00007100: 2022 2222 0a20 2020 2020 2020 205f 6967   """.        _ig
+00007110: 6e6f 7265 5f74 6162 6c65 7320 3d20 5b0a  nore_tables = [.
+00007120: 2020 2020 2020 2020 2020 2020 2263 6f6d              "com
+00007130: 6d65 6e74 5f74 6573 7422 2c0a 2020 2020  ment_test",.    
+00007140: 2020 2020 2020 2020 226e 6f6e 636f 6c5f          "noncol_
+00007150: 6964 785f 7465 7374 5f70 6b22 2c0a 2020  idx_test_pk",.  
+00007160: 2020 2020 2020 2020 2020 226e 6f6e 636f            "nonco
+00007170: 6c5f 6964 785f 7465 7374 5f6e 6f70 6b22  l_idx_test_nopk"
+00007180: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
+00007190: 6f63 616c 5f74 6162 6c65 222c 0a20 2020  ocal_table",.   
+000071a0: 2020 2020 2020 2020 2022 7265 6d6f 7465           "remote
+000071b0: 5f74 6162 6c65 222c 0a20 2020 2020 2020  _table",.       
+000071c0: 2020 2020 2022 7265 6d6f 7465 5f74 6162       "remote_tab
+000071d0: 6c65 5f32 222c 0a20 2020 2020 2020 205d  le_2",.        ]
+000071e0: 0a20 2020 2020 2020 206d 6574 6120 3d20  .        meta = 
+000071f0: 7365 6c66 2e6d 6574 6164 6174 610a 0a20  self.metadata.. 
+00007200: 2020 2020 2020 2069 6e73 7020 3d20 696e         insp = in
+00007210: 7370 6563 7428 6d65 7461 2e62 696e 6429  spect(meta.bind)
+00007220: 0a0a 2020 2020 2020 2020 6966 2074 6162  ..        if tab
+00007230: 6c65 5f74 7970 6520 3d3d 2022 7669 6577  le_type == "view
+00007240: 2220 616e 6420 6e6f 7420 626f 6f6c 286f  " and not bool(o
+00007250: 732e 656e 7669 726f 6e2e 6765 7428 2253  s.environ.get("S
+00007260: 5041 4e4e 4552 5f45 4d55 4c41 544f 525f  PANNER_EMULATOR_
+00007270: 484f 5354 2229 293a 0a20 2020 2020 2020  HOST")):.       
+00007280: 2020 2020 2074 6162 6c65 5f6e 616d 6573       table_names
+00007290: 203d 2069 6e73 702e 6765 745f 7669 6577   = insp.get_view
+000072a0: 5f6e 616d 6573 2873 6368 656d 6129 0a20  _names(schema). 
+000072b0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+000072c0: 5f6e 616d 6573 2e73 6f72 7428 290a 2020  _names.sort().  
+000072d0: 2020 2020 2020 2020 2020 616e 7377 6572            answer
+000072e0: 203d 205b 2265 6d61 696c 5f61 6464 7265   = ["email_addre
+000072f0: 7373 6573 5f76 222c 2022 7573 6572 735f  sses_v", "users_
+00007300: 7622 5d0a 2020 2020 2020 2020 2020 2020  v"].            
+00007310: 6571 5f28 736f 7274 6564 2874 6162 6c65  eq_(sorted(table
+00007320: 5f6e 616d 6573 292c 2061 6e73 7765 7229  _names), answer)
+00007330: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00007340: 2020 2020 2020 2020 2020 2069 6620 6f72             if or
+00007350: 6465 725f 6279 3a0a 2020 2020 2020 2020  der_by:.        
+00007360: 2020 2020 2020 2020 7461 626c 6573 203d          tables =
+00007370: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00007380: 2020 2020 2020 2072 6563 5b30 5d0a 2020         rec[0].  
+00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073a0: 2020 666f 7220 7265 6320 696e 2069 6e73    for rec in ins
+000073b0: 702e 6765 745f 736f 7274 6564 5f74 6162  p.get_sorted_tab
+000073c0: 6c65 5f61 6e64 5f66 6b63 5f6e 616d 6573  le_and_fkc_names
+000073d0: 2873 6368 656d 6129 0a20 2020 2020 2020  (schema).       
+000073e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000073f0: 7265 635b 305d 0a20 2020 2020 2020 2020  rec[0].         
+00007400: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00007410: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00007420: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+00007430: 7320 3d20 696e 7370 2e67 6574 5f74 6162  s = insp.get_tab
+00007440: 6c65 5f6e 616d 6573 2873 6368 656d 6129  le_names(schema)
+00007450: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
+00007460: 6c65 5f6e 616d 6573 203d 205b 7420 666f  le_names = [t fo
+00007470: 7220 7420 696e 2074 6162 6c65 7320 6966  r t in tables if
+00007480: 2074 206e 6f74 2069 6e20 5f69 676e 6f72   t not in _ignor
+00007490: 655f 7461 626c 6573 5d0a 0a20 2020 2020  e_tables]..     
+000074a0: 2020 2020 2020 2069 6620 6f72 6465 725f         if order_
+000074b0: 6279 203d 3d20 2266 6f72 6569 676e 5f6b  by == "foreign_k
+000074c0: 6579 223a 0a20 2020 2020 2020 2020 2020  ey":.           
+000074d0: 2020 2020 2061 6e73 7765 7220 3d20 7b22       answer = {"
+000074e0: 6469 6e67 616c 696e 6773 222c 2022 656d  dingalings", "em
+000074f0: 6169 6c5f 6164 6472 6573 7365 7322 2c20  ail_addresses", 
+00007500: 2275 7365 725f 746d 7022 2c20 2275 7365  "user_tmp", "use
+00007510: 7273 227d 0a20 2020 2020 2020 2020 2020  rs"}.           
+00007520: 2020 2020 2065 715f 2873 6574 2874 6162       eq_(set(tab
+00007530: 6c65 5f6e 616d 6573 292c 2061 6e73 7765  le_names), answe
+00007540: 7229 0a20 2020 2020 2020 2020 2020 2065  r).            e
+00007550: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00007560: 2020 2020 2061 6e73 7765 7220 3d20 5b22       answer = ["
+00007570: 6469 6e67 616c 696e 6773 222c 2022 656d  dingalings", "em
+00007580: 6169 6c5f 6164 6472 6573 7365 7322 2c20  ail_addresses", 
+00007590: 2275 7365 725f 746d 7022 2c20 2275 7365  "user_tmp", "use
+000075a0: 7273 225d 0a20 2020 2020 2020 2020 2020  rs"].           
+000075b0: 2020 2020 2065 715f 2873 6f72 7465 6428       eq_(sorted(
+000075c0: 7461 626c 655f 6e61 6d65 7329 2c20 616e  table_names), an
+000075d0: 7377 6572 290a 0a20 2020 2040 7079 7465  swer)..    @pyte
+000075e0: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
+000075f0: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
+00007600: 7070 6f72 7420 7465 6d70 6f72 6172 7920  pport temporary 
+00007610: 7461 626c 6573 2229 0a20 2020 2064 6566  tables").    def
+00007620: 2074 6573 745f 6765 745f 7465 6d70 5f74   test_get_temp_t
+00007630: 6162 6c65 5f69 6e64 6578 6573 2873 656c  able_indexes(sel
+00007640: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00007650: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
+00007660: 726b 2e73 6b69 7028 2253 7061 6e6e 6572  rk.skip("Spanner
+00007670: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
+00007680: 2074 656d 706f 7261 7279 2074 6162 6c65   temporary table
+00007690: 7322 290a 2020 2020 6465 6620 7465 7374  s").    def test
+000076a0: 5f67 6574 5f74 656d 705f 7461 626c 655f  _get_temp_table_
+000076b0: 756e 6971 7565 5f63 6f6e 7374 7261 696e  unique_constrain
+000076c0: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
+000076d0: 2020 7061 7373 0a0a 2020 2020 4070 7974    pass..    @pyt
+000076e0: 6573 742e 6d61 726b 2e73 6b69 7028 2253  est.mark.skip("S
+000076f0: 7061 6e6e 6572 2064 6f65 736e 2774 2073  panner doesn't s
+00007700: 7570 706f 7274 2074 656d 706f 7261 7279  upport temporary
+00007710: 2074 6162 6c65 7322 290a 2020 2020 6465   tables").    de
+00007720: 6620 7465 7374 5f67 6574 5f74 656d 705f  f test_get_temp_
+00007730: 7461 626c 655f 636f 6c75 6d6e 7328 7365  table_columns(se
+00007740: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+00007750: 730a 0a20 2020 2064 6566 205f 6173 7365  s..    def _asse
+00007760: 7274 5f69 6e73 705f 696e 6465 7865 7328  rt_insp_indexes(
+00007770: 7365 6c66 2c20 696e 6465 7865 732c 2065  self, indexes, e
+00007780: 7870 6563 7465 645f 696e 6465 7865 7329  xpected_indexes)
+00007790: 3a0a 2020 2020 2020 2020 6578 7065 6374  :.        expect
+000077a0: 6564 5f69 6e64 6578 6573 2e73 6f72 7428  ed_indexes.sort(
+000077b0: 6b65 793d 6c61 6d62 6461 2069 7465 6d3a  key=lambda item:
+000077c0: 2069 7465 6d5b 226e 616d 6522 5d29 0a0a   item["name"])..
+000077d0: 2020 2020 2020 2020 696e 6465 785f 6e61          index_na
+000077e0: 6d65 7320 3d20 5b64 5b22 6e61 6d65 225d  mes = [d["name"]
+000077f0: 2066 6f72 2064 2069 6e20 696e 6465 7865   for d in indexe
+00007800: 735d 0a20 2020 2020 2020 2065 7870 5f69  s].        exp_i
+00007810: 6e64 6578 5f6e 616d 6573 203d 205b 645b  ndex_names = [d[
+00007820: 226e 616d 6522 5d20 666f 7220 6420 696e  "name"] for d in
+00007830: 2065 7870 6563 7465 645f 696e 6465 7865   expected_indexe
+00007840: 735d 0a20 2020 2020 2020 2061 7373 6572  s].        asser
+00007850: 7420 736f 7274 6564 2869 6e64 6578 5f6e  t sorted(index_n
+00007860: 616d 6573 2920 3d3d 2073 6f72 7465 6428  ames) == sorted(
+00007870: 6578 705f 696e 6465 785f 6e61 6d65 7329  exp_index_names)
+00007880: 0a0a 0a63 6c61 7373 2043 6f6d 706f 7369  ...class Composi
+00007890: 7465 4b65 7952 6566 6c65 6374 696f 6e54  teKeyReflectionT
+000078a0: 6573 7428 5f43 6f6d 706f 7369 7465 4b65  est(_CompositeKe
+000078b0: 7952 6566 6c65 6374 696f 6e54 6573 7429  yReflectionTest)
+000078c0: 3a0a 2020 2020 4074 6573 7469 6e67 2e72  :.    @testing.r
+000078d0: 6571 7569 7265 732e 666f 7265 6967 6e5f  equires.foreign_
+000078e0: 6b65 795f 636f 6e73 7472 6169 6e74 5f72  key_constraint_r
+000078f0: 6566 6c65 6374 696f 6e0a 2020 2020 6465  eflection.    de
+00007900: 6620 7465 7374 5f66 6b5f 636f 6c75 6d6e  f test_fk_column
+00007910: 5f6f 7264 6572 2873 656c 6629 3a0a 2020  _order(self):.  
+00007920: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00007930: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
+00007940: 4445 3a0a 0a20 2020 2020 2020 2053 7061  DE:..        Spa
+00007950: 6e6e 6572 2063 6f6c 756d 6e20 7573 6167  nner column usag
+00007960: 6520 7265 666c 6563 7469 6f6e 2064 6f65  e reflection doe
+00007970: 736e 2774 2073 7570 706f 7274 2064 6574  sn't support det
+00007980: 6572 6d65 6e69 7374 6963 0a20 2020 2020  ermenistic.     
+00007990: 2020 206f 7264 6572 696e 672e 204f 7665     ordering. Ove
+000079a0: 7272 6964 696e 6720 7468 6520 7465 7374  rriding the test
+000079b0: 2074 6f20 6368 6563 6b20 7468 6174 2063   to check that c
+000079c0: 6f6c 756d 6e73 2061 7265 0a20 2020 2020  olumns are.     
+000079d0: 2020 2072 6566 6c65 6374 6564 2063 6f72     reflected cor
+000079e0: 7265 6374 6c79 2c20 7769 7468 6f75 7420  rectly, without 
+000079f0: 636f 6e73 6964 6572 696e 6720 7468 6569  considering thei
+00007a00: 7220 6f72 6465 722e 0a20 2020 2020 2020  r order..       
+00007a10: 2022 2222 0a20 2020 2020 2020 2023 2074   """.        # t
+00007a20: 6573 7420 666f 7220 6973 7375 6520 2335  est for issue #5
+00007a30: 3636 310a 2020 2020 2020 2020 696e 7370  661.        insp
+00007a40: 203d 2069 6e73 7065 6374 2873 656c 662e   = inspect(self.
+00007a50: 6269 6e64 290a 2020 2020 2020 2020 666f  bind).        fo
+00007a60: 7265 6967 6e5f 6b65 7973 203d 2069 6e73  reign_keys = ins
+00007a70: 702e 6765 745f 666f 7265 6967 6e5f 6b65  p.get_foreign_ke
+00007a80: 7973 2873 656c 662e 7461 626c 6573 2e74  ys(self.tables.t
+00007a90: 6232 2e6e 616d 6529 0a20 2020 2020 2020  b2.name).       
+00007aa0: 2065 715f 286c 656e 2866 6f72 6569 676e   eq_(len(foreign
+00007ab0: 5f6b 6579 7329 2c20 3129 0a20 2020 2020  _keys), 1).     
+00007ac0: 2020 2066 6b65 7931 203d 2066 6f72 6569     fkey1 = forei
+00007ad0: 676e 5f6b 6579 735b 305d 0a20 2020 2020  gn_keys[0].     
+00007ae0: 2020 2065 715f 2873 6574 2866 6b65 7931     eq_(set(fkey1
+00007af0: 2e67 6574 2822 7265 6665 7272 6564 5f63  .get("referred_c
+00007b00: 6f6c 756d 6e73 2229 292c 207b 226e 616d  olumns")), {"nam
+00007b10: 6522 2c20 2269 6422 2c20 2261 7474 7222  e", "id", "attr"
+00007b20: 7d29 0a20 2020 2020 2020 2065 715f 2873  }).        eq_(s
+00007b30: 6574 2866 6b65 7931 2e67 6574 2822 636f  et(fkey1.get("co
+00007b40: 6e73 7472 6169 6e65 645f 636f 6c75 6d6e  nstrained_column
+00007b50: 7322 2929 2c20 7b22 706e 616d 6522 2c20  s")), {"pname", 
+00007b60: 2270 6964 222c 2022 7061 7474 7222 7d29  "pid", "pattr"})
+00007b70: 0a0a 2020 2020 4074 6573 7469 6e67 2e72  ..    @testing.r
+00007b80: 6571 7569 7265 732e 7072 696d 6172 795f  equires.primary_
+00007b90: 6b65 795f 636f 6e73 7472 6169 6e74 5f72  key_constraint_r
+00007ba0: 6566 6c65 6374 696f 6e0a 2020 2020 6465  eflection.    de
+00007bb0: 6620 7465 7374 5f70 6b5f 636f 6c75 6d6e  f test_pk_column
+00007bc0: 5f6f 7264 6572 2873 656c 662c 2063 6f6e  _order(self, con
+00007bd0: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
+00007be0: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
+00007bf0: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
+00007c00: 2020 2020 2020 2020 456d 756c 746f 7220          Emultor 
+00007c10: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
+00007c20: 7265 7475 726e 696e 6720 706b 2073 6f72  returning pk sor
+00007c30: 7465 6420 6279 206f 7264 696e 616c 2076  ted by ordinal v
+00007c40: 616c 7565 0a20 2020 2020 2020 206f 6620  alue.        of 
+00007c50: 636f 6c75 6d6e 732e 0a20 2020 2020 2020  columns..       
+00007c60: 2022 2222 0a20 2020 2020 2020 2069 6e73   """.        ins
+00007c70: 7020 3d20 696e 7370 6563 7428 636f 6e6e  p = inspect(conn
+00007c80: 6563 7469 6f6e 290a 2020 2020 2020 2020  ection).        
+00007c90: 7072 696d 6172 795f 6b65 7920 3d20 696e  primary_key = in
+00007ca0: 7370 2e67 6574 5f70 6b5f 636f 6e73 7472  sp.get_pk_constr
+00007cb0: 6169 6e74 2873 656c 662e 7461 626c 6573  aint(self.tables
+00007cc0: 2e74 6231 2e6e 616d 6529 0a20 2020 2020  .tb1.name).     
+00007cd0: 2020 2065 7870 203d 2028 0a20 2020 2020     exp = (.     
+00007ce0: 2020 2020 2020 205b 2269 6422 2c20 226e         ["id", "n
+00007cf0: 616d 6522 2c20 2261 7474 7222 5d0a 2020  ame", "attr"].  
+00007d00: 2020 2020 2020 2020 2020 6966 2062 6f6f            if boo
+00007d10: 6c28 6f73 2e65 6e76 6972 6f6e 2e67 6574  l(os.environ.get
+00007d20: 2822 5350 414e 4e45 525f 454d 554c 4154  ("SPANNER_EMULAT
+00007d30: 4f52 5f48 4f53 5422 2929 0a20 2020 2020  OR_HOST")).     
+00007d40: 2020 2020 2020 2065 6c73 6520 5b22 6e61         else ["na
+00007d50: 6d65 222c 2022 6964 222c 2022 6174 7472  me", "id", "attr
+00007d60: 225d 0a20 2020 2020 2020 2029 0a20 2020  "].        ).   
+00007d70: 2020 2020 2065 715f 2870 7269 6d61 7279       eq_(primary
+00007d80: 5f6b 6579 2e67 6574 2822 636f 6e73 7472  _key.get("constr
+00007d90: 6169 6e65 645f 636f 6c75 6d6e 7322 292c  ained_columns"),
+00007da0: 2065 7870 290a 0a0a 4070 7974 6573 742e   exp)...@pytest.
+00007db0: 6d61 726b 2e73 6b69 7028 2253 7061 6e6e  mark.skip("Spann
+00007dc0: 6572 2064 6f65 736e 2774 2073 7570 706f  er doesn't suppo
+00007dd0: 7274 2071 756f 7465 7320 696e 2074 6162  rt quotes in tab
+00007de0: 6c65 206e 616d 6573 2e22 290a 636c 6173  le names.").clas
+00007df0: 7320 5175 6f74 6564 4e61 6d65 4172 6775  s QuotedNameArgu
+00007e00: 6d65 6e74 5465 7374 285f 5175 6f74 6564  mentTest(_Quoted
+00007e10: 4e61 6d65 4172 6775 6d65 6e74 5465 7374  NameArgumentTest
+00007e20: 293a 0a20 2020 2070 6173 730a 0a0a 636c  ):.    pass...cl
+00007e30: 6173 7320 5f44 6174 6546 6978 7475 7265  ass _DateFixture
+00007e40: 285f 5f44 6174 6546 6978 7475 7265 293a  (__DateFixture):
+00007e50: 0a20 2020 2063 6f6d 7061 7265 203d 204e  .    compare = N
+00007e60: 6f6e 650a 0a20 2020 2040 636c 6173 736d  one..    @classm
+00007e70: 6574 686f 640a 2020 2020 6465 6620 6465  ethod.    def de
+00007e80: 6669 6e65 5f74 6162 6c65 7328 636c 732c  fine_tables(cls,
+00007e90: 206d 6574 6164 6174 6129 3a0a 2020 2020   metadata):.    
+00007ea0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00007eb0: 5350 414e 4e45 5220 4f56 4552 5249 4445  SPANNER OVERRIDE
+00007ec0: 3a0a 0a20 2020 2020 2020 2043 6c6f 7564  :..        Cloud
+00007ed0: 2053 7061 6e6e 6572 2064 6f65 736e 2774   Spanner doesn't
+00007ee0: 2073 7570 706f 7274 2061 7574 6f20 696e   support auto in
+00007ef0: 6372 656d 656e 7469 6e67 2069 6473 2066  crementing ids f
+00007f00: 6561 7475 7265 2c0a 2020 2020 2020 2020  eature,.        
+00007f10: 7768 6963 6820 6973 2075 7365 6420 6279  which is used by
+00007f20: 2074 6865 206f 7269 6769 6e61 6c20 7465   the original te
+00007f30: 7374 2e20 4f76 6572 7269 6469 6e67 2074  st. Overriding t
+00007f40: 6865 2074 6573 7420 6461 7461 0a20 2020  he test data.   
+00007f50: 2020 2020 2063 7265 6174 696f 6e20 6d65       creation me
+00007f60: 7468 6f64 2074 6f20 6469 7361 626c 6520  thod to disable 
+00007f70: 6175 746f 696e 6372 656d 656e 7420 616e  autoincrement an
+00007f80: 6420 6d61 6b65 2069 6420 636f 6c75 6d6e  d make id column
+00007f90: 0a20 2020 2020 2020 206e 756c 6c61 626c  .        nullabl
+00007fa0: 652e 0a20 2020 2020 2020 2022 2222 0a0a  e..        """..
+00007fb0: 2020 2020 2020 2020 636c 6173 7320 4465          class De
+00007fc0: 636f 7261 7465 6428 7371 6c61 6c63 6865  corated(sqlalche
+00007fd0: 6d79 2e54 7970 6544 6563 6f72 6174 6f72  my.TypeDecorator
+00007fe0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00007ff0: 6d70 6c20 3d20 636c 732e 6461 7461 7479  mpl = cls.dataty
+00008000: 7065 0a20 2020 2020 2020 2020 2020 2063  pe.            c
+00008010: 6163 6865 5f6f 6b20 3d20 5472 7565 0a0a  ache_ok = True..
+00008020: 2020 2020 2020 2020 5461 626c 6528 0a20          Table(. 
+00008030: 2020 2020 2020 2020 2020 2022 6461 7465             "date
+00008040: 5f74 6162 6c65 222c 0a20 2020 2020 2020  _table",.       
+00008050: 2020 2020 206d 6574 6164 6174 612c 0a20       metadata,. 
+00008060: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00008070: 6e28 2269 6422 2c20 496e 7465 6765 722c  n("id", Integer,
+00008080: 2070 7269 6d61 7279 5f6b 6579 3d54 7275   primary_key=Tru
+00008090: 652c 206e 756c 6c61 626c 653d 5472 7565  e, nullable=True
+000080a0: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
+000080b0: 6f6c 756d 6e28 2264 6174 655f 6461 7461  olumn("date_data
+000080c0: 222c 2063 6c73 2e64 6174 6174 7970 6529  ", cls.datatype)
+000080d0: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
+000080e0: 6c75 6d6e 2822 6465 636f 7261 7465 645f  lumn("decorated_
+000080f0: 6461 7465 5f64 6174 6122 2c20 4465 636f  date_data", Deco
+00008100: 7261 7465 6429 2c0a 2020 2020 2020 2020  rated),.        
+00008110: 290a 0a0a 636c 6173 7320 4461 7465 5465  )...class DateTe
+00008120: 7374 285f 4461 7465 5465 7374 293a 0a20  st(_DateTest):. 
+00008130: 2020 2022 2222 0a20 2020 2053 5041 4e4e     """.    SPANN
+00008140: 4552 204f 5645 5252 4944 453a 0a0a 2020  ER OVERRIDE:..  
+00008150: 2020 4461 7465 5465 7374 2074 6573 7473    DateTest tests
+00008160: 2075 7365 6420 7361 6d65 2063 6c61 7373   used same class
+00008170: 206d 6574 686f 6420 746f 2063 7265 6174   method to creat
+00008180: 6520 7461 626c 652c 2073 6f20 746f 2061  e table, so to a
+00008190: 766f 6964 2074 686f 7365 2066 6169 6c75  void those failu
+000081a0: 7265 730a 2020 2020 616e 6420 6d61 696e  res.    and main
+000081b0: 7461 696e 2044 5259 2063 6f6e 6365 7074  tain DRY concept
+000081c0: 206a 7573 7420 696e 6865 7269 7420 7468   just inherit th
+000081d0: 6520 636c 6173 7320 746f 2072 756e 2074  e class to run t
+000081e0: 6573 7473 2073 7563 6365 7373 6675 6c6c  ests successfull
+000081f0: 792e 0a20 2020 2022 2222 0a0a 2020 2020  y..    """..    
+00008200: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+00008210: 7069 6628 0a20 2020 2020 2020 2062 6f6f  pif(.        boo
+00008220: 6c28 6f73 2e65 6e76 6972 6f6e 2e67 6574  l(os.environ.get
+00008230: 2822 5350 414e 4e45 525f 454d 554c 4154  ("SPANNER_EMULAT
+00008240: 4f52 5f48 4f53 5422 2929 2c20 7265 6173  OR_HOST")), reas
+00008250: 6f6e 3d22 536b 6970 7065 6420 6f6e 2065  on="Skipped on e
+00008260: 6d75 6c61 746f 7222 0a20 2020 2029 0a20  mulator".    ). 
+00008270: 2020 2064 6566 2074 6573 745f 6e75 6c6c     def test_null
+00008280: 5f62 6f75 6e64 5f63 6f6d 7061 7269 736f  _bound_compariso
+00008290: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
+000082a0: 2073 7570 6572 2829 2e74 6573 745f 6e75   super().test_nu
+000082b0: 6c6c 5f62 6f75 6e64 5f63 6f6d 7061 7269  ll_bound_compari
+000082c0: 736f 6e28 290a 0a20 2020 2040 7079 7465  son()..    @pyte
+000082d0: 7374 2e6d 6172 6b2e 736b 6970 6966 280a  st.mark.skipif(.
+000082e0: 2020 2020 2020 2020 626f 6f6c 286f 732e          bool(os.
+000082f0: 656e 7669 726f 6e2e 6765 7428 2253 5041  environ.get("SPA
+00008300: 4e4e 4552 5f45 4d55 4c41 544f 525f 484f  NNER_EMULATOR_HO
+00008310: 5354 2229 292c 2072 6561 736f 6e3d 2253  ST")), reason="S
+00008320: 6b69 7070 6564 206f 6e20 656d 756c 6174  kipped on emulat
+00008330: 6f72 220a 2020 2020 290a 2020 2020 6465  or".    ).    de
+00008340: 6620 7465 7374 5f6e 756c 6c28 7365 6c66  f test_null(self
+00008350: 2c20 636f 6e6e 6563 7469 6f6e 293a 0a20  , connection):. 
+00008360: 2020 2020 2020 2073 7570 6572 2829 2e74         super().t
+00008370: 6573 745f 6e75 6c6c 2863 6f6e 6e65 6374  est_null(connect
+00008380: 696f 6e29 0a0a 0a63 6c61 7373 2043 5445  ion)...class CTE
+00008390: 5465 7374 285f 4354 4554 6573 7429 3a0a  Test(_CTETest):.
+000083a0: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+000083b0: 0a20 2020 2064 6566 2064 6566 696e 655f  .    def define_
+000083c0: 7461 626c 6573 2863 6c73 2c20 6d65 7461  tables(cls, meta
+000083d0: 6461 7461 293a 0a20 2020 2020 2020 2022  data):.        "
+000083e0: 2222 0a20 2020 2020 2020 2054 6865 206f  "".        The o
+000083f0: 7269 6769 6e61 6c20 6d65 7468 6f64 2063  riginal method c
+00008400: 7265 6174 6573 2061 2066 6f72 6569 676e  reates a foreign
+00008410: 206b 6579 2077 6974 686f 7574 2061 206e   key without a n
+00008420: 616d 652c 0a20 2020 2020 2020 2077 6869  ame,.        whi
+00008430: 6368 2063 6175 7365 7320 7472 6f75 626c  ch causes troubl
+00008440: 6573 206f 6e20 7465 7374 2063 6c65 616e  es on test clean
+00008450: 7570 2e20 4f76 6572 7269 6469 6e67 2074  up. Overriding t
+00008460: 6865 0a20 2020 2020 2020 206d 6574 686f  he.        metho
+00008470: 6420 746f 2065 7870 6c69 6369 746c 7920  d to explicitly 
+00008480: 7365 7420 6120 666f 7265 6967 6e20 6b65  set a foreign ke
+00008490: 7920 6e61 6d65 2e0a 2020 2020 2020 2020  y name..        
+000084a0: 2222 220a 2020 2020 2020 2020 5461 626c  """.        Tabl
+000084b0: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
+000084c0: 736f 6d65 5f74 6162 6c65 222c 0a20 2020  some_table",.   
+000084d0: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+000084e0: 612c 0a20 2020 2020 2020 2020 2020 2043  a,.            C
+000084f0: 6f6c 756d 6e28 2269 6422 2c20 496e 7465  olumn("id", Inte
+00008500: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
+00008510: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
+00008520: 2020 2020 436f 6c75 6d6e 2822 6461 7461      Column("data
+00008530: 222c 2053 7472 696e 6728 3530 2929 2c0a  ", String(50)),.
+00008540: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
+00008550: 6d6e 2822 7061 7265 6e74 5f69 6422 2c20  mn("parent_id", 
+00008560: 466f 7265 6967 6e4b 6579 2822 736f 6d65  ForeignKey("some
+00008570: 5f74 6162 6c65 2e69 6422 2c20 6e61 6d65  _table.id", name
+00008580: 3d22 666b 5f73 6f6d 655f 7461 626c 6522  ="fk_some_table"
+00008590: 2929 2c0a 2020 2020 2020 2020 290a 0a20  )),.        ).. 
+000085a0: 2020 2020 2020 2054 6162 6c65 280a 2020         Table(.  
+000085b0: 2020 2020 2020 2020 2020 2273 6f6d 655f            "some_
+000085c0: 6f74 6865 725f 7461 626c 6522 2c0a 2020  other_table",.  
+000085d0: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
+000085e0: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+000085f0: 436f 6c75 6d6e 2822 6964 222c 2049 6e74  Column("id", Int
+00008600: 6567 6572 2c20 7072 696d 6172 795f 6b65  eger, primary_ke
+00008610: 793d 5472 7565 292c 0a20 2020 2020 2020  y=True),.       
+00008620: 2020 2020 2043 6f6c 756d 6e28 2264 6174       Column("dat
+00008630: 6122 2c20 5374 7269 6e67 2835 3029 292c  a", String(50)),
+00008640: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
+00008650: 756d 6e28 2270 6172 656e 745f 6964 222c  umn("parent_id",
+00008660: 2049 6e74 6567 6572 292c 0a20 2020 2020   Integer),.     
+00008670: 2020 2029 0a0a 2020 2020 4070 7974 6573     )..    @pytes
+00008680: 742e 6d61 726b 2e73 6b69 7028 2249 4e53  t.mark.skip("INS
+00008690: 4552 5420 6672 6f6d 2057 4954 4820 7375  ERT from WITH su
+000086a0: 6271 7565 7279 2069 7320 6e6f 7420 7375  bquery is not su
+000086b0: 7070 6f72 7465 6422 290a 2020 2020 6465  pported").    de
+000086c0: 6620 7465 7374 5f69 6e73 6572 745f 6672  f test_insert_fr
+000086d0: 6f6d 5f73 656c 6563 745f 726f 756e 645f  om_select_round_
+000086e0: 7472 6970 2873 656c 6629 3a0a 2020 2020  trip(self):.    
+000086f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00008700: 5468 6520 7465 7374 2063 6865 636b 7320  The test checks 
+00008710: 6966 2061 6e20 494e 5345 5254 2063 616e  if an INSERT can
+00008720: 2062 6520 646f 6e65 2066 726f 6d20 6120   be done from a 
+00008730: 6374 652c 206c 696b 653a 0a0a 2020 2020  cte, like:..    
+00008740: 2020 2020 5749 5448 2073 6f6d 655f 6374      WITH some_ct
+00008750: 6520 4153 2028 2e2e 2e29 0a20 2020 2020  e AS (...).     
+00008760: 2020 2049 4e53 4552 5420 494e 544f 2073     INSERT INTO s
+00008770: 6f6d 655f 6f74 6865 725f 7461 626c 6520  ome_other_table 
+00008780: 282e 2e2e 2053 454c 4543 5420 2a20 4652  (... SELECT * FR
+00008790: 4f4d 2073 6f6d 655f 6374 6529 0a0a 2020  OM some_cte)..  
+000087a0: 2020 2020 2020 5375 6368 2071 7565 7269        Such queri
+000087b0: 6573 2061 7265 206e 6f74 2073 7570 706f  es are not suppo
+000087c0: 7274 6564 2062 7920 5370 616e 6e65 722e  rted by Spanner.
+000087d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000087e0: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
+000087f0: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
+00008800: 2822 4445 4c45 5445 2066 726f 6d20 5749  ("DELETE from WI
+00008810: 5448 2073 7562 7175 6572 7920 6973 206e  TH subquery is n
+00008820: 6f74 2073 7570 706f 7274 6564 2229 0a20  ot supported"). 
+00008830: 2020 2064 6566 2074 6573 745f 6465 6c65     def test_dele
+00008840: 7465 5f73 6361 6c61 725f 7375 6271 5f72  te_scalar_subq_r
+00008850: 6f75 6e64 5f74 7269 7028 7365 6c66 293a  ound_trip(self):
+00008860: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00008870: 2020 2020 2054 6865 2074 6573 7420 6368       The test ch
+00008880: 6563 6b73 2069 6620 6120 4445 4c45 5445  ecks if a DELETE
+00008890: 2063 616e 2062 6520 646f 6e65 2066 726f   can be done fro
+000088a0: 6d20 6120 6374 652c 206c 696b 653a 0a0a  m a cte, like:..
+000088b0: 2020 2020 2020 2020 5749 5448 2073 6f6d          WITH som
+000088c0: 655f 6374 6520 4153 2028 2e2e 2e29 0a20  e_cte AS (...). 
+000088d0: 2020 2020 2020 2044 454c 4554 4520 4652         DELETE FR
+000088e0: 4f4d 2073 6f6d 655f 6f74 6865 725f 7461  OM some_other_ta
+000088f0: 626c 6520 282e 2e2e 2053 454c 4543 5420  ble (... SELECT 
+00008900: 2a20 4652 4f4d 2073 6f6d 655f 6374 6529  * FROM some_cte)
+00008910: 0a0a 2020 2020 2020 2020 5375 6368 2071  ..        Such q
+00008920: 7565 7269 6573 2061 7265 206e 6f74 2073  ueries are not s
+00008930: 7570 706f 7274 6564 2062 7920 5370 616e  upported by Span
+00008940: 6e65 722e 0a20 2020 2020 2020 2022 2222  ner..        """
+00008950: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00008960: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+00008970: 736b 6970 2822 4445 4c45 5445 2066 726f  skip("DELETE fro
+00008980: 6d20 5749 5448 2073 7562 7175 6572 7920  m WITH subquery 
+00008990: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
+000089a0: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
+000089b0: 6465 6c65 7465 5f66 726f 6d5f 726f 756e  delete_from_roun
+000089c0: 645f 7472 6970 2873 656c 6629 3a0a 2020  d_trip(self):.  
+000089d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000089e0: 2020 5468 6520 7465 7374 2063 6865 636b    The test check
+000089f0: 7320 6966 2061 2044 454c 4554 4520 6361  s if a DELETE ca
+00008a00: 6e20 6265 2064 6f6e 6520 6672 6f6d 2061  n be done from a
+00008a10: 2063 7465 2c20 6c69 6b65 3a0a 0a20 2020   cte, like:..   
+00008a20: 2020 2020 2057 4954 4820 736f 6d65 5f63       WITH some_c
+00008a30: 7465 2041 5320 282e 2e2e 290a 2020 2020  te AS (...).    
+00008a40: 2020 2020 4445 4c45 5445 2046 524f 4d20      DELETE FROM 
+00008a50: 736f 6d65 5f6f 7468 6572 5f74 6162 6c65  some_other_table
+00008a60: 2028 2e2e 2e20 5345 4c45 4354 202a 2046   (... SELECT * F
+00008a70: 524f 4d20 736f 6d65 5f63 7465 290a 0a20  ROM some_cte).. 
+00008a80: 2020 2020 2020 2053 7563 6820 7175 6572         Such quer
+00008a90: 6965 7320 6172 6520 6e6f 7420 7375 7070  ies are not supp
+00008aa0: 6f72 7465 6420 6279 2053 7061 6e6e 6572  orted by Spanner
+00008ab0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00008ac0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00008ad0: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+00008ae0: 7028 2255 5044 4154 4520 6672 6f6d 2057  p("UPDATE from W
+00008af0: 4954 4820 7375 6271 7565 7279 2069 7320  ITH subquery is 
+00008b00: 6e6f 7420 7375 7070 6f72 7465 6422 290a  not supported").
+00008b10: 2020 2020 6465 6620 7465 7374 5f75 7064      def test_upd
+00008b20: 6174 655f 6672 6f6d 5f72 6f75 6e64 5f74  ate_from_round_t
+00008b30: 7269 7028 7365 6c66 293a 0a20 2020 2020  rip(self):.     
+00008b40: 2020 2022 2222 0a20 2020 2020 2020 2054     """.        T
+00008b50: 6865 2074 6573 7420 6368 6563 6b73 2069  he test checks i
+00008b60: 6620 616e 2055 5044 4154 4520 6361 6e20  f an UPDATE can 
+00008b70: 6265 2064 6f6e 6520 6672 6f6d 2061 2063  be done from a c
+00008b80: 7465 2c20 6c69 6b65 3a0a 0a20 2020 2020  te, like:..     
+00008b90: 2020 2057 4954 4820 736f 6d65 5f63 7465     WITH some_cte
+00008ba0: 2041 5320 282e 2e2e 290a 2020 2020 2020   AS (...).      
+00008bb0: 2020 5550 4441 5445 2073 6f6d 655f 6f74    UPDATE some_ot
+00008bc0: 6865 725f 7461 626c 650a 2020 2020 2020  her_table.      
+00008bd0: 2020 5345 5420 282e 2e2e 2053 454c 4543    SET (... SELEC
+00008be0: 5420 2a20 4652 4f4d 2073 6f6d 655f 6374  T * FROM some_ct
+00008bf0: 6529 0a0a 2020 2020 2020 2020 5375 6368  e)..        Such
+00008c00: 2071 7565 7269 6573 2061 7265 206e 6f74   queries are not
+00008c10: 2073 7570 706f 7274 6564 2062 7920 5370   supported by Sp
+00008c20: 616e 6e65 722e 0a20 2020 2020 2020 2022  anner..        "
+00008c30: 2222 0a20 2020 2020 2020 2070 6173 730a  "".        pass.
+00008c40: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+00008c50: 6b2e 736b 6970 2822 5749 5448 2052 4543  k.skip("WITH REC
+00008c60: 5552 5349 5645 2073 7562 7175 6572 6965  URSIVE subquerie
+00008c70: 7320 6172 6520 6e6f 7420 7375 7070 6f72  s are not suppor
+00008c80: 7465 6422 290a 2020 2020 6465 6620 7465  ted").    def te
+00008c90: 7374 5f73 656c 6563 745f 7265 6375 7273  st_select_recurs
+00008ca0: 6976 655f 726f 756e 645f 7472 6970 2873  ive_round_trip(s
+00008cb0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+00008cc0: 7373 0a0a 0a63 6c61 7373 2044 6174 6554  ss...class DateT
+00008cd0: 696d 654d 6963 726f 7365 636f 6e64 7354  imeMicrosecondsT
+00008ce0: 6573 7428 5f44 6174 6554 696d 654d 6963  est(_DateTimeMic
+00008cf0: 726f 7365 636f 6e64 7354 6573 742c 2044  rosecondsTest, D
+00008d00: 6174 6554 6573 7429 3a0a 2020 2020 4070  ateTest):.    @p
+00008d10: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+00008d20: 2253 7061 6e6e 6572 2064 6174 6573 2061  "Spanner dates a
+00008d30: 7265 2074 696d 6520 7a6f 6e65 2069 6e64  re time zone ind
+00008d40: 6570 656e 6465 6e74 2229 0a20 2020 2064  ependent").    d
+00008d50: 6566 2074 6573 745f 7365 6c65 6374 5f64  ef test_select_d
+00008d60: 6972 6563 7428 7365 6c66 293a 0a20 2020  irect(self):.   
+00008d70: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00008d80: 6566 2074 6573 745f 726f 756e 645f 7472  ef test_round_tr
+00008d90: 6970 2873 656c 6629 3a0a 2020 2020 2020  ip(self):.      
+00008da0: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
+00008db0: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
+00008dc0: 0a20 2020 2020 2020 2053 7061 6e6e 6572  .        Spanner
+00008dd0: 2063 6f6e 7665 7274 7320 7469 6d65 7374   converts timest
+00008de0: 616d 7020 696e 746f 2060 2559 2d25 6d2d  amp into `%Y-%m-
+00008df0: 2564 5425 483a 254d 3a25 532e 2566 5a60  %dT%H:%M:%S.%fZ`
+00008e00: 2066 6f72 6d61 742c 2073 6f20 746f 2061   format, so to a
+00008e10: 766f 6964 0a20 2020 2020 2020 2061 7373  void.        ass
+00008e20: 6572 7420 6661 696c 7572 6573 2063 6f6e  ert failures con
+00008e30: 7665 7274 2064 6174 6574 696d 6520 696e  vert datetime in
+00008e40: 7075 7420 746f 2074 6865 2064 6573 6972  put to the desir
+00008e50: 6520 7469 6d65 7374 616d 7020 666f 726d  e timestamp form
+00008e60: 6174 2e0a 2020 2020 2020 2020 2222 220a  at..        """.
+00008e70: 2020 2020 2020 2020 6461 7465 5f74 6162          date_tab
+00008e80: 6c65 203d 2073 656c 662e 7461 626c 6573  le = self.tables
+00008e90: 2e64 6174 655f 7461 626c 650a 2020 2020  .date_table.    
+00008ea0: 2020 2020 636f 6e66 6967 2e64 622e 6578      config.db.ex
+00008eb0: 6563 7574 6528 6461 7465 5f74 6162 6c65  ecute(date_table
+00008ec0: 2e69 6e73 6572 7428 292c 207b 2264 6174  .insert(), {"dat
+00008ed0: 655f 6461 7461 223a 2073 656c 662e 6461  e_data": self.da
+00008ee0: 7461 2c20 2269 6422 3a20 3235 307d 290a  ta, "id": 250}).
+00008ef0: 0a20 2020 2020 2020 2072 6f77 203d 2063  .        row = c
+00008f00: 6f6e 6669 672e 6462 2e65 7865 6375 7465  onfig.db.execute
+00008f10: 2873 656c 6563 7428 5b64 6174 655f 7461  (select([date_ta
+00008f20: 626c 652e 632e 6461 7465 5f64 6174 615d  ble.c.date_data]
+00008f30: 2929 2e66 6972 7374 2829 0a20 2020 2020  )).first().     
+00008f40: 2020 2063 6f6d 7061 7265 203d 2073 656c     compare = sel
+00008f50: 662e 636f 6d70 6172 6520 6f72 2073 656c  f.compare or sel
+00008f60: 662e 6461 7461 0a20 2020 2020 2020 2063  f.data.        c
+00008f70: 6f6d 7061 7265 203d 2063 6f6d 7061 7265  ompare = compare
+00008f80: 2e73 7472 6674 696d 6528 2225 592d 256d  .strftime("%Y-%m
+00008f90: 2d25 6454 2548 3a25 4d3a 2553 2e25 665a  -%dT%H:%M:%S.%fZ
+00008fa0: 2229 0a20 2020 2020 2020 2065 715f 2872  ").        eq_(r
+00008fb0: 6f77 5b30 5d2e 7266 6333 3333 3928 292c  ow[0].rfc3339(),
+00008fc0: 2063 6f6d 7061 7265 290a 2020 2020 2020   compare).      
+00008fd0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+00008fe0: 6e63 6528 726f 775b 305d 2c20 4461 7465  nce(row[0], Date
+00008ff0: 7469 6d65 5769 7468 4e61 6e6f 7365 636f  timeWithNanoseco
+00009000: 6e64 7329 0a0a 2020 2020 6465 6620 7465  nds)..    def te
+00009010: 7374 5f72 6f75 6e64 5f74 7269 705f 6465  st_round_trip_de
+00009020: 636f 7261 7465 6428 7365 6c66 2c20 636f  corated(self, co
+00009030: 6e6e 6563 7469 6f6e 293a 0a20 2020 2020  nnection):.     
+00009040: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+00009050: 5041 4e4e 4552 204f 5645 5252 4944 453a  PANNER OVERRIDE:
+00009060: 0a0a 2020 2020 2020 2020 5370 616e 6e65  ..        Spanne
+00009070: 7220 636f 6e76 6572 7473 2074 696d 6573  r converts times
+00009080: 7461 6d70 2069 6e74 6f20 6025 592d 256d  tamp into `%Y-%m
+00009090: 2d25 6454 2548 3a25 4d3a 2553 2e25 665a  -%dT%H:%M:%S.%fZ
+000090a0: 6020 666f 726d 6174 2c20 736f 2074 6f20  ` format, so to 
+000090b0: 6176 6f69 640a 2020 2020 2020 2020 6173  avoid.        as
+000090c0: 7365 7274 2066 6169 6c75 7265 7320 636f  sert failures co
+000090d0: 6e76 6572 7420 6461 7465 7469 6d65 2069  nvert datetime i
+000090e0: 6e70 7574 2074 6f20 7468 6520 6465 7369  nput to the desi
+000090f0: 7265 2074 696d 6573 7461 6d70 2066 6f72  re timestamp for
+00009100: 6d61 742e 0a20 2020 2020 2020 2022 2222  mat..        """
+00009110: 0a20 2020 2020 2020 2064 6174 655f 7461  .        date_ta
+00009120: 626c 6520 3d20 7365 6c66 2e74 6162 6c65  ble = self.table
+00009130: 732e 6461 7465 5f74 6162 6c65 0a0a 2020  s.date_table..  
+00009140: 2020 2020 2020 636f 6e6e 6563 7469 6f6e        connection
+00009150: 2e65 7865 6375 7465 280a 2020 2020 2020  .execute(.      
+00009160: 2020 2020 2020 6461 7465 5f74 6162 6c65        date_table
+00009170: 2e69 6e73 6572 7428 292c 207b 2269 6422  .insert(), {"id"
+00009180: 3a20 312c 2022 6465 636f 7261 7465 645f  : 1, "decorated_
+00009190: 6461 7465 5f64 6174 6122 3a20 7365 6c66  date_data": self
+000091a0: 2e64 6174 617d 0a20 2020 2020 2020 2029  .data}.        )
+000091b0: 0a0a 2020 2020 2020 2020 726f 7720 3d20  ..        row = 
+000091c0: 636f 6e6e 6563 7469 6f6e 2e65 7865 6375  connection.execu
+000091d0: 7465 2873 656c 6563 7428 6461 7465 5f74  te(select(date_t
+000091e0: 6162 6c65 2e63 2e64 6563 6f72 6174 6564  able.c.decorated
+000091f0: 5f64 6174 655f 6461 7461 2929 2e66 6972  _date_data)).fir
+00009200: 7374 2829 0a0a 2020 2020 2020 2020 636f  st()..        co
+00009210: 6d70 6172 6520 3d20 7365 6c66 2e63 6f6d  mpare = self.com
+00009220: 7061 7265 206f 7220 7365 6c66 2e64 6174  pare or self.dat
+00009230: 610a 2020 2020 2020 2020 636f 6d70 6172  a.        compar
+00009240: 6520 3d20 636f 6d70 6172 652e 7374 7266  e = compare.strf
+00009250: 7469 6d65 2822 2559 2d25 6d2d 2564 5425  time("%Y-%m-%dT%
+00009260: 483a 254d 3a25 532e 2566 5a22 290a 2020  H:%M:%S.%fZ").  
+00009270: 2020 2020 2020 6571 5f28 726f 775b 305d        eq_(row[0]
+00009280: 2e72 6663 3333 3339 2829 2c20 636f 6d70  .rfc3339(), comp
+00009290: 6172 6529 0a20 2020 2020 2020 2061 7373  are).        ass
+000092a0: 6572 7420 6973 696e 7374 616e 6365 2872  ert isinstance(r
+000092b0: 6f77 5b30 5d2c 2044 6174 6574 696d 6557  ow[0], DatetimeW
+000092c0: 6974 684e 616e 6f73 6563 6f6e 6473 290a  ithNanoseconds).
+000092d0: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+000092e0: 6b2e 736b 6970 6966 280a 2020 2020 2020  k.skipif(.      
+000092f0: 2020 626f 6f6c 286f 732e 656e 7669 726f    bool(os.enviro
+00009300: 6e2e 6765 7428 2253 5041 4e4e 4552 5f45  n.get("SPANNER_E
+00009310: 4d55 4c41 544f 525f 484f 5354 2229 292c  MULATOR_HOST")),
+00009320: 2072 6561 736f 6e3d 2253 6b69 7070 6564   reason="Skipped
+00009330: 206f 6e20 656d 756c 6174 6f72 220a 2020   on emulator".  
+00009340: 2020 290a 2020 2020 6465 6620 7465 7374    ).    def test
+00009350: 5f6e 756c 6c5f 626f 756e 645f 636f 6d70  _null_bound_comp
+00009360: 6172 6973 6f6e 2873 656c 6629 3a0a 2020  arison(self):.  
+00009370: 2020 2020 2020 7375 7065 7228 292e 7465        super().te
+00009380: 7374 5f6e 756c 6c5f 626f 756e 645f 636f  st_null_bound_co
+00009390: 6d70 6172 6973 6f6e 2829 0a0a 2020 2020  mparison()..    
+000093a0: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+000093b0: 7069 6628 0a20 2020 2020 2020 2062 6f6f  pif(.        boo
+000093c0: 6c28 6f73 2e65 6e76 6972 6f6e 2e67 6574  l(os.environ.get
+000093d0: 2822 5350 414e 4e45 525f 454d 554c 4154  ("SPANNER_EMULAT
+000093e0: 4f52 5f48 4f53 5422 2929 2c20 7265 6173  OR_HOST")), reas
+000093f0: 6f6e 3d22 536b 6970 7065 6420 6f6e 2065  on="Skipped on e
+00009400: 6d75 6c61 746f 7222 0a20 2020 2029 0a20  mulator".    ). 
+00009410: 2020 2064 6566 2074 6573 745f 6e75 6c6c     def test_null
+00009420: 2873 656c 662c 2063 6f6e 6e65 6374 696f  (self, connectio
+00009430: 6e29 3a0a 2020 2020 2020 2020 7375 7065  n):.        supe
+00009440: 7228 292e 7465 7374 5f6e 756c 6c28 636f  r().test_null(co
+00009450: 6e6e 6563 7469 6f6e 290a 0a0a 636c 6173  nnection)...clas
+00009460: 7320 4461 7465 5469 6d65 5465 7374 285f  s DateTimeTest(_
+00009470: 4461 7465 5469 6d65 5465 7374 2c20 4461  DateTimeTest, Da
+00009480: 7465 5469 6d65 4d69 6372 6f73 6563 6f6e  teTimeMicrosecon
+00009490: 6473 5465 7374 293a 0a20 2020 2022 2222  dsTest):.    """
+000094a0: 0a20 2020 2053 5041 4e4e 4552 204f 5645  .    SPANNER OVE
+000094b0: 5252 4944 453a 0a0a 2020 2020 4461 7465  RRIDE:..    Date
+000094c0: 5469 6d65 5465 7374 2074 6573 7473 2068  TimeTest tests h
+000094d0: 6176 6520 7468 6520 7361 6d65 2066 6169  ave the same fai
+000094e0: 6c75 7265 7320 7361 6d65 2061 7320 4461  lures same as Da
+000094f0: 7465 5469 6d65 4d69 6372 6f73 6563 6f6e  teTimeMicrosecon
+00009500: 6473 5465 7374 2074 6573 7473 2c0a 2020  dsTest tests,.  
+00009510: 2020 736f 2074 6f20 6176 6f69 6420 7468    so to avoid th
+00009520: 6f73 6520 6661 696c 7572 6573 2061 6e64  ose failures and
+00009530: 206d 6169 6e74 6169 6e20 4452 5920 636f   maintain DRY co
+00009540: 6e63 6570 7420 6a75 7374 2069 6e68 6572  ncept just inher
+00009550: 6974 2074 6865 2063 6c61 7373 2074 6f20  it the class to 
+00009560: 7275 6e0a 2020 2020 7465 7374 7320 7375  run.    tests su
+00009570: 6363 6573 7366 756c 6c79 2e0a 2020 2020  ccessfully..    
+00009580: 2222 220a 0a20 2020 2040 7079 7465 7374  """..    @pytest
+00009590: 2e6d 6172 6b2e 736b 6970 6966 280a 2020  .mark.skipif(.  
+000095a0: 2020 2020 2020 626f 6f6c 286f 732e 656e        bool(os.en
+000095b0: 7669 726f 6e2e 6765 7428 2253 5041 4e4e  viron.get("SPANN
+000095c0: 4552 5f45 4d55 4c41 544f 525f 484f 5354  ER_EMULATOR_HOST
+000095d0: 2229 292c 2072 6561 736f 6e3d 2253 6b69  ")), reason="Ski
+000095e0: 7070 6564 206f 6e20 656d 756c 6174 6f72  pped on emulator
+000095f0: 220a 2020 2020 290a 2020 2020 6465 6620  ".    ).    def 
+00009600: 7465 7374 5f6e 756c 6c5f 626f 756e 645f  test_null_bound_
+00009610: 636f 6d70 6172 6973 6f6e 2873 656c 6629  comparison(self)
+00009620: 3a0a 2020 2020 2020 2020 7375 7065 7228  :.        super(
+00009630: 292e 7465 7374 5f6e 756c 6c5f 626f 756e  ).test_null_boun
+00009640: 645f 636f 6d70 6172 6973 6f6e 2829 0a0a  d_comparison()..
+00009650: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+00009660: 2e73 6b69 7069 6628 0a20 2020 2020 2020  .skipif(.       
+00009670: 2062 6f6f 6c28 6f73 2e65 6e76 6972 6f6e   bool(os.environ
+00009680: 2e67 6574 2822 5350 414e 4e45 525f 454d  .get("SPANNER_EM
+00009690: 554c 4154 4f52 5f48 4f53 5422 2929 2c20  ULATOR_HOST")), 
+000096a0: 7265 6173 6f6e 3d22 536b 6970 7065 6420  reason="Skipped 
+000096b0: 6f6e 2065 6d75 6c61 746f 7222 0a20 2020  on emulator".   
+000096c0: 2029 0a20 2020 2064 6566 2074 6573 745f   ).    def test_
+000096d0: 6e75 6c6c 2873 656c 662c 2063 6f6e 6e65  null(self, conne
+000096e0: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
+000096f0: 7375 7065 7228 292e 7465 7374 5f6e 756c  super().test_nul
+00009700: 6c28 636f 6e6e 6563 7469 6f6e 290a 0a20  l(connection).. 
+00009710: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+00009720: 736b 6970 2822 5370 616e 6e65 7220 6461  skip("Spanner da
+00009730: 7465 7320 6172 6520 7469 6d65 207a 6f6e  tes are time zon
+00009740: 6520 696e 6465 7065 6e64 656e 7422 290a  e independent").
+00009750: 2020 2020 6465 6620 7465 7374 5f73 656c      def test_sel
+00009760: 6563 745f 6469 7265 6374 2873 656c 6629  ect_direct(self)
+00009770: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00009780: 0a40 7079 7465 7374 2e6d 6172 6b2e 736b  .@pytest.mark.sk
+00009790: 6970 2822 4e6f 7420 7375 7070 6f72 7465  ip("Not supporte
+000097a0: 6420 6279 2053 7061 6e6e 6572 2229 0a63  d by Spanner").c
+000097b0: 6c61 7373 2044 6966 6669 6375 6c74 5061  lass DifficultPa
+000097c0: 7261 6d65 7465 7273 5465 7374 285f 4469  rametersTest(_Di
+000097d0: 6666 6963 756c 7450 6172 616d 6574 6572  fficultParameter
+000097e0: 7354 6573 7429 3a0a 2020 2020 7061 7373  sTest):.    pass
+000097f0: 0a0a 0a63 6c61 7373 2046 6574 6368 4c69  ...class FetchLi
+00009800: 6d69 744f 6666 7365 7454 6573 7428 5f46  mitOffsetTest(_F
+00009810: 6574 6368 4c69 6d69 744f 6666 7365 7454  etchLimitOffsetT
+00009820: 6573 7429 3a0a 2020 2020 4070 7974 6573  est):.    @pytes
+00009830: 742e 6d61 726b 2e73 6b69 7028 2253 7061  t.mark.skip("Spa
+00009840: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
+00009850: 706f 7274 2063 6f6d 706f 7369 7465 204c  port composite L
+00009860: 494d 4954 2061 6e64 204f 4646 5345 5420  IMIT and OFFSET 
+00009870: 636c 6175 7365 7322 290a 2020 2020 6465  clauses").    de
+00009880: 6620 7465 7374 5f65 7870 725f 6c69 6d69  f test_expr_limi
+00009890: 7428 7365 6c66 2c20 636f 6e6e 6563 7469  t(self, connecti
+000098a0: 6f6e 293a 0a20 2020 2020 2020 2070 6173  on):.        pas
+000098b0: 730a 0a20 2020 2040 7079 7465 7374 2e6d  s..    @pytest.m
+000098c0: 6172 6b2e 736b 6970 2822 5370 616e 6e65  ark.skip("Spanne
+000098d0: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
+000098e0: 7420 636f 6d70 6f73 6974 6520 4c49 4d49  t composite LIMI
+000098f0: 5420 616e 6420 4f46 4653 4554 2063 6c61  T and OFFSET cla
+00009900: 7573 6573 2229 0a20 2020 2064 6566 2074  uses").    def t
+00009910: 6573 745f 6578 7072 5f6f 6666 7365 7428  est_expr_offset(
+00009920: 7365 6c66 2c20 636f 6e6e 6563 7469 6f6e  self, connection
+00009930: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00009940: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+00009950: 6b2e 736b 6970 2822 5370 616e 6e65 7220  k.skip("Spanner 
+00009960: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
+00009970: 636f 6d70 6f73 6974 6520 4c49 4d49 5420  composite LIMIT 
+00009980: 616e 6420 4f46 4653 4554 2063 6c61 7573  and OFFSET claus
+00009990: 6573 2229 0a20 2020 2064 6566 2074 6573  es").    def tes
+000099a0: 745f 6578 7072 5f6c 696d 6974 5f6f 6666  t_expr_limit_off
+000099b0: 7365 7428 7365 6c66 2c20 636f 6e6e 6563  set(self, connec
+000099c0: 7469 6f6e 293a 0a20 2020 2020 2020 2070  tion):.        p
+000099d0: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
+000099e0: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
+000099f0: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
+00009a00: 6f72 7420 636f 6d70 6f73 6974 6520 4c49  ort composite LI
+00009a10: 4d49 5420 616e 6420 4f46 4653 4554 2063  MIT and OFFSET c
+00009a20: 6c61 7573 6573 2229 0a20 2020 2064 6566  lauses").    def
+00009a30: 2074 6573 745f 6578 7072 5f6c 696d 6974   test_expr_limit
+00009a40: 5f73 696d 706c 655f 6f66 6673 6574 2873  _simple_offset(s
+00009a50: 656c 662c 2063 6f6e 6e65 6374 696f 6e29  elf, connection)
+00009a60: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00009a70: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+00009a80: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
+00009a90: 6f65 736e 2774 2073 7570 706f 7274 2063  oesn't support c
+00009aa0: 6f6d 706f 7369 7465 204c 494d 4954 2061  omposite LIMIT a
+00009ab0: 6e64 204f 4646 5345 5420 636c 6175 7365  nd OFFSET clause
+00009ac0: 7322 290a 2020 2020 6465 6620 7465 7374  s").    def test
+00009ad0: 5f73 696d 706c 655f 6c69 6d69 745f 6578  _simple_limit_ex
+00009ae0: 7072 5f6f 6666 7365 7428 7365 6c66 2c20  pr_offset(self, 
+00009af0: 636f 6e6e 6563 7469 6f6e 293a 0a20 2020  connection):.   
+00009b00: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
+00009b10: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
+00009b20: 2822 5370 616e 6e65 7220 646f 6573 6e27  ("Spanner doesn'
+00009b30: 7420 7375 7070 6f72 7420 636f 6d70 6f73  t support compos
+00009b40: 6974 6520 4c49 4d49 5420 616e 6420 4f46  ite LIMIT and OF
+00009b50: 4653 4554 2063 6c61 7573 6573 2229 0a20  FSET clauses"). 
+00009b60: 2020 2064 6566 2074 6573 745f 626f 756e     def test_boun
+00009b70: 645f 6f66 6673 6574 2873 656c 662c 2063  d_offset(self, c
+00009b80: 6f6e 6e65 6374 696f 6e29 3a0a 2020 2020  onnection):.    
+00009b90: 2020 2020 7061 7373 0a0a 2020 2020 4070      pass..    @p
+00009ba0: 7974 6573 742e 6d61 726b 2e73 6b69 7069  ytest.mark.skipi
+00009bb0: 6628 0a20 2020 2020 2020 2062 6f6f 6c28  f(.        bool(
+00009bc0: 6f73 2e65 6e76 6972 6f6e 2e67 6574 2822  os.environ.get("
+00009bd0: 5350 414e 4e45 525f 454d 554c 4154 4f52  SPANNER_EMULATOR
+00009be0: 5f48 4f53 5422 2929 2c20 7265 6173 6f6e  _HOST")), reason
+00009bf0: 3d22 536b 6970 7065 6420 6f6e 2065 6d75  ="Skipped on emu
+00009c00: 6c61 746f 7222 0a20 2020 2029 0a20 2020  lator".    ).   
+00009c10: 2064 6566 2074 6573 745f 6c69 6d69 745f   def test_limit_
+00009c20: 7265 6e64 6572 5f6d 756c 7469 706c 655f  render_multiple_
+00009c30: 7469 6d65 7328 7365 6c66 2c20 636f 6e6e  times(self, conn
+00009c40: 6563 7469 6f6e 293a 0a20 2020 2020 2020  ection):.       
+00009c50: 2074 6162 6c65 203d 2073 656c 662e 7461   table = self.ta
+00009c60: 626c 6573 2e73 6f6d 655f 7461 626c 650a  bles.some_table.
+00009c70: 2020 2020 2020 2020 7374 6d74 203d 2073          stmt = s
+00009c80: 656c 6563 7428 7461 626c 652e 632e 6964  elect(table.c.id
+00009c90: 292e 6c69 6d69 7428 3129 2e73 6361 6c61  ).limit(1).scala
+00009ca0: 725f 7375 6271 7565 7279 2829 0a0a 2020  r_subquery()..  
+00009cb0: 2020 2020 2020 7520 3d20 756e 696f 6e28        u = union(
+00009cc0: 7365 6c65 6374 2873 746d 7429 2c20 7365  select(stmt), se
+00009cd0: 6c65 6374 2873 746d 7429 292e 7375 6271  lect(stmt)).subq
+00009ce0: 7565 7279 2829 2e73 656c 6563 7428 290a  uery().select().
+00009cf0: 0a20 2020 2020 2020 2073 656c 662e 5f61  .        self._a
+00009d00: 7373 6572 745f 7265 7375 6c74 280a 2020  ssert_result(.  
+00009d10: 2020 2020 2020 2020 2020 636f 6e6e 6563            connec
+00009d20: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+00009d30: 2020 752c 0a20 2020 2020 2020 2020 2020    u,.           
+00009d40: 205b 2831 2c29 5d2c 0a20 2020 2020 2020   [(1,)],.       
+00009d50: 2029 0a0a 2020 2020 4074 6573 7469 6e67   )..    @testing
+00009d60: 2e72 6571 7569 7265 732e 6f66 6673 6574  .requires.offset
+00009d70: 0a20 2020 2064 6566 2074 6573 745f 7369  .    def test_si
+00009d80: 6d70 6c65 5f6f 6666 7365 7428 7365 6c66  mple_offset(self
+00009d90: 2c20 636f 6e6e 6563 7469 6f6e 293a 0a20  , connection):. 
+00009da0: 2020 2020 2020 2074 6162 6c65 203d 2073         table = s
+00009db0: 656c 662e 7461 626c 6573 2e73 6f6d 655f  elf.tables.some_
+00009dc0: 7461 626c 650a 2020 2020 2020 2020 7365  table.        se
+00009dd0: 6c66 2e5f 6173 7365 7274 5f72 6573 756c  lf._assert_resul
+00009de0: 7428 0a20 2020 2020 2020 2020 2020 2063  t(.            c
+00009df0: 6f6e 6e65 6374 696f 6e2c 0a20 2020 2020  onnection,.     
+00009e00: 2020 2020 2020 2073 656c 6563 7428 7461         select(ta
+00009e10: 626c 6529 2e6f 7264 6572 5f62 7928 7461  ble).order_by(ta
+00009e20: 626c 652e 632e 6964 292e 6f66 6673 6574  ble.c.id).offset
+00009e30: 2832 292c 0a20 2020 2020 2020 2020 2020  (2),.           
+00009e40: 205b 2833 2c20 332c 2034 292c 2028 342c   [(3, 3, 4), (4,
+00009e50: 2034 2c20 3529 2c20 2835 2c20 342c 2036   4, 5), (5, 4, 6
+00009e60: 295d 2c0a 2020 2020 2020 2020 290a 0a0a  )],.        )...
+00009e70: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+00009e80: 7028 2253 7061 6e6e 6572 2064 6f65 736e  p("Spanner doesn
+00009e90: 2774 2073 7570 706f 7274 2061 7574 6f69  't support autoi
+00009ea0: 6e63 7265 6d65 6e74 2229 0a63 6c61 7373  ncrement").class
+00009eb0: 2049 6465 6e74 6974 7941 7574 6f69 6e63   IdentityAutoinc
+00009ec0: 7265 6d65 6e74 5465 7374 285f 4964 656e  rementTest(_Iden
+00009ed0: 7469 7479 4175 746f 696e 6372 656d 656e  tityAutoincremen
+00009ee0: 7454 6573 7429 3a0a 2020 2020 7061 7373  tTest):.    pass
+00009ef0: 0a0a 0a63 6c61 7373 2045 7363 6170 696e  ...class Escapin
+00009f00: 6754 6573 7428 5f45 7363 6170 696e 6754  gTest(_EscapingT
+00009f10: 6573 7429 3a0a 2020 2020 4070 726f 7669  est):.    @provi
+00009f20: 6465 5f6d 6574 6164 6174 610a 2020 2020  de_metadata.    
+00009f30: 6465 6620 7465 7374 5f70 6572 6365 6e74  def test_percent
+00009f40: 5f73 6967 6e5f 726f 756e 645f 7472 6970  _sign_round_trip
+00009f50: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00009f60: 2222 2254 6573 7420 7468 6174 2074 6865  """Test that the
+00009f70: 2044 4241 5049 2061 6363 6f6d 6d6f 6461   DBAPI accommoda
+00009f80: 7465 7320 666f 7220 6573 6361 7065 6420  tes for escaped 
+00009f90: 2f20 6e6f 6e65 7363 6170 6564 0a20 2020  / nonescaped.   
+00009fa0: 2020 2020 2070 6572 6365 6e74 2073 6967       percent sig
+00009fb0: 6e73 2069 6e20 6120 7761 7920 7468 6174  ns in a way that
+00009fc0: 206d 6174 6368 6573 2074 6865 2063 6f6d   matches the com
+00009fd0: 7069 6c65 720a 0a20 2020 2020 2020 2053  piler..        S
+00009fe0: 5041 4e4e 4552 204f 5645 5252 4944 450a  PANNER OVERRIDE.
+00009ff0: 2020 2020 2020 2020 436c 6f75 6420 5370          Cloud Sp
+0000a000: 616e 6e65 7220 7375 7070 6f72 7473 2074  anner supports t
+0000a010: 6162 6c65 7320 7769 7468 2065 6d70 7479  ables with empty
+0000a020: 2070 7269 6d61 7279 206b 6579 2c20 6275   primary key, bu
+0000a030: 740a 2020 2020 2020 2020 6f6e 6c79 2073  t.        only s
+0000a040: 696e 676c 6520 6f6e 6520 726f 7720 6361  ingle one row ca
+0000a050: 6e20 6265 2069 6e73 6572 7465 6420 696e  n be inserted in
+0000a060: 746f 2073 7563 6820 6120 7461 626c 6520  to such a table 
+0000a070: 2d0a 2020 2020 2020 2020 666f 6c6c 6f77  -.        follow
+0000a080: 696e 6720 696e 7365 7274 696f 6e73 2077  ing insertions w
+0000a090: 696c 6c20 6661 696c 2077 6974 6820 6052  ill fail with `R
+0000a0a0: 6f77 205b 5d20 616c 7265 6164 7920 6578  ow [] already ex
+0000a0b0: 6973 7473 222e 0a20 2020 2020 2020 204f  ists"..        O
+0000a0c0: 7665 7272 6964 696e 6720 7468 6520 7465  verriding the te
+0000a0d0: 7374 2074 6f20 6176 6f69 6420 7468 6520  st to avoid the 
+0000a0e0: 7361 6d65 2066 6169 6c75 7265 2e0a 2020  same failure..  
+0000a0f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000a100: 2020 6d20 3d20 7365 6c66 2e6d 6574 6164    m = self.metad
+0000a110: 6174 610a 2020 2020 2020 2020 7420 3d20  ata.        t = 
+0000a120: 5461 626c 6528 2274 222c 206d 2c20 436f  Table("t", m, Co
+0000a130: 6c75 6d6e 2822 6461 7461 222c 2053 7472  lumn("data", Str
+0000a140: 696e 6728 3530 2929 290a 2020 2020 2020  ing(50))).      
+0000a150: 2020 742e 6372 6561 7465 2863 6f6e 6669    t.create(confi
+0000a160: 672e 6462 290a 2020 2020 2020 2020 7769  g.db).        wi
+0000a170: 7468 2063 6f6e 6669 672e 6462 2e62 6567  th config.db.beg
+0000a180: 696e 2829 2061 7320 636f 6e6e 3a0a 2020  in() as conn:.  
+0000a190: 2020 2020 2020 2020 2020 636f 6e6e 2e65            conn.e
+0000a1a0: 7865 6375 7465 2874 2e69 6e73 6572 7428  xecute(t.insert(
+0000a1b0: 292c 2064 6963 7428 6461 7461 3d22 736f  ), dict(data="so
+0000a1c0: 6d65 2025 2076 616c 7565 2229 290a 0a20  me % value")).. 
+0000a1d0: 2020 2020 2020 2020 2020 2065 715f 280a             eq_(.
+0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1f0: 636f 6e6e 2e73 6361 6c61 7228 0a20 2020  conn.scalar(.   
+0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a210: 2073 656c 6563 7428 5b74 2e63 2e64 6174   select([t.c.dat
+0000a220: 615d 292e 7768 6572 6528 0a20 2020 2020  a]).where(.     
+0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a240: 2020 2074 2e63 2e64 6174 6120 3d3d 206c     t.c.data == l
+0000a250: 6974 6572 616c 5f63 6f6c 756d 6e28 2227  iteral_column("'
+0000a260: 736f 6d65 2025 2076 616c 7565 2722 290a  some % value'").
+0000a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a280: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000a290: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+0000a2a0: 2020 2020 2020 2020 2022 736f 6d65 2025           "some %
+0000a2b0: 2076 616c 7565 222c 0a20 2020 2020 2020   value",.       
+0000a2c0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000a2d0: 2020 2020 636f 6e6e 2e65 7865 6375 7465      conn.execute
+0000a2e0: 2874 2e64 656c 6574 6528 2929 0a20 2020  (t.delete()).   
+0000a2f0: 2020 2020 2020 2020 2063 6f6e 6e2e 6578           conn.ex
+0000a300: 6563 7574 6528 742e 696e 7365 7274 2829  ecute(t.insert()
+0000a310: 2c20 6469 6374 2864 6174 613d 2273 6f6d  , dict(data="som
+0000a320: 6520 2525 206f 7468 6572 2076 616c 7565  e %% other value
+0000a330: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
+0000a340: 6571 5f28 0a20 2020 2020 2020 2020 2020  eq_(.           
+0000a350: 2020 2020 2063 6f6e 6e2e 7363 616c 6172       conn.scalar
+0000a360: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000a370: 2020 2020 2020 7365 6c65 6374 285b 742e        select([t.
+0000a380: 632e 6461 7461 5d29 2e77 6865 7265 280a  c.data]).where(.
+0000a390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3a0: 2020 2020 2020 2020 742e 632e 6461 7461          t.c.data
+0000a3b0: 203d 3d20 6c69 7465 7261 6c5f 636f 6c75   == literal_colu
+0000a3c0: 6d6e 2822 2773 6f6d 6520 2525 206f 7468  mn("'some %% oth
+0000a3d0: 6572 2076 616c 7565 2722 290a 2020 2020  er value'").    
+0000a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a400: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+0000a410: 2020 2020 2022 736f 6d65 2025 2520 6f74       "some %% ot
+0000a420: 6865 7220 7661 6c75 6522 2c0a 2020 2020  her value",.    
+0000a430: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
+0000a440: 7320 4578 6973 7473 5465 7374 285f 4578  s ExistsTest(_Ex
+0000a450: 6973 7473 5465 7374 293a 0a20 2020 2064  istsTest):.    d
+0000a460: 6566 2074 6573 745f 7365 6c65 6374 5f65  ef test_select_e
+0000a470: 7869 7374 7328 7365 6c66 2c20 636f 6e6e  xists(self, conn
+0000a480: 6563 7469 6f6e 293a 0a20 2020 2020 2020  ection):.       
+0000a490: 2022 2222 0a20 2020 2020 2020 2053 5041   """.        SPA
+0000a4a0: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
+0000a4b0: 2020 2020 2020 2020 5468 6520 6f72 6967          The orig
+0000a4c0: 696e 616c 2074 6573 7420 6973 2074 7279  inal test is try
+0000a4d0: 696e 6720 746f 2065 7865 6375 7465 2061  ing to execute a
+0000a4e0: 2071 7565 7279 206c 696b 653a 0a0a 2020   query like:..  
+0000a4f0: 2020 2020 2020 5345 4c45 4354 202e 2e2e        SELECT ...
+0000a500: 0a20 2020 2020 2020 2057 4845 5245 2045  .        WHERE E
+0000a510: 5849 5354 5320 2853 454c 4543 5420 2e2e  XISTS (SELECT ..
+0000a520: 2e29 0a0a 2020 2020 2020 2020 5345 4c45  .)..        SELE
+0000a530: 4354 2057 4845 5245 2077 6974 686f 7574  CT WHERE without
+0000a540: 2046 524f 4d20 636c 6175 7365 2069 7320   FROM clause is 
+0000a550: 6e6f 7420 7375 7070 6f72 7465 6420 6279  not supported by
+0000a560: 2053 7061 6e6e 6572 2e0a 2020 2020 2020   Spanner..      
+0000a570: 2020 5265 7772 6974 696e 6720 7468 6520    Rewriting the 
+0000a580: 7465 7374 2074 6f20 666f 7263 6520 6974  test to force it
+0000a590: 2074 6f20 6765 6e65 7261 7465 2061 2071   to generate a q
+0000a5a0: 7565 7279 206c 696b 653a 0a0a 2020 2020  uery like:..    
+0000a5b0: 2020 2020 5345 4c45 4354 2045 5849 5354      SELECT EXIST
+0000a5c0: 5320 2853 454c 4543 5420 2e2e 2e29 0a20  S (SELECT ...). 
+0000a5d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000a5e0: 2020 2073 7475 6666 203d 2073 656c 662e     stuff = self.
+0000a5f0: 7461 626c 6573 2e73 7475 6666 0a20 2020  tables.stuff.   
+0000a600: 2020 2020 2065 715f 280a 2020 2020 2020       eq_(.      
+0000a610: 2020 2020 2020 636f 6e6e 6563 7469 6f6e        connection
+0000a620: 2e65 7865 6375 7465 280a 2020 2020 2020  .execute(.      
+0000a630: 2020 2020 2020 2020 2020 7365 6c65 6374            select
+0000a640: 2828 6578 6973 7473 2829 2e77 6865 7265  ((exists().where
+0000a650: 2873 7475 6666 2e63 2e64 6174 6120 3d3d  (stuff.c.data ==
+0000a660: 2022 736f 6d65 2064 6174 6122 292c 2929   "some data"),))
+0000a670: 0a20 2020 2020 2020 2020 2020 2029 2e66  .            ).f
+0000a680: 6574 6368 616c 6c28 292c 0a20 2020 2020  etchall(),.     
+0000a690: 2020 2020 2020 205b 2854 7275 652c 295d         [(True,)]
+0000a6a0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+0000a6b0: 2064 6566 2074 6573 745f 7365 6c65 6374   def test_select
+0000a6c0: 5f65 7869 7374 735f 6661 6c73 6528 7365  _exists_false(se
+0000a6d0: 6c66 2c20 636f 6e6e 6563 7469 6f6e 293a  lf, connection):
+0000a6e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000a6f0: 2020 2020 2053 5041 4e4e 4552 204f 5645       SPANNER OVE
+0000a700: 5252 4944 453a 0a0a 2020 2020 2020 2020  RRIDE:..        
+0000a710: 5468 6520 6f72 6967 696e 616c 2074 6573  The original tes
+0000a720: 7420 6973 2074 7279 696e 6720 746f 2065  t is trying to e
+0000a730: 7865 6375 7465 2061 2071 7565 7279 206c  xecute a query l
+0000a740: 696b 653a 0a0a 2020 2020 2020 2020 5345  ike:..        SE
+0000a750: 4c45 4354 202e 2e2e 0a20 2020 2020 2020  LECT ....       
+0000a760: 2057 4845 5245 2045 5849 5354 5320 2853   WHERE EXISTS (S
+0000a770: 454c 4543 5420 2e2e 2e29 0a0a 2020 2020  ELECT ...)..    
+0000a780: 2020 2020 5345 4c45 4354 2057 4845 5245      SELECT WHERE
+0000a790: 2077 6974 686f 7574 2046 524f 4d20 636c   without FROM cl
+0000a7a0: 6175 7365 2069 7320 6e6f 7420 7375 7070  ause is not supp
+0000a7b0: 6f72 7465 6420 6279 2053 7061 6e6e 6572  orted by Spanner
+0000a7c0: 2e0a 2020 2020 2020 2020 5265 7772 6974  ..        Rewrit
+0000a7d0: 696e 6720 7468 6520 7465 7374 2074 6f20  ing the test to 
+0000a7e0: 666f 7263 6520 6974 2074 6f20 6765 6e65  force it to gene
+0000a7f0: 7261 7465 2061 2071 7565 7279 206c 696b  rate a query lik
+0000a800: 653a 0a0a 2020 2020 2020 2020 5345 4c45  e:..        SELE
+0000a810: 4354 2045 5849 5354 5320 2853 454c 4543  CT EXISTS (SELEC
+0000a820: 5420 2e2e 2e29 0a20 2020 2020 2020 2022  T ...).        "
+0000a830: 2222 0a20 2020 2020 2020 2073 7475 6666  "".        stuff
+0000a840: 203d 2073 656c 662e 7461 626c 6573 2e73   = self.tables.s
+0000a850: 7475 6666 0a20 2020 2020 2020 2065 715f  tuff.        eq_
+0000a860: 280a 2020 2020 2020 2020 2020 2020 636f  (.            co
+0000a870: 6e6e 6563 7469 6f6e 2e65 7865 6375 7465  nnection.execute
+0000a880: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000a890: 2020 7365 6c65 6374 2828 6578 6973 7473    select((exists
+0000a8a0: 2829 2e77 6865 7265 2873 7475 6666 2e63  ().where(stuff.c
+0000a8b0: 2e64 6174 6120 3d3d 2022 6e6f 2064 6174  .data == "no dat
+0000a8c0: 6122 292c 2929 0a20 2020 2020 2020 2020  a"),)).         
+0000a8d0: 2020 2029 2e66 6574 6368 616c 6c28 292c     ).fetchall(),
+0000a8e0: 0a20 2020 2020 2020 2020 2020 205b 2846  .            [(F
+0000a8f0: 616c 7365 2c29 5d2c 0a20 2020 2020 2020  alse,)],.       
+0000a900: 2029 0a0a 0a63 6c61 7373 2054 6162 6c65   )...class Table
+0000a910: 4444 4c54 6573 7428 5f54 6162 6c65 4444  DDLTest(_TableDD
+0000a920: 4c54 6573 7429 3a0a 2020 2020 4070 7974  LTest):.    @pyt
+0000a930: 6573 742e 6d61 726b 2e73 6b69 7028 0a20  est.mark.skip(. 
+0000a940: 2020 2020 2020 2022 5370 616e 6e65 7220         "Spanner 
+0000a950: 7461 626c 6520 6e61 6d65 206d 7573 7420  table name must 
+0000a960: 7374 6172 7420 7769 7468 2061 6e20 7570  start with an up
+0000a970: 7065 7263 6173 6520 6f72 206c 6f77 6572  percase or lower
+0000a980: 6361 7365 206c 6574 7465 7222 0a20 2020  case letter".   
+0000a990: 2029 0a20 2020 2064 6566 2074 6573 745f   ).    def test_
+0000a9a0: 756e 6465 7273 636f 7265 5f6e 616d 6573  underscore_names
+0000a9b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000a9c0: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
+0000a9d0: 742e 6d61 726b 2e73 6b69 7028 2254 6162  t.mark.skip("Tab
+0000a9e0: 6c65 206e 616d 6573 2069 6e63 7564 696e  le names incudin
+0000a9f0: 6720 7363 6865 6d61 7320 6172 6520 6e6f  g schemas are no
+0000aa00: 7420 7375 7070 6f72 7465 6420 6279 2053  t supported by S
+0000aa10: 7061 6e6e 6572 2229 0a20 2020 2064 6566  panner").    def
+0000aa20: 2074 6573 745f 6372 6561 7465 5f74 6162   test_create_tab
+0000aa30: 6c65 5f73 6368 656d 6128 7365 6c66 293a  le_schema(self):
+0000aa40: 0a20 2020 2020 2020 2070 6173 730a 0a0a  .        pass...
+0000aa50: 636c 6173 7320 4675 7475 7265 5461 626c  class FutureTabl
+0000aa60: 6544 444c 5465 7374 285f 4675 7475 7265  eDDLTest(_Future
+0000aa70: 5461 626c 6544 444c 5465 7374 293a 0a20  TableDDLTest):. 
+0000aa80: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+0000aa90: 736b 6970 2822 5461 626c 6520 6e61 6d65  skip("Table name
+0000aaa0: 7320 696e 6375 6469 6e67 2073 6368 656d  s incuding schem
+0000aab0: 6173 2061 7265 206e 6f74 2073 7570 706f  as are not suppo
+0000aac0: 7274 6564 2062 7920 5370 616e 6e65 7222  rted by Spanner"
+0000aad0: 290a 2020 2020 6465 6620 7465 7374 5f63  ).    def test_c
+0000aae0: 7265 6174 655f 7461 626c 655f 7363 6865  reate_table_sche
+0000aaf0: 6d61 2873 656c 6629 3a0a 2020 2020 2020  ma(self):.      
+0000ab00: 2020 7061 7373 0a0a 2020 2020 4070 7974    pass..    @pyt
+0000ab10: 6573 742e 6d61 726b 2e73 6b69 7028 0a20  est.mark.skip(. 
+0000ab20: 2020 2020 2020 2022 5370 616e 6e65 7220         "Spanner 
+0000ab30: 7461 626c 6520 6e61 6d65 206d 7573 7420  table name must 
+0000ab40: 7374 6172 7420 7769 7468 2061 6e20 7570  start with an up
+0000ab50: 7065 7263 6173 6520 6f72 206c 6f77 6572  percase or lower
+0000ab60: 6361 7365 206c 6574 7465 7222 0a20 2020  case letter".   
+0000ab70: 2029 0a20 2020 2064 6566 2074 6573 745f   ).    def test_
+0000ab80: 756e 6465 7273 636f 7265 5f6e 616d 6573  underscore_names
+0000ab90: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000aba0: 7061 7373 0a0a 0a40 7079 7465 7374 2e6d  pass...@pytest.m
+0000abb0: 6172 6b2e 736b 6970 2822 4d61 7820 6964  ark.skip("Max id
+0000abc0: 656e 7469 6669 6572 206c 656e 6774 6820  entifier length 
+0000abd0: 696e 2053 7061 6e6e 6572 2069 7320 3132  in Spanner is 12
+0000abe0: 3822 290a 636c 6173 7320 4c6f 6e67 4e61  8").class LongNa
+0000abf0: 6d65 426c 6f77 6f75 7454 6573 7428 5f4c  meBlowoutTest(_L
+0000ac00: 6f6e 674e 616d 6542 6c6f 776f 7574 5465  ongNameBlowoutTe
+0000ac10: 7374 293a 0a20 2020 2070 6173 730a 0a0a  st):.    pass...
+0000ac20: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+0000ac30: 7028 2253 7061 6e6e 6572 2064 6f65 736e  p("Spanner doesn
+0000ac40: 2774 2073 7570 706f 7274 2054 696d 6520  't support Time 
+0000ac50: 6461 7461 2074 7970 652e 2229 0a63 6c61  data type.").cla
+0000ac60: 7373 2054 696d 6554 6573 7473 285f 5469  ss TimeTests(_Ti
+0000ac70: 6d65 4d69 6372 6f73 6563 6f6e 6473 5465  meMicrosecondsTe
+0000ac80: 7374 2c20 5f54 696d 6554 6573 7429 3a0a  st, _TimeTest):.
+0000ac90: 2020 2020 7061 7373 0a0a 0a40 7079 7465      pass...@pyte
+0000aca0: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
+0000acb0: 616e 6e65 7220 646f 6573 6e27 7420 636f  anner doesn't co
+0000acc0: 6572 6365 2064 6174 6573 2066 726f 6d20  erce dates from 
+0000acd0: 6461 7465 7469 6d65 2e22 290a 636c 6173  datetime.").clas
+0000ace0: 7320 4461 7465 5469 6d65 436f 6572 6365  s DateTimeCoerce
+0000acf0: 6454 6f44 6174 6554 696d 6554 6573 7428  dToDateTimeTest(
+0000ad00: 5f44 6174 6554 696d 6543 6f65 7263 6564  _DateTimeCoerced
+0000ad10: 546f 4461 7465 5469 6d65 5465 7374 293a  ToDateTimeTest):
+0000ad20: 0a20 2020 2070 6173 730a 0a0a 636c 6173  .    pass...clas
+0000ad30: 7320 496e 7465 6765 7254 6573 7428 5f49  s IntegerTest(_I
+0000ad40: 6e74 6567 6572 5465 7374 293a 0a20 2020  ntegerTest):.   
+0000ad50: 2040 7072 6f76 6964 655f 6d65 7461 6461   @provide_metada
+0000ad60: 7461 0a20 2020 2064 6566 205f 726f 756e  ta.    def _roun
+0000ad70: 645f 7472 6970 2873 656c 662c 2064 6174  d_trip(self, dat
+0000ad80: 6174 7970 652c 2064 6174 6129 3a0a 2020  atype, data):.  
+0000ad90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000ada0: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
+0000adb0: 4445 3a0a 0a20 2020 2020 2020 2054 6869  DE:..        Thi
+0000adc0: 7320 6973 2074 6865 2068 656c 7065 7220  s is the helper 
+0000add0: 6d65 7468 6f64 2066 6f72 2069 6e74 6567  method for integ
+0000ade0: 6572 2063 6c61 7373 2074 6573 7473 2077  er class tests w
+0000adf0: 6869 6368 2063 7265 6174 6573 2061 2074  hich creates a t
+0000ae00: 6162 6c65 2061 6e64 0a20 2020 2020 2020  able and.       
+0000ae10: 2070 6572 666f 726d 7320 616e 2069 6e73   performs an ins
+0000ae20: 6572 7420 6f70 6572 6174 696f 6e2e 0a20  ert operation.. 
+0000ae30: 2020 2020 2020 2043 6c6f 7564 2053 7061         Cloud Spa
+0000ae40: 6e6e 6572 2073 7570 706f 7274 7320 7461  nner supports ta
+0000ae50: 626c 6573 2077 6974 6820 616e 2065 6d70  bles with an emp
+0000ae60: 7479 2070 7269 6d61 7279 206b 6579 2c20  ty primary key, 
+0000ae70: 6275 7420 6f6e 6c79 206f 6e65 0a20 2020  but only one.   
+0000ae80: 2020 2020 2072 6f77 2063 616e 2062 6520       row can be 
+0000ae90: 696e 7365 7274 6564 2069 6e74 6f20 7375  inserted into su
+0000aea0: 6368 2061 2074 6162 6c65 202d 2066 6f6c  ch a table - fol
+0000aeb0: 6c6f 7769 6e67 2069 6e73 6572 7469 6f6e  lowing insertion
+0000aec0: 7320 7769 6c6c 2066 6169 6c20 7769 7468  s will fail with
+0000aed0: 0a20 2020 2020 2020 2060 3430 3020 6964  .        `400 id
+0000aee0: 206d 7573 7420 6e6f 7420 6265 204e 554c   must not be NUL
+0000aef0: 4c20 696e 2074 6162 6c65 2064 6174 655f  L in table date_
+0000af00: 7461 626c 6560 2e0a 2020 2020 2020 2020  table`..        
+0000af10: 4f76 6572 7269 6469 6e67 2074 6865 2074  Overriding the t
+0000af20: 6573 7473 2061 6e64 2061 6464 696e 6720  ests and adding 
+0000af30: 6120 6d61 6e75 616c 2070 7269 6d61 7279  a manual primary
+0000af40: 206b 6579 2076 616c 7565 2074 6f20 6176   key value to av
+0000af50: 6f69 6420 7468 6520 7361 6d65 0a20 2020  oid the same.   
+0000af60: 2020 2020 2066 6169 6c75 7265 732e 0a20       failures.. 
+0000af70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000af80: 2020 206d 6574 6164 6174 6120 3d20 7365     metadata = se
+0000af90: 6c66 2e6d 6574 6164 6174 610a 2020 2020  lf.metadata.    
+0000afa0: 2020 2020 696e 745f 7461 626c 6520 3d20      int_table = 
+0000afb0: 5461 626c 6528 0a20 2020 2020 2020 2020  Table(.         
+0000afc0: 2020 2022 696e 7465 6765 725f 7461 626c     "integer_tabl
+0000afd0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+0000afe0: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+0000aff0: 2020 2020 2020 436f 6c75 6d6e 2822 6964        Column("id
+0000b000: 222c 2049 6e74 6567 6572 2c20 7072 696d  ", Integer, prim
+0000b010: 6172 795f 6b65 793d 5472 7565 2c20 7465  ary_key=True, te
+0000b020: 7374 5f6e 6565 6473 5f61 7574 6f69 6e63  st_needs_autoinc
+0000b030: 7265 6d65 6e74 3d54 7275 6529 2c0a 2020  rement=True),.  
+0000b040: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
+0000b050: 2822 696e 7465 6765 725f 6461 7461 222c  ("integer_data",
+0000b060: 2064 6174 6174 7970 6529 2c0a 2020 2020   datatype),.    
+0000b070: 2020 2020 290a 0a20 2020 2020 2020 206d      )..        m
+0000b080: 6574 6164 6174 612e 6372 6561 7465 5f61  etadata.create_a
+0000b090: 6c6c 2863 6f6e 6669 672e 6462 290a 0a20  ll(config.db).. 
+0000b0a0: 2020 2020 2020 2063 6f6e 6669 672e 6462         config.db
+0000b0b0: 2e65 7865 6375 7465 2869 6e74 5f74 6162  .execute(int_tab
+0000b0c0: 6c65 2e69 6e73 6572 7428 292c 207b 2269  le.insert(), {"i
+0000b0d0: 6422 3a20 312c 2022 696e 7465 6765 725f  d": 1, "integer_
+0000b0e0: 6461 7461 223a 2064 6174 617d 290a 0a20  data": data}).. 
+0000b0f0: 2020 2020 2020 2072 6f77 203d 2063 6f6e         row = con
+0000b100: 6669 672e 6462 2e65 7865 6375 7465 2873  fig.db.execute(s
+0000b110: 656c 6563 7428 5b69 6e74 5f74 6162 6c65  elect([int_table
+0000b120: 2e63 2e69 6e74 6567 6572 5f64 6174 615d  .c.integer_data]
+0000b130: 2929 2e66 6972 7374 2829 0a0a 2020 2020  )).first()..    
+0000b140: 2020 2020 6571 5f28 726f 772c 2028 6461      eq_(row, (da
+0000b150: 7461 2c29 290a 0a20 2020 2020 2020 2069  ta,))..        i
+0000b160: 6620 7574 696c 2e70 7933 6b3a 0a20 2020  f util.py3k:.   
+0000b170: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000b180: 6973 696e 7374 616e 6365 2872 6f77 5b30  isinstance(row[0
+0000b190: 5d2c 2069 6e74 290a 2020 2020 2020 2020  ], int).        
+0000b1a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000b1b0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+0000b1c0: 6e63 6528 726f 775b 305d 2c20 286c 6f6e  nce(row[0], (lon
+0000b1d0: 672c 2069 6e74 2929 2020 2320 6e6f 7161  g, int))  # noqa
+0000b1e0: 0a0a 0a63 6c61 7373 205f 556e 6963 6f64  ...class _Unicod
+0000b1f0: 6546 6978 7475 7265 285f 5f55 6e69 636f  eFixture(__Unico
+0000b200: 6465 4669 7874 7572 6529 3a0a 2020 2020  deFixture):.    
+0000b210: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+0000b220: 2064 6566 2064 6566 696e 655f 7461 626c   def define_tabl
+0000b230: 6573 2863 6c73 2c20 6d65 7461 6461 7461  es(cls, metadata
+0000b240: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000b250: 2020 2020 2020 2053 5041 4e4e 4552 204f         SPANNER O
+0000b260: 5645 5252 4944 453a 0a0a 2020 2020 2020  VERRIDE:..      
+0000b270: 2020 436c 6f75 6420 5370 616e 6e65 7220    Cloud Spanner 
+0000b280: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
+0000b290: 6175 746f 2069 6e63 7265 6d65 6e74 696e  auto incrementin
+0000b2a0: 6720 6964 7320 6665 6174 7572 652c 0a20  g ids feature,. 
+0000b2b0: 2020 2020 2020 2077 6869 6368 2069 7320         which is 
+0000b2c0: 7573 6564 2062 7920 7468 6520 6f72 6967  used by the orig
+0000b2d0: 696e 616c 2074 6573 742e 204f 7665 7272  inal test. Overr
+0000b2e0: 6964 696e 6720 7468 6520 7465 7374 2064  iding the test d
+0000b2f0: 6174 610a 2020 2020 2020 2020 6372 6561  ata.        crea
+0000b300: 7469 6f6e 206d 6574 686f 6420 746f 2064  tion method to d
+0000b310: 6973 6162 6c65 2061 7574 6f69 6e63 7265  isable autoincre
+0000b320: 6d65 6e74 2061 6e64 206d 616b 6520 6964  ment and make id
+0000b330: 2063 6f6c 756d 6e0a 2020 2020 2020 2020   column.        
+0000b340: 6e75 6c6c 6162 6c65 2e0a 2020 2020 2020  nullable..      
+0000b350: 2020 2222 220a 2020 2020 2020 2020 5461    """.        Ta
 0000b360: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
-0000b370: 2020 2020 2022 7422 2c0a 2020 2020 2020       "t",.      
-0000b380: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
-0000b390: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
-0000b3a0: 2020 2020 436f 6c75 6d6e 2822 7822 2c20      Column("x", 
-0000b3b0: 7479 7065 5f29 2c0a 2020 2020 2020 2020  type_),.        
-0000b3c0: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-0000b3d0: 6964 222c 2049 6e74 6567 6572 2c20 7072  id", Integer, pr
-0000b3e0: 696d 6172 795f 6b65 793d 5472 7565 292c  imary_key=True),
-0000b3f0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000b400: 2020 2020 2020 2020 2020 2074 2e63 7265             t.cre
-0000b410: 6174 6528 636f 6e6e 6563 7469 6f6e 290a  ate(connection).
-0000b420: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
-0000b430: 6563 7469 6f6e 2e63 6f6e 6e65 6374 696f  ection.connectio
-0000b440: 6e2e 636f 6d6d 6974 2829 0a20 2020 2020  n.commit().     
-0000b450: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
-0000b460: 6e2e 6578 6563 7574 6528 0a20 2020 2020  n.execute(.     
-0000b470: 2020 2020 2020 2020 2020 2074 2e69 6e73             t.ins
-0000b480: 6572 7428 292c 205b 7b22 7822 3a20 782c  ert(), [{"x": x,
-0000b490: 2022 6964 223a 2069 7d20 666f 7220 692c   "id": i} for i,
-0000b4a0: 2078 2069 6e20 656e 756d 6572 6174 6528   x in enumerate(
-0000b4b0: 696e 7075 745f 295d 0a20 2020 2020 2020  input_)].       
-0000b4c0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000b4d0: 2020 2020 7265 7375 6c74 203d 207b 726f      result = {ro
-0000b4e0: 775b 305d 2066 6f72 2072 6f77 2069 6e20  w[0] for row in 
-0000b4f0: 636f 6e6e 6563 7469 6f6e 2e65 7865 6375  connection.execu
-0000b500: 7465 2874 2e73 656c 6563 7428 2929 7d0a  te(t.select())}.
-0000b510: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-0000b520: 7574 203d 2073 6574 286f 7574 7075 7429  ut = set(output)
-0000b530: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000b540: 6669 6c74 6572 5f3a 0a20 2020 2020 2020  filter_:.       
-0000b550: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-0000b560: 3d20 7365 7428 6669 6c74 6572 5f28 7829  = set(filter_(x)
-0000b570: 2066 6f72 2078 2069 6e20 7265 7375 6c74   for x in result
-0000b580: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000b590: 2020 6f75 7470 7574 203d 2073 6574 2866    output = set(f
-0000b5a0: 696c 7465 725f 2878 2920 666f 7220 7820  ilter_(x) for x 
-0000b5b0: 696e 206f 7574 7075 7429 0a20 2020 2020  in output).     
-0000b5c0: 2020 2020 2020 2065 715f 2872 6573 756c         eq_(resul
-0000b5d0: 742c 206f 7574 7075 7429 0a20 2020 2020  t, output).     
-0000b5e0: 2020 2020 2020 2069 6620 6368 6563 6b5f         if check_
-0000b5f0: 7363 616c 653a 0a20 2020 2020 2020 2020  scale:.         
-0000b600: 2020 2020 2020 2065 715f 285b 7374 7228         eq_([str(
-0000b610: 7829 2066 6f72 2078 2069 6e20 7265 7375  x) for x in resu
-0000b620: 6c74 5d2c 205b 7374 7228 7829 2066 6f72  lt], [str(x) for
-0000b630: 2078 2069 6e20 6f75 7470 7574 5d29 0a0a   x in output])..
-0000b640: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0000b650: 756e 0a0a 2020 2020 4065 6d69 7473 5f77  un..    @emits_w
-0000b660: 6172 6e69 6e67 2872 222e 2a64 6f65 7320  arning(r".*does 
-0000b670: 5c2a 6e6f 745c 2a20 7375 7070 6f72 7420  \*not\* support 
-0000b680: 4465 6369 6d61 6c20 6f62 6a65 6374 7320  Decimal objects 
-0000b690: 6e61 7469 7665 6c79 2229 0a20 2020 2064  natively").    d
-0000b6a0: 6566 2074 6573 745f 7265 6e64 6572 5f6c  ef test_render_l
-0000b6b0: 6974 6572 616c 5f6e 756d 6572 6963 2873  iteral_numeric(s
-0000b6c0: 656c 662c 206c 6974 6572 616c 5f72 6f75  elf, literal_rou
-0000b6d0: 6e64 5f74 7269 7029 3a0a 2020 2020 2020  nd_trip):.      
-0000b6e0: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
-0000b6f0: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
-0000b700: 0a20 2020 2020 2020 2043 6c6f 7564 2053  .        Cloud S
-0000b710: 7061 6e6e 6572 2073 7570 706f 7274 7320  panner supports 
-0000b720: 7461 626c 6573 2077 6974 6820 616e 2065  tables with an e
-0000b730: 6d70 7479 2070 7269 6d61 7279 206b 6579  mpty primary key
-0000b740: 2c20 6275 740a 2020 2020 2020 2020 6f6e  , but.        on
-0000b750: 6c79 2061 2073 696e 676c 6520 726f 7720  ly a single row 
-0000b760: 6361 6e20 6265 2069 6e73 6572 7465 6420  can be inserted 
-0000b770: 696e 746f 2073 7563 6820 6120 7461 626c  into such a tabl
-0000b780: 6520 2d0a 2020 2020 2020 2020 666f 6c6c  e -.        foll
-0000b790: 6f77 696e 6720 696e 7365 7274 696f 6e73  owing insertions
-0000b7a0: 2077 696c 6c20 6661 696c 2077 6974 6820   will fail with 
-0000b7b0: 6052 6f77 205b 5d20 616c 7265 6164 7920  `Row [] already 
-0000b7c0: 6578 6973 7473 222e 0a20 2020 2020 2020  exists"..       
-0000b7d0: 204f 7665 7272 6964 696e 6720 7468 6520   Overriding the 
-0000b7e0: 7465 7374 2074 6f20 6176 6f69 6420 7468  test to avoid th
-0000b7f0: 6520 7361 6d65 2066 6169 6c75 7265 2e0a  e same failure..
-0000b800: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000b810: 2020 2020 6c69 7465 7261 6c5f 726f 756e      literal_roun
-0000b820: 645f 7472 6970 280a 2020 2020 2020 2020  d_trip(.        
-0000b830: 2020 2020 4e75 6d65 7269 6328 7072 6563      Numeric(prec
-0000b840: 6973 696f 6e3d 382c 2073 6361 6c65 3d34  ision=8, scale=4
-0000b850: 292c 0a20 2020 2020 2020 2020 2020 205b  ),.            [
-0000b860: 6465 6369 6d61 6c2e 4465 6369 6d61 6c28  decimal.Decimal(
-0000b870: 2231 352e 3735 3633 2229 5d2c 0a20 2020  "15.7563")],.   
-0000b880: 2020 2020 2020 2020 205b 6465 6369 6d61           [decima
-0000b890: 6c2e 4465 6369 6d61 6c28 2231 352e 3735  l.Decimal("15.75
-0000b8a0: 3633 2229 5d2c 0a20 2020 2020 2020 2029  63")],.        )
-0000b8b0: 0a0a 2020 2020 4065 6d69 7473 5f77 6172  ..    @emits_war
-0000b8c0: 6e69 6e67 2872 222e 2a64 6f65 7320 5c2a  ning(r".*does \*
-0000b8d0: 6e6f 745c 2a20 7375 7070 6f72 7420 4465  not\* support De
-0000b8e0: 6369 6d61 6c20 6f62 6a65 6374 7320 6e61  cimal objects na
-0000b8f0: 7469 7665 6c79 2229 0a20 2020 2064 6566  tively").    def
-0000b900: 2074 6573 745f 7265 6e64 6572 5f6c 6974   test_render_lit
-0000b910: 6572 616c 5f6e 756d 6572 6963 5f61 7366  eral_numeric_asf
-0000b920: 6c6f 6174 2873 656c 662c 206c 6974 6572  loat(self, liter
-0000b930: 616c 5f72 6f75 6e64 5f74 7269 7029 3a0a  al_round_trip):.
-0000b940: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000b950: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
-0000b960: 5249 4445 3a0a 0a20 2020 2020 2020 2043  RIDE:..        C
-0000b970: 6c6f 7564 2053 7061 6e6e 6572 2073 7570  loud Spanner sup
-0000b980: 706f 7274 7320 7461 626c 6573 2077 6974  ports tables wit
-0000b990: 6820 616e 2065 6d70 7479 2070 7269 6d61  h an empty prima
-0000b9a0: 7279 206b 6579 2c20 6275 740a 2020 2020  ry key, but.    
-0000b9b0: 2020 2020 6f6e 6c79 2061 2073 696e 676c      only a singl
-0000b9c0: 6520 726f 7720 6361 6e20 6265 2069 6e73  e row can be ins
-0000b9d0: 6572 7465 6420 696e 746f 2073 7563 6820  erted into such 
-0000b9e0: 6120 7461 626c 6520 2d0a 2020 2020 2020  a table -.      
-0000b9f0: 2020 666f 6c6c 6f77 696e 6720 696e 7365    following inse
-0000ba00: 7274 696f 6e73 2077 696c 6c20 6661 696c  rtions will fail
-0000ba10: 2077 6974 6820 6052 6f77 205b 5d20 616c   with `Row [] al
-0000ba20: 7265 6164 7920 6578 6973 7473 222e 0a20  ready exists".. 
-0000ba30: 2020 2020 2020 204f 7665 7272 6964 696e         Overridin
-0000ba40: 6720 7468 6520 7465 7374 2074 6f20 6176  g the test to av
-0000ba50: 6f69 6420 7468 6520 7361 6d65 2066 6169  oid the same fai
-0000ba60: 6c75 7265 2e0a 2020 2020 2020 2020 2222  lure..        ""
-0000ba70: 220a 2020 2020 2020 2020 6c69 7465 7261  ".        litera
-0000ba80: 6c5f 726f 756e 645f 7472 6970 280a 2020  l_round_trip(.  
-0000ba90: 2020 2020 2020 2020 2020 4e75 6d65 7269            Numeri
-0000baa0: 6328 7072 6563 6973 696f 6e3d 382c 2073  c(precision=8, s
-0000bab0: 6361 6c65 3d34 2c20 6173 6465 6369 6d61  cale=4, asdecima
-0000bac0: 6c3d 4661 6c73 6529 2c0a 2020 2020 2020  l=False),.      
-0000bad0: 2020 2020 2020 5b64 6563 696d 616c 2e44        [decimal.D
-0000bae0: 6563 696d 616c 2822 3135 2e37 3536 3322  ecimal("15.7563"
-0000baf0: 295d 2c0a 2020 2020 2020 2020 2020 2020  )],.            
-0000bb00: 5b31 352e 3735 3633 5d2c 0a20 2020 2020  [15.7563],.     
-0000bb10: 2020 2029 0a0a 2020 2020 6465 6620 7465     )..    def te
-0000bb20: 7374 5f72 656e 6465 725f 6c69 7465 7261  st_render_litera
-0000bb30: 6c5f 666c 6f61 7428 7365 6c66 2c20 6c69  l_float(self, li
-0000bb40: 7465 7261 6c5f 726f 756e 645f 7472 6970  teral_round_trip
-0000bb50: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000bb60: 2020 2020 2020 2053 5041 4e4e 4552 204f         SPANNER O
-0000bb70: 5645 5252 4944 453a 0a0a 2020 2020 2020  VERRIDE:..      
-0000bb80: 2020 436c 6f75 6420 5370 616e 6e65 7220    Cloud Spanner 
-0000bb90: 7375 7070 6f72 7473 2074 6162 6c65 7320  supports tables 
-0000bba0: 7769 7468 2061 6e20 656d 7074 7920 7072  with an empty pr
-0000bbb0: 696d 6172 7920 6b65 792c 2062 7574 0a20  imary key, but. 
-0000bbc0: 2020 2020 2020 206f 6e6c 7920 6120 7369         only a si
-0000bbd0: 6e67 6c65 2072 6f77 2063 616e 2062 6520  ngle row can be 
-0000bbe0: 696e 7365 7274 6564 2069 6e74 6f20 7375  inserted into su
-0000bbf0: 6368 2061 2074 6162 6c65 202d 0a20 2020  ch a table -.   
-0000bc00: 2020 2020 2066 6f6c 6c6f 7769 6e67 2069       following i
-0000bc10: 6e73 6572 7469 6f6e 7320 7769 6c6c 2066  nsertions will f
-0000bc20: 6169 6c20 7769 7468 2060 526f 7720 5b5d  ail with `Row []
-0000bc30: 2061 6c72 6561 6479 2065 7869 7374 7322   already exists"
-0000bc40: 2e0a 2020 2020 2020 2020 4f76 6572 7269  ..        Overri
-0000bc50: 6469 6e67 2074 6865 2074 6573 7420 746f  ding the test to
-0000bc60: 2061 766f 6964 2074 6865 2073 616d 6520   avoid the same 
-0000bc70: 6661 696c 7572 652e 0a20 2020 2020 2020  failure..       
-0000bc80: 2022 2222 0a20 2020 2020 2020 206c 6974   """.        lit
-0000bc90: 6572 616c 5f72 6f75 6e64 5f74 7269 7028  eral_round_trip(
-0000bca0: 0a20 2020 2020 2020 2020 2020 2046 6c6f  .            Flo
-0000bcb0: 6174 2834 292c 0a20 2020 2020 2020 2020  at(4),.         
-0000bcc0: 2020 205b 6465 6369 6d61 6c2e 4465 6369     [decimal.Deci
-0000bcd0: 6d61 6c28 2231 352e 3735 3633 2229 5d2c  mal("15.7563")],
-0000bce0: 0a20 2020 2020 2020 2020 2020 205b 3135  .            [15
-0000bcf0: 2e37 3536 335d 2c0a 2020 2020 2020 2020  .7563],.        
-0000bd00: 2020 2020 6669 6c74 6572 5f3d 6c61 6d62      filter_=lamb
-0000bd10: 6461 206e 3a20 6e20 6973 206e 6f74 204e  da n: n is not N
-0000bd20: 6f6e 6520 616e 6420 726f 756e 6428 6e2c  one and round(n,
-0000bd30: 2035 2920 6f72 204e 6f6e 652c 0a20 2020   5) or None,.   
-0000bd40: 2020 2020 2029 0a0a 2020 2020 4072 6571       )..    @req
-0000bd50: 7569 7265 732e 7072 6563 6973 696f 6e5f  uires.precision_
-0000bd60: 6765 6e65 7269 635f 666c 6f61 745f 7479  generic_float_ty
-0000bd70: 7065 0a20 2020 2064 6566 2074 6573 745f  pe.    def test_
-0000bd80: 666c 6f61 745f 6375 7374 6f6d 5f73 6361  float_custom_sca
-0000bd90: 6c65 2873 656c 662c 2064 6f5f 6e75 6d65  le(self, do_nume
-0000bda0: 7269 635f 7465 7374 293a 0a20 2020 2020  ric_test):.     
-0000bdb0: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-0000bdc0: 5041 4e4e 4552 204f 5645 5252 4944 453a  PANNER OVERRIDE:
-0000bdd0: 0a0a 2020 2020 2020 2020 436c 6f75 6420  ..        Cloud 
-0000bde0: 5370 616e 6e65 7220 7375 7070 6f72 7473  Spanner supports
-0000bdf0: 2074 6162 6c65 7320 7769 7468 2061 6e20   tables with an 
-0000be00: 656d 7074 7920 7072 696d 6172 7920 6b65  empty primary ke
-0000be10: 792c 2062 7574 0a20 2020 2020 2020 206f  y, but.        o
-0000be20: 6e6c 7920 6120 7369 6e67 6c65 2072 6f77  nly a single row
-0000be30: 2063 616e 2062 6520 696e 7365 7274 6564   can be inserted
-0000be40: 2069 6e74 6f20 7375 6368 2061 2074 6162   into such a tab
-0000be50: 6c65 202d 0a20 2020 2020 2020 2066 6f6c  le -.        fol
-0000be60: 6c6f 7769 6e67 2069 6e73 6572 7469 6f6e  lowing insertion
-0000be70: 7320 7769 6c6c 2066 6169 6c20 7769 7468  s will fail with
-0000be80: 2060 526f 7720 5b5d 2061 6c72 6561 6479   `Row [] already
-0000be90: 2065 7869 7374 7322 2e0a 2020 2020 2020   exists"..      
-0000bea0: 2020 4f76 6572 7269 6469 6e67 2074 6865    Overriding the
-0000beb0: 2074 6573 7420 746f 2061 766f 6964 2074   test to avoid t
-0000bec0: 6865 2073 616d 6520 6661 696c 7572 652e  he same failure.
-0000bed0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000bee0: 2020 2020 2064 6f5f 6e75 6d65 7269 635f       do_numeric_
-0000bef0: 7465 7374 280a 2020 2020 2020 2020 2020  test(.          
-0000bf00: 2020 466c 6f61 7428 4e6f 6e65 2c20 6465    Float(None, de
-0000bf10: 6369 6d61 6c5f 7265 7475 726e 5f73 6361  cimal_return_sca
-0000bf20: 6c65 3d37 2c20 6173 6465 6369 6d61 6c3d  le=7, asdecimal=
-0000bf30: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-0000bf40: 2020 205b 6465 6369 6d61 6c2e 4465 6369     [decimal.Deci
-0000bf50: 6d61 6c28 2231 352e 3735 3633 3832 3722  mal("15.7563827"
-0000bf60: 292c 2064 6563 696d 616c 2e44 6563 696d  ), decimal.Decim
-0000bf70: 616c 2822 3135 2e37 3536 3338 3237 2229  al("15.7563827")
-0000bf80: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-0000bf90: 6465 6369 6d61 6c2e 4465 6369 6d61 6c28  decimal.Decimal(
-0000bfa0: 2231 352e 3735 3633 3832 3722 295d 2c0a  "15.7563827")],.
-0000bfb0: 2020 2020 2020 2020 2020 2020 6368 6563              chec
-0000bfc0: 6b5f 7363 616c 653d 5472 7565 2c0a 2020  k_scale=True,.  
-0000bfd0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-0000bfe0: 2074 6573 745f 6e75 6d65 7269 635f 6173   test_numeric_as
-0000bff0: 5f64 6563 696d 616c 2873 656c 662c 2064  _decimal(self, d
-0000c000: 6f5f 6e75 6d65 7269 635f 7465 7374 293a  o_numeric_test):
-0000c010: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c020: 2020 2020 2053 5041 4e4e 4552 204f 5645       SPANNER OVE
-0000c030: 5252 4944 453a 0a0a 2020 2020 2020 2020  RRIDE:..        
-0000c040: 5370 616e 6e65 7220 7468 726f 7773 2061  Spanner throws a
-0000c050: 6e20 6572 726f 7220 3430 3020 5661 6c75  n error 400 Valu
-0000c060: 6520 6861 7320 7479 7065 2046 4c4f 4154  e has type FLOAT
-0000c070: 3634 2077 6869 6368 2063 616e 6e6f 7420  64 which cannot 
-0000c080: 6265 0a20 2020 2020 2020 2069 6e73 6572  be.        inser
-0000c090: 7465 6420 696e 746f 2063 6f6c 756d 6e20  ted into column 
-0000c0a0: 782c 2077 6869 6368 2068 6173 2074 7970  x, which has typ
-0000c0b0: 6520 4e55 4d45 5249 4320 666f 7220 7661  e NUMERIC for va
-0000c0c0: 6c75 6520 3135 2e37 3536 332e 0a20 2020  lue 15.7563..   
-0000c0d0: 2020 2020 204f 7665 7272 6964 696e 6720       Overriding 
-0000c0e0: 7468 6520 7465 7374 2074 6f20 7265 6d6f  the test to remo
-0000c0f0: 7665 2074 6865 2066 6169 6c75 7265 2063  ve the failure c
-0000c100: 6173 652e 0a20 2020 2020 2020 2022 2222  ase..        """
-0000c110: 0a20 2020 2020 2020 2064 6f5f 6e75 6d65  .        do_nume
-0000c120: 7269 635f 7465 7374 280a 2020 2020 2020  ric_test(.      
-0000c130: 2020 2020 2020 4e75 6d65 7269 6328 7072        Numeric(pr
-0000c140: 6563 6973 696f 6e3d 382c 2073 6361 6c65  ecision=8, scale
-0000c150: 3d34 292c 0a20 2020 2020 2020 2020 2020  =4),.           
-0000c160: 205b 6465 6369 6d61 6c2e 4465 6369 6d61   [decimal.Decima
-0000c170: 6c28 2231 352e 3735 3633 2229 2c20 6465  l("15.7563"), de
-0000c180: 6369 6d61 6c2e 4465 6369 6d61 6c28 2231  cimal.Decimal("1
-0000c190: 352e 3735 3633 2229 5d2c 0a20 2020 2020  5.7563")],.     
-0000c1a0: 2020 2020 2020 205b 6465 6369 6d61 6c2e         [decimal.
-0000c1b0: 4465 6369 6d61 6c28 2231 352e 3735 3633  Decimal("15.7563
-0000c1c0: 2229 5d2c 0a20 2020 2020 2020 2029 0a0a  ")],.        )..
-0000c1d0: 2020 2020 6465 6620 7465 7374 5f6e 756d      def test_num
-0000c1e0: 6572 6963 5f61 735f 666c 6f61 7428 7365  eric_as_float(se
-0000c1f0: 6c66 2c20 646f 5f6e 756d 6572 6963 5f74  lf, do_numeric_t
-0000c200: 6573 7429 3a0a 2020 2020 2020 2020 2222  est):.        ""
-0000c210: 220a 2020 2020 2020 2020 5350 414e 4e45  ".        SPANNE
-0000c220: 5220 4f56 4552 5249 4445 3a0a 0a20 2020  R OVERRIDE:..   
-0000c230: 2020 2020 2053 7061 6e6e 6572 2074 6872       Spanner thr
-0000c240: 6f77 7320 616e 2065 7272 6f72 2034 3030  ows an error 400
-0000c250: 2056 616c 7565 2068 6173 2074 7970 6520   Value has type 
-0000c260: 464c 4f41 5436 3420 7768 6963 6820 6361  FLOAT64 which ca
-0000c270: 6e6e 6f74 2062 650a 2020 2020 2020 2020  nnot be.        
-0000c280: 696e 7365 7274 6564 2069 6e74 6f20 636f  inserted into co
-0000c290: 6c75 6d6e 2078 2c20 7768 6963 6820 6861  lumn x, which ha
-0000c2a0: 7320 7479 7065 204e 554d 4552 4943 2066  s type NUMERIC f
-0000c2b0: 6f72 2076 616c 7565 2031 352e 3735 3633  or value 15.7563
-0000c2c0: 2e0a 2020 2020 2020 2020 4f76 6572 7269  ..        Overri
-0000c2d0: 6469 6e67 2074 6865 2074 6573 7420 746f  ding the test to
-0000c2e0: 2072 656d 6f76 6520 7468 6520 6661 696c   remove the fail
-0000c2f0: 7572 6520 6361 7365 2e0a 2020 2020 2020  ure case..      
-0000c300: 2020 2222 220a 2020 2020 2020 2020 646f    """.        do
-0000c310: 5f6e 756d 6572 6963 5f74 6573 7428 0a20  _numeric_test(. 
-0000c320: 2020 2020 2020 2020 2020 204e 756d 6572             Numer
-0000c330: 6963 2870 7265 6369 7369 6f6e 3d38 2c20  ic(precision=8, 
-0000c340: 7363 616c 653d 342c 2061 7364 6563 696d  scale=4, asdecim
-0000c350: 616c 3d46 616c 7365 292c 0a20 2020 2020  al=False),.     
-0000c360: 2020 2020 2020 205b 6465 6369 6d61 6c2e         [decimal.
-0000c370: 4465 6369 6d61 6c28 2231 352e 3735 3633  Decimal("15.7563
-0000c380: 2229 2c20 6465 6369 6d61 6c2e 4465 6369  "), decimal.Deci
-0000c390: 6d61 6c28 2231 352e 3735 3633 2229 5d2c  mal("15.7563")],
-0000c3a0: 0a20 2020 2020 2020 2020 2020 205b 3135  .            [15
-0000c3b0: 2e37 3536 335d 2c0a 2020 2020 2020 2020  .7563],.        
-0000c3c0: 290a 0a20 2020 2040 7265 7175 6972 6573  )..    @requires
-0000c3d0: 2e66 6c6f 6174 735f 746f 5f66 6f75 725f  .floats_to_four_
-0000c3e0: 6465 6369 6d61 6c73 0a20 2020 2064 6566  decimals.    def
-0000c3f0: 2074 6573 745f 666c 6f61 745f 6173 5f64   test_float_as_d
-0000c400: 6563 696d 616c 2873 656c 662c 2064 6f5f  ecimal(self, do_
-0000c410: 6e75 6d65 7269 635f 7465 7374 293a 0a20  numeric_test):. 
-0000c420: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000c430: 2020 2053 5041 4e4e 4552 204f 5645 5252     SPANNER OVERR
-0000c440: 4944 453a 0a0a 2020 2020 2020 2020 436c  IDE:..        Cl
-0000c450: 6f75 6420 5370 616e 6e65 7220 7375 7070  oud Spanner supp
-0000c460: 6f72 7473 2074 6162 6c65 7320 7769 7468  orts tables with
-0000c470: 2061 6e20 656d 7074 7920 7072 696d 6172   an empty primar
-0000c480: 7920 6b65 792c 2062 7574 0a20 2020 2020  y key, but.     
-0000c490: 2020 206f 6e6c 7920 6120 7369 6e67 6c65     only a single
-0000c4a0: 2072 6f77 2063 616e 2062 6520 696e 7365   row can be inse
-0000c4b0: 7274 6564 2069 6e74 6f20 7375 6368 2061  rted into such a
-0000c4c0: 2074 6162 6c65 202d 0a20 2020 2020 2020   table -.       
-0000c4d0: 2066 6f6c 6c6f 7769 6e67 2069 6e73 6572   following inser
-0000c4e0: 7469 6f6e 7320 7769 6c6c 2066 6169 6c20  tions will fail 
-0000c4f0: 7769 7468 2060 526f 7720 5b5d 2061 6c72  with `Row [] alr
-0000c500: 6561 6479 2065 7869 7374 7322 2e0a 2020  eady exists"..  
-0000c510: 2020 2020 2020 4f76 6572 7269 6469 6e67        Overriding
-0000c520: 2074 6865 2074 6573 7420 746f 2061 766f   the test to avo
-0000c530: 6964 2074 6865 2073 616d 6520 6661 696c  id the same fail
-0000c540: 7572 652e 0a20 2020 2020 2020 2022 2222  ure..        """
-0000c550: 0a20 2020 2020 2020 2064 6f5f 6e75 6d65  .        do_nume
-0000c560: 7269 635f 7465 7374 280a 2020 2020 2020  ric_test(.      
-0000c570: 2020 2020 2020 466c 6f61 7428 7072 6563        Float(prec
-0000c580: 6973 696f 6e3d 382c 2061 7364 6563 696d  ision=8, asdecim
-0000c590: 616c 3d54 7275 6529 2c0a 2020 2020 2020  al=True),.      
-0000c5a0: 2020 2020 2020 5b64 6563 696d 616c 2e44        [decimal.D
-0000c5b0: 6563 696d 616c 2822 3135 2e37 3536 3322  ecimal("15.7563"
-0000c5c0: 292c 2064 6563 696d 616c 2e44 6563 696d  ), decimal.Decim
-0000c5d0: 616c 2822 3135 2e37 3536 3322 292c 204e  al("15.7563"), N
-0000c5e0: 6f6e 655d 2c0a 2020 2020 2020 2020 2020  one],.          
-0000c5f0: 2020 5b64 6563 696d 616c 2e44 6563 696d    [decimal.Decim
-0000c600: 616c 2822 3135 2e37 3536 3322 292c 204e  al("15.7563"), N
-0000c610: 6f6e 655d 2c0a 2020 2020 2020 2020 2020  one],.          
-0000c620: 2020 6669 6c74 6572 5f3d 6c61 6d62 6461    filter_=lambda
-0000c630: 206e 3a20 6e20 6973 206e 6f74 204e 6f6e   n: n is not Non
-0000c640: 6520 616e 6420 726f 756e 6428 6e2c 2034  e and round(n, 4
-0000c650: 2920 6f72 204e 6f6e 652c 0a20 2020 2020  ) or None,.     
-0000c660: 2020 2029 0a0a 2020 2020 6465 6620 7465     )..    def te
-0000c670: 7374 5f66 6c6f 6174 5f61 735f 666c 6f61  st_float_as_floa
-0000c680: 7428 7365 6c66 2c20 646f 5f6e 756d 6572  t(self, do_numer
-0000c690: 6963 5f74 6573 7429 3a0a 2020 2020 2020  ic_test):.      
-0000c6a0: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
-0000c6b0: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
-0000c6c0: 0a20 2020 2020 2020 2043 6c6f 7564 2053  .        Cloud S
-0000c6d0: 7061 6e6e 6572 2073 7570 706f 7274 7320  panner supports 
-0000c6e0: 7461 626c 6573 2077 6974 6820 616e 2065  tables with an e
-0000c6f0: 6d70 7479 2070 7269 6d61 7279 206b 6579  mpty primary key
-0000c700: 2c20 6275 740a 2020 2020 2020 2020 6f6e  , but.        on
-0000c710: 6c79 2061 2073 696e 676c 6520 726f 7720  ly a single row 
-0000c720: 6361 6e20 6265 2069 6e73 6572 7465 6420  can be inserted 
-0000c730: 696e 746f 2073 7563 6820 6120 7461 626c  into such a tabl
-0000c740: 6520 2d0a 2020 2020 2020 2020 666f 6c6c  e -.        foll
-0000c750: 6f77 696e 6720 696e 7365 7274 696f 6e73  owing insertions
-0000c760: 2077 696c 6c20 6661 696c 2077 6974 6820   will fail with 
-0000c770: 6052 6f77 205b 5d20 616c 7265 6164 7920  `Row [] already 
-0000c780: 6578 6973 7473 222e 0a20 2020 2020 2020  exists"..       
-0000c790: 204f 7665 7272 6964 696e 6720 7468 6520   Overriding the 
-0000c7a0: 7465 7374 2074 6f20 6176 6f69 6420 7468  test to avoid th
-0000c7b0: 6520 7361 6d65 2066 6169 6c75 7265 2e0a  e same failure..
-0000c7c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000c7d0: 2020 2020 646f 5f6e 756d 6572 6963 5f74      do_numeric_t
-0000c7e0: 6573 7428 0a20 2020 2020 2020 2020 2020  est(.           
-0000c7f0: 2046 6c6f 6174 2870 7265 6369 7369 6f6e   Float(precision
-0000c800: 3d38 292c 0a20 2020 2020 2020 2020 2020  =8),.           
-0000c810: 205b 6465 6369 6d61 6c2e 4465 6369 6d61   [decimal.Decima
-0000c820: 6c28 2231 352e 3735 3633 2229 2c20 6465  l("15.7563"), de
-0000c830: 6369 6d61 6c2e 4465 6369 6d61 6c28 2231  cimal.Decimal("1
-0000c840: 352e 3735 3633 2229 5d2c 0a20 2020 2020  5.7563")],.     
-0000c850: 2020 2020 2020 205b 3135 2e37 3536 335d         [15.7563]
-0000c860: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
-0000c870: 6c74 6572 5f3d 6c61 6d62 6461 206e 3a20  lter_=lambda n: 
-0000c880: 6e20 6973 206e 6f74 204e 6f6e 6520 616e  n is not None an
-0000c890: 6420 726f 756e 6428 6e2c 2035 2920 6f72  d round(n, 5) or
-0000c8a0: 204e 6f6e 652c 0a20 2020 2020 2020 2029   None,.        )
-0000c8b0: 0a0a 2020 2020 4072 6571 7569 7265 732e  ..    @requires.
-0000c8c0: 7072 6563 6973 696f 6e5f 6e75 6d65 7269  precision_numeri
-0000c8d0: 6373 5f67 656e 6572 616c 0a20 2020 2064  cs_general.    d
-0000c8e0: 6566 2074 6573 745f 7072 6563 6973 696f  ef test_precisio
-0000c8f0: 6e5f 6465 6369 6d61 6c28 7365 6c66 2c20  n_decimal(self, 
-0000c900: 646f 5f6e 756d 6572 6963 5f74 6573 7429  do_numeric_test)
-0000c910: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000c920: 2020 2020 2020 5350 414e 4e45 5220 4f56        SPANNER OV
-0000c930: 4552 5249 4445 3a0a 0a20 2020 2020 2020  ERRIDE:..       
-0000c940: 2043 6c6f 7564 2053 7061 6e6e 6572 2073   Cloud Spanner s
-0000c950: 7570 706f 7274 7320 7461 626c 6573 2077  upports tables w
-0000c960: 6974 6820 616e 2065 6d70 7479 2070 7269  ith an empty pri
-0000c970: 6d61 7279 206b 6579 2c20 6275 740a 2020  mary key, but.  
-0000c980: 2020 2020 2020 6f6e 6c79 2061 2073 696e        only a sin
-0000c990: 676c 6520 726f 7720 6361 6e20 6265 2069  gle row can be i
-0000c9a0: 6e73 6572 7465 6420 696e 746f 2073 7563  nserted into suc
-0000c9b0: 6820 6120 7461 626c 6520 2d0a 2020 2020  h a table -.    
-0000c9c0: 2020 2020 666f 6c6c 6f77 696e 6720 696e      following in
-0000c9d0: 7365 7274 696f 6e73 2077 696c 6c20 6661  sertions will fa
-0000c9e0: 696c 2077 6974 6820 6052 6f77 205b 5d20  il with `Row [] 
-0000c9f0: 616c 7265 6164 7920 6578 6973 7473 222e  already exists".
-0000ca00: 0a20 2020 2020 2020 204f 7665 7272 6964  .        Overrid
-0000ca10: 696e 6720 7468 6520 7465 7374 2074 6f20  ing the test to 
-0000ca20: 6176 6f69 6420 7468 6520 7361 6d65 2066  avoid the same f
-0000ca30: 6169 6c75 7265 2e0a 0a20 2020 2020 2020  ailure...       
-0000ca40: 2052 656d 6f76 6520 616e 2065 7874 7261   Remove an extra
-0000ca50: 2064 6967 6974 7320 6166 7465 7220 6465   digits after de
-0000ca60: 6369 6d61 6c20 706f 696e 7420 6173 2063  cimal point as c
-0000ca70: 6c6f 7564 2073 7061 6e6e 6572 2069 730a  loud spanner is.
-0000ca80: 2020 2020 2020 2020 6361 7061 626c 6520          capable 
-0000ca90: 6f66 2072 6570 7265 7365 6e74 696e 6720  of representing 
-0000caa0: 616e 2065 7861 6374 206e 756d 6572 6963  an exact numeric
-0000cab0: 2076 616c 7565 2077 6974 6820 6120 7072   value with a pr
-0000cac0: 6563 6973 696f 6e0a 2020 2020 2020 2020  ecision.        
-0000cad0: 6f66 2033 3820 616e 6420 7363 616c 6520  of 38 and scale 
-0000cae0: 6f66 2039 2e0a 2020 2020 2020 2020 2222  of 9..        ""
-0000caf0: 220a 2020 2020 2020 2020 6e75 6d62 6572  ".        number
-0000cb00: 7320 3d20 7365 7428 0a20 2020 2020 2020  s = set(.       
-0000cb10: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-0000cb20: 2020 2020 2020 2064 6563 696d 616c 2e44         decimal.D
-0000cb30: 6563 696d 616c 2822 3534 2e32 3436 3435  ecimal("54.24645
-0000cb40: 3136 3530 2229 2c0a 2020 2020 2020 2020  1650"),.        
-0000cb50: 2020 2020 2020 2020 6465 6369 6d61 6c2e          decimal.
-0000cb60: 4465 6369 6d61 6c28 2230 2e30 3034 3335  Decimal("0.00435
-0000cb70: 3422 292c 0a20 2020 2020 2020 2020 2020  4"),.           
-0000cb80: 2020 2020 2064 6563 696d 616c 2e44 6563       decimal.Dec
-0000cb90: 696d 616c 2822 3930 302e 3022 292c 0a20  imal("900.0"),. 
-0000cba0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-0000cbb0: 2020 2020 2029 0a20 2020 2020 2020 2064       ).        d
-0000cbc0: 6f5f 6e75 6d65 7269 635f 7465 7374 284e  o_numeric_test(N
-0000cbd0: 756d 6572 6963 2870 7265 6369 7369 6f6e  umeric(precision
-0000cbe0: 3d31 382c 2073 6361 6c65 3d39 292c 206e  =18, scale=9), n
-0000cbf0: 756d 6265 7273 2c20 6e75 6d62 6572 7329  umbers, numbers)
-0000cc00: 0a0a 2020 2020 4074 6573 7469 6e67 2e72  ..    @testing.r
-0000cc10: 6571 7569 7265 732e 7072 6563 6973 696f  equires.precisio
-0000cc20: 6e5f 6e75 6d65 7269 6373 5f65 6e6f 7461  n_numerics_enota
-0000cc30: 7469 6f6e 5f6c 6172 6765 0a20 2020 2064  tion_large.    d
-0000cc40: 6566 2074 6573 745f 656e 6f74 6174 696f  ef test_enotatio
-0000cc50: 6e5f 6465 6369 6d61 6c5f 6c61 7267 6528  n_decimal_large(
-0000cc60: 7365 6c66 2c20 646f 5f6e 756d 6572 6963  self, do_numeric
-0000cc70: 5f74 6573 7429 3a0a 2020 2020 2020 2020  _test):.        
-0000cc80: 2222 2274 6573 7420 6578 6365 6564 696e  """test exceedin
-0000cc90: 676c 7920 6c61 7267 6520 6465 6369 6d61  gly large decima
-0000cca0: 6c73 2e0a 0a20 2020 2020 2020 2053 5041  ls...        SPA
-0000ccb0: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
-0000ccc0: 2020 2020 2020 2020 436c 6f75 6420 5370          Cloud Sp
-0000ccd0: 616e 6e65 7220 7375 7070 6f72 7473 2074  anner supports t
-0000cce0: 6162 6c65 7320 7769 7468 2061 6e20 656d  ables with an em
-0000ccf0: 7074 7920 7072 696d 6172 7920 6b65 792c  pty primary key,
-0000cd00: 2062 7574 0a20 2020 2020 2020 206f 6e6c   but.        onl
-0000cd10: 7920 6120 7369 6e67 6c65 2072 6f77 2063  y a single row c
-0000cd20: 616e 2062 6520 696e 7365 7274 6564 2069  an be inserted i
-0000cd30: 6e74 6f20 7375 6368 2061 2074 6162 6c65  nto such a table
-0000cd40: 202d 0a20 2020 2020 2020 2066 6f6c 6c6f   -.        follo
-0000cd50: 7769 6e67 2069 6e73 6572 7469 6f6e 7320  wing insertions 
-0000cd60: 7769 6c6c 2066 6169 6c20 7769 7468 2060  will fail with `
-0000cd70: 526f 7720 5b5d 2061 6c72 6561 6479 2065  Row [] already e
-0000cd80: 7869 7374 7322 2e0a 2020 2020 2020 2020  xists"..        
-0000cd90: 4f76 6572 7269 6469 6e67 2074 6865 2074  Overriding the t
-0000cda0: 6573 7420 746f 2061 766f 6964 2074 6865  est to avoid the
-0000cdb0: 2073 616d 6520 6661 696c 7572 652e 0a20   same failure.. 
-0000cdc0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000cdd0: 2020 206e 756d 6265 7273 203d 2073 6574     numbers = set
-0000cde0: 280a 2020 2020 2020 2020 2020 2020 5b0a  (.            [.
-0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce00: 6465 6369 6d61 6c2e 4465 6369 6d61 6c28  decimal.Decimal(
-0000ce10: 2234 452b 3822 292c 0a20 2020 2020 2020  "4E+8"),.       
-0000ce20: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
-0000ce30: 2e44 6563 696d 616c 2822 3537 3438 452b  .Decimal("5748E+
-0000ce40: 3135 2229 2c0a 2020 2020 2020 2020 2020  15"),.          
-0000ce50: 2020 2020 2020 6465 6369 6d61 6c2e 4465        decimal.De
-0000ce60: 6369 6d61 6c28 2231 2e35 3231 452b 3135  cimal("1.521E+15
-0000ce70: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-0000ce80: 2020 2020 6465 6369 6d61 6c2e 4465 6369      decimal.Deci
-0000ce90: 6d61 6c28 2230 3030 3030 3030 3030 2e31  mal("000000000.1
-0000cea0: 452b 3922 292c 0a20 2020 2020 2020 2020  E+9"),.         
-0000ceb0: 2020 205d 0a20 2020 2020 2020 2029 0a20     ].        ). 
-0000cec0: 2020 2020 2020 2064 6f5f 6e75 6d65 7269         do_numeri
-0000ced0: 635f 7465 7374 284e 756d 6572 6963 2870  c_test(Numeric(p
-0000cee0: 7265 6369 7369 6f6e 3d32 352c 2073 6361  recision=25, sca
-0000cef0: 6c65 3d32 292c 206e 756d 6265 7273 2c20  le=2), numbers, 
-0000cf00: 6e75 6d62 6572 7329 0a0a 2020 2020 4074  numbers)..    @t
-0000cf10: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
-0000cf20: 7072 6563 6973 696f 6e5f 6e75 6d65 7269  precision_numeri
-0000cf30: 6373 5f65 6e6f 7461 7469 6f6e 5f6c 6172  cs_enotation_lar
-0000cf40: 6765 0a20 2020 2064 6566 2074 6573 745f  ge.    def test_
-0000cf50: 656e 6f74 6174 696f 6e5f 6465 6369 6d61  enotation_decima
-0000cf60: 6c28 7365 6c66 2c20 646f 5f6e 756d 6572  l(self, do_numer
-0000cf70: 6963 5f74 6573 7429 3a0a 2020 2020 2020  ic_test):.      
-0000cf80: 2020 2222 2274 6573 7420 6578 6365 6564    """test exceed
-0000cf90: 696e 676c 7920 736d 616c 6c20 6465 6369  ingly small deci
-0000cfa0: 6d61 6c73 2e0a 0a20 2020 2020 2020 2044  mals...        D
-0000cfb0: 6563 696d 616c 2072 6570 6f72 7473 2076  ecimal reports v
-0000cfc0: 616c 7565 7320 7769 7468 2045 206e 6f74  alues with E not
-0000cfd0: 6174 696f 6e20 7768 656e 2074 6865 2065  ation when the e
-0000cfe0: 7870 6f6e 656e 740a 2020 2020 2020 2020  xponent.        
-0000cff0: 6973 2067 7265 6174 6572 2074 6861 6e20  is greater than 
-0000d000: 362e 0a0a 2020 2020 2020 2020 5350 414e  6...        SPAN
-0000d010: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
-0000d020: 2020 2020 2020 2052 656d 6f76 6520 6578         Remove ex
-0000d030: 7472 6120 6469 6769 7473 2061 6674 6572  tra digits after
-0000d040: 2064 6563 696d 616c 2070 6f69 6e74 2061   decimal point a
-0000d050: 7320 436c 6f75 6420 5370 616e 6e65 7220  s Cloud Spanner 
-0000d060: 6973 0a20 2020 2020 2020 2063 6170 6162  is.        capab
-0000d070: 6c65 206f 6620 7265 7072 6573 656e 7469  le of representi
-0000d080: 6e67 2061 6e20 6578 6163 7420 6e75 6d65  ng an exact nume
-0000d090: 7269 6320 7661 6c75 6520 7769 7468 2061  ric value with a
-0000d0a0: 2070 7265 6369 7369 6f6e 0a20 2020 2020   precision.     
-0000d0b0: 2020 206f 6620 3338 2061 6e64 2073 6361     of 38 and sca
-0000d0c0: 6c65 206f 6620 392e 0a20 2020 2020 2020  le of 9..       
-0000d0d0: 2022 2222 0a20 2020 2020 2020 206e 756d   """.        num
-0000d0e0: 6265 7273 203d 2073 6574 280a 2020 2020  bers = set(.    
-0000d0f0: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
-0000d100: 2020 2020 2020 2020 2020 6465 6369 6d61            decima
-0000d110: 6c2e 4465 6369 6d61 6c28 2231 452d 3222  l.Decimal("1E-2"
-0000d120: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000d130: 2020 2064 6563 696d 616c 2e44 6563 696d     decimal.Decim
-0000d140: 616c 2822 3145 2d33 2229 2c0a 2020 2020  al("1E-3"),.    
-0000d150: 2020 2020 2020 2020 2020 2020 6465 6369              deci
-0000d160: 6d61 6c2e 4465 6369 6d61 6c28 2231 452d  mal.Decimal("1E-
-0000d170: 3422 292c 0a20 2020 2020 2020 2020 2020  4"),.           
-0000d180: 2020 2020 2064 6563 696d 616c 2e44 6563       decimal.Dec
-0000d190: 696d 616c 2822 3145 2d35 2229 2c0a 2020  imal("1E-5"),.  
-0000d1a0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-0000d1b0: 6369 6d61 6c2e 4465 6369 6d61 6c28 2231  cimal.Decimal("1
-0000d1c0: 452d 3622 292c 0a20 2020 2020 2020 2020  E-6"),.         
-0000d1d0: 2020 2020 2020 2064 6563 696d 616c 2e44         decimal.D
-0000d1e0: 6563 696d 616c 2822 3145 2d37 2229 2c0a  ecimal("1E-7"),.
-0000d1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d200: 6465 6369 6d61 6c2e 4465 6369 6d61 6c28  decimal.Decimal(
-0000d210: 2231 452d 3822 292c 0a20 2020 2020 2020  "1E-8"),.       
-0000d220: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
-0000d230: 2e44 6563 696d 616c 2822 302e 3130 3539  .Decimal("0.1059
-0000d240: 3430 3639 3622 292c 0a20 2020 2020 2020  40696"),.       
-0000d250: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
-0000d260: 2e44 6563 696d 616c 2822 302e 3030 3539  .Decimal("0.0059
-0000d270: 3430 3639 3622 292c 0a20 2020 2020 2020  40696"),.       
-0000d280: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
-0000d290: 2e44 6563 696d 616c 2822 302e 3030 3030  .Decimal("0.0000
-0000d2a0: 3030 3639 3622 292c 0a20 2020 2020 2020  00696"),.       
-0000d2b0: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
-0000d2c0: 2e44 6563 696d 616c 2822 302e 3730 3030  .Decimal("0.7000
-0000d2d0: 3030 3639 3622 292c 0a20 2020 2020 2020  00696"),.       
-0000d2e0: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
-0000d2f0: 2e44 6563 696d 616c 2822 3639 3645 2d39  .Decimal("696E-9
-0000d300: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-0000d310: 5d0a 2020 2020 2020 2020 290a 2020 2020  ].        ).    
-0000d320: 2020 2020 646f 5f6e 756d 6572 6963 5f74      do_numeric_t
-0000d330: 6573 7428 4e75 6d65 7269 6328 7072 6563  est(Numeric(prec
-0000d340: 6973 696f 6e3d 3338 2c20 7363 616c 653d  ision=38, scale=
-0000d350: 3929 2c20 6e75 6d62 6572 732c 206e 756d  9), numbers, num
-0000d360: 6265 7273 290a 0a0a 636c 6173 7320 4c69  bers)...class Li
-0000d370: 6b65 4675 6e63 7469 6f6e 7354 6573 7428  keFunctionsTest(
-0000d380: 5f4c 696b 6546 756e 6374 696f 6e73 5465  _LikeFunctionsTe
-0000d390: 7374 293a 0a20 2020 2040 7079 7465 7374  st):.    @pytest
-0000d3a0: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
-0000d3b0: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
-0000d3c0: 6f72 7420 4c49 4b45 2045 5343 4150 4520  ort LIKE ESCAPE 
-0000d3d0: 636c 6175 7365 2229 0a20 2020 2064 6566  clause").    def
-0000d3e0: 2074 6573 745f 636f 6e74 6169 6e73 5f61   test_contains_a
-0000d3f0: 7574 6f65 7363 6170 6528 7365 6c66 293a  utoescape(self):
-0000d400: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-0000d410: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-0000d420: 736b 6970 2822 5370 616e 6e65 7220 646f  skip("Spanner do
-0000d430: 6573 6e27 7420 7375 7070 6f72 7420 4c49  esn't support LI
-0000d440: 4b45 2045 5343 4150 4520 636c 6175 7365  KE ESCAPE clause
-0000d450: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
-0000d460: 636f 6e74 6169 6e73 5f61 7574 6f65 7363  contains_autoesc
-0000d470: 6170 655f 6573 6361 7065 2873 656c 6629  ape_escape(self)
-0000d480: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-0000d490: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-0000d4a0: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
-0000d4b0: 6f65 736e 2774 2073 7570 706f 7274 204c  oesn't support L
-0000d4c0: 494b 4520 4553 4341 5045 2063 6c61 7573  IKE ESCAPE claus
-0000d4d0: 6522 290a 2020 2020 6465 6620 7465 7374  e").    def test
-0000d4e0: 5f63 6f6e 7461 696e 735f 6573 6361 7065  _contains_escape
-0000d4f0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000d500: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
-0000d510: 742e 6d61 726b 2e73 6b69 7028 2253 7061  t.mark.skip("Spa
-0000d520: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
-0000d530: 706f 7274 204c 494b 4520 4553 4341 5045  port LIKE ESCAPE
-0000d540: 2063 6c61 7573 6522 290a 2020 2020 6465   clause").    de
-0000d550: 6620 7465 7374 5f65 6e64 7377 6974 685f  f test_endswith_
-0000d560: 6175 746f 6573 6361 7065 2873 656c 6629  autoescape(self)
-0000d570: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-0000d580: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-0000d590: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
-0000d5a0: 6f65 736e 2774 2073 7570 706f 7274 204c  oesn't support L
-0000d5b0: 494b 4520 4553 4341 5045 2063 6c61 7573  IKE ESCAPE claus
-0000d5c0: 6522 290a 2020 2020 6465 6620 7465 7374  e").    def test
-0000d5d0: 5f65 6e64 7377 6974 685f 6573 6361 7065  _endswith_escape
-0000d5e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000d5f0: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
-0000d600: 742e 6d61 726b 2e73 6b69 7028 2253 7061  t.mark.skip("Spa
-0000d610: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
-0000d620: 706f 7274 204c 494b 4520 4553 4341 5045  port LIKE ESCAPE
-0000d630: 2063 6c61 7573 6522 290a 2020 2020 6465   clause").    de
-0000d640: 6620 7465 7374 5f65 6e64 7377 6974 685f  f test_endswith_
-0000d650: 6175 746f 6573 6361 7065 5f65 7363 6170  autoescape_escap
-0000d660: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-0000d670: 2070 6173 730a 0a20 2020 2040 7079 7465   pass..    @pyte
-0000d680: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
-0000d690: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
-0000d6a0: 7070 6f72 7420 4c49 4b45 2045 5343 4150  pport LIKE ESCAP
-0000d6b0: 4520 636c 6175 7365 2229 0a20 2020 2064  E clause").    d
-0000d6c0: 6566 2074 6573 745f 7374 6172 7473 7769  ef test_startswi
-0000d6d0: 7468 5f61 7574 6f65 7363 6170 6528 7365  th_autoescape(se
-0000d6e0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-0000d6f0: 730a 0a20 2020 2040 7079 7465 7374 2e6d  s..    @pytest.m
-0000d700: 6172 6b2e 736b 6970 2822 5370 616e 6e65  ark.skip("Spanne
-0000d710: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
-0000d720: 7420 4c49 4b45 2045 5343 4150 4520 636c  t LIKE ESCAPE cl
-0000d730: 6175 7365 2229 0a20 2020 2064 6566 2074  ause").    def t
-0000d740: 6573 745f 7374 6172 7473 7769 7468 5f65  est_startswith_e
-0000d750: 7363 6170 6528 7365 6c66 293a 0a20 2020  scape(self):.   
-0000d760: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
-0000d770: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-0000d780: 2822 5370 616e 6e65 7220 646f 6573 6e27  ("Spanner doesn'
-0000d790: 7420 7375 7070 6f72 7420 4c49 4b45 2045  t support LIKE E
-0000d7a0: 5343 4150 4520 636c 6175 7365 2229 0a20  SCAPE clause"). 
-0000d7b0: 2020 2064 6566 2074 6573 745f 7374 6172     def test_star
-0000d7c0: 7473 7769 7468 5f61 7574 6f65 7363 6170  tswith_autoescap
-0000d7d0: 655f 6573 6361 7065 2873 656c 6629 3a0a  e_escape(self):.
-0000d7e0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-0000d7f0: 2020 6465 6620 7465 7374 5f65 7363 6170    def test_escap
-0000d800: 655f 6b65 7977 6f72 645f 7261 6973 6573  e_keyword_raises
-0000d810: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000d820: 2222 2243 6865 636b 2074 6861 7420 4553  """Check that ES
-0000d830: 4341 5045 206b 6579 776f 7264 2063 6175  CAPE keyword cau
-0000d840: 7365 7320 616e 2065 7863 6570 7469 6f6e  ses an exception
-0000d850: 2077 6865 6e20 7573 6564 2e22 2222 0a20   when used.""". 
-0000d860: 2020 2020 2020 2077 6974 6820 7079 7465         with pyte
-0000d870: 7374 2e72 6169 7365 7328 4e6f 7449 6d70  st.raises(NotImp
-0000d880: 6c65 6d65 6e74 6564 4572 726f 7229 3a0a  lementedError):.
-0000d890: 2020 2020 2020 2020 2020 2020 636f 6c20              col 
-0000d8a0: 3d20 7365 6c66 2e74 6162 6c65 732e 736f  = self.tables.so
-0000d8b0: 6d65 5f74 6162 6c65 2e63 2e64 6174 610a  me_table.c.data.
-0000d8c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d8d0: 2e5f 7465 7374 2863 6f6c 2e63 6f6e 7461  ._test(col.conta
-0000d8e0: 696e 7328 2262 2323 6364 6522 2c20 6573  ins("b##cde", es
-0000d8f0: 6361 7065 3d22 2322 292c 207b 377d 290a  cape="#"), {7}).
-0000d900: 0a0a 4070 7974 6573 742e 6d61 726b 2e73  ..@pytest.mark.s
-0000d910: 6b69 7028 2253 7061 6e6e 6572 2064 6f65  kip("Spanner doe
-0000d920: 736e 2774 2073 7570 706f 7274 2049 5320  sn't support IS 
-0000d930: 4449 5354 494e 4354 2046 524f 4d20 636c  DISTINCT FROM cl
-0000d940: 6175 7365 2229 0a63 6c61 7373 2049 734f  ause").class IsO
-0000d950: 7249 734e 6f74 4469 7374 696e 6374 4672  rIsNotDistinctFr
-0000d960: 6f6d 5465 7374 285f 4973 4f72 4973 4e6f  omTest(_IsOrIsNo
-0000d970: 7444 6973 7469 6e63 7446 726f 6d54 6573  tDistinctFromTes
-0000d980: 7429 3a0a 2020 2020 7061 7373 0a0a 0a63  t):.    pass...c
-0000d990: 6c61 7373 204f 7264 6572 4279 4c61 6265  lass OrderByLabe
-0000d9a0: 6c54 6573 7428 5f4f 7264 6572 4279 4c61  lTest(_OrderByLa
-0000d9b0: 6265 6c54 6573 7429 3a0a 2020 2020 4070  belTest):.    @p
-0000d9c0: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
-0000d9d0: 0a20 2020 2020 2020 2022 5370 616e 6e65  .        "Spanne
-0000d9e0: 7220 7265 7175 6972 6573 2061 6e20 616c  r requires an al
-0000d9f0: 6961 7320 666f 7220 7468 6520 4752 4f55  ias for the GROU
-0000da00: 5020 4259 206c 6973 7420 7768 656e 2073  P BY list when s
-0000da10: 7065 6369 6679 696e 6720 6465 7269 7665  pecifying derive
-0000da20: 6420 220a 2020 2020 2020 2020 2263 6f6c  d ".        "col
-0000da30: 756d 6e73 2061 6c73 6f20 7573 6564 2069  umns also used i
-0000da40: 6e20 5345 4c45 4354 220a 2020 2020 290a  n SELECT".    ).
-0000da50: 2020 2020 6465 6620 7465 7374 5f67 726f      def test_gro
-0000da60: 7570 5f62 795f 636f 6d70 6f73 6564 2873  up_by_composed(s
-0000da70: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-0000da80: 7373 0a0a 0a63 6c61 7373 2043 6f6d 706f  ss...class Compo
-0000da90: 756e 6453 656c 6563 7454 6573 7428 5f43  undSelectTest(_C
-0000daa0: 6f6d 706f 756e 6453 656c 6563 7454 6573  ompoundSelectTes
-0000dab0: 7429 3a0a 2020 2020 2222 220a 2020 2020  t):.    """.    
-0000dac0: 5365 653a 2068 7474 7073 3a2f 2f67 6974  See: https://git
-0000dad0: 6875 622e 636f 6d2f 676f 6f67 6c65 6170  hub.com/googleap
-0000dae0: 6973 2f70 7974 686f 6e2d 7370 616e 6e65  is/python-spanne
-0000daf0: 722f 6973 7375 6573 2f33 3437 0a20 2020  r/issues/347.   
-0000db00: 2022 2222 0a0a 2020 2020 4070 7974 6573   """..    @pytes
-0000db10: 742e 6d61 726b 2e73 6b69 7028 0a20 2020  t.mark.skip(.   
-0000db20: 2020 2020 2022 5370 616e 6e65 7220 4442       "Spanner DB
-0000db30: 4150 4920 696e 636f 7272 6563 746c 7920  API incorrectly 
-0000db40: 636c 6173 7369 6679 2074 6865 2073 7461  classify the sta
-0000db50: 7465 6d65 6e74 2073 7461 7274 696e 6720  tement starting 
-0000db60: 7769 7468 2062 7261 636b 6574 732e 220a  with brackets.".
-0000db70: 2020 2020 290a 2020 2020 6465 6620 7465      ).    def te
-0000db80: 7374 5f6c 696d 6974 5f6f 6666 7365 745f  st_limit_offset_
-0000db90: 7365 6c65 6374 6162 6c65 5f69 6e5f 756e  selectable_in_un
-0000dba0: 696f 6e73 2873 656c 6629 3a0a 2020 2020  ions(self):.    
-0000dbb0: 2020 2020 7061 7373 0a0a 2020 2020 4070      pass..    @p
-0000dbc0: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
-0000dbd0: 0a20 2020 2020 2020 2022 5370 616e 6e65  .        "Spanne
-0000dbe0: 7220 4442 4150 4920 696e 636f 7272 6563  r DBAPI incorrec
-0000dbf0: 746c 7920 636c 6173 7369 6679 2074 6865  tly classify the
-0000dc00: 2073 7461 7465 6d65 6e74 2073 7461 7274   statement start
-0000dc10: 696e 6720 7769 7468 2062 7261 636b 6574  ing with bracket
-0000dc20: 732e 220a 2020 2020 290a 2020 2020 6465  s.".    ).    de
-0000dc30: 6620 7465 7374 5f6f 7264 6572 5f62 795f  f test_order_by_
-0000dc40: 7365 6c65 6374 6162 6c65 5f69 6e5f 756e  selectable_in_un
-0000dc50: 696f 6e73 2873 656c 6629 3a0a 2020 2020  ions(self):.    
-0000dc60: 2020 2020 7061 7373 0a0a 0a63 6c61 7373      pass...class
-0000dc70: 2054 6573 7451 7565 7279 4869 6e74 7328   TestQueryHints(
-0000dc80: 6669 7874 7572 6573 2e54 6162 6c65 7354  fixtures.TablesT
-0000dc90: 6573 7429 3a0a 2020 2020 2222 220a 2020  est):.    """.  
-0000dca0: 2020 436f 6d70 696c 6520 6120 636f 6d70    Compile a comp
-0000dcb0: 6c65 7820 7175 6572 7920 7769 7468 204a  lex query with J
-0000dcc0: 4f49 4e20 616e 6420 6368 6563 6b20 7468  OIN and check th
-0000dcd0: 6174 0a20 2020 2074 6865 2074 6162 6c65  at.    the table
-0000dce0: 2068 696e 7420 7761 7320 7365 7420 696e   hint was set in
-0000dcf0: 746f 2074 6865 2072 6967 6874 2070 6c61  to the right pla
-0000dd00: 6365 2e0a 2020 2020 2222 220a 0a20 2020  ce..    """..   
-0000dd10: 205f 5f62 6163 6b65 6e64 5f5f 203d 2054   __backend__ = T
-0000dd20: 7275 650a 0a20 2020 2064 6566 2074 6573  rue..    def tes
-0000dd30: 745f 636f 6d70 6c65 785f 7175 6572 795f  t_complex_query_
-0000dd40: 7461 626c 655f 6869 6e74 7328 7365 6c66  table_hints(self
-0000dd50: 293a 0a20 2020 2020 2020 2045 5850 4543  ):.        EXPEC
-0000dd60: 5445 445f 5155 4552 5920 3d20 280a 2020  TED_QUERY = (.  
-0000dd70: 2020 2020 2020 2020 2020 2253 454c 4543            "SELEC
-0000dd80: 5420 7573 6572 732e 6964 2c20 7573 6572  T users.id, user
-0000dd90: 732e 6e61 6d65 205c 6e46 524f 4d20 7573  s.name \nFROM us
-0000dda0: 6572 7320 407b 464f 5243 455f 494e 4445  ers @{FORCE_INDE
-0000ddb0: 583d 7461 626c 655f 315f 6279 5f69 6e74  X=table_1_by_int
-0000ddc0: 5f69 6478 7d22 0a20 2020 2020 2020 2020  _idx}".         
-0000ddd0: 2020 2022 204a 4f49 4e20 6164 6472 6573     " JOIN addres
-0000dde0: 7365 7320 4f4e 2075 7365 7273 2e69 6420  ses ON users.id 
-0000ddf0: 3d20 6164 6472 6573 7365 732e 7573 6572  = addresses.user
-0000de00: 5f69 6420 220a 2020 2020 2020 2020 2020  _id ".          
-0000de10: 2020 225c 6e57 4845 5245 2075 7365 7273    "\nWHERE users
-0000de20: 2e6e 616d 6520 494e 2028 5f5f 5b50 4f53  .name IN (__[POS
-0000de30: 5443 4f4d 5049 4c45 5f6e 616d 655f 315d  TCOMPILE_name_1]
-0000de40: 2922 0a20 2020 2020 2020 2029 0a0a 2020  )".        )..  
-0000de50: 2020 2020 2020 4261 7365 203d 2064 6563        Base = dec
-0000de60: 6c61 7261 7469 7665 5f62 6173 6528 290a  larative_base().
-0000de70: 2020 2020 2020 2020 656e 6769 6e65 203d          engine =
-0000de80: 2063 7265 6174 655f 656e 6769 6e65 280a   create_engine(.
-0000de90: 2020 2020 2020 2020 2020 2020 2273 7061              "spa
-0000dea0: 6e6e 6572 3a2f 2f2f 7072 6f6a 6563 7473  nner:///projects
-0000deb0: 2f70 726f 6a65 6374 2d69 642f 696e 7374  /project-id/inst
-0000dec0: 616e 6365 732f 696e 7374 616e 6365 2d69  ances/instance-i
-0000ded0: 642f 6461 7461 6261 7365 732f 6461 7461  d/databases/data
-0000dee0: 6261 7365 2d69 6422 0a20 2020 2020 2020  base-id".       
-0000def0: 2029 0a0a 2020 2020 2020 2020 636c 6173   )..        clas
-0000df00: 7320 5573 6572 2842 6173 6529 3a0a 2020  s User(Base):.  
-0000df10: 2020 2020 2020 2020 2020 5f5f 7461 626c            __tabl
-0000df20: 656e 616d 655f 5f20 3d20 2275 7365 7273  ename__ = "users
-0000df30: 220a 2020 2020 2020 2020 2020 2020 6964  ".            id
-0000df40: 203d 2043 6f6c 756d 6e28 496e 7465 6765   = Column(Intege
-0000df50: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
-0000df60: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-0000df70: 206e 616d 6520 3d20 436f 6c75 6d6e 2853   name = Column(S
-0000df80: 7472 696e 6728 3530 2929 0a20 2020 2020  tring(50)).     
-0000df90: 2020 2020 2020 2061 6464 7265 7373 6573         addresses
-0000dfa0: 203d 2072 656c 6174 696f 6e28 2241 6464   = relation("Add
-0000dfb0: 7265 7373 222c 2062 6163 6b72 6566 3d22  ress", backref="
-0000dfc0: 7573 6572 2229 0a0a 2020 2020 2020 2020  user")..        
-0000dfd0: 636c 6173 7320 4164 6472 6573 7328 4261  class Address(Ba
-0000dfe0: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
-0000dff0: 205f 5f74 6162 6c65 6e61 6d65 5f5f 203d   __tablename__ =
-0000e000: 2022 6164 6472 6573 7365 7322 0a20 2020   "addresses".   
-0000e010: 2020 2020 2020 2020 2069 6420 3d20 436f           id = Co
-0000e020: 6c75 6d6e 2849 6e74 6567 6572 2c20 7072  lumn(Integer, pr
-0000e030: 696d 6172 795f 6b65 793d 5472 7565 290a  imary_key=True).
-0000e040: 2020 2020 2020 2020 2020 2020 656d 6169              emai
-0000e050: 6c20 3d20 436f 6c75 6d6e 2853 7472 696e  l = Column(Strin
-0000e060: 6728 3530 2929 0a20 2020 2020 2020 2020  g(50)).         
-0000e070: 2020 2075 7365 725f 6964 203d 2043 6f6c     user_id = Col
-0000e080: 756d 6e28 496e 7465 6765 722c 2046 6f72  umn(Integer, For
-0000e090: 6569 676e 4b65 7928 2275 7365 7273 2e69  eignKey("users.i
-0000e0a0: 6422 2929 0a0a 2020 2020 2020 2020 7365  d"))..        se
-0000e0b0: 7373 696f 6e20 3d20 5365 7373 696f 6e28  ssion = Session(
-0000e0c0: 656e 6769 6e65 290a 0a20 2020 2020 2020  engine)..       
-0000e0d0: 2071 7565 7279 203d 2073 6573 7369 6f6e   query = session
-0000e0e0: 2e71 7565 7279 2855 7365 7229 0a20 2020  .query(User).   
-0000e0f0: 2020 2020 2071 7565 7279 203d 2071 7565       query = que
-0000e100: 7279 2e77 6974 685f 6869 6e74 280a 2020  ry.with_hint(.  
-0000e110: 2020 2020 2020 2020 2020 7365 6c65 6374            select
-0000e120: 6162 6c65 3d55 7365 722c 2074 6578 743d  able=User, text=
-0000e130: 2240 7b46 4f52 4345 5f49 4e44 4558 3d74  "@{FORCE_INDEX=t
-0000e140: 6162 6c65 5f31 5f62 795f 696e 745f 6964  able_1_by_int_id
-0000e150: 787d 220a 2020 2020 2020 2020 290a 0a20  x}".        ).. 
-0000e160: 2020 2020 2020 2071 7565 7279 203d 2071         query = q
-0000e170: 7565 7279 2e66 696c 7465 7228 5573 6572  uery.filter(User
-0000e180: 2e6e 616d 652e 696e 5f28 5b22 7661 6c31  .name.in_(["val1
-0000e190: 222c 2022 7661 6c32 225d 2929 0a20 2020  ", "val2"])).   
-0000e1a0: 2020 2020 2071 7565 7279 203d 2071 7565       query = que
-0000e1b0: 7279 2e6a 6f69 6e28 4164 6472 6573 7329  ry.join(Address)
-0000e1c0: 0a0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-0000e1d0: 2073 7472 2871 7565 7279 2e73 7461 7465   str(query.state
-0000e1e0: 6d65 6e74 2e63 6f6d 7069 6c65 2873 6573  ment.compile(ses
-0000e1f0: 7369 6f6e 2e62 696e 6429 2920 3d3d 2045  sion.bind)) == E
-0000e200: 5850 4543 5445 445f 5155 4552 590a 0a0a  XPECTED_QUERY...
-0000e210: 636c 6173 7320 496e 7465 726c 6561 7665  class Interleave
-0000e220: 6454 6162 6c65 7354 6573 7428 6669 7874  dTablesTest(fixt
-0000e230: 7572 6573 2e54 6573 7442 6173 6529 3a0a  ures.TestBase):.
-0000e240: 2020 2020 2222 220a 2020 2020 4368 6563      """.    Chec
-0000e250: 6b20 7468 6174 2043 5245 4154 4520 5441  k that CREATE TA
-0000e260: 424c 4520 7374 6174 656d 656e 7473 2066  BLE statements f
-0000e270: 6f72 2069 6e74 6572 6c65 6176 6564 2074  or interleaved t
-0000e280: 6162 6c65 7320 6172 6520 636f 7272 6563  ables are correc
-0000e290: 746c 790a 2020 2020 6765 6e65 7261 7465  tly.    generate
-0000e2a0: 642e 0a20 2020 2022 2222 0a0a 2020 2020  d..    """..    
-0000e2b0: 6465 6620 7365 7455 7028 7365 6c66 293a  def setUp(self):
-0000e2c0: 0a20 2020 2020 2020 2073 656c 662e 5f65  .        self._e
-0000e2d0: 6e67 696e 6520 3d20 6372 6561 7465 5f65  ngine = create_e
-0000e2e0: 6e67 696e 6528 0a20 2020 2020 2020 2020  ngine(.         
-0000e2f0: 2020 2022 7370 616e 6e65 723a 2f2f 2f70     "spanner:///p
-0000e300: 726f 6a65 6374 732f 6170 7064 6576 2d73  rojects/appdev-s
-0000e310: 6f64 612d 7370 616e 6e65 722d 7374 6167  oda-spanner-stag
-0000e320: 696e 672f 696e 7374 616e 6365 732f 220a  ing/instances/".
-0000e330: 2020 2020 2020 2020 2020 2020 2273 716c              "sql
-0000e340: 616c 6368 656d 792d 6469 616c 6563 742d  alchemy-dialect-
-0000e350: 7465 7374 2f64 6174 6162 6173 6573 2f63  test/databases/c
-0000e360: 6f6d 706c 6961 6e63 652d 7465 7374 220a  ompliance-test".
-0000e370: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000e380: 2020 7365 6c66 2e5f 6d65 7461 6461 7461    self._metadata
-0000e390: 203d 204d 6574 6144 6174 6128 6269 6e64   = MetaData(bind
-0000e3a0: 3d73 656c 662e 5f65 6e67 696e 6529 0a0a  =self._engine)..
-0000e3b0: 2020 2020 6465 6620 7465 7374 5f69 6e74      def test_int
-0000e3c0: 6572 6c65 6176 6528 7365 6c66 293a 0a20  erleave(self):. 
-0000e3d0: 2020 2020 2020 2045 5850 5f51 5545 5259         EXP_QUERY
-0000e3e0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-0000e3f0: 2022 5c6e 4352 4541 5445 2054 4142 4c45   "\nCREATE TABLE
-0000e400: 2063 6c69 656e 7420 285c 6e5c 7474 6561   client (\n\ttea
-0000e410: 6d5f 6964 2049 4e54 3634 204e 4f54 204e  m_id INT64 NOT N
-0000e420: 554c 4c2c 2022 0a20 2020 2020 2020 2020  ULL, ".         
-0000e430: 2020 2022 5c6e 5c74 636c 6965 6e74 5f69     "\n\tclient_i
-0000e440: 6420 494e 5436 3420 4e4f 5420 4e55 4c4c  d INT64 NOT NULL
-0000e450: 2c20 220a 2020 2020 2020 2020 2020 2020  , ".            
-0000e460: 225c 6e5c 7463 6c69 656e 745f 6e61 6d65  "\n\tclient_name
-0000e470: 2053 5452 494e 4728 3136 2920 4e4f 5420   STRING(16) NOT 
-0000e480: 4e55 4c4c 220a 2020 2020 2020 2020 2020  NULL".          
-0000e490: 2020 225c 6e29 2050 5249 4d41 5259 204b    "\n) PRIMARY K
-0000e4a0: 4559 2028 7465 616d 5f69 642c 2063 6c69  EY (team_id, cli
-0000e4b0: 656e 745f 6964 292c 220a 2020 2020 2020  ent_id),".      
-0000e4c0: 2020 2020 2020 225c 6e49 4e54 4552 4c45        "\nINTERLE
-0000e4d0: 4156 4520 494e 2050 4152 454e 5420 7465  AVE IN PARENT te
-0000e4e0: 616d 5c6e 5c6e 220a 2020 2020 2020 2020  am\n\n".        
-0000e4f0: 290a 2020 2020 2020 2020 636c 6965 6e74  ).        client
-0000e500: 203d 2054 6162 6c65 280a 2020 2020 2020   = Table(.      
-0000e510: 2020 2020 2020 2263 6c69 656e 7422 2c0a        "client",.
-0000e520: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e530: 2e5f 6d65 7461 6461 7461 2c0a 2020 2020  ._metadata,.    
-0000e540: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-0000e550: 7465 616d 5f69 6422 2c20 496e 7465 6765  team_id", Intege
-0000e560: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
-0000e570: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
-0000e580: 2020 436f 6c75 6d6e 2822 636c 6965 6e74    Column("client
-0000e590: 5f69 6422 2c20 496e 7465 6765 722c 2070  _id", Integer, p
-0000e5a0: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
-0000e5b0: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
-0000e5c0: 6c75 6d6e 2822 636c 6965 6e74 5f6e 616d  lumn("client_nam
-0000e5d0: 6522 2c20 5374 7269 6e67 2831 3629 2c20  e", String(16), 
-0000e5e0: 6e75 6c6c 6162 6c65 3d46 616c 7365 292c  nullable=False),
-0000e5f0: 0a20 2020 2020 2020 2020 2020 2073 7061  .            spa
-0000e600: 6e6e 6572 5f69 6e74 6572 6c65 6176 655f  nner_interleave_
-0000e610: 696e 3d22 7465 616d 222c 0a20 2020 2020  in="team",.     
-0000e620: 2020 2029 0a20 2020 2020 2020 2077 6974     ).        wit
-0000e630: 6820 6d6f 636b 2e70 6174 6368 2822 676f  h mock.patch("go
-0000e640: 6f67 6c65 2e63 6c6f 7564 2e73 7061 6e6e  ogle.cloud.spann
-0000e650: 6572 5f64 6261 7069 2e63 7572 736f 722e  er_dbapi.cursor.
-0000e660: 4375 7273 6f72 2e65 7865 6375 7465 2229  Cursor.execute")
-0000e670: 2061 7320 6578 6563 7574 653a 0a20 2020   as execute:.   
-0000e680: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
-0000e690: 6372 6561 7465 2873 656c 662e 5f65 6e67  create(self._eng
-0000e6a0: 696e 6529 0a20 2020 2020 2020 2020 2020  ine).           
-0000e6b0: 2065 7865 6375 7465 2e61 7373 6572 745f   execute.assert_
-0000e6c0: 6361 6c6c 6564 5f6f 6e63 655f 7769 7468  called_once_with
-0000e6d0: 2845 5850 5f51 5545 5259 2c20 5b5d 290a  (EXP_QUERY, []).
-0000e6e0: 0a20 2020 2064 6566 2074 6573 745f 696e  .    def test_in
-0000e6f0: 7465 726c 6561 7665 5f6f 6e5f 6465 6c65  terleave_on_dele
-0000e700: 7465 5f63 6173 6361 6465 2873 656c 6629  te_cascade(self)
-0000e710: 3a0a 2020 2020 2020 2020 4558 505f 5155  :.        EXP_QU
-0000e720: 4552 5920 3d20 280a 2020 2020 2020 2020  ERY = (.        
-0000e730: 2020 2020 225c 6e43 5245 4154 4520 5441      "\nCREATE TA
-0000e740: 424c 4520 636c 6965 6e74 2028 5c6e 5c74  BLE client (\n\t
-0000e750: 7465 616d 5f69 6420 494e 5436 3420 4e4f  team_id INT64 NO
-0000e760: 5420 4e55 4c4c 2c20 220a 2020 2020 2020  T NULL, ".      
-0000e770: 2020 2020 2020 225c 6e5c 7463 6c69 656e        "\n\tclien
-0000e780: 745f 6964 2049 4e54 3634 204e 4f54 204e  t_id INT64 NOT N
-0000e790: 554c 4c2c 2022 0a20 2020 2020 2020 2020  ULL, ".         
-0000e7a0: 2020 2022 5c6e 5c74 636c 6965 6e74 5f6e     "\n\tclient_n
-0000e7b0: 616d 6520 5354 5249 4e47 2831 3629 204e  ame STRING(16) N
-0000e7c0: 4f54 204e 554c 4c22 0a20 2020 2020 2020  OT NULL".       
-0000e7d0: 2020 2020 2022 5c6e 2920 5052 494d 4152       "\n) PRIMAR
-0000e7e0: 5920 4b45 5920 2874 6561 6d5f 6964 2c20  Y KEY (team_id, 
-0000e7f0: 636c 6965 6e74 5f69 6429 2c22 0a20 2020  client_id),".   
-0000e800: 2020 2020 2020 2020 2022 5c6e 494e 5445           "\nINTE
-0000e810: 524c 4541 5645 2049 4e20 5041 5245 4e54  RLEAVE IN PARENT
-0000e820: 2074 6561 6d20 4f4e 2044 454c 4554 4520   team ON DELETE 
-0000e830: 4341 5343 4144 455c 6e5c 6e22 0a20 2020  CASCADE\n\n".   
-0000e840: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
-0000e850: 6c69 656e 7420 3d20 5461 626c 6528 0a20  lient = Table(. 
-0000e860: 2020 2020 2020 2020 2020 2022 636c 6965             "clie
-0000e870: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
-0000e880: 2073 656c 662e 5f6d 6574 6164 6174 612c   self._metadata,
-0000e890: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-0000e8a0: 756d 6e28 2274 6561 6d5f 6964 222c 2049  umn("team_id", I
-0000e8b0: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
-0000e8c0: 6b65 793d 5472 7565 292c 0a20 2020 2020  key=True),.     
-0000e8d0: 2020 2020 2020 2043 6f6c 756d 6e28 2263         Column("c
-0000e8e0: 6c69 656e 745f 6964 222c 2049 6e74 6567  lient_id", Integ
-0000e8f0: 6572 2c20 7072 696d 6172 795f 6b65 793d  er, primary_key=
-0000e900: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-0000e910: 2020 2043 6f6c 756d 6e28 2263 6c69 656e     Column("clien
-0000e920: 745f 6e61 6d65 222c 2053 7472 696e 6728  t_name", String(
-0000e930: 3136 292c 206e 756c 6c61 626c 653d 4661  16), nullable=Fa
-0000e940: 6c73 6529 2c0a 2020 2020 2020 2020 2020  lse),.          
-0000e950: 2020 7370 616e 6e65 725f 696e 7465 726c    spanner_interl
-0000e960: 6561 7665 5f69 6e3d 2274 6561 6d22 2c0a  eave_in="team",.
-0000e970: 2020 2020 2020 2020 2020 2020 7370 616e              span
-0000e980: 6e65 725f 696e 7465 726c 6561 7665 5f6f  ner_interleave_o
-0000e990: 6e5f 6465 6c65 7465 5f63 6173 6361 6465  n_delete_cascade
-0000e9a0: 3d54 7275 652c 0a20 2020 2020 2020 2029  =True,.        )
-0000e9b0: 0a20 2020 2020 2020 2077 6974 6820 6d6f  .        with mo
-0000e9c0: 636b 2e70 6174 6368 2822 676f 6f67 6c65  ck.patch("google
-0000e9d0: 2e63 6c6f 7564 2e73 7061 6e6e 6572 5f64  .cloud.spanner_d
-0000e9e0: 6261 7069 2e63 7572 736f 722e 4375 7273  bapi.cursor.Curs
-0000e9f0: 6f72 2e65 7865 6375 7465 2229 2061 7320  or.execute") as 
-0000ea00: 6578 6563 7574 653a 0a20 2020 2020 2020  execute:.       
-0000ea10: 2020 2020 2063 6c69 656e 742e 6372 6561       client.crea
-0000ea20: 7465 2873 656c 662e 5f65 6e67 696e 6529  te(self._engine)
-0000ea30: 0a20 2020 2020 2020 2020 2020 2065 7865  .            exe
-0000ea40: 6375 7465 2e61 7373 6572 745f 6361 6c6c  cute.assert_call
-0000ea50: 6564 5f6f 6e63 655f 7769 7468 2845 5850  ed_once_with(EXP
-0000ea60: 5f51 5545 5259 2c20 5b5d 290a 0a0a 636c  _QUERY, [])...cl
-0000ea70: 6173 7320 5573 6572 4167 656e 7454 6573  ass UserAgentTes
-0000ea80: 7428 6669 7874 7572 6573 2e54 6573 7442  t(fixtures.TestB
-0000ea90: 6173 6529 3a0a 2020 2020 2222 2243 6865  ase):.    """Che
-0000eaa0: 636b 2074 6861 7420 5351 4c41 6c63 6865  ck that SQLAlche
-0000eab0: 6d79 2064 6961 6c65 6374 2075 7365 7320  my dialect uses 
-0000eac0: 636f 7272 6563 7420 7573 6572 2061 6765  correct user age
-0000ead0: 6e74 2e22 2222 0a0a 2020 2020 6465 6620  nt."""..    def 
-0000eae0: 7365 7455 7028 7365 6c66 293a 0a20 2020  setUp(self):.   
-0000eaf0: 2020 2020 2073 656c 662e 5f65 6e67 696e       self._engin
-0000eb00: 6520 3d20 6372 6561 7465 5f65 6e67 696e  e = create_engin
-0000eb10: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
-0000eb20: 7370 616e 6e65 723a 2f2f 2f70 726f 6a65  spanner:///proje
-0000eb30: 6374 732f 6170 7064 6576 2d73 6f64 612d  cts/appdev-soda-
-0000eb40: 7370 616e 6e65 722d 7374 6167 696e 672f  spanner-staging/
-0000eb50: 696e 7374 616e 6365 732f 220a 2020 2020  instances/".    
-0000eb60: 2020 2020 2020 2020 2273 716c 616c 6368          "sqlalch
-0000eb70: 656d 792d 6469 616c 6563 742d 7465 7374  emy-dialect-test
-0000eb80: 2f64 6174 6162 6173 6573 2f63 6f6d 706c  /databases/compl
-0000eb90: 6961 6e63 652d 7465 7374 220a 2020 2020  iance-test".    
-0000eba0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-0000ebb0: 6c66 2e5f 6d65 7461 6461 7461 203d 204d  lf._metadata = M
-0000ebc0: 6574 6144 6174 6128 6269 6e64 3d73 656c  etaData(bind=sel
-0000ebd0: 662e 5f65 6e67 696e 6529 0a0a 2020 2020  f._engine)..    
-0000ebe0: 6465 6620 7465 7374 5f75 7365 725f 6167  def test_user_ag
-0000ebf0: 656e 7428 7365 6c66 293a 0a20 2020 2020  ent(self):.     
-0000ec00: 2020 2064 6973 7420 3d20 706b 675f 7265     dist = pkg_re
-0000ec10: 736f 7572 6365 732e 6765 745f 6469 7374  sources.get_dist
-0000ec20: 7269 6275 7469 6f6e 2822 7371 6c61 6c63  ribution("sqlalc
-0000ec30: 6865 6d79 2d73 7061 6e6e 6572 2229 0a0a  hemy-spanner")..
-0000ec40: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0000ec50: 662e 5f65 6e67 696e 652e 636f 6e6e 6563  f._engine.connec
-0000ec60: 7428 2920 6173 2063 6f6e 6e65 6374 696f  t() as connectio
-0000ec70: 6e3a 0a20 2020 2020 2020 2020 2020 2061  n:.            a
-0000ec80: 7373 6572 7420 280a 2020 2020 2020 2020  ssert (.        
-0000ec90: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
-0000eca0: 6f6e 2e63 6f6e 6e65 6374 696f 6e2e 696e  on.connection.in
-0000ecb0: 7374 616e 6365 2e5f 636c 6965 6e74 2e5f  stance._client._
-0000ecc0: 636c 6965 6e74 5f69 6e66 6f2e 7573 6572  client_info.user
-0000ecd0: 5f61 6765 6e74 0a20 2020 2020 2020 2020  _agent.         
-0000ece0: 2020 2020 2020 203d 3d20 2267 6c2d 2220         == "gl-" 
-0000ecf0: 2b20 6469 7374 2e70 726f 6a65 6374 5f6e  + dist.project_n
-0000ed00: 616d 6520 2b20 222f 2220 2b20 6469 7374  ame + "/" + dist
-0000ed10: 2e76 6572 7369 6f6e 0a20 2020 2020 2020  .version.       
-0000ed20: 2020 2020 2029 0a0a 0a63 6c61 7373 2053       )...class S
-0000ed30: 696d 706c 6555 7064 6174 6544 656c 6574  impleUpdateDelet
-0000ed40: 6554 6573 7428 5f53 696d 706c 6555 7064  eTest(_SimpleUpd
-0000ed50: 6174 6544 656c 6574 6554 6573 7429 3a0a  ateDeleteTest):.
-0000ed60: 2020 2020 2222 220a 2020 2020 5350 414e      """.    SPAN
-0000ed70: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
-0000ed80: 2020 2053 7061 6e6e 6572 2064 6f65 736e     Spanner doesn
-0000ed90: 2774 2073 7570 706f 7274 2060 726f 7763  't support `rowc
-0000eda0: 6f75 6e74 6020 7072 6f70 6572 7479 2e20  ount` property. 
-0000edb0: 5468 6573 650a 2020 2020 7465 7374 2063  These.    test c
-0000edc0: 6173 6573 206f 7665 7272 6964 6573 206f  ases overrides o
-0000edd0: 6d69 7420 6072 6f77 636f 756e 7460 2063  mit `rowcount` c
-0000ede0: 6865 636b 732e 0a20 2020 2022 2222 0a0a  hecks..    """..
-0000edf0: 2020 2020 6465 6620 7465 7374 5f64 656c      def test_del
-0000ee00: 6574 6528 7365 6c66 2c20 636f 6e6e 6563  ete(self, connec
-0000ee10: 7469 6f6e 293a 0a20 2020 2020 2020 2074  tion):.        t
-0000ee20: 203d 2073 656c 662e 7461 626c 6573 2e70   = self.tables.p
-0000ee30: 6c61 696e 5f70 6b0a 2020 2020 2020 2020  lain_pk.        
-0000ee40: 7220 3d20 636f 6e6e 6563 7469 6f6e 2e65  r = connection.e
-0000ee50: 7865 6375 7465 2874 2e64 656c 6574 6528  xecute(t.delete(
-0000ee60: 292e 7768 6572 6528 742e 632e 6964 203d  ).where(t.c.id =
-0000ee70: 3d20 3229 290a 2020 2020 2020 2020 6173  = 2)).        as
-0000ee80: 7365 7274 206e 6f74 2072 2e69 735f 696e  sert not r.is_in
-0000ee90: 7365 7274 0a20 2020 2020 2020 2061 7373  sert.        ass
-0000eea0: 6572 7420 6e6f 7420 722e 7265 7475 726e  ert not r.return
-0000eeb0: 735f 726f 7773 0a20 2020 2020 2020 2065  s_rows.        e
-0000eec0: 715f 280a 2020 2020 2020 2020 2020 2020  q_(.            
-0000eed0: 636f 6e6e 6563 7469 6f6e 2e65 7865 6375  connection.execu
-0000eee0: 7465 2874 2e73 656c 6563 7428 292e 6f72  te(t.select().or
-0000eef0: 6465 725f 6279 2874 2e63 2e69 6429 292e  der_by(t.c.id)).
-0000ef00: 6665 7463 6861 6c6c 2829 2c0a 2020 2020  fetchall(),.    
-0000ef10: 2020 2020 2020 2020 5b28 312c 2022 6431          [(1, "d1
-0000ef20: 2229 2c20 2833 2c20 2264 3322 295d 2c0a  "), (3, "d3")],.
-0000ef30: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-0000ef40: 6566 2074 6573 745f 7570 6461 7465 2873  ef test_update(s
-0000ef50: 656c 662c 2063 6f6e 6e65 6374 696f 6e29  elf, connection)
-0000ef60: 3a0a 2020 2020 2020 2020 7420 3d20 7365  :.        t = se
-0000ef70: 6c66 2e74 6162 6c65 732e 706c 6169 6e5f  lf.tables.plain_
-0000ef80: 706b 0a20 2020 2020 2020 2072 203d 2063  pk.        r = c
-0000ef90: 6f6e 6e65 6374 696f 6e2e 6578 6563 7574  onnection.execut
-0000efa0: 6528 742e 7570 6461 7465 2829 2e77 6865  e(t.update().whe
-0000efb0: 7265 2874 2e63 2e69 6420 3d3d 2032 292c  re(t.c.id == 2),
-0000efc0: 2064 6963 7428 6461 7461 3d22 6432 5f6e   dict(data="d2_n
-0000efd0: 6577 2229 290a 2020 2020 2020 2020 6173  ew")).        as
-0000efe0: 7365 7274 206e 6f74 2072 2e69 735f 696e  sert not r.is_in
-0000eff0: 7365 7274 0a20 2020 2020 2020 2061 7373  sert.        ass
-0000f000: 6572 7420 6e6f 7420 722e 7265 7475 726e  ert not r.return
-0000f010: 735f 726f 7773 0a0a 2020 2020 2020 2020  s_rows..        
-0000f020: 6571 5f28 0a20 2020 2020 2020 2020 2020  eq_(.           
-0000f030: 2063 6f6e 6e65 6374 696f 6e2e 6578 6563   connection.exec
-0000f040: 7574 6528 742e 7365 6c65 6374 2829 2e6f  ute(t.select().o
-0000f050: 7264 6572 5f62 7928 742e 632e 6964 2929  rder_by(t.c.id))
-0000f060: 2e66 6574 6368 616c 6c28 292c 0a20 2020  .fetchall(),.   
-0000f070: 2020 2020 2020 2020 205b 2831 2c20 2264           [(1, "d
-0000f080: 3122 292c 2028 322c 2022 6432 5f6e 6577  1"), (2, "d2_new
-0000f090: 2229 2c20 2833 2c20 2264 3322 295d 2c0a  "), (3, "d3")],.
-0000f0a0: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
-0000f0b0: 7320 4861 7349 6e64 6578 5465 7374 285f  s HasIndexTest(_
-0000f0c0: 4861 7349 6e64 6578 5465 7374 293a 0a20  HasIndexTest):. 
-0000f0d0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-0000f0e0: 2020 2020 6465 6620 6465 6669 6e65 5f74      def define_t
-0000f0f0: 6162 6c65 7328 636c 732c 206d 6574 6164  ables(cls, metad
-0000f100: 6174 6129 3a0a 2020 2020 2020 2020 7474  ata):.        tt
-0000f110: 203d 2054 6162 6c65 280a 2020 2020 2020   = Table(.      
-0000f120: 2020 2020 2020 2274 6573 745f 7461 626c        "test_tabl
-0000f130: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-0000f140: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
-0000f150: 2020 2020 2020 436f 6c75 6d6e 2822 6964        Column("id
-0000f160: 222c 2049 6e74 6567 6572 2c20 7072 696d  ", Integer, prim
-0000f170: 6172 795f 6b65 793d 5472 7565 292c 0a20  ary_key=True),. 
-0000f180: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
-0000f190: 6e28 2264 6174 6122 2c20 5374 7269 6e67  n("data", String
-0000f1a0: 2835 3029 292c 0a20 2020 2020 2020 2029  (50)),.        )
-0000f1b0: 0a20 2020 2020 2020 2073 716c 616c 6368  .        sqlalch
-0000f1c0: 656d 792e 496e 6465 7828 226d 795f 6964  emy.Index("my_id
-0000f1d0: 7822 2c20 7474 2e63 2e64 6174 6129 0a0a  x", tt.c.data)..
-0000f1e0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-0000f1f0: 2e73 6b69 7028 224e 6f74 2073 7570 706f  .skip("Not suppo
-0000f200: 7274 6564 2062 7920 436c 6f75 6420 5370  rted by Cloud Sp
-0000f210: 616e 6e65 7222 290a 2020 2020 6465 6620  anner").    def 
-0000f220: 7465 7374 5f68 6173 5f69 6e64 6578 5f73  test_has_index_s
-0000f230: 6368 656d 6128 7365 6c66 293a 0a20 2020  chema(self):.   
-0000f240: 2020 2020 2070 6173 730a 0a0a 636c 6173       pass...clas
-0000f250: 7320 4861 7354 6162 6c65 5465 7374 285f  s HasTableTest(_
-0000f260: 4861 7354 6162 6c65 5465 7374 293a 0a20  HasTableTest):. 
-0000f270: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-0000f280: 2020 2020 6465 6620 6465 6669 6e65 5f74      def define_t
-0000f290: 6162 6c65 7328 636c 732c 206d 6574 6164  ables(cls, metad
-0000f2a0: 6174 6129 3a0a 2020 2020 2020 2020 5461  ata):.        Ta
-0000f2b0: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
-0000f2c0: 2022 7465 7374 5f74 6162 6c65 222c 0a20   "test_table",. 
-0000f2d0: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-0000f2e0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-0000f2f0: 2043 6f6c 756d 6e28 2269 6422 2c20 496e   Column("id", In
-0000f300: 7465 6765 722c 2070 7269 6d61 7279 5f6b  teger, primary_k
-0000f310: 6579 3d54 7275 6529 2c0a 2020 2020 2020  ey=True),.      
-0000f320: 2020 2020 2020 436f 6c75 6d6e 2822 6461        Column("da
-0000f330: 7461 222c 2053 7472 696e 6728 3530 2929  ta", String(50))
-0000f340: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0000f350: 2040 7079 7465 7374 2e6d 6172 6b2e 736b   @pytest.mark.sk
-0000f360: 6970 2822 4e6f 7420 7375 7070 6f72 7465  ip("Not supporte
-0000f370: 6420 6279 2043 6c6f 7564 2053 7061 6e6e  d by Cloud Spann
-0000f380: 6572 2229 0a20 2020 2064 6566 2074 6573  er").    def tes
-0000f390: 745f 6861 735f 7461 626c 655f 7363 6865  t_has_table_sche
-0000f3a0: 6d61 2873 656c 6629 3a0a 2020 2020 2020  ma(self):.      
-0000f3b0: 2020 7061 7373 0a0a 0a63 6c61 7373 2050    pass...class P
-0000f3c0: 6f73 7443 6f6d 7069 6c65 5061 7261 6d73  ostCompileParams
-0000f3d0: 5465 7374 285f 506f 7374 436f 6d70 696c  Test(_PostCompil
-0000f3e0: 6550 6172 616d 7354 6573 7429 3a0a 2020  eParamsTest):.  
-0000f3f0: 2020 6465 6620 7465 7374 5f65 7865 6375    def test_execu
-0000f400: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-0000f410: 2020 7461 626c 6520 3d20 7365 6c66 2e74    table = self.t
-0000f420: 6162 6c65 732e 736f 6d65 5f74 6162 6c65  ables.some_table
-0000f430: 0a0a 2020 2020 2020 2020 7374 6d74 203d  ..        stmt =
-0000f440: 2073 656c 6563 7428 7461 626c 652e 632e   select(table.c.
-0000f450: 6964 292e 7768 6572 6528 0a20 2020 2020  id).where(.     
-0000f460: 2020 2020 2020 2074 6162 6c65 2e63 2e78         table.c.x
-0000f470: 203d 3d20 7371 6c61 6c63 6865 6d79 2e62   == sqlalchemy.b
-0000f480: 696e 6470 6172 616d 2822 7122 2c20 6c69  indparam("q", li
-0000f490: 7465 7261 6c5f 6578 6563 7574 653d 5472  teral_execute=Tr
-0000f4a0: 7565 290a 2020 2020 2020 2020 290a 0a20  ue).        ).. 
-0000f4b0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000f4c0: 2e73 716c 5f65 7865 6375 7469 6f6e 5f61  .sql_execution_a
-0000f4d0: 7373 6572 7465 7228 2920 6173 2061 7373  sserter() as ass
-0000f4e0: 6572 7465 723a 0a20 2020 2020 2020 2020  erter:.         
-0000f4f0: 2020 2077 6974 6820 636f 6e66 6967 2e64     with config.d
-0000f500: 622e 636f 6e6e 6563 7428 2920 6173 2063  b.connect() as c
-0000f510: 6f6e 6e3a 0a20 2020 2020 2020 2020 2020  onn:.           
-0000f520: 2020 2020 2063 6f6e 6e2e 6578 6563 7574       conn.execut
-0000f530: 6528 7374 6d74 2c20 6469 6374 2871 3d31  e(stmt, dict(q=1
-0000f540: 3029 290a 0a20 2020 2020 2020 2061 7373  0))..        ass
-0000f550: 6572 7465 722e 6173 7365 7274 5f28 0a20  erter.assert_(. 
-0000f560: 2020 2020 2020 2020 2020 2073 716c 616c             sqlal
-0000f570: 6368 656d 792e 7465 7374 696e 672e 6173  chemy.testing.as
-0000f580: 7365 7274 7371 6c2e 4375 7273 6f72 5351  sertsql.CursorSQ
-0000f590: 4c28 0a20 2020 2020 2020 2020 2020 2020  L(.             
-0000f5a0: 2020 2022 5345 4c45 4354 2073 6f6d 655f     "SELECT some_
-0000f5b0: 7461 626c 652e 6964 205c 6e46 524f 4d20  table.id \nFROM 
-0000f5c0: 736f 6d65 5f74 6162 6c65 2022 2022 5c6e  some_table " "\n
-0000f5d0: 5748 4552 4520 736f 6d65 5f74 6162 6c65  WHERE some_table
-0000f5e0: 2e78 203d 2031 3022 2c0a 2020 2020 2020  .x = 10",.      
-0000f5f0: 2020 2020 2020 2020 2020 5b5d 2069 6620            [] if 
-0000f600: 636f 6e66 6967 2e64 622e 6469 616c 6563  config.db.dialec
-0000f610: 742e 706f 7369 7469 6f6e 616c 2065 6c73  t.positional els
-0000f620: 6520 7b7d 2c0a 2020 2020 2020 2020 2020  e {},.          
-0000f630: 2020 290a 2020 2020 2020 2020 290a 0a20    ).        ).. 
-0000f640: 2020 2064 6566 2074 6573 745f 6578 6563     def test_exec
-0000f650: 7574 655f 6578 7061 6e64 696e 675f 706c  ute_expanding_pl
-0000f660: 7573 5f6c 6974 6572 616c 5f65 7865 6375  us_literal_execu
-0000f670: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-0000f680: 2020 7461 626c 6520 3d20 7365 6c66 2e74    table = self.t
-0000f690: 6162 6c65 732e 736f 6d65 5f74 6162 6c65  ables.some_table
-0000f6a0: 0a0a 2020 2020 2020 2020 7374 6d74 203d  ..        stmt =
-0000f6b0: 2073 656c 6563 7428 7461 626c 652e 632e   select(table.c.
-0000f6c0: 6964 292e 7768 6572 6528 0a20 2020 2020  id).where(.     
-0000f6d0: 2020 2020 2020 2074 6162 6c65 2e63 2e78         table.c.x
-0000f6e0: 2e69 6e5f 280a 2020 2020 2020 2020 2020  .in_(.          
-0000f6f0: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
-0000f700: 2e62 696e 6470 6172 616d 2822 7122 2c20  .bindparam("q", 
-0000f710: 6578 7061 6e64 696e 673d 5472 7565 2c20  expanding=True, 
-0000f720: 6c69 7465 7261 6c5f 6578 6563 7574 653d  literal_execute=
-0000f730: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-0000f740: 2020 290a 2020 2020 2020 2020 290a 0a20    ).        ).. 
-0000f750: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000f760: 2e73 716c 5f65 7865 6375 7469 6f6e 5f61  .sql_execution_a
-0000f770: 7373 6572 7465 7228 2920 6173 2061 7373  sserter() as ass
-0000f780: 6572 7465 723a 0a20 2020 2020 2020 2020  erter:.         
-0000f790: 2020 2077 6974 6820 636f 6e66 6967 2e64     with config.d
-0000f7a0: 622e 636f 6e6e 6563 7428 2920 6173 2063  b.connect() as c
-0000f7b0: 6f6e 6e3a 0a20 2020 2020 2020 2020 2020  onn:.           
-0000f7c0: 2020 2020 2063 6f6e 6e2e 6578 6563 7574       conn.execut
-0000f7d0: 6528 7374 6d74 2c20 6469 6374 2871 3d5b  e(stmt, dict(q=[
-0000f7e0: 352c 2036 2c20 375d 2929 0a0a 2020 2020  5, 6, 7]))..    
-0000f7f0: 2020 2020 6173 7365 7274 6572 2e61 7373      asserter.ass
-0000f800: 6572 745f 280a 2020 2020 2020 2020 2020  ert_(.          
-0000f810: 2020 7371 6c61 6c63 6865 6d79 2e74 6573    sqlalchemy.tes
-0000f820: 7469 6e67 2e61 7373 6572 7473 716c 2e43  ting.assertsql.C
-0000f830: 7572 736f 7253 514c 280a 2020 2020 2020  ursorSQL(.      
-0000f840: 2020 2020 2020 2020 2020 2253 454c 4543            "SELEC
-0000f850: 5420 736f 6d65 5f74 6162 6c65 2e69 6420  T some_table.id 
-0000f860: 5c6e 4652 4f4d 2073 6f6d 655f 7461 626c  \nFROM some_tabl
-0000f870: 6520 220a 2020 2020 2020 2020 2020 2020  e ".            
-0000f880: 2020 2020 225c 6e57 4845 5245 2073 6f6d      "\nWHERE som
-0000f890: 655f 7461 626c 652e 7820 494e 2028 352c  e_table.x IN (5,
-0000f8a0: 2036 2c20 3729 222c 0a20 2020 2020 2020   6, 7)",.       
-0000f8b0: 2020 2020 2020 2020 205b 5d20 6966 2063           [] if c
-0000f8c0: 6f6e 6669 672e 6462 2e64 6961 6c65 6374  onfig.db.dialect
-0000f8d0: 2e70 6f73 6974 696f 6e61 6c20 656c 7365  .positional else
-0000f8e0: 207b 7d2c 0a20 2020 2020 2020 2020 2020   {},.           
-0000f8f0: 2029 0a20 2020 2020 2020 2029 0a0a 2020   ).        )..  
-0000f900: 2020 4074 6573 7469 6e67 2e72 6571 7569    @testing.requi
-0000f910: 7265 732e 7475 706c 655f 696e 0a20 2020  res.tuple_in.   
-0000f920: 2064 6566 2074 6573 745f 6578 6563 7574   def test_execut
-0000f930: 655f 7475 706c 655f 6578 7061 6e64 696e  e_tuple_expandin
-0000f940: 675f 706c 7573 5f6c 6974 6572 616c 5f65  g_plus_literal_e
-0000f950: 7865 6375 7465 2873 656c 6629 3a0a 2020  xecute(self):.  
-0000f960: 2020 2020 2020 7461 626c 6520 3d20 7365        table = se
-0000f970: 6c66 2e74 6162 6c65 732e 736f 6d65 5f74  lf.tables.some_t
-0000f980: 6162 6c65 0a0a 2020 2020 2020 2020 7374  able..        st
-0000f990: 6d74 203d 2073 656c 6563 7428 7461 626c  mt = select(tabl
-0000f9a0: 652e 632e 6964 292e 7768 6572 6528 0a20  e.c.id).where(. 
-0000f9b0: 2020 2020 2020 2020 2020 2073 716c 616c             sqlal
-0000f9c0: 6368 656d 792e 7475 706c 655f 2874 6162  chemy.tuple_(tab
-0000f9d0: 6c65 2e63 2e78 2c20 7461 626c 652e 632e  le.c.x, table.c.
-0000f9e0: 7929 2e69 6e5f 280a 2020 2020 2020 2020  y).in_(.        
-0000f9f0: 2020 2020 2020 2020 7371 6c61 6c63 6865          sqlalche
-0000fa00: 6d79 2e62 696e 6470 6172 616d 2822 7122  my.bindparam("q"
-0000fa10: 2c20 6578 7061 6e64 696e 673d 5472 7565  , expanding=True
-0000fa20: 2c20 6c69 7465 7261 6c5f 6578 6563 7574  , literal_execut
-0000fa30: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
-0000fa40: 2020 2020 290a 2020 2020 2020 2020 290a      ).        ).
-0000fa50: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000fa60: 6c66 2e73 716c 5f65 7865 6375 7469 6f6e  lf.sql_execution
-0000fa70: 5f61 7373 6572 7465 7228 2920 6173 2061  _asserter() as a
-0000fa80: 7373 6572 7465 723a 0a20 2020 2020 2020  sserter:.       
-0000fa90: 2020 2020 2077 6974 6820 636f 6e66 6967       with config
-0000faa0: 2e64 622e 636f 6e6e 6563 7428 2920 6173  .db.connect() as
-0000fab0: 2063 6f6e 6e3a 0a20 2020 2020 2020 2020   conn:.         
-0000fac0: 2020 2020 2020 2063 6f6e 6e2e 6578 6563         conn.exec
-0000fad0: 7574 6528 7374 6d74 2c20 6469 6374 2871  ute(stmt, dict(q
-0000fae0: 3d5b 2835 2c20 3130 292c 2028 3132 2c20  =[(5, 10), (12, 
-0000faf0: 3138 295d 2929 0a0a 2020 2020 2020 2020  18)]))..        
-0000fb00: 6173 7365 7274 6572 2e61 7373 6572 745f  asserter.assert_
-0000fb10: 280a 2020 2020 2020 2020 2020 2020 7371  (.            sq
-0000fb20: 6c61 6c63 6865 6d79 2e74 6573 7469 6e67  lalchemy.testing
-0000fb30: 2e61 7373 6572 7473 716c 2e43 7572 736f  .assertsql.Curso
-0000fb40: 7253 514c 280a 2020 2020 2020 2020 2020  rSQL(.          
-0000fb50: 2020 2020 2020 2253 454c 4543 5420 736f        "SELECT so
-0000fb60: 6d65 5f74 6162 6c65 2e69 6420 5c6e 4652  me_table.id \nFR
-0000fb70: 4f4d 2073 6f6d 655f 7461 626c 6520 220a  OM some_table ".
-0000fb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb90: 225c 6e57 4845 5245 2028 736f 6d65 5f74  "\nWHERE (some_t
-0000fba0: 6162 6c65 2e78 2c20 736f 6d65 5f74 6162  able.x, some_tab
-0000fbb0: 6c65 2e79 2920 220a 2020 2020 2020 2020  le.y) ".        
-0000fbc0: 2020 2020 2020 2020 2249 4e20 2825 7328          "IN (%s(
-0000fbd0: 352c 2031 3029 2c20 2831 322c 2031 3829  5, 10), (12, 18)
-0000fbe0: 2922 0a20 2020 2020 2020 2020 2020 2020  )".             
-0000fbf0: 2020 2025 2028 2256 414c 5545 5320 2220     % ("VALUES " 
-0000fc00: 6966 2063 6f6e 6669 672e 6462 2e64 6961  if config.db.dia
-0000fc10: 6c65 6374 2e74 7570 6c65 5f69 6e5f 7661  lect.tuple_in_va
-0000fc20: 6c75 6573 2065 6c73 6520 2222 292c 0a20  lues else ""),. 
-0000fc30: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-0000fc40: 2920 6966 2063 6f6e 6669 672e 6462 2e64  ) if config.db.d
-0000fc50: 6961 6c65 6374 2e70 6f73 6974 696f 6e61  ialect.positiona
-0000fc60: 6c20 656c 7365 207b 7d2c 0a20 2020 2020  l else {},.     
-0000fc70: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000fc80: 2029 0a0a 2020 2020 4074 6573 7469 6e67   )..    @testing
-0000fc90: 2e72 6571 7569 7265 732e 7475 706c 655f  .requires.tuple_
-0000fca0: 696e 0a20 2020 2064 6566 2074 6573 745f  in.    def test_
-0000fcb0: 6578 6563 7574 655f 7475 706c 655f 6578  execute_tuple_ex
-0000fcc0: 7061 6e64 696e 675f 706c 7573 5f6c 6974  panding_plus_lit
-0000fcd0: 6572 616c 5f68 6574 6572 6f67 656e 656f  eral_heterogeneo
-0000fce0: 7573 5f65 7865 6375 7465 2873 656c 6629  us_execute(self)
-0000fcf0: 3a0a 2020 2020 2020 2020 7461 626c 6520  :.        table 
-0000fd00: 3d20 7365 6c66 2e74 6162 6c65 732e 736f  = self.tables.so
-0000fd10: 6d65 5f74 6162 6c65 0a0a 2020 2020 2020  me_table..      
-0000fd20: 2020 7374 6d74 203d 2073 656c 6563 7428    stmt = select(
-0000fd30: 7461 626c 652e 632e 6964 292e 7768 6572  table.c.id).wher
-0000fd40: 6528 0a20 2020 2020 2020 2020 2020 2073  e(.            s
-0000fd50: 716c 616c 6368 656d 792e 7475 706c 655f  qlalchemy.tuple_
-0000fd60: 2874 6162 6c65 2e63 2e78 2c20 7461 626c  (table.c.x, tabl
-0000fd70: 652e 632e 7a29 2e69 6e5f 280a 2020 2020  e.c.z).in_(.    
-0000fd80: 2020 2020 2020 2020 2020 2020 7371 6c61              sqla
-0000fd90: 6c63 6865 6d79 2e62 696e 6470 6172 616d  lchemy.bindparam
-0000fda0: 2822 7122 2c20 6578 7061 6e64 696e 673d  ("q", expanding=
-0000fdb0: 5472 7565 2c20 6c69 7465 7261 6c5f 6578  True, literal_ex
-0000fdc0: 6563 7574 653d 5472 7565 290a 2020 2020  ecute=True).    
-0000fdd0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000fde0: 2020 290a 0a20 2020 2020 2020 2077 6974    )..        wit
-0000fdf0: 6820 7365 6c66 2e73 716c 5f65 7865 6375  h self.sql_execu
-0000fe00: 7469 6f6e 5f61 7373 6572 7465 7228 2920  tion_asserter() 
-0000fe10: 6173 2061 7373 6572 7465 723a 0a20 2020  as asserter:.   
-0000fe20: 2020 2020 2020 2020 2077 6974 6820 636f           with co
-0000fe30: 6e66 6967 2e64 622e 636f 6e6e 6563 7428  nfig.db.connect(
-0000fe40: 2920 6173 2063 6f6e 6e3a 0a20 2020 2020  ) as conn:.     
-0000fe50: 2020 2020 2020 2020 2020 2063 6f6e 6e2e             conn.
-0000fe60: 6578 6563 7574 6528 7374 6d74 2c20 6469  execute(stmt, di
-0000fe70: 6374 2871 3d5b 2835 2c20 227a 3122 292c  ct(q=[(5, "z1"),
-0000fe80: 2028 3132 2c20 227a 3322 295d 2929 0a0a   (12, "z3")]))..
-0000fe90: 2020 2020 2020 2020 6173 7365 7274 6572          asserter
-0000fea0: 2e61 7373 6572 745f 280a 2020 2020 2020  .assert_(.      
-0000feb0: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
-0000fec0: 2e74 6573 7469 6e67 2e61 7373 6572 7473  .testing.asserts
-0000fed0: 716c 2e43 7572 736f 7253 514c 280a 2020  ql.CursorSQL(.  
-0000fee0: 2020 2020 2020 2020 2020 2020 2020 2253                "S
-0000fef0: 454c 4543 5420 736f 6d65 5f74 6162 6c65  ELECT some_table
-0000ff00: 2e69 6420 5c6e 4652 4f4d 2073 6f6d 655f  .id \nFROM some_
-0000ff10: 7461 626c 6520 220a 2020 2020 2020 2020  table ".        
-0000ff20: 2020 2020 2020 2020 225c 6e57 4845 5245          "\nWHERE
-0000ff30: 2028 736f 6d65 5f74 6162 6c65 2e78 2c20   (some_table.x, 
-0000ff40: 736f 6d65 5f74 6162 6c65 2e7a 2920 220a  some_table.z) ".
-0000ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff60: 2249 4e20 2825 7328 352c 2027 7a31 2729  "IN (%s(5, 'z1')
-0000ff70: 2c20 2831 322c 2027 7a33 2729 2922 0a20  , (12, 'z3'))". 
-0000ff80: 2020 2020 2020 2020 2020 2020 2020 2025                 %
-0000ff90: 2028 2256 414c 5545 5320 2220 6966 2063   ("VALUES " if c
-0000ffa0: 6f6e 6669 672e 6462 2e64 6961 6c65 6374  onfig.db.dialect
-0000ffb0: 2e74 7570 6c65 5f69 6e5f 7661 6c75 6573  .tuple_in_values
-0000ffc0: 2065 6c73 6520 2222 292c 0a20 2020 2020   else ""),.     
-0000ffd0: 2020 2020 2020 2020 2020 2028 2920 6966             () if
-0000ffe0: 2063 6f6e 6669 672e 6462 2e64 6961 6c65   config.db.diale
-0000fff0: 6374 2e70 6f73 6974 696f 6e61 6c20 656c  ct.positional el
-00010000: 7365 207b 7d2c 0a20 2020 2020 2020 2020  se {},.         
-00010010: 2020 2029 0a20 2020 2020 2020 2029 0a0a     ).        )..
-00010020: 0a63 6c61 7373 2043 6f6d 7075 7465 6452  .class ComputedR
-00010030: 6566 6c65 6374 696f 6e46 6978 7475 7265  eflectionFixture
-00010040: 5465 7374 285f 436f 6d70 7574 6564 5265  Test(_ComputedRe
-00010050: 666c 6563 7469 6f6e 4669 7874 7572 6554  flectionFixtureT
-00010060: 6573 7429 3a0a 2020 2020 4063 6c61 7373  est):.    @class
-00010070: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
-00010080: 6566 696e 655f 7461 626c 6573 2863 6c73  efine_tables(cls
-00010090: 2c20 6d65 7461 6461 7461 293a 0a20 2020  , metadata):.   
-000100a0: 2020 2020 2022 2222 5350 414e 4e45 5220       """SPANNER 
-000100b0: 4f56 4552 5249 4445 3a0a 0a20 2020 2020  OVERRIDE:..     
-000100c0: 2020 2041 766f 6964 2075 7369 6e67 2064     Avoid using d
-000100d0: 6566 6175 6c74 2076 616c 7565 7320 666f  efault values fo
-000100e0: 7220 636f 6d70 7574 6564 2063 6f6c 756d  r computed colum
-000100f0: 6e73 2e0a 2020 2020 2020 2020 2222 220a  ns..        """.
-00010100: 2020 2020 2020 2020 5461 626c 6528 0a20          Table(. 
-00010110: 2020 2020 2020 2020 2020 2022 636f 6d70             "comp
-00010120: 7574 6564 5f64 6566 6175 6c74 5f74 6162  uted_default_tab
-00010130: 6c65 222c 0a20 2020 2020 2020 2020 2020  le",.           
-00010140: 206d 6574 6164 6174 612c 0a20 2020 2020   metadata,.     
-00010150: 2020 2020 2020 2043 6f6c 756d 6e28 2269         Column("i
-00010160: 6422 2c20 496e 7465 6765 722c 2070 7269  d", Integer, pri
-00010170: 6d61 7279 5f6b 6579 3d54 7275 6529 2c0a  mary_key=True),.
-00010180: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
-00010190: 6d6e 2822 6e6f 726d 616c 222c 2049 6e74  mn("normal", Int
-000101a0: 6567 6572 292c 0a20 2020 2020 2020 2020  eger),.         
-000101b0: 2020 2043 6f6c 756d 6e28 2263 6f6d 7075     Column("compu
-000101c0: 7465 645f 636f 6c22 2c20 496e 7465 6765  ted_col", Intege
-000101d0: 722c 2043 6f6d 7075 7465 6428 226e 6f72  r, Computed("nor
-000101e0: 6d61 6c20 2b20 3432 2229 292c 0a20 2020  mal + 42")),.   
-000101f0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00010200: 2277 6974 685f 6465 6661 756c 7422 2c20  "with_default", 
-00010210: 496e 7465 6765 7229 2c0a 2020 2020 2020  Integer),.      
-00010220: 2020 290a 0a20 2020 2020 2020 2074 203d    )..        t =
-00010230: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
-00010240: 2020 2020 2263 6f6d 7075 7465 645f 636f      "computed_co
-00010250: 6c75 6d6e 5f74 6162 6c65 222c 0a20 2020  lumn_table",.   
-00010260: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
-00010270: 612c 0a20 2020 2020 2020 2020 2020 2043  a,.            C
-00010280: 6f6c 756d 6e28 2269 6422 2c20 496e 7465  olumn("id", Inte
-00010290: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
-000102a0: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
-000102b0: 2020 2020 436f 6c75 6d6e 2822 6e6f 726d      Column("norm
-000102c0: 616c 222c 2049 6e74 6567 6572 292c 0a20  al", Integer),. 
-000102d0: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
-000102e0: 6e28 2263 6f6d 7075 7465 645f 6e6f 5f66  n("computed_no_f
-000102f0: 6c61 6722 2c20 496e 7465 6765 722c 2043  lag", Integer, C
-00010300: 6f6d 7075 7465 6428 226e 6f72 6d61 6c20  omputed("normal 
-00010310: 2b20 3432 2229 292c 0a20 2020 2020 2020  + 42")),.       
-00010320: 2029 0a0a 2020 2020 2020 2020 6966 2074   )..        if t
-00010330: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
-00010340: 636f 6d70 7574 6564 5f63 6f6c 756d 6e73  computed_columns
-00010350: 5f76 6972 7475 616c 2e65 6e61 626c 6564  _virtual.enabled
-00010360: 3a0a 2020 2020 2020 2020 2020 2020 742e  :.            t.
-00010370: 6170 7065 6e64 5f63 6f6c 756d 6e28 0a20  append_column(. 
-00010380: 2020 2020 2020 2020 2020 2020 2020 2043                 C
-00010390: 6f6c 756d 6e28 0a20 2020 2020 2020 2020  olumn(.         
-000103a0: 2020 2020 2020 2020 2020 2022 636f 6d70             "comp
-000103b0: 7574 6564 5f76 6972 7475 616c 222c 0a20  uted_virtual",. 
-000103c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103d0: 2020 2049 6e74 6567 6572 2c0a 2020 2020     Integer,.    
-000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103f0: 436f 6d70 7574 6564 2822 6e6f 726d 616c  Computed("normal
-00010400: 202b 2032 222c 2070 6572 7369 7374 6564   + 2", persisted
-00010410: 3d46 616c 7365 292c 0a20 2020 2020 2020  =False),.       
-00010420: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00010430: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00010440: 2069 6620 7465 7374 696e 672e 7265 7175   if testing.requ
-00010450: 6972 6573 2e63 6f6d 7075 7465 645f 636f  ires.computed_co
-00010460: 6c75 6d6e 735f 7374 6f72 6564 2e65 6e61  lumns_stored.ena
-00010470: 626c 6564 3a0a 2020 2020 2020 2020 2020  bled:.          
-00010480: 2020 742e 6170 7065 6e64 5f63 6f6c 756d    t.append_colum
-00010490: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-000104a0: 2020 2043 6f6c 756d 6e28 0a20 2020 2020     Column(.     
-000104b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000104c0: 636f 6d70 7574 6564 5f73 746f 7265 6422  computed_stored"
-000104d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000104e0: 2020 2020 2020 496e 7465 6765 722c 0a20        Integer,. 
-000104f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010500: 2020 2043 6f6d 7075 7465 6428 226e 6f72     Computed("nor
-00010510: 6d61 6c20 2d20 3432 222c 2070 6572 7369  mal - 42", persi
-00010520: 7374 6564 3d54 7275 6529 2c0a 2020 2020  sted=True),.    
-00010530: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00010540: 2020 2020 2020 2020 2020 290a 0a0a 636c            )...cl
-00010550: 6173 7320 436f 6d70 7574 6564 5265 666c  ass ComputedRefl
-00010560: 6563 7469 6f6e 5465 7374 285f 436f 6d70  ectionTest(_Comp
-00010570: 7574 6564 5265 666c 6563 7469 6f6e 5465  utedReflectionTe
-00010580: 7374 2c20 436f 6d70 7574 6564 5265 666c  st, ComputedRefl
-00010590: 6563 7469 6f6e 4669 7874 7572 6554 6573  ectionFixtureTes
-000105a0: 7429 3a0a 2020 2020 4074 6573 7469 6e67  t):.    @testing
-000105b0: 2e72 6571 7569 7265 732e 7363 6865 6d61  .requires.schema
-000105c0: 730a 2020 2020 6465 6620 7465 7374 5f67  s.    def test_g
-000105d0: 6574 5f63 6f6c 756d 6e5f 7265 7475 726e  et_column_return
-000105e0: 735f 7065 7273 6973 7465 645f 7769 7468  s_persisted_with
-000105f0: 5f73 6368 656d 6128 7365 6c66 293a 0a20  _schema(self):. 
-00010600: 2020 2020 2020 2069 6e73 7020 3d20 696e         insp = in
-00010610: 7370 6563 7428 636f 6e66 6967 2e64 6229  spect(config.db)
-00010620: 0a0a 2020 2020 2020 2020 636f 6c73 203d  ..        cols =
-00010630: 2069 6e73 702e 6765 745f 636f 6c75 6d6e   insp.get_column
-00010640: 7328 2263 6f6d 7075 7465 645f 636f 6c75  s("computed_colu
-00010650: 6d6e 5f74 6162 6c65 222c 2073 6368 656d  mn_table", schem
-00010660: 613d 636f 6e66 6967 2e74 6573 745f 7363  a=config.test_sc
-00010670: 6865 6d61 290a 2020 2020 2020 2020 6461  hema).        da
-00010680: 7461 203d 207b 635b 226e 616d 6522 5d3a  ta = {c["name"]:
-00010690: 2063 2066 6f72 2063 2069 6e20 636f 6c73   c for c in cols
-000106a0: 7d0a 0a20 2020 2020 2020 2073 656c 662e  }..        self.
-000106b0: 6368 6563 6b5f 636f 6c75 6d6e 280a 2020  check_column(.  
-000106c0: 2020 2020 2020 2020 2020 6461 7461 2c0a            data,.
-000106d0: 2020 2020 2020 2020 2020 2020 2263 6f6d              "com
-000106e0: 7075 7465 645f 6e6f 5f66 6c61 6722 2c0a  puted_no_flag",.
-000106f0: 2020 2020 2020 2020 2020 2020 226e 6f72              "nor
-00010700: 6d61 6c2b 3432 222c 0a20 2020 2020 2020  mal+42",.       
-00010710: 2020 2020 2074 6573 7469 6e67 2e72 6571       testing.req
-00010720: 7569 7265 732e 636f 6d70 7574 6564 5f63  uires.computed_c
-00010730: 6f6c 756d 6e73 5f64 6566 6175 6c74 5f70  olumns_default_p
-00010740: 6572 7369 7374 6564 2e65 6e61 626c 6564  ersisted.enabled
-00010750: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00010760: 2020 2020 6966 2074 6573 7469 6e67 2e72      if testing.r
-00010770: 6571 7569 7265 732e 636f 6d70 7574 6564  equires.computed
-00010780: 5f63 6f6c 756d 6e73 5f76 6972 7475 616c  _columns_virtual
-00010790: 2e65 6e61 626c 6564 3a0a 2020 2020 2020  .enabled:.      
-000107a0: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
-000107b0: 5f63 6f6c 756d 6e28 0a20 2020 2020 2020  _column(.       
-000107c0: 2020 2020 2020 2020 2064 6174 612c 0a20           data,. 
-000107d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000107e0: 636f 6d70 7574 6564 5f76 6972 7475 616c  computed_virtual
-000107f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00010800: 2020 2022 6e6f 726d 616c 2f32 222c 0a20     "normal/2",. 
-00010810: 2020 2020 2020 2020 2020 2020 2020 2046                 F
-00010820: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00010830: 2020 290a 2020 2020 2020 2020 6966 2074    ).        if t
-00010840: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
-00010850: 636f 6d70 7574 6564 5f63 6f6c 756d 6e73  computed_columns
-00010860: 5f73 746f 7265 642e 656e 6162 6c65 643a  _stored.enabled:
-00010870: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010880: 662e 6368 6563 6b5f 636f 6c75 6d6e 280a  f.check_column(.
-00010890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108a0: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
-000108b0: 2020 2020 2020 2263 6f6d 7075 7465 645f        "computed_
-000108c0: 7374 6f72 6564 222c 0a20 2020 2020 2020  stored",.       
-000108d0: 2020 2020 2020 2020 2022 6e6f 726d 616c           "normal
-000108e0: 2d34 3222 2c0a 2020 2020 2020 2020 2020  -42",.          
-000108f0: 2020 2020 2020 5472 7565 2c0a 2020 2020        True,.    
-00010900: 2020 2020 2020 2020 290a 0a20 2020 2040          )..    @
-00010910: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-00010920: 2822 4465 6661 756c 7420 7661 6c75 6573  ("Default values
-00010930: 2061 7265 206e 6f74 2073 7570 706f 7274   are not support
-00010940: 6564 2e22 290a 2020 2020 6465 6620 7465  ed.").    def te
-00010950: 7374 5f63 6f6d 7075 7465 645f 636f 6c5f  st_computed_col_
-00010960: 6465 6661 756c 745f 6e6f 745f 7365 7428  default_not_set(
-00010970: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00010980: 6173 730a 0a20 2020 2064 6566 2074 6573  ass..    def tes
-00010990: 745f 6765 745f 636f 6c75 6d6e 5f72 6574  t_get_column_ret
-000109a0: 7572 6e73 5f63 6f6d 7075 7465 6428 7365  urns_computed(se
-000109b0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-000109c0: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
-000109d0: 204f 5645 5252 4944 453a 0a0a 2020 2020   OVERRIDE:..    
-000109e0: 2020 2020 496e 2053 7061 6e6e 6572 2061      In Spanner a
-000109f0: 6c6c 2074 6865 2067 656e 6572 6174 6564  ll the generated
-00010a00: 2063 6f6c 756d 6e73 2061 7265 2053 544f   columns are STO
-00010a10: 5245 442c 0a20 2020 2020 2020 206d 6561  RED,.        mea
-00010a20: 6e69 6e67 2074 6865 7265 2061 7265 206e  ning there are n
-00010a30: 6f20 7065 7273 6973 7465 6420 616e 6420  o persisted and 
-00010a40: 6e6f 7420 7065 7273 6973 7465 640a 2020  not persisted.  
-00010a50: 2020 2020 2020 2869 6e20 7468 6520 7465        (in the te
-00010a60: 726d 7320 6f66 2074 6865 2053 514c 416c  rms of the SQLAl
-00010a70: 6368 656d 7929 2063 6f6c 756d 6e73 2e20  chemy) columns. 
-00010a80: 5468 650a 2020 2020 2020 2020 6d65 7468  The.        meth
-00010a90: 6f64 206f 7665 7272 6964 6520 6f6d 6974  od override omit
-00010aa0: 7320 7468 6520 7065 7273 6973 7465 6e63  s the persistenc
-00010ab0: 6520 7265 666c 6563 7469 6f6e 2063 6865  e reflection che
-00010ac0: 636b 732e 0a20 2020 2020 2020 2022 2222  cks..        """
-00010ad0: 0a20 2020 2020 2020 2069 6e73 7020 3d20  .        insp = 
-00010ae0: 696e 7370 6563 7428 636f 6e66 6967 2e64  inspect(config.d
-00010af0: 6229 0a0a 2020 2020 2020 2020 636f 6c73  b)..        cols
-00010b00: 203d 2069 6e73 702e 6765 745f 636f 6c75   = insp.get_colu
-00010b10: 6d6e 7328 2263 6f6d 7075 7465 645f 6465  mns("computed_de
-00010b20: 6661 756c 745f 7461 626c 6522 290a 2020  fault_table").  
-00010b30: 2020 2020 2020 6461 7461 203d 207b 635b        data = {c[
-00010b40: 226e 616d 6522 5d3a 2063 2066 6f72 2063  "name"]: c for c
-00010b50: 2069 6e20 636f 6c73 7d0a 2020 2020 2020   in cols}.      
-00010b60: 2020 666f 7220 6b65 7920 696e 2028 2269    for key in ("i
-00010b70: 6422 2c20 226e 6f72 6d61 6c22 2c20 2277  d", "normal", "w
-00010b80: 6974 685f 6465 6661 756c 7422 293a 0a20  ith_default"):. 
-00010b90: 2020 2020 2020 2020 2020 2069 735f 7472             is_tr
-00010ba0: 7565 2822 636f 6d70 7574 6564 2220 6e6f  ue("computed" no
-00010bb0: 7420 696e 2064 6174 615b 6b65 795d 290a  t in data[key]).
-00010bc0: 2020 2020 2020 2020 636f 6d70 4461 7461          compData
-00010bd0: 203d 2064 6174 615b 2263 6f6d 7075 7465   = data["compute
-00010be0: 645f 636f 6c22 5d0a 2020 2020 2020 2020  d_col"].        
-00010bf0: 6973 5f74 7275 6528 2263 6f6d 7075 7465  is_true("compute
-00010c00: 6422 2069 6e20 636f 6d70 4461 7461 290a  d" in compData).
-00010c10: 2020 2020 2020 2020 6973 5f74 7275 6528          is_true(
-00010c20: 2273 716c 7465 7874 2220 696e 2063 6f6d  "sqltext" in com
-00010c30: 7044 6174 615b 2263 6f6d 7075 7465 6422  pData["computed"
-00010c40: 5d29 0a20 2020 2020 2020 2065 715f 2873  ]).        eq_(s
-00010c50: 656c 662e 6e6f 726d 616c 697a 6528 636f  elf.normalize(co
-00010c60: 6d70 4461 7461 5b22 636f 6d70 7574 6564  mpData["computed
-00010c70: 225d 5b22 7371 6c74 6578 7422 5d29 2c20  "]["sqltext"]), 
-00010c80: 226e 6f72 6d61 6c2b 3432 2229 0a0a 2020  "normal+42")..  
-00010c90: 2020 6465 6620 7465 7374 5f63 7265 6174    def test_creat
-00010ca0: 655f 6e6f 745f 6e75 6c6c 5f63 6f6d 7075  e_not_null_compu
-00010cb0: 7465 645f 636f 6c75 6d6e 2873 656c 6629  ted_column(self)
-00010cc0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00010cd0: 2020 2020 2020 5350 414e 4e45 5220 5445        SPANNER TE
-00010ce0: 5354 3a0a 0a20 2020 2020 2020 2043 6865  ST:..        Che
-00010cf0: 636b 2074 6861 7420 6f6e 2063 7265 6174  ck that on creat
-00010d00: 696e 6720 6120 636f 6d70 7574 6564 2063  ing a computed c
-00010d10: 6f6c 756d 6e20 7769 7468 2061 204e 4f54  olumn with a NOT
-00010d20: 204e 554c 4c0a 2020 2020 2020 2020 636c   NULL.        cl
-00010d30: 6175 7365 2074 6865 2063 6c61 7573 6520  ause the clause 
-00010d40: 6973 2073 6574 2069 6e20 6672 6f6e 7420  is set in front 
-00010d50: 6f66 2074 6865 2063 6f6d 7075 7465 6420  of the computed 
-00010d60: 636f 6c75 6d6e 0a20 2020 2020 2020 2073  column.        s
-00010d70: 7461 7465 6d65 6e74 2064 6566 696e 6974  tatement definit
-00010d80: 696f 6e20 616e 6420 646f 6573 6e27 7420  ion and doesn't 
-00010d90: 6361 7573 6520 6661 696c 7572 6573 2e0a  cause failures..
-00010da0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010db0: 2020 2020 656e 6769 6e65 203d 2063 7265      engine = cre
-00010dc0: 6174 655f 656e 6769 6e65 2867 6574 5f64  ate_engine(get_d
-00010dd0: 625f 7572 6c28 2929 0a20 2020 2020 2020  b_url()).       
-00010de0: 206d 6574 6164 6174 6120 3d20 4d65 7461   metadata = Meta
-00010df0: 4461 7461 2862 696e 643d 656e 6769 6e65  Data(bind=engine
-00010e00: 290a 0a20 2020 2020 2020 2054 6162 6c65  )..        Table
-00010e10: 280a 2020 2020 2020 2020 2020 2020 2253  (.            "S
-00010e20: 696e 6765 7273 222c 0a20 2020 2020 2020  ingers",.       
-00010e30: 2020 2020 206d 6574 6164 6174 612c 0a20       metadata,. 
-00010e40: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
-00010e50: 6e28 2253 696e 6765 7249 6422 2c20 5374  n("SingerId", St
-00010e60: 7269 6e67 2833 3629 2c20 7072 696d 6172  ring(36), primar
-00010e70: 795f 6b65 793d 5472 7565 2c20 6e75 6c6c  y_key=True, null
-00010e80: 6162 6c65 3d46 616c 7365 292c 0a20 2020  able=False),.   
-00010e90: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00010ea0: 2246 6972 7374 4e61 6d65 222c 2053 7472  "FirstName", Str
-00010eb0: 696e 6728 3230 3029 292c 0a20 2020 2020  ing(200)),.     
-00010ec0: 2020 2020 2020 2043 6f6c 756d 6e28 224c         Column("L
-00010ed0: 6173 744e 616d 6522 2c20 5374 7269 6e67  astName", String
-00010ee0: 2832 3030 292c 206e 756c 6c61 626c 653d  (200), nullable=
-00010ef0: 4661 6c73 6529 2c0a 2020 2020 2020 2020  False),.        
-00010f00: 2020 2020 436f 6c75 6d6e 280a 2020 2020      Column(.    
-00010f10: 2020 2020 2020 2020 2020 2020 2246 756c              "Ful
-00010f20: 6c4e 616d 6522 2c0a 2020 2020 2020 2020  lName",.        
-00010f30: 2020 2020 2020 2020 5374 7269 6e67 2834          String(4
-00010f40: 3030 292c 0a20 2020 2020 2020 2020 2020  00),.           
-00010f50: 2020 2020 2043 6f6d 7075 7465 6428 2243       Computed("C
-00010f60: 4f41 4c45 5343 4528 4669 7273 744e 616d  OALESCE(FirstNam
-00010f70: 6520 7c7c 2027 2027 2c20 2727 2920 7c7c  e || ' ', '') ||
-00010f80: 204c 6173 744e 616d 6522 292c 0a20 2020   LastName"),.   
-00010f90: 2020 2020 2020 2020 2020 2020 206e 756c               nul
-00010fa0: 6c61 626c 653d 4661 6c73 652c 0a20 2020  lable=False,.   
-00010fb0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00010fc0: 2020 2020 290a 0a20 2020 2020 2020 206d      )..        m
-00010fd0: 6574 6164 6174 612e 6372 6561 7465 5f61  etadata.create_a
-00010fe0: 6c6c 2865 6e67 696e 6529 0a0a 0a40 7079  ll(engine)...@py
-00010ff0: 7465 7374 2e6d 6172 6b2e 736b 6970 6966  test.mark.skipif
-00011000: 280a 2020 2020 626f 6f6c 286f 732e 656e  (.    bool(os.en
-00011010: 7669 726f 6e2e 6765 7428 2253 5041 4e4e  viron.get("SPANN
-00011020: 4552 5f45 4d55 4c41 544f 525f 484f 5354  ER_EMULATOR_HOST
-00011030: 2229 292c 2072 6561 736f 6e3d 2253 6b69  ")), reason="Ski
-00011040: 7070 6564 206f 6e20 656d 756c 6174 6f72  pped on emulator
-00011050: 220a 290a 636c 6173 7320 4a53 4f4e 5465  ".).class JSONTe
-00011060: 7374 285f 4a53 4f4e 5465 7374 293a 0a20  st(_JSONTest):. 
-00011070: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-00011080: 736b 6970 2822 5661 6c75 6573 2077 6974  skip("Values wit
-00011090: 686f 7574 206b 6579 7320 6172 6520 6e6f  hout keys are no
-000110a0: 7420 7375 7070 6f72 7465 642e 2229 0a20  t supported."). 
-000110b0: 2020 2064 6566 2074 6573 745f 7369 6e67     def test_sing
-000110c0: 6c65 5f65 6c65 6d65 6e74 5f72 6f75 6e64  le_element_round
-000110d0: 5f74 7269 7028 7365 6c66 2c20 656c 656d  _trip(self, elem
-000110e0: 656e 7429 3a0a 2020 2020 2020 2020 7061  ent):.        pa
-000110f0: 7373 0a0a 2020 2020 6465 6620 5f74 6573  ss..    def _tes
-00011100: 745f 726f 756e 645f 7472 6970 2873 656c  t_round_trip(sel
-00011110: 662c 2064 6174 615f 656c 656d 656e 7429  f, data_element)
-00011120: 3a0a 2020 2020 2020 2020 6461 7461 5f74  :.        data_t
-00011130: 6162 6c65 203d 2073 656c 662e 7461 626c  able = self.tabl
-00011140: 6573 2e64 6174 615f 7461 626c 650a 0a20  es.data_table.. 
-00011150: 2020 2020 2020 2063 6f6e 6669 672e 6462         config.db
-00011160: 2e65 7865 6375 7465 280a 2020 2020 2020  .execute(.      
-00011170: 2020 2020 2020 6461 7461 5f74 6162 6c65        data_table
-00011180: 2e69 6e73 6572 7428 292c 0a20 2020 2020  .insert(),.     
-00011190: 2020 2020 2020 207b 2269 6422 3a20 7261         {"id": ra
-000111a0: 6e64 6f6d 2e72 616e 6469 6e74 2831 2c20  ndom.randint(1, 
-000111b0: 3130 3030 3030 3030 3029 2c20 226e 616d  100000000), "nam
-000111c0: 6522 3a20 2272 6f77 3122 2c20 2264 6174  e": "row1", "dat
-000111d0: 6122 3a20 6461 7461 5f65 6c65 6d65 6e74  a": data_element
-000111e0: 7d2c 0a20 2020 2020 2020 2029 0a0a 2020  },.        )..  
-000111f0: 2020 2020 2020 726f 7720 3d20 636f 6e66        row = conf
-00011200: 6967 2e64 622e 6578 6563 7574 6528 7365  ig.db.execute(se
-00011210: 6c65 6374 285b 6461 7461 5f74 6162 6c65  lect([data_table
-00011220: 2e63 2e64 6174 615d 2929 2e66 6972 7374  .c.data])).first
-00011230: 2829 0a0a 2020 2020 2020 2020 6571 5f28  ()..        eq_(
-00011240: 726f 772c 2028 6461 7461 5f65 6c65 6d65  row, (data_eleme
-00011250: 6e74 2c29 290a 0a20 2020 2064 6566 2074  nt,))..    def t
-00011260: 6573 745f 756e 6963 6f64 655f 726f 756e  est_unicode_roun
-00011270: 645f 7472 6970 2873 656c 6629 3a0a 2020  d_trip(self):.  
-00011280: 2020 2020 2020 2320 6e6f 7465 2077 6520        # note we 
-00011290: 696e 636c 7564 6520 556e 6963 6f64 6520  include Unicode 
-000112a0: 7375 7070 6c65 6d65 6e74 6172 7920 6368  supplementary ch
-000112b0: 6172 6163 7465 7273 2061 7320 7765 6c6c  aracters as well
-000112c0: 0a20 2020 2020 2020 2077 6974 6820 636f  .        with co
-000112d0: 6e66 6967 2e64 622e 636f 6e6e 6563 7428  nfig.db.connect(
-000112e0: 2920 6173 2063 6f6e 6e3a 0a20 2020 2020  ) as conn:.     
-000112f0: 2020 2020 2020 2063 6f6e 6e2e 6578 6563         conn.exec
-00011300: 7574 6528 0a20 2020 2020 2020 2020 2020  ute(.           
-00011310: 2020 2020 2073 656c 662e 7461 626c 6573       self.tables
-00011320: 2e64 6174 615f 7461 626c 652e 696e 7365  .data_table.inse
-00011330: 7274 2829 2c0a 2020 2020 2020 2020 2020  rt(),.          
-00011340: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00011350: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
-00011360: 3a20 7261 6e64 6f6d 2e72 616e 6469 6e74  : random.randint
-00011370: 2831 2c20 3130 3030 3030 3030 3029 2c0a  (1, 100000000),.
-00011380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011390: 2020 2020 226e 616d 6522 3a20 2272 3122      "name": "r1"
-000113a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000113b0: 2020 2020 2020 2264 6174 6122 3a20 7b0a        "data": {.
-000113c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113d0: 2020 2020 2020 2020 7574 696c 2e75 2822          util.u("
-000113e0: 72c3 a976 65f0 9f90 8d20 696c 6cc3 a922  r..ve.... ill.."
-000113f0: 293a 2075 7469 6c2e 7528 2272 c3a9 7665  ): util.u("r..ve
-00011400: f09f 908d 2069 6c6c c3a9 2229 2c0a 2020  .... ill.."),.  
-00011410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011420: 2020 2020 2020 2264 6174 6122 3a20 7b22        "data": {"
-00011430: 6b31 223a 2075 7469 6c2e 7528 2264 72c3  k1": util.u("dr.
-00011440: b46c f09f 908d 6522 297d 2c0a 2020 2020  .l....e")},.    
-00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011460: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00011470: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00011480: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
-00011490: 2065 715f 280a 2020 2020 2020 2020 2020   eq_(.          
-000114a0: 2020 2020 2020 636f 6e6e 2e73 6361 6c61        conn.scala
-000114b0: 7228 7365 6c65 6374 285b 7365 6c66 2e74  r(select([self.t
-000114c0: 6162 6c65 732e 6461 7461 5f74 6162 6c65  ables.data_table
-000114d0: 2e63 2e64 6174 615d 2929 2c0a 2020 2020  .c.data])),.    
-000114e0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011500: 2020 7574 696c 2e75 2822 72c3 a976 65f0    util.u("r..ve.
-00011510: 9f90 8d20 696c 6cc3 a922 293a 2075 7469  ... ill.."): uti
-00011520: 6c2e 7528 2272 c3a9 7665 f09f 908d 2069  l.u("r..ve.... i
-00011530: 6c6c c3a9 2229 2c0a 2020 2020 2020 2020  ll.."),.        
-00011540: 2020 2020 2020 2020 2020 2020 2264 6174              "dat
-00011550: 6122 3a20 7b22 6b31 223a 2075 7469 6c2e  a": {"k1": util.
-00011560: 7528 2264 72c3 b46c f09f 908d 6522 297d  u("dr..l....e")}
-00011570: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011580: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00011590: 2029 0a0a 2020 2020 4070 7974 6573 742e   )..    @pytest.
-000115a0: 6d61 726b 2e73 6b69 7028 2250 6172 616d  mark.skip("Param
-000115b0: 6574 6572 697a 6564 2074 7970 6573 2061  eterized types a
-000115c0: 7265 206e 6f74 2073 7570 706f 7274 6564  re not supported
-000115d0: 2e22 290a 2020 2020 6465 6620 7465 7374  .").    def test
-000115e0: 5f65 7661 6c5f 6e6f 6e65 5f66 6c61 675f  _eval_none_flag_
-000115f0: 6f72 6d28 7365 6c66 293a 0a20 2020 2020  orm(self):.     
-00011600: 2020 2070 6173 730a 0a20 2020 2040 7079     pass..    @py
-00011610: 7465 7374 2e6d 6172 6b2e 736b 6970 280a  test.mark.skip(.
-00011620: 2020 2020 2020 2020 2253 7061 6e6e 6572          "Spanner
-00011630: 204a 534f 4e5f 5641 4c55 4528 2920 616c   JSON_VALUE() al
-00011640: 7761 7973 2072 6574 7572 6e73 2053 5452  ways returns STR
-00011650: 494e 472c 220a 2020 2020 2020 2020 2274  ING,".        "t
-00011660: 6875 732c 2074 6869 7320 7465 7374 2063  hus, this test c
-00011670: 6173 6520 6361 6e27 7420 6265 2065 7865  ase can't be exe
-00011680: 6375 7465 642e 220a 2020 2020 290a 2020  cuted.".    ).  
-00011690: 2020 6465 6620 7465 7374 5f69 6e64 6578    def test_index
-000116a0: 5f74 7970 6564 5f63 6f6d 7061 7269 736f  _typed_compariso
-000116b0: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
-000116c0: 2070 6173 730a 0a20 2020 2040 7079 7465   pass..    @pyte
-000116d0: 7374 2e6d 6172 6b2e 736b 6970 280a 2020  st.mark.skip(.  
-000116e0: 2020 2020 2020 2253 7061 6e6e 6572 204a        "Spanner J
-000116f0: 534f 4e5f 5641 4c55 4528 2920 616c 7761  SON_VALUE() alwa
-00011700: 7973 2072 6574 7572 6e73 2053 5452 494e  ys returns STRIN
-00011710: 472c 220a 2020 2020 2020 2020 2274 6875  G,".        "thu
-00011720: 732c 2074 6869 7320 7465 7374 2063 6173  s, this test cas
-00011730: 6520 6361 6e27 7420 6265 2065 7865 6375  e can't be execu
-00011740: 7465 642e 220a 2020 2020 290a 2020 2020  ted.".    ).    
-00011750: 6465 6620 7465 7374 5f70 6174 685f 7479  def test_path_ty
-00011760: 7065 645f 636f 6d70 6172 6973 6f6e 2873  ped_comparison(s
-00011770: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-00011780: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
-00011790: 6d61 726b 2e73 6b69 7028 2243 7573 746f  mark.skip("Custo
-000117a0: 6d20 4a53 4f4e 2064 652d 2f73 6572 6961  m JSON de-/seria
-000117b0: 6c69 7a65 7273 2061 7265 206e 6f74 2073  lizers are not s
-000117c0: 7570 706f 7274 6564 2e22 290a 2020 2020  upported.").    
-000117d0: 6465 6620 7465 7374 5f72 6f75 6e64 5f74  def test_round_t
-000117e0: 7269 705f 6375 7374 6f6d 5f6a 736f 6e28  rip_custom_json(
-000117f0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00011800: 6173 730a 0a20 2020 2064 6566 205f 696e  ass..    def _in
-00011810: 6465 785f 6669 7874 7572 6573 2866 6e29  dex_fixtures(fn)
-00011820: 3a0a 2020 2020 2020 2020 666e 203d 2074  :.        fn = t
-00011830: 6573 7469 6e67 2e63 6f6d 6269 6e61 7469  esting.combinati
-00011840: 6f6e 7328 0a20 2020 2020 2020 2020 2020  ons(.           
-00011850: 2028 2262 6f6f 6c65 616e 222c 2054 7275   ("boolean", Tru
-00011860: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00011870: 2822 626f 6f6c 6561 6e22 2c20 4661 6c73  ("boolean", Fals
-00011880: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00011890: 2822 626f 6f6c 6561 6e22 2c20 4e6f 6e65  ("boolean", None
-000118a0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-000118b0: 2273 7472 696e 6722 2c20 2273 6f6d 6520  "string", "some 
-000118c0: 7374 7269 6e67 2229 2c0a 2020 2020 2020  string"),.      
-000118d0: 2020 2020 2020 2822 7374 7269 6e67 222c        ("string",
-000118e0: 204e 6f6e 6529 2c0a 2020 2020 2020 2020   None),.        
-000118f0: 2020 2020 2822 696e 7465 6765 7222 2c20      ("integer", 
-00011900: 3135 292c 0a20 2020 2020 2020 2020 2020  15),.           
-00011910: 2028 2269 6e74 6567 6572 222c 2031 292c   ("integer", 1),
-00011920: 0a20 2020 2020 2020 2020 2020 2028 2269  .            ("i
-00011930: 6e74 6567 6572 222c 2030 292c 0a20 2020  nteger", 0),.   
-00011940: 2020 2020 2020 2020 2028 2269 6e74 6567           ("integ
-00011950: 6572 222c 204e 6f6e 6529 2c0a 2020 2020  er", None),.    
-00011960: 2020 2020 2020 2020 2822 666c 6f61 7422          ("float"
-00011970: 2c20 3238 2e35 292c 0a20 2020 2020 2020  , 28.5),.       
-00011980: 2020 2020 2028 2266 6c6f 6174 222c 204e       ("float", N
-00011990: 6f6e 6529 2c0a 2020 2020 2020 2020 2020  one),.          
-000119a0: 2020 6964 5f3d 2273 6122 2c0a 2020 2020    id_="sa",.    
-000119b0: 2020 2020 2928 666e 290a 2020 2020 2020      )(fn).      
-000119c0: 2020 7265 7475 726e 2066 6e0a 0a20 2020    return fn..   
-000119d0: 2040 5f69 6e64 6578 5f66 6978 7475 7265   @_index_fixture
-000119e0: 730a 2020 2020 6465 6620 7465 7374 5f69  s.    def test_i
-000119f0: 6e64 6578 5f74 7970 6564 5f61 6363 6573  ndex_typed_acces
-00011a00: 7328 7365 6c66 2c20 6461 7461 7479 7065  s(self, datatype
-00011a10: 2c20 7661 6c75 6529 3a0a 2020 2020 2020  , value):.      
-00011a20: 2020 6461 7461 5f74 6162 6c65 203d 2073    data_table = s
-00011a30: 656c 662e 7461 626c 6573 2e64 6174 615f  elf.tables.data_
-00011a40: 7461 626c 650a 2020 2020 2020 2020 6461  table.        da
-00011a50: 7461 5f65 6c65 6d65 6e74 203d 207b 226b  ta_element = {"k
-00011a60: 6579 3122 3a20 7661 6c75 657d 0a20 2020  ey1": value}.   
-00011a70: 2020 2020 2077 6974 6820 636f 6e66 6967       with config
-00011a80: 2e64 622e 636f 6e6e 6563 7428 2920 6173  .db.connect() as
-00011a90: 2063 6f6e 6e3a 0a20 2020 2020 2020 2020   conn:.         
-00011aa0: 2020 2063 6f6e 6e2e 6578 6563 7574 6528     conn.execute(
-00011ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011ac0: 2064 6174 615f 7461 626c 652e 696e 7365   data_table.inse
-00011ad0: 7274 2829 2c0a 2020 2020 2020 2020 2020  rt(),.          
-00011ae0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00011af0: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
-00011b00: 3a20 7261 6e64 6f6d 2e72 616e 6469 6e74  : random.randint
-00011b10: 2831 2c20 3130 3030 3030 3030 3029 2c0a  (1, 100000000),.
-00011b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b30: 2020 2020 226e 616d 6522 3a20 2272 6f77      "name": "row
-00011b40: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
-00011b50: 2020 2020 2020 2020 2264 6174 6122 3a20          "data": 
-00011b60: 6461 7461 5f65 6c65 6d65 6e74 2c0a 2020  data_element,.  
-00011b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b80: 2020 226e 756c 6c64 6174 6122 3a20 6461    "nulldata": da
-00011b90: 7461 5f65 6c65 6d65 6e74 2c0a 2020 2020  ta_element,.    
-00011ba0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00011bb0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00011bc0: 2020 2020 2020 2020 2020 6578 7072 203d            expr =
-00011bd0: 2064 6174 615f 7461 626c 652e 632e 6461   data_table.c.da
-00011be0: 7461 5b22 6b65 7931 225d 0a20 2020 2020  ta["key1"].     
-00011bf0: 2020 2020 2020 2065 7870 7220 3d20 6765         expr = ge
-00011c00: 7461 7474 7228 6578 7072 2c20 2261 735f  tattr(expr, "as_
-00011c10: 2573 2220 2520 6461 7461 7479 7065 2928  %s" % datatype)(
-00011c20: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00011c30: 6f75 6e64 7472 6970 203d 2063 6f6e 6e2e  oundtrip = conn.
-00011c40: 7363 616c 6172 2873 656c 6563 7428 5b65  scalar(select([e
-00011c50: 7870 725d 2929 0a20 2020 2020 2020 2020  xpr])).         
-00011c60: 2020 2069 6620 726f 756e 6474 7269 7020     if roundtrip 
-00011c70: 696e 2028 2274 7275 6522 2c20 2266 616c  in ("true", "fal
-00011c80: 7365 222c 204e 6f6e 6529 3a0a 2020 2020  se", None):.    
-00011c90: 2020 2020 2020 2020 2020 2020 726f 756e              roun
-00011ca0: 6474 7269 7020 3d20 7374 7228 726f 756e  dtrip = str(roun
-00011cb0: 6474 7269 7029 2e63 6170 6974 616c 697a  dtrip).capitaliz
-00011cc0: 6528 290a 0a20 2020 2020 2020 2020 2020  e()..           
-00011cd0: 2065 715f 2873 7472 2872 6f75 6e64 7472   eq_(str(roundtr
-00011ce0: 6970 292c 2073 7472 2876 616c 7565 2929  ip), str(value))
-00011cf0: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-00011d00: 726b 2e73 6b69 7028 0a20 2020 2020 2020  rk.skip(.       
-00011d10: 2022 5370 616e 6e65 7220 646f 6573 6e27   "Spanner doesn'
-00011d20: 7420 7375 7070 6f72 7420 7479 7065 2063  t support type c
-00011d30: 6173 7473 2069 6e73 6964 6520 4a53 4f4e  asts inside JSON
-00011d40: 5f56 414c 5545 2829 2066 756e 6374 696f  _VALUE() functio
-00011d50: 6e2e 220a 2020 2020 290a 2020 2020 6465  n.".    ).    de
-00011d60: 6620 7465 7374 5f72 6f75 6e64 5f74 7269  f test_round_tri
-00011d70: 705f 6a73 6f6e 5f6e 756c 6c5f 6173 5f6a  p_json_null_as_j
-00011d80: 736f 6e5f 6e75 6c6c 2873 656c 6629 3a0a  son_null(self):.
-00011d90: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00011da0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-00011db0: 6b69 7028 0a20 2020 2020 2020 2022 5370  kip(.        "Sp
-00011dc0: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
-00011dd0: 7070 6f72 7420 7479 7065 2063 6173 7473  pport type casts
-00011de0: 2069 6e73 6964 6520 4a53 4f4e 5f56 414c   inside JSON_VAL
-00011df0: 5545 2829 2066 756e 6374 696f 6e2e 220a  UE() function.".
-00011e00: 2020 2020 290a 2020 2020 6465 6620 7465      ).    def te
-00011e10: 7374 5f72 6f75 6e64 5f74 7269 705f 6e6f  st_round_trip_no
-00011e20: 6e65 5f61 735f 6a73 6f6e 5f6e 756c 6c28  ne_as_json_null(
-00011e30: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00011e40: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
-00011e50: 2e6d 6172 6b2e 736b 6970 280a 2020 2020  .mark.skip(.    
-00011e60: 2020 2020 2253 7061 6e6e 6572 2064 6f65      "Spanner doe
-00011e70: 736e 2774 2073 7570 706f 7274 2074 7970  sn't support typ
-00011e80: 6520 6361 7374 7320 696e 7369 6465 204a  e casts inside J
-00011e90: 534f 4e5f 5641 4c55 4528 2920 6675 6e63  SON_VALUE() func
-00011ea0: 7469 6f6e 2e22 0a20 2020 2029 0a20 2020  tion.".    ).   
-00011eb0: 2064 6566 2074 6573 745f 726f 756e 645f   def test_round_
-00011ec0: 7472 6970 5f6e 6f6e 655f 6173 5f73 716c  trip_none_as_sql
-00011ed0: 5f6e 756c 6c28 7365 6c66 293a 0a20 2020  _null(self):.   
-00011ee0: 2020 2020 2070 6173 730a 0a0a 636c 6173       pass...clas
-00011ef0: 7320 4578 6563 7574 696f 6e4f 7074 696f  s ExecutionOptio
-00011f00: 6e73 5265 7175 6573 7450 7269 6f72 6f74  nsRequestPriorot
-00011f10: 7954 6573 7428 6669 7874 7572 6573 2e54  yTest(fixtures.T
-00011f20: 6573 7442 6173 6529 3a0a 2020 2020 6465  estBase):.    de
-00011f30: 6620 7365 7455 7028 7365 6c66 293a 0a20  f setUp(self):. 
-00011f40: 2020 2020 2020 2073 656c 662e 5f65 6e67         self._eng
-00011f50: 696e 6520 3d20 6372 6561 7465 5f65 6e67  ine = create_eng
-00011f60: 696e 6528 6765 745f 6462 5f75 726c 2829  ine(get_db_url()
-00011f70: 2c20 706f 6f6c 5f73 697a 653d 3129 0a20  , pool_size=1). 
-00011f80: 2020 2020 2020 206d 6574 6164 6174 6120         metadata 
-00011f90: 3d20 4d65 7461 4461 7461 2862 696e 643d  = MetaData(bind=
-00011fa0: 7365 6c66 2e5f 656e 6769 6e65 290a 0a20  self._engine).. 
-00011fb0: 2020 2020 2020 2073 656c 662e 5f74 6162         self._tab
-00011fc0: 6c65 203d 2054 6162 6c65 280a 2020 2020  le = Table(.    
-00011fd0: 2020 2020 2020 2020 2265 7865 6375 7469          "executi
-00011fe0: 6f6e 5f6f 7074 696f 6e73 3222 2c0a 2020  on_options2",.  
-00011ff0: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
-00012000: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
-00012010: 436f 6c75 6d6e 2822 6f70 745f 6964 222c  Column("opt_id",
-00012020: 2049 6e74 6567 6572 2c20 7072 696d 6172   Integer, primar
-00012030: 795f 6b65 793d 5472 7565 292c 0a20 2020  y_key=True),.   
-00012040: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00012050: 226f 7074 5f6e 616d 6522 2c20 5374 7269  "opt_name", Stri
-00012060: 6e67 2831 3629 2c20 6e75 6c6c 6162 6c65  ng(16), nullable
-00012070: 3d46 616c 7365 292c 0a20 2020 2020 2020  =False),.       
-00012080: 2029 0a0a 2020 2020 2020 2020 6d65 7461   )..        meta
-00012090: 6461 7461 2e63 7265 6174 655f 616c 6c28  data.create_all(
-000120a0: 7365 6c66 2e5f 656e 6769 6e65 290a 2020  self._engine).  
-000120b0: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
-000120c0: 2831 290a 0a20 2020 2064 6566 2074 6573  (1)..    def tes
-000120d0: 745f 7265 7175 6573 745f 7072 696f 7269  t_request_priori
-000120e0: 7479 2873 656c 6629 3a0a 2020 2020 2020  ty(self):.      
-000120f0: 2020 5052 494f 5249 5459 203d 2052 6571    PRIORITY = Req
-00012100: 7565 7374 4f70 7469 6f6e 732e 5072 696f  uestOptions.Prio
-00012110: 7269 7479 2e50 5249 4f52 4954 595f 4d45  rity.PRIORITY_ME
-00012120: 4449 554d 0a20 2020 2020 2020 2077 6974  DIUM.        wit
-00012130: 6820 7365 6c66 2e5f 656e 6769 6e65 2e63  h self._engine.c
-00012140: 6f6e 6e65 6374 2829 2e65 7865 6375 7469  onnect().executi
-00012150: 6f6e 5f6f 7074 696f 6e73 280a 2020 2020  on_options(.    
-00012160: 2020 2020 2020 2020 7265 7175 6573 745f          request_
-00012170: 7072 696f 7269 7479 3d50 5249 4f52 4954  priority=PRIORIT
-00012180: 590a 2020 2020 2020 2020 2920 6173 2063  Y.        ) as c
-00012190: 6f6e 6e65 6374 696f 6e3a 0a20 2020 2020  onnection:.     
-000121a0: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
-000121b0: 6e2e 6578 6563 7574 6528 7365 6c65 6374  n.execute(select
-000121c0: 285b 222a 225d 2c20 6672 6f6d 5f6f 626a  (["*"], from_obj
-000121d0: 3d73 656c 662e 5f74 6162 6c65 2929 2e66  =self._table)).f
-000121e0: 6574 6368 616c 6c28 290a 0a20 2020 2020  etchall()..     
-000121f0: 2020 2077 6974 6820 7365 6c66 2e5f 656e     with self._en
-00012200: 6769 6e65 2e63 6f6e 6e65 6374 2829 2061  gine.connect() a
-00012210: 7320 636f 6e6e 6563 7469 6f6e 3a0a 2020  s connection:.  
-00012220: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00012230: 2063 6f6e 6e65 6374 696f 6e2e 636f 6e6e   connection.conn
-00012240: 6563 7469 6f6e 2e72 6571 7565 7374 5f70  ection.request_p
-00012250: 7269 6f72 6974 7920 6973 204e 6f6e 650a  riority is None.
-00012260: 0a20 2020 2020 2020 2065 6e67 696e 6520  .        engine 
-00012270: 3d20 6372 6561 7465 5f65 6e67 696e 6528  = create_engine(
-00012280: 2273 716c 6974 653a 2f2f 2f64 6174 6162  "sqlite:///datab
-00012290: 6173 6522 290a 2020 2020 2020 2020 7769  ase").        wi
-000122a0: 7468 2065 6e67 696e 652e 636f 6e6e 6563  th engine.connec
-000122b0: 7428 2920 6173 2063 6f6e 6e65 6374 696f  t() as connectio
-000122c0: 6e3a 0a20 2020 2020 2020 2020 2020 2070  n:.            p
-000122d0: 6173 730a 0a0a 636c 6173 7320 4372 6561  ass...class Crea
-000122e0: 7465 456e 6769 6e65 5769 7468 436c 6965  teEngineWithClie
-000122f0: 6e74 4f62 6a65 6374 5465 7374 2866 6978  ntObjectTest(fix
-00012300: 7475 7265 732e 5465 7374 4261 7365 293a  tures.TestBase):
-00012310: 0a20 2020 2064 6566 2074 6573 745f 6372  .    def test_cr
-00012320: 6561 7465 5f65 6e67 696e 655f 775f 7661  eate_engine_w_va
-00012330: 6c69 645f 636c 6965 6e74 5f6f 626a 6563  lid_client_objec
-00012340: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
-00012350: 2022 2222 0a20 2020 2020 2020 2053 5041   """.        SPA
-00012360: 4e4e 4552 2054 4553 543a 0a0a 2020 2020  NNER TEST:..    
-00012370: 2020 2020 4368 6563 6b20 7468 6174 2077      Check that w
-00012380: 6520 6361 6e20 636f 6e6e 6563 7420 746f  e can connect to
-00012390: 2053 716c 416c 6368 656d 790a 2020 2020   SqlAlchemy.    
-000123a0: 2020 2020 6279 2070 6173 7369 6e67 2063      by passing c
-000123b0: 7573 746f 6d20 436c 6965 6e74 206f 626a  ustom Client obj
-000123c0: 6563 742e 0a20 2020 2020 2020 2022 2222  ect..        """
-000123d0: 0a20 2020 2020 2020 2063 6c69 656e 7420  .        client 
-000123e0: 3d20 436c 6965 6e74 2870 726f 6a65 6374  = Client(project
-000123f0: 3d67 6574 5f70 726f 6a65 6374 2829 290a  =get_project()).
-00012400: 2020 2020 2020 2020 656e 6769 6e65 203d          engine =
-00012410: 2063 7265 6174 655f 656e 6769 6e65 2867   create_engine(g
-00012420: 6574 5f64 625f 7572 6c28 292c 2063 6f6e  et_db_url(), con
-00012430: 6e65 6374 5f61 7267 733d 7b22 636c 6965  nect_args={"clie
-00012440: 6e74 223a 2063 6c69 656e 747d 290a 2020  nt": client}).  
-00012450: 2020 2020 2020 7769 7468 2065 6e67 696e        with engin
-00012460: 652e 636f 6e6e 6563 7428 2920 6173 2063  e.connect() as c
-00012470: 6f6e 6e65 6374 696f 6e3a 0a20 2020 2020  onnection:.     
-00012480: 2020 2020 2020 2061 7373 6572 7420 636f         assert co
-00012490: 6e6e 6563 7469 6f6e 2e63 6f6e 6e65 6374  nnection.connect
-000124a0: 696f 6e2e 696e 7374 616e 6365 2e5f 636c  ion.instance._cl
-000124b0: 6965 6e74 203d 3d20 636c 6965 6e74 0a0a  ient == client..
-000124c0: 2020 2020 6465 6620 7465 7374 5f63 7265      def test_cre
-000124d0: 6174 655f 656e 6769 6e65 5f77 5f69 6e76  ate_engine_w_inv
-000124e0: 616c 6964 5f63 6c69 656e 745f 6f62 6a65  alid_client_obje
-000124f0: 6374 2873 656c 6629 3a0a 2020 2020 2020  ct(self):.      
-00012500: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
-00012510: 414e 4e45 5220 5445 5354 3a0a 0a20 2020  ANNER TEST:..   
-00012520: 2020 2020 2043 6865 636b 2074 6861 7420       Check that 
-00012530: 6966 2070 726f 6a65 6374 2069 6420 696e  if project id in
-00012540: 2075 726c 2061 6e64 2063 7573 746f 6d20   url and custom 
-00012550: 436c 6965 6e74 0a20 2020 2020 2020 204f  Client.        O
-00012560: 626a 6563 7420 7061 7373 6564 2074 6f20  bject passed to 
-00012570: 656e 6769 6e65 7220 6d69 736d 6174 6368  enginer mismatch
-00012580: 2c20 6572 726f 7220 6973 2074 6872 6f77  , error is throw
-00012590: 6e2e 0a20 2020 2020 2020 2022 2222 0a20  n..        """. 
-000125a0: 2020 2020 2020 2063 6c69 656e 7420 3d20         client = 
-000125b0: 436c 6965 6e74 2870 726f 6a65 6374 3d22  Client(project="
-000125c0: 7072 6f6a 6563 745f 6964 2229 0a20 2020  project_id").   
-000125d0: 2020 2020 2065 6e67 696e 6520 3d20 6372       engine = cr
-000125e0: 6561 7465 5f65 6e67 696e 6528 6765 745f  eate_engine(get_
-000125f0: 6462 5f75 726c 2829 2c20 636f 6e6e 6563  db_url(), connec
-00012600: 745f 6172 6773 3d7b 2263 6c69 656e 7422  t_args={"client"
-00012610: 3a20 636c 6965 6e74 7d29 0a0a 2020 2020  : client})..    
-00012620: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
-00012630: 7261 6973 6573 2856 616c 7565 4572 726f  raises(ValueErro
-00012640: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00012650: 656e 6769 6e65 2e63 6f6e 6e65 6374 2829  engine.connect()
-00012660: 0a                                       .
+0000b370: 2022 756e 6963 6f64 655f 7461 626c 6522   "unicode_table"
+0000b380: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
+0000b390: 7461 6461 7461 2c0a 2020 2020 2020 2020  tadata,.        
+0000b3a0: 2020 2020 436f 6c75 6d6e 2822 6964 222c      Column("id",
+0000b3b0: 2049 6e74 6567 6572 2c20 7072 696d 6172   Integer, primar
+0000b3c0: 795f 6b65 793d 5472 7565 2c20 6e75 6c6c  y_key=True, null
+0000b3d0: 6162 6c65 3d54 7275 6529 2c0a 2020 2020  able=True),.    
+0000b3e0: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+0000b3f0: 756e 6963 6f64 655f 6461 7461 222c 2063  unicode_data", c
+0000b400: 6c73 2e64 6174 6174 7970 6529 2c0a 2020  ls.datatype),.  
+0000b410: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+0000b420: 2074 6573 745f 726f 756e 645f 7472 6970   test_round_trip
+0000b430: 5f65 7865 6375 7465 6d61 6e79 2873 656c  _executemany(sel
+0000b440: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+0000b450: 2020 2020 2020 2020 5350 414e 4e45 5220          SPANNER 
+0000b460: 4f56 4552 5249 4445 0a0a 2020 2020 2020  OVERRIDE..      
+0000b470: 2020 436c 6f75 6420 5370 616e 6e65 7220    Cloud Spanner 
+0000b480: 7375 7070 6f72 7473 2074 6162 6c65 7320  supports tables 
+0000b490: 7769 7468 2065 6d70 7479 2070 7269 6d61  with empty prima
+0000b4a0: 7279 206b 6579 2c20 6275 740a 2020 2020  ry key, but.    
+0000b4b0: 2020 2020 6f6e 6c79 2073 696e 676c 6520      only single 
+0000b4c0: 6f6e 6520 726f 7720 6361 6e20 6265 2069  one row can be i
+0000b4d0: 6e73 6572 7465 6420 696e 746f 2073 7563  nserted into suc
+0000b4e0: 6820 6120 7461 626c 6520 2d0a 2020 2020  h a table -.    
+0000b4f0: 2020 2020 666f 6c6c 6f77 696e 6720 696e      following in
+0000b500: 7365 7274 696f 6e73 2077 696c 6c20 6661  sertions will fa
+0000b510: 696c 2077 6974 6820 6052 6f77 205b 5d20  il with `Row [] 
+0000b520: 616c 7265 6164 7920 6578 6973 7473 222e  already exists".
+0000b530: 0a20 2020 2020 2020 204f 7665 7272 6964  .        Overrid
+0000b540: 696e 6720 7468 6520 7465 7374 2074 6f20  ing the test to 
+0000b550: 6176 6f69 6420 7468 6520 7361 6d65 2066  avoid the same f
+0000b560: 6169 6c75 7265 2e0a 2020 2020 2020 2020  ailure..        
+0000b570: 2222 220a 2020 2020 2020 2020 756e 6963  """.        unic
+0000b580: 6f64 655f 7461 626c 6520 3d20 7365 6c66  ode_table = self
+0000b590: 2e74 6162 6c65 732e 756e 6963 6f64 655f  .tables.unicode_
+0000b5a0: 7461 626c 650a 0a20 2020 2020 2020 2063  table..        c
+0000b5b0: 6f6e 6669 672e 6462 2e65 7865 6375 7465  onfig.db.execute
+0000b5c0: 280a 2020 2020 2020 2020 2020 2020 756e  (.            un
+0000b5d0: 6963 6f64 655f 7461 626c 652e 696e 7365  icode_table.inse
+0000b5e0: 7274 2829 2c0a 2020 2020 2020 2020 2020  rt(),.          
+0000b5f0: 2020 5b7b 2269 6422 3a20 692c 2022 756e    [{"id": i, "un
+0000b600: 6963 6f64 655f 6461 7461 223a 2073 656c  icode_data": sel
+0000b610: 662e 6461 7461 7d20 666f 7220 6920 696e  f.data} for i in
+0000b620: 2072 616e 6765 2833 295d 2c0a 2020 2020   range(3)],.    
+0000b630: 2020 2020 290a 0a20 2020 2020 2020 2072      )..        r
+0000b640: 6f77 7320 3d20 636f 6e66 6967 2e64 622e  ows = config.db.
+0000b650: 6578 6563 7574 6528 7365 6c65 6374 285b  execute(select([
+0000b660: 756e 6963 6f64 655f 7461 626c 652e 632e  unicode_table.c.
+0000b670: 756e 6963 6f64 655f 6461 7461 5d29 292e  unicode_data])).
+0000b680: 6665 7463 6861 6c6c 2829 0a20 2020 2020  fetchall().     
+0000b690: 2020 2065 715f 2872 6f77 732c 205b 2873     eq_(rows, [(s
+0000b6a0: 656c 662e 6461 7461 2c29 2066 6f72 2069  elf.data,) for i
+0000b6b0: 2069 6e20 7261 6e67 6528 3329 5d29 0a20   in range(3)]). 
+0000b6c0: 2020 2020 2020 2066 6f72 2072 6f77 2069         for row i
+0000b6d0: 6e20 726f 7773 3a0a 2020 2020 2020 2020  n rows:.        
+0000b6e0: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+0000b6f0: 7461 6e63 6528 726f 775b 305d 2c20 7574  tance(row[0], ut
+0000b700: 696c 2e74 6578 745f 7479 7065 290a 0a20  il.text_type).. 
+0000b710: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+0000b720: 736b 6970 2822 5370 616e 6e65 7220 646f  skip("Spanner do
+0000b730: 6573 6e27 7420 7375 7070 6f72 7420 6e6f  esn't support no
+0000b740: 6e2d 6173 6369 6920 6368 6172 6163 7465  n-ascii characte
+0000b750: 7273 2229 0a20 2020 2064 6566 2074 6573  rs").    def tes
+0000b760: 745f 6c69 7465 7261 6c28 7365 6c66 293a  t_literal(self):
+0000b770: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+0000b780: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+0000b790: 736b 6970 2822 5370 616e 6e65 7220 646f  skip("Spanner do
+0000b7a0: 6573 6e27 7420 7375 7070 6f72 7420 6e6f  esn't support no
+0000b7b0: 6e2d 6173 6369 6920 6368 6172 6163 7465  n-ascii characte
+0000b7c0: 7273 2229 0a20 2020 2064 6566 2074 6573  rs").    def tes
+0000b7d0: 745f 6c69 7465 7261 6c5f 6e6f 6e5f 6173  t_literal_non_as
+0000b7e0: 6369 6928 7365 6c66 293a 0a20 2020 2020  cii(self):.     
+0000b7f0: 2020 2070 6173 730a 0a0a 636c 6173 7320     pass...class 
+0000b800: 556e 6963 6f64 6556 6172 6368 6172 5465  UnicodeVarcharTe
+0000b810: 7374 285f 556e 6963 6f64 6546 6978 7475  st(_UnicodeFixtu
+0000b820: 7265 2c20 5f55 6e69 636f 6465 5661 7263  re, _UnicodeVarc
+0000b830: 6861 7254 6573 7429 3a0a 2020 2020 2222  harTest):.    ""
+0000b840: 220a 2020 2020 5350 414e 4e45 5220 4f56  ".    SPANNER OV
+0000b850: 4552 5249 4445 3a0a 0a20 2020 2055 6e69  ERRIDE:..    Uni
+0000b860: 636f 6465 5661 7263 6861 7254 6573 7420  codeVarcharTest 
+0000b870: 636c 6173 7320 696e 6865 7269 7473 2074  class inherits t
+0000b880: 6865 205f 5f55 6e69 636f 6465 4669 7874  he __UnicodeFixt
+0000b890: 7572 6520 636c 6173 7327 7320 7465 7374  ure class's test
+0000b8a0: 732c 0a20 2020 2073 6f20 746f 2061 766f  s,.    so to avo
+0000b8b0: 6964 2074 686f 7365 2066 6169 6c75 7265  id those failure
+0000b8c0: 7320 616e 6420 6d61 696e 7461 696e 2044  s and maintain D
+0000b8d0: 5259 2063 6f6e 6365 7074 206a 7573 7420  RY concept just 
+0000b8e0: 696e 6865 7269 7420 7468 6520 636c 6173  inherit the clas
+0000b8f0: 7320 746f 2072 756e 0a20 2020 2074 6573  s to run.    tes
+0000b900: 7473 2073 7563 6365 7373 6675 6c6c 792e  ts successfully.
+0000b910: 0a20 2020 2022 2222 0a0a 2020 2020 7061  .    """..    pa
+0000b920: 7373 0a0a 0a63 6c61 7373 2055 6e69 636f  ss...class Unico
+0000b930: 6465 5465 7874 5465 7374 285f 556e 6963  deTextTest(_Unic
+0000b940: 6f64 6546 6978 7475 7265 2c20 5f55 6e69  odeFixture, _Uni
+0000b950: 636f 6465 5465 7874 5465 7374 293a 0a20  codeTextTest):. 
+0000b960: 2020 2022 2222 0a20 2020 2053 5041 4e4e     """.    SPANN
+0000b970: 4552 204f 5645 5252 4944 453a 0a0a 2020  ER OVERRIDE:..  
+0000b980: 2020 556e 6963 6f64 6554 6578 7454 6573    UnicodeTextTes
+0000b990: 7420 636c 6173 7320 696e 6865 7269 7473  t class inherits
+0000b9a0: 2074 6865 205f 5f55 6e69 636f 6465 4669   the __UnicodeFi
+0000b9b0: 7874 7572 6520 636c 6173 7327 7320 7465  xture class's te
+0000b9c0: 7374 732c 0a20 2020 2073 6f20 746f 2061  sts,.    so to a
+0000b9d0: 766f 6964 2074 686f 7365 2066 6169 6c75  void those failu
+0000b9e0: 7265 7320 616e 6420 6d61 696e 7461 696e  res and maintain
+0000b9f0: 2044 5259 2063 6f6e 6365 7074 206a 7573   DRY concept jus
+0000ba00: 7420 696e 6865 7269 7420 7468 6520 636c  t inherit the cl
+0000ba10: 6173 7320 746f 2072 756e 0a20 2020 2074  ass to run.    t
+0000ba20: 6573 7473 2073 7563 6365 7373 6675 6c6c  ests successfull
+0000ba30: 792e 0a20 2020 2022 2222 0a0a 2020 2020  y..    """..    
+0000ba40: 7061 7373 0a0a 0a63 6c61 7373 2052 6f77  pass...class Row
+0000ba50: 4665 7463 6854 6573 7428 5f52 6f77 4665  FetchTest(_RowFe
+0000ba60: 7463 6854 6573 7429 3a0a 2020 2020 6465  tchTest):.    de
+0000ba70: 6620 7465 7374 5f72 6f77 5f77 5f73 6361  f test_row_w_sca
+0000ba80: 6c61 725f 7365 6c65 6374 2873 656c 6629  lar_select(self)
+0000ba90: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000baa0: 2020 2020 2020 5350 414e 4e45 5220 4f56        SPANNER OV
+0000bab0: 4552 5249 4445 3a0a 0a20 2020 2020 2020  ERRIDE:..       
+0000bac0: 2043 6c6f 7564 2053 7061 6e6e 6572 2072   Cloud Spanner r
+0000bad0: 6574 7572 6e73 2061 2044 6174 6574 696d  eturns a Datetim
+0000bae0: 6557 6974 684e 616e 6f73 6563 6f6e 6473  eWithNanoseconds
+0000baf0: 2829 2066 6f72 2064 6174 650a 2020 2020  () for date.    
+0000bb00: 2020 2020 6461 7461 2074 7970 6573 2e20      data types. 
+0000bb10: 4f76 6572 7269 6469 6e67 2074 6865 2074  Overriding the t
+0000bb20: 6573 7420 746f 2075 7365 2061 2044 6174  est to use a Dat
+0000bb30: 6574 696d 6557 6974 684e 616e 6f73 6563  etimeWithNanosec
+0000bb40: 6f6e 6473 0a20 2020 2020 2020 2074 7970  onds.        typ
+0000bb50: 6520 7661 6c75 6520 6173 2061 6e20 6578  e value as an ex
+0000bb60: 7065 6374 6564 2072 6573 756c 742e 0a20  pected result.. 
+0000bb70: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000bb80: 2d2d 2d2d 2d0a 0a20 2020 2020 2020 2074  -----..        t
+0000bb90: 6573 7420 7468 6174 2061 2073 6361 6c61  est that a scala
+0000bba0: 7220 7365 6c65 6374 2061 7320 6120 636f  r select as a co
+0000bbb0: 6c75 6d6e 2069 7320 7265 7475 726e 6564  lumn is returned
+0000bbc0: 2061 7320 7375 6368 0a20 2020 2020 2020   as such.       
+0000bbd0: 2061 6e64 2074 6861 7420 7479 7065 2063   and that type c
+0000bbe0: 6f6e 7665 7273 696f 6e20 776f 726b 7320  onversion works 
+0000bbf0: 4f4b 2e0a 0a20 2020 2020 2020 2028 7468  OK...        (th
+0000bc00: 6973 2069 7320 6861 6c66 2061 2053 514c  is is half a SQL
+0000bc10: 416c 6368 656d 7920 436f 7265 2074 6573  Alchemy Core tes
+0000bc20: 7420 616e 6420 6861 6c66 2074 6f20 6361  t and half to ca
+0000bc30: 7463 6820 6461 7461 6261 7365 0a20 2020  tch database.   
+0000bc40: 2020 2020 2062 6163 6b65 6e64 7320 7468       backends th
+0000bc50: 6174 206d 6179 2068 6176 6520 756e 7573  at may have unus
+0000bc60: 7561 6c20 6265 6861 7669 6f72 2077 6974  ual behavior wit
+0000bc70: 6820 7363 616c 6172 2073 656c 6563 7473  h scalar selects
+0000bc80: 2e29 0a20 2020 2020 2020 2022 2222 0a20  .).        """. 
+0000bc90: 2020 2020 2020 2064 6174 6574 6162 6c65         datetable
+0000bca0: 203d 2073 656c 662e 7461 626c 6573 2e68   = self.tables.h
+0000bcb0: 6173 5f64 6174 6573 0a20 2020 2020 2020  as_dates.       
+0000bcc0: 2073 203d 2073 656c 6563 7428 5b64 6174   s = select([dat
+0000bcd0: 6574 6162 6c65 2e61 6c69 6173 2822 7822  etable.alias("x"
+0000bce0: 292e 632e 746f 6461 795d 292e 7363 616c  ).c.today]).scal
+0000bcf0: 6172 5f73 7562 7175 6572 7928 290a 2020  ar_subquery().  
+0000bd00: 2020 2020 2020 7332 203d 2073 656c 6563        s2 = selec
+0000bd10: 7428 5b64 6174 6574 6162 6c65 2e63 2e69  t([datetable.c.i
+0000bd20: 642c 2073 2e6c 6162 656c 2822 736f 6d65  d, s.label("some
+0000bd30: 6c61 6265 6c22 295d 290a 2020 2020 2020  label")]).      
+0000bd40: 2020 726f 7720 3d20 636f 6e66 6967 2e64    row = config.d
+0000bd50: 622e 6578 6563 7574 6528 7332 292e 6669  b.execute(s2).fi
+0000bd60: 7273 7428 290a 0a20 2020 2020 2020 2065  rst()..        e
+0000bd70: 715f 280a 2020 2020 2020 2020 2020 2020  q_(.            
+0000bd80: 726f 775b 2273 6f6d 656c 6162 656c 225d  row["somelabel"]
+0000bd90: 2c0a 2020 2020 2020 2020 2020 2020 4461  ,.            Da
+0000bda0: 7465 7469 6d65 5769 7468 4e61 6e6f 7365  tetimeWithNanose
+0000bdb0: 636f 6e64 7328 3230 3036 2c20 352c 2031  conds(2006, 5, 1
+0000bdc0: 322c 2031 322c 2030 2c20 302c 2074 7a69  2, 12, 0, 0, tzi
+0000bdd0: 6e66 6f3d 7469 6d65 7a6f 6e65 2e75 7463  nfo=timezone.utc
+0000bde0: 292c 0a20 2020 2020 2020 2029 0a0a 0a63  ),.        )...c
+0000bdf0: 6c61 7373 2049 6e73 6572 7442 6568 6176  lass InsertBehav
+0000be00: 696f 7254 6573 7428 5f49 6e73 6572 7442  iorTest(_InsertB
+0000be10: 6568 6176 696f 7254 6573 7429 3a0a 2020  ehaviorTest):.  
+0000be20: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+0000be30: 6b69 7028 2253 7061 6e6e 6572 2064 6f65  kip("Spanner doe
+0000be40: 736e 2774 2073 7570 706f 7274 2065 6d70  sn't support emp
+0000be50: 7479 2069 6e73 6572 7473 2229 0a20 2020  ty inserts").   
+0000be60: 2064 6566 2074 6573 745f 656d 7074 795f   def test_empty_
+0000be70: 696e 7365 7274 2873 656c 6629 3a0a 2020  insert(self):.  
+0000be80: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+0000be90: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+0000bea0: 7028 2253 7061 6e6e 6572 2064 6f65 736e  p("Spanner doesn
+0000beb0: 2774 2073 7570 706f 7274 2065 6d70 7479  't support empty
+0000bec0: 2069 6e73 6572 7473 2229 0a20 2020 2064   inserts").    d
+0000bed0: 6566 2074 6573 745f 656d 7074 795f 696e  ef test_empty_in
+0000bee0: 7365 7274 5f6d 756c 7469 706c 6528 7365  sert_multiple(se
+0000bef0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+0000bf00: 730a 0a20 2020 2040 7079 7465 7374 2e6d  s..    @pytest.m
+0000bf10: 6172 6b2e 736b 6970 2822 5370 616e 6e65  ark.skip("Spanne
+0000bf20: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
+0000bf30: 7420 6175 746f 2069 6e63 7265 6d65 6e74  t auto increment
+0000bf40: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
+0000bf50: 696e 7365 7274 5f66 726f 6d5f 7365 6c65  insert_from_sele
+0000bf60: 6374 5f61 7574 6f69 6e63 2873 656c 6629  ct_autoinc(self)
+0000bf70: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+0000bf80: 2020 2020 6465 6620 7465 7374 5f61 7574      def test_aut
+0000bf90: 6f63 6c6f 7365 5f6f 6e5f 696e 7365 7274  oclose_on_insert
+0000bfa0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000bfb0: 2222 220a 2020 2020 2020 2020 5350 414e  """.        SPAN
+0000bfc0: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
+0000bfd0: 2020 2020 2020 2043 6c6f 7564 2053 7061         Cloud Spa
+0000bfe0: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
+0000bff0: 706f 7274 2074 6162 6c65 7320 7769 7468  port tables with
+0000c000: 2061 6e20 6175 746f 2069 6e63 7265 6d65   an auto increme
+0000c010: 6e74 2070 7269 6d61 7279 206b 6579 2c0a  nt primary key,.
+0000c020: 2020 2020 2020 2020 666f 6c6c 6f77 696e          followin
+0000c030: 6720 696e 7365 7274 696f 6e73 2077 696c  g insertions wil
+0000c040: 6c20 6661 696c 2077 6974 6820 6034 3030  l fail with `400
+0000c050: 2069 6420 6d75 7374 206e 6f74 2062 6520   id must not be 
+0000c060: 4e55 4c4c 2069 6e20 7461 626c 650a 2020  NULL in table.  
+0000c070: 2020 2020 2020 6175 746f 696e 635f 706b        autoinc_pk
+0000c080: 602e 0a0a 2020 2020 2020 2020 4f76 6572  `...        Over
+0000c090: 7269 6469 6e67 2074 6865 2074 6573 7473  riding the tests
+0000c0a0: 2061 6e64 2061 6464 696e 6720 6120 6d61   and adding a ma
+0000c0b0: 6e75 616c 2070 7269 6d61 7279 206b 6579  nual primary key
+0000c0c0: 2076 616c 7565 2074 6f20 6176 6f69 6420   value to avoid 
+0000c0d0: 7468 6520 7361 6d65 0a20 2020 2020 2020  the same.       
+0000c0e0: 2066 6169 6c75 7265 732e 0a20 2020 2020   failures..     
+0000c0f0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+0000c100: 6620 636f 6e66 6967 2e72 6571 7569 7265  f config.require
+0000c110: 6d65 6e74 732e 7265 7475 726e 696e 672e  ments.returning.
+0000c120: 656e 6162 6c65 643a 0a20 2020 2020 2020  enabled:.       
+0000c130: 2020 2020 2065 6e67 696e 6520 3d20 656e       engine = en
+0000c140: 6769 6e65 732e 7465 7374 696e 675f 656e  gines.testing_en
+0000c150: 6769 6e65 286f 7074 696f 6e73 3d7b 2269  gine(options={"i
+0000c160: 6d70 6c69 6369 745f 7265 7475 726e 696e  mplicit_returnin
+0000c170: 6722 3a20 4661 6c73 657d 290a 2020 2020  g": False}).    
+0000c180: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000c190: 2020 2020 2020 656e 6769 6e65 203d 2063        engine = c
+0000c1a0: 6f6e 6669 672e 6462 0a0a 2020 2020 2020  onfig.db..      
+0000c1b0: 2020 7769 7468 2065 6e67 696e 652e 6265    with engine.be
+0000c1c0: 6769 6e28 2920 6173 2063 6f6e 6e3a 0a20  gin() as conn:. 
+0000c1d0: 2020 2020 2020 2020 2020 2072 203d 2063             r = c
+0000c1e0: 6f6e 6e2e 6578 6563 7574 6528 0a20 2020  onn.execute(.   
+0000c1f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c200: 662e 7461 626c 6573 2e61 7574 6f69 6e63  f.tables.autoinc
+0000c210: 5f70 6b2e 696e 7365 7274 2829 2c20 6469  _pk.insert(), di
+0000c220: 6374 2869 643d 312c 2064 6174 613d 2273  ct(id=1, data="s
+0000c230: 6f6d 6520 6461 7461 2229 0a20 2020 2020  ome data").     
+0000c240: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000c250: 2020 6173 7365 7274 2072 2e5f 736f 6674    assert r._soft
+0000c260: 5f63 6c6f 7365 640a 2020 2020 2020 2020  _closed.        
+0000c270: 6173 7365 7274 206e 6f74 2072 2e63 6c6f  assert not r.clo
+0000c280: 7365 640a 2020 2020 2020 2020 6173 7365  sed.        asse
+0000c290: 7274 2072 2e69 735f 696e 7365 7274 0a20  rt r.is_insert. 
+0000c2a0: 2020 2020 2020 2061 7373 6572 7420 6e6f         assert no
+0000c2b0: 7420 722e 7265 7475 726e 735f 726f 7773  t r.returns_rows
+0000c2c0: 0a0a 0a63 6c61 7373 2042 7974 6573 5465  ...class BytesTe
+0000c2d0: 7374 285f 4c69 7465 7261 6c52 6f75 6e64  st(_LiteralRound
+0000c2e0: 5472 6970 4669 7874 7572 652c 2066 6978  TripFixture, fix
+0000c2f0: 7475 7265 732e 5465 7374 4261 7365 293a  tures.TestBase):
+0000c300: 0a20 2020 205f 5f62 6163 6b65 6e64 5f5f  .    __backend__
+0000c310: 203d 2054 7275 650a 0a20 2020 2064 6566   = True..    def
+0000c320: 2074 6573 745f 6e6f 6c65 6e67 7468 5f62   test_nolength_b
+0000c330: 696e 6172 7928 7365 6c66 293a 0a20 2020  inary(self):.   
+0000c340: 2020 2020 206d 6574 6164 6174 6120 3d20       metadata = 
+0000c350: 4d65 7461 4461 7461 2829 0a20 2020 2020  MetaData().     
+0000c360: 2020 2066 6f6f 203d 2054 6162 6c65 2822     foo = Table("
+0000c370: 666f 6f22 2c20 6d65 7461 6461 7461 2c20  foo", metadata, 
+0000c380: 436f 6c75 6d6e 2822 6f6e 6522 2c20 4c61  Column("one", La
+0000c390: 7267 6542 696e 6172 7929 290a 0a20 2020  rgeBinary))..   
+0000c3a0: 2020 2020 2066 6f6f 2e63 7265 6174 6528       foo.create(
+0000c3b0: 636f 6e66 6967 2e64 6229 0a20 2020 2020  config.db).     
+0000c3c0: 2020 2066 6f6f 2e64 726f 7028 636f 6e66     foo.drop(conf
+0000c3d0: 6967 2e64 6229 0a0a 0a63 6c61 7373 2053  ig.db)...class S
+0000c3e0: 7472 696e 6754 6573 7428 5f53 7472 696e  tringTest(_Strin
+0000c3f0: 6754 6573 7429 3a0a 2020 2020 4070 7974  gTest):.    @pyt
+0000c400: 6573 742e 6d61 726b 2e73 6b69 7028 2253  est.mark.skip("S
+0000c410: 7061 6e6e 6572 2064 6f65 736e 2774 2073  panner doesn't s
+0000c420: 7570 706f 7274 206e 6f6e 2d61 7363 6969  upport non-ascii
+0000c430: 2063 6861 7261 6374 6572 7322 290a 2020   characters").  
+0000c440: 2020 6465 6620 7465 7374 5f6c 6974 6572    def test_liter
+0000c450: 616c 5f6e 6f6e 5f61 7363 6969 2873 656c  al_non_ascii(sel
+0000c460: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+0000c470: 0a0a 0a63 6c61 7373 2054 6578 7454 6573  ...class TextTes
+0000c480: 7428 5f54 6578 7454 6573 7429 3a0a 2020  t(_TextTest):.  
+0000c490: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+0000c4a0: 2020 2064 6566 2064 6566 696e 655f 7461     def define_ta
+0000c4b0: 626c 6573 2863 6c73 2c20 6d65 7461 6461  bles(cls, metada
+0000c4c0: 7461 293a 0a20 2020 2020 2020 2022 2222  ta):.        """
+0000c4d0: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
+0000c4e0: 204f 5645 5252 4944 453a 0a0a 2020 2020   OVERRIDE:..    
+0000c4f0: 2020 2020 436c 6f75 6420 5370 616e 6e65      Cloud Spanne
+0000c500: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
+0000c510: 7420 6175 746f 2069 6e63 7265 6d65 6e74  t auto increment
+0000c520: 696e 6720 6964 7320 6665 6174 7572 652c  ing ids feature,
+0000c530: 0a20 2020 2020 2020 2077 6869 6368 2069  .        which i
+0000c540: 7320 7573 6564 2062 7920 7468 6520 6f72  s used by the or
+0000c550: 6967 696e 616c 2074 6573 742e 204f 7665  iginal test. Ove
+0000c560: 7272 6964 696e 6720 7468 6520 7465 7374  rriding the test
+0000c570: 2064 6174 610a 2020 2020 2020 2020 6372   data.        cr
+0000c580: 6561 7469 6f6e 206d 6574 686f 6420 746f  eation method to
+0000c590: 2064 6973 6162 6c65 2061 7574 6f69 6e63   disable autoinc
+0000c5a0: 7265 6d65 6e74 2061 6e64 206d 616b 6520  rement and make 
+0000c5b0: 6964 2063 6f6c 756d 6e0a 2020 2020 2020  id column.      
+0000c5c0: 2020 6e75 6c6c 6162 6c65 2e0a 2020 2020    nullable..    
+0000c5d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000c5e0: 5461 626c 6528 0a20 2020 2020 2020 2020  Table(.         
+0000c5f0: 2020 2022 7465 7874 5f74 6162 6c65 222c     "text_table",
+0000c600: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+0000c610: 6164 6174 612c 0a20 2020 2020 2020 2020  adata,.         
+0000c620: 2020 2043 6f6c 756d 6e28 2269 6422 2c20     Column("id", 
+0000c630: 496e 7465 6765 722c 2070 7269 6d61 7279  Integer, primary
+0000c640: 5f6b 6579 3d54 7275 652c 206e 756c 6c61  _key=True, nulla
+0000c650: 626c 653d 5472 7565 292c 0a20 2020 2020  ble=True),.     
+0000c660: 2020 2020 2020 2043 6f6c 756d 6e28 2274         Column("t
+0000c670: 6578 745f 6461 7461 222c 2054 6578 7429  ext_data", Text)
+0000c680: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+0000c690: 2040 7079 7465 7374 2e6d 6172 6b2e 736b   @pytest.mark.sk
+0000c6a0: 6970 2822 5370 616e 6e65 7220 646f 6573  ip("Spanner does
+0000c6b0: 6e27 7420 7375 7070 6f72 7420 6e6f 6e2d  n't support non-
+0000c6c0: 6173 6369 6920 6368 6172 6163 7465 7273  ascii characters
+0000c6d0: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
+0000c6e0: 6c69 7465 7261 6c5f 6e6f 6e5f 6173 6369  literal_non_asci
+0000c6f0: 6928 7365 6c66 293a 0a20 2020 2020 2020  i(self):.       
+0000c700: 2070 6173 730a 0a20 2020 2040 7079 7465   pass..    @pyte
+0000c710: 7374 2e6d 6172 6b2e 736b 6970 2822 4e6f  st.mark.skip("No
+0000c720: 7420 7375 7070 6f72 7465 6420 6279 2053  t supported by S
+0000c730: 7061 6e6e 6572 2229 0a20 2020 2064 6566  panner").    def
+0000c740: 2074 6573 745f 7465 7874 5f72 6f75 6e64   test_text_round
+0000c750: 7472 6970 2873 656c 662c 2063 6f6e 6e65  trip(self, conne
+0000c760: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
+0000c770: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
+0000c780: 742e 6d61 726b 2e73 6b69 7028 224e 6f74  t.mark.skip("Not
+0000c790: 2073 7570 706f 7274 6564 2062 7920 5370   supported by Sp
+0000c7a0: 616e 6e65 7222 290a 2020 2020 6465 6620  anner").    def 
+0000c7b0: 7465 7374 5f74 6578 745f 656d 7074 795f  test_text_empty_
+0000c7c0: 7374 7269 6e67 7328 7365 6c66 2c20 636f  strings(self, co
+0000c7d0: 6e6e 6563 7469 6f6e 293a 0a20 2020 2020  nnection):.     
+0000c7e0: 2020 2070 6173 730a 0a20 2020 2040 7079     pass..    @py
+0000c7f0: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
+0000c800: 4e6f 7420 7375 7070 6f72 7465 6420 6279  Not supported by
+0000c810: 2053 7061 6e6e 6572 2229 0a20 2020 2064   Spanner").    d
+0000c820: 6566 2074 6573 745f 7465 7874 5f6e 756c  ef test_text_nul
+0000c830: 6c5f 7374 7269 6e67 7328 7365 6c66 2c20  l_strings(self, 
+0000c840: 636f 6e6e 6563 7469 6f6e 293a 0a20 2020  connection):.   
+0000c850: 2020 2020 2070 6173 730a 0a0a 636c 6173       pass...clas
+0000c860: 7320 4e75 6d65 7269 6354 6573 7428 5f4e  s NumericTest(_N
+0000c870: 756d 6572 6963 5465 7374 293a 0a20 2020  umericTest):.   
+0000c880: 2040 7465 7374 696e 672e 6669 7874 7572   @testing.fixtur
+0000c890: 650a 2020 2020 6465 6620 646f 5f6e 756d  e.    def do_num
+0000c8a0: 6572 6963 5f74 6573 7428 7365 6c66 2c20  eric_test(self, 
+0000c8b0: 6d65 7461 6461 7461 2c20 636f 6e6e 6563  metadata, connec
+0000c8c0: 7469 6f6e 293a 0a20 2020 2020 2020 2040  tion):.        @
+0000c8d0: 7465 7374 696e 672e 656d 6974 735f 7761  testing.emits_wa
+0000c8e0: 726e 696e 6728 7222 2e2a 646f 6573 205c  rning(r".*does \
+0000c8f0: 2a6e 6f74 5c2a 2073 7570 706f 7274 2044  *not\* support D
+0000c900: 6563 696d 616c 206f 626a 6563 7473 206e  ecimal objects n
+0000c910: 6174 6976 656c 7922 290a 2020 2020 2020  atively").      
+0000c920: 2020 6465 6620 7275 6e28 7479 7065 5f2c    def run(type_,
+0000c930: 2069 6e70 7574 5f2c 206f 7574 7075 742c   input_, output,
+0000c940: 2066 696c 7465 725f 3d4e 6f6e 652c 2063   filter_=None, c
+0000c950: 6865 636b 5f73 6361 6c65 3d46 616c 7365  heck_scale=False
+0000c960: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
+0000c970: 203d 2054 6162 6c65 280a 2020 2020 2020   = Table(.      
+0000c980: 2020 2020 2020 2020 2020 2274 222c 0a20            "t",. 
+0000c990: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000c9a0: 6574 6164 6174 612c 0a20 2020 2020 2020  etadata,.       
+0000c9b0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+0000c9c0: 2278 222c 2074 7970 655f 292c 0a20 2020  "x", type_),.   
+0000c9d0: 2020 2020 2020 2020 2020 2020 2043 6f6c               Col
+0000c9e0: 756d 6e28 2269 6422 2c20 496e 7465 6765  umn("id", Intege
+0000c9f0: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
+0000ca00: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
+0000ca10: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000ca20: 742e 6372 6561 7465 2863 6f6e 6e65 6374  t.create(connect
+0000ca30: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
+0000ca40: 2063 6f6e 6e65 6374 696f 6e2e 636f 6e6e   connection.conn
+0000ca50: 6563 7469 6f6e 2e63 6f6d 6d69 7428 290a  ection.commit().
+0000ca60: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
+0000ca70: 6563 7469 6f6e 2e65 7865 6375 7465 280a  ection.execute(.
+0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca90: 742e 696e 7365 7274 2829 2c20 5b7b 2278  t.insert(), [{"x
+0000caa0: 223a 2078 2c20 2269 6422 3a20 697d 2066  ": x, "id": i} f
+0000cab0: 6f72 2069 2c20 7820 696e 2065 6e75 6d65  or i, x in enume
+0000cac0: 7261 7465 2869 6e70 7574 5f29 5d0a 2020  rate(input_)].  
+0000cad0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000cae0: 2020 2020 2020 2020 2072 6573 756c 7420           result 
+0000caf0: 3d20 7b72 6f77 5b30 5d20 666f 7220 726f  = {row[0] for ro
+0000cb00: 7720 696e 2063 6f6e 6e65 6374 696f 6e2e  w in connection.
+0000cb10: 6578 6563 7574 6528 742e 7365 6c65 6374  execute(t.select
+0000cb20: 2829 297d 0a20 2020 2020 2020 2020 2020  ())}.           
+0000cb30: 206f 7574 7075 7420 3d20 7365 7428 6f75   output = set(ou
+0000cb40: 7470 7574 290a 2020 2020 2020 2020 2020  tput).          
+0000cb50: 2020 6966 2066 696c 7465 725f 3a0a 2020    if filter_:.  
+0000cb60: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000cb70: 7375 6c74 203d 2073 6574 2866 696c 7465  sult = set(filte
+0000cb80: 725f 2878 2920 666f 7220 7820 696e 2072  r_(x) for x in r
+0000cb90: 6573 756c 7429 0a20 2020 2020 2020 2020  esult).         
+0000cba0: 2020 2020 2020 206f 7574 7075 7420 3d20         output = 
+0000cbb0: 7365 7428 6669 6c74 6572 5f28 7829 2066  set(filter_(x) f
+0000cbc0: 6f72 2078 2069 6e20 6f75 7470 7574 290a  or x in output).
+0000cbd0: 2020 2020 2020 2020 2020 2020 6571 5f28              eq_(
+0000cbe0: 7265 7375 6c74 2c20 6f75 7470 7574 290a  result, output).
+0000cbf0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+0000cc00: 6865 636b 5f73 6361 6c65 3a0a 2020 2020  heck_scale:.    
+0000cc10: 2020 2020 2020 2020 2020 2020 6571 5f28              eq_(
+0000cc20: 5b73 7472 2878 2920 666f 7220 7820 696e  [str(x) for x in
+0000cc30: 2072 6573 756c 745d 2c20 5b73 7472 2878   result], [str(x
+0000cc40: 2920 666f 7220 7820 696e 206f 7574 7075  ) for x in outpu
+0000cc50: 745d 290a 0a20 2020 2020 2020 2072 6574  t])..        ret
+0000cc60: 7572 6e20 7275 6e0a 0a20 2020 2040 656d  urn run..    @em
+0000cc70: 6974 735f 7761 726e 696e 6728 7222 2e2a  its_warning(r".*
+0000cc80: 646f 6573 205c 2a6e 6f74 5c2a 2073 7570  does \*not\* sup
+0000cc90: 706f 7274 2044 6563 696d 616c 206f 626a  port Decimal obj
+0000cca0: 6563 7473 206e 6174 6976 656c 7922 290a  ects natively").
+0000ccb0: 2020 2020 6465 6620 7465 7374 5f72 656e      def test_ren
+0000ccc0: 6465 725f 6c69 7465 7261 6c5f 6e75 6d65  der_literal_nume
+0000ccd0: 7269 6328 7365 6c66 2c20 6c69 7465 7261  ric(self, litera
+0000cce0: 6c5f 726f 756e 645f 7472 6970 293a 0a20  l_round_trip):. 
+0000ccf0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000cd00: 2020 2053 5041 4e4e 4552 204f 5645 5252     SPANNER OVERR
+0000cd10: 4944 453a 0a0a 2020 2020 2020 2020 436c  IDE:..        Cl
+0000cd20: 6f75 6420 5370 616e 6e65 7220 7375 7070  oud Spanner supp
+0000cd30: 6f72 7473 2074 6162 6c65 7320 7769 7468  orts tables with
+0000cd40: 2061 6e20 656d 7074 7920 7072 696d 6172   an empty primar
+0000cd50: 7920 6b65 792c 2062 7574 0a20 2020 2020  y key, but.     
+0000cd60: 2020 206f 6e6c 7920 6120 7369 6e67 6c65     only a single
+0000cd70: 2072 6f77 2063 616e 2062 6520 696e 7365   row can be inse
+0000cd80: 7274 6564 2069 6e74 6f20 7375 6368 2061  rted into such a
+0000cd90: 2074 6162 6c65 202d 0a20 2020 2020 2020   table -.       
+0000cda0: 2066 6f6c 6c6f 7769 6e67 2069 6e73 6572   following inser
+0000cdb0: 7469 6f6e 7320 7769 6c6c 2066 6169 6c20  tions will fail 
+0000cdc0: 7769 7468 2060 526f 7720 5b5d 2061 6c72  with `Row [] alr
+0000cdd0: 6561 6479 2065 7869 7374 7322 2e0a 2020  eady exists"..  
+0000cde0: 2020 2020 2020 4f76 6572 7269 6469 6e67        Overriding
+0000cdf0: 2074 6865 2074 6573 7420 746f 2061 766f   the test to avo
+0000ce00: 6964 2074 6865 2073 616d 6520 6661 696c  id the same fail
+0000ce10: 7572 652e 0a20 2020 2020 2020 2022 2222  ure..        """
+0000ce20: 0a20 2020 2020 2020 206c 6974 6572 616c  .        literal
+0000ce30: 5f72 6f75 6e64 5f74 7269 7028 0a20 2020  _round_trip(.   
+0000ce40: 2020 2020 2020 2020 204e 756d 6572 6963           Numeric
+0000ce50: 2870 7265 6369 7369 6f6e 3d38 2c20 7363  (precision=8, sc
+0000ce60: 616c 653d 3429 2c0a 2020 2020 2020 2020  ale=4),.        
+0000ce70: 2020 2020 5b64 6563 696d 616c 2e44 6563      [decimal.Dec
+0000ce80: 696d 616c 2822 3135 2e37 3536 3322 295d  imal("15.7563")]
+0000ce90: 2c0a 2020 2020 2020 2020 2020 2020 5b64  ,.            [d
+0000cea0: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
+0000ceb0: 3135 2e37 3536 3322 295d 2c0a 2020 2020  15.7563")],.    
+0000cec0: 2020 2020 290a 0a20 2020 2040 656d 6974      )..    @emit
+0000ced0: 735f 7761 726e 696e 6728 7222 2e2a 646f  s_warning(r".*do
+0000cee0: 6573 205c 2a6e 6f74 5c2a 2073 7570 706f  es \*not\* suppo
+0000cef0: 7274 2044 6563 696d 616c 206f 626a 6563  rt Decimal objec
+0000cf00: 7473 206e 6174 6976 656c 7922 290a 2020  ts natively").  
+0000cf10: 2020 6465 6620 7465 7374 5f72 656e 6465    def test_rende
+0000cf20: 725f 6c69 7465 7261 6c5f 6e75 6d65 7269  r_literal_numeri
+0000cf30: 635f 6173 666c 6f61 7428 7365 6c66 2c20  c_asfloat(self, 
+0000cf40: 6c69 7465 7261 6c5f 726f 756e 645f 7472  literal_round_tr
+0000cf50: 6970 293a 0a20 2020 2020 2020 2022 2222  ip):.        """
+0000cf60: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
+0000cf70: 204f 5645 5252 4944 453a 0a0a 2020 2020   OVERRIDE:..    
+0000cf80: 2020 2020 436c 6f75 6420 5370 616e 6e65      Cloud Spanne
+0000cf90: 7220 7375 7070 6f72 7473 2074 6162 6c65  r supports table
+0000cfa0: 7320 7769 7468 2061 6e20 656d 7074 7920  s with an empty 
+0000cfb0: 7072 696d 6172 7920 6b65 792c 2062 7574  primary key, but
+0000cfc0: 0a20 2020 2020 2020 206f 6e6c 7920 6120  .        only a 
+0000cfd0: 7369 6e67 6c65 2072 6f77 2063 616e 2062  single row can b
+0000cfe0: 6520 696e 7365 7274 6564 2069 6e74 6f20  e inserted into 
+0000cff0: 7375 6368 2061 2074 6162 6c65 202d 0a20  such a table -. 
+0000d000: 2020 2020 2020 2066 6f6c 6c6f 7769 6e67         following
+0000d010: 2069 6e73 6572 7469 6f6e 7320 7769 6c6c   insertions will
+0000d020: 2066 6169 6c20 7769 7468 2060 526f 7720   fail with `Row 
+0000d030: 5b5d 2061 6c72 6561 6479 2065 7869 7374  [] already exist
+0000d040: 7322 2e0a 2020 2020 2020 2020 4f76 6572  s"..        Over
+0000d050: 7269 6469 6e67 2074 6865 2074 6573 7420  riding the test 
+0000d060: 746f 2061 766f 6964 2074 6865 2073 616d  to avoid the sam
+0000d070: 6520 6661 696c 7572 652e 0a20 2020 2020  e failure..     
+0000d080: 2020 2022 2222 0a20 2020 2020 2020 206c     """.        l
+0000d090: 6974 6572 616c 5f72 6f75 6e64 5f74 7269  iteral_round_tri
+0000d0a0: 7028 0a20 2020 2020 2020 2020 2020 204e  p(.            N
+0000d0b0: 756d 6572 6963 2870 7265 6369 7369 6f6e  umeric(precision
+0000d0c0: 3d38 2c20 7363 616c 653d 342c 2061 7364  =8, scale=4, asd
+0000d0d0: 6563 696d 616c 3d46 616c 7365 292c 0a20  ecimal=False),. 
+0000d0e0: 2020 2020 2020 2020 2020 205b 6465 6369             [deci
+0000d0f0: 6d61 6c2e 4465 6369 6d61 6c28 2231 352e  mal.Decimal("15.
+0000d100: 3735 3633 2229 5d2c 0a20 2020 2020 2020  7563")],.       
+0000d110: 2020 2020 205b 3135 2e37 3536 335d 2c0a       [15.7563],.
+0000d120: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+0000d130: 6566 2074 6573 745f 7265 6e64 6572 5f6c  ef test_render_l
+0000d140: 6974 6572 616c 5f66 6c6f 6174 2873 656c  iteral_float(sel
+0000d150: 662c 206c 6974 6572 616c 5f72 6f75 6e64  f, literal_round
+0000d160: 5f74 7269 7029 3a0a 2020 2020 2020 2020  _trip):.        
+0000d170: 2222 220a 2020 2020 2020 2020 5350 414e  """.        SPAN
+0000d180: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
+0000d190: 2020 2020 2020 2043 6c6f 7564 2053 7061         Cloud Spa
+0000d1a0: 6e6e 6572 2073 7570 706f 7274 7320 7461  nner supports ta
+0000d1b0: 626c 6573 2077 6974 6820 616e 2065 6d70  bles with an emp
+0000d1c0: 7479 2070 7269 6d61 7279 206b 6579 2c20  ty primary key, 
+0000d1d0: 6275 740a 2020 2020 2020 2020 6f6e 6c79  but.        only
+0000d1e0: 2061 2073 696e 676c 6520 726f 7720 6361   a single row ca
+0000d1f0: 6e20 6265 2069 6e73 6572 7465 6420 696e  n be inserted in
+0000d200: 746f 2073 7563 6820 6120 7461 626c 6520  to such a table 
+0000d210: 2d0a 2020 2020 2020 2020 666f 6c6c 6f77  -.        follow
+0000d220: 696e 6720 696e 7365 7274 696f 6e73 2077  ing insertions w
+0000d230: 696c 6c20 6661 696c 2077 6974 6820 6052  ill fail with `R
+0000d240: 6f77 205b 5d20 616c 7265 6164 7920 6578  ow [] already ex
+0000d250: 6973 7473 222e 0a20 2020 2020 2020 204f  ists"..        O
+0000d260: 7665 7272 6964 696e 6720 7468 6520 7465  verriding the te
+0000d270: 7374 2074 6f20 6176 6f69 6420 7468 6520  st to avoid the 
+0000d280: 7361 6d65 2066 6169 6c75 7265 2e0a 2020  same failure..  
+0000d290: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000d2a0: 2020 6c69 7465 7261 6c5f 726f 756e 645f    literal_round_
+0000d2b0: 7472 6970 280a 2020 2020 2020 2020 2020  trip(.          
+0000d2c0: 2020 466c 6f61 7428 3429 2c0a 2020 2020    Float(4),.    
+0000d2d0: 2020 2020 2020 2020 5b64 6563 696d 616c          [decimal
+0000d2e0: 2e44 6563 696d 616c 2822 3135 2e37 3536  .Decimal("15.756
+0000d2f0: 3322 295d 2c0a 2020 2020 2020 2020 2020  3")],.          
+0000d300: 2020 5b31 352e 3735 3633 5d2c 0a20 2020    [15.7563],.   
+0000d310: 2020 2020 2020 2020 2066 696c 7465 725f           filter_
+0000d320: 3d6c 616d 6264 6120 6e3a 206e 2069 7320  =lambda n: n is 
+0000d330: 6e6f 7420 4e6f 6e65 2061 6e64 2072 6f75  not None and rou
+0000d340: 6e64 286e 2c20 3529 206f 7220 4e6f 6e65  nd(n, 5) or None
+0000d350: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+0000d360: 2040 7265 7175 6972 6573 2e70 7265 6369   @requires.preci
+0000d370: 7369 6f6e 5f67 656e 6572 6963 5f66 6c6f  sion_generic_flo
+0000d380: 6174 5f74 7970 650a 2020 2020 6465 6620  at_type.    def 
+0000d390: 7465 7374 5f66 6c6f 6174 5f63 7573 746f  test_float_custo
+0000d3a0: 6d5f 7363 616c 6528 7365 6c66 2c20 646f  m_scale(self, do
+0000d3b0: 5f6e 756d 6572 6963 5f74 6573 7429 3a0a  _numeric_test):.
+0000d3c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000d3d0: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
+0000d3e0: 5249 4445 3a0a 0a20 2020 2020 2020 2043  RIDE:..        C
+0000d3f0: 6c6f 7564 2053 7061 6e6e 6572 2073 7570  loud Spanner sup
+0000d400: 706f 7274 7320 7461 626c 6573 2077 6974  ports tables wit
+0000d410: 6820 616e 2065 6d70 7479 2070 7269 6d61  h an empty prima
+0000d420: 7279 206b 6579 2c20 6275 740a 2020 2020  ry key, but.    
+0000d430: 2020 2020 6f6e 6c79 2061 2073 696e 676c      only a singl
+0000d440: 6520 726f 7720 6361 6e20 6265 2069 6e73  e row can be ins
+0000d450: 6572 7465 6420 696e 746f 2073 7563 6820  erted into such 
+0000d460: 6120 7461 626c 6520 2d0a 2020 2020 2020  a table -.      
+0000d470: 2020 666f 6c6c 6f77 696e 6720 696e 7365    following inse
+0000d480: 7274 696f 6e73 2077 696c 6c20 6661 696c  rtions will fail
+0000d490: 2077 6974 6820 6052 6f77 205b 5d20 616c   with `Row [] al
+0000d4a0: 7265 6164 7920 6578 6973 7473 222e 0a20  ready exists".. 
+0000d4b0: 2020 2020 2020 204f 7665 7272 6964 696e         Overridin
+0000d4c0: 6720 7468 6520 7465 7374 2074 6f20 6176  g the test to av
+0000d4d0: 6f69 6420 7468 6520 7361 6d65 2066 6169  oid the same fai
+0000d4e0: 6c75 7265 2e0a 2020 2020 2020 2020 2222  lure..        ""
+0000d4f0: 220a 2020 2020 2020 2020 646f 5f6e 756d  ".        do_num
+0000d500: 6572 6963 5f74 6573 7428 0a20 2020 2020  eric_test(.     
+0000d510: 2020 2020 2020 2046 6c6f 6174 284e 6f6e         Float(Non
+0000d520: 652c 2064 6563 696d 616c 5f72 6574 7572  e, decimal_retur
+0000d530: 6e5f 7363 616c 653d 372c 2061 7364 6563  n_scale=7, asdec
+0000d540: 696d 616c 3d54 7275 6529 2c0a 2020 2020  imal=True),.    
+0000d550: 2020 2020 2020 2020 5b64 6563 696d 616c          [decimal
+0000d560: 2e44 6563 696d 616c 2822 3135 2e37 3536  .Decimal("15.756
+0000d570: 3338 3237 2229 2c20 6465 6369 6d61 6c2e  3827"), decimal.
+0000d580: 4465 6369 6d61 6c28 2231 352e 3735 3633  Decimal("15.7563
+0000d590: 3832 3722 295d 2c0a 2020 2020 2020 2020  827")],.        
+0000d5a0: 2020 2020 5b64 6563 696d 616c 2e44 6563      [decimal.Dec
+0000d5b0: 696d 616c 2822 3135 2e37 3536 3338 3237  imal("15.7563827
+0000d5c0: 2229 5d2c 0a20 2020 2020 2020 2020 2020  ")],.           
+0000d5d0: 2063 6865 636b 5f73 6361 6c65 3d54 7275   check_scale=Tru
+0000d5e0: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
+0000d5f0: 2020 6465 6620 7465 7374 5f6e 756d 6572    def test_numer
+0000d600: 6963 5f61 735f 6465 6369 6d61 6c28 7365  ic_as_decimal(se
+0000d610: 6c66 2c20 646f 5f6e 756d 6572 6963 5f74  lf, do_numeric_t
+0000d620: 6573 7429 3a0a 2020 2020 2020 2020 2222  est):.        ""
+0000d630: 220a 2020 2020 2020 2020 5350 414e 4e45  ".        SPANNE
+0000d640: 5220 4f56 4552 5249 4445 3a0a 0a20 2020  R OVERRIDE:..   
+0000d650: 2020 2020 2053 7061 6e6e 6572 2074 6872       Spanner thr
+0000d660: 6f77 7320 616e 2065 7272 6f72 2034 3030  ows an error 400
+0000d670: 2056 616c 7565 2068 6173 2074 7970 6520   Value has type 
+0000d680: 464c 4f41 5436 3420 7768 6963 6820 6361  FLOAT64 which ca
+0000d690: 6e6e 6f74 2062 650a 2020 2020 2020 2020  nnot be.        
+0000d6a0: 696e 7365 7274 6564 2069 6e74 6f20 636f  inserted into co
+0000d6b0: 6c75 6d6e 2078 2c20 7768 6963 6820 6861  lumn x, which ha
+0000d6c0: 7320 7479 7065 204e 554d 4552 4943 2066  s type NUMERIC f
+0000d6d0: 6f72 2076 616c 7565 2031 352e 3735 3633  or value 15.7563
+0000d6e0: 2e0a 2020 2020 2020 2020 4f76 6572 7269  ..        Overri
+0000d6f0: 6469 6e67 2074 6865 2074 6573 7420 746f  ding the test to
+0000d700: 2072 656d 6f76 6520 7468 6520 6661 696c   remove the fail
+0000d710: 7572 6520 6361 7365 2e0a 2020 2020 2020  ure case..      
+0000d720: 2020 2222 220a 2020 2020 2020 2020 646f    """.        do
+0000d730: 5f6e 756d 6572 6963 5f74 6573 7428 0a20  _numeric_test(. 
+0000d740: 2020 2020 2020 2020 2020 204e 756d 6572             Numer
+0000d750: 6963 2870 7265 6369 7369 6f6e 3d38 2c20  ic(precision=8, 
+0000d760: 7363 616c 653d 3429 2c0a 2020 2020 2020  scale=4),.      
+0000d770: 2020 2020 2020 5b64 6563 696d 616c 2e44        [decimal.D
+0000d780: 6563 696d 616c 2822 3135 2e37 3536 3322  ecimal("15.7563"
+0000d790: 292c 2064 6563 696d 616c 2e44 6563 696d  ), decimal.Decim
+0000d7a0: 616c 2822 3135 2e37 3536 3322 295d 2c0a  al("15.7563")],.
+0000d7b0: 2020 2020 2020 2020 2020 2020 5b64 6563              [dec
+0000d7c0: 696d 616c 2e44 6563 696d 616c 2822 3135  imal.Decimal("15
+0000d7d0: 2e37 3536 3322 295d 2c0a 2020 2020 2020  .7563")],.      
+0000d7e0: 2020 290a 0a20 2020 2064 6566 2074 6573    )..    def tes
+0000d7f0: 745f 6e75 6d65 7269 635f 6173 5f66 6c6f  t_numeric_as_flo
+0000d800: 6174 2873 656c 662c 2064 6f5f 6e75 6d65  at(self, do_nume
+0000d810: 7269 635f 7465 7374 293a 0a20 2020 2020  ric_test):.     
+0000d820: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+0000d830: 5041 4e4e 4552 204f 5645 5252 4944 453a  PANNER OVERRIDE:
+0000d840: 0a0a 2020 2020 2020 2020 5370 616e 6e65  ..        Spanne
+0000d850: 7220 7468 726f 7773 2061 6e20 6572 726f  r throws an erro
+0000d860: 7220 3430 3020 5661 6c75 6520 6861 7320  r 400 Value has 
+0000d870: 7479 7065 2046 4c4f 4154 3634 2077 6869  type FLOAT64 whi
+0000d880: 6368 2063 616e 6e6f 7420 6265 0a20 2020  ch cannot be.   
+0000d890: 2020 2020 2069 6e73 6572 7465 6420 696e       inserted in
+0000d8a0: 746f 2063 6f6c 756d 6e20 782c 2077 6869  to column x, whi
+0000d8b0: 6368 2068 6173 2074 7970 6520 4e55 4d45  ch has type NUME
+0000d8c0: 5249 4320 666f 7220 7661 6c75 6520 3135  RIC for value 15
+0000d8d0: 2e37 3536 332e 0a20 2020 2020 2020 204f  .7563..        O
+0000d8e0: 7665 7272 6964 696e 6720 7468 6520 7465  verriding the te
+0000d8f0: 7374 2074 6f20 7265 6d6f 7665 2074 6865  st to remove the
+0000d900: 2066 6169 6c75 7265 2063 6173 652e 0a20   failure case.. 
+0000d910: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000d920: 2020 2064 6f5f 6e75 6d65 7269 635f 7465     do_numeric_te
+0000d930: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
+0000d940: 4e75 6d65 7269 6328 7072 6563 6973 696f  Numeric(precisio
+0000d950: 6e3d 382c 2073 6361 6c65 3d34 2c20 6173  n=8, scale=4, as
+0000d960: 6465 6369 6d61 6c3d 4661 6c73 6529 2c0a  decimal=False),.
+0000d970: 2020 2020 2020 2020 2020 2020 5b64 6563              [dec
+0000d980: 696d 616c 2e44 6563 696d 616c 2822 3135  imal.Decimal("15
+0000d990: 2e37 3536 3322 292c 2064 6563 696d 616c  .7563"), decimal
+0000d9a0: 2e44 6563 696d 616c 2822 3135 2e37 3536  .Decimal("15.756
+0000d9b0: 3322 295d 2c0a 2020 2020 2020 2020 2020  3")],.          
+0000d9c0: 2020 5b31 352e 3735 3633 5d2c 0a20 2020    [15.7563],.   
+0000d9d0: 2020 2020 2029 0a0a 2020 2020 4072 6571       )..    @req
+0000d9e0: 7569 7265 732e 666c 6f61 7473 5f74 6f5f  uires.floats_to_
+0000d9f0: 666f 7572 5f64 6563 696d 616c 730a 2020  four_decimals.  
+0000da00: 2020 6465 6620 7465 7374 5f66 6c6f 6174    def test_float
+0000da10: 5f61 735f 6465 6369 6d61 6c28 7365 6c66  _as_decimal(self
+0000da20: 2c20 646f 5f6e 756d 6572 6963 5f74 6573  , do_numeric_tes
+0000da30: 7429 3a0a 2020 2020 2020 2020 2222 220a  t):.        """.
+0000da40: 2020 2020 2020 2020 5350 414e 4e45 5220          SPANNER 
+0000da50: 4f56 4552 5249 4445 3a0a 0a20 2020 2020  OVERRIDE:..     
+0000da60: 2020 2043 6c6f 7564 2053 7061 6e6e 6572     Cloud Spanner
+0000da70: 2073 7570 706f 7274 7320 7461 626c 6573   supports tables
+0000da80: 2077 6974 6820 616e 2065 6d70 7479 2070   with an empty p
+0000da90: 7269 6d61 7279 206b 6579 2c20 6275 740a  rimary key, but.
+0000daa0: 2020 2020 2020 2020 6f6e 6c79 2061 2073          only a s
+0000dab0: 696e 676c 6520 726f 7720 6361 6e20 6265  ingle row can be
+0000dac0: 2069 6e73 6572 7465 6420 696e 746f 2073   inserted into s
+0000dad0: 7563 6820 6120 7461 626c 6520 2d0a 2020  uch a table -.  
+0000dae0: 2020 2020 2020 666f 6c6c 6f77 696e 6720        following 
+0000daf0: 696e 7365 7274 696f 6e73 2077 696c 6c20  insertions will 
+0000db00: 6661 696c 2077 6974 6820 6052 6f77 205b  fail with `Row [
+0000db10: 5d20 616c 7265 6164 7920 6578 6973 7473  ] already exists
+0000db20: 222e 0a20 2020 2020 2020 204f 7665 7272  "..        Overr
+0000db30: 6964 696e 6720 7468 6520 7465 7374 2074  iding the test t
+0000db40: 6f20 6176 6f69 6420 7468 6520 7361 6d65  o avoid the same
+0000db50: 2066 6169 6c75 7265 2e0a 2020 2020 2020   failure..      
+0000db60: 2020 2222 220a 2020 2020 2020 2020 646f    """.        do
+0000db70: 5f6e 756d 6572 6963 5f74 6573 7428 0a20  _numeric_test(. 
+0000db80: 2020 2020 2020 2020 2020 2046 6c6f 6174             Float
+0000db90: 2870 7265 6369 7369 6f6e 3d38 2c20 6173  (precision=8, as
+0000dba0: 6465 6369 6d61 6c3d 5472 7565 292c 0a20  decimal=True),. 
+0000dbb0: 2020 2020 2020 2020 2020 205b 6465 6369             [deci
+0000dbc0: 6d61 6c2e 4465 6369 6d61 6c28 2231 352e  mal.Decimal("15.
+0000dbd0: 3735 3633 2229 2c20 6465 6369 6d61 6c2e  7563"), decimal.
+0000dbe0: 4465 6369 6d61 6c28 2231 352e 3735 3633  Decimal("15.7563
+0000dbf0: 2229 2c20 4e6f 6e65 5d2c 0a20 2020 2020  "), None],.     
+0000dc00: 2020 2020 2020 205b 6465 6369 6d61 6c2e         [decimal.
+0000dc10: 4465 6369 6d61 6c28 2231 352e 3735 3633  Decimal("15.7563
+0000dc20: 2229 2c20 4e6f 6e65 5d2c 0a20 2020 2020  "), None],.     
+0000dc30: 2020 2020 2020 2066 696c 7465 725f 3d6c         filter_=l
+0000dc40: 616d 6264 6120 6e3a 206e 2069 7320 6e6f  ambda n: n is no
+0000dc50: 7420 4e6f 6e65 2061 6e64 2072 6f75 6e64  t None and round
+0000dc60: 286e 2c20 3429 206f 7220 4e6f 6e65 2c0a  (n, 4) or None,.
+0000dc70: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+0000dc80: 6566 2074 6573 745f 666c 6f61 745f 6173  ef test_float_as
+0000dc90: 5f66 6c6f 6174 2873 656c 662c 2064 6f5f  _float(self, do_
+0000dca0: 6e75 6d65 7269 635f 7465 7374 293a 0a20  numeric_test):. 
+0000dcb0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000dcc0: 2020 2053 5041 4e4e 4552 204f 5645 5252     SPANNER OVERR
+0000dcd0: 4944 453a 0a0a 2020 2020 2020 2020 436c  IDE:..        Cl
+0000dce0: 6f75 6420 5370 616e 6e65 7220 7375 7070  oud Spanner supp
+0000dcf0: 6f72 7473 2074 6162 6c65 7320 7769 7468  orts tables with
+0000dd00: 2061 6e20 656d 7074 7920 7072 696d 6172   an empty primar
+0000dd10: 7920 6b65 792c 2062 7574 0a20 2020 2020  y key, but.     
+0000dd20: 2020 206f 6e6c 7920 6120 7369 6e67 6c65     only a single
+0000dd30: 2072 6f77 2063 616e 2062 6520 696e 7365   row can be inse
+0000dd40: 7274 6564 2069 6e74 6f20 7375 6368 2061  rted into such a
+0000dd50: 2074 6162 6c65 202d 0a20 2020 2020 2020   table -.       
+0000dd60: 2066 6f6c 6c6f 7769 6e67 2069 6e73 6572   following inser
+0000dd70: 7469 6f6e 7320 7769 6c6c 2066 6169 6c20  tions will fail 
+0000dd80: 7769 7468 2060 526f 7720 5b5d 2061 6c72  with `Row [] alr
+0000dd90: 6561 6479 2065 7869 7374 7322 2e0a 2020  eady exists"..  
+0000dda0: 2020 2020 2020 4f76 6572 7269 6469 6e67        Overriding
+0000ddb0: 2074 6865 2074 6573 7420 746f 2061 766f   the test to avo
+0000ddc0: 6964 2074 6865 2073 616d 6520 6661 696c  id the same fail
+0000ddd0: 7572 652e 0a20 2020 2020 2020 2022 2222  ure..        """
+0000dde0: 0a20 2020 2020 2020 2064 6f5f 6e75 6d65  .        do_nume
+0000ddf0: 7269 635f 7465 7374 280a 2020 2020 2020  ric_test(.      
+0000de00: 2020 2020 2020 466c 6f61 7428 7072 6563        Float(prec
+0000de10: 6973 696f 6e3d 3829 2c0a 2020 2020 2020  ision=8),.      
+0000de20: 2020 2020 2020 5b64 6563 696d 616c 2e44        [decimal.D
+0000de30: 6563 696d 616c 2822 3135 2e37 3536 3322  ecimal("15.7563"
+0000de40: 292c 2064 6563 696d 616c 2e44 6563 696d  ), decimal.Decim
+0000de50: 616c 2822 3135 2e37 3536 3322 295d 2c0a  al("15.7563")],.
+0000de60: 2020 2020 2020 2020 2020 2020 5b31 352e              [15.
+0000de70: 3735 3633 5d2c 0a20 2020 2020 2020 2020  7563],.         
+0000de80: 2020 2066 696c 7465 725f 3d6c 616d 6264     filter_=lambd
+0000de90: 6120 6e3a 206e 2069 7320 6e6f 7420 4e6f  a n: n is not No
+0000dea0: 6e65 2061 6e64 2072 6f75 6e64 286e 2c20  ne and round(n, 
+0000deb0: 3529 206f 7220 4e6f 6e65 2c0a 2020 2020  5) or None,.    
+0000dec0: 2020 2020 290a 0a20 2020 2040 7265 7175      )..    @requ
+0000ded0: 6972 6573 2e70 7265 6369 7369 6f6e 5f6e  ires.precision_n
+0000dee0: 756d 6572 6963 735f 6765 6e65 7261 6c0a  umerics_general.
+0000def0: 2020 2020 6465 6620 7465 7374 5f70 7265      def test_pre
+0000df00: 6369 7369 6f6e 5f64 6563 696d 616c 2873  cision_decimal(s
+0000df10: 656c 662c 2064 6f5f 6e75 6d65 7269 635f  elf, do_numeric_
+0000df20: 7465 7374 293a 0a20 2020 2020 2020 2022  test):.        "
+0000df30: 2222 0a20 2020 2020 2020 2053 5041 4e4e  "".        SPANN
+0000df40: 4552 204f 5645 5252 4944 453a 0a0a 2020  ER OVERRIDE:..  
+0000df50: 2020 2020 2020 436c 6f75 6420 5370 616e        Cloud Span
+0000df60: 6e65 7220 7375 7070 6f72 7473 2074 6162  ner supports tab
+0000df70: 6c65 7320 7769 7468 2061 6e20 656d 7074  les with an empt
+0000df80: 7920 7072 696d 6172 7920 6b65 792c 2062  y primary key, b
+0000df90: 7574 0a20 2020 2020 2020 206f 6e6c 7920  ut.        only 
+0000dfa0: 6120 7369 6e67 6c65 2072 6f77 2063 616e  a single row can
+0000dfb0: 2062 6520 696e 7365 7274 6564 2069 6e74   be inserted int
+0000dfc0: 6f20 7375 6368 2061 2074 6162 6c65 202d  o such a table -
+0000dfd0: 0a20 2020 2020 2020 2066 6f6c 6c6f 7769  .        followi
+0000dfe0: 6e67 2069 6e73 6572 7469 6f6e 7320 7769  ng insertions wi
+0000dff0: 6c6c 2066 6169 6c20 7769 7468 2060 526f  ll fail with `Ro
+0000e000: 7720 5b5d 2061 6c72 6561 6479 2065 7869  w [] already exi
+0000e010: 7374 7322 2e0a 2020 2020 2020 2020 4f76  sts"..        Ov
+0000e020: 6572 7269 6469 6e67 2074 6865 2074 6573  erriding the tes
+0000e030: 7420 746f 2061 766f 6964 2074 6865 2073  t to avoid the s
+0000e040: 616d 6520 6661 696c 7572 652e 0a0a 2020  ame failure...  
+0000e050: 2020 2020 2020 5265 6d6f 7665 2061 6e20        Remove an 
+0000e060: 6578 7472 6120 6469 6769 7473 2061 6674  extra digits aft
+0000e070: 6572 2064 6563 696d 616c 2070 6f69 6e74  er decimal point
+0000e080: 2061 7320 636c 6f75 6420 7370 616e 6e65   as cloud spanne
+0000e090: 7220 6973 0a20 2020 2020 2020 2063 6170  r is.        cap
+0000e0a0: 6162 6c65 206f 6620 7265 7072 6573 656e  able of represen
+0000e0b0: 7469 6e67 2061 6e20 6578 6163 7420 6e75  ting an exact nu
+0000e0c0: 6d65 7269 6320 7661 6c75 6520 7769 7468  meric value with
+0000e0d0: 2061 2070 7265 6369 7369 6f6e 0a20 2020   a precision.   
+0000e0e0: 2020 2020 206f 6620 3338 2061 6e64 2073       of 38 and s
+0000e0f0: 6361 6c65 206f 6620 392e 0a20 2020 2020  cale of 9..     
+0000e100: 2020 2022 2222 0a20 2020 2020 2020 206e     """.        n
+0000e110: 756d 6265 7273 203d 2073 6574 280a 2020  umbers = set(.  
+0000e120: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
+0000e130: 2020 2020 2020 2020 2020 2020 6465 6369              deci
+0000e140: 6d61 6c2e 4465 6369 6d61 6c28 2235 342e  mal.Decimal("54.
+0000e150: 3234 3634 3531 3635 3022 292c 0a20 2020  246451650"),.   
+0000e160: 2020 2020 2020 2020 2020 2020 2064 6563               dec
+0000e170: 696d 616c 2e44 6563 696d 616c 2822 302e  imal.Decimal("0.
+0000e180: 3030 3433 3534 2229 2c0a 2020 2020 2020  004354"),.      
+0000e190: 2020 2020 2020 2020 2020 6465 6369 6d61            decima
+0000e1a0: 6c2e 4465 6369 6d61 6c28 2239 3030 2e30  l.Decimal("900.0
+0000e1b0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+0000e1c0: 5d0a 2020 2020 2020 2020 290a 2020 2020  ].        ).    
+0000e1d0: 2020 2020 646f 5f6e 756d 6572 6963 5f74      do_numeric_t
+0000e1e0: 6573 7428 4e75 6d65 7269 6328 7072 6563  est(Numeric(prec
+0000e1f0: 6973 696f 6e3d 3138 2c20 7363 616c 653d  ision=18, scale=
+0000e200: 3929 2c20 6e75 6d62 6572 732c 206e 756d  9), numbers, num
+0000e210: 6265 7273 290a 0a20 2020 2040 7465 7374  bers)..    @test
+0000e220: 696e 672e 7265 7175 6972 6573 2e70 7265  ing.requires.pre
+0000e230: 6369 7369 6f6e 5f6e 756d 6572 6963 735f  cision_numerics_
+0000e240: 656e 6f74 6174 696f 6e5f 6c61 7267 650a  enotation_large.
+0000e250: 2020 2020 6465 6620 7465 7374 5f65 6e6f      def test_eno
+0000e260: 7461 7469 6f6e 5f64 6563 696d 616c 5f6c  tation_decimal_l
+0000e270: 6172 6765 2873 656c 662c 2064 6f5f 6e75  arge(self, do_nu
+0000e280: 6d65 7269 635f 7465 7374 293a 0a20 2020  meric_test):.   
+0000e290: 2020 2020 2022 2222 7465 7374 2065 7863       """test exc
+0000e2a0: 6565 6469 6e67 6c79 206c 6172 6765 2064  eedingly large d
+0000e2b0: 6563 696d 616c 732e 0a0a 2020 2020 2020  ecimals...      
+0000e2c0: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
+0000e2d0: 4445 3a0a 0a20 2020 2020 2020 2043 6c6f  DE:..        Clo
+0000e2e0: 7564 2053 7061 6e6e 6572 2073 7570 706f  ud Spanner suppo
+0000e2f0: 7274 7320 7461 626c 6573 2077 6974 6820  rts tables with 
+0000e300: 616e 2065 6d70 7479 2070 7269 6d61 7279  an empty primary
+0000e310: 206b 6579 2c20 6275 740a 2020 2020 2020   key, but.      
+0000e320: 2020 6f6e 6c79 2061 2073 696e 676c 6520    only a single 
+0000e330: 726f 7720 6361 6e20 6265 2069 6e73 6572  row can be inser
+0000e340: 7465 6420 696e 746f 2073 7563 6820 6120  ted into such a 
+0000e350: 7461 626c 6520 2d0a 2020 2020 2020 2020  table -.        
+0000e360: 666f 6c6c 6f77 696e 6720 696e 7365 7274  following insert
+0000e370: 696f 6e73 2077 696c 6c20 6661 696c 2077  ions will fail w
+0000e380: 6974 6820 6052 6f77 205b 5d20 616c 7265  ith `Row [] alre
+0000e390: 6164 7920 6578 6973 7473 222e 0a20 2020  ady exists"..   
+0000e3a0: 2020 2020 204f 7665 7272 6964 696e 6720       Overriding 
+0000e3b0: 7468 6520 7465 7374 2074 6f20 6176 6f69  the test to avoi
+0000e3c0: 6420 7468 6520 7361 6d65 2066 6169 6c75  d the same failu
+0000e3d0: 7265 2e0a 2020 2020 2020 2020 2222 220a  re..        """.
+0000e3e0: 2020 2020 2020 2020 6e75 6d62 6572 7320          numbers 
+0000e3f0: 3d20 7365 7428 0a20 2020 2020 2020 2020  = set(.         
+0000e400: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+0000e410: 2020 2020 2064 6563 696d 616c 2e44 6563       decimal.Dec
+0000e420: 696d 616c 2822 3445 2b38 2229 2c0a 2020  imal("4E+8"),.  
+0000e430: 2020 2020 2020 2020 2020 2020 2020 6465                de
+0000e440: 6369 6d61 6c2e 4465 6369 6d61 6c28 2235  cimal.Decimal("5
+0000e450: 3734 3845 2b31 3522 292c 0a20 2020 2020  748E+15"),.     
+0000e460: 2020 2020 2020 2020 2020 2064 6563 696d             decim
+0000e470: 616c 2e44 6563 696d 616c 2822 312e 3532  al.Decimal("1.52
+0000e480: 3145 2b31 3522 292c 0a20 2020 2020 2020  1E+15"),.       
+0000e490: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
+0000e4a0: 2e44 6563 696d 616c 2822 3030 3030 3030  .Decimal("000000
+0000e4b0: 3030 302e 3145 2b39 2229 2c0a 2020 2020  000.1E+9"),.    
+0000e4c0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+0000e4d0: 2020 290a 2020 2020 2020 2020 646f 5f6e    ).        do_n
+0000e4e0: 756d 6572 6963 5f74 6573 7428 4e75 6d65  umeric_test(Nume
+0000e4f0: 7269 6328 7072 6563 6973 696f 6e3d 3235  ric(precision=25
+0000e500: 2c20 7363 616c 653d 3229 2c20 6e75 6d62  , scale=2), numb
+0000e510: 6572 732c 206e 756d 6265 7273 290a 0a20  ers, numbers).. 
+0000e520: 2020 2040 7465 7374 696e 672e 7265 7175     @testing.requ
+0000e530: 6972 6573 2e70 7265 6369 7369 6f6e 5f6e  ires.precision_n
+0000e540: 756d 6572 6963 735f 656e 6f74 6174 696f  umerics_enotatio
+0000e550: 6e5f 6c61 7267 650a 2020 2020 6465 6620  n_large.    def 
+0000e560: 7465 7374 5f65 6e6f 7461 7469 6f6e 5f64  test_enotation_d
+0000e570: 6563 696d 616c 2873 656c 662c 2064 6f5f  ecimal(self, do_
+0000e580: 6e75 6d65 7269 635f 7465 7374 293a 0a20  numeric_test):. 
+0000e590: 2020 2020 2020 2022 2222 7465 7374 2065         """test e
+0000e5a0: 7863 6565 6469 6e67 6c79 2073 6d61 6c6c  xceedingly small
+0000e5b0: 2064 6563 696d 616c 732e 0a0a 2020 2020   decimals...    
+0000e5c0: 2020 2020 4465 6369 6d61 6c20 7265 706f      Decimal repo
+0000e5d0: 7274 7320 7661 6c75 6573 2077 6974 6820  rts values with 
+0000e5e0: 4520 6e6f 7461 7469 6f6e 2077 6865 6e20  E notation when 
+0000e5f0: 7468 6520 6578 706f 6e65 6e74 0a20 2020  the exponent.   
+0000e600: 2020 2020 2069 7320 6772 6561 7465 7220       is greater 
+0000e610: 7468 616e 2036 2e0a 0a20 2020 2020 2020  than 6...       
+0000e620: 2053 5041 4e4e 4552 204f 5645 5252 4944   SPANNER OVERRID
+0000e630: 453a 0a0a 2020 2020 2020 2020 5265 6d6f  E:..        Remo
+0000e640: 7665 2065 7874 7261 2064 6967 6974 7320  ve extra digits 
+0000e650: 6166 7465 7220 6465 6369 6d61 6c20 706f  after decimal po
+0000e660: 696e 7420 6173 2043 6c6f 7564 2053 7061  int as Cloud Spa
+0000e670: 6e6e 6572 2069 730a 2020 2020 2020 2020  nner is.        
+0000e680: 6361 7061 626c 6520 6f66 2072 6570 7265  capable of repre
+0000e690: 7365 6e74 696e 6720 616e 2065 7861 6374  senting an exact
+0000e6a0: 206e 756d 6572 6963 2076 616c 7565 2077   numeric value w
+0000e6b0: 6974 6820 6120 7072 6563 6973 696f 6e0a  ith a precision.
+0000e6c0: 2020 2020 2020 2020 6f66 2033 3820 616e          of 38 an
+0000e6d0: 6420 7363 616c 6520 6f66 2039 2e0a 2020  d scale of 9..  
+0000e6e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000e6f0: 2020 6e75 6d62 6572 7320 3d20 7365 7428    numbers = set(
+0000e700: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
+0000e710: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000e720: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
+0000e730: 3145 2d32 2229 2c0a 2020 2020 2020 2020  1E-2"),.        
+0000e740: 2020 2020 2020 2020 6465 6369 6d61 6c2e          decimal.
+0000e750: 4465 6369 6d61 6c28 2231 452d 3322 292c  Decimal("1E-3"),
+0000e760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e770: 2064 6563 696d 616c 2e44 6563 696d 616c   decimal.Decimal
+0000e780: 2822 3145 2d34 2229 2c0a 2020 2020 2020  ("1E-4"),.      
+0000e790: 2020 2020 2020 2020 2020 6465 6369 6d61            decima
+0000e7a0: 6c2e 4465 6369 6d61 6c28 2231 452d 3522  l.Decimal("1E-5"
+0000e7b0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000e7c0: 2020 2064 6563 696d 616c 2e44 6563 696d     decimal.Decim
+0000e7d0: 616c 2822 3145 2d36 2229 2c0a 2020 2020  al("1E-6"),.    
+0000e7e0: 2020 2020 2020 2020 2020 2020 6465 6369              deci
+0000e7f0: 6d61 6c2e 4465 6369 6d61 6c28 2231 452d  mal.Decimal("1E-
+0000e800: 3722 292c 0a20 2020 2020 2020 2020 2020  7"),.           
+0000e810: 2020 2020 2064 6563 696d 616c 2e44 6563       decimal.Dec
+0000e820: 696d 616c 2822 3145 2d38 2229 2c0a 2020  imal("1E-8"),.  
+0000e830: 2020 2020 2020 2020 2020 2020 2020 6465                de
+0000e840: 6369 6d61 6c2e 4465 6369 6d61 6c28 2230  cimal.Decimal("0
+0000e850: 2e31 3035 3934 3036 3936 2229 2c0a 2020  .105940696"),.  
+0000e860: 2020 2020 2020 2020 2020 2020 2020 6465                de
+0000e870: 6369 6d61 6c2e 4465 6369 6d61 6c28 2230  cimal.Decimal("0
+0000e880: 2e30 3035 3934 3036 3936 2229 2c0a 2020  .005940696"),.  
+0000e890: 2020 2020 2020 2020 2020 2020 2020 6465                de
+0000e8a0: 6369 6d61 6c2e 4465 6369 6d61 6c28 2230  cimal.Decimal("0
+0000e8b0: 2e30 3030 3030 3036 3936 2229 2c0a 2020  .000000696"),.  
+0000e8c0: 2020 2020 2020 2020 2020 2020 2020 6465                de
+0000e8d0: 6369 6d61 6c2e 4465 6369 6d61 6c28 2230  cimal.Decimal("0
+0000e8e0: 2e37 3030 3030 3036 3936 2229 2c0a 2020  .700000696"),.  
+0000e8f0: 2020 2020 2020 2020 2020 2020 2020 6465                de
+0000e900: 6369 6d61 6c2e 4465 6369 6d61 6c28 2236  cimal.Decimal("6
+0000e910: 3936 452d 3922 292c 0a20 2020 2020 2020  96E-9"),.       
+0000e920: 2020 2020 205d 0a20 2020 2020 2020 2029       ].        )
+0000e930: 0a20 2020 2020 2020 2064 6f5f 6e75 6d65  .        do_nume
+0000e940: 7269 635f 7465 7374 284e 756d 6572 6963  ric_test(Numeric
+0000e950: 2870 7265 6369 7369 6f6e 3d33 382c 2073  (precision=38, s
+0000e960: 6361 6c65 3d39 292c 206e 756d 6265 7273  cale=9), numbers
+0000e970: 2c20 6e75 6d62 6572 7329 0a0a 0a63 6c61  , numbers)...cla
+0000e980: 7373 204c 696b 6546 756e 6374 696f 6e73  ss LikeFunctions
+0000e990: 5465 7374 285f 4c69 6b65 4675 6e63 7469  Test(_LikeFuncti
+0000e9a0: 6f6e 7354 6573 7429 3a0a 2020 2020 4070  onsTest):.    @p
+0000e9b0: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+0000e9c0: 2253 7061 6e6e 6572 2064 6f65 736e 2774  "Spanner doesn't
+0000e9d0: 2073 7570 706f 7274 204c 494b 4520 4553   support LIKE ES
+0000e9e0: 4341 5045 2063 6c61 7573 6522 290a 2020  CAPE clause").  
+0000e9f0: 2020 6465 6620 7465 7374 5f63 6f6e 7461    def test_conta
+0000ea00: 696e 735f 6175 746f 6573 6361 7065 2873  ins_autoescape(s
+0000ea10: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+0000ea20: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
+0000ea30: 6d61 726b 2e73 6b69 7028 2253 7061 6e6e  mark.skip("Spann
+0000ea40: 6572 2064 6f65 736e 2774 2073 7570 706f  er doesn't suppo
+0000ea50: 7274 204c 494b 4520 4553 4341 5045 2063  rt LIKE ESCAPE c
+0000ea60: 6c61 7573 6522 290a 2020 2020 6465 6620  lause").    def 
+0000ea70: 7465 7374 5f63 6f6e 7461 696e 735f 6175  test_contains_au
+0000ea80: 746f 6573 6361 7065 5f65 7363 6170 6528  toescape_escape(
+0000ea90: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+0000eaa0: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
+0000eab0: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
+0000eac0: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
+0000ead0: 6f72 7420 4c49 4b45 2045 5343 4150 4520  ort LIKE ESCAPE 
+0000eae0: 636c 6175 7365 2229 0a20 2020 2064 6566  clause").    def
+0000eaf0: 2074 6573 745f 636f 6e74 6169 6e73 5f65   test_contains_e
+0000eb00: 7363 6170 6528 7365 6c66 293a 0a20 2020  scape(self):.   
+0000eb10: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
+0000eb20: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
+0000eb30: 2822 5370 616e 6e65 7220 646f 6573 6e27  ("Spanner doesn'
+0000eb40: 7420 7375 7070 6f72 7420 4c49 4b45 2045  t support LIKE E
+0000eb50: 5343 4150 4520 636c 6175 7365 2229 0a20  SCAPE clause"). 
+0000eb60: 2020 2064 6566 2074 6573 745f 656e 6473     def test_ends
+0000eb70: 7769 7468 5f61 7574 6f65 7363 6170 6528  with_autoescape(
+0000eb80: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+0000eb90: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
+0000eba0: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
+0000ebb0: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
+0000ebc0: 6f72 7420 4c49 4b45 2045 5343 4150 4520  ort LIKE ESCAPE 
+0000ebd0: 636c 6175 7365 2229 0a20 2020 2064 6566  clause").    def
+0000ebe0: 2074 6573 745f 656e 6473 7769 7468 5f65   test_endswith_e
+0000ebf0: 7363 6170 6528 7365 6c66 293a 0a20 2020  scape(self):.   
+0000ec00: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
+0000ec10: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
+0000ec20: 2822 5370 616e 6e65 7220 646f 6573 6e27  ("Spanner doesn'
+0000ec30: 7420 7375 7070 6f72 7420 4c49 4b45 2045  t support LIKE E
+0000ec40: 5343 4150 4520 636c 6175 7365 2229 0a20  SCAPE clause"). 
+0000ec50: 2020 2064 6566 2074 6573 745f 656e 6473     def test_ends
+0000ec60: 7769 7468 5f61 7574 6f65 7363 6170 655f  with_autoescape_
+0000ec70: 6573 6361 7065 2873 656c 6629 3a0a 2020  escape(self):.  
+0000ec80: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+0000ec90: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+0000eca0: 7028 2253 7061 6e6e 6572 2064 6f65 736e  p("Spanner doesn
+0000ecb0: 2774 2073 7570 706f 7274 204c 494b 4520  't support LIKE 
+0000ecc0: 4553 4341 5045 2063 6c61 7573 6522 290a  ESCAPE clause").
+0000ecd0: 2020 2020 6465 6620 7465 7374 5f73 7461      def test_sta
+0000ece0: 7274 7377 6974 685f 6175 746f 6573 6361  rtswith_autoesca
+0000ecf0: 7065 2873 656c 6629 3a0a 2020 2020 2020  pe(self):.      
+0000ed00: 2020 7061 7373 0a0a 2020 2020 4070 7974    pass..    @pyt
+0000ed10: 6573 742e 6d61 726b 2e73 6b69 7028 2253  est.mark.skip("S
+0000ed20: 7061 6e6e 6572 2064 6f65 736e 2774 2073  panner doesn't s
+0000ed30: 7570 706f 7274 204c 494b 4520 4553 4341  upport LIKE ESCA
+0000ed40: 5045 2063 6c61 7573 6522 290a 2020 2020  PE clause").    
+0000ed50: 6465 6620 7465 7374 5f73 7461 7274 7377  def test_startsw
+0000ed60: 6974 685f 6573 6361 7065 2873 656c 6629  ith_escape(self)
+0000ed70: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+0000ed80: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+0000ed90: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
+0000eda0: 6f65 736e 2774 2073 7570 706f 7274 204c  oesn't support L
+0000edb0: 494b 4520 4553 4341 5045 2063 6c61 7573  IKE ESCAPE claus
+0000edc0: 6522 290a 2020 2020 6465 6620 7465 7374  e").    def test
+0000edd0: 5f73 7461 7274 7377 6974 685f 6175 746f  _startswith_auto
+0000ede0: 6573 6361 7065 5f65 7363 6170 6528 7365  escape_escape(se
+0000edf0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+0000ee00: 730a 0a20 2020 2064 6566 2074 6573 745f  s..    def test_
+0000ee10: 6573 6361 7065 5f6b 6579 776f 7264 5f72  escape_keyword_r
+0000ee20: 6169 7365 7328 7365 6c66 293a 0a20 2020  aises(self):.   
+0000ee30: 2020 2020 2022 2222 4368 6563 6b20 7468       """Check th
+0000ee40: 6174 2045 5343 4150 4520 6b65 7977 6f72  at ESCAPE keywor
+0000ee50: 6420 6361 7573 6573 2061 6e20 6578 6365  d causes an exce
+0000ee60: 7074 696f 6e20 7768 656e 2075 7365 642e  ption when used.
+0000ee70: 2222 220a 2020 2020 2020 2020 7769 7468  """.        with
+0000ee80: 2070 7974 6573 742e 7261 6973 6573 284e   pytest.raises(N
+0000ee90: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
+0000eea0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+0000eeb0: 2063 6f6c 203d 2073 656c 662e 7461 626c   col = self.tabl
+0000eec0: 6573 2e73 6f6d 655f 7461 626c 652e 632e  es.some_table.c.
+0000eed0: 6461 7461 0a20 2020 2020 2020 2020 2020  data.           
+0000eee0: 2073 656c 662e 5f74 6573 7428 636f 6c2e   self._test(col.
+0000eef0: 636f 6e74 6169 6e73 2822 6223 2363 6465  contains("b##cde
+0000ef00: 222c 2065 7363 6170 653d 2223 2229 2c20  ", escape="#"), 
+0000ef10: 7b37 7d29 0a0a 0a40 7079 7465 7374 2e6d  {7})...@pytest.m
+0000ef20: 6172 6b2e 736b 6970 2822 5370 616e 6e65  ark.skip("Spanne
+0000ef30: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
+0000ef40: 7420 4953 2044 4953 5449 4e43 5420 4652  t IS DISTINCT FR
+0000ef50: 4f4d 2063 6c61 7573 6522 290a 636c 6173  OM clause").clas
+0000ef60: 7320 4973 4f72 4973 4e6f 7444 6973 7469  s IsOrIsNotDisti
+0000ef70: 6e63 7446 726f 6d54 6573 7428 5f49 734f  nctFromTest(_IsO
+0000ef80: 7249 734e 6f74 4469 7374 696e 6374 4672  rIsNotDistinctFr
+0000ef90: 6f6d 5465 7374 293a 0a20 2020 2070 6173  omTest):.    pas
+0000efa0: 730a 0a0a 636c 6173 7320 4f72 6465 7242  s...class OrderB
+0000efb0: 794c 6162 656c 5465 7374 285f 4f72 6465  yLabelTest(_Orde
+0000efc0: 7242 794c 6162 656c 5465 7374 293a 0a20  rByLabelTest):. 
+0000efd0: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+0000efe0: 736b 6970 280a 2020 2020 2020 2020 2253  skip(.        "S
+0000eff0: 7061 6e6e 6572 2072 6571 7569 7265 7320  panner requires 
+0000f000: 616e 2061 6c69 6173 2066 6f72 2074 6865  an alias for the
+0000f010: 2047 524f 5550 2042 5920 6c69 7374 2077   GROUP BY list w
+0000f020: 6865 6e20 7370 6563 6966 7969 6e67 2064  hen specifying d
+0000f030: 6572 6976 6564 2022 0a20 2020 2020 2020  erived ".       
+0000f040: 2022 636f 6c75 6d6e 7320 616c 736f 2075   "columns also u
+0000f050: 7365 6420 696e 2053 454c 4543 5422 0a20  sed in SELECT". 
+0000f060: 2020 2029 0a20 2020 2064 6566 2074 6573     ).    def tes
+0000f070: 745f 6772 6f75 705f 6279 5f63 6f6d 706f  t_group_by_compo
+0000f080: 7365 6428 7365 6c66 293a 0a20 2020 2020  sed(self):.     
+0000f090: 2020 2070 6173 730a 0a0a 636c 6173 7320     pass...class 
+0000f0a0: 436f 6d70 6f75 6e64 5365 6c65 6374 5465  CompoundSelectTe
+0000f0b0: 7374 285f 436f 6d70 6f75 6e64 5365 6c65  st(_CompoundSele
+0000f0c0: 6374 5465 7374 293a 0a20 2020 2022 2222  ctTest):.    """
+0000f0d0: 0a20 2020 2053 6565 3a20 6874 7470 733a  .    See: https:
+0000f0e0: 2f2f 6769 7468 7562 2e63 6f6d 2f67 6f6f  //github.com/goo
+0000f0f0: 676c 6561 7069 732f 7079 7468 6f6e 2d73  gleapis/python-s
+0000f100: 7061 6e6e 6572 2f69 7373 7565 732f 3334  panner/issues/34
+0000f110: 370a 2020 2020 2222 220a 0a20 2020 2040  7.    """..    @
+0000f120: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
+0000f130: 280a 2020 2020 2020 2020 2253 7061 6e6e  (.        "Spann
+0000f140: 6572 2044 4241 5049 2069 6e63 6f72 7265  er DBAPI incorre
+0000f150: 6374 6c79 2063 6c61 7373 6966 7920 7468  ctly classify th
+0000f160: 6520 7374 6174 656d 656e 7420 7374 6172  e statement star
+0000f170: 7469 6e67 2077 6974 6820 6272 6163 6b65  ting with bracke
+0000f180: 7473 2e22 0a20 2020 2029 0a20 2020 2064  ts.".    ).    d
+0000f190: 6566 2074 6573 745f 6c69 6d69 745f 6f66  ef test_limit_of
+0000f1a0: 6673 6574 5f73 656c 6563 7461 626c 655f  fset_selectable_
+0000f1b0: 696e 5f75 6e69 6f6e 7328 7365 6c66 293a  in_unions(self):
+0000f1c0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+0000f1d0: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+0000f1e0: 736b 6970 280a 2020 2020 2020 2020 2253  skip(.        "S
+0000f1f0: 7061 6e6e 6572 2044 4241 5049 2069 6e63  panner DBAPI inc
+0000f200: 6f72 7265 6374 6c79 2063 6c61 7373 6966  orrectly classif
+0000f210: 7920 7468 6520 7374 6174 656d 656e 7420  y the statement 
+0000f220: 7374 6172 7469 6e67 2077 6974 6820 6272  starting with br
+0000f230: 6163 6b65 7473 2e22 0a20 2020 2029 0a20  ackets.".    ). 
+0000f240: 2020 2064 6566 2074 6573 745f 6f72 6465     def test_orde
+0000f250: 725f 6279 5f73 656c 6563 7461 626c 655f  r_by_selectable_
+0000f260: 696e 5f75 6e69 6f6e 7328 7365 6c66 293a  in_unions(self):
+0000f270: 0a20 2020 2020 2020 2070 6173 730a 0a0a  .        pass...
+0000f280: 636c 6173 7320 5465 7374 5175 6572 7948  class TestQueryH
+0000f290: 696e 7473 2866 6978 7475 7265 732e 5461  ints(fixtures.Ta
+0000f2a0: 626c 6573 5465 7374 293a 0a20 2020 2022  blesTest):.    "
+0000f2b0: 2222 0a20 2020 2043 6f6d 7069 6c65 2061  "".    Compile a
+0000f2c0: 2063 6f6d 706c 6578 2071 7565 7279 2077   complex query w
+0000f2d0: 6974 6820 4a4f 494e 2061 6e64 2063 6865  ith JOIN and che
+0000f2e0: 636b 2074 6861 740a 2020 2020 7468 6520  ck that.    the 
+0000f2f0: 7461 626c 6520 6869 6e74 2077 6173 2073  table hint was s
+0000f300: 6574 2069 6e74 6f20 7468 6520 7269 6768  et into the righ
+0000f310: 7420 706c 6163 652e 0a20 2020 2022 2222  t place..    """
+0000f320: 0a0a 2020 2020 5f5f 6261 636b 656e 645f  ..    __backend_
+0000f330: 5f20 3d20 5472 7565 0a0a 2020 2020 6465  _ = True..    de
+0000f340: 6620 7465 7374 5f63 6f6d 706c 6578 5f71  f test_complex_q
+0000f350: 7565 7279 5f74 6162 6c65 5f68 696e 7473  uery_table_hints
+0000f360: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000f370: 4558 5045 4354 4544 5f51 5545 5259 203d  EXPECTED_QUERY =
+0000f380: 2028 0a20 2020 2020 2020 2020 2020 2022   (.            "
+0000f390: 5345 4c45 4354 2075 7365 7273 2e69 642c  SELECT users.id,
+0000f3a0: 2075 7365 7273 2e6e 616d 6520 5c6e 4652   users.name \nFR
+0000f3b0: 4f4d 2075 7365 7273 2040 7b46 4f52 4345  OM users @{FORCE
+0000f3c0: 5f49 4e44 4558 3d74 6162 6c65 5f31 5f62  _INDEX=table_1_b
+0000f3d0: 795f 696e 745f 6964 787d 220a 2020 2020  y_int_idx}".    
+0000f3e0: 2020 2020 2020 2020 2220 4a4f 494e 2061          " JOIN a
+0000f3f0: 6464 7265 7373 6573 204f 4e20 7573 6572  ddresses ON user
+0000f400: 732e 6964 203d 2061 6464 7265 7373 6573  s.id = addresses
+0000f410: 2e75 7365 725f 6964 2022 0a20 2020 2020  .user_id ".     
+0000f420: 2020 2020 2020 2022 5c6e 5748 4552 4520         "\nWHERE 
+0000f430: 7573 6572 732e 6e61 6d65 2049 4e20 285f  users.name IN (_
+0000f440: 5f5b 504f 5354 434f 4d50 494c 455f 6e61  _[POSTCOMPILE_na
+0000f450: 6d65 5f31 5d29 220a 2020 2020 2020 2020  me_1])".        
+0000f460: 290a 0a20 2020 2020 2020 2042 6173 6520  )..        Base 
+0000f470: 3d20 6465 636c 6172 6174 6976 655f 6261  = declarative_ba
+0000f480: 7365 2829 0a20 2020 2020 2020 2065 6e67  se().        eng
+0000f490: 696e 6520 3d20 6372 6561 7465 5f65 6e67  ine = create_eng
+0000f4a0: 696e 6528 0a20 2020 2020 2020 2020 2020  ine(.           
+0000f4b0: 2022 7370 616e 6e65 723a 2f2f 2f70 726f   "spanner:///pro
+0000f4c0: 6a65 6374 732f 7072 6f6a 6563 742d 6964  jects/project-id
+0000f4d0: 2f69 6e73 7461 6e63 6573 2f69 6e73 7461  /instances/insta
+0000f4e0: 6e63 652d 6964 2f64 6174 6162 6173 6573  nce-id/databases
+0000f4f0: 2f64 6174 6162 6173 652d 6964 220a 2020  /database-id".  
+0000f500: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000f510: 2063 6c61 7373 2055 7365 7228 4261 7365   class User(Base
+0000f520: 293a 0a20 2020 2020 2020 2020 2020 205f  ):.            _
+0000f530: 5f74 6162 6c65 6e61 6d65 5f5f 203d 2022  _tablename__ = "
+0000f540: 7573 6572 7322 0a20 2020 2020 2020 2020  users".         
+0000f550: 2020 2069 6420 3d20 436f 6c75 6d6e 2849     id = Column(I
+0000f560: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
+0000f570: 6b65 793d 5472 7565 290a 2020 2020 2020  key=True).      
+0000f580: 2020 2020 2020 6e61 6d65 203d 2043 6f6c        name = Col
+0000f590: 756d 6e28 5374 7269 6e67 2835 3029 290a  umn(String(50)).
+0000f5a0: 2020 2020 2020 2020 2020 2020 6164 6472              addr
+0000f5b0: 6573 7365 7320 3d20 7265 6c61 7469 6f6e  esses = relation
+0000f5c0: 2822 4164 6472 6573 7322 2c20 6261 636b  ("Address", back
+0000f5d0: 7265 663d 2275 7365 7222 290a 0a20 2020  ref="user")..   
+0000f5e0: 2020 2020 2063 6c61 7373 2041 6464 7265       class Addre
+0000f5f0: 7373 2842 6173 6529 3a0a 2020 2020 2020  ss(Base):.      
+0000f600: 2020 2020 2020 5f5f 7461 626c 656e 616d        __tablenam
+0000f610: 655f 5f20 3d20 2261 6464 7265 7373 6573  e__ = "addresses
+0000f620: 220a 2020 2020 2020 2020 2020 2020 6964  ".            id
+0000f630: 203d 2043 6f6c 756d 6e28 496e 7465 6765   = Column(Intege
+0000f640: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
+0000f650: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+0000f660: 2065 6d61 696c 203d 2043 6f6c 756d 6e28   email = Column(
+0000f670: 5374 7269 6e67 2835 3029 290a 2020 2020  String(50)).    
+0000f680: 2020 2020 2020 2020 7573 6572 5f69 6420          user_id 
+0000f690: 3d20 436f 6c75 6d6e 2849 6e74 6567 6572  = Column(Integer
+0000f6a0: 2c20 466f 7265 6967 6e4b 6579 2822 7573  , ForeignKey("us
+0000f6b0: 6572 732e 6964 2229 290a 0a20 2020 2020  ers.id"))..     
+0000f6c0: 2020 2073 6573 7369 6f6e 203d 2053 6573     session = Ses
+0000f6d0: 7369 6f6e 2865 6e67 696e 6529 0a0a 2020  sion(engine)..  
+0000f6e0: 2020 2020 2020 7175 6572 7920 3d20 7365        query = se
+0000f6f0: 7373 696f 6e2e 7175 6572 7928 5573 6572  ssion.query(User
+0000f700: 290a 2020 2020 2020 2020 7175 6572 7920  ).        query 
+0000f710: 3d20 7175 6572 792e 7769 7468 5f68 696e  = query.with_hin
+0000f720: 7428 0a20 2020 2020 2020 2020 2020 2073  t(.            s
+0000f730: 656c 6563 7461 626c 653d 5573 6572 2c20  electable=User, 
+0000f740: 7465 7874 3d22 407b 464f 5243 455f 494e  text="@{FORCE_IN
+0000f750: 4445 583d 7461 626c 655f 315f 6279 5f69  DEX=table_1_by_i
+0000f760: 6e74 5f69 6478 7d22 0a20 2020 2020 2020  nt_idx}".       
+0000f770: 2029 0a0a 2020 2020 2020 2020 7175 6572   )..        quer
+0000f780: 7920 3d20 7175 6572 792e 6669 6c74 6572  y = query.filter
+0000f790: 2855 7365 722e 6e61 6d65 2e69 6e5f 285b  (User.name.in_([
+0000f7a0: 2276 616c 3122 2c20 2276 616c 3222 5d29  "val1", "val2"])
+0000f7b0: 290a 2020 2020 2020 2020 7175 6572 7920  ).        query 
+0000f7c0: 3d20 7175 6572 792e 6a6f 696e 2841 6464  = query.join(Add
+0000f7d0: 7265 7373 290a 0a20 2020 2020 2020 2061  ress)..        a
+0000f7e0: 7373 6572 7420 7374 7228 7175 6572 792e  ssert str(query.
+0000f7f0: 7374 6174 656d 656e 742e 636f 6d70 696c  statement.compil
+0000f800: 6528 7365 7373 696f 6e2e 6269 6e64 2929  e(session.bind))
+0000f810: 203d 3d20 4558 5045 4354 4544 5f51 5545   == EXPECTED_QUE
+0000f820: 5259 0a0a 0a63 6c61 7373 2049 6e74 6572  RY...class Inter
+0000f830: 6c65 6176 6564 5461 626c 6573 5465 7374  leavedTablesTest
+0000f840: 2866 6978 7475 7265 732e 5465 7374 4261  (fixtures.TestBa
+0000f850: 7365 293a 0a20 2020 2022 2222 0a20 2020  se):.    """.   
+0000f860: 2043 6865 636b 2074 6861 7420 4352 4541   Check that CREA
+0000f870: 5445 2054 4142 4c45 2073 7461 7465 6d65  TE TABLE stateme
+0000f880: 6e74 7320 666f 7220 696e 7465 726c 6561  nts for interlea
+0000f890: 7665 6420 7461 626c 6573 2061 7265 2063  ved tables are c
+0000f8a0: 6f72 7265 6374 6c79 0a20 2020 2067 656e  orrectly.    gen
+0000f8b0: 6572 6174 6564 2e0a 2020 2020 2222 220a  erated..    """.
+0000f8c0: 0a20 2020 2064 6566 2073 6574 5570 2873  .    def setUp(s
+0000f8d0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+0000f8e0: 6c66 2e5f 656e 6769 6e65 203d 2063 7265  lf._engine = cre
+0000f8f0: 6174 655f 656e 6769 6e65 280a 2020 2020  ate_engine(.    
+0000f900: 2020 2020 2020 2020 2273 7061 6e6e 6572          "spanner
+0000f910: 3a2f 2f2f 7072 6f6a 6563 7473 2f61 7070  :///projects/app
+0000f920: 6465 762d 736f 6461 2d73 7061 6e6e 6572  dev-soda-spanner
+0000f930: 2d73 7461 6769 6e67 2f69 6e73 7461 6e63  -staging/instanc
+0000f940: 6573 2f22 0a20 2020 2020 2020 2020 2020  es/".           
+0000f950: 2022 7371 6c61 6c63 6865 6d79 2d64 6961   "sqlalchemy-dia
+0000f960: 6c65 6374 2d74 6573 742f 6461 7461 6261  lect-test/databa
+0000f970: 7365 732f 636f 6d70 6c69 616e 6365 2d74  ses/compliance-t
+0000f980: 6573 7422 0a20 2020 2020 2020 2029 0a20  est".        ). 
+0000f990: 2020 2020 2020 2073 656c 662e 5f6d 6574         self._met
+0000f9a0: 6164 6174 6120 3d20 4d65 7461 4461 7461  adata = MetaData
+0000f9b0: 2862 696e 643d 7365 6c66 2e5f 656e 6769  (bind=self._engi
+0000f9c0: 6e65 290a 0a20 2020 2064 6566 2074 6573  ne)..    def tes
+0000f9d0: 745f 696e 7465 726c 6561 7665 2873 656c  t_interleave(sel
+0000f9e0: 6629 3a0a 2020 2020 2020 2020 4558 505f  f):.        EXP_
+0000f9f0: 5155 4552 5920 3d20 280a 2020 2020 2020  QUERY = (.      
+0000fa00: 2020 2020 2020 225c 6e43 5245 4154 4520        "\nCREATE 
+0000fa10: 5441 424c 4520 636c 6965 6e74 2028 5c6e  TABLE client (\n
+0000fa20: 5c74 7465 616d 5f69 6420 494e 5436 3420  \tteam_id INT64 
+0000fa30: 4e4f 5420 4e55 4c4c 2c20 220a 2020 2020  NOT NULL, ".    
+0000fa40: 2020 2020 2020 2020 225c 6e5c 7463 6c69          "\n\tcli
+0000fa50: 656e 745f 6964 2049 4e54 3634 204e 4f54  ent_id INT64 NOT
+0000fa60: 204e 554c 4c2c 2022 0a20 2020 2020 2020   NULL, ".       
+0000fa70: 2020 2020 2022 5c6e 5c74 636c 6965 6e74       "\n\tclient
+0000fa80: 5f6e 616d 6520 5354 5249 4e47 2831 3629  _name STRING(16)
+0000fa90: 204e 4f54 204e 554c 4c22 0a20 2020 2020   NOT NULL".     
+0000faa0: 2020 2020 2020 2022 5c6e 2920 5052 494d         "\n) PRIM
+0000fab0: 4152 5920 4b45 5920 2874 6561 6d5f 6964  ARY KEY (team_id
+0000fac0: 2c20 636c 6965 6e74 5f69 6429 2c22 0a20  , client_id),". 
+0000fad0: 2020 2020 2020 2020 2020 2022 5c6e 494e             "\nIN
+0000fae0: 5445 524c 4541 5645 2049 4e20 5041 5245  TERLEAVE IN PARE
+0000faf0: 4e54 2074 6561 6d5c 6e5c 6e22 0a20 2020  NT team\n\n".   
+0000fb00: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
+0000fb10: 6c69 656e 7420 3d20 5461 626c 6528 0a20  lient = Table(. 
+0000fb20: 2020 2020 2020 2020 2020 2022 636c 6965             "clie
+0000fb30: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
+0000fb40: 2073 656c 662e 5f6d 6574 6164 6174 612c   self._metadata,
+0000fb50: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
+0000fb60: 756d 6e28 2274 6561 6d5f 6964 222c 2049  umn("team_id", I
+0000fb70: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
+0000fb80: 6b65 793d 5472 7565 292c 0a20 2020 2020  key=True),.     
+0000fb90: 2020 2020 2020 2043 6f6c 756d 6e28 2263         Column("c
+0000fba0: 6c69 656e 745f 6964 222c 2049 6e74 6567  lient_id", Integ
+0000fbb0: 6572 2c20 7072 696d 6172 795f 6b65 793d  er, primary_key=
+0000fbc0: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
+0000fbd0: 2020 2043 6f6c 756d 6e28 2263 6c69 656e     Column("clien
+0000fbe0: 745f 6e61 6d65 222c 2053 7472 696e 6728  t_name", String(
+0000fbf0: 3136 292c 206e 756c 6c61 626c 653d 4661  16), nullable=Fa
+0000fc00: 6c73 6529 2c0a 2020 2020 2020 2020 2020  lse),.          
+0000fc10: 2020 7370 616e 6e65 725f 696e 7465 726c    spanner_interl
+0000fc20: 6561 7665 5f69 6e3d 2274 6561 6d22 2c0a  eave_in="team",.
+0000fc30: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000fc40: 2020 7769 7468 206d 6f63 6b2e 7061 7463    with mock.patc
+0000fc50: 6828 2267 6f6f 676c 652e 636c 6f75 642e  h("google.cloud.
+0000fc60: 7370 616e 6e65 725f 6462 6170 692e 6375  spanner_dbapi.cu
+0000fc70: 7273 6f72 2e43 7572 736f 722e 6578 6563  rsor.Cursor.exec
+0000fc80: 7574 6522 2920 6173 2065 7865 6375 7465  ute") as execute
+0000fc90: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
+0000fca0: 6965 6e74 2e63 7265 6174 6528 7365 6c66  ient.create(self
+0000fcb0: 2e5f 656e 6769 6e65 290a 2020 2020 2020  ._engine).      
+0000fcc0: 2020 2020 2020 6578 6563 7574 652e 6173        execute.as
+0000fcd0: 7365 7274 5f63 616c 6c65 645f 6f6e 6365  sert_called_once
+0000fce0: 5f77 6974 6828 4558 505f 5155 4552 592c  _with(EXP_QUERY,
+0000fcf0: 205b 5d29 0a0a 2020 2020 6465 6620 7465   [])..    def te
+0000fd00: 7374 5f69 6e74 6572 6c65 6176 655f 6f6e  st_interleave_on
+0000fd10: 5f64 656c 6574 655f 6361 7363 6164 6528  _delete_cascade(
+0000fd20: 7365 6c66 293a 0a20 2020 2020 2020 2045  self):.        E
+0000fd30: 5850 5f51 5545 5259 203d 2028 0a20 2020  XP_QUERY = (.   
+0000fd40: 2020 2020 2020 2020 2022 5c6e 4352 4541           "\nCREA
+0000fd50: 5445 2054 4142 4c45 2063 6c69 656e 7420  TE TABLE client 
+0000fd60: 285c 6e5c 7474 6561 6d5f 6964 2049 4e54  (\n\tteam_id INT
+0000fd70: 3634 204e 4f54 204e 554c 4c2c 2022 0a20  64 NOT NULL, ". 
+0000fd80: 2020 2020 2020 2020 2020 2022 5c6e 5c74             "\n\t
+0000fd90: 636c 6965 6e74 5f69 6420 494e 5436 3420  client_id INT64 
+0000fda0: 4e4f 5420 4e55 4c4c 2c20 220a 2020 2020  NOT NULL, ".    
+0000fdb0: 2020 2020 2020 2020 225c 6e5c 7463 6c69          "\n\tcli
+0000fdc0: 656e 745f 6e61 6d65 2053 5452 494e 4728  ent_name STRING(
+0000fdd0: 3136 2920 4e4f 5420 4e55 4c4c 220a 2020  16) NOT NULL".  
+0000fde0: 2020 2020 2020 2020 2020 225c 6e29 2050            "\n) P
+0000fdf0: 5249 4d41 5259 204b 4559 2028 7465 616d  RIMARY KEY (team
+0000fe00: 5f69 642c 2063 6c69 656e 745f 6964 292c  _id, client_id),
+0000fe10: 220a 2020 2020 2020 2020 2020 2020 225c  ".            "\
+0000fe20: 6e49 4e54 4552 4c45 4156 4520 494e 2050  nINTERLEAVE IN P
+0000fe30: 4152 454e 5420 7465 616d 204f 4e20 4445  ARENT team ON DE
+0000fe40: 4c45 5445 2043 4153 4341 4445 5c6e 5c6e  LETE CASCADE\n\n
+0000fe50: 220a 2020 2020 2020 2020 290a 2020 2020  ".        ).    
+0000fe60: 2020 2020 636c 6965 6e74 203d 2054 6162      client = Tab
+0000fe70: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
+0000fe80: 2263 6c69 656e 7422 2c0a 2020 2020 2020  "client",.      
+0000fe90: 2020 2020 2020 7365 6c66 2e5f 6d65 7461        self._meta
+0000fea0: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
+0000feb0: 2020 436f 6c75 6d6e 2822 7465 616d 5f69    Column("team_i
+0000fec0: 6422 2c20 496e 7465 6765 722c 2070 7269  d", Integer, pri
+0000fed0: 6d61 7279 5f6b 6579 3d54 7275 6529 2c0a  mary_key=True),.
+0000fee0: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
+0000fef0: 6d6e 2822 636c 6965 6e74 5f69 6422 2c20  mn("client_id", 
+0000ff00: 496e 7465 6765 722c 2070 7269 6d61 7279  Integer, primary
+0000ff10: 5f6b 6579 3d54 7275 6529 2c0a 2020 2020  _key=True),.    
+0000ff20: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+0000ff30: 636c 6965 6e74 5f6e 616d 6522 2c20 5374  client_name", St
+0000ff40: 7269 6e67 2831 3629 2c20 6e75 6c6c 6162  ring(16), nullab
+0000ff50: 6c65 3d46 616c 7365 292c 0a20 2020 2020  le=False),.     
+0000ff60: 2020 2020 2020 2073 7061 6e6e 6572 5f69         spanner_i
+0000ff70: 6e74 6572 6c65 6176 655f 696e 3d22 7465  nterleave_in="te
+0000ff80: 616d 222c 0a20 2020 2020 2020 2020 2020  am",.           
+0000ff90: 2073 7061 6e6e 6572 5f69 6e74 6572 6c65   spanner_interle
+0000ffa0: 6176 655f 6f6e 5f64 656c 6574 655f 6361  ave_on_delete_ca
+0000ffb0: 7363 6164 653d 5472 7565 2c0a 2020 2020  scade=True,.    
+0000ffc0: 2020 2020 290a 2020 2020 2020 2020 7769      ).        wi
+0000ffd0: 7468 206d 6f63 6b2e 7061 7463 6828 2267  th mock.patch("g
+0000ffe0: 6f6f 676c 652e 636c 6f75 642e 7370 616e  oogle.cloud.span
+0000fff0: 6e65 725f 6462 6170 692e 6375 7273 6f72  ner_dbapi.cursor
+00010000: 2e43 7572 736f 722e 6578 6563 7574 6522  .Cursor.execute"
+00010010: 2920 6173 2065 7865 6375 7465 3a0a 2020  ) as execute:.  
+00010020: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+00010030: 2e63 7265 6174 6528 7365 6c66 2e5f 656e  .create(self._en
+00010040: 6769 6e65 290a 2020 2020 2020 2020 2020  gine).          
+00010050: 2020 6578 6563 7574 652e 6173 7365 7274    execute.assert
+00010060: 5f63 616c 6c65 645f 6f6e 6365 5f77 6974  _called_once_wit
+00010070: 6828 4558 505f 5155 4552 592c 205b 5d29  h(EXP_QUERY, [])
+00010080: 0a0a 0a63 6c61 7373 2055 7365 7241 6765  ...class UserAge
+00010090: 6e74 5465 7374 2866 6978 7475 7265 732e  ntTest(fixtures.
+000100a0: 5465 7374 4261 7365 293a 0a20 2020 2022  TestBase):.    "
+000100b0: 2222 4368 6563 6b20 7468 6174 2053 514c  ""Check that SQL
+000100c0: 416c 6368 656d 7920 6469 616c 6563 7420  Alchemy dialect 
+000100d0: 7573 6573 2063 6f72 7265 6374 2075 7365  uses correct use
+000100e0: 7220 6167 656e 742e 2222 220a 0a20 2020  r agent."""..   
+000100f0: 2064 6566 2073 6574 5570 2873 656c 6629   def setUp(self)
+00010100: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00010110: 656e 6769 6e65 203d 2063 7265 6174 655f  engine = create_
+00010120: 656e 6769 6e65 280a 2020 2020 2020 2020  engine(.        
+00010130: 2020 2020 2273 7061 6e6e 6572 3a2f 2f2f      "spanner:///
+00010140: 7072 6f6a 6563 7473 2f61 7070 6465 762d  projects/appdev-
+00010150: 736f 6461 2d73 7061 6e6e 6572 2d73 7461  soda-spanner-sta
+00010160: 6769 6e67 2f69 6e73 7461 6e63 6573 2f22  ging/instances/"
+00010170: 0a20 2020 2020 2020 2020 2020 2022 7371  .            "sq
+00010180: 6c61 6c63 6865 6d79 2d64 6961 6c65 6374  lalchemy-dialect
+00010190: 2d74 6573 742f 6461 7461 6261 7365 732f  -test/databases/
+000101a0: 636f 6d70 6c69 616e 6365 2d74 6573 7422  compliance-test"
+000101b0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000101c0: 2020 2073 656c 662e 5f6d 6574 6164 6174     self._metadat
+000101d0: 6120 3d20 4d65 7461 4461 7461 2862 696e  a = MetaData(bin
+000101e0: 643d 7365 6c66 2e5f 656e 6769 6e65 290a  d=self._engine).
+000101f0: 0a20 2020 2064 6566 2074 6573 745f 7573  .    def test_us
+00010200: 6572 5f61 6765 6e74 2873 656c 6629 3a0a  er_agent(self):.
+00010210: 2020 2020 2020 2020 6469 7374 203d 2070          dist = p
+00010220: 6b67 5f72 6573 6f75 7263 6573 2e67 6574  kg_resources.get
+00010230: 5f64 6973 7472 6962 7574 696f 6e28 2273  _distribution("s
+00010240: 716c 616c 6368 656d 792d 7370 616e 6e65  qlalchemy-spanne
+00010250: 7222 290a 0a20 2020 2020 2020 2077 6974  r")..        wit
+00010260: 6820 7365 6c66 2e5f 656e 6769 6e65 2e63  h self._engine.c
+00010270: 6f6e 6e65 6374 2829 2061 7320 636f 6e6e  onnect() as conn
+00010280: 6563 7469 6f6e 3a0a 2020 2020 2020 2020  ection:.        
+00010290: 2020 2020 6173 7365 7274 2028 0a20 2020      assert (.   
+000102a0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+000102b0: 6e65 6374 696f 6e2e 636f 6e6e 6563 7469  nection.connecti
+000102c0: 6f6e 2e69 6e73 7461 6e63 652e 5f63 6c69  on.instance._cli
+000102d0: 656e 742e 5f63 6c69 656e 745f 696e 666f  ent._client_info
+000102e0: 2e75 7365 725f 6167 656e 740a 2020 2020  .user_agent.    
+000102f0: 2020 2020 2020 2020 2020 2020 3d3d 2022              == "
+00010300: 676c 2d22 202b 2064 6973 742e 7072 6f6a  gl-" + dist.proj
+00010310: 6563 745f 6e61 6d65 202b 2022 2f22 202b  ect_name + "/" +
+00010320: 2064 6973 742e 7665 7273 696f 6e0a 2020   dist.version.  
+00010330: 2020 2020 2020 2020 2020 290a 0a0a 636c            )...cl
+00010340: 6173 7320 5369 6d70 6c65 5570 6461 7465  ass SimpleUpdate
+00010350: 4465 6c65 7465 5465 7374 285f 5369 6d70  DeleteTest(_Simp
+00010360: 6c65 5570 6461 7465 4465 6c65 7465 5465  leUpdateDeleteTe
+00010370: 7374 293a 0a20 2020 2022 2222 0a20 2020  st):.    """.   
+00010380: 2053 5041 4e4e 4552 204f 5645 5252 4944   SPANNER OVERRID
+00010390: 453a 0a0a 2020 2020 5370 616e 6e65 7220  E:..    Spanner 
+000103a0: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
+000103b0: 6072 6f77 636f 756e 7460 2070 726f 7065  `rowcount` prope
+000103c0: 7274 792e 2054 6865 7365 0a20 2020 2074  rty. These.    t
+000103d0: 6573 7420 6361 7365 7320 6f76 6572 7269  est cases overri
+000103e0: 6465 7320 6f6d 6974 2060 726f 7763 6f75  des omit `rowcou
+000103f0: 6e74 6020 6368 6563 6b73 2e0a 2020 2020  nt` checks..    
+00010400: 2222 220a 0a20 2020 2064 6566 2074 6573  """..    def tes
+00010410: 745f 6465 6c65 7465 2873 656c 662c 2063  t_delete(self, c
+00010420: 6f6e 6e65 6374 696f 6e29 3a0a 2020 2020  onnection):.    
+00010430: 2020 2020 7420 3d20 7365 6c66 2e74 6162      t = self.tab
+00010440: 6c65 732e 706c 6169 6e5f 706b 0a20 2020  les.plain_pk.   
+00010450: 2020 2020 2072 203d 2063 6f6e 6e65 6374       r = connect
+00010460: 696f 6e2e 6578 6563 7574 6528 742e 6465  ion.execute(t.de
+00010470: 6c65 7465 2829 2e77 6865 7265 2874 2e63  lete().where(t.c
+00010480: 2e69 6420 3d3d 2032 2929 0a20 2020 2020  .id == 2)).     
+00010490: 2020 2061 7373 6572 7420 6e6f 7420 722e     assert not r.
+000104a0: 6973 5f69 6e73 6572 740a 2020 2020 2020  is_insert.      
+000104b0: 2020 6173 7365 7274 206e 6f74 2072 2e72    assert not r.r
+000104c0: 6574 7572 6e73 5f72 6f77 730a 2020 2020  eturns_rows.    
+000104d0: 2020 2020 6571 5f28 0a20 2020 2020 2020      eq_(.       
+000104e0: 2020 2020 2063 6f6e 6e65 6374 696f 6e2e       connection.
+000104f0: 6578 6563 7574 6528 742e 7365 6c65 6374  execute(t.select
+00010500: 2829 2e6f 7264 6572 5f62 7928 742e 632e  ().order_by(t.c.
+00010510: 6964 2929 2e66 6574 6368 616c 6c28 292c  id)).fetchall(),
+00010520: 0a20 2020 2020 2020 2020 2020 205b 2831  .            [(1
+00010530: 2c20 2264 3122 292c 2028 332c 2022 6433  , "d1"), (3, "d3
+00010540: 2229 5d2c 0a20 2020 2020 2020 2029 0a0a  ")],.        )..
+00010550: 2020 2020 6465 6620 7465 7374 5f75 7064      def test_upd
+00010560: 6174 6528 7365 6c66 2c20 636f 6e6e 6563  ate(self, connec
+00010570: 7469 6f6e 293a 0a20 2020 2020 2020 2074  tion):.        t
+00010580: 203d 2073 656c 662e 7461 626c 6573 2e70   = self.tables.p
+00010590: 6c61 696e 5f70 6b0a 2020 2020 2020 2020  lain_pk.        
+000105a0: 7220 3d20 636f 6e6e 6563 7469 6f6e 2e65  r = connection.e
+000105b0: 7865 6375 7465 2874 2e75 7064 6174 6528  xecute(t.update(
+000105c0: 292e 7768 6572 6528 742e 632e 6964 203d  ).where(t.c.id =
+000105d0: 3d20 3229 2c20 6469 6374 2864 6174 613d  = 2), dict(data=
+000105e0: 2264 325f 6e65 7722 2929 0a20 2020 2020  "d2_new")).     
+000105f0: 2020 2061 7373 6572 7420 6e6f 7420 722e     assert not r.
+00010600: 6973 5f69 6e73 6572 740a 2020 2020 2020  is_insert.      
+00010610: 2020 6173 7365 7274 206e 6f74 2072 2e72    assert not r.r
+00010620: 6574 7572 6e73 5f72 6f77 730a 0a20 2020  eturns_rows..   
+00010630: 2020 2020 2065 715f 280a 2020 2020 2020       eq_(.      
+00010640: 2020 2020 2020 636f 6e6e 6563 7469 6f6e        connection
+00010650: 2e65 7865 6375 7465 2874 2e73 656c 6563  .execute(t.selec
+00010660: 7428 292e 6f72 6465 725f 6279 2874 2e63  t().order_by(t.c
+00010670: 2e69 6429 292e 6665 7463 6861 6c6c 2829  .id)).fetchall()
+00010680: 2c0a 2020 2020 2020 2020 2020 2020 5b28  ,.            [(
+00010690: 312c 2022 6431 2229 2c20 2832 2c20 2264  1, "d1"), (2, "d
+000106a0: 325f 6e65 7722 292c 2028 332c 2022 6433  2_new"), (3, "d3
+000106b0: 2229 5d2c 0a20 2020 2020 2020 2029 0a0a  ")],.        )..
+000106c0: 0a63 6c61 7373 2048 6173 496e 6465 7854  .class HasIndexT
+000106d0: 6573 7428 5f48 6173 496e 6465 7854 6573  est(_HasIndexTes
+000106e0: 7429 3a0a 2020 2020 4063 6c61 7373 6d65  t):.    @classme
+000106f0: 7468 6f64 0a20 2020 2064 6566 2064 6566  thod.    def def
+00010700: 696e 655f 7461 626c 6573 2863 6c73 2c20  ine_tables(cls, 
+00010710: 6d65 7461 6461 7461 293a 0a20 2020 2020  metadata):.     
+00010720: 2020 2074 7420 3d20 5461 626c 6528 0a20     tt = Table(. 
+00010730: 2020 2020 2020 2020 2020 2022 7465 7374             "test
+00010740: 5f74 6162 6c65 222c 0a20 2020 2020 2020  _table",.       
+00010750: 2020 2020 206d 6574 6164 6174 612c 0a20       metadata,. 
+00010760: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00010770: 6e28 2269 6422 2c20 496e 7465 6765 722c  n("id", Integer,
+00010780: 2070 7269 6d61 7279 5f6b 6579 3d54 7275   primary_key=Tru
+00010790: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+000107a0: 436f 6c75 6d6e 2822 6461 7461 222c 2053  Column("data", S
+000107b0: 7472 696e 6728 3530 2929 2c0a 2020 2020  tring(50)),.    
+000107c0: 2020 2020 290a 2020 2020 2020 2020 7371      ).        sq
+000107d0: 6c61 6c63 6865 6d79 2e49 6e64 6578 2822  lalchemy.Index("
+000107e0: 6d79 5f69 6478 222c 2074 742e 632e 6461  my_idx", tt.c.da
+000107f0: 7461 290a 0a20 2020 2040 7079 7465 7374  ta)..    @pytest
+00010800: 2e6d 6172 6b2e 736b 6970 2822 4e6f 7420  .mark.skip("Not 
+00010810: 7375 7070 6f72 7465 6420 6279 2043 6c6f  supported by Clo
+00010820: 7564 2053 7061 6e6e 6572 2229 0a20 2020  ud Spanner").   
+00010830: 2064 6566 2074 6573 745f 6861 735f 696e   def test_has_in
+00010840: 6465 785f 7363 6865 6d61 2873 656c 6629  dex_schema(self)
+00010850: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00010860: 0a63 6c61 7373 2048 6173 5461 626c 6554  .class HasTableT
+00010870: 6573 7428 5f48 6173 5461 626c 6554 6573  est(_HasTableTes
+00010880: 7429 3a0a 2020 2020 4063 6c61 7373 6d65  t):.    @classme
+00010890: 7468 6f64 0a20 2020 2064 6566 2064 6566  thod.    def def
+000108a0: 696e 655f 7461 626c 6573 2863 6c73 2c20  ine_tables(cls, 
+000108b0: 6d65 7461 6461 7461 293a 0a20 2020 2020  metadata):.     
+000108c0: 2020 2054 6162 6c65 280a 2020 2020 2020     Table(.      
+000108d0: 2020 2020 2020 2274 6573 745f 7461 626c        "test_tabl
+000108e0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+000108f0: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+00010900: 2020 2020 2020 436f 6c75 6d6e 2822 6964        Column("id
+00010910: 222c 2049 6e74 6567 6572 2c20 7072 696d  ", Integer, prim
+00010920: 6172 795f 6b65 793d 5472 7565 292c 0a20  ary_key=True),. 
+00010930: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00010940: 6e28 2264 6174 6122 2c20 5374 7269 6e67  n("data", String
+00010950: 2835 3029 292c 0a20 2020 2020 2020 2029  (50)),.        )
+00010960: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
+00010970: 726b 2e73 6b69 7028 224e 6f74 2073 7570  rk.skip("Not sup
+00010980: 706f 7274 6564 2062 7920 436c 6f75 6420  ported by Cloud 
+00010990: 5370 616e 6e65 7222 290a 2020 2020 6465  Spanner").    de
+000109a0: 6620 7465 7374 5f68 6173 5f74 6162 6c65  f test_has_table
+000109b0: 5f73 6368 656d 6128 7365 6c66 293a 0a20  _schema(self):. 
+000109c0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+000109d0: 2040 7465 7374 696e 672e 7265 7175 6972   @testing.requir
+000109e0: 6573 2e76 6965 7773 0a20 2020 2064 6566  es.views.    def
+000109f0: 2074 6573 745f 6861 735f 7461 626c 655f   test_has_table_
+00010a00: 7669 6577 2873 656c 662c 2063 6f6e 6e65  view(self, conne
+00010a10: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
+00010a20: 7061 7373 0a0a 2020 2020 4074 6573 7469  pass..    @testi
+00010a30: 6e67 2e72 6571 7569 7265 732e 7669 6577  ng.requires.view
+00010a40: 730a 2020 2020 6465 6620 7465 7374 5f68  s.    def test_h
+00010a50: 6173 5f74 6162 6c65 5f76 6965 775f 7363  as_table_view_sc
+00010a60: 6865 6d61 2873 656c 662c 2063 6f6e 6e65  hema(self, conne
+00010a70: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
+00010a80: 7061 7373 0a0a 0a63 6c61 7373 2050 6f73  pass...class Pos
+00010a90: 7443 6f6d 7069 6c65 5061 7261 6d73 5465  tCompileParamsTe
+00010aa0: 7374 285f 506f 7374 436f 6d70 696c 6550  st(_PostCompileP
+00010ab0: 6172 616d 7354 6573 7429 3a0a 2020 2020  aramsTest):.    
+00010ac0: 6465 6620 7465 7374 5f65 7865 6375 7465  def test_execute
+00010ad0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00010ae0: 7461 626c 6520 3d20 7365 6c66 2e74 6162  table = self.tab
+00010af0: 6c65 732e 736f 6d65 5f74 6162 6c65 0a0a  les.some_table..
+00010b00: 2020 2020 2020 2020 7374 6d74 203d 2073          stmt = s
+00010b10: 656c 6563 7428 7461 626c 652e 632e 6964  elect(table.c.id
+00010b20: 292e 7768 6572 6528 0a20 2020 2020 2020  ).where(.       
+00010b30: 2020 2020 2074 6162 6c65 2e63 2e78 203d       table.c.x =
+00010b40: 3d20 7371 6c61 6c63 6865 6d79 2e62 696e  = sqlalchemy.bin
+00010b50: 6470 6172 616d 2822 7122 2c20 6c69 7465  dparam("q", lite
+00010b60: 7261 6c5f 6578 6563 7574 653d 5472 7565  ral_execute=True
+00010b70: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
+00010b80: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+00010b90: 716c 5f65 7865 6375 7469 6f6e 5f61 7373  ql_execution_ass
+00010ba0: 6572 7465 7228 2920 6173 2061 7373 6572  erter() as asser
+00010bb0: 7465 723a 0a20 2020 2020 2020 2020 2020  ter:.           
+00010bc0: 2077 6974 6820 636f 6e66 6967 2e64 622e   with config.db.
+00010bd0: 636f 6e6e 6563 7428 2920 6173 2063 6f6e  connect() as con
+00010be0: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
+00010bf0: 2020 2063 6f6e 6e2e 6578 6563 7574 6528     conn.execute(
+00010c00: 7374 6d74 2c20 6469 6374 2871 3d31 3029  stmt, dict(q=10)
+00010c10: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00010c20: 7465 722e 6173 7365 7274 5f28 0a20 2020  ter.assert_(.   
+00010c30: 2020 2020 2020 2020 2073 716c 616c 6368           sqlalch
+00010c40: 656d 792e 7465 7374 696e 672e 6173 7365  emy.testing.asse
+00010c50: 7274 7371 6c2e 4375 7273 6f72 5351 4c28  rtsql.CursorSQL(
+00010c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010c70: 2022 5345 4c45 4354 2073 6f6d 655f 7461   "SELECT some_ta
+00010c80: 626c 652e 6964 205c 6e46 524f 4d20 736f  ble.id \nFROM so
+00010c90: 6d65 5f74 6162 6c65 2022 2022 5c6e 5748  me_table " "\nWH
+00010ca0: 4552 4520 736f 6d65 5f74 6162 6c65 2e78  ERE some_table.x
+00010cb0: 203d 2031 3022 2c0a 2020 2020 2020 2020   = 10",.        
+00010cc0: 2020 2020 2020 2020 5b5d 2069 6620 636f          [] if co
+00010cd0: 6e66 6967 2e64 622e 6469 616c 6563 742e  nfig.db.dialect.
+00010ce0: 706f 7369 7469 6f6e 616c 2065 6c73 6520  positional else 
+00010cf0: 7b7d 2c0a 2020 2020 2020 2020 2020 2020  {},.            
+00010d00: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
+00010d10: 2064 6566 2074 6573 745f 6578 6563 7574   def test_execut
+00010d20: 655f 6578 7061 6e64 696e 675f 706c 7573  e_expanding_plus
+00010d30: 5f6c 6974 6572 616c 5f65 7865 6375 7465  _literal_execute
+00010d40: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00010d50: 7461 626c 6520 3d20 7365 6c66 2e74 6162  table = self.tab
+00010d60: 6c65 732e 736f 6d65 5f74 6162 6c65 0a0a  les.some_table..
+00010d70: 2020 2020 2020 2020 7374 6d74 203d 2073          stmt = s
+00010d80: 656c 6563 7428 7461 626c 652e 632e 6964  elect(table.c.id
+00010d90: 292e 7768 6572 6528 0a20 2020 2020 2020  ).where(.       
+00010da0: 2020 2020 2074 6162 6c65 2e63 2e78 2e69       table.c.x.i
+00010db0: 6e5f 280a 2020 2020 2020 2020 2020 2020  n_(.            
+00010dc0: 2020 2020 7371 6c61 6c63 6865 6d79 2e62      sqlalchemy.b
+00010dd0: 696e 6470 6172 616d 2822 7122 2c20 6578  indparam("q", ex
+00010de0: 7061 6e64 696e 673d 5472 7565 2c20 6c69  panding=True, li
+00010df0: 7465 7261 6c5f 6578 6563 7574 653d 5472  teral_execute=Tr
+00010e00: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00010e10: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
+00010e20: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+00010e30: 716c 5f65 7865 6375 7469 6f6e 5f61 7373  ql_execution_ass
+00010e40: 6572 7465 7228 2920 6173 2061 7373 6572  erter() as asser
+00010e50: 7465 723a 0a20 2020 2020 2020 2020 2020  ter:.           
+00010e60: 2077 6974 6820 636f 6e66 6967 2e64 622e   with config.db.
+00010e70: 636f 6e6e 6563 7428 2920 6173 2063 6f6e  connect() as con
+00010e80: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
+00010e90: 2020 2063 6f6e 6e2e 6578 6563 7574 6528     conn.execute(
+00010ea0: 7374 6d74 2c20 6469 6374 2871 3d5b 352c  stmt, dict(q=[5,
+00010eb0: 2036 2c20 375d 2929 0a0a 2020 2020 2020   6, 7]))..      
+00010ec0: 2020 6173 7365 7274 6572 2e61 7373 6572    asserter.asser
+00010ed0: 745f 280a 2020 2020 2020 2020 2020 2020  t_(.            
+00010ee0: 7371 6c61 6c63 6865 6d79 2e74 6573 7469  sqlalchemy.testi
+00010ef0: 6e67 2e61 7373 6572 7473 716c 2e43 7572  ng.assertsql.Cur
+00010f00: 736f 7253 514c 280a 2020 2020 2020 2020  sorSQL(.        
+00010f10: 2020 2020 2020 2020 2253 454c 4543 5420          "SELECT 
+00010f20: 736f 6d65 5f74 6162 6c65 2e69 6420 5c6e  some_table.id \n
+00010f30: 4652 4f4d 2073 6f6d 655f 7461 626c 6520  FROM some_table 
+00010f40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00010f50: 2020 225c 6e57 4845 5245 2073 6f6d 655f    "\nWHERE some_
+00010f60: 7461 626c 652e 7820 494e 2028 352c 2036  table.x IN (5, 6
+00010f70: 2c20 3729 222c 0a20 2020 2020 2020 2020  , 7)",.         
+00010f80: 2020 2020 2020 205b 5d20 6966 2063 6f6e         [] if con
+00010f90: 6669 672e 6462 2e64 6961 6c65 6374 2e70  fig.db.dialect.p
+00010fa0: 6f73 6974 696f 6e61 6c20 656c 7365 207b  ositional else {
+00010fb0: 7d2c 0a20 2020 2020 2020 2020 2020 2029  },.            )
+00010fc0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00010fd0: 4074 6573 7469 6e67 2e72 6571 7569 7265  @testing.require
+00010fe0: 732e 7475 706c 655f 696e 0a20 2020 2064  s.tuple_in.    d
+00010ff0: 6566 2074 6573 745f 6578 6563 7574 655f  ef test_execute_
+00011000: 7475 706c 655f 6578 7061 6e64 696e 675f  tuple_expanding_
+00011010: 706c 7573 5f6c 6974 6572 616c 5f65 7865  plus_literal_exe
+00011020: 6375 7465 2873 656c 6629 3a0a 2020 2020  cute(self):.    
+00011030: 2020 2020 7461 626c 6520 3d20 7365 6c66      table = self
+00011040: 2e74 6162 6c65 732e 736f 6d65 5f74 6162  .tables.some_tab
+00011050: 6c65 0a0a 2020 2020 2020 2020 7374 6d74  le..        stmt
+00011060: 203d 2073 656c 6563 7428 7461 626c 652e   = select(table.
+00011070: 632e 6964 292e 7768 6572 6528 0a20 2020  c.id).where(.   
+00011080: 2020 2020 2020 2020 2073 716c 616c 6368           sqlalch
+00011090: 656d 792e 7475 706c 655f 2874 6162 6c65  emy.tuple_(table
+000110a0: 2e63 2e78 2c20 7461 626c 652e 632e 7929  .c.x, table.c.y)
+000110b0: 2e69 6e5f 280a 2020 2020 2020 2020 2020  .in_(.          
+000110c0: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
+000110d0: 2e62 696e 6470 6172 616d 2822 7122 2c20  .bindparam("q", 
+000110e0: 6578 7061 6e64 696e 673d 5472 7565 2c20  expanding=True, 
+000110f0: 6c69 7465 7261 6c5f 6578 6563 7574 653d  literal_execute=
+00011100: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+00011110: 2020 290a 2020 2020 2020 2020 290a 0a20    ).        ).. 
+00011120: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00011130: 2e73 716c 5f65 7865 6375 7469 6f6e 5f61  .sql_execution_a
+00011140: 7373 6572 7465 7228 2920 6173 2061 7373  sserter() as ass
+00011150: 6572 7465 723a 0a20 2020 2020 2020 2020  erter:.         
+00011160: 2020 2077 6974 6820 636f 6e66 6967 2e64     with config.d
+00011170: 622e 636f 6e6e 6563 7428 2920 6173 2063  b.connect() as c
+00011180: 6f6e 6e3a 0a20 2020 2020 2020 2020 2020  onn:.           
+00011190: 2020 2020 2063 6f6e 6e2e 6578 6563 7574       conn.execut
+000111a0: 6528 7374 6d74 2c20 6469 6374 2871 3d5b  e(stmt, dict(q=[
+000111b0: 2835 2c20 3130 292c 2028 3132 2c20 3138  (5, 10), (12, 18
+000111c0: 295d 2929 0a0a 2020 2020 2020 2020 6173  )]))..        as
+000111d0: 7365 7274 6572 2e61 7373 6572 745f 280a  serter.assert_(.
+000111e0: 2020 2020 2020 2020 2020 2020 7371 6c61              sqla
+000111f0: 6c63 6865 6d79 2e74 6573 7469 6e67 2e61  lchemy.testing.a
+00011200: 7373 6572 7473 716c 2e43 7572 736f 7253  ssertsql.CursorS
+00011210: 514c 280a 2020 2020 2020 2020 2020 2020  QL(.            
+00011220: 2020 2020 2253 454c 4543 5420 736f 6d65      "SELECT some
+00011230: 5f74 6162 6c65 2e69 6420 5c6e 4652 4f4d  _table.id \nFROM
+00011240: 2073 6f6d 655f 7461 626c 6520 220a 2020   some_table ".  
+00011250: 2020 2020 2020 2020 2020 2020 2020 225c                "\
+00011260: 6e57 4845 5245 2028 736f 6d65 5f74 6162  nWHERE (some_tab
+00011270: 6c65 2e78 2c20 736f 6d65 5f74 6162 6c65  le.x, some_table
+00011280: 2e79 2920 220a 2020 2020 2020 2020 2020  .y) ".          
+00011290: 2020 2020 2020 2249 4e20 2825 7328 352c        "IN (%s(5,
+000112a0: 2031 3029 2c20 2831 322c 2031 3829 2922   10), (12, 18))"
+000112b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000112c0: 2025 2028 2256 414c 5545 5320 2220 6966   % ("VALUES " if
+000112d0: 2063 6f6e 6669 672e 6462 2e64 6961 6c65   config.db.diale
+000112e0: 6374 2e74 7570 6c65 5f69 6e5f 7661 6c75  ct.tuple_in_valu
+000112f0: 6573 2065 6c73 6520 2222 292c 0a20 2020  es else ""),.   
+00011300: 2020 2020 2020 2020 2020 2020 2028 2920               () 
+00011310: 6966 2063 6f6e 6669 672e 6462 2e64 6961  if config.db.dia
+00011320: 6c65 6374 2e70 6f73 6974 696f 6e61 6c20  lect.positional 
+00011330: 656c 7365 207b 7d2c 0a20 2020 2020 2020  else {},.       
+00011340: 2020 2020 2029 0a20 2020 2020 2020 2029       ).        )
+00011350: 0a0a 2020 2020 4074 6573 7469 6e67 2e72  ..    @testing.r
+00011360: 6571 7569 7265 732e 7475 706c 655f 696e  equires.tuple_in
+00011370: 0a20 2020 2064 6566 2074 6573 745f 6578  .    def test_ex
+00011380: 6563 7574 655f 7475 706c 655f 6578 7061  ecute_tuple_expa
+00011390: 6e64 696e 675f 706c 7573 5f6c 6974 6572  nding_plus_liter
+000113a0: 616c 5f68 6574 6572 6f67 656e 656f 7573  al_heterogeneous
+000113b0: 5f65 7865 6375 7465 2873 656c 6629 3a0a  _execute(self):.
+000113c0: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
+000113d0: 7365 6c66 2e74 6162 6c65 732e 736f 6d65  self.tables.some
+000113e0: 5f74 6162 6c65 0a0a 2020 2020 2020 2020  _table..        
+000113f0: 7374 6d74 203d 2073 656c 6563 7428 7461  stmt = select(ta
+00011400: 626c 652e 632e 6964 292e 7768 6572 6528  ble.c.id).where(
+00011410: 0a20 2020 2020 2020 2020 2020 2073 716c  .            sql
+00011420: 616c 6368 656d 792e 7475 706c 655f 2874  alchemy.tuple_(t
+00011430: 6162 6c65 2e63 2e78 2c20 7461 626c 652e  able.c.x, table.
+00011440: 632e 7a29 2e69 6e5f 280a 2020 2020 2020  c.z).in_(.      
+00011450: 2020 2020 2020 2020 2020 7371 6c61 6c63            sqlalc
+00011460: 6865 6d79 2e62 696e 6470 6172 616d 2822  hemy.bindparam("
+00011470: 7122 2c20 6578 7061 6e64 696e 673d 5472  q", expanding=Tr
+00011480: 7565 2c20 6c69 7465 7261 6c5f 6578 6563  ue, literal_exec
+00011490: 7574 653d 5472 7565 290a 2020 2020 2020  ute=True).      
+000114a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000114b0: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+000114c0: 7365 6c66 2e73 716c 5f65 7865 6375 7469  self.sql_executi
+000114d0: 6f6e 5f61 7373 6572 7465 7228 2920 6173  on_asserter() as
+000114e0: 2061 7373 6572 7465 723a 0a20 2020 2020   asserter:.     
+000114f0: 2020 2020 2020 2077 6974 6820 636f 6e66         with conf
+00011500: 6967 2e64 622e 636f 6e6e 6563 7428 2920  ig.db.connect() 
+00011510: 6173 2063 6f6e 6e3a 0a20 2020 2020 2020  as conn:.       
+00011520: 2020 2020 2020 2020 2063 6f6e 6e2e 6578           conn.ex
+00011530: 6563 7574 6528 7374 6d74 2c20 6469 6374  ecute(stmt, dict
+00011540: 2871 3d5b 2835 2c20 227a 3122 292c 2028  (q=[(5, "z1"), (
+00011550: 3132 2c20 227a 3322 295d 2929 0a0a 2020  12, "z3")]))..  
+00011560: 2020 2020 2020 6173 7365 7274 6572 2e61        asserter.a
+00011570: 7373 6572 745f 280a 2020 2020 2020 2020  ssert_(.        
+00011580: 2020 2020 7371 6c61 6c63 6865 6d79 2e74      sqlalchemy.t
+00011590: 6573 7469 6e67 2e61 7373 6572 7473 716c  esting.assertsql
+000115a0: 2e43 7572 736f 7253 514c 280a 2020 2020  .CursorSQL(.    
+000115b0: 2020 2020 2020 2020 2020 2020 2253 454c              "SEL
+000115c0: 4543 5420 736f 6d65 5f74 6162 6c65 2e69  ECT some_table.i
+000115d0: 6420 5c6e 4652 4f4d 2073 6f6d 655f 7461  d \nFROM some_ta
+000115e0: 626c 6520 220a 2020 2020 2020 2020 2020  ble ".          
+000115f0: 2020 2020 2020 225c 6e57 4845 5245 2028        "\nWHERE (
+00011600: 736f 6d65 5f74 6162 6c65 2e78 2c20 736f  some_table.x, so
+00011610: 6d65 5f74 6162 6c65 2e7a 2920 220a 2020  me_table.z) ".  
+00011620: 2020 2020 2020 2020 2020 2020 2020 2249                "I
+00011630: 4e20 2825 7328 352c 2027 7a31 2729 2c20  N (%s(5, 'z1'), 
+00011640: 2831 322c 2027 7a33 2729 2922 0a20 2020  (12, 'z3'))".   
+00011650: 2020 2020 2020 2020 2020 2020 2025 2028               % (
+00011660: 2256 414c 5545 5320 2220 6966 2063 6f6e  "VALUES " if con
+00011670: 6669 672e 6462 2e64 6961 6c65 6374 2e74  fig.db.dialect.t
+00011680: 7570 6c65 5f69 6e5f 7661 6c75 6573 2065  uple_in_values e
+00011690: 6c73 6520 2222 292c 0a20 2020 2020 2020  lse ""),.       
+000116a0: 2020 2020 2020 2020 2028 2920 6966 2063           () if c
+000116b0: 6f6e 6669 672e 6462 2e64 6961 6c65 6374  onfig.db.dialect
+000116c0: 2e70 6f73 6974 696f 6e61 6c20 656c 7365  .positional else
+000116d0: 207b 7d2c 0a20 2020 2020 2020 2020 2020   {},.           
+000116e0: 2029 0a20 2020 2020 2020 2029 0a0a 0a63   ).        )...c
+000116f0: 6c61 7373 2043 6f6d 7075 7465 6452 6566  lass ComputedRef
+00011700: 6c65 6374 696f 6e46 6978 7475 7265 5465  lectionFixtureTe
+00011710: 7374 285f 436f 6d70 7574 6564 5265 666c  st(_ComputedRefl
+00011720: 6563 7469 6f6e 4669 7874 7572 6554 6573  ectionFixtureTes
+00011730: 7429 3a0a 2020 2020 4063 6c61 7373 6d65  t):.    @classme
+00011740: 7468 6f64 0a20 2020 2064 6566 2064 6566  thod.    def def
+00011750: 696e 655f 7461 626c 6573 2863 6c73 2c20  ine_tables(cls, 
+00011760: 6d65 7461 6461 7461 293a 0a20 2020 2020  metadata):.     
+00011770: 2020 2022 2222 5350 414e 4e45 5220 4f56     """SPANNER OV
+00011780: 4552 5249 4445 3a0a 0a20 2020 2020 2020  ERRIDE:..       
+00011790: 2041 766f 6964 2075 7369 6e67 2064 6566   Avoid using def
+000117a0: 6175 6c74 2076 616c 7565 7320 666f 7220  ault values for 
+000117b0: 636f 6d70 7574 6564 2063 6f6c 756d 6e73  computed columns
+000117c0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000117d0: 2020 2020 2020 5461 626c 6528 0a20 2020        Table(.   
+000117e0: 2020 2020 2020 2020 2022 636f 6d70 7574           "comput
+000117f0: 6564 5f64 6566 6175 6c74 5f74 6162 6c65  ed_default_table
+00011800: 222c 0a20 2020 2020 2020 2020 2020 206d  ",.            m
+00011810: 6574 6164 6174 612c 0a20 2020 2020 2020  etadata,.       
+00011820: 2020 2020 2043 6f6c 756d 6e28 2269 6422       Column("id"
+00011830: 2c20 496e 7465 6765 722c 2070 7269 6d61  , Integer, prima
+00011840: 7279 5f6b 6579 3d54 7275 6529 2c0a 2020  ry_key=True),.  
+00011850: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
+00011860: 2822 6e6f 726d 616c 222c 2049 6e74 6567  ("normal", Integ
+00011870: 6572 292c 0a20 2020 2020 2020 2020 2020  er),.           
+00011880: 2043 6f6c 756d 6e28 2263 6f6d 7075 7465   Column("compute
+00011890: 645f 636f 6c22 2c20 496e 7465 6765 722c  d_col", Integer,
+000118a0: 2043 6f6d 7075 7465 6428 226e 6f72 6d61   Computed("norma
+000118b0: 6c20 2b20 3432 2229 292c 0a20 2020 2020  l + 42")),.     
+000118c0: 2020 2020 2020 2043 6f6c 756d 6e28 2277         Column("w
+000118d0: 6974 685f 6465 6661 756c 7422 2c20 496e  ith_default", In
+000118e0: 7465 6765 7229 2c0a 2020 2020 2020 2020  teger),.        
+000118f0: 290a 0a20 2020 2020 2020 2074 203d 2054  )..        t = T
+00011900: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
+00011910: 2020 2263 6f6d 7075 7465 645f 636f 6c75    "computed_colu
+00011920: 6d6e 5f74 6162 6c65 222c 0a20 2020 2020  mn_table",.     
+00011930: 2020 2020 2020 206d 6574 6164 6174 612c         metadata,
+00011940: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
+00011950: 756d 6e28 2269 6422 2c20 496e 7465 6765  umn("id", Intege
+00011960: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
+00011970: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
+00011980: 2020 436f 6c75 6d6e 2822 6e6f 726d 616c    Column("normal
+00011990: 222c 2049 6e74 6567 6572 292c 0a20 2020  ", Integer),.   
+000119a0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+000119b0: 2263 6f6d 7075 7465 645f 6e6f 5f66 6c61  "computed_no_fla
+000119c0: 6722 2c20 496e 7465 6765 722c 2043 6f6d  g", Integer, Com
+000119d0: 7075 7465 6428 226e 6f72 6d61 6c20 2b20  puted("normal + 
+000119e0: 3432 2229 292c 0a20 2020 2020 2020 2029  42")),.        )
+000119f0: 0a0a 2020 2020 2020 2020 6966 2074 6573  ..        if tes
+00011a00: 7469 6e67 2e72 6571 7569 7265 732e 636f  ting.requires.co
+00011a10: 6d70 7574 6564 5f63 6f6c 756d 6e73 5f76  mputed_columns_v
+00011a20: 6972 7475 616c 2e65 6e61 626c 6564 3a0a  irtual.enabled:.
+00011a30: 2020 2020 2020 2020 2020 2020 742e 6170              t.ap
+00011a40: 7065 6e64 5f63 6f6c 756d 6e28 0a20 2020  pend_column(.   
+00011a50: 2020 2020 2020 2020 2020 2020 2043 6f6c               Col
+00011a60: 756d 6e28 0a20 2020 2020 2020 2020 2020  umn(.           
+00011a70: 2020 2020 2020 2020 2022 636f 6d70 7574           "comput
+00011a80: 6564 5f76 6972 7475 616c 222c 0a20 2020  ed_virtual",.   
+00011a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011aa0: 2049 6e74 6567 6572 2c0a 2020 2020 2020   Integer,.      
+00011ab0: 2020 2020 2020 2020 2020 2020 2020 436f                Co
+00011ac0: 6d70 7574 6564 2822 6e6f 726d 616c 202b  mputed("normal +
+00011ad0: 2032 222c 2070 6572 7369 7374 6564 3d46   2", persisted=F
+00011ae0: 616c 7365 292c 0a20 2020 2020 2020 2020  alse),.         
+00011af0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00011b00: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+00011b10: 6620 7465 7374 696e 672e 7265 7175 6972  f testing.requir
+00011b20: 6573 2e63 6f6d 7075 7465 645f 636f 6c75  es.computed_colu
+00011b30: 6d6e 735f 7374 6f72 6564 2e65 6e61 626c  mns_stored.enabl
+00011b40: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+00011b50: 742e 6170 7065 6e64 5f63 6f6c 756d 6e28  t.append_column(
+00011b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011b70: 2043 6f6c 756d 6e28 0a20 2020 2020 2020   Column(.       
+00011b80: 2020 2020 2020 2020 2020 2020 2022 636f               "co
+00011b90: 6d70 7574 6564 5f73 746f 7265 6422 2c0a  mputed_stored",.
+00011ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bb0: 2020 2020 496e 7465 6765 722c 0a20 2020      Integer,.   
+00011bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bd0: 2043 6f6d 7075 7465 6428 226e 6f72 6d61   Computed("norma
+00011be0: 6c20 2d20 3432 222c 2070 6572 7369 7374  l - 42", persist
+00011bf0: 6564 3d54 7275 6529 2c0a 2020 2020 2020  ed=True),.      
+00011c00: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00011c10: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
+00011c20: 7320 436f 6d70 7574 6564 5265 666c 6563  s ComputedReflec
+00011c30: 7469 6f6e 5465 7374 285f 436f 6d70 7574  tionTest(_Comput
+00011c40: 6564 5265 666c 6563 7469 6f6e 5465 7374  edReflectionTest
+00011c50: 2c20 436f 6d70 7574 6564 5265 666c 6563  , ComputedReflec
+00011c60: 7469 6f6e 4669 7874 7572 6554 6573 7429  tionFixtureTest)
+00011c70: 3a0a 2020 2020 4074 6573 7469 6e67 2e72  :.    @testing.r
+00011c80: 6571 7569 7265 732e 7363 6865 6d61 730a  equires.schemas.
+00011c90: 2020 2020 6465 6620 7465 7374 5f67 6574      def test_get
+00011ca0: 5f63 6f6c 756d 6e5f 7265 7475 726e 735f  _column_returns_
+00011cb0: 7065 7273 6973 7465 645f 7769 7468 5f73  persisted_with_s
+00011cc0: 6368 656d 6128 7365 6c66 293a 0a20 2020  chema(self):.   
+00011cd0: 2020 2020 2069 6e73 7020 3d20 696e 7370       insp = insp
+00011ce0: 6563 7428 636f 6e66 6967 2e64 6229 0a0a  ect(config.db)..
+00011cf0: 2020 2020 2020 2020 636f 6c73 203d 2069          cols = i
+00011d00: 6e73 702e 6765 745f 636f 6c75 6d6e 7328  nsp.get_columns(
+00011d10: 2263 6f6d 7075 7465 645f 636f 6c75 6d6e  "computed_column
+00011d20: 5f74 6162 6c65 222c 2073 6368 656d 613d  _table", schema=
+00011d30: 636f 6e66 6967 2e74 6573 745f 7363 6865  config.test_sche
+00011d40: 6d61 290a 2020 2020 2020 2020 6461 7461  ma).        data
+00011d50: 203d 207b 635b 226e 616d 6522 5d3a 2063   = {c["name"]: c
+00011d60: 2066 6f72 2063 2069 6e20 636f 6c73 7d0a   for c in cols}.
+00011d70: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
+00011d80: 6563 6b5f 636f 6c75 6d6e 280a 2020 2020  eck_column(.    
+00011d90: 2020 2020 2020 2020 6461 7461 2c0a 2020          data,.  
+00011da0: 2020 2020 2020 2020 2020 2263 6f6d 7075            "compu
+00011db0: 7465 645f 6e6f 5f66 6c61 6722 2c0a 2020  ted_no_flag",.  
+00011dc0: 2020 2020 2020 2020 2020 226e 6f72 6d61            "norma
+00011dd0: 6c2b 3432 222c 0a20 2020 2020 2020 2020  l+42",.         
+00011de0: 2020 2074 6573 7469 6e67 2e72 6571 7569     testing.requi
+00011df0: 7265 732e 636f 6d70 7574 6564 5f63 6f6c  res.computed_col
+00011e00: 756d 6e73 5f64 6566 6175 6c74 5f70 6572  umns_default_per
+00011e10: 7369 7374 6564 2e65 6e61 626c 6564 2c0a  sisted.enabled,.
+00011e20: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00011e30: 2020 6966 2074 6573 7469 6e67 2e72 6571    if testing.req
+00011e40: 7569 7265 732e 636f 6d70 7574 6564 5f63  uires.computed_c
+00011e50: 6f6c 756d 6e73 5f76 6972 7475 616c 2e65  olumns_virtual.e
+00011e60: 6e61 626c 6564 3a0a 2020 2020 2020 2020  nabled:.        
+00011e70: 2020 2020 7365 6c66 2e63 6865 636b 5f63      self.check_c
+00011e80: 6f6c 756d 6e28 0a20 2020 2020 2020 2020  olumn(.         
+00011e90: 2020 2020 2020 2064 6174 612c 0a20 2020         data,.   
+00011ea0: 2020 2020 2020 2020 2020 2020 2022 636f               "co
+00011eb0: 6d70 7574 6564 5f76 6972 7475 616c 222c  mputed_virtual",
+00011ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011ed0: 2022 6e6f 726d 616c 2f32 222c 0a20 2020   "normal/2",.   
+00011ee0: 2020 2020 2020 2020 2020 2020 2046 616c               Fal
+00011ef0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00011f00: 290a 2020 2020 2020 2020 6966 2074 6573  ).        if tes
+00011f10: 7469 6e67 2e72 6571 7569 7265 732e 636f  ting.requires.co
+00011f20: 6d70 7574 6564 5f63 6f6c 756d 6e73 5f73  mputed_columns_s
+00011f30: 746f 7265 642e 656e 6162 6c65 643a 0a20  tored.enabled:. 
+00011f40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011f50: 6368 6563 6b5f 636f 6c75 6d6e 280a 2020  check_column(.  
+00011f60: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00011f70: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+00011f80: 2020 2020 2263 6f6d 7075 7465 645f 7374      "computed_st
+00011f90: 6f72 6564 222c 0a20 2020 2020 2020 2020  ored",.         
+00011fa0: 2020 2020 2020 2022 6e6f 726d 616c 2d34         "normal-4
+00011fb0: 3222 2c0a 2020 2020 2020 2020 2020 2020  2",.            
+00011fc0: 2020 2020 5472 7565 2c0a 2020 2020 2020      True,.      
+00011fd0: 2020 2020 2020 290a 0a20 2020 2040 7079        )..    @py
+00011fe0: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
+00011ff0: 4465 6661 756c 7420 7661 6c75 6573 2061  Default values a
+00012000: 7265 206e 6f74 2073 7570 706f 7274 6564  re not supported
+00012010: 2e22 290a 2020 2020 6465 6620 7465 7374  .").    def test
+00012020: 5f63 6f6d 7075 7465 645f 636f 6c5f 6465  _computed_col_de
+00012030: 6661 756c 745f 6e6f 745f 7365 7428 7365  fault_not_set(se
+00012040: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+00012050: 730a 0a20 2020 2064 6566 2074 6573 745f  s..    def test_
+00012060: 6765 745f 636f 6c75 6d6e 5f72 6574 7572  get_column_retur
+00012070: 6e73 5f63 6f6d 7075 7465 6428 7365 6c66  ns_computed(self
+00012080: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00012090: 2020 2020 2020 2053 5041 4e4e 4552 204f         SPANNER O
+000120a0: 5645 5252 4944 453a 0a0a 2020 2020 2020  VERRIDE:..      
+000120b0: 2020 496e 2053 7061 6e6e 6572 2061 6c6c    In Spanner all
+000120c0: 2074 6865 2067 656e 6572 6174 6564 2063   the generated c
+000120d0: 6f6c 756d 6e73 2061 7265 2053 544f 5245  olumns are STORE
+000120e0: 442c 0a20 2020 2020 2020 206d 6561 6e69  D,.        meani
+000120f0: 6e67 2074 6865 7265 2061 7265 206e 6f20  ng there are no 
+00012100: 7065 7273 6973 7465 6420 616e 6420 6e6f  persisted and no
+00012110: 7420 7065 7273 6973 7465 640a 2020 2020  t persisted.    
+00012120: 2020 2020 2869 6e20 7468 6520 7465 726d      (in the term
+00012130: 7320 6f66 2074 6865 2053 514c 416c 6368  s of the SQLAlch
+00012140: 656d 7929 2063 6f6c 756d 6e73 2e20 5468  emy) columns. Th
+00012150: 650a 2020 2020 2020 2020 6d65 7468 6f64  e.        method
+00012160: 206f 7665 7272 6964 6520 6f6d 6974 7320   override omits 
+00012170: 7468 6520 7065 7273 6973 7465 6e63 6520  the persistence 
+00012180: 7265 666c 6563 7469 6f6e 2063 6865 636b  reflection check
+00012190: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+000121a0: 2020 2020 2020 2069 6e73 7020 3d20 696e         insp = in
+000121b0: 7370 6563 7428 636f 6e66 6967 2e64 6229  spect(config.db)
+000121c0: 0a0a 2020 2020 2020 2020 636f 6c73 203d  ..        cols =
+000121d0: 2069 6e73 702e 6765 745f 636f 6c75 6d6e   insp.get_column
+000121e0: 7328 2263 6f6d 7075 7465 645f 6465 6661  s("computed_defa
+000121f0: 756c 745f 7461 626c 6522 290a 2020 2020  ult_table").    
+00012200: 2020 2020 6461 7461 203d 207b 635b 226e      data = {c["n
+00012210: 616d 6522 5d3a 2063 2066 6f72 2063 2069  ame"]: c for c i
+00012220: 6e20 636f 6c73 7d0a 2020 2020 2020 2020  n cols}.        
+00012230: 666f 7220 6b65 7920 696e 2028 2269 6422  for key in ("id"
+00012240: 2c20 226e 6f72 6d61 6c22 2c20 2277 6974  , "normal", "wit
+00012250: 685f 6465 6661 756c 7422 293a 0a20 2020  h_default"):.   
+00012260: 2020 2020 2020 2020 2069 735f 7472 7565           is_true
+00012270: 2822 636f 6d70 7574 6564 2220 6e6f 7420  ("computed" not 
+00012280: 696e 2064 6174 615b 6b65 795d 290a 2020  in data[key]).  
+00012290: 2020 2020 2020 636f 6d70 4461 7461 203d        compData =
+000122a0: 2064 6174 615b 2263 6f6d 7075 7465 645f   data["computed_
+000122b0: 636f 6c22 5d0a 2020 2020 2020 2020 6973  col"].        is
+000122c0: 5f74 7275 6528 2263 6f6d 7075 7465 6422  _true("computed"
+000122d0: 2069 6e20 636f 6d70 4461 7461 290a 2020   in compData).  
+000122e0: 2020 2020 2020 6973 5f74 7275 6528 2273        is_true("s
+000122f0: 716c 7465 7874 2220 696e 2063 6f6d 7044  qltext" in compD
+00012300: 6174 615b 2263 6f6d 7075 7465 6422 5d29  ata["computed"])
+00012310: 0a20 2020 2020 2020 2065 715f 2873 656c  .        eq_(sel
+00012320: 662e 6e6f 726d 616c 697a 6528 636f 6d70  f.normalize(comp
+00012330: 4461 7461 5b22 636f 6d70 7574 6564 225d  Data["computed"]
+00012340: 5b22 7371 6c74 6578 7422 5d29 2c20 226e  ["sqltext"]), "n
+00012350: 6f72 6d61 6c2b 3432 2229 0a0a 2020 2020  ormal+42")..    
+00012360: 6465 6620 7465 7374 5f63 7265 6174 655f  def test_create_
+00012370: 6e6f 745f 6e75 6c6c 5f63 6f6d 7075 7465  not_null_compute
+00012380: 645f 636f 6c75 6d6e 2873 656c 6629 3a0a  d_column(self):.
+00012390: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000123a0: 2020 2020 5350 414e 4e45 5220 5445 5354      SPANNER TEST
+000123b0: 3a0a 0a20 2020 2020 2020 2043 6865 636b  :..        Check
+000123c0: 2074 6861 7420 6f6e 2063 7265 6174 696e   that on creatin
+000123d0: 6720 6120 636f 6d70 7574 6564 2063 6f6c  g a computed col
+000123e0: 756d 6e20 7769 7468 2061 204e 4f54 204e  umn with a NOT N
+000123f0: 554c 4c0a 2020 2020 2020 2020 636c 6175  ULL.        clau
+00012400: 7365 2074 6865 2063 6c61 7573 6520 6973  se the clause is
+00012410: 2073 6574 2069 6e20 6672 6f6e 7420 6f66   set in front of
+00012420: 2074 6865 2063 6f6d 7075 7465 6420 636f   the computed co
+00012430: 6c75 6d6e 0a20 2020 2020 2020 2073 7461  lumn.        sta
+00012440: 7465 6d65 6e74 2064 6566 696e 6974 696f  tement definitio
+00012450: 6e20 616e 6420 646f 6573 6e27 7420 6361  n and doesn't ca
+00012460: 7573 6520 6661 696c 7572 6573 2e0a 2020  use failures..  
+00012470: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012480: 2020 656e 6769 6e65 203d 2063 7265 6174    engine = creat
+00012490: 655f 656e 6769 6e65 2867 6574 5f64 625f  e_engine(get_db_
+000124a0: 7572 6c28 2929 0a20 2020 2020 2020 206d  url()).        m
+000124b0: 6574 6164 6174 6120 3d20 4d65 7461 4461  etadata = MetaDa
+000124c0: 7461 2862 696e 643d 656e 6769 6e65 290a  ta(bind=engine).
+000124d0: 0a20 2020 2020 2020 2054 6162 6c65 280a  .        Table(.
+000124e0: 2020 2020 2020 2020 2020 2020 2253 696e              "Sin
+000124f0: 6765 7273 222c 0a20 2020 2020 2020 2020  gers",.         
+00012500: 2020 206d 6574 6164 6174 612c 0a20 2020     metadata,.   
+00012510: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00012520: 2253 696e 6765 7249 6422 2c20 5374 7269  "SingerId", Stri
+00012530: 6e67 2833 3629 2c20 7072 696d 6172 795f  ng(36), primary_
+00012540: 6b65 793d 5472 7565 2c20 6e75 6c6c 6162  key=True, nullab
+00012550: 6c65 3d46 616c 7365 292c 0a20 2020 2020  le=False),.     
+00012560: 2020 2020 2020 2043 6f6c 756d 6e28 2246         Column("F
+00012570: 6972 7374 4e61 6d65 222c 2053 7472 696e  irstName", Strin
+00012580: 6728 3230 3029 292c 0a20 2020 2020 2020  g(200)),.       
+00012590: 2020 2020 2043 6f6c 756d 6e28 224c 6173       Column("Las
+000125a0: 744e 616d 6522 2c20 5374 7269 6e67 2832  tName", String(2
+000125b0: 3030 292c 206e 756c 6c61 626c 653d 4661  00), nullable=Fa
+000125c0: 6c73 6529 2c0a 2020 2020 2020 2020 2020  lse),.          
+000125d0: 2020 436f 6c75 6d6e 280a 2020 2020 2020    Column(.      
+000125e0: 2020 2020 2020 2020 2020 2246 756c 6c4e            "FullN
+000125f0: 616d 6522 2c0a 2020 2020 2020 2020 2020  ame",.          
+00012600: 2020 2020 2020 5374 7269 6e67 2834 3030        String(400
+00012610: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00012620: 2020 2043 6f6d 7075 7465 6428 2243 4f41     Computed("COA
+00012630: 4c45 5343 4528 4669 7273 744e 616d 6520  LESCE(FirstName 
+00012640: 7c7c 2027 2027 2c20 2727 2920 7c7c 204c  || ' ', '') || L
+00012650: 6173 744e 616d 6522 292c 0a20 2020 2020  astName"),.     
+00012660: 2020 2020 2020 2020 2020 206e 756c 6c61             nulla
+00012670: 626c 653d 4661 6c73 652c 0a20 2020 2020  ble=False,.     
+00012680: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00012690: 2020 290a 0a20 2020 2020 2020 206d 6574    )..        met
+000126a0: 6164 6174 612e 6372 6561 7465 5f61 6c6c  adata.create_all
+000126b0: 2865 6e67 696e 6529 0a0a 0a40 7079 7465  (engine)...@pyte
+000126c0: 7374 2e6d 6172 6b2e 736b 6970 6966 280a  st.mark.skipif(.
+000126d0: 2020 2020 626f 6f6c 286f 732e 656e 7669      bool(os.envi
+000126e0: 726f 6e2e 6765 7428 2253 5041 4e4e 4552  ron.get("SPANNER
+000126f0: 5f45 4d55 4c41 544f 525f 484f 5354 2229  _EMULATOR_HOST")
+00012700: 292c 2072 6561 736f 6e3d 2253 6b69 7070  ), reason="Skipp
+00012710: 6564 206f 6e20 656d 756c 6174 6f72 220a  ed on emulator".
+00012720: 290a 636c 6173 7320 4a53 4f4e 5465 7374  ).class JSONTest
+00012730: 285f 4a53 4f4e 5465 7374 293a 0a20 2020  (_JSONTest):.   
+00012740: 2040 7079 7465 7374 2e6d 6172 6b2e 736b   @pytest.mark.sk
+00012750: 6970 2822 5661 6c75 6573 2077 6974 686f  ip("Values witho
+00012760: 7574 206b 6579 7320 6172 6520 6e6f 7420  ut keys are not 
+00012770: 7375 7070 6f72 7465 642e 2229 0a20 2020  supported.").   
+00012780: 2064 6566 2074 6573 745f 7369 6e67 6c65   def test_single
+00012790: 5f65 6c65 6d65 6e74 5f72 6f75 6e64 5f74  _element_round_t
+000127a0: 7269 7028 7365 6c66 2c20 656c 656d 656e  rip(self, elemen
+000127b0: 7429 3a0a 2020 2020 2020 2020 7061 7373  t):.        pass
+000127c0: 0a0a 2020 2020 6465 6620 5f74 6573 745f  ..    def _test_
+000127d0: 726f 756e 645f 7472 6970 2873 656c 662c  round_trip(self,
+000127e0: 2064 6174 615f 656c 656d 656e 742c 2063   data_element, c
+000127f0: 6f6e 6e65 6374 696f 6e29 3a0a 2020 2020  onnection):.    
+00012800: 2020 2020 6461 7461 5f74 6162 6c65 203d      data_table =
+00012810: 2073 656c 662e 7461 626c 6573 2e64 6174   self.tables.dat
+00012820: 615f 7461 626c 650a 0a20 2020 2020 2020  a_table..       
+00012830: 2063 6f6e 6669 672e 6462 2e65 7865 6375   config.db.execu
+00012840: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
+00012850: 6461 7461 5f74 6162 6c65 2e69 6e73 6572  data_table.inser
+00012860: 7428 292c 0a20 2020 2020 2020 2020 2020  t(),.           
+00012870: 207b 2269 6422 3a20 7261 6e64 6f6d 2e72   {"id": random.r
+00012880: 616e 6469 6e74 2831 2c20 3130 3030 3030  andint(1, 100000
+00012890: 3030 3029 2c20 226e 616d 6522 3a20 2272  000), "name": "r
+000128a0: 6f77 3122 2c20 2264 6174 6122 3a20 6461  ow1", "data": da
+000128b0: 7461 5f65 6c65 6d65 6e74 7d2c 0a20 2020  ta_element},.   
+000128c0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+000128d0: 726f 7720 3d20 636f 6e66 6967 2e64 622e  row = config.db.
+000128e0: 6578 6563 7574 6528 7365 6c65 6374 285b  execute(select([
+000128f0: 6461 7461 5f74 6162 6c65 2e63 2e64 6174  data_table.c.dat
+00012900: 615d 2929 2e66 6972 7374 2829 0a0a 2020  a])).first()..  
+00012910: 2020 2020 2020 6571 5f28 726f 772c 2028        eq_(row, (
+00012920: 6461 7461 5f65 6c65 6d65 6e74 2c29 290a  data_element,)).
+00012930: 0a20 2020 2064 6566 2074 6573 745f 756e  .    def test_un
+00012940: 6963 6f64 655f 726f 756e 645f 7472 6970  icode_round_trip
+00012950: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00012960: 2320 6e6f 7465 2077 6520 696e 636c 7564  # note we includ
+00012970: 6520 556e 6963 6f64 6520 7375 7070 6c65  e Unicode supple
+00012980: 6d65 6e74 6172 7920 6368 6172 6163 7465  mentary characte
+00012990: 7273 2061 7320 7765 6c6c 0a20 2020 2020  rs as well.     
+000129a0: 2020 2077 6974 6820 636f 6e66 6967 2e64     with config.d
+000129b0: 622e 636f 6e6e 6563 7428 2920 6173 2063  b.connect() as c
+000129c0: 6f6e 6e3a 0a20 2020 2020 2020 2020 2020  onn:.           
+000129d0: 2063 6f6e 6e2e 6578 6563 7574 6528 0a20   conn.execute(. 
+000129e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000129f0: 656c 662e 7461 626c 6573 2e64 6174 615f  elf.tables.data_
+00012a00: 7461 626c 652e 696e 7365 7274 2829 2c0a  table.insert(),.
+00012a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a20: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00012a30: 2020 2020 2020 2269 6422 3a20 7261 6e64        "id": rand
+00012a40: 6f6d 2e72 616e 6469 6e74 2831 2c20 3130  om.randint(1, 10
+00012a50: 3030 3030 3030 3029 2c0a 2020 2020 2020  0000000),.      
+00012a60: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00012a70: 616d 6522 3a20 2272 3122 2c0a 2020 2020  ame": "r1",.    
+00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a90: 2264 6174 6122 3a20 7b0a 2020 2020 2020  "data": {.      
+00012aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ab0: 2020 7574 696c 2e75 2822 72c3 a976 65f0    util.u("r..ve.
+00012ac0: 9f90 8d20 696c 6cc3 a922 293a 2075 7469  ... ill.."): uti
+00012ad0: 6c2e 7528 2272 c3a9 7665 f09f 908d 2069  l.u("r..ve.... i
+00012ae0: 6c6c c3a9 2229 2c0a 2020 2020 2020 2020  ll.."),.        
+00012af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b00: 2264 6174 6122 3a20 7b22 6b31 223a 2075  "data": {"k1": u
+00012b10: 7469 6c2e 7528 2264 72c3 b46c f09f 908d  til.u("dr..l....
+00012b20: 6522 297d 2c0a 2020 2020 2020 2020 2020  e")},.          
+00012b30: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00012b40: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00012b50: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00012b60: 2020 2020 2020 2020 2020 2065 715f 280a             eq_(.
+00012b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b80: 636f 6e6e 2e73 6361 6c61 7228 7365 6c65  conn.scalar(sele
+00012b90: 6374 285b 7365 6c66 2e74 6162 6c65 732e  ct([self.tables.
+00012ba0: 6461 7461 5f74 6162 6c65 2e63 2e64 6174  data_table.c.dat
+00012bb0: 615d 2929 2c0a 2020 2020 2020 2020 2020  a])),.          
+00012bc0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00012bd0: 2020 2020 2020 2020 2020 2020 7574 696c              util
+00012be0: 2e75 2822 72c3 a976 65f0 9f90 8d20 696c  .u("r..ve.... il
+00012bf0: 6cc3 a922 293a 2075 7469 6c2e 7528 2272  l.."): util.u("r
+00012c00: c3a9 7665 f09f 908d 2069 6c6c c3a9 2229  ..ve.... ill..")
+00012c10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012c20: 2020 2020 2020 2264 6174 6122 3a20 7b22        "data": {"
+00012c30: 6b31 223a 2075 7469 6c2e 7528 2264 72c3  k1": util.u("dr.
+00012c40: b46c f09f 908d 6522 297d 2c0a 2020 2020  .l....e")},.    
+00012c50: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00012c60: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00012c70: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+00012c80: 6b69 7028 2250 6172 616d 6574 6572 697a  kip("Parameteriz
+00012c90: 6564 2074 7970 6573 2061 7265 206e 6f74  ed types are not
+00012ca0: 2073 7570 706f 7274 6564 2e22 290a 2020   supported.").  
+00012cb0: 2020 6465 6620 7465 7374 5f65 7661 6c5f    def test_eval_
+00012cc0: 6e6f 6e65 5f66 6c61 675f 6f72 6d28 7365  none_flag_orm(se
+00012cd0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+00012ce0: 730a 0a20 2020 2040 7079 7465 7374 2e6d  s..    @pytest.m
+00012cf0: 6172 6b2e 736b 6970 280a 2020 2020 2020  ark.skip(.      
+00012d00: 2020 2253 7061 6e6e 6572 204a 534f 4e5f    "Spanner JSON_
+00012d10: 5641 4c55 4528 2920 616c 7761 7973 2072  VALUE() always r
+00012d20: 6574 7572 6e73 2053 5452 494e 472c 220a  eturns STRING,".
+00012d30: 2020 2020 2020 2020 2274 6875 732c 2074          "thus, t
+00012d40: 6869 7320 7465 7374 2063 6173 6520 6361  his test case ca
+00012d50: 6e27 7420 6265 2065 7865 6375 7465 642e  n't be executed.
+00012d60: 220a 2020 2020 290a 2020 2020 6465 6620  ".    ).    def 
+00012d70: 7465 7374 5f69 6e64 6578 5f74 7970 6564  test_index_typed
+00012d80: 5f63 6f6d 7061 7269 736f 6e28 7365 6c66  _comparison(self
+00012d90: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00012da0: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+00012db0: 6b2e 736b 6970 280a 2020 2020 2020 2020  k.skip(.        
+00012dc0: 2253 7061 6e6e 6572 204a 534f 4e5f 5641  "Spanner JSON_VA
+00012dd0: 4c55 4528 2920 616c 7761 7973 2072 6574  LUE() always ret
+00012de0: 7572 6e73 2053 5452 494e 472c 220a 2020  urns STRING,".  
+00012df0: 2020 2020 2020 2274 6875 732c 2074 6869        "thus, thi
+00012e00: 7320 7465 7374 2063 6173 6520 6361 6e27  s test case can'
+00012e10: 7420 6265 2065 7865 6375 7465 642e 220a  t be executed.".
+00012e20: 2020 2020 290a 2020 2020 6465 6620 7465      ).    def te
+00012e30: 7374 5f70 6174 685f 7479 7065 645f 636f  st_path_typed_co
+00012e40: 6d70 6172 6973 6f6e 2873 656c 6629 3a0a  mparison(self):.
+00012e50: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00012e60: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+00012e70: 6b69 7028 2243 7573 746f 6d20 4a53 4f4e  kip("Custom JSON
+00012e80: 2064 652d 2f73 6572 6961 6c69 7a65 7273   de-/serializers
+00012e90: 2061 7265 206e 6f74 2073 7570 706f 7274   are not support
+00012ea0: 6564 2e22 290a 2020 2020 6465 6620 7465  ed.").    def te
+00012eb0: 7374 5f72 6f75 6e64 5f74 7269 705f 6375  st_round_trip_cu
+00012ec0: 7374 6f6d 5f6a 736f 6e28 7365 6c66 293a  stom_json(self):
+00012ed0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00012ee0: 2020 2064 6566 205f 696e 6465 785f 6669     def _index_fi
+00012ef0: 7874 7572 6573 2866 6e29 3a0a 2020 2020  xtures(fn):.    
+00012f00: 2020 2020 666e 203d 2074 6573 7469 6e67      fn = testing
+00012f10: 2e63 6f6d 6269 6e61 7469 6f6e 7328 0a20  .combinations(. 
+00012f20: 2020 2020 2020 2020 2020 2028 2262 6f6f             ("boo
+00012f30: 6c65 616e 222c 2054 7275 6529 2c0a 2020  lean", True),.  
+00012f40: 2020 2020 2020 2020 2020 2822 626f 6f6c            ("bool
+00012f50: 6561 6e22 2c20 4661 6c73 6529 2c0a 2020  ean", False),.  
+00012f60: 2020 2020 2020 2020 2020 2822 626f 6f6c            ("bool
+00012f70: 6561 6e22 2c20 4e6f 6e65 292c 0a20 2020  ean", None),.   
+00012f80: 2020 2020 2020 2020 2028 2273 7472 696e           ("strin
+00012f90: 6722 2c20 2273 6f6d 6520 7374 7269 6e67  g", "some string
+00012fa0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00012fb0: 2822 7374 7269 6e67 222c 204e 6f6e 6529  ("string", None)
+00012fc0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+00012fd0: 696e 7465 6765 7222 2c20 3135 292c 0a20  integer", 15),. 
+00012fe0: 2020 2020 2020 2020 2020 2028 2269 6e74             ("int
+00012ff0: 6567 6572 222c 2031 292c 0a20 2020 2020  eger", 1),.     
+00013000: 2020 2020 2020 2028 2269 6e74 6567 6572         ("integer
+00013010: 222c 2030 292c 0a20 2020 2020 2020 2020  ", 0),.         
+00013020: 2020 2028 2269 6e74 6567 6572 222c 204e     ("integer", N
+00013030: 6f6e 6529 2c0a 2020 2020 2020 2020 2020  one),.          
+00013040: 2020 2822 666c 6f61 7422 2c20 3238 2e35    ("float", 28.5
+00013050: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00013060: 2266 6c6f 6174 222c 204e 6f6e 6529 2c0a  "float", None),.
+00013070: 2020 2020 2020 2020 2020 2020 6964 5f3d              id_=
+00013080: 2273 6122 2c0a 2020 2020 2020 2020 2928  "sa",.        )(
+00013090: 666e 290a 2020 2020 2020 2020 7265 7475  fn).        retu
+000130a0: 726e 2066 6e0a 0a20 2020 2040 5f69 6e64  rn fn..    @_ind
+000130b0: 6578 5f66 6978 7475 7265 730a 2020 2020  ex_fixtures.    
+000130c0: 6465 6620 7465 7374 5f69 6e64 6578 5f74  def test_index_t
+000130d0: 7970 6564 5f61 6363 6573 7328 7365 6c66  yped_access(self
+000130e0: 2c20 6461 7461 7479 7065 2c20 7661 6c75  , datatype, valu
+000130f0: 6529 3a0a 2020 2020 2020 2020 6461 7461  e):.        data
+00013100: 5f74 6162 6c65 203d 2073 656c 662e 7461  _table = self.ta
+00013110: 626c 6573 2e64 6174 615f 7461 626c 650a  bles.data_table.
+00013120: 2020 2020 2020 2020 6461 7461 5f65 6c65          data_ele
+00013130: 6d65 6e74 203d 207b 226b 6579 3122 3a20  ment = {"key1": 
+00013140: 7661 6c75 657d 0a20 2020 2020 2020 2077  value}.        w
+00013150: 6974 6820 636f 6e66 6967 2e64 622e 636f  ith config.db.co
+00013160: 6e6e 6563 7428 2920 6173 2063 6f6e 6e3a  nnect() as conn:
+00013170: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00013180: 6e2e 6578 6563 7574 6528 0a20 2020 2020  n.execute(.     
+00013190: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+000131a0: 7461 626c 652e 696e 7365 7274 2829 2c0a  table.insert(),.
+000131b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131c0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000131d0: 2020 2020 2020 2269 6422 3a20 7261 6e64        "id": rand
+000131e0: 6f6d 2e72 616e 6469 6e74 2831 2c20 3130  om.randint(1, 10
+000131f0: 3030 3030 3030 3029 2c0a 2020 2020 2020  0000000),.      
+00013200: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00013210: 616d 6522 3a20 2272 6f77 3122 2c0a 2020  ame": "row1",.  
+00013220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013230: 2020 2264 6174 6122 3a20 6461 7461 5f65    "data": data_e
+00013240: 6c65 6d65 6e74 2c0a 2020 2020 2020 2020  lement,.        
+00013250: 2020 2020 2020 2020 2020 2020 226e 756c              "nul
+00013260: 6c64 6174 6122 3a20 6461 7461 5f65 6c65  ldata": data_ele
+00013270: 6d65 6e74 2c0a 2020 2020 2020 2020 2020  ment,.          
+00013280: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00013290: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+000132a0: 2020 2020 6578 7072 203d 2064 6174 615f      expr = data_
+000132b0: 7461 626c 652e 632e 6461 7461 5b22 6b65  table.c.data["ke
+000132c0: 7931 225d 0a20 2020 2020 2020 2020 2020  y1"].           
+000132d0: 2065 7870 7220 3d20 6765 7461 7474 7228   expr = getattr(
+000132e0: 6578 7072 2c20 2261 735f 2573 2220 2520  expr, "as_%s" % 
+000132f0: 6461 7461 7479 7065 2928 290a 0a20 2020  datatype)()..   
+00013300: 2020 2020 2020 2020 2072 6f75 6e64 7472           roundtr
+00013310: 6970 203d 2063 6f6e 6e2e 7363 616c 6172  ip = conn.scalar
+00013320: 2873 656c 6563 7428 5b65 7870 725d 2929  (select([expr]))
+00013330: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00013340: 726f 756e 6474 7269 7020 696e 2028 2274  roundtrip in ("t
+00013350: 7275 6522 2c20 2266 616c 7365 222c 204e  rue", "false", N
+00013360: 6f6e 6529 3a0a 2020 2020 2020 2020 2020  one):.          
+00013370: 2020 2020 2020 726f 756e 6474 7269 7020        roundtrip 
+00013380: 3d20 7374 7228 726f 756e 6474 7269 7029  = str(roundtrip)
+00013390: 2e63 6170 6974 616c 697a 6528 290a 0a20  .capitalize().. 
+000133a0: 2020 2020 2020 2020 2020 2065 715f 2873             eq_(s
+000133b0: 7472 2872 6f75 6e64 7472 6970 292c 2073  tr(roundtrip), s
+000133c0: 7472 2876 616c 7565 2929 0a0a 2020 2020  tr(value))..    
+000133d0: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+000133e0: 7028 0a20 2020 2020 2020 2022 5370 616e  p(.        "Span
+000133f0: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
+00013400: 6f72 7420 7479 7065 2063 6173 7473 2069  ort type casts i
+00013410: 6e73 6964 6520 4a53 4f4e 5f56 414c 5545  nside JSON_VALUE
+00013420: 2829 2066 756e 6374 696f 6e2e 220a 2020  () function.".  
+00013430: 2020 290a 2020 2020 6465 6620 7465 7374    ).    def test
+00013440: 5f72 6f75 6e64 5f74 7269 705f 6a73 6f6e  _round_trip_json
+00013450: 5f6e 756c 6c5f 6173 5f6a 736f 6e5f 6e75  _null_as_json_nu
+00013460: 6c6c 2873 656c 6629 3a0a 2020 2020 2020  ll(self):.      
+00013470: 2020 7061 7373 0a0a 2020 2020 4070 7974    pass..    @pyt
+00013480: 6573 742e 6d61 726b 2e73 6b69 7028 0a20  est.mark.skip(. 
+00013490: 2020 2020 2020 2022 5370 616e 6e65 7220         "Spanner 
+000134a0: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
+000134b0: 7479 7065 2063 6173 7473 2069 6e73 6964  type casts insid
+000134c0: 6520 4a53 4f4e 5f56 414c 5545 2829 2066  e JSON_VALUE() f
+000134d0: 756e 6374 696f 6e2e 220a 2020 2020 290a  unction.".    ).
+000134e0: 2020 2020 6465 6620 7465 7374 5f72 6f75      def test_rou
+000134f0: 6e64 5f74 7269 705f 6e6f 6e65 5f61 735f  nd_trip_none_as_
+00013500: 6a73 6f6e 5f6e 756c 6c28 7365 6c66 293a  json_null(self):
+00013510: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00013520: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+00013530: 736b 6970 280a 2020 2020 2020 2020 2253  skip(.        "S
+00013540: 7061 6e6e 6572 2064 6f65 736e 2774 2073  panner doesn't s
+00013550: 7570 706f 7274 2074 7970 6520 6361 7374  upport type cast
+00013560: 7320 696e 7369 6465 204a 534f 4e5f 5641  s inside JSON_VA
+00013570: 4c55 4528 2920 6675 6e63 7469 6f6e 2e22  LUE() function."
+00013580: 0a20 2020 2029 0a20 2020 2064 6566 2074  .    ).    def t
+00013590: 6573 745f 726f 756e 645f 7472 6970 5f6e  est_round_trip_n
+000135a0: 6f6e 655f 6173 5f73 716c 5f6e 756c 6c28  one_as_sql_null(
+000135b0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+000135c0: 6173 730a 0a0a 636c 6173 7320 4578 6563  ass...class Exec
+000135d0: 7574 696f 6e4f 7074 696f 6e73 5265 7175  utionOptionsRequ
+000135e0: 6573 7450 7269 6f72 6f74 7954 6573 7428  estPriorotyTest(
+000135f0: 6669 7874 7572 6573 2e54 6573 7442 6173  fixtures.TestBas
+00013600: 6529 3a0a 2020 2020 6465 6620 7365 7455  e):.    def setU
+00013610: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00013620: 2073 656c 662e 5f65 6e67 696e 6520 3d20   self._engine = 
+00013630: 6372 6561 7465 5f65 6e67 696e 6528 6765  create_engine(ge
+00013640: 745f 6462 5f75 726c 2829 2c20 706f 6f6c  t_db_url(), pool
+00013650: 5f73 697a 653d 3129 0a20 2020 2020 2020  _size=1).       
+00013660: 206d 6574 6164 6174 6120 3d20 4d65 7461   metadata = Meta
+00013670: 4461 7461 2862 696e 643d 7365 6c66 2e5f  Data(bind=self._
+00013680: 656e 6769 6e65 290a 0a20 2020 2020 2020  engine)..       
+00013690: 2073 656c 662e 5f74 6162 6c65 203d 2054   self._table = T
+000136a0: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
+000136b0: 2020 2265 7865 6375 7469 6f6e 5f6f 7074    "execution_opt
+000136c0: 696f 6e73 3222 2c0a 2020 2020 2020 2020  ions2",.        
+000136d0: 2020 2020 6d65 7461 6461 7461 2c0a 2020      metadata,.  
+000136e0: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
+000136f0: 2822 6f70 745f 6964 222c 2049 6e74 6567  ("opt_id", Integ
+00013700: 6572 2c20 7072 696d 6172 795f 6b65 793d  er, primary_key=
+00013710: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
+00013720: 2020 2043 6f6c 756d 6e28 226f 7074 5f6e     Column("opt_n
+00013730: 616d 6522 2c20 5374 7269 6e67 2831 3629  ame", String(16)
+00013740: 2c20 6e75 6c6c 6162 6c65 3d46 616c 7365  , nullable=False
+00013750: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
+00013760: 2020 2020 2020 6d65 7461 6461 7461 2e63        metadata.c
+00013770: 7265 6174 655f 616c 6c28 7365 6c66 2e5f  reate_all(self._
+00013780: 656e 6769 6e65 290a 2020 2020 2020 2020  engine).        
+00013790: 7469 6d65 2e73 6c65 6570 2831 290a 0a20  time.sleep(1).. 
+000137a0: 2020 2064 6566 2074 6573 745f 7265 7175     def test_requ
+000137b0: 6573 745f 7072 696f 7269 7479 2873 656c  est_priority(sel
+000137c0: 6629 3a0a 2020 2020 2020 2020 5052 494f  f):.        PRIO
+000137d0: 5249 5459 203d 2052 6571 7565 7374 4f70  RITY = RequestOp
+000137e0: 7469 6f6e 732e 5072 696f 7269 7479 2e50  tions.Priority.P
+000137f0: 5249 4f52 4954 595f 4d45 4449 554d 0a20  RIORITY_MEDIUM. 
+00013800: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00013810: 2e5f 656e 6769 6e65 2e63 6f6e 6e65 6374  ._engine.connect
+00013820: 2829 2e65 7865 6375 7469 6f6e 5f6f 7074  ().execution_opt
+00013830: 696f 6e73 280a 2020 2020 2020 2020 2020  ions(.          
+00013840: 2020 7265 7175 6573 745f 7072 696f 7269    request_priori
+00013850: 7479 3d50 5249 4f52 4954 590a 2020 2020  ty=PRIORITY.    
+00013860: 2020 2020 2920 6173 2063 6f6e 6e65 6374      ) as connect
+00013870: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+00013880: 2063 6f6e 6e65 6374 696f 6e2e 6578 6563   connection.exec
+00013890: 7574 6528 7365 6c65 6374 285b 222a 225d  ute(select(["*"]
+000138a0: 2c20 6672 6f6d 5f6f 626a 3d73 656c 662e  , from_obj=self.
+000138b0: 5f74 6162 6c65 2929 2e66 6574 6368 616c  _table)).fetchal
+000138c0: 6c28 290a 0a20 2020 2020 2020 2077 6974  l()..        wit
+000138d0: 6820 7365 6c66 2e5f 656e 6769 6e65 2e63  h self._engine.c
+000138e0: 6f6e 6e65 6374 2829 2061 7320 636f 6e6e  onnect() as conn
+000138f0: 6563 7469 6f6e 3a0a 2020 2020 2020 2020  ection:.        
+00013900: 2020 2020 6173 7365 7274 2063 6f6e 6e65      assert conne
+00013910: 6374 696f 6e2e 636f 6e6e 6563 7469 6f6e  ction.connection
+00013920: 2e72 6571 7565 7374 5f70 7269 6f72 6974  .request_priorit
+00013930: 7920 6973 204e 6f6e 650a 0a20 2020 2020  y is None..     
+00013940: 2020 2065 6e67 696e 6520 3d20 6372 6561     engine = crea
+00013950: 7465 5f65 6e67 696e 6528 2273 716c 6974  te_engine("sqlit
+00013960: 653a 2f2f 2f64 6174 6162 6173 6522 290a  e:///database").
+00013970: 2020 2020 2020 2020 7769 7468 2065 6e67          with eng
+00013980: 696e 652e 636f 6e6e 6563 7428 2920 6173  ine.connect() as
+00013990: 2063 6f6e 6e65 6374 696f 6e3a 0a20 2020   connection:.   
+000139a0: 2020 2020 2020 2020 2070 6173 730a 0a0a           pass...
+000139b0: 636c 6173 7320 4372 6561 7465 456e 6769  class CreateEngi
+000139c0: 6e65 5769 7468 436c 6965 6e74 4f62 6a65  neWithClientObje
+000139d0: 6374 5465 7374 2866 6978 7475 7265 732e  ctTest(fixtures.
+000139e0: 5465 7374 4261 7365 293a 0a20 2020 2064  TestBase):.    d
+000139f0: 6566 2074 6573 745f 6372 6561 7465 5f65  ef test_create_e
+00013a00: 6e67 696e 655f 775f 7661 6c69 645f 636c  ngine_w_valid_cl
+00013a10: 6965 6e74 5f6f 626a 6563 7428 7365 6c66  ient_object(self
+00013a20: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00013a30: 2020 2020 2020 2053 5041 4e4e 4552 2054         SPANNER T
+00013a40: 4553 543a 0a0a 2020 2020 2020 2020 4368  EST:..        Ch
+00013a50: 6563 6b20 7468 6174 2077 6520 6361 6e20  eck that we can 
+00013a60: 636f 6e6e 6563 7420 746f 2053 716c 416c  connect to SqlAl
+00013a70: 6368 656d 790a 2020 2020 2020 2020 6279  chemy.        by
+00013a80: 2070 6173 7369 6e67 2063 7573 746f 6d20   passing custom 
+00013a90: 436c 6965 6e74 206f 626a 6563 742e 0a20  Client object.. 
+00013aa0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013ab0: 2020 2063 6c69 656e 7420 3d20 436c 6965     client = Clie
+00013ac0: 6e74 2870 726f 6a65 6374 3d67 6574 5f70  nt(project=get_p
+00013ad0: 726f 6a65 6374 2829 290a 2020 2020 2020  roject()).      
+00013ae0: 2020 656e 6769 6e65 203d 2063 7265 6174    engine = creat
+00013af0: 655f 656e 6769 6e65 2867 6574 5f64 625f  e_engine(get_db_
+00013b00: 7572 6c28 292c 2063 6f6e 6e65 6374 5f61  url(), connect_a
+00013b10: 7267 733d 7b22 636c 6965 6e74 223a 2063  rgs={"client": c
+00013b20: 6c69 656e 747d 290a 2020 2020 2020 2020  lient}).        
+00013b30: 7769 7468 2065 6e67 696e 652e 636f 6e6e  with engine.conn
+00013b40: 6563 7428 2920 6173 2063 6f6e 6e65 6374  ect() as connect
+00013b50: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+00013b60: 2061 7373 6572 7420 636f 6e6e 6563 7469   assert connecti
+00013b70: 6f6e 2e63 6f6e 6e65 6374 696f 6e2e 696e  on.connection.in
+00013b80: 7374 616e 6365 2e5f 636c 6965 6e74 203d  stance._client =
+00013b90: 3d20 636c 6965 6e74 0a0a 2020 2020 6465  = client..    de
+00013ba0: 6620 7465 7374 5f63 7265 6174 655f 656e  f test_create_en
+00013bb0: 6769 6e65 5f77 5f69 6e76 616c 6964 5f63  gine_w_invalid_c
+00013bc0: 6c69 656e 745f 6f62 6a65 6374 2873 656c  lient_object(sel
+00013bd0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+00013be0: 2020 2020 2020 2020 5350 414e 4e45 5220          SPANNER 
+00013bf0: 5445 5354 3a0a 0a20 2020 2020 2020 2043  TEST:..        C
+00013c00: 6865 636b 2074 6861 7420 6966 2070 726f  heck that if pro
+00013c10: 6a65 6374 2069 6420 696e 2075 726c 2061  ject id in url a
+00013c20: 6e64 2063 7573 746f 6d20 436c 6965 6e74  nd custom Client
+00013c30: 0a20 2020 2020 2020 204f 626a 6563 7420  .        Object 
+00013c40: 7061 7373 6564 2074 6f20 656e 6769 6e65  passed to engine
+00013c50: 7220 6d69 736d 6174 6368 2c20 6572 726f  r mismatch, erro
+00013c60: 7220 6973 2074 6872 6f77 6e2e 0a20 2020  r is thrown..   
+00013c70: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013c80: 2063 6c69 656e 7420 3d20 436c 6965 6e74   client = Client
+00013c90: 2870 726f 6a65 6374 3d22 7072 6f6a 6563  (project="projec
+00013ca0: 745f 6964 2229 0a20 2020 2020 2020 2065  t_id").        e
+00013cb0: 6e67 696e 6520 3d20 6372 6561 7465 5f65  ngine = create_e
+00013cc0: 6e67 696e 6528 6765 745f 6462 5f75 726c  ngine(get_db_url
+00013cd0: 2829 2c20 636f 6e6e 6563 745f 6172 6773  (), connect_args
+00013ce0: 3d7b 2263 6c69 656e 7422 3a20 636c 6965  ={"client": clie
+00013cf0: 6e74 7d29 0a0a 2020 2020 2020 2020 7769  nt})..        wi
+00013d00: 7468 2070 7974 6573 742e 7261 6973 6573  th pytest.raises
+00013d10: 2856 616c 7565 4572 726f 7229 3a0a 2020  (ValueError):.  
+00013d20: 2020 2020 2020 2020 2020 656e 6769 6e65            engine
+00013d30: 2e63 6f6e 6e65 6374 2829 0a              .connect().
```

