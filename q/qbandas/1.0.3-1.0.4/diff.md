# Comparing `tmp/qbandas-1.0.3.tar.gz` & `tmp/qbandas-1.0.4.tar.gz`

## Comparing `qbandas-1.0.3.tar` & `qbandas-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,15 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 qbandas-1.0.3/requirements.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 qbandas-1.0.3/setup.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 qbandas-1.0.3/src/qbandas/__init__.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 qbandas-1.0.3/src/qbandas/__main__.py
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 qbandas-1.0.3/src/qbandas/config.py
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 qbandas-1.0.3/src/qbandas/pack.py
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 qbandas-1.0.3/src/qbandas/schema.py
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 qbandas-1.0.3/src/qbandas/upload.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 qbandas-1.0.3/src/qbandas/util.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 qbandas-1.0.3/test/data.csv
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 qbandas-1.0.3/test/test.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 qbandas-1.0.3/test/schemas/Example Table.json
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 qbandas-1.0.3/test/schemas/bs397hfuy.json
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 qbandas-1.0.3/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 qbandas-1.0.3/LICENSE
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 qbandas-1.0.3/README.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 qbandas-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 qbandas-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qbandas-1.0.4/requirements.txt
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/__init__.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/__main__.py
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/headers.py
+-rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/pack.py
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/schema.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/test_headers.py
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/upload.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/util.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/data/field_types.json
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 qbandas-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 qbandas-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 qbandas-1.0.4/README.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 qbandas-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 qbandas-1.0.4/PKG-INFO
```

### Comparing `qbandas-1.0.3/src/qbandas/schema.py` & `qbandas-1.0.4/qbandas/schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,163 +1,167 @@
 """
 Methods that deal with resolving the structure of local and remote (QuickBase) tables.
 """
+import json
+import os
+from os.path import exists, join
+from pathlib import Path
+from typing import NoReturn
 
-import json, requests, os
+import requests
 
-def pull_schema(DBID: str, **kwargs) -> None:
+from . import headers
+
+
+def pull(DBID: str, directory: Path|str = None, **kwargs) -> NoReturn:
     """
-    Download a local copy of a table's structure from a QuickBase application.
+    Download a local copy of a table's structure from a QuickBase 
+    application.
 
-    This operation is authorized by `./headers.json`. The schema will be placed into `./schemas/` where other qBandas operations can use it. 
+    This operation is authorized by `./headers.json`. The schema will be
+    placed into `./schemas/` where other qBandas operations can use it. 
 
     Parameters
     ----------
     DBID : str
         The unique identifier of the table in QuickBase.
+    directory : None | Path | str
+        The directory to use for this operation. Default is current
+
+    Examples
+    --------
+    >>> import qbandas
+    >>> # qbandas.schema.pull('bb7f543') # unauthorized
+
     """
-    # Can set the directory with dir=<dir>
-    dir = kwargs['dir'] if 'dir' in kwargs else os.getcwd()
+    directory = directory if directory else os.getcwd()  
+    if not os.path.isdir(directory):
+        raise FileNotFoundError(f'{directory = } is not a valid directory')
 
-    # resolve the headers
-    with open(os.path.join(dir, 'headers.json'), 'r') as f:
-            headers = json.load(f)
+    headers_ = headers.read(directory = directory)
 
     # send the request to quickbase
-    params = {
-        'tableId': DBID,
-        'includeFieldPerms': "false"
-    }
-    r = requests.get(
-        'https://api.quickbase.com/v1/fields', 
-        params = params, 
-        headers = headers
-    )
+    params = {'tableId': DBID, 'includeFieldPerms': "false"}
+    r = requests.get('https://api.quickbase.com/v1/fields', params = params, headers = headers_)
     r.raise_for_status()
 
     # convert the language in the api to user language
     type_conversion = {
         "timestamp": "datetime",
         "recordid": "numeric",
         "email": "email-address",
-        "phone": "phone-number"
-    }
+        "phone": "phone-number",
+        }
 
     address_subfields = {
         ": Street 1": 1,
         ": Street 2": 2,
         ": City": 3,
         ": State": 4,
         ": Zip": 5,
-        ": Country": 6
-    }
+        ": Country": 6,
+        }
 
     # parse the schema from the response
     schema = dict()
     schema['_DBID_'] = DBID
     for field in r.json():
 
         # address fields send extra unlabeled info that we cannot use. remove it
         if field['label'] in ['Street 1', 'Street 2', 'City', 'State/Region', 'Postal Code', 'Country']:
             continue
 
