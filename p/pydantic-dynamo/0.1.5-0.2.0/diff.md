# Comparing `tmp/pydantic_dynamo-0.1.5.tar.gz` & `tmp/pydantic_dynamo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_dynamo-0.1.5.tar", max compression
+gzip compressed data, was "pydantic_dynamo-0.2.0.tar", max compression
```

## Comparing `pydantic_dynamo-0.1.5.tar` & `pydantic_dynamo-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0     1121 2023-03-07 03:45:50.202681 pydantic_dynamo-0.1.5/LICENSE
--rw-r--r--   0        0        0        0 2023-03-07 03:36:36.814175 pydantic_dynamo-0.1.5/pydantic_dynamo/__init__.py
--rw-r--r--   0        0        0       53 2023-03-07 03:09:09.986643 pydantic_dynamo-0.1.5/pydantic_dynamo/exceptions.py
--rw-r--r--   0        0        0     2703 2023-03-07 01:09:18.686810 pydantic_dynamo-0.1.5/pydantic_dynamo/models.py
--rw-r--r--   0        0        0    23881 2023-03-14 13:45:10.978371 pydantic_dynamo-0.1.5/pydantic_dynamo/repository.py
--rw-r--r--   0        0        0      573 2023-03-07 03:09:04.521825 pydantic_dynamo-0.1.5/pydantic_dynamo/utils.py
--rw-r--r--   0        0        0      986 2023-03-29 00:17:51.985793 pydantic_dynamo-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    10533 2023-03-13 23:57:33.629068 pydantic_dynamo-0.1.5/README.md
--rw-r--r--   0        0        0    11256 1970-01-01 00:00:00.000000 pydantic_dynamo-0.1.5/setup.py
--rw-r--r--   0        0        0    10817 1970-01-01 00:00:00.000000 pydantic_dynamo-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1121 2023-03-07 03:45:50.202681 pydantic_dynamo-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-03-07 03:36:36.814175 pydantic_dynamo-0.2.0/pydantic_dynamo/__init__.py
+-rw-r--r--   0        0        0      243 2023-04-04 19:40:26.272160 pydantic_dynamo-0.2.0/pydantic_dynamo/constants.py
+-rw-r--r--   0        0        0       53 2023-03-07 03:09:09.986643 pydantic_dynamo-0.2.0/pydantic_dynamo/exceptions.py
+-rw-r--r--   0        0        0     3294 2023-04-19 02:51:16.873917 pydantic_dynamo-0.2.0/pydantic_dynamo/models.py
+-rw-r--r--   0        0        0    14586 2023-04-13 17:24:33.661892 pydantic_dynamo-0.2.0/pydantic_dynamo/repository.py
+-rw-r--r--   0        0        0    10579 2023-04-19 02:51:16.873917 pydantic_dynamo-0.2.0/pydantic_dynamo/utils.py
+-rw-r--r--   0        0        0        0 2023-04-04 19:23:43.683503 pydantic_dynamo-0.2.0/pydantic_dynamo/v2/__init__.py
+-rw-r--r--   0        0        0     4200 2023-04-19 15:32:16.137607 pydantic_dynamo-0.2.0/pydantic_dynamo/v2/models.py
+-rw-r--r--   0        0        0    16452 2023-04-19 17:58:49.187593 pydantic_dynamo-0.2.0/pydantic_dynamo/v2/repository.py
+-rw-r--r--   0        0        0     3703 2023-04-19 15:48:17.692524 pydantic_dynamo-0.2.0/pydantic_dynamo/v2/sync_repository.py
+-rw-r--r--   0        0        0     1190 2023-04-19 17:59:23.770865 pydantic_dynamo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    15133 2023-04-19 17:57:46.241111 pydantic_dynamo-0.2.0/README.md
+-rw-r--r--   0        0        0    15912 1970-01-01 00:00:00.000000 pydantic_dynamo-0.2.0/setup.py
+-rw-r--r--   0        0        0    15340 1970-01-01 00:00:00.000000 pydantic_dynamo-0.2.0/PKG-INFO
```

### Comparing `pydantic_dynamo-0.1.5/LICENSE` & `pydantic_dynamo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.1.5/pydantic_dynamo/models.py` & `pydantic_dynamo-0.2.0/pydantic_dynamo/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,16 +21,29 @@
 ObjT = TypeVar("ObjT", bound=BaseModel)
 
 
 class PartitionedContent(GenericModel, Generic[ObjT]):
     partition_ids: List[str]
     content_ids: List[str]
     item: ObjT
