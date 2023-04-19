# Comparing `tmp/cognite_gql_pygen-0.1.4.tar.gz` & `tmp/cognite_gql_pygen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_gql_pygen-0.1.4.tar", max compression
+gzip compressed data, was "cognite_gql_pygen-0.2.0.tar", max compression
```

## Comparing `cognite_gql_pygen-0.1.4.tar` & `cognite_gql_pygen-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,37 @@
--rw-r--r--   0        0        0    11349 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/LICENSE
--rw-r--r--   0        0        0     1782 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/README.md
--rw-r--r--   0        0        0     8930 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/README.md
--rw-r--r--   0        0        0        0 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/__init__.py
--rw-r--r--   0        0        0      238 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/bin/_functions.sh
--rwxr-xr-x   0        0        0      572 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/bin/cdf_signin.sh
--rwxr-xr-x   0        0        0      379 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/bin/schema_publish.sh
--rwxr-xr-x   0        0        0      369 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/bin/schema_render.sh
--rw-r--r--   0        0        0      167 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/cdf/__init__.py
--rw-r--r--   0        0        0    19068 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/cdf/client_dm_v3.py
--rw-r--r--   0        0        0     3910 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/cdf/data_classes_dm_v3.py
--rw-r--r--   0        0        0     2629 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/cdf/get_client.py
--rwxr-xr-x   0        0        0      346 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/config.py
--rw-r--r--   0        0        0      192 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/custom_types/__init__.py
--rw-r--r--   0        0        0      236 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/custom_types/_scalars.py
--rw-r--r--   0        0        0      760 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/custom_types/jsonobject.py
--rw-r--r--   0        0        0     4724 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/custom_types/timestamp.py
--rw-r--r--   0        0        0      196 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/__init__.py
--rw-r--r--   0        0        0     6259 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/domain_client.py
--rw-r--r--   0        0        0     3046 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/domain_model.py
--rw-r--r--   0        0        0    15859 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/domain_model_api.py
--rw-r--r--   0        0        0     3609 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/relationship_api.py
--rw-r--r--   0        0        0     6828 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/schema.py
--rw-r--r--   0        0        0      868 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/dm_clients/main.py
--rw-r--r--   0        0        0     1423 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/dm_clients/misc.py
--rw-r--r--   0        0        0        0 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/dm_clients/py.typed
--rw-r--r--   0        0        0       76 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/gqlpygen/__init__.py
--rw-r--r--   0        0        0      300 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/gqlpygen/main.py
--rw-r--r--   0        0        0       22 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/gqlpygen/version.py
--rw-r--r--   0        0        0     1900 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4050 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/README.md
+-rw-r--r--   0        0        0     8930 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/__init__.py
+-rw-r--r--   0        0        0      238 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/bin/_functions.sh
+-rwxr-xr-x   0        0        0      572 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/bin/cdf_signin.sh
+-rwxr-xr-x   0        0        0      379 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/bin/schema_publish.sh
+-rwxr-xr-x   0        0        0      209 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/bin/schema_render.sh
+-rw-r--r--   0        0        0      167 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/cdf/__init__.py
+-rw-r--r--   0        0        0    19068 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/cdf/client_dm_v3.py
+-rw-r--r--   0        0        0     3910 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/cdf/data_classes_dm_v3.py
+-rw-r--r--   0        0        0     2629 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/cdf/get_client.py
+-rwxr-xr-x   0        0        0      346 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/config.py
+-rw-r--r--   0        0        0      192 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/custom_types/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/custom_types/_scalars.py
+-rw-r--r--   0        0        0      760 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/custom_types/jsonobject.py
+-rw-r--r--   0        0        0     4724 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/custom_types/timestamp.py
+-rw-r--r--   0        0        0      196 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/__init__.py
+-rw-r--r--   0        0        0     6259 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/domain_client.py
+-rw-r--r--   0        0        0     3046 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/domain_model.py
+-rw-r--r--   0        0        0    15859 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/domain_model_api.py
+-rw-r--r--   0        0        0     3609 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/relationship_api.py
+-rw-r--r--   0        0        0     7034 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/schema.py
+-rw-r--r--   0        0        0      868 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/main.py
+-rw-r--r--   0        0        0     1423 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/misc.py
+-rw-r--r--   0        0        0        0 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/py.typed
+-rw-r--r--   0        0        0       76 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/__init__.py
+-rw-r--r--   0        0        0     1868 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/data_classes.py
+-rw-r--r--   0        0        0     1560 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/generator.py
+-rw-r--r--   0        0        0     2008 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/main.py
+-rw-r--r--   0        0        0      416 2023-04-19 05:11:21.589093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/misc.py
+-rw-r--r--   0        0        0     1288 2023-04-19 05:11:21.589093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/parser.py
+-rw-r--r--   0        0        0     1333 2023-04-19 05:11:21.589093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/templates/client.txt
+-rw-r--r--   0        0        0      803 2023-04-19 05:11:21.589093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/templates/schema.txt
+-rw-r--r--   0        0        0       22 2023-04-19 05:11:21.589093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/version.py
+-rw-r--r--   0        0        0     1965 2023-04-19 05:11:21.589093 cognite_gql_pygen-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5062 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.2.0/PKG-INFO
```

### Comparing `cognite_gql_pygen-0.1.4/LICENSE` & `cognite_gql_pygen-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.4/cognite/dm_clients/README.md` & `cognite_gql_pygen-0.2.0/cognite/dm_clients/README.md`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.4/cognite/dm_clients/bin/cdf_signin.sh` & `cognite_gql_pygen-0.2.0/cognite/dm_clients/bin/cdf_signin.sh`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.4/cognite/dm_clients/cdf/client_dm_v3.py` & `cognite_gql_pygen-0.2.0/cognite/dm_clients/cdf/client_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.4/cognite/dm_clients/cdf/data_classes_dm_v3.py` & `cognite_gql_pygen-0.2.0/cognite/dm_clients/cdf/data_classes_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.4/cognite/dm_clients/cdf/get_client.py` & `cognite_gql_pygen-0.2.0/cognite/dm_clients/cdf/get_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.4/cognite/dm_clients/custom_types/jsonobject.py` & `cognite_gql_pygen-0.2.0/cognite/dm_clients/custom_types/jsonobject.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.4/cognite/dm_clients/custom_types/timestamp.py` & `cognite_gql_pygen-0.2.0/cognite/dm_clients/custom_types/timestamp.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/domain_client.py` & `cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/domain_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/domain_model.py` & `cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/domain_model.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/domain_model_api.py` & `cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/domain_model_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/relationship_api.py` & `cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/relationship_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/schema.py` & `cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 from ..custom_types import SCALARS
 from ..custom_types._scalars import *  # noqa
 
 DomainModelT = TypeVar("DomainModelT", bound=DomainModel)
 
 
 logger = logging.getLogger(__name__)