-        _type = field['fieldType']
-        if _type in type_conversion:
-            _type = type_conversion[_type]
+        type_ = field['fieldType']
+        if type_ in type_conversion:
+            type_ = type_conversion[type_]
         
-        schema[field['label']] = {
-            'id': field['id'],
-            'type': _type
-        }
+        schema[field['label']] = {'id': field['id'], 'type': type_}
 
         # recreate subfields for adresses with propper names
-        if _type == 'address':
+        if type_ == 'address':
             for sufix, fid_offset in address_subfields.items():
                 schema[field['label'] + sufix] = {
                     'id': field['id'] + fid_offset,
                     'type': "text"
                 }
 
-    # dump the schmea to disk
-    if not os.path.exists(os.path.join(dir, 'schemas')):
-        os.makedirs(os.path.join(dir, 'schemas'))
-    with open(os.path.join(dir, 'schemas', DBID + '.json'), 'w+') as f:
+    # dump the schema to disk
+    schemas_dir = join(directory, 'schemas')
+    if not exists(schemas_dir):
+        os.makedirs(schemas_dir)
+    with open(join(schemas_dir, DBID + '.json'), 'w') as f:
         json.dump(schema, f, indent=4)
     
         
-def add_args(schema_name: str, field: str, **kwargs):
+def add_args(schema_name: str, directory: Path|str = None, *args, **kwargs):
     """
-    Append new config options (args) for a field in a schema.
+    Append new config options (args) for fields in a schema.
 
     Parameters
     ----------
     schema_name : str
         The schema to modify.
-    field : str
-        This field will be configured.
+    directory : None | Path | str
+        The directory to use for this operation. Default is current
+    *args
+        These fields will be configured.
     **kwargs
         The arguments to add.
-
-    Examples
-    --------
-    ``` 
-    >>> import qbandas as qb
-    TODO
-    ```
+        
     """
 
-    # Can set the directory with dir=<dir>
-    dir = os.getcwd()
-    if 'dir' in kwargs:
-        dir = kwargs['dir']
-        del kwargs['dir']
+    directory = directory if directory else os.getcwd()  
+    if not os.path.isdir(directory):
+        raise FileNotFoundError(f'{directory = } is not a valid directory')
 
     # read in the schema
     file_name = schema_name + '.json'
-    with open(os.path.join(dir, 'schemas', file_name), 'r') as f:
+    with open(os.path.join(directory, 'schemas', file_name), 'r') as f:
         schema = json.load(f)
 
     # append the new arguments
-    if field not in schema:
-        raise Exception(f"The field {field} is not in the schema {schema_name}")
-    if 'args' not in schema[field]:
-        schema[field]['args'] = kwargs
-    else:
-        schema[field]['args'] = schema[field]['args'] | kwargs
+    for field in args:
+        if field not in schema:
+            raise Exception(f"The field {field} is not in the schema {schema_name}")
+        if 'args' not in schema[field]:
+            schema[field]['args'] = kwargs
+        else:
+            schema[field]['args'] = schema[field]['args'] | kwargs
 
     # put the schema pack into the file
-    with open(os.path.join(dir, 'schemas', file_name), 'w') as f:
+    with open(join(directory, 'schemas', file_name), 'w') as f:
         json.dump(schema, f, indent=4)
 
-def set_args(schema_name: str, field: str, **kwargs):
+def set_args(schema_name: str, directory: Path|str = None, *args, **kwargs):
     """
-    Set the config options (args) for a field in a schema.
+    Set the config options (args) for fields in a schema.
 
     Parameters
     ----------
     schema_name : str
         The schema to modify.
-    field : str
-        This field will be configured.
+    directory : None | Path | str
+        The directory to use for this operation. Default is current
+    *args
+        These fields will be configured.
     **kwargs
         The arguments to add.
     """
 