+    current_version: int = 1
     expiry: Optional[datetime]
 
+    def __lt__(self, other):
+        return (self.partition_ids + self.content_ids) < (other.partition_ids + other.content_ids)
+
+    def __gt__(self, other):
+        return (self.partition_ids + self.content_ids) > (other.partition_ids + other.content_ids)
+
+    def __le__(self, other):
+        return (self.partition_ids + self.content_ids) <= (other.partition_ids + other.content_ids)
+
+    def __ge__(self, other):
+        return (self.partition_ids + self.content_ids) >= (other.partition_ids + other.content_ids)
+
 
 class UpdateCommand(BaseModel):
     current_version: Optional[int]
     set_commands: Dict[str, Any] = {}
     increment_attrs: Dict[str, int] = {}
     append_attrs: Dict[str, Optional[List[Union[str, Dict]]]] = {}
     expiry: Optional[datetime]
@@ -91,14 +104,15 @@
 
     @abstractmethod
     def update(
         self,
         partition_id: Optional[Sequence[str]],
         content_id: Optional[Sequence[str]],
         command: UpdateCommand,
+        require_exists: bool,
     ) -> None:
         pass
 
     @abstractmethod
     def delete(
         self,
         partition_id: Optional[Sequence[str]],
```

### Comparing `pydantic_dynamo-0.1.5/pyproject.toml` & `pydantic_dynamo-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 [tool.poetry]
 name = "pydantic-dynamo"
-version = "0.1.5"
+version = "0.2.0"
 description = ""
 authors = ["David Jetter <davidajetter@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pydantic_dynamo"}]
 homepage = "https://github.com/david-a-jetter/pydantic-dynamo"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = "^1.20.32"
 pydantic = "^1.10.5"
 botocore = "^1.23.32"
+aioboto3 = "^11.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 black = "^23.1.0"
 factory-boy = "^3.2.1"
 faker = "^17.6.0"
 doit = "^0.36.0"
 pytest-cov = "^4.0.0"
 mypy = "^1.1.1"
 flake8 = "^6.0.0"
+testcontainers = "^3.7.1"
+tzdata = "^2023.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
 
+#[tool.coverage.run]
+#source = ["pydantic_dynamo"]
 
 [tool.mypy]
 python_version = 3.9
+plugins = "pydantic.mypy"
 warn_return_any = true
 warn_unused_configs = true
 show_error_codes = true
 
 [[tool.mypy.overrides]]
 module = [
+    "aioboto3",
     "boto3",
     "boto3.dynamodb.conditions",
     "botocore.response",
     "factory",
     "faker",
+    "testcontainers.core.container",
 ]
 ignore_missing_imports = true
