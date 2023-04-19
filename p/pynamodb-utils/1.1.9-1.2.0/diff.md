# Comparing `tmp/pynamodb_utils-1.1.9.tar.gz` & `tmp/pynamodb_utils-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamodb_utils-1.1.9.tar", last modified: Mon Oct  3 13:40:44 2022, max compression
+gzip compressed data, was "pynamodb_utils-1.2.0.tar", last modified: Wed Apr 19 15:13:07 2023, max compression
```

## Comparing `pynamodb_utils-1.1.9.tar` & `pynamodb_utils-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 13:40:44.780430 pynamodb_utils-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)     3565 2022-10-03 13:40:44.780430 pynamodb_utils-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2406 2022-10-03 13:40:38.000000 pynamodb_utils-1.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 13:40:44.780430 pynamodb_utils-1.1.9/pynamodb_utils/
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-03 13:40:38.000000 pynamodb_utils-1.1.9/pynamodb_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3176 2022-10-03 13:40:38.000000 pynamodb_utils-1.1.9/pynamodb_utils/attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-10-03 13:40:38.000000 pynamodb_utils-1.1.9/pynamodb_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1688 2022-10-03 13:40:38.000000 pynamodb_utils-1.1.9/pynamodb_utils/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-10-03 13:40:38.000000 pynamodb_utils-1.1.9/pynamodb_utils/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     5165 2022-10-03 13:40:38.000000 pynamodb_utils-1.1.9/pynamodb_utils/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3010 2022-10-03 13:40:38.000000 pynamodb_utils-1.1.9/pynamodb_utils/query_serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-10-03 13:40:38.000000 pynamodb_utils-1.1.9/pynamodb_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 13:40:44.780430 pynamodb_utils-1.1.9/pynamodb_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3565 2022-10-03 13:40:44.000000 pynamodb_utils-1.1.9/pynamodb_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-10-03 13:40:44.000000 pynamodb_utils-1.1.9/pynamodb_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 13:40:44.000000 pynamodb_utils-1.1.9/pynamodb_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-03 13:40:44.000000 pynamodb_utils-1.1.9/pynamodb_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-03 13:40:44.000000 pynamodb_utils-1.1.9/pynamodb_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-10-03 13:40:44.784431 pynamodb_utils-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-10-03 13:40:38.000000 pynamodb_utils-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:13:07.656191 pynamodb_utils-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-19 15:12:59.000000 pynamodb_utils-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-19 15:13:07.656191 pynamodb_utils-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-19 15:12:59.000000 pynamodb_utils-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-19 15:13:07.656191 pynamodb_utils-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-19 15:12:59.000000 pynamodb_utils-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:13:07.652191 pynamodb_utils-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:13:07.656191 pynamodb_utils-1.2.0/src/pynamodb_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 15:12:59.000000 pynamodb_utils-1.2.0/src/pynamodb_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-19 15:12:59.000000 pynamodb_utils-1.2.0/src/pynamodb_utils/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-19 15:12:59.000000 pynamodb_utils-1.2.0/src/pynamodb_utils/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-19 15:12:59.000000 pynamodb_utils-1.2.0/src/pynamodb_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-19 15:12:59.000000 pynamodb_utils-1.2.0/src/pynamodb_utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-04-19 15:12:59.000000 pynamodb_utils-1.2.0/src/pynamodb_utils/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-19 15:12:59.000000 pynamodb_utils-1.2.0/src/pynamodb_utils/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-19 15:12:59.000000 pynamodb_utils-1.2.0/src/pynamodb_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:13:07.656191 pynamodb_utils-1.2.0/src/pynamodb_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-19 15:13:07.000000 pynamodb_utils-1.2.0/src/pynamodb_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-19 15:13:07.000000 pynamodb_utils-1.2.0/src/pynamodb_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:13:07.000000 pynamodb_utils-1.2.0/src/pynamodb_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 15:13:07.000000 pynamodb_utils-1.2.0/src/pynamodb_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 15:13:07.000000 pynamodb_utils-1.2.0/src/pynamodb_utils.egg-info/top_level.txt
```

### Comparing `pynamodb_utils-1.1.9/PKG-INFO` & `pynamodb_utils-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,113 @@
 Metadata-Version: 2.1
 Name: pynamodb_utils