-    # Can set the directory with dir=<dir>
-    dir = os.getcwd()
-    if 'dir' in kwargs:
-        dir = kwargs['dir']
-        del kwargs['dir']
-
+    directory = directory if directory else os.getcwd()  
+    if not os.path.isdir(directory):
+        raise FileNotFoundError(f'{directory = } is not a valid directory')
+    
     # read in the schema
     file_name = schema_name + '.json'
-    with open(os.path.join(dir, 'schemas', file_name), 'r') as f:
+    with open(os.path.join(directory, 'schemas', file_name), 'r') as f:
         schema = json.load(f)
 
     # set the arguments
-    if field not in schema:
-        raise Exception(f"The field {field} is not in the schema {schema_name}")
-    schema[field]['args'] = kwargs
+    for field in args:
+        if field not in schema:
+            raise Exception(f"The field {field} is not in the schema {schema_name}")
+        schema[field]['args'] = kwargs
 
     # put the schema pack into the file
-    with open(os.path.join(dir, 'schemas', file_name), 'w') as f:
+    with open(os.path.join(directory, 'schemas', file_name), 'w') as f:
         json.dump(schema, f, indent=4)
```

### Comparing `qbandas-1.0.3/src/qbandas/upload.py` & `qbandas-1.0.4/qbandas/upload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,109 +1,129 @@
 """
-Functions that deal with sending records or information to a Quickbase application.
+Functions that deal with sending records or information to a Quickbase 
+application.
 """
 
-import requests, json, os
+import json
+import os
 from functools import partial
+from os.path import join
+from pathlib import Path
+from typing import NoReturn
 
 import pandas as pd
+import requests
 
-from .config import field_types
+from . import FIELD_TYPES, headers
 
-def upload_records(df: pd.DataFrame, table_name: str, **kwargs): 
+
+def records(df: pd.DataFrame, table_name: str, directory: Path|str = None,
+            **kwargs) -> NoReturn: 
     """
     Send a table of records (rows) to a table on QuickBase.
 
-    If no errors are thrown, the data was successfully uploaded to QuickBase. If an error occurs when sending the data, it is possible that only _some_ of your records will have been uploaded to QuickBase. If that is an issue, please fix the data, and send it all again.
+    If no errors are thrown, the data was successfully uploaded to 
+    QuickBase. If an error occurs when sending the data, it is possible 
+    that only _some_ of your records will have been uploaded to 
+    QuickBase. If that is an issue, please fix the data, and send it 
+    all again.
 
     Parameters
     ----------
     df : pd.DataFrame
         The table of records
     table_name : str
-        Identifies which table to send the data to. You should use `pull_schema()` to create a valid `table_name`.
+        Identifies which table to send the data to. You should use 
+        `pull_schema()` to create a valid `table_name`.
+    directory : None | Path | str
+        The directory to use for this operation. Default is current
     """
 
-    debug = 'debug' in kwargs and kwargs['debug']
+    # enable debugging print statements
+    debug = kwargs.get('debug')
     if debug:
         from .util import str_dict, str_resp
         print(df.head())
     
-
-    # setup: read in the headers and the schema
-    # Can set the directory with dir=<dir>, defaults to .
-    dir = kwargs['dir'] if 'dir' in kwargs else os.getcwd()
-    with open(os.path.join(dir, 'headers.json'), 'r') as f:
-            headers = json.load(f)
-    with open(os.path.join(dir, 'schemas', table_name+'.json'), 'r') as f:
-            schema = json.load(f)
+    directory = directory if directory else os.getcwd()  
+    if not os.path.isdir(directory):
+        raise FileNotFoundError(f'{directory = } is not a valid directory')
+    
+    headers_ = headers.read(directory = directory)
+    with open(join(directory, 'schemas', f'{table_name}.json'), 'r') as f:
+        schema = json.load(f)
 
     if debug:
-        print(str_dict(headers))
+        print(str_dict(headers_))
         print(str_dict(schema))
 
     # Check that the columns in the df match the schema