```

### Comparing `pydantic_dynamo-0.1.5/setup.py` & `pydantic_dynamo-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,438 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pydantic-dynamo
+Version: 0.2.0
+Summary: 
+Home-page: https://github.com/david-a-jetter/pydantic-dynamo
+Author: David Jetter
+Author-email: davidajetter@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aioboto3 (>=11.1.0,<12.0.0)
+Requires-Dist: boto3 (>=1.20.32,<2.0.0)
+Requires-Dist: botocore (>=1.23.32,<2.0.0)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['pydantic_dynamo']
+# pydantic-dynamo
+A Python repository over DynamoDB, leveraging the excellent 
+[Pydantic](https://docs.pydantic.dev/) library to model records.
 
-package_data = \
-{'': ['*']}
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-install_requires = \
-['boto3>=1.20.32,<2.0.0', 'botocore>=1.23.32,<2.0.0', 'pydantic>=1.10.5,<2.0.0']
-
-setup_kwargs = {
-    'name': 'pydantic-dynamo',
-    'version': '0.1.5',
-    'description': '',
-    'long_description': '# pydantic-dynamo\nA Python repository over DynamoDB leveraging the excellent \n[Pydantic](https://docs.pydantic.dev/) library to model records.\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n## Contributing\n\nPlease see [the contributing guide](./contributing.md).\n\n## Installation\nInstall from PyPI `pip install pydantic-dynamo`\n\nOr even better, use [Poetry](https://python-poetry.org/docs/) `poetry add pydantic-dynamo`\n\n## Usage\n\nThe intended usage of this package is a low-to-medium complexity application. You will lose\nsome benefits of the single-table pattern, specifically the ability to query\nand retrieve objects of different types in one connection. For most use cases except\nthe most complex examples, access patterns can be implemented to utilize the `list`/`list_between`\nand `get_batch` functions, documented below, to prevent N+1 queries.\n\nThis package assumes the specified table already exists and the application it is\nrunning from has sufficient access to the table.\n\nCurrently, the package requires the table be created with a partition key named \n`_table_item_id` and a sort key named `_table_content_id`.\n\nThe following IAM permissions are required:\n\n```yaml\n- dynamodb:BatchGetItem\n- dynamodb:BatchWriteItem\n- dynamodb:GetItem\n- dynamodb:PutItem\n- dynamodb:Query\n- dynamodb:UpdateItem\n```\n\n### Modeling\nCreate a Pydantic model specifically for storage. This should generally not be shared\nin API contracts or other external interfaces to adhere to single-responsibility principle.\n\n```python\nfrom pydantic import BaseModel\nfrom typing import Optional\n\nclass FilmActor(BaseModel):\n    id: str\n    name: str\n    review: Optional[str]\n    \n```\n\n### Instantiation\nThe repository configuration will dictate the prefix values used for the partition and sort\nkey attributes. Once data is saved, these values cannot be changed without losing\naccess to previously saved data.\n\n`partition_prefix` can be used to categorize data and potentially implement\nrow-based access control. See [DynamoDB docs](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/specifying-conditions.html)\nand [IAM Condition docs](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_elements_condition.html).\n**Access control in this manner is only theoretical right now and has not been fully tested.**\n\n`partition_name` is used in conjunction with the `partition_prefix`, with a `#` delimiter,\nto form the partition key value of items within the repository. Individual items can then be\nsaved with their own partition ID value to allow querying based on the sort key values only,\nor they can be saved without their own partition ID to allow querying across the entire \nrepository.\n\n`content_type` is used as the prefix of the sort key value. Typically, this should be set\nto the snake-cased version of the pydantic class name, eg: `movie_character`.\n\nIf all repositories are sharing a single table, it\'s important that each repository \nhas a different combination of the above three values to ensure that the data is segmented.\nYou can choose to point repositories to different tables, but managing capacity becomes\na more complicated problem, which is outside the scope of this library.\n\nThere are two ways to instantiate a repository instance:\n\nThrough the `build` method that will generate the boto3 session and table objects:\n\n```python\nfrom pydantic_dynamo.repository import DynamoRepository\nrepo = DynamoRepository[FilmActor].build(\n    table_name="dynamodb-table-name",\n    item_class=FilmActor,\n    partition_prefix="content",\n    partition_name="movies",\n    content_type="character",\n)\n```\n\nOr directly to the `__init__` if you want control over how the boto3 objects are created:\n\n```python\nfrom pydantic_dynamo.repository import DynamoRepository\nfrom boto3 import Session\n\nresource = Session().resource("dynamodb")\ntable = resource.Table("dynamodb-table-name")\n\nrepo = DynamoRepository[FilmActor](\n    item_class=FilmActor,\n    partition_prefix="content",\n    partition_name="movies",\n    content_type="character",\n    table=table,\n    resource=resource\n)\n```\n### Saving Data\n\nData is saved using an instance of the generic `PartitionedContent[ObjT]` class found in \n[models.py](./pydantic_dynamo/models.py). The `partition_ids` and `content_ids` are `List[str]`. \nEach value in the list is eventually concatenated, and prefixed with the repository\'s configured values.\n\nParticularly for the `content_ids` field, you can leverage this to achieve degrees of query-ability for\nmore complex use cases, eg: `content_ids=["usa", "ny", "saratoga", "12020"]` will result in a \nsort key value of `usa#ny#saratoga#12020` that can be efficiently queried with DynamoDB\'s `begins_with`\ncondition, utilized in this library\'s `list` function.\n\nIt\'s wise to ensure that any values being used in the partition and content IDs are also retained as \nfields on the model object as well, which will make updates easier to perform.\n\n#### Put Single Item\n\nThis is logically similar to the DynamoDB Put operation, and will overwrite an existing item with \nidentical partition and content IDs.\n\n```python\nfrom pydantic_dynamo.models import PartitionedContent\nfrom uuid import uuid4\n\nid1 = str(uuid4())\nactor1 = FilmActor(id=id1, name="Daniel Day-Lewis")\n\nrepo.put(\n    PartitionedContent[FilmActor](\n        partition_ids=[], content_ids=[id1], item=actor1\n    )\n)\n```\n\n#### Put Multiple Items\n\nWhen saving more than one item, you can use a batch operation that will utilize DynamoDB\'s `write_batch` \noperation, which will more efficiently buffer data and minimize the total number of network calls compared to calling\n`put` in a loop.\n\n```python\nfrom pydantic_dynamo.models import PartitionedContent\nfrom uuid import uuid4\n\nid1 = str(uuid4())\nactor1 = FilmActor(id=id1, name="Daniel Day-Lewis")\nid2 = str(uuid4())\nactor2 = FilmActor(id=id2, name="Steve Buscemi")\n\n\nrepo.put_batch(\n    (\n        PartitionedContent[FilmActor](\n            partition_ids=[], content_ids=[id1], item=actor1\n        ),\n        PartitionedContent[FilmActor](\n            partition_ids=[], content_ids=[id2], item=actor2\n        ),\n    )\n)\n```\n\n#### Update an item\n\nNB: Please review the limitation in [issue #1](https://github.com/david-a-jetter/pydantic-dynamo/issues/1)\n\nUpdates are handled in a somewhat more complex and manual manner using an `UpdateCommand` object. \nSince this is constructed by sending `Dict[str, Any]`, dictionary entries are validated against\nthe pydantic model\'s schema before sending data to DynamoDB.\n\n`set_commands` can be used to map attributes\' names to a new value.\n`increment_attrs` can be used to increment attributes\' current values by some integer.\n`append_attrs` can be used to extend a `List` attribute\'s values\n\n`current_version` can be used to enforce a check on the object\'s version number to\nadhere to an object versioning pattern. Since there isn\'t a way the repo currently returns\nand object\'s version, this is not useful at the moment but is an experiment in progress.\n\n\n```python\nfrom pydantic_dynamo.models import UpdateCommand\n\nrepo.update(\n    partition_id=None,\n    content_id=[id1],\n    command=UpdateCommand(\n        set_commands={"review": "Talented, but unfriendly in Gangs of New York"}\n    )\n)\n\n```\n\n### Reading Data\n\n#### Get Item\n\nFinally, something simple to document. This gets a single item by its partition and content IDs,\nreturning `None` if no item is found.\n\nThis example would retrieve just the first actor item.\n```python\nfrom typing import Optional\n\nitem: Optional[FilmActor] = repo.get(partition_id=None, content_id=[id1])\n```\n\n#### Get Multiple Items\n\nThis leverages DynamoDB\'s `batch_get_item` API to collect multiple items by their partition and content IDs.\nThis is often useful after having collected a previous set of records that have potentially related\nitems that you want to retrieve, and then associate the two in a subsequent mapping logic layer.\n\nThis example would retrieve both actor items in a single network request.\n```python\nfrom typing import List\n\nitems: List[FilmActor] = repo.get_batch([(None, [id1]), (None, [id2])])\n\n```\n\n#### Listing Items\nThe following two functions leverage DynamoDB\'s `query` API and offers the ability \nto filter on content ID values, change sort order, limit the quantity of items. \n\nNB: These returns an `Iterator` type, which will not execute any query until it begins iteration.\n\nYou may also pass an optional `FilterCommand` to filter on non-key attributes. All fields\non this object are optional, and are applied utilizing `and` logic.\n\n\n```python\nfrom pydantic_dynamo.models import FilterCommand\n\n# Find actors without a `review` attribute\nfilter1 = FilterCommand(\n    not_exists={"review"}\n)\n\n# Find actors who are talented but unfriendly in Gangs of New York\nfilter2 = FilterCommand(\n    equals={"review": "Talented, but unfriendly in Gangs of New York"}\n)\n\n# Find actors who are not talented but unfriendly in Gangs of New York\nfilter3 = FilterCommand(\n    not_equals={"review": "Talented, but unfriendly in Gangs of New York"}\n)\n\n```\n\n##### List\nThis function supports filter items with a `begins_with` filter on their content IDs.\n\nThis example would retrieve all actor items.\n```python\nfrom typing import Iterator\n\nitems: Iterator[FilmActor] = repo.list(\n    partition_id=None,\n    content_prefix=None,\n    sort_ascending=True, # default order by sort key value\n    limit=None,\n    filters=None\n)\n```\n\n##### List Between\nThis function supports filter items with a `between` filter on their content IDs.\n\nNB: If `content_start == content_end` this will revert to calling `list` using `begins_with`.\n\nThis example would retrieve all actor items. It\'s a lame example and should be updated\nwith something more interesting. A common use case is to include an ISO-formatted datetime\nvalue at the end of a content ID, and you can retrieve all values in a given partition\nbetween two specified datetimes.\n```python\nfrom typing import Iterator\n\nitems: Iterator[FilmActor] = repo.list_between(\n    partition_id=None,\n    content_start=None,\n    content_end=None,\n    sort_ascending=True, # default order by sort key value\n    limit=None,\n    filters=None\n)\n\n```\n',
-    'author': 'David Jetter',
-    'author_email': 'davidajetter@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/david-a-jetter/pydantic-dynamo',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+## Contributing
 
+Please see [the contributing guide](./contributing.md).
+
+## Installation
+Install from PyPI:
+```
+pip install pydantic-dynamo
+```
+
+Or even better, use [Poetry](https://python-poetry.org/docs/):
+```
+poetry add pydantic-dynamo
+```
+
+## Usage
+
+The ideal consumer a developer of a low-to-medium complexity application. You will lose
+some benefits of the single-table pattern, specifically the ability to query
+and retrieve objects of different types in a single connection. Except the most complex single-table examples, 
+access patterns can be implemented to utilize the `list`/`list_between`
+and `get_batch` functions, documented below, to prevent N+1 queries and provide sufficient performance.
+
+
+### Table Creation
+
+This package assumes the specified table already exists and the application it is
+running from has sufficient access to the table.
+
+The following IAM permissions are required:
+
+```yaml
+- dynamodb:BatchGetItem
+- dynamodb:BatchWriteItem
+- dynamodb:GetItem
+- dynamodb:PutItem
+- dynamodb:Query
+- dynamodb:UpdateItem
+```
+
+### Modeling
+Create a Pydantic model specifically for storage. This should generally not be shared
+in API contracts or other external interfaces to adhere to single-responsibility principle.
+
+```python
+from pydantic import BaseModel
+from typing import Optional
+
+class FilmActor(BaseModel):
+    id: str
+    name: str
+    review: Optional[str]
+    
+```
+
+#### Reserved Attribute Names
+This package implicitly uses the following attributes, and therefore they should not be used in any
+object model classes.
+
+| Attribute            | Usage                                                                                                                   |
+|----------------------|-------------------------------------------------------------------------------------------------------------------------|
+| `_table_item_id`     | Default Partition Key name, can be overridden in repository instantiation. *Not a default in v2*                        |
+| `_table_content_id`  | Default Sort Key name, can be overridden in repository instantiation. *Not a default in v2*                             |
+| `_timestamp`         | Automatic ISO-formatted timestamp for when record was created or updated                                                |
+| `_object_version`    | Internal object versioning integer, automatically incremented on update, and can be used to enforce conditional updates |
+| `_ttl`               | Optionally used to store the DynamoDB TTL expiry value, which must be declared in the table's `TimeToLiveSpecification` |
+
+
+## Version 1 (Deprecated)
+The original repository implementation that still exists but will no longer receive updates.
+This will be removed in a future release.
+
+[V1 Documentation](./docs/v1.md) has been moved to keep the main README a reasonable size.
+
+## Version 2 (Experimental)
+This is the implementation that is intended for longer-term maintenance and will receive updates.
+
+### Instantiation
+V2 removes the `build` convenience function found in V1 and provides only a `__init__` constructor. Since V2 is async-first
+the table and resource objects need to be constructed from [aioboto3](https://aioboto3.readthedocs.io/en/latest/usage.html#dynamodb-examples)
+
+A working example can be found in the [integration tests conftest.py](./tests/test_integration/conftest.py)
+
+```python
+from aioboto3 import Session
+from pydantic_dynamo.v2.repository import DynamoRepository
+from tests.models import Example # Use your record model instead
+
+session = Session()
+boto3_kwargs = {"service_name": "dynamodb"} # endpoint_url, region_name, etc.
+async with session.resource(**boto3_kwargs) as resource:
+    repo = DynamoRepository[Example](
+        item_class=Example,
+        partition_prefix="test",
+        partition_name="integration",
+        content_type="example",
+        table_name="table_name",
+        partition_key="PARTITION_KEY",
+        sort_key="SORT_KEY",
+        table=await resource.Table("table_name"),
+        resource=resource,
+    )
+```
+
+There is also a synchronous variant that can be used if you don't want to work with async/await and async generators
+in your business code. Most of the subsequent documentation is focused on the async variant.
+
+```python
+from aioboto3 import Session
+from pydantic_dynamo.v2.repository import DynamoRepository
+from pydantic_dynamo.v2.sync_repository import SyncDynamoRepository
+from tests.models import Example # Use your record model instead
+
+session = Session()
+boto3_kwargs = {"service_name": "dynamodb"} # endpoint_url, region_name, etc.
+async with session.resource(**boto3_kwargs) as resource:
+    repo = DynamoRepository[Example](
+        item_class=Example,
+        partition_prefix="test",
+        partition_name="integration",
+        content_type="example",
+        table_name="table_name",
+        partition_key="PARTITION_KEY",
+        sort_key="SORT_KEY",
+        table=await resource.Table("table_name"),
+        resource=resource,
+    )
+
+    sync_repo = SyncDynamoRepository[Example](async_repo=repo)
+```
+### Saving Data
+
+Data is saved using an instance of the generic `PartitionedContent[ObjT]` class found in 
+[models.py](./pydantic_dynamo/models.py). The `partition_ids` and `content_ids` are `List[str]`. 
+Each value in the list is concatenated before saving, and prefixed with the repository's configured values.
+
+For the `content_ids` field, you can leverage this to achieve degrees of query-ability for
+more complex use cases, eg: `content_ids=["usa", "ny", "saratoga", "12020"]` will result in a 
+sort key value of `usa#ny#saratoga#12020` that can be efficiently queried with DynamoDB's `begins_with`
+condition, utilized in this library's `list` function.
+
+It's wise to ensure that any values being used in the partition and content IDs are also retained as 
+fields on the model object as well, which will make updates easier to perform. *This is less critical now
+since the V2 responses include reified `PartitionedContent[ObjT]` objects instead of just the modeled records in V1.*
+
+#### Put Single Item
+
+This leverages the DynamoDB Put operation, and will overwrite an existing item with identical partition and content IDs.
+
+```python
+from pydantic_dynamo.models import PartitionedContent
+from uuid import uuid4
+
+id1 = str(uuid4())
+actor1 = FilmActor(id=id1, name="Daniel Day-Lewis")
+
+await repo.put(
+    PartitionedContent[FilmActor](
+        partition_ids=[], content_ids=[id1], item=actor1
+    )
+)
+```
+
+#### Put Multiple Items
+
+When saving more than one item, you can use a batch operation that will utilize DynamoDB's `write_batch` 
+operation, which will more efficiently buffer data and minimize the total number of network calls compared to calling
+`put` in a loop.
+
+```python
+from pydantic_dynamo.models import PartitionedContent
+from uuid import uuid4
+
+id1 = str(uuid4())
+actor1 = FilmActor(id=id1, name="Daniel Day-Lewis")
+id2 = str(uuid4())
+actor2 = FilmActor(id=id2, name="Steve Buscemi")
+
+
+await repo.put_batch(
+    (
+        PartitionedContent[FilmActor](
+            partition_ids=[], content_ids=[id1], item=actor1
+        ),
+        PartitionedContent[FilmActor](
+            partition_ids=[], content_ids=[id2], item=actor2
+        ),
+    )
+)
+```
+
+#### Update an item
+
+NB: Please review the limitation in [issue #1](https://github.com/david-a-jetter/pydantic-dynamo/issues/1)
+
+Updates are handled in a somewhat more complex and manual manner using an `UpdateCommand` object. 
+Since this is constructed by sending `Dict[str, Any]`, dictionary entries are validated against
+the pydantic model's schema before sending data to DynamoDB.
+
+`set_commands` can be used to map attributes' names to a new value.
+`increment_attrs` can be used to increment attributes' current values by some integer.
+`append_attrs` can be used to extend a `List` attribute's values
+
+`current_version` can be used to enforce a check on the object's version number to
+adhere to an object versioning pattern. 
+
+
+```python
+from pydantic_dynamo.models import UpdateCommand
+
+await repo.update(
+    partition_id=None,
+    content_id=[id1],
+    command=UpdateCommand(
+        set_commands={"review": "Talented, but unfriendly in Gangs of New York"}
+    )
+)
+
+```
+
+
+### Reading Data
+
+#### Get Item
+
+Finally, something simple to document. This gets a single item by its partition and content IDs,
+returning `None` if no item is found.
+
+This example would retrieve just the first actor item.
+```python
+from typing import Optional
+from pydantic_dynamo.models import PartitionedContent
+
+item: Optional[PartitionedContent[FilmActor]] = await repo.get(partition_id=None, content_id=[id1])
+```
+
+#### Reading Multiple Items
+
+This and all subsequent read operations return `AsyncIterable[BatchResponse[ObjT]]` references. These cannot be directly awaited,
+but rather need to be iterated in an async loop. See [PEP-525](https://peps.python.org/pep-0525/) for details and this
+repository's tests for complete examples.
+
+Most DynamoDB batch operations implement a continuation token pattern, where the API will return a subset of the data
+that matches the parameters up to some stored size (eg. 1MB) and then includes a continuation token to use in a subsequent
+API call.
+
+A single `BatchResponse[ObjT]` represents one API response from DynamoDB, and contains an `Iterable[ObjT]` reference. This leaves
+you as the consumer in complete control whether you should lazily stream the records or project them all into a list.
+
+#### Get Batch by Key
+
+This leverages DynamoDB's `batch_get_item` API to collect multiple items by their partition and content IDs.
+This is often useful after having collected a previous set of records that have potentially related
+items that you want to retrieve, and then associate the two in a subsequent mapping logic layer.
+
+This example would retrieve both actor items in a single network request.
+```python
+from typing import List
+from pydantic_dynamo.models import PartitionedContent
+
+items: List[PartitionedContent[FilmActor]] = [
+    content 
+    async for response in repo.get_batch([(None, [id1]), (None, [id2])])
+    for content in response.contents                      
+]
+```
+
+#### Listing Items
+The following two functions leverage DynamoDB's `query` API and offers the ability 
+to filter on partial content ID values, change sort order, limit the quantity of items.
+
+These operations support optional kwargs: 
+* `limit` integer to cap the number of records returned
+* `sort_ascending` boolean to change sort order based on the sort key value, which defaults to `True`
+
+##### Filtering
+
+You may also pass an optional `FilterCommand` to filter on non-key attributes. All fields
+on this object are optional, and are applied utilizing `and` logic.
+
+```python
+from pydantic_dynamo.models import FilterCommand
+
+# Find actors without a `review` attribute
+filter1 = FilterCommand(
+    not_exists={"review"}
+)
+
+# Find actors who are talented but unfriendly in Gangs of New York
+filter2 = FilterCommand(
+    equals={"review": "Talented, but unfriendly in Gangs of New York"}
+)
+
+# Find actors who are not talented but unfriendly in Gangs of New York
+filter3 = FilterCommand(
+    not_equals={"review": "Talented, but unfriendly in Gangs of New York"}
+)
+
+```
+
+These operations are more interesting with a more complex data model, so let's pretend there might be 
+more than one opinion on a given actor, so we'll store many reviews instead of just my own.
+
+Let's define a review model that can be related to an actor:
+```python
+from pydantic import BaseModel
+from datetime import datetime
+
+class ActorReview(BaseModel):
+    id: str
+    actor_id: str
+    created: datetime
+    review: str
+```
+
+and then pretend we save a few of them:
+
+```python
+from datetime import datetime, timezone
+from uuid import uuid4
+
+now = datetime.now(tz=timezone.utc)
+
+await repo.put_batch(
+    (
+        PartitionedContent[ActorReview](
+            partition_ids=[actor1.id],
+            content_ids=[now.isoformat()],
+            item=ActorReview(
+                id=str(uuid4()),
+                actor_id=actor1.id,
+                created=now,
+                review="I really thought he was the hero of this movie"
+            )
+        ),
+        PartitionedContent[ActorReview](
+            partition_ids=[actor1.id],
+            content_ids=[now.isoformat()],
+            item=ActorReview(
+                id=str(uuid4()),
+                actor_id=actor1.id,
+                created=now,
+                review="He really embodies the New York state of mind"
+            )
+        )
+    )
+)
+```
+
+##### List
+This function supports filter items with a `begins_with` filter on their content IDs.
+
+This example would retrieve all review items for `actor1` that we previously saved.
+```python
+from typing import List
+from pydantic_dynamo.models import PartitionedContent
+
+items: List[PartitionedContent[ActorReview]] = [
+    content
+    async for response in repo.list(
+        partition_id=[actor1.id],
+        content_prefix=None,
+        sort_ascending=True,
+        limit=None,
+        filters=None
+    )
+    for content in response.contents
+]
+```
+
+This example would retrieve all of the reviews created on a given year, because ISO-formatted datetime
+values are lexicographically sortable.
+```python
+from typing import List
+from pydantic_dynamo.models import PartitionedContent
+
+items: List[PartitionedContent[ActorReview]] = [
+    content
+    async for response in repo.list(
+        partition_id=[actor1.id],
+        content_prefix=["2023"],
+        sort_ascending=True,
+        limit=None,
+        filters=None
+    )
+    for content in response.contents
+]
+```
+
+##### List Between
+This function supports filter items with a `between` filter on their content IDs.
+
+NB: If `content_start == content_end` this will revert to calling `list` using `begins_with`. This prevents
+unexpected behavior of returning no records due to how Dynamo's Query API handles `between` conditions.
+
+This example would retrieve all reviews for actor1 that were created in or after January 2023 *and* in or before March 2023.
+```python
+from typing import List
+from pydantic_dynamo.models import PartitionedContent
+
+items: List[PartitionedContent[[FilmActor]] = [
+    content
+    async for response in repo.list_between(
+        partition_id=[actor1.id],
+        content_start=["2023-01"],
+        content_end=["2023-04"],
+        sort_ascending=True,
+        limit=None,
+        filters=None
+    )
+    for content in response.contents
+]
+```
 
-setup(**setup_kwargs)
```