+AUTO_GENERATED_COMMENT = """# THIS FILE IS AUTO-GENERATED!
+# Use `dm_clients schema render` to update it, see `dm_clients --help` for more information.
+
+"""
 
 
 class Schema(Generic[DomainModelT]):
     def __init__(self) -> None:
         self.types_map: Dict[str, Type[DomainModelT]] = {}
         self._root_type: Optional[type] = None
         self._root_type_cls: Optional[Type[DomainModelT]] = None
@@ -48,14 +52,16 @@
                 continue
             if line.startswith("schema {"):
                 dm_lines.pop()
                 dm_lines.pop()
                 dm_lines.pop()
                 continue
             dm_lines.append(line)
+
+        dm_lines.append(AUTO_GENERATED_COMMENT)
         return "\n".join(dm_lines[::-1])
 
     def register_type(
         self, lowercase_type_name: Optional[Union[str, Type[DomainModelT]]] = None, root_type: bool = False
     ):
         """
         Class decorator for schema types.
```

### Comparing `cognite_gql_pygen-0.1.4/cognite/dm_clients/main.py` & `cognite_gql_pygen-0.2.0/cognite/dm_clients/main.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.4/cognite/dm_clients/misc.py` & `cognite_gql_pygen-0.2.0/cognite/dm_clients/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.4/pyproject.toml` & `cognite_gql_pygen-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-gql-pygen"
-version = "0.1.4"
+version = "0.2.0"
 description = "Cognite graphQL Python generation SDK"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 
 packages = [{ include="cognite", from="." }]
 exclude = ["cognite/dm_clients/*.toml"]
 
@@ -15,17 +15,18 @@
 
 [tool.isort]
 line_length=120                # corresponds to -w  flag
 multi_line_output=3            # corresponds to -m  flag
 include_trailing_comma=true    # corresponds to -tc flag
 skip_glob = '^((?!py$).)*$'    # this makes sort all Python files
 known_third_party = []
+src_paths = [".", "examples"]
 
 [tool.poetry.scripts]
-cogpygen = "cognite.gqlpygen.main:main"
+dm = "cognite.gqlpygen.main:main"
 dm_clients = "cognite.dm_clients.main:main"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = ">=1.10"
 typer = {version = "*", extras = ["all"] }
@@ -36,14 +37,16 @@
 numpy = "^1.23.2"
 strawberry-graphql = "^0.156.4"
 docopt = "^0.6.2"
 cachelib = "^0.10.2"
 retry = "^0.9.2"
 loguru = "^0.6.0"
 dynaconf = "^3.1.12"
+graphql-core = ">=3.2"
+Jinja2 = ">=3.1"
 
 [tool.poetry.dev-dependencies]
 twine = "*"
 pre-commit = "*"
 toml = "*"
 python-dotenv = "*"
 pytest = "*"
@@ -65,14 +68,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 check_untyped_defs = true
 #disallow_any_generics = true
 #no_implicit_reexport = true
 #disallow_untyped_defs = true
 
+
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
 
 [build-system]
```