-    if 'drop' not in kwargs or not kwargs['drop']:
+    if not kwargs.get('drop'):
         unknown_columns = [] # columns in df that aren't in schema
         for column in df.columns:
             if column not in schema.keys():
                 unknown_columns.append(column)
         if unknown_columns:
-            raise Exception(f"The following columns from your dataframe have no matching column in the specified QuickBase table. If you want to drop these columns (not send their data), add `drop=True` to this function call. Columns: " + ', '.join(unknown_columns))
+            raise Exception(f"The following columns from your dataframe have \
+                            no matching column in the specified QuickBase \
+                            table. If you want to drop these columns (not \
+                            send their data), add `drop=True` to this function \
+                            call. Columns: " + ', '.join(unknown_columns))
     
     # pack all the values into qb's crazy formats
     packed_df = pd.DataFrame()
     for col in df.columns:
 
         if col not in schema: # dropped columns
             continue
 
         col_info = schema[col]
         col_type = col_info['type']
         col_kwargs = col_info['args'] if 'args' in col_info else {}
 
-        # Magic lines! Get the related parsing function from config, create a partial of it with the given column arguments, apply it to a copy of the current column, and save it in the output
         try:
-            packing_func = field_types[col_type].packing_func
-            packed_df[col] = df[col].copy().apply(partial(packing_func, **col_kwargs))
+            # get the packing function and apply it
+            packing_func = partial(FIELD_TYPES[col_type]['pack'], **col_kwargs)
+            packed_df[col] = df[col].copy().apply(packing_func)
         except Exception as e:
-            e.args = (f"Failed parsing column '{col}' with column type '{col_type}' and arguments '{col_kwargs}'", *e.args)
+            e.args = (f"Failed parsing column '{col}' with column type \
+                      '{col_type}' and arguments '{col_kwargs}'", *e.args)
             raise
 
     if debug:
         print(packed_df.head())
 
     # grab the feild ids from schema, rename columns 
-    fids = {k:v['id'] for k,v in schema.items() if k != '_DBID_' and k in packed_df.columns}
+    fids = {k: v['id'] for k, v in schema.items() if \
+            k != '_DBID_' and k in packed_df.columns}
     renamed_df = packed_df.copy().rename(columns=fids) 
 
-    # Convert each row to a dictonary, drop keys with null values, create the list of records
     def _row_to_dict(row):
-        "Convert a row into a dictonary"
+        '''Convert a row into a dictonary and drop nulls'''
         row = dict(row)                                         
         return {k: v for k, v in row.items() if not pd.isna(v)} 
     records = list(renamed_df.apply(_row_to_dict, axis=1)) 
 
     if debug:
         print(str_dict(records[:5]))
 
-     # setup destination information
+    # setup destination information
     body = {"to": schema['_DBID_']}
 
     # look for optinal arguments to include from kwargs
     for option in ["fieldsToReturn", 'mergeFieldId']:
         if option in kwargs:
             body[option] = kwargs[option]
 
     # send the data one batch a time
     batch_size = kwargs["Payload-Size"] if "Payload-Size" in kwargs else 20_000
     for i in range(0, len(records), batch_size):
         body["data"] = records[i:i+batch_size]
         r = requests.post(
             'https://api.quickbase.com/v1/records', 
-            headers = headers, 
+            headers = headers_, 
             json = body
         )
         if debug:
             print(str_resp(r))
         r.raise_for_status()