-Version: 1.1.9
+Version: 1.2.0
 Summary: Utilities package for pynamodb.
 Home-page: https://github.com/micmurawski/pynamodb-utils/
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 License: MIT
-Description: # Introduction
-        
-        Pynamodb Utils is a collection of small helper functions, utilities and classes which make common patterns easier. It helped me make my job easier in the past.
-        
-        [![Tests](https://github.com/micmurawski/pynamodb-utils/actions/workflows/main.yml/badge.svg)](https://github.com/micmurawski/pynamodb-utils/actions/workflows/main.yml) [![pypi](https://img.shields.io/pypi/v/pynamodb-utils.svg)](https://pypi.org/project/pynamodb-utils/)
-        
-        ## Examples are:
-        
-         - Models with automatic ``updated_at``, ``created_at`` and ``deleted_at`` fields
-         - Attributes for enums and dynamic mappings
-         - Class with methods that allow to generate from JSON/dict query/scan conditions
-        
-        ## To install:
-        Run ``pip install pynamodb-utils`` or execute ``python setup.py install`` in the source directory
-        
-        ## Example of Usage
-        
-        To setup pynamodb models with authomaticly generated timestamps and useful functions allowing serialization of scan conditions from JSON input from API.
-        
-        ```python
-        from datetime import timezone, datetime
-        from pynamodb.attributes import UnicodeAttribute
-        from pynamodb_utils import DynamicMapAttribute, AsDictModel,
-        JSONQueryModel, TimestampedModel
-        
-        
-        class Post(AsDictModel, JSONQueryModel, TimestampedModel):
-            name = UnicodeAttribute(hash_key=True)
-            content = UnicodeAttribute()
-            tags = DynamicMapAttribute(default={})
-        
-            class Meta:
-                table_name = 'example-table-name'
-                TZINFO = timezone.utc
-        
-        Post.create_table(read_capacity_units=10, write_capacity_units=10)
-        
-        post = Post(
-            name='A weekly news.',
-            content='Last week took place...',
-            tags={
-                "type": "news",
-                "topics": ["stock exchange", "NYSE"]
-            }
-        )
-        post.save()
-        
-        condition = Post.get_conditions_from_json(query={
-            "created_at__lte": str(datetime.now()),
-            "tags.type__equals": "news",
-            "tags.topics__contains": ["NYSE"]
-        })
-        results = Post.scan(filter_condition=condition)
-        print(next(results).as_dict())
-        ```
-        That lines of code should result with following output
-        
-        ```
-        {
-                'name': 'A weekly news.',
-                'created_at': '2019-01-01 00:00:00+00:00',
-                'updated_at': '2019-01-01 00:00:00+00:00',
-                'deleted_at': None,
-                'content': 'Last week took place...',
-                'tags': {
-                    'type': 'news',
-                    'topics': ['stock exchange', 'NYSE']
-                }
-            }
-        ```
-        
-        ## Links
-        * https://github.com/pynamodb/PynamoDB
-        * https://pypi.org/project/pynamodb-utils/
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Introduction
+
+Pynamodb Utils is a collection of small helper functions, utilities and classes which make common patterns easier. It helped me make my job easier in the past.
+
+[![Tests](https://github.com/micmurawski/pynamodb-utils/actions/workflows/main.yml/badge.svg)](https://github.com/micmurawski/pynamodb-utils/actions/workflows/main.yml) [![pypi](https://img.shields.io/pypi/v/pynamodb-utils.svg)](https://pypi.org/project/pynamodb-utils/)
+
+## Examples are:
+
+ - Models with automatic ``updated_at``, ``created_at`` and ``deleted_at`` fields
+ - Attributes for enums and dynamic mappings
+ - Class with methods that allow to generate from JSON/dict query/scan conditions
+
+## To install:
+Run ``pip install pynamodb-utils`` or execute ``python setup.py install`` in the source directory
+
+## Example of Usage
+
+To setup pynamodb models with authomaticly generated timestamps and useful functions allowing serialization of scan conditions from JSON input from API.
+
+```python
+from datetime import timezone, datetime
+from pynamodb.attributes import UnicodeAttribute
+from pynamodb_utils import DynamicMapAttribute, AsDictModel,
+JSONQueryModel, TimestampedModel
+
+
+class CategoryEnum(enum.Enum):
+    finance = enum.auto()
+    politics = enum.auto()
+
+class PostCategoryCreatedAtGSI(GlobalSecondaryIndex):
+    category = EnumAttribute(hash_key=True, enum=CategoryEnum)
+    created_at = UTCDateTimeAttribute(range_key=True)
+
+    class Meta:
+        index_name = "example-index-name"
+        projection = AllProjection
+
+class Post(AsDictModel, JSONQueryModel, TimestampedModel):
+    name = UnicodeAttribute(hash_key=True)
+    sub_name = UnicodeAttribute(range_key=True)
+    category = EnumAttribute(enum=CategoryEnum, default=CategoryEnum.finance)
+    content = UnicodeAttribute()
+    tags = DynamicMapAttribute(default={})
+    category_created_at_gsi = PostCategoryCreatedAtGSI()
+
+    class Meta:
+        table_name = 'example-table-name'
+        TZINFO = timezone.utc
+
+Post.create_table(read_capacity_units=10, write_capacity_units=10)
+
+post = Post(
+    name='A weekly news.',
+    sub_name='Shocking revelations',
+    content='Last week took place...',
+    category=CategoryEnum.finance,
+    tags={
+        "type": "news",
+        "topics": ["stock exchange", "NYSE"]
+    }
+)
+post.save()
+
+condition = Post.make_index_query(
+    query={
+        "created_at__lte": str(datetime.now()),
+        "sub_name__exists": None,
+        "category__equals": "finance",
+        "OR": {"tags.type__equals": "news", "tags.topics__contains": ["NYSE"]},
+    }
+) # class method executes query on the most optimal index
+print(next(results).as_dict())
+```
+That lines of code should result with following output
+
+```
+{
+        'name': 'A weekly news.',
+        'created_at': '2019-01-01 00:00:00+00:00',
+        'updated_at': '2019-01-01 00:00:00+00:00',
+        'deleted_at': None,
+        'content': 'Last week took place...',
+        'tags': {
+            'type': 'news',
+            'topics': ['stock exchange', 'NYSE']
+        }
+    }
+```
+
+## Links
+* https://github.com/pynamodb/PynamoDB
+* https://pypi.org/project/pynamodb-utils/
+
+
```

### Comparing `pynamodb_utils-1.1.9/README.md` & `pynamodb_utils-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,41 +20,60 @@
 ```python
 from datetime import timezone, datetime
 from pynamodb.attributes import UnicodeAttribute
 from pynamodb_utils import DynamicMapAttribute, AsDictModel,
 JSONQueryModel, TimestampedModel
 
 
+class CategoryEnum(enum.Enum):
+    finance = enum.auto()
+    politics = enum.auto()
+
+class PostCategoryCreatedAtGSI(GlobalSecondaryIndex):
+    category = EnumAttribute(hash_key=True, enum=CategoryEnum)
+    created_at = UTCDateTimeAttribute(range_key=True)
+
+    class Meta:
+        index_name = "example-index-name"
+        projection = AllProjection
+
 class Post(AsDictModel, JSONQueryModel, TimestampedModel):
     name = UnicodeAttribute(hash_key=True)
+    sub_name = UnicodeAttribute(range_key=True)
+    category = EnumAttribute(enum=CategoryEnum, default=CategoryEnum.finance)
     content = UnicodeAttribute()
     tags = DynamicMapAttribute(default={})
+    category_created_at_gsi = PostCategoryCreatedAtGSI()
 
     class Meta:
         table_name = 'example-table-name'
         TZINFO = timezone.utc
 
 Post.create_table(read_capacity_units=10, write_capacity_units=10)
 
 post = Post(
     name='A weekly news.',
+    sub_name='Shocking revelations',
     content='Last week took place...',
+    category=CategoryEnum.finance,
     tags={
         "type": "news",
         "topics": ["stock exchange", "NYSE"]
     }
 )
 post.save()
 
-condition = Post.get_conditions_from_json(query={
-    "created_at__lte": str(datetime.now()),
-    "tags.type__equals": "news",
-    "tags.topics__contains": ["NYSE"]
-})
-results = Post.scan(filter_condition=condition)
+condition = Post.make_index_query(
+    query={
+        "created_at__lte": str(datetime.now()),
+        "sub_name__exists": None,
+        "category__equals": "finance",
+        "OR": {"tags.type__equals": "news", "tags.topics__contains": ["NYSE"]},
+    }
+) # class method executes query on the most optimal index
 print(next(results).as_dict())
 ```
 That lines of code should result with following output
 
 ```
 {
         'name': 'A weekly news.',
@@ -67,8 +86,8 @@
             'topics': ['stock exchange', 'NYSE']
         }
     }
 ```
 
 ## Links
 * https://github.com/pynamodb/PynamoDB
-* https://pypi.org/project/pynamodb-utils/
+* https://pypi.org/project/pynamodb-utils/
```

### Comparing `pynamodb_utils-1.1.9/pynamodb_utils/filters.py` & `pynamodb_utils-1.2.0/src/pynamodb_utils/conditions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,56 @@
 import operator
 from functools import reduce
-from typing import Type
+from typing import Any, Callable, Dict
 
 from pynamodb.attributes import Attribute
+from pynamodb.expressions.condition import Condition
 from pynamodb.expressions.operand import Path
 from pynamodb.models import Model
 
 from pynamodb_utils.exceptions import FilterError
 from pynamodb_utils.parsers import OPERATORS_MAPPING
 from pynamodb_utils.utils import get_nested_attribute
 
 
-def create_model_filter(model: Type[Model], args, _operator=operator.and_, raise_exception=True):
+def create_model_condition(
+    model: Model,
+    args: Dict[str, Any],
+    _operator: Callable = operator.and_,
+    raise_exception: bool = True
+) -> Condition:
+    """
+        Function creates pynamodb conditions based on input dictionary (args)
+        Parameters:
+                model (pynamodb.model.Model): Corresponing pynamodb model
+                args (dict): The input dictionary with query
+                _operator (Callable): operator used to consolidate conditions
+                raise_exception (bool): boolean value enabling expceptions on missing nested attrs
+        Returns:
+                condtion (Condition): computed pynamodb condition
+    """
     conditions_list = []
 
     for key, value in args.items():
         array = key.rsplit('__', 1)
         field_name = array[0]
         operator_name = array[1] if len(array) > 1 and array[1] != 'not' else ''
         if operator_name.replace('not_', '') not in OPERATORS_MAPPING:
             raise FilterError(
                 message={key: [f'Operator {operator_name} does not exist.'
                                f' Choose some of available: {", ".join(OPERATORS_MAPPING.keys())}']},
                 status_code=400
             )
         nested_attr = get_nested_attribute(model, field_name, raise_exception)
+
         if isinstance(nested_attr, (Attribute, Path)):
             if 'not_' in operator_name:
                 operator_name = operator_name.replace('not_', '')
-                operator_handler = OPERATORS_MAPPING.get(operator_name)
+                operator_handler = OPERATORS_MAPPING[operator_name]
                 conditions_list.append(~operator_handler(model, field_name, nested_attr, value))
             else:
-                operator_handler = OPERATORS_MAPPING.get(operator_name)
+                operator_handler = OPERATORS_MAPPING[operator_name]
                 conditions_list.append(operator_handler(model, field_name, nested_attr, value))
-
     if not conditions_list:
         return None
     else:
         return reduce(_operator, conditions_list)
```

### Comparing `pynamodb_utils-1.1.9/pynamodb_utils/models.py` & `pynamodb_utils-1.2.0/src/pynamodb_utils/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,55 @@
 from datetime import timezone
 
-from marshmallow.exceptions import ValidationError
 from pynamodb.attributes import UTCDateTimeAttribute
-from pynamodb.models import Model
+from pynamodb.expressions.condition import Condition
+from pynamodb.models import Model, ResultIterator
 
-from pynamodb_utils.exceptions import FilterError
-from pynamodb_utils.query_serializer import QuerySerializer
+from pynamodb_utils.serializers import ConditionsSerializer, QuerySerializer
 from pynamodb_utils.utils import get_timestamp, parse_attrs_to_dict
 
 
 class JSONQueryModel(Model):
-
     class Meta:
         abstract = True
 
     @classmethod
-    def get_conditions_from_json(cls, query: dict):
-        try:
-            return QuerySerializer().load(model=cls, data=query)
-        except ValidationError as e:
-            raise FilterError(message=e.messages, status_code=400)
+    def get_conditions_from_json(cls, query: dict) -> Condition:
+        """
+            Class method parses query dictionary and returns computed pynamodb condition.
+
+            Parameters:
+                    query (dict): A decimal integer
+
+            Returns:
+                    condtion (Condition): computed pynamodb condition
+        """
+        return ConditionsSerializer(cls).load(data=query)
+
+    @classmethod
+    def make_index_query(cls, query: dict, **kwargs) -> ResultIterator[Model]:
+        """
+            Class method parses query dictionary and executes query on index most suitable index
+
+            Parameters:
+                    query (dict): A decimal integer
+
+            Returns:
+                    result_iterator (result_iterator): result iterator for optimized query
+        """
+        idx, query = QuerySerializer(cls).load(data=query)
+        return idx.query(**query, **kwargs)
 
 
 class AsDictModel(Model):
-
     class Meta:
         abstract = True
 
-    def as_dict(self):
+    def as_dict(self) -> dict:
+        """ Parses pynamodb model instance to python dict"""
         return parse_attrs_to_dict(self)
 
 
 class TimestampedModel(Model):
     created_at = UTCDateTimeAttribute(default=get_timestamp)
     updated_at = UTCDateTimeAttribute(default=get_timestamp)
     deleted_at = UTCDateTimeAttribute(null=True)
@@ -45,10 +63,11 @@
         self.updated_at = get_timestamp(tzinfo=tz_info)
         super().save(condition=condition)
 
     def save_without_timestamp_update(self, condition=None):
         super().save(condition=condition)
 
     def soft_delete(self, condition=None):
+        """ Puts delete_at timestamp """
         tz_info = getattr(self.Meta, "TZINFO", None)
         self.deleted_at = get_timestamp(tz_info)
         super().save(condition=condition)
```

### Comparing `pynamodb_utils-1.1.9/pynamodb_utils/parsers.py` & `pynamodb_utils-1.2.0/src/pynamodb_utils/parsers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,161 +1,189 @@
 from datetime import datetime
-from typing import Dict, List, Union
+from typing import Any, Dict, List, Union
 
 from pynamodb import attributes
+from pynamodb.attributes import Attribute
+from pynamodb.expressions.condition import Condition
 from pynamodb.expressions.operand import Path
+from pynamodb.models import Model
 
 from pynamodb_utils.attributes import EnumNumberAttribute, EnumUnicodeAttribute
 from pynamodb_utils.exceptions import FilterError
 
 
 def parse_string_to_datetime(value: str, field_name: str, *args):
     for fmt in DATETIME_FORMATS:
         try:
             return datetime.strptime(value, fmt)
         except ValueError:
             pass
-    raise FilterError(message={field_name: [
-        f"{value} is not valid type of {field_name}. Supported formats are {', '.join(DATETIME_FORMATS)}"]})
+    raise FilterError(
+        message={
+            field_name: [
+                f"{value} is not valid type of {field_name}. Supported formats are {', '.join(DATETIME_FORMATS)}"
+            ]
+        }
+    )
 
 
 DATETIME_FORMATS = [
-    '%Y-%m-%dT%H:%M:%S.%f+00:00',
-    '%Y-%m-%dT%H:%M:%S.%f',
-    '%Y-%m-%dT%H:%M:%S',
-    '%Y-%m-%dT%H:%M',
-    '%Y-%m-%d %H:%M:%S.%f+00:00',
-    '%Y-%m-%d %H:%M:%S.%f',
-    '%Y-%m-%d %H:%M:%S',
-    '%Y-%m-%d %H:%M',
-    '%Y-%m-%d'
+    "%Y-%m-%dT%H:%M:%S.%f+00:00",
+    "%Y-%m-%dT%H:%M:%S.%f",
+    "%Y-%m-%dT%H:%M:%S",
+    "%Y-%m-%dT%H:%M",
+    "%Y-%m-%d %H:%M:%S.%f+00:00",
+    "%Y-%m-%d %H:%M:%S.%f",
+    "%Y-%m-%d %H:%M:%S",
+    "%Y-%m-%d %H:%M",
+    "%Y-%m-%d",
 ]
 
 NoneType = type(None)
 
 
-def default_parser(value, *args):
+def default_parser(value: Any, *args) -> Any:
     return value
 
 
-def default_list_parser(value: List, field_name: str, *args):
+def default_list_parser(value: List[Any], field_name: str, *args) -> List[Any]:
     if isinstance(value, (list, NoneType)):
         return value
-    raise FilterError(message={field_name: [f"{value} is not valid type of {field_name}."]})
+    raise FilterError(
+        message={field_name: [f"{value} is not valid type of {field_name}."]}
+    )
 
 
-def default_dict_parser(value: Dict, field_name: str, *args):
+def default_dict_parser(value: Dict, field_name: str, *args) -> Dict[Any, Any]:
     if isinstance(value, (dict, NoneType)):
         return value
-    raise FilterError(message={field_name: [f"{value} is not valid type of {field_name}."]})
+    raise FilterError(
+        message={field_name: [f"{value} is not valid type of {field_name}."]}
+    )
 
 
-def default_bool_parser(value: bool, field_name: str, *args):
+def default_bool_parser(value: bool, field_name: str, *args) -> bool:
     if isinstance(value, (bool, NoneType)):
         return value
-    raise FilterError(message={field_name: [f"{value} is not valid type of {field_name}."]})
+    raise FilterError(
+        message={field_name: [f"{value} is not valid type of {field_name}."]}
+    )
 
 
-def default_str_parser(value, field_name: str, *args):
+def default_str_parser(value: Any, field_name: str, *args) -> str:
     if isinstance(value, (str, NoneType)):
         return value
-    raise FilterError(message={field_name: [f"{value} is not valid type of {field_name}."]})
+    raise FilterError(
+        message={field_name: [f"{value} is not valid type of {field_name}."]}
+    )
 
 
-def default_number_parser(value: Union[float, int], field_name: str, *args):
+def default_number_parser(value: Union[float, int], field_name: str, *args) -> Union[float, int]:
     if isinstance(value, (float, int, NoneType)):
         return value
-    raise FilterError(message={field_name: [f"{value} is not valid type of {field_name}."]})
+    raise FilterError(
+        message={field_name: [f"{value} is not valid type of {field_name}."]}
+    )
 
 
-def default_enum_parser(value, field_name: str, model):
+def default_enum_parser(value: Any, field_name: str, model: Model) -> Any:
     if isinstance(value, NoneType):
         return None
 
     values = getattr(model, field_name).enum.__members__
 
     _value = set(value) if isinstance(value, list) else {value}
 
     if _value.issubset(set(values)):
         return value
 
-    raise FilterError(message={field_name: [
-        f"{', '.join(value) if isinstance(value, list) else value} is not member of {', '.join(values)}."]})
+    raise FilterError(
+        message={
+            field_name: [
+                f"{', '.join(value) if isinstance(value, list) else value} is not member of {', '.join(values)}."
+            ]
+        }
+    )
 
 
 TYPE_MAPPING = {
     attributes.UTCDateTimeAttribute: parse_string_to_datetime,
     attributes.UnicodeAttribute: default_str_parser,
     Path: default_parser,
     attributes.ListAttribute: default_list_parser,
     attributes.JSONAttribute: default_dict_parser,
     attributes.MapAttribute: default_parser,
     attributes.BooleanAttribute: default_bool_parser,
     attributes.NumberAttribute: default_number_parser,
     EnumNumberAttribute: default_enum_parser,
-    EnumUnicodeAttribute: default_enum_parser
+    EnumUnicodeAttribute: default_enum_parser,
 }
 
 
-def parse_value(model, field_name: str, value):
-    attrs = field_name.split('.')
+def parse_value(model: Model, field_name: str, value: Any) -> Any:
+    attrs = field_name.split(".")
     if len(attrs) == 1:
         _type = type(getattr(model, field_name))
         if issubclass(_type, attributes.MapAttribute):
             return TYPE_MAPPING[attributes.MapAttribute](value, field_name, model)
         return TYPE_MAPPING[_type](value, field_name, model)
     else:
         return TYPE_MAPPING[attributes.MapAttribute](value, field_name, model)
 
 
-def get_equals_condition(model, field_name: str, attr, value):
+def get_equals_condition(model: Model, field_name: str, attr: Attribute, value: Any) -> Condition:
     parsed_value = parse_value(model, field_name, value)
     if parsed_value is None:
         return attr.does_not_exist()
     return attr.__eq__(parsed_value)
 
 
-def get_startswith_condition(model, field_name: str, attr, value):
+def get_startswith_condition(model: Model, field_name: str, attr: Attribute, value: Any) -> Condition:
     return attr.startswith(parse_value(model, field_name, value))
 
 
-def get_gt_condition(model, field_name: str, attr, value):
+def get_exists_condition(model: Model, field_name: str, attr: Attribute, value: Any) -> Condition:
+    return attr.exists()
+
+
+def get_gt_condition(model: Model, field_name: str, attr: Attribute, value: Any) -> Condition:
     return attr.__gt__(parse_value(model, field_name, value))
 
 
-def get_lt_condition(model, field_name: str, attr, value):
+def get_lt_condition(model: Model, field_name: str, attr: Attribute, value: Any) -> Condition:
     return attr.__lt__(parse_value(model, field_name, value))
 
 
-def get_gte_condition(model, field_name: str, attr, value):
+def get_gte_condition(model: Model, field_name: str, attr: Attribute, value: Any) -> Condition:
     return attr.__ge__(parse_value(model, field_name, value))
 
 
-def get_lte_condition(model, field_name: str, attr, value):
+def get_lte_condition(model: Model, field_name: str, attr: Attribute, value: Any) -> Condition:
     return attr.__le__(parse_value(model, field_name, value))
 
 
-def get_contains_condition(model, field_name: str, attr, value):
+def get_contains_condition(model: Model, field_name: str, attr: Attribute, value: Any) -> Condition:
     parsed_value = parse_value(model, field_name, value)
     if isinstance(parsed_value, list):
         return attr.contains(*parsed_value)
     return attr.contains(parsed_value)
 
 
-def get_is_in_condition(model, field_name: str, attr, value):
+def get_is_in_condition(model: Model, field_name: str, attr: Attribute, value: Any) -> Condition:
     parsed_value = parse_value(model, field_name, value)
     if isinstance(parsed_value, list):
         return attr.is_in(*parsed_value)
     return attr.is_in(parsed_value)
 
 
 OPERATORS_MAPPING = {
-    '': get_equals_condition,
-    'equals': get_equals_condition,
-    'contains': get_contains_condition,
-    'startswith': get_startswith_condition,
-    'gt': get_gt_condition,
-    'lt': get_lt_condition,
-    'gte': get_gte_condition,
-    'lte': get_lte_condition,
-    'is_in': get_is_in_condition,
+    "": get_equals_condition,
+    "equals": get_equals_condition,
+    "contains": get_contains_condition,
+    "exists": get_exists_condition,
+    "startswith": get_startswith_condition,
+    "gt": get_gt_condition,
+    "lt": get_lt_condition,
+    "gte": get_gte_condition,
+    "lte": get_lte_condition,
+    "is_in": get_is_in_condition,
 }
```

### Comparing `pynamodb_utils-1.1.9/pynamodb_utils.egg-info/PKG-INFO` & `pynamodb_utils-1.2.0/src/pynamodb_utils.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,113 @@
 Metadata-Version: 2.1
 Name: pynamodb-utils
-Version: 1.1.9
+Version: 1.2.0
 Summary: Utilities package for pynamodb.
 Home-page: https://github.com/micmurawski/pynamodb-utils/
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 License: MIT
-Description: # Introduction
-        
-        Pynamodb Utils is a collection of small helper functions, utilities and classes which make common patterns easier. It helped me make my job easier in the past.
-        
-        [![Tests](https://github.com/micmurawski/pynamodb-utils/actions/workflows/main.yml/badge.svg)](https://github.com/micmurawski/pynamodb-utils/actions/workflows/main.yml) [![pypi](https://img.shields.io/pypi/v/pynamodb-utils.svg)](https://pypi.org/project/pynamodb-utils/)
-        
-        ## Examples are:
-        
-         - Models with automatic ``updated_at``, ``created_at`` and ``deleted_at`` fields
-         - Attributes for enums and dynamic mappings
-         - Class with methods that allow to generate from JSON/dict query/scan conditions
-        
-        ## To install:
-        Run ``pip install pynamodb-utils`` or execute ``python setup.py install`` in the source directory
-        
-        ## Example of Usage
-        
-        To setup pynamodb models with authomaticly generated timestamps and useful functions allowing serialization of scan conditions from JSON input from API.
-        
-        ```python
-        from datetime import timezone, datetime
-        from pynamodb.attributes import UnicodeAttribute
-        from pynamodb_utils import DynamicMapAttribute, AsDictModel,
-        JSONQueryModel, TimestampedModel
-        
-        
-        class Post(AsDictModel, JSONQueryModel, TimestampedModel):
-            name = UnicodeAttribute(hash_key=True)
-            content = UnicodeAttribute()
-            tags = DynamicMapAttribute(default={})
-        
-            class Meta:
-                table_name = 'example-table-name'
-                TZINFO = timezone.utc
-        
-        Post.create_table(read_capacity_units=10, write_capacity_units=10)
-        
-        post = Post(
-            name='A weekly news.',
-            content='Last week took place...',
-            tags={
-                "type": "news",
-                "topics": ["stock exchange", "NYSE"]
-            }
-        )
-        post.save()
-        
-        condition = Post.get_conditions_from_json(query={
-            "created_at__lte": str(datetime.now()),
-            "tags.type__equals": "news",
-            "tags.topics__contains": ["NYSE"]
-        })
-        results = Post.scan(filter_condition=condition)
-        print(next(results).as_dict())
-        ```
-        That lines of code should result with following output
-        
-        ```
-        {
-                'name': 'A weekly news.',
-                'created_at': '2019-01-01 00:00:00+00:00',
-                'updated_at': '2019-01-01 00:00:00+00:00',
-                'deleted_at': None,
-                'content': 'Last week took place...',
-                'tags': {
-                    'type': 'news',
-                    'topics': ['stock exchange', 'NYSE']
-                }
-            }
-        ```
-        
-        ## Links
-        * https://github.com/pynamodb/PynamoDB
-        * https://pypi.org/project/pynamodb-utils/
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Introduction
+
+Pynamodb Utils is a collection of small helper functions, utilities and classes which make common patterns easier. It helped me make my job easier in the past.
+
+[![Tests](https://github.com/micmurawski/pynamodb-utils/actions/workflows/main.yml/badge.svg)](https://github.com/micmurawski/pynamodb-utils/actions/workflows/main.yml) [![pypi](https://img.shields.io/pypi/v/pynamodb-utils.svg)](https://pypi.org/project/pynamodb-utils/)
+
+## Examples are:
+
+ - Models with automatic ``updated_at``, ``created_at`` and ``deleted_at`` fields
+ - Attributes for enums and dynamic mappings
+ - Class with methods that allow to generate from JSON/dict query/scan conditions
+
+## To install:
+Run ``pip install pynamodb-utils`` or execute ``python setup.py install`` in the source directory
+
+## Example of Usage
+
+To setup pynamodb models with authomaticly generated timestamps and useful functions allowing serialization of scan conditions from JSON input from API.
+
+```python
+from datetime import timezone, datetime
+from pynamodb.attributes import UnicodeAttribute
+from pynamodb_utils import DynamicMapAttribute, AsDictModel,
+JSONQueryModel, TimestampedModel
+
+
+class CategoryEnum(enum.Enum):
+    finance = enum.auto()
+    politics = enum.auto()
+
+class PostCategoryCreatedAtGSI(GlobalSecondaryIndex):
+    category = EnumAttribute(hash_key=True, enum=CategoryEnum)
+    created_at = UTCDateTimeAttribute(range_key=True)
+
+    class Meta:
+        index_name = "example-index-name"
+        projection = AllProjection
+
+class Post(AsDictModel, JSONQueryModel, TimestampedModel):
+    name = UnicodeAttribute(hash_key=True)
+    sub_name = UnicodeAttribute(range_key=True)
+    category = EnumAttribute(enum=CategoryEnum, default=CategoryEnum.finance)
+    content = UnicodeAttribute()
+    tags = DynamicMapAttribute(default={})
+    category_created_at_gsi = PostCategoryCreatedAtGSI()
+
+    class Meta:
+        table_name = 'example-table-name'
+        TZINFO = timezone.utc
+
+Post.create_table(read_capacity_units=10, write_capacity_units=10)
+
+post = Post(
+    name='A weekly news.',
+    sub_name='Shocking revelations',
+    content='Last week took place...',
+    category=CategoryEnum.finance,
+    tags={
+        "type": "news",
+        "topics": ["stock exchange", "NYSE"]
+    }
+)
+post.save()
+
+condition = Post.make_index_query(
+    query={
+        "created_at__lte": str(datetime.now()),
+        "sub_name__exists": None,
+        "category__equals": "finance",
+        "OR": {"tags.type__equals": "news", "tags.topics__contains": ["NYSE"]},
+    }
+) # class method executes query on the most optimal index
+print(next(results).as_dict())
+```
+That lines of code should result with following output
+
+```
+{
+        'name': 'A weekly news.',
+        'created_at': '2019-01-01 00:00:00+00:00',
+        'updated_at': '2019-01-01 00:00:00+00:00',
+        'deleted_at': None,
+        'content': 'Last week took place...',
+        'tags': {
+            'type': 'news',
+            'topics': ['stock exchange', 'NYSE']
+        }
+    }
+```
+
+## Links
+* https://github.com/pynamodb/PynamoDB
+* https://pypi.org/project/pynamodb-utils/
+
+
```

### Comparing `pynamodb_utils-1.1.9/setup.py` & `pynamodb_utils-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,38 +3,39 @@
 
 from setuptools import find_packages, setup
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 
 def read(*parts):
-    return codecs.open(os.path.join(HERE, *parts), 'r').read()
+    return codecs.open(os.path.join(HERE, *parts), "r").read()
 
 
 setup(
-    name='pynamodb_utils',
-    version='1.1.9',
+    name="pynamodb_utils",
+    version="1.2.0",
     author="Michal Murawski",
     author_email="mmurawski777@gmail.com",
     description="Utilities package for pynamodb.",
-    long_description=read('README.md'),
+    long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/micmurawski/pynamodb-utils/",
-    packages=find_packages(exclude=(
-        'build',
-        'tests',
-    )),
-    install_requires=[
-        'marshmallow>=3.0.0',
-        'pynamodb>=5.0.0'
-    ],
+    package_dir={"": "src"},
+    packages=find_packages(
+        where="./src",
+        exclude=(
+            'build',
+            'tests',
+        )
+    ),
+    install_requires=["pynamodb>=5.0.0"],
     include_package_data=True,
-    python_requires='>=3.6',
+    python_requires=">=3.6",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8"
+        "Programming Language :: Python :: 3.8",
     ],
 )
```