```

### Comparing `qbandas-1.0.3/src/qbandas/util.py` & `qbandas-1.0.4/qbandas/util.py`

 * *Files identical despite different names*

### Comparing `qbandas-1.0.3/LICENSE` & `qbandas-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qbandas-1.0.3/README.md` & `qbandas-1.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-# qBandas
-
-qBandas (QuickBase + Pandas) is a Python package designed to effeciently transfer tabular data between QuickBase applications and the popular Python data handling library Pandas. If you are new to Pandas, you can read more about it [here](https://pandas.pydata.org/).
-
-The advantages of this approach over a QuickBase pipeline are:
-* Access to databases through Python libraries like [pyodbc](https://github.com/mkleehammer/pyodbc) and [SASPy](https://sassoftware.github.io/saspy/).
-* Greater control over features like error logging, data processing, automated reporting, and scheduling.
-* Significantly less performance impact on your QuickBase application.
-* Access tabular data from local sources. 
-* Coming in v1.1.0: Use SQL to pull data from your QuickBase app.
-
-The disadvantages of this approach compared to a pipeline are:
-* Requires knowledge of Python and Pandas.
-
-## Setup
-
-To use this library, simply get it from pypi. First, update your pip, then install qBandas 
-
-
-```bash
-python3 -m pip install --upgrade pip
-python3 -m pip install qbandas
-```
-
-You can now use it through import.
-
-```python
-import qbandas as qb
-```
-
-## Getting Started
-
-To show you the ropes, I will do a walkthrough of uploading a DataFrame to QuickBase. If you are new to Python or Pandas, it might be a good idea to follow along with this example before you try to deploy this yourself. Unfortunately, there are no example QuickBase apps to send data to, but everything else is doable.
-
-### 1) Get Your Data
-
-Read your tabular data into Python. The method you use for this is up to you. This step is one of the greatest strenghts of this method compared to a pipeline. I will simply hardcode mine. 
-
-```python
-import pandas as pd
-
-data = {
-  "name": ['John', 'Michael', 'Jill'],
-  "age": [50, 40, 45],
-  "phone": ["(555) 123-456", "(123) 999-4321", "(675) 555-1234x777"]
-}
-
-df = pd.DataFrame(data) # my data is in df
-```
-
-### 2) Gathering QuickBase Information - `headers.json`
-
-You will need to provide credentials in the form of a `headers.json` file in the working directory of your project. You can automaitically generate a template for the file by running the following
-
-```bash
-python -m qbandas --head
-```
-
-Fill in the header information. Some explanations are provided below.
-
-```json
-{
-    "QB-Realm-Hostname": "{QB-Realm-Hostname}",
-    "User-Agent": "{User-Agent}",
-    "Authorization": "{Authorization}"
-}
-```
-
-* `"QB-Realm-Hostname"` 
-    - Something like `"example.quickbase.com"`
-* `"User-Agent"`
-    - A name to identify yourself in the app logs. Can be anything.
-* `"Authorization"` 
-    - This is typically a QuickBase user token. Learn how to get one [here](https://developer.quickbase.com/auth).
-
-### 3) Creating a Schema
-
-Once you have the `headers.json` file you can make a schema for your destination table. You will need the table's `DBID`; this is the hash that comes after `/db/` in any QuickBase url. Each table has a unique identifier, and they can be found by visiting the table on the web. Run the Python command below replacing `"dbid"` with your table's `DBID`.
-
-```python
-qb.pull_schema("dbid")
-```
-
-### 4) Sending the Data
-
-You are all set! You can send data to your app now.
-
-```python 
-qb.upload_records(df, "dbid")
+Metadata-Version: 2.1
+Name: qbandas
+Version: 1.0.4
+Summary: Integrates the popular data handling library Pandas and the QuickBase API
+Project-URL: Homepage, https://github.com/jhopwood-jjk/qBandas
+Author: Joshua Hopwood
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+# qBandas
+
+qBandas (QuickBase + Pandas) is a Python package designed to effeciently transfer tabular data between QuickBase applications and the popular Python data handling library Pandas. If you are new to Pandas, you can read more about it [here](https://pandas.pydata.org/).
+
+The advantages of this approach over a QuickBase pipeline are:
+* Access to databases through Python libraries like [pyodbc](https://github.com/mkleehammer/pyodbc) and [SASPy](https://sassoftware.github.io/saspy/).
+* Greater control over features like error logging, data processing, automated reporting, and scheduling.
+* Significantly less performance impact on your QuickBase application.
+* Access tabular data from local sources. 
+* Coming in v1.1.0: ~~Use SQL to pull data from your QuickBase app.~~ Easily pull data from a QuickBase app.
+
+The disadvantages of this approach compared to a pipeline are:
+* Requires some knowledge of Python and Pandas.
+
+## Setup
+
+To use this library, simply get it from pypi. First, update your pip, then install qBandas 
+
+
+```bash
+python -m pip install -U pip qbandas
+```
+
+You can now use it through import.
+
+```python
+import qbandas
+```
+
+## Getting Started
+
+To show you the ropes, I will demo a walkthrough of uploading a DataFrame to QuickBase. 
+
+### 1) Get Your Data
+
+Read your tabular data into Python. The method you use for this is up to you. This step is one of the greatest strenghts of this method compared to a pipeline as you can get your data from anywher. 
+
+```python
+import pandas as pd
+
+data = {
+  "name": ['John', 'Michael', 'Jill'],
+  "age": [50, 40, 45],
+  "phone": ["(555) 123-456", "(123) 999-4321", "(675) 555-1234x777"]
+}
+
+df = pd.DataFrame(data) # my data is in df
+```
+
+### 2) Gathering QuickBase Information
+
+You will need to provide credentials in the form of a `headers.json` file. This file is used to authenticate requests to the QuickBase API. You can create the file by running the following. 
+
+```python
+qbandas.headers.create(interactive = True, repair = True)
+```
+
+### 3) Getting a Schema
+
+__What is this an why do I have to do it?__ \
+Schemas are just META data bout a table. qBandas uses locally stored schemas to automatically handle data formatting for you. The QuickBase API has strict rules about how the data should be delivered, so we need to "ask" the API ahead of time for a schema *before* we can send any data. 
+
+All you will need is the table's `DBID`; this is the hash that comes after `/db/` in any QuickBase url.  
+
+```python
+qbandas.schema.pull("dbid")
+```
+
+You should see that a `./schemas/` directory was created with one file in it. I recommend that you rerun the schema pull anytime your QuickBase table adds, removes, or modifies its fields __not__ its records. 
+
+### 4) Sending the Data
+
+You are all set! You can send data to your app now.
+
+```python 
+qbandas.upload.records(df, "dbid")
 ```
```

### Comparing `qbandas-1.0.3/pyproject.toml` & `qbandas-1.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
-00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
-00000020: 6368 6c69 6e67 222c 2022 7061 6e64 6173  chling", "pandas
-00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
-00000040: 6420 3d20 2268 6174 6368 6c69 6e67 2e62  d = "hatchling.b
-00000050: 7569 6c64 220d 0a0d 0a5b 7072 6f6a 6563  uild"....[projec
-00000060: 745d 0d0a 6e61 6d65 203d 2022 7162 616e  t]..name = "qban
-00000070: 6461 7322 0d0a 7665 7273 696f 6e20 3d20  das"..version = 
-00000080: 2231 2e30 2e33 220d 0a61 7574 686f 7273  "1.0.3"..authors
-00000090: 203d 205b 0d0a 2020 7b20 6e61 6d65 3d22   = [..  { name="
-000000a0: 4a6f 7368 7561 2048 6f70 776f 6f64 2220  Joshua Hopwood" 
-000000b0: 7d2c 0d0a 5d0d 0a64 6573 6372 6970 7469  },..]..descripti
-000000c0: 6f6e 203d 2022 496e 7465 6772 6174 6573  on = "Integrates
-000000d0: 2074 6865 2070 6f70 756c 6172 2064 6174   the popular dat
-000000e0: 6120 6861 6e64 6c69 6e67 206c 6962 7261  a handling libra
-000000f0: 7279 2050 616e 6461 7320 616e 6420 7468  ry Pandas and th
-00000100: 6520 5175 6963 6b42 6173 6520 4150 4922  e QuickBase API"
-00000110: 0d0a 7265 6164 6d65 203d 2022 5245 4144  ..readme = "READ
-00000120: 4d45 2e6d 6422 0d0a 7265 7175 6972 6573  ME.md"..requires
-00000130: 2d70 7974 686f 6e20 3d20 223e 3d33 2e37  -python = ">=3.7
-00000140: 220d 0a63 6c61 7373 6966 6965 7273 203d  "..classifiers =
-00000150: 205b 0d0a 2020 2020 2250 726f 6772 616d   [..    "Program
-00000160: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000170: 2050 7974 686f 6e20 3a3a 2033 222c 0d0a   Python :: 3",..
-00000180: 2020 2020 224c 6963 656e 7365 203a 3a20      "License :: 
-00000190: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-000001a0: 4d49 5420 4c69 6365 6e73 6522 2c0d 0a20  MIT License",.. 
-000001b0: 2020 2022 4f70 6572 6174 696e 6720 5379     "Operating Sy
-000001c0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-000001d0: 656e 6465 6e74 222c 0d0a 5d0d 0a0d 0a5b  endent",..]....[
-000001e0: 7072 6f6a 6563 742e 7572 6c73 5d0d 0a22  project.urls].."
-000001f0: 486f 6d65 7061 6765 2220 3d20 2268 7474  Homepage" = "htt
-00000200: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000210: 6a68 6f70 776f 6f64 2d6a 6a6b 2f71 4261  jhopwood-jjk/qBa
-00000220: 6e64 6173 220d 0a                        ndas"..
+00000010: 7265 7175 6972 6573 203d 205b 0d0a 2020  requires = [..  
+00000020: 2268 6174 6368 6c69 6e67 222c 200d 0a20  "hatchling", .. 
+00000030: 2022 7061 6e64 6173 3d3d 312e 342e 3322   "pandas==1.4.3"
+00000040: 2c0d 0a20 2022 7265 7175 6573 7473 3d3d  ,..  "requests==
+00000050: 322e 3238 2e31 220d 0a20 205d 0d0a 6275  2.28.1"..  ]..bu
+00000060: 696c 642d 6261 636b 656e 6420 3d20 2268  ild-backend = "h
+00000070: 6174 6368 6c69 6e67 2e62 7569 6c64 220d  atchling.build".
+00000080: 0a0d 0a5b 7072 6f6a 6563 745d 0d0a 6e61  ...[project]..na
+00000090: 6d65 203d 2022 7162 616e 6461 7322 0d0a  me = "qbandas"..
+000000a0: 7665 7273 696f 6e20 3d20 2231 2e30 2e34  version = "1.0.4
+000000b0: 220d 0a61 7574 686f 7273 203d 205b 0d0a  "..authors = [..
+000000c0: 2020 7b20 6e61 6d65 3d22 4a6f 7368 7561    { name="Joshua
+000000d0: 2048 6f70 776f 6f64 2220 7d2c 0d0a 5d0d   Hopwood" },..].
+000000e0: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
+000000f0: 496e 7465 6772 6174 6573 2074 6865 2070  Integrates the p
+00000100: 6f70 756c 6172 2064 6174 6120 6861 6e64  opular data hand
+00000110: 6c69 6e67 206c 6962 7261 7279 2050 616e  ling library Pan
+00000120: 6461 7320 616e 6420 7468 6520 5175 6963  das and the Quic
+00000130: 6b42 6173 6520 4150 4922 0d0a 7265 6164  kBase API"..read
+00000140: 6d65 203d 2022 5245 4144 4d45 2e6d 6422  me = "README.md"
+00000150: 0d0a 7265 7175 6972 6573 2d70 7974 686f  ..requires-pytho
+00000160: 6e20 3d20 223e 3d33 2e37 220d 0a63 6c61  n = ">=3.7"..cla
+00000170: 7373 6966 6965 7273 203d 205b 0d0a 2020  ssifiers = [..  
+00000180: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
+00000190: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001a0: 6e20 3a3a 2033 222c 0d0a 2020 2020 224c  n :: 3",..    "L
+000001b0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+000001c0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+000001d0: 6365 6e73 6522 2c0d 0a20 2020 2022 4f70  cense",..    "Op
+000001e0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+000001f0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+00000200: 222c 0d0a 5d0d 0a0d 0a5b 7072 6f6a 6563  ",..]....[projec
+00000210: 742e 7572 6c73 5d0d 0a22 486f 6d65 7061  t.urls].."Homepa
+00000220: 6765 2220 3d20 2268 7474 7073 3a2f 2f67  ge" = "https://g
+00000230: 6974 6875 622e 636f 6d2f 6a68 6f70 776f  ithub.com/jhopwo
+00000240: 6f64 2d6a 6a6b 2f71 4261 6e64 6173 22    od-jjk/qBandas"
```

