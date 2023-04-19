# Comparing `tmp/authomize-rest-api-client-3.1.5.tar.gz` & `tmp/authomize-rest-api-client-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-3.1.5.tar", last modified: Thu Apr 13 14:25:11 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-3.1.6.tar", last modified: Wed Apr 19 21:40:02 2023, max compression
```

## Comparing `authomize-rest-api-client-3.1.5.tar` & `authomize-rest-api-client-3.1.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2120 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2040 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10105 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    12633 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69815 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22617 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   183916 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63846 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-04-13 14:25:11.000000 authomize-rest-api-client-3.1.5/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-04-13 14:25:11.000000 authomize-rest-api-client-3.1.5/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 14:25:11.000000 authomize-rest-api-client-3.1.5/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      216 2023-04-13 14:25:11.000000 authomize-rest-api-client-3.1.5/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-13 14:25:11.000000 authomize-rest-api-client-3.1.5/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1163 2023-04-13 14:24:55.000000 authomize-rest-api-client-3.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10105 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    12633 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73155 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23487 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185133 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63873 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-04-19 21:40:02.000000 authomize-rest-api-client-3.1.6/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-04-19 21:40:02.000000 authomize-rest-api-client-3.1.6/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 21:40:02.000000 authomize-rest-api-client-3.1.6/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      216 2023-04-19 21:40:02.000000 authomize-rest-api-client-3.1.6/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-19 21:40:02.000000 authomize-rest-api-client-3.1.6/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-04-19 21:39:45.000000 authomize-rest-api-client-3.1.6/setup.py
```

### Comparing `authomize-rest-api-client-3.1.5/LICENSE.txt` & `authomize-rest-api-client-3.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.5/README.md` & `authomize-rest-api-client-3.1.6/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.5/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-3.1.6/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-04-13T14:20:13+00:00
+#   timestamp: 2023-04-19T21:29:38+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
@@ -234,39 +234,39 @@
         description='List of **invalid** target grouping ids.',
         title='Invalidtargetids',
     )
 
 
 class NewAccountsAssociationResponseSchema(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
-        None,
+        default=None,
         description='**The accepted time of the request**',
         title='Acceptedtimestamp',
     )
     requestId: str = Field(..., description='**Request id**', title='Requestid')
     numberOfAcceptedEntities: int = Field(
         ...,
         description='**The number of entities that pass validation and uploaded**',
         title='Numberofacceptedentities',
     )
     data: Optional[NewAccountsAssociationResponseDataSchema] = Field(
-        {}, description='Response data.', title='Data'
+        default={}, description='Response data.', title='Data'
     )
 
 
 class NewAccountsAssociationsListRequestSchema(BaseModel):
     data: List[NewAccountsAssociationRequestSchema] = Field(
         ...,
         description='New Accounts Associations',
         max_items=10000,
         min_items=1,
         title='Data',
     )
     validateOnly: Optional[bool] = Field(
-        False,
+        default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
     )
 
 
 class NewAssetInheritanceRequestSchema(BaseModel):
     sourceId: constr(min_length=1) = Field(
@@ -280,66 +280,70 @@
 
 
 class NewAssetRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ..., description='Asset ID. **Mandatory, must be unique.**\n', title='Uniqueid'
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The asset ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
     name: constr(min_length=1) = Field(
         ...,
         description='The name of the asset. The default is the Asset ID. **Mandatory**\n',
         title='Name',
     )
     type: Optional[AssetType] = Field(
-        'Other',
+        default='Other',
         description='The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   •\t`Application` (federation) \n   •\t`Database`\n   •\t`Drive`\n   •\t`File`\n   •\t`Folder`\n   •\t`GitRepository`\n   •\t`Integration`\n   •\t`Project`\n   •\t`Site`\n   •\t`Table`\n   •\t`Ticket`\n   •\t`VirtualMachine`\n   •\t`Other`\n\nIf the asset type does not exist use `Other`.\n',
     )
     originType: Optional[str] = Field(
-        None,
+        default=None,
         description='The asset type in the source system.\nThe default is the canonical type (if not mentioned).\n',
         title='Origintype',
     )
     createdAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description='The date (in ISO 8601 format) that the asset was created.\nThe default is `null`.\n',
         title='Createdat',
     )
     lastUsedAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description='The date (in ISO 8601 format) of the last time that the asset was in use.\nThe default is `null`.\n',
         title='Lastusedat',
     )
     description: Optional[str] = Field(
-        None,
+        default=None,
         description='A description of the asset (up to 512 characters).\n',
         title='Description',
     )
     href: Optional[str] = Field(
-        None, description='A link to the asset in the source system.\n', title='Href'
+        default=None,
+        description='A link to the asset in the source system.\n',
+        title='Href',
+    )
+    owner: Optional[str] = Field(
+        default=None, description='The owner ID', title='Owner'
     )
-    owner: Optional[str] = Field(None, description='The owner ID', title='Owner')
     tags: Optional[List[constr(min_length=1)]] = Field(
-        None, description='Tags associated with the asset.\n', title='Tags'
+        default=None, description='Tags associated with the asset.\n', title='Tags'
     )
 
 
 class NewAssetsInheritanceListRequestSchema(BaseModel):
     data: List[NewAssetInheritanceRequestSchema] = Field(
         ...,
         description='New Assets Inheritance',
         max_items=10000,
         min_items=1,
         title='Data',
     )
     validateOnly: Optional[bool] = Field(
-        False,
+        default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
     )
 
 
 class NewAssetsInheritanceResponseDataSchema(BaseModel):
     validSourceIds: List[str] = Field(
@@ -358,53 +362,53 @@
         description='List of **invalid** target assets ids.',
         title='Invalidtargetids',
     )
 
 
 class NewAssetsInheritanceResponseSchema(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
-        None,
+        default=None,
         description='**The accepted time of the request**',
         title='Acceptedtimestamp',
     )
     requestId: str = Field(..., description='**Request id**', title='Requestid')
     numberOfAcceptedEntities: int = Field(
         ...,
         description='**The number of entities that pass validation and uploaded**',
         title='Numberofacceptedentities',
     )
     data: Optional[NewAssetsInheritanceResponseDataSchema] = Field(
-        {}, description='Response data.', title='Data'
+        default={}, description='Response data.', title='Data'
     )
 
 
 class NewAssetsListRequestSchema(BaseModel):
     data: List[NewAssetRequestSchema] = Field(
         ..., description='New Assets', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
-        False,
+        default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
     )
 
 
 class NewAssetsResponseSchema(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
-        None,
+        default=None,
         description='**The accepted time of the request**',
         title='Acceptedtimestamp',
     )
     requestId: str = Field(..., description='**Request id**', title='Requestid')
     numberOfAcceptedEntities: int = Field(
         ...,
         description='**The number of entities that pass validation and uploaded**',
         title='Numberofacceptedentities',
     )
-    data: Optional[Any] = Field({}, description='Response data.', title='Data')
+    data: Optional[Any] = Field(default={}, description='Response data.', title='Data')
     validOwnerIds: List[str] = Field(
         ..., description='List of **valid** owner (user) ids.', title='Validownerids'
     )
     invalidOwnerIds: List[str] = Field(
         ...,
         description='List of **invalid** owner (user) ids.',
         title='Invalidownerids',
@@ -414,61 +418,65 @@
 class NewGroupingRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ...,
         description='\nGrouping ID. **Mandatory, must be unique.**\n',
         title='Uniqueid',
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The groupping ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
     name: constr(min_length=1) = Field(
         ...,
         description='The name of the grouping. The default is the ID field. **Mandatory**\n',
         title='Name',
     )
     originType: Optional[str] = Field(
-        None,
+        default=None,
         description='The name of the type of grouping in the source system. The default is `Group`. Example: Group/Alias/AWS Role\n',
         title='Origintype',
     )
     type: Optional[GroupingType] = Field(
-        'Group',
+        default='Group',
         description='Allowed values are `Group` and `VirtualGroup`.\n\nThe default is `Group`.\n\n`VirtualGroup` are mapped to the Authomize access explorer graph and are not present in other places in the user interface nor are they counted as a group.\n',
     )
     isRole: Optional[bool] = Field(
-        False,
+        default=False,
         description='If `Role`, the grouping represents a role in the source application and the name of the role is the grouping `name`.\n\nThe default is `False`.\n',
         title='Isrole',
     )
     anyoneCanJoinOrLeave: Optional[bool] = Field(
-        False,
+        default=False,
         description="Must be either `ture` or `false`.\nWhen set to `true` users can give themselves membership in this grouping without the grouping's managers' or owners' permission. \nExamples include public groups (M365), Google Groups with specific flags, ...\nValid only when `groupingType = Group`\n",
         title='Anyonecanjoinorleave',
     )
-    owner: Optional[str] = Field(None, description='The owner ID', title='Owner')
+    owner: Optional[str] = Field(
+        default=None,
+        description='The uniqueId of the user who is the "owner" (or manager) of the group.\n',
+        title='Owner',
+    )
     tags: Optional[List[constr(min_length=1)]] = Field(
-        None, description='Tags on the access grouping.\n', title='Tags'
+        default=None, description='Tags on the access grouping.\n', title='Tags'
     )
 
 
 class NewGroupingResponseSchema(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
-        None,
+        default=None,
         description='**The accepted time of the request**',
         title='Acceptedtimestamp',
     )
     requestId: str = Field(..., description='**Request id**', title='Requestid')
     numberOfAcceptedEntities: int = Field(
         ...,
         description='**The number of entities that pass validation and uploaded**',
         title='Numberofacceptedentities',
     )
-    data: Optional[Any] = Field({}, description='Response data.', title='Data')
+    data: Optional[Any] = Field(default={}, description='Response data.', title='Data')
     validOwnerIds: List[str] = Field(
         ..., description='List of **valid** owner (user) ids.', title='Validownerids'
     )
     invalidOwnerIds: List[str] = Field(
         ...,
         description='List of **invalid** owner (user) ids.',
         title='Invalidownerids',
@@ -507,68 +515,68 @@
         description='List of **invalid** target grouping ids.',
         title='Invalidtargetids',
     )
 
 
 class NewGroupingsAssociationResponseSchema(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
-        None,
+        default=None,
         description='**The accepted time of the request**',
         title='Acceptedtimestamp',
     )
     requestId: str = Field(..., description='**Request id**', title='Requestid')
     numberOfAcceptedEntities: int = Field(
         ...,
         description='**The number of entities that pass validation and uploaded**',
         title='Numberofacceptedentities',
     )
     data: Optional[NewGroupingsAssociationResponseDataSchema] = Field(
-        {}, description='Response data.', title='Data'
+        default={}, description='Response data.', title='Data'
     )
 
 
 class NewGroupingsAssociationsListRequestSchema(BaseModel):
     data: List[NewGroupingsAssociationRequestSchema] = Field(
         ...,
         description='New Groupings Associations',
         max_items=10000,
         min_items=1,
         title='Data',
     )
     validateOnly: Optional[bool] = Field(
-        False,
+        default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
     )
 
 
 class NewGroupingsListRequestSchema(BaseModel):
     data: List[NewGroupingRequestSchema] = Field(
         ..., description='New Groupings', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
-        False,
+        default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
     )
 
 
 class NewIdentityResponseSchema(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
-        None,
+        default=None,
         description='**The accepted time of the request**',
         title='Acceptedtimestamp',
     )
     requestId: str = Field(..., description='**Request id**', title='Requestid')
     numberOfAcceptedEntities: int = Field(
         ...,
         description='**The number of entities that pass validation and uploaded**',
         title='Numberofacceptedentities',
     )
-    data: Optional[Any] = Field({}, description='Response data.', title='Data')
+    data: Optional[Any] = Field(default={}, description='Response data.', title='Data')
 
 
 class NewPermissionsResponseDataSchema(BaseModel):
     validUserIds: List[str] = Field(
         ..., description='List of **valid** user ids.', title='Validuserids'
     )
     validGroupingIds: List[str] = Field(
@@ -594,26 +602,26 @@
         description='List of **invalid** privilege ids.',
         title='Invalidprivilegeids',
     )
 
 
 class NewPermissionsResponseSchema(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
-        None,
+        default=None,
         description='**The accepted time of the request**',
         title='Acceptedtimestamp',
     )
     requestId: str = Field(..., description='**Request id**', title='Requestid')
     numberOfAcceptedEntities: int = Field(
         ...,
         description='**The number of entities that pass validation and uploaded**',
         title='Numberofacceptedentities',
     )
     data: Optional[NewPermissionsResponseDataSchema] = Field(
-        {}, description='Response data.', title='Data'
+        default={}, description='Response data.', title='Data'
     )
 
 
 class NewPrivilegeGrantsRequestSchema(BaseModel):
     sourceId: constr(min_length=1) = Field(
         ..., description='ID of the source privilege. **Mandatory**\n', title='Sourceid'
     )
@@ -645,85 +653,85 @@
         description='List of **invalid** target privilege ids.',
         title='Invalidtargetids',
     )
 
 
 class NewPrivilegeGrantsResponseSchema(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
-        None,
+        default=None,
         description='**The accepted time of the request**',
         title='Acceptedtimestamp',
     )
     requestId: str = Field(..., description='**Request id**', title='Requestid')
     numberOfAcceptedEntities: int = Field(
         ...,
         description='**The number of entities that pass validation and uploaded**',
         title='Numberofacceptedentities',
     )
     data: Optional[NewPrivilegeGrantsResponseDataSchema] = Field(
-        {}, description='Response data.', title='Data'
+        default={}, description='Response data.', title='Data'
     )
 
 
 class NewPrivilegesGrantsListRequestSchema(BaseModel):
     data: List[NewPrivilegeGrantsRequestSchema] = Field(
         ...,
         description='New Privileges Grants',
         max_items=10000,
         min_items=1,
         title='Data',
     )
     validateOnly: Optional[bool] = Field(
-        False,
+        default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
     )
 
 
 class NewPrivilegesResponseSchema(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
-        None,
+        default=None,
         description='**The accepted time of the request**',
         title='Acceptedtimestamp',
     )
     requestId: str = Field(..., description='**Request id**', title='Requestid')
     numberOfAcceptedEntities: int = Field(
         ...,
         description='**The number of entities that pass validation and uploaded**',
         title='Numberofacceptedentities',
     )
-    data: Optional[Any] = Field({}, description='Response data.', title='Data')
+    data: Optional[Any] = Field(default={}, description='Response data.', title='Data')
 
 
 class NewRestApiConnectorSchema(BaseModel):
-    config: Optional[Dict[str, Any]] = Field(None, title='Config')
+    config: Optional[Dict[str, Any]] = Field(default=None, title='Config')
     serviceId: constr(min_length=1) = Field(..., title='Serviceid')
 
 
 class NewUserResponseSchema(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
-        None,
+        default=None,
         description='**The accepted time of the request**',
         title='Acceptedtimestamp',
     )
     requestId: str = Field(..., description='**Request id**', title='Requestid')
     numberOfAcceptedEntities: int = Field(
         ...,
         description='**The number of entities that pass validation and uploaded**',
         title='Numberofacceptedentities',
     )
-    data: Optional[Any] = Field({}, description='Response data.', title='Data')
+    data: Optional[Any] = Field(default={}, description='Response data.', title='Data')
 
 
 class Pagination(BaseModel):
-    limit: Optional[int] = Field(-1, title='Limit')
-    skip: Optional[int] = Field(0, title='Skip')
-    total: Optional[int] = Field(-1, title='Total')
-    hasMore: Optional[bool] = Field(None, title='Hasmore')
-    search_after: Optional[List] = Field(None, title='Search After')
+    limit: Optional[int] = Field(default=-1, title='Limit')
+    skip: Optional[int] = Field(default=0, title='Skip')
+    total: Optional[int] = Field(default=-1, title='Total')
+    hasMore: Optional[bool] = Field(default=None, title='Hasmore')
+    search_after: Optional[List] = Field(default=None, title='Search After')
 
 
 class PermissionSourceType(Enum):
     User = 'User'
     Grouping = 'Grouping'
 
 
@@ -759,34 +767,34 @@
     Join = 'Join'
     Invite = 'Invite'
     Share = 'Share'
 
 
 class RequestSubmitResponse(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
-        None,
+        default=None,
         description='**The accepted time of the request**',
         title='Acceptedtimestamp',
     )
     requestId: str = Field(..., description='**Request id**', title='Requestid')
 
 
 class RestApiConnectorSchema(BaseModel):
-    config: Optional[Dict[str, Any]] = Field(None, title='Config')
-    serviceId: Optional[str] = Field('', title='Serviceid')
+    config: Optional[Dict[str, Any]] = Field(default=None, title='Config')
+    serviceId: Optional[str] = Field(default='', title='Serviceid')
     id: str = Field(..., title='Id')
-    createdAt: Optional[datetime] = Field(None, title='Createdat')
-    lastSyncedAt: Optional[str] = Field(None, title='Lastsyncedat')
-    lastError: Optional[str] = Field(None, title='Lasterror')
-    modifiedAt: Optional[datetime] = Field(None, title='Modifiedat')
+    createdAt: Optional[datetime] = Field(default=None, title='Createdat')
+    lastSyncedAt: Optional[str] = Field(default=None, title='Lastsyncedat')
+    lastError: Optional[str] = Field(default=None, title='Lasterror')
+    modifiedAt: Optional[datetime] = Field(default=None, title='Modifiedat')
     status: Optional[ConnectorStatus] = 'disabled'
     serviceType: str = Field(..., title='Servicetype')
     availableConnectorId: Optional[AvailableConnectorId] = 'restApiImport'
-    actorType: Optional[str] = Field(None, title='Actortype')
-    actorId: Optional[str] = Field(None, title='Actorid')
+    actorType: Optional[str] = Field(default=None, title='Actortype')
+    actorId: Optional[str] = Field(default=None, title='Actorid')
 
 
 class SearchAccountsAssociationsListResponseSchema(BaseModel):
     data: List[AccountsAssociationSchema] = Field(
         ..., description='Accounts Associations', title='Data'
     )
 
@@ -807,20 +815,20 @@
     data: List[PrivilegeGrantSchema] = Field(
         ..., description='Privilege Grants', title='Data'
     )
 
 
 class ServiceDescription(BaseModel):
     name: str = Field(..., title='Name')
-    icon: Optional[str] = Field(None, title='Icon')
+    icon: Optional[str] = Field(default=None, title='Icon')
 
 
 class SubmitResponse(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
-        None,
+        default=None,
         description='**The accepted time of the request**',
         title='Acceptedtimestamp',
     )
 
 
 class TransactionStateType(Enum):
     Applying = 'Applying'
@@ -833,53 +841,57 @@
 
 
 class UpdateAssetRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ..., description='Asset ID. **Mandatory, must be unique.**\n', title='Uniqueid'
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The asset ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
     name: constr(min_length=1) = Field(
         ...,
         description='The name of the asset. The default is the Asset ID. **Mandatory**\n',
         title='Name',
     )
     type: Optional[AssetType] = Field(
-        'Other',
+        default='Other',
         description='The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   •\t`Application` (federation) \n   •\t`Database`\n   •\t`Drive`\n   •\t`File`\n   •\t`Folder`\n   •\t`GitRepository`\n   •\t`Integration`\n   •\t`Project`\n   •\t`Site`\n   •\t`Table`\n   •\t`Ticket`\n   •\t`VirtualMachine`\n   •\t`Other`\n\nIf the asset type does not exist use `Other`.\n',
     )
     originType: Optional[str] = Field(
-        None,
+        default=None,
         description='The asset type in the source system.\nThe default is the canonical type (if not mentioned).\n',
         title='Origintype',
     )
     createdAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description='The date (in ISO 8601 format) that the asset was created.\nThe default is `null`.\n',
         title='Createdat',
     )
     lastUsedAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description='The date (in ISO 8601 format) of the last time that the asset was in use.\nThe default is `null`.\n',
         title='Lastusedat',
     )
     description: Optional[str] = Field(
-        None,
+        default=None,
         description='A description of the asset (up to 512 characters).\n',
         title='Description',
     )
     href: Optional[str] = Field(
-        None, description='A link to the asset in the source system.\n', title='Href'
+        default=None,
+        description='A link to the asset in the source system.\n',
+        title='Href',
+    )
+    owner: Optional[str] = Field(
+        default=None, description='The owner ID', title='Owner'
     )
-    owner: Optional[str] = Field(None, description='The owner ID', title='Owner')
     tags: Optional[List[constr(min_length=1)]] = Field(
-        None, description='Tags associated with the asset.\n', title='Tags'
+        default=None, description='Tags associated with the asset.\n', title='Tags'
     )
 
 
 class UpdateAssetsListRequestSchema(BaseModel):
     data: List[UpdateAssetRequestSchema] = Field(
         ..., description='Update Assets', max_items=10000, min_items=1, title='Data'
     )
@@ -888,65 +900,86 @@
 class UpdateGroupingsRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ...,
         description='\nGrouping ID. **Mandatory, must be unique.**\n',
         title='Uniqueid',
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The groupping ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
     name: constr(min_length=1) = Field(
         ...,
         description='The name of the grouping. The default is the ID field. **Mandatory**\n',
         title='Name',
     )
     originType: Optional[str] = Field(
-        None,
+        default=None,
         description='The name of the type of grouping in the source system. The default is `Group`. Example: Group/Alias/AWS Role\n',
         title='Origintype',
     )
     type: Optional[GroupingType] = Field(
-        'Group',
+        default='Group',
         description='Allowed values are `Group` and `VirtualGroup`.\n\nThe default is `Group`.\n\n`VirtualGroup` are mapped to the Authomize access explorer graph and are not present in other places in the user interface nor are they counted as a group.\n',
     )
     isRole: Optional[bool] = Field(
-        False,
+        default=False,
         description='If `Role`, the grouping represents a role in the source application and the name of the role is the grouping `name`.\n\nThe default is `False`.\n',
         title='Isrole',
     )
     anyoneCanJoinOrLeave: Optional[bool] = Field(
-        False,
+        default=False,
         description="Must be either `ture` or `false`.\nWhen set to `true` users can give themselves membership in this grouping without the grouping's managers' or owners' permission. \nExamples include public groups (M365), Google Groups with specific flags, ...\nValid only when `groupingType = Group`\n",
         title='Anyonecanjoinorleave',
     )
-    owner: Optional[str] = Field(None, description='The owner ID', title='Owner')
+    owner: Optional[str] = Field(
+        default=None,
+        description='The uniqueId of the user who is the "owner" (or manager) of the group.\n',
+        title='Owner',
+    )
     tags: Optional[List[constr(min_length=1)]] = Field(
-        None, description='Tags on the access grouping.\n', title='Tags'
+        default=None, description='Tags on the access grouping.\n', title='Tags'
     )
 
 
+class UpdateGroupingsResponseSchema(BaseModel):
+    acceptedTimestamp: Optional[datetime] = Field(
+        default=None,
+        description='**The accepted time of the request**',
+        title='Acceptedtimestamp',
+    )
+    requestId: str = Field(..., description='**Request id**', title='Requestid')
+    numberOfAcceptedEntities: int = Field(
+        ...,
+        description='**The number of entities that pass validation and uploaded**',
+        title='Numberofacceptedentities',
+    )
+    data: Optional[Any] = Field(default={}, description='Response data.', title='Data')
+
+
 class UpdatePrivilegeRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ...,
         description='Privilege ID.\n\nIf not defined, set as originName. **Mandatory, must be unique.**\n',
         title='Uniqueid',
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The privilege ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
     type: Optional[PrivilegeType] = Field(
-        None,
+        default=None,
         description='The "canonical" privilege types that are supported by Authomize off-the-shelf: **Mandatory**\n\nPermitted values: \n   •\t`Administrative`\n   •\t`Unknown`\n   •\t`Read`\n   •\t`ReadMetadata`\n   •\t`Write`\n   •\t`Create`\n   •\t`Delete`\n   •\t`Execute`\n   •\t`Enable`\n   •\t`Assign`\n   •\t`Restore`\n   •\t`Import`\n   •\t`Export`\n   •\t`Update`\n   •\t`Cancel`\n   •\t`Use`\n   •\t`Delegate`\n   •\t`Join`\n   •\t`Invite`\n   •\t`Share`\n\nIf the privilege type does not exist use `Unknown` or `Use`.\n',
     )
     originName: Optional[str] = Field(
-        None, description='The privilege name in the source system.', title='Originname'
+        default=None,
+        description='The privilege name in the source system.',
+        title='Originname',
     )
 
 
 class UpdatePrivilegesListRequestSchema(BaseModel):
     data: List[UpdatePrivilegeRequestSchema] = Field(
         ..., description='Update Privileges', max_items=10000, min_items=1, title='Data'
     )
@@ -965,311 +998,333 @@
     loc: List[str] = Field(..., title='Location')
     msg: str = Field(..., title='Message')
     type: str = Field(..., title='Error Type')
 
 
 class AccessDescription(BaseModel):
     fromIdentityId: str = Field(..., title='Fromidentityid')
-    toAssetId: Optional[str] = Field(None, title='Toassetid')
+    toAssetId: Optional[str] = Field(default=None, title='Toassetid')
     accessType: AccessTypes
-    accessName: Optional[str] = Field(None, title='Accessname')
+    accessName: Optional[str] = Field(default=None, title='Accessname')
 
 
 class AssetDescription(BaseModel):
     id: str = Field(..., title='Id')
     name: str = Field(..., title='Name')
     type: AssetTypes
-    description: Optional[str] = Field(None, title='Description')
-    logoUrl: Optional[str] = Field(None, title='Logourl')
-    href: Optional[str] = Field(None, title='Href')
-    createdAt: Optional[datetime] = Field(None, title='Createdat')
-    isAuxiliary: Optional[bool] = Field(None, title='Isauxiliary')
-    service: Optional[str] = Field(None, title='Service')
-    isFederated: Optional[bool] = Field(None, title='Isfederated')
+    description: Optional[str] = Field(default=None, title='Description')
+    logoUrl: Optional[str] = Field(default=None, title='Logourl')
+    href: Optional[str] = Field(default=None, title='Href')
+    createdAt: Optional[datetime] = Field(default=None, title='Createdat')
+    isAuxiliary: Optional[bool] = Field(default=None, title='Isauxiliary')
+    service: Optional[str] = Field(default=None, title='Service')
+    isFederated: Optional[bool] = Field(default=None, title='Isfederated')
 
 
 class AssetSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ..., description='Asset ID. **Mandatory, must be unique.**\n', title='Uniqueid'
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The asset ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
     name: constr(min_length=1) = Field(
         ...,
         description='The name of the asset. The default is the Asset ID. **Mandatory**\n',
         title='Name',
     )
     type: Optional[AssetType] = Field(
-        'Other',
+        default='Other',
         description='The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   •\t`Application` (federation) \n   •\t`Database`\n   •\t`Drive`\n   •\t`File`\n   •\t`Folder`\n   •\t`GitRepository`\n   •\t`Integration`\n   •\t`Project`\n   •\t`Site`\n   •\t`Table`\n   •\t`Ticket`\n   •\t`VirtualMachine`\n   •\t`Other`\n\nIf the asset type does not exist use `Other`.\n',
     )
     originType: Optional[str] = Field(
-        None,
+        default=None,
         description='The asset type in the source system.\nThe default is the canonical type (if not mentioned).\n',
         title='Origintype',
     )
     createdAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description='The date (in ISO 8601 format) that the asset was created.\nThe default is `null`.\n',
         title='Createdat',
     )
     lastUsedAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description='The date (in ISO 8601 format) of the last time that the asset was in use.\nThe default is `null`.\n',
         title='Lastusedat',
     )
     description: Optional[str] = Field(
-        None,
+        default=None,
         description='A description of the asset (up to 512 characters).\n',
         title='Description',
     )
     href: Optional[str] = Field(
-        None, description='A link to the asset in the source system.\n', title='Href'
+        default=None,
+        description='A link to the asset in the source system.\n',
+        title='Href',
+    )
+    owner: Optional[str] = Field(
+        default=None, description='The owner ID', title='Owner'
     )
-    owner: Optional[str] = Field(None, description='The owner ID', title='Owner')
     tags: Optional[List[constr(min_length=1)]] = Field(
-        None, description='Tags associated with the asset.\n', title='Tags'
+        default=None, description='Tags associated with the asset.\n', title='Tags'
     )
 
 
 class BundleTransactionSchema(BaseModel):
     connectorId: str = Field(..., title='Connectorid')
-    transactionCreatedAt: Optional[datetime] = Field(None, title='Transactioncreatedat')
-    warnings: Optional[List[str]] = Field(None, title='Warnings')
-    validations: Optional[Dict[str, Any]] = Field(None, title='Validations')
+    transactionCreatedAt: Optional[datetime] = Field(
+        default=None, title='Transactioncreatedat'
+    )
+    warnings: Optional[List[str]] = Field(default=None, title='Warnings')
+    validations: Optional[Dict[str, Any]] = Field(default=None, title='Validations')
     id: str = Field(..., title='Id')
     state: TransactionStateType
 
 
 class GroupingSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ...,
         description='\nGrouping ID. **Mandatory, must be unique.**\n',
         title='Uniqueid',
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The groupping ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
     name: constr(min_length=1) = Field(
         ...,
         description='The name of the grouping. The default is the ID field. **Mandatory**\n',
         title='Name',
     )
     originType: Optional[str] = Field(
-        None,
+        default=None,
         description='The name of the type of grouping in the source system. The default is `Group`. Example: Group/Alias/AWS Role\n',
         title='Origintype',
     )
     type: Optional[GroupingType] = Field(
-        'Group',
+        default='Group',
         description='Allowed values are `Group` and `VirtualGroup`.\n\nThe default is `Group`.\n\n`VirtualGroup` are mapped to the Authomize access explorer graph and are not present in other places in the user interface nor are they counted as a group.\n',
     )
     isRole: Optional[bool] = Field(
-        False,
+        default=False,
         description='If `Role`, the grouping represents a role in the source application and the name of the role is the grouping `name`.\n\nThe default is `False`.\n',
         title='Isrole',
     )
     anyoneCanJoinOrLeave: Optional[bool] = Field(
-        False,
+        default=False,
         description="Must be either `ture` or `false`.\nWhen set to `true` users can give themselves membership in this grouping without the grouping's managers' or owners' permission. \nExamples include public groups (M365), Google Groups with specific flags, ...\nValid only when `groupingType = Group`\n",
         title='Anyonecanjoinorleave',
     )
-    owner: Optional[str] = Field(None, description='The owner ID', title='Owner')
+    owner: Optional[str] = Field(
+        default=None,
+        description='The uniqueId of the user who is the "owner" (or manager) of the group.\n',
+        title='Owner',
+    )
     tags: Optional[List[constr(min_length=1)]] = Field(
-        None, description='Tags on the access grouping.\n', title='Tags'
+        default=None, description='Tags on the access grouping.\n', title='Tags'
     )
 
 
 class HTTPValidationError(BaseModel):
-    detail: Optional[List[ValidationError]] = Field(None, title='Detail')
+    detail: Optional[List[ValidationError]] = Field(default=None, title='Detail')
 
 
 class IdentityDescription(BaseModel):
     id: str = Field(..., title='Id')
-    name: Optional[str] = Field(None, title='Name')
+    name: Optional[str] = Field(default=None, title='Name')
     type: IdentityTypes
-    userType: Optional[str] = Field(None, title='Usertype')
-    email: Optional[str] = Field(None, title='Email')
-    manager: Optional[str] = Field(None, title='Manager')
-    title: Optional[str] = Field(None, title='Title')
-    department: Optional[str] = Field(None, title='Department')
-    description: Optional[str] = Field(None, title='Description')
-    href: Optional[str] = Field(None, title='Href')
-    createdAt: Optional[datetime] = Field(None, title='Createdat')
-    terminationDate: Optional[datetime] = Field(None, title='Terminationdate')
-    isExternal: Optional[bool] = Field(None, title='Isexternal')
-    isAuxiliary: Optional[bool] = Field(None, title='Isauxiliary')
+    userType: Optional[str] = Field(default=None, title='Usertype')
+    email: Optional[str] = Field(default=None, title='Email')
+    manager: Optional[str] = Field(default=None, title='Manager')
+    title: Optional[str] = Field(default=None, title='Title')
+    department: Optional[str] = Field(default=None, title='Department')
+    description: Optional[str] = Field(default=None, title='Description')
+    href: Optional[str] = Field(default=None, title='Href')
+    createdAt: Optional[datetime] = Field(default=None, title='Createdat')
+    terminationDate: Optional[datetime] = Field(default=None, title='Terminationdate')
+    isExternal: Optional[bool] = Field(default=None, title='Isexternal')
+    isAuxiliary: Optional[bool] = Field(default=None, title='Isauxiliary')
     hasTwoFactorAuthenticationEnabled: Optional[bool] = Field(
-        None, title='Hastwofactorauthenticationenabled'
+        default=None, title='Hastwofactorauthenticationenabled'
     )
-    firstName: Optional[str] = Field(None, title='Firstname')
-    lastName: Optional[str] = Field(None, title='Lastname')
-    userName: Optional[str] = Field(None, title='Username')
+    firstName: Optional[str] = Field(default=None, title='Firstname')
+    lastName: Optional[str] = Field(default=None, title='Lastname')
+    userName: Optional[str] = Field(default=None, title='Username')
     status: Optional[UserStatus] = None
-    service: Optional[str] = Field(None, title='Service')
-    lastLoginAt: Optional[datetime] = Field(None, title='Lastloginat')
-    anyoneCanJoinOrLeave: Optional[bool] = Field(None, title='Anyonecanjoinorleave')
-    tags: Optional[List[str]] = Field(None, title='Tags')
-    city: Optional[str] = Field(None, title='City')
-    country: Optional[str] = Field(None, title='Country')
-    division: Optional[str] = Field(None, title='Division')
-    employeeNumber: Optional[str] = Field(None, title='Employeenumber')
-    personalEmail: Optional[str] = Field(None, title='Personalemail')
-    hireDate: Optional[datetime] = Field(None, title='Hiredate')
+    service: Optional[str] = Field(default=None, title='Service')
+    lastLoginAt: Optional[datetime] = Field(default=None, title='Lastloginat')
+    anyoneCanJoinOrLeave: Optional[bool] = Field(
+        default=None, title='Anyonecanjoinorleave'
+    )
+    tags: Optional[List[str]] = Field(default=None, title='Tags')
+    city: Optional[str] = Field(default=None, title='City')
+    country: Optional[str] = Field(default=None, title='Country')
+    division: Optional[str] = Field(default=None, title='Division')
+    employeeNumber: Optional[str] = Field(default=None, title='Employeenumber')
+    personalEmail: Optional[str] = Field(default=None, title='Personalemail')
+    hireDate: Optional[datetime] = Field(default=None, title='Hiredate')
 
 
 class IdentitySchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ..., description='Identity ID **Mandatory**\n', title='Uniqueid'
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The identity ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
-    name: Optional[str] = Field(None, description='Username', title='Name')
+    name: Optional[str] = Field(default=None, description='Username', title='Name')
     email: Optional[str] = Field(
-        None, description="User's work email address.\n", title='Email'
+        default=None, description="User's work email address.\n", title='Email'
     )
     personalEmail: Optional[str] = Field(
-        None, description="User's personal email address.\n", title='Personalemail'
+        default=None,
+        description="User's personal email address.\n",
+        title='Personalemail',
     )
     firstName: Optional[str] = Field(
-        None, description="User's first name\n", title='Firstname'
+        default=None, description="User's first name\n", title='Firstname'
     )
     lastName: Optional[str] = Field(
-        None, description="The user's last name.\n", title='Lastname'
+        default=None, description="The user's last name.\n", title='Lastname'
     )
     employeeNumber: Optional[str] = Field(
-        None, description='Employee number', title='Employeenumber'
+        default=None, description='Employee number', title='Employeenumber'
     )
     status: Optional[UserStatus] = Field(
-        None,
+        default=None,
         description='The user status must be one of the following: `Deleted`, `Disabled`, `Enabled`, `Staged` or `Suspended`.\n',
     )
-    country: Optional[str] = Field(None, description='Country', title='Country')
-    city: Optional[str] = Field(None, description='City', title='City')
+    country: Optional[str] = Field(default=None, description='Country', title='Country')
+    city: Optional[str] = Field(default=None, description='City', title='City')
     department: Optional[str] = Field(
-        None,
+        default=None,
         description="The identity's department in the organization.\n",
         title='Department',
     )
     division: Optional[str] = Field(
-        None,
+        default=None,
         description="The identity's division in their organization.\n",
         title='Division',
     )
     title: Optional[str] = Field(
-        None, description="The user's job title.\n", title='Title'
+        default=None, description="The user's job title.\n", title='Title'
     )
     managerId: Optional[str] = Field(
-        None, description="The manager identity's ID.\n", title='Managerid'
+        default=None, description="The manager identity's ID.\n", title='Managerid'
     )
     hireAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description="The user's first day of work (in ISO 8601 format).\n",
         title='Hireat',
     )
     terminationAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description="The user's last day of work (in ISO 8601 format).\n",
         title='Terminationat',
     )
     description: Optional[str] = Field(
-        None,
+        default=None,
         description='Additional description of the identity.\n',
         title='Description',
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
-        None, description='One or more tags on the user account.\n', title='Tags'
+        default=None,
+        description='One or more tags on the user account.\n',
+        title='Tags',
     )
 
 
 class ItemsBundleSchema(BaseModel):
-    services: Optional[List[ServiceDescription]] = Field(None, title='Services')
-    identities: Optional[List[IdentityDescription]] = Field(None, title='Identities')
-    assets: Optional[List[AssetDescription]] = Field(None, title='Assets')
+    services: Optional[List[ServiceDescription]] = Field(default=None, title='Services')
+    identities: Optional[List[IdentityDescription]] = Field(
+        default=None, title='Identities'
+    )
+    assets: Optional[List[AssetDescription]] = Field(default=None, title='Assets')
     inheritanceIdentities: Optional[List[IdentitiesInheritance]] = Field(
-        None, title='Inheritanceidentities'
+        default=None, title='Inheritanceidentities'
     )
     inheritanceAssets: Optional[List[AssetsInheritance]] = Field(
-        None, title='Inheritanceassets'
+        default=None, title='Inheritanceassets'
     )
-    access: Optional[List[AccessDescription]] = Field(None, title='Access')
+    access: Optional[List[AccessDescription]] = Field(default=None, title='Access')
 
 
 class NewIdentityRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ..., description='Identity ID **Mandatory**\n', title='Uniqueid'
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The identity ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
-    name: Optional[str] = Field(None, description='Username', title='Name')
+    name: Optional[str] = Field(default=None, description='Username', title='Name')
     email: Optional[str] = Field(
-        None, description="User's work email address.\n", title='Email'
+        default=None, description="User's work email address.\n", title='Email'
     )
     personalEmail: Optional[str] = Field(
-        None, description="User's personal email address.\n", title='Personalemail'
+        default=None,
+        description="User's personal email address.\n",
+        title='Personalemail',
     )
     firstName: Optional[str] = Field(
-        None, description="User's first name\n", title='Firstname'
+        default=None, description="User's first name\n", title='Firstname'
     )
     lastName: Optional[str] = Field(
-        None, description="The user's last name.\n", title='Lastname'
+        default=None, description="The user's last name.\n", title='Lastname'
     )
     employeeNumber: Optional[str] = Field(
-        None, description='Employee number', title='Employeenumber'
+        default=None, description='Employee number', title='Employeenumber'
     )
     status: Optional[UserStatus] = Field(
-        None,
+        default=None,
         description='The user status must be one of the following: `Deleted`, `Disabled`, `Enabled`, `Staged` or `Suspended`.\n',
     )
-    country: Optional[str] = Field(None, description='Country', title='Country')
-    city: Optional[str] = Field(None, description='City', title='City')
+    country: Optional[str] = Field(default=None, description='Country', title='Country')
+    city: Optional[str] = Field(default=None, description='City', title='City')
     department: Optional[str] = Field(
-        None,
+        default=None,
         description="The identity's department in the organization.\n",
         title='Department',
     )
     division: Optional[str] = Field(
-        None,
+        default=None,
         description="The identity's division in their organization.\n",
         title='Division',
     )
     title: Optional[str] = Field(
-        None, description="The user's job title.\n", title='Title'
+        default=None, description="The user's job title.\n", title='Title'
     )
     managerId: Optional[str] = Field(
-        None, description="The manager identity's ID.\n", title='Managerid'
+        default=None, description="The manager identity's ID.\n", title='Managerid'
     )
     hireAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description="The user's first day of work (in ISO 8601 format).\n",
         title='Hireat',
     )
     terminationAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description="The user's last day of work (in ISO 8601 format).\n",
         title='Terminationat',
     )
     description: Optional[str] = Field(
-        None,
+        default=None,
         description='Additional description of the identity.\n',
         title='Description',
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
-        None, description='One or more tags on the user account.\n', title='Tags'
+        default=None,
+        description='One or more tags on the user account.\n',
+        title='Tags',
     )
 
 
 class NewPermissionRequestSchema(BaseModel):
     sourceUniqueId: constr(min_length=1) = Field(
         ...,
         description="The unique ID of the permission's source. Must be either `userId` or `groupingId`. **Mandatory**.\n",
@@ -1281,124 +1336,130 @@
     )
     privilegeId: constr(min_length=1) = Field(
         ...,
         description='The ID of the privilege, allows access to assets. **Mandatory**.\n',
         title='Privilegeid',
     )
     assetId: Optional[str] = Field(
-        None,
+        default=None,
         description='The ID of the asset.\n\nWhen `null`, this is a global permission on the entire application (not just locally).',
         title='Assetid',
     )
     isRole: Optional[bool] = Field(
-        False,
+        default=False,
         description='If `true`, the permissions represent the role in the source application.\nThe default is `false`.\n',
         title='Isrole',
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
-        None, description='Tags on access permissions.\n', title='Tags'
+        default=None, description='Tags on access permissions.\n', title='Tags'
     )
 
 
 class NewPermissionsListRequestSchema(BaseModel):
     data: List[NewPermissionRequestSchema] = Field(
         ..., description='New Permissions', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
-        False,
+        default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
     )
 
 
 class NewPrivilegeRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ...,
         description='Privilege ID.\n\nIf not defined, set as originName. **Mandatory, must be unique.**\n',
         title='Uniqueid',
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The privilege ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
     type: PrivilegeType = Field(
         ...,
         description='The "canonical" privilege types that are supported by Authomize off-the-shelf: **Mandatory**\n\nPermitted values: \n   •\t`Administrative`\n   •\t`Unknown`\n   •\t`Read`\n   •\t`ReadMetadata`\n   •\t`Write`\n   •\t`Create`\n   •\t`Delete`\n   •\t`Execute`\n   •\t`Enable`\n   •\t`Assign`\n   •\t`Restore`\n   •\t`Import`\n   •\t`Export`\n   •\t`Update`\n   •\t`Cancel`\n   •\t`Use`\n   •\t`Delegate`\n   •\t`Join`\n   •\t`Invite`\n   •\t`Share`\n\nIf the privilege type does not exist use `Unknown` or `Use`.\n',
     )
     originName: Optional[str] = Field(
-        None, description='The privilege name in the source system.', title='Originname'
+        default=None,
+        description='The privilege name in the source system.',
+        title='Originname',
     )
 
 
 class NewPrivilegesListRequestSchema(BaseModel):
     data: List[NewPrivilegeRequestSchema] = Field(
         ..., description='New Privileges', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
-        False,
+        default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
     )
 
 
 class NewUserRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ...,
         description="User's Account ID. **Mandatory, must be unique.**\n",
         title='Uniqueid',
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The user ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
-    name: Optional[str] = Field(None, description='Username\n', title='Name')
+    name: Optional[str] = Field(default=None, description='Username\n', title='Name')
     email: Optional[str] = Field(
-        None, description="User's email address.", title='Email'
+        default=None, description="User's email address.", title='Email'
     )
     firstName: Optional[str] = Field(
-        None, description="User's first name\n", title='Firstname'
+        default=None, description="User's first name\n", title='Firstname'
     )
     lastName: Optional[str] = Field(
-        None, description="The user's last name.\n", title='Lastname'
+        default=None, description="The user's last name.\n", title='Lastname'
     )
     status: Optional[UserStatus] = Field(
-        None,
+        default=None,
         description='User status must be: `Deleted`, `Disabled`, `Enabled`, `Staged`, `Suspended`, or `Unknown`.\n',
     )
     description: Optional[str] = Field(
-        None, description='Additional description of the user.\n', title='Description'
+        default=None,
+        description='Additional description of the user.\n',
+        title='Description',
     )
     isExternal: Optional[bool] = Field(
-        False,
+        default=False,
         description='Account is external to Authomize.\nMust be either `true` or `false`.\n',
         title='Isexternal',
     )
     hasMFA: Optional[bool] = Field(
-        None,
+        default=None,
         description='Has Multi-Factor Authentication enabled.\nMust be either `true` or `false`.\n',
         title='Hasmfa',
     )
     lastLoginAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description='The last login date in ISO 8601 format.\n',
         title='Lastloginat',
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
-        None, description='One or more tags on the user account.\n', title='Tags'
+        default=None,
+        description='One or more tags on the user account.\n',
+        title='Tags',
     )
 
 
 class NewUsersListRequestSchema(BaseModel):
     data: List[NewUserRequestSchema] = Field(
         ..., description='New Users', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
-        False,
+        default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
     )
 
 
 class PermissionSchema(BaseModel):
     sourceUniqueId: constr(min_length=1) = Field(
@@ -1412,106 +1473,108 @@
     )
     privilegeId: constr(min_length=1) = Field(
         ...,
         description='The ID of the privilege, allows access to assets. **Mandatory**.\n',
         title='Privilegeid',
     )
     assetId: Optional[str] = Field(
-        None,
+        default=None,
         description='The ID of the asset.\n\nWhen `null`, this is a global permission on the entire application (not just locally).',
         title='Assetid',
     )
     isRole: Optional[bool] = Field(
-        False,
+        default=False,
         description='If `true`, the permissions represent the role in the source application.\nThe default is `false`.\n',
         title='Isrole',
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
-        None, description='Tags on access permissions.\n', title='Tags'
+        default=None, description='Tags on access permissions.\n', title='Tags'
     )
 
 
 class PrivilegeSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ...,
         description='Privilege ID.\n\nIf not defined, set as originName. **Mandatory, must be unique.**\n',
         title='Uniqueid',
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The privilege ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
     type: PrivilegeType = Field(
         ...,
         description='The "canonical" privilege types that are supported by Authomize off-the-shelf: **Mandatory**\n\nPermitted values: \n   •\t`Administrative`\n   •\t`Unknown`\n   •\t`Read`\n   •\t`ReadMetadata`\n   •\t`Write`\n   •\t`Create`\n   •\t`Delete`\n   •\t`Execute`\n   •\t`Enable`\n   •\t`Assign`\n   •\t`Restore`\n   •\t`Import`\n   •\t`Export`\n   •\t`Update`\n   •\t`Cancel`\n   •\t`Use`\n   •\t`Delegate`\n   •\t`Join`\n   •\t`Invite`\n   •\t`Share`\n\nIf the privilege type does not exist use `Unknown` or `Use`.\n',
     )
     originName: Optional[str] = Field(
-        None, description='The privilege name in the source system.', title='Originname'
+        default=None,
+        description='The privilege name in the source system.',
+        title='Originname',
     )
 
 
 class RequestsBundleSchema(BaseModel):
     delete_app_data: Optional[bool] = Field(
-        False,
+        default=False,
         description='The Delete Application Data API is used to delete app data by `{appId}`.',
         title='Delete App Data',
     )
-    createdAt: Optional[datetime] = Field(None, title='Createdat')
+    createdAt: Optional[datetime] = Field(default=None, title='Createdat')
     new_users: Optional[List[NewUserRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Users APIs sets up App users(by App ID).',
         title='New Users',
     )
     new_groupings: Optional[List[NewGroupingRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Groupings API is used to create groups that have access to a particular app.',
         title='New Groupings',
     )
     new_permissions: Optional[List[NewPermissionRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Permissions API is used to create a set of privileges, assigned to a specific target.\nA permission (also referred to as an “entitlement”) is a set of privileges, assigned to a specific target. \nExamples include: file permissions, file shares, GCP entitlements, the actual policies assigning access to roles in AWS, and inline policies.',
         title='New Permissions',
     )
     new_privileges: Optional[List[NewPrivilegeRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Privileges API is used to define privileges that can be associated with assets.\nFor example, Read privileges on a file.\nHere you can define the type of privileges and associate it to assets in the Permission API.\n',
         title='New Privileges',
     )
     new_privileges_grants: Optional[List[NewPrivilegeGrantsRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Privileges Grants API enables you to establish inheritance between privileges, so that a single privilege contains a set of other privileges. \nFor example, an Administrative privilege that contains read and write privileges.',
         title='New Privileges Grants',
     )
     new_accounts_association: Optional[
         List[NewAccountsAssociationRequestSchema]
     ] = Field(
-        None,
+        default=None,
         description='The Create Accounts Association API creates account associations between user accounts and groups.',
         title='New Accounts Association',
     )
     new_groupings_association: Optional[
         List[NewGroupingsAssociationRequestSchema]
     ] = Field(
-        None,
+        default=None,
         description='The Create Groupings Association API creates associations between groups and other groups.\n',
         title='New Groupings Association',
     )
     new_assets: Optional[List[NewAssetRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Assets API creates assets (including asset data).',
         title='New Assets',
     )
     new_assets_inheritance: Optional[List[NewAssetInheritanceRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Assets Inheritence API enables you to create a connection between different assets (for example, a folder that contains multiple files).\n',
         title='New Assets Inheritance',
     )
     new_identities: Optional[List[NewIdentityRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Identities API is used to create identities. \nThe data of the identity from this API is considered "the source of truth" and overrides the identity data from other systems.\n',
         title='New Identities',
     )
 
 
 class RestApiConnectorListSchema(BaseModel):
     pagination: Pagination
@@ -1554,235 +1617,247 @@
 
 
 class UpdateIdentityRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ..., description='Identity ID **Mandatory**\n', title='Uniqueid'
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The identity ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
-    name: Optional[str] = Field(None, description='Username', title='Name')
+    name: Optional[str] = Field(default=None, description='Username', title='Name')
     email: Optional[str] = Field(
-        None, description="User's work email address.\n", title='Email'
+        default=None, description="User's work email address.\n", title='Email'
     )
     personalEmail: Optional[str] = Field(
-        None, description="User's personal email address.\n", title='Personalemail'
+        default=None,
+        description="User's personal email address.\n",
+        title='Personalemail',
     )
     firstName: Optional[str] = Field(
-        None, description="User's first name\n", title='Firstname'
+        default=None, description="User's first name\n", title='Firstname'
     )
     lastName: Optional[str] = Field(
-        None, description="The user's last name.\n", title='Lastname'
+        default=None, description="The user's last name.\n", title='Lastname'
     )
     employeeNumber: Optional[str] = Field(
-        None, description='Employee number', title='Employeenumber'
+        default=None, description='Employee number', title='Employeenumber'
     )
     status: Optional[UserStatus] = Field(
-        None,
+        default=None,
         description='The user status must be one of the following: `Deleted`, `Disabled`, `Enabled`, `Staged` or `Suspended`.\n',
     )
-    country: Optional[str] = Field(None, description='Country', title='Country')
-    city: Optional[str] = Field(None, description='City', title='City')
+    country: Optional[str] = Field(default=None, description='Country', title='Country')
+    city: Optional[str] = Field(default=None, description='City', title='City')
     department: Optional[str] = Field(
-        None,
+        default=None,
         description="The identity's department in the organization.\n",
         title='Department',
     )
     division: Optional[str] = Field(
-        None,
+        default=None,
         description="The identity's division in their organization.\n",
         title='Division',
     )
     title: Optional[str] = Field(
-        None, description="The user's job title.\n", title='Title'
+        default=None, description="The user's job title.\n", title='Title'
     )
     managerId: Optional[str] = Field(
-        None, description="The manager identity's ID.\n", title='Managerid'
+        default=None, description="The manager identity's ID.\n", title='Managerid'
     )
     hireAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description="The user's first day of work (in ISO 8601 format).\n",
         title='Hireat',
     )
     terminationAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description="The user's last day of work (in ISO 8601 format).\n",
         title='Terminationat',
     )
     description: Optional[str] = Field(
-        None,
+        default=None,
         description='Additional description of the identity.\n',
         title='Description',
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
-        None, description='One or more tags on the user account.\n', title='Tags'
+        default=None,
+        description='One or more tags on the user account.\n',
+        title='Tags',
     )
 
 
 class UpdateUserRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ...,
         description="User's Account ID. **Mandatory, must be unique.**\n",
         title='Uniqueid',
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The user ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
-    name: Optional[str] = Field(None, description='Username\n', title='Name')
+    name: Optional[str] = Field(default=None, description='Username\n', title='Name')
     email: Optional[str] = Field(
-        None, description="User's email address.", title='Email'
+        default=None, description="User's email address.", title='Email'
     )
     firstName: Optional[str] = Field(
-        None, description="User's first name\n", title='Firstname'
+        default=None, description="User's first name\n", title='Firstname'
     )
     lastName: Optional[str] = Field(
-        None, description="The user's last name.\n", title='Lastname'
+        default=None, description="The user's last name.\n", title='Lastname'
     )
     status: Optional[UserStatus] = Field(
-        None,
+        default=None,
         description='User status must be: `Deleted`, `Disabled`, `Enabled`, `Staged`, `Suspended`, or `Unknown`.\n',
     )
     description: Optional[str] = Field(
-        None, description='Additional description of the user.\n', title='Description'
+        default=None,
+        description='Additional description of the user.\n',
+        title='Description',
     )
     isExternal: Optional[bool] = Field(
-        False,
+        default=False,
         description='Account is external to Authomize.\nMust be either `true` or `false`.\n',
         title='Isexternal',
     )
     hasMFA: Optional[bool] = Field(
-        None,
+        default=None,
         description='Has Multi-Factor Authentication enabled.\nMust be either `true` or `false`.\n',
         title='Hasmfa',
     )
     lastLoginAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description='The last login date in ISO 8601 format.\n',
         title='Lastloginat',
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
-        None, description='One or more tags on the user account.\n', title='Tags'
+        default=None,
+        description='One or more tags on the user account.\n',
+        title='Tags',
     )
 
 
 class UserSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ...,
         description="User's Account ID. **Mandatory, must be unique.**\n",
         title='Uniqueid',
     )
     originId: Optional[constr(min_length=1)] = Field(
-        None,
+        default=None,
         description="The user ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
         title='Originid',
     )
-    name: Optional[str] = Field(None, description='Username\n', title='Name')
+    name: Optional[str] = Field(default=None, description='Username\n', title='Name')
     email: Optional[str] = Field(
-        None, description="User's email address.", title='Email'
+        default=None, description="User's email address.", title='Email'
     )
     firstName: Optional[str] = Field(
-        None, description="User's first name\n", title='Firstname'
+        default=None, description="User's first name\n", title='Firstname'
     )
     lastName: Optional[str] = Field(
-        None, description="The user's last name.\n", title='Lastname'
+        default=None, description="The user's last name.\n", title='Lastname'
     )
     status: Optional[UserStatus] = Field(
-        None,
+        default=None,
         description='User status must be: `Deleted`, `Disabled`, `Enabled`, `Staged`, `Suspended`, or `Unknown`.\n',
     )
     description: Optional[str] = Field(
-        None, description='Additional description of the user.\n', title='Description'
+        default=None,
+        description='Additional description of the user.\n',
+        title='Description',
     )
     isExternal: Optional[bool] = Field(
-        False,
+        default=False,
         description='Account is external to Authomize.\nMust be either `true` or `false`.\n',
         title='Isexternal',
     )
     hasMFA: Optional[bool] = Field(
-        None,
+        default=None,
         description='Has Multi-Factor Authentication enabled.\nMust be either `true` or `false`.\n',
         title='Hasmfa',
     )
     lastLoginAt: Optional[datetime] = Field(
-        None,
+        default=None,
         description='The last login date in ISO 8601 format.\n',
         title='Lastloginat',
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
-        None, description='One or more tags on the user account.\n', title='Tags'
+        default=None,
+        description='One or more tags on the user account.\n',
+        title='Tags',
     )
 
 
 class IngestionDataBundleSchema(BaseModel):
     new_users: Optional[List[NewUserRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Users APIs sets up App users(by App ID).',
         title='New Users',
     )
     new_groupings: Optional[List[NewGroupingRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Groupings API is used to create groups that have access to a particular app.',
         title='New Groupings',
     )
     new_permissions: Optional[List[NewPermissionRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Permissions API is used to create a set of privileges, assigned to a specific target.\nA permission (also referred to as an “entitlement”) is a set of privileges, assigned to a specific target. \nExamples include: file permissions, file shares, GCP entitlements, the actual policies assigning access to roles in AWS, and inline policies.',
         title='New Permissions',
     )
     new_privileges: Optional[List[NewPrivilegeRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Privileges API is used to define privileges that can be associated with assets.\nFor example, Read privileges on a file.\nHere you can define the type of privileges and associate it to assets in the Permission API.\n',
         title='New Privileges',
     )
     new_privileges_grants: Optional[List[NewPrivilegeGrantsRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Privileges Grants API enables you to establish inheritance between privileges, so that a single privilege contains a set of other privileges. \nFor example, an Administrative privilege that contains read and write privileges.',
         title='New Privileges Grants',
     )
     new_accounts_association: Optional[
         List[NewAccountsAssociationRequestSchema]
     ] = Field(
-        None,
+        default=None,
         description='The Create Accounts Association API creates account associations between user accounts and groups.',
         title='New Accounts Association',
     )
     new_groupings_association: Optional[
         List[NewGroupingsAssociationRequestSchema]
     ] = Field(
-        None,
+        default=None,
         description='The Create Groupings Association API creates associations between groups and other groups.\n',
         title='New Groupings Association',
     )
     new_assets: Optional[List[NewAssetRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Assets API creates assets (including asset data).',
         title='New Assets',
     )
     new_assets_inheritance: Optional[List[NewAssetInheritanceRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Assets Inheritence API enables you to create a connection between different assets (for example, a folder that contains multiple files).\n',
         title='New Assets Inheritance',
     )
     new_identities: Optional[List[NewIdentityRequestSchema]] = Field(
-        None,
+        default=None,
         description='The Create Identities API is used to create identities. \nThe data of the identity from this API is considered "the source of truth" and overrides the identity data from other systems.\n',
         title='New Identities',
     )
 
 
 class NewIdentitiesListRequestSchema(BaseModel):
     data: List[NewIdentityRequestSchema] = Field(
         ..., description='New Identities', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
-        False,
+        default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
     )
 
 
 class SearchUsersListResponseSchema(BaseModel):
     data: List[UserSchema] = Field(..., description='Users', title='Data')
```

### Comparing `authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-03-08T16:14:40+00:00
+#   timestamp: 2023-04-19T21:34:40+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Union
 
@@ -75,42 +75,45 @@
 
 
 class BaseBooleanFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_eq: Optional[bool] = Field(
-        None, alias='$eq', description='Equals To', title='$Eq'
+        default=None, alias='$eq', description='Equals To', title='$Eq'
     )
 
 
 class BaseDateFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_gt: Optional[datetime] = Field(
-        None, alias='$gt', description='Greater Than', title='$Gt'
+        default=None, alias='$gt', description='Greater Than', title='$Gt'
     )
     field_gte: Optional[datetime] = Field(
-        None, alias='$gte', description='Greater Than Or Equals To', title='$Gte'
+        default=None,
+        alias='$gte',
+        description='Greater Than Or Equals To',
+        title='$Gte',
     )
     field_lt: Optional[datetime] = Field(
-        None, alias='$lt', description='Less Than', title='$Lt'
+        default=None, alias='$lt', description='Less Than', title='$Lt'
     )
     field_lte: Optional[datetime] = Field(
-        None, alias='$lte', description='Less Than Or Equals To', title='$Lte'
+        default=None, alias='$lte', description='Less Than Or Equals To', title='$Lte'
     )
 
 
 class BaseSingleValuedStringFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_eq: Optional[str] = Field(
-        None, alias='$eq', description='Equals To', title='$Eq'
+        default=None, alias='$eq', description='Equals To', title='$Eq'
     )
 
 
 class CampaignExpansion(Enum):
     owner = 'owner'
 
 
@@ -189,16 +192,16 @@
     field_13_4 = '13.4'
     field_13_9 = '13.9'
     field_13_10 = '13.10'
 
 
 class Cisv8(BaseModel):
     values: List[CisV8Standard] = Field(..., description='Values')
-    id: Optional[str] = Field('cisv8', description='UniqueID', title='Id')
-    name: Optional[str] = Field('CIS v.8', description='Name', title='Name')
+    id: Optional[str] = Field(default='cisv8', description='UniqueID', title='Id')
+    name: Optional[str] = Field(default='CIS v.8', description='Name', title='Name')
 
 
 class CommentSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     id: str = Field(..., description='Unique ID of comment.', title='Id')
@@ -267,15 +270,17 @@
     A_9_4_5 = 'A.9.4.5'
     A_8_2_3 = 'A.8.2.3'
     A_7_3_1 = 'A.7.3.1'
     A_8_1_4 = 'A.8.1.4'
 
 
 class MeResponse(BaseModel):
-    version: Optional[str] = Field('3.1.2', description='**version**', title='Version')
+    version: Optional[str] = Field(
+        default='3.1.5', description='**version**', title='Version'
+    )
     id: str = Field(..., description='**id**', title='Id')
     tenant: str = Field(..., description='**tenant**', title='Tenant')
 
 
 class NonPaginatedResponseSchemaCommentSchema(BaseModel):
     class Config:
         extra = Extra.forbid
@@ -283,27 +288,27 @@
     data: CommentSchema = Field(..., description='Actual Data', title='Data')
 
 
 class PaginationRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    limit: Optional[int] = Field(None, description='Limit', title='Limit')
+    limit: Optional[int] = Field(default=None, description='Limit', title='Limit')
     nextPage: Optional[str] = Field(
-        None, description='Starting after', title='NextPage'
+        default=None, description='Starting after', title='NextPage'
     )
 
 
 class PaginationResponseSchema(BaseModel):
-    limit: Optional[int] = Field(-1, description='Limit', title='Limit')
+    limit: Optional[int] = Field(default=20, description='Limit', title='Limit')
     hasMore: Optional[bool] = Field(
-        None, description='Has more? `true` or `false`.', title='HasMore'
+        default=None, description='Has more? `true` or `false`.', title='HasMore'
     )
     nextPage: Optional[str] = Field(
-        None, description='Starting after', title='NextPage'
+        default=None, description='Starting after', title='NextPage'
     )
 
 
 class PermissionsExpansion(Enum):
     reviewer_user = 'reviewer.user'
 
 
@@ -347,47 +352,51 @@
 class SortSchemaFieldName(BaseModel):
     class Config:
         extra = Extra.forbid
 
     fieldName: FieldName = Field(
         ..., description='Sort By Field Name', title='FieldName'
     )
-    order: Optional[SortOrder] = Field('ASC', description='Sort Order', title='Order')
+    order: Optional[SortOrder] = Field(
+        default='ASC', description='Sort Order', title='Order'
+    )
 
 
 class SortSchemaSearchIncidentsSortFields(BaseModel):
     class Config:
         extra = Extra.forbid
 
     fieldName: SearchIncidentsSortFields = Field(
         ..., description='Sort By Field Name', title='FieldName'
     )
-    order: Optional[SortOrder] = Field('ASC', description='Sort Order', title='Order')
+    order: Optional[SortOrder] = Field(
+        default='ASC', description='Sort Order', title='Order'
+    )
 
 
 class SourceAppSchema(BaseModel):
     id: str = Field(..., description='Unique ID', title='Id')
     name: str = Field(..., description='Name', title='Name')
 
 
 class UpdateIncidentRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     assigneeId: Optional[str] = Field(
-        None,
+        default=None,
         description='ID of the entity assigned to this incident.',
         title='Assigneeid',
     )
     status: Optional[IncidentStatus] = Field(
-        None,
+        default=None,
         description='The status of the incident (Open, InProgress, WaitingForInput, or Closed).',
     )
     severity: Optional[IncidentSeverity] = Field(
-        None,
+        default=None,
         description='The severity of the incident (Low, Medium, High or Critical).',
     )
 
 
 class UserSchema(BaseModel):
     userId: str = Field(..., description='Unique ID', title='Userid')
     userFirstName: str = Field(..., description='First Name', title='Userfirstname')
@@ -399,58 +408,64 @@
     loc: List[str] = Field(..., title='Location')
     msg: str = Field(..., title='Message')
     type: str = Field(..., title='Error Type')
 
 
 class AicpaTsc2017(BaseModel):
     values: List[AicpaTsc2017Standard] = Field(..., description='Values')
-    id: Optional[str] = Field('aicpaTsc2017', description='UniqueID', title='Id')
-    name: Optional[str] = Field('SOC 2 (TSC 2017)', description='Name', title='Name')
+    id: Optional[str] = Field(
+        default='aicpaTsc2017', description='UniqueID', title='Id'
+    )
+    name: Optional[str] = Field(
+        default='SOC 2 (TSC 2017)', description='Name', title='Name'
+    )
 
 
 class BasicEnumFilterCampaignStatus(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_in: Optional[List[CampaignStatus]] = Field(
-        None, alias='$in', description='In'
+        default=None, alias='$in', description='In'
     )
 
 
 class BasicEnumFilterIncidentSeverity(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_in: Optional[List[IncidentSeverity]] = Field(
-        None, alias='$in', description='In'
+        default=None, alias='$in', description='In'
     )
 
 
 class BasicEnumFilterIncidentStatus(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_in: Optional[List[IncidentStatus]] = Field(
-        None, alias='$in', description='In'
+        default=None, alias='$in', description='In'
     )
 
 
 class BasicEnumFilterSelection(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[Selection]] = Field(None, alias='$in', description='In')
+    field_in: Optional[List[Selection]] = Field(
+        default=None, alias='$in', description='In'
+    )
 
 
 class CampaignPermissionsSearchFilterBody(BaseModel):
     class Config:
         extra = Extra.forbid
 
     decision: Optional[BasicEnumFilterSelection] = Field(
-        None,
+        default=None,
         description='Reviewer decisions (keep, revoke or null).\n',
         title='Decision',
     )
 
 
 class CampaignSchema(BaseModel):
     id: str = Field(..., description='Unique ID of campaign', title='Id')
@@ -465,81 +480,87 @@
     createdAt: datetime = Field(
         ..., description='Time of creation of campaign', title='Createdat'
     )
     ownerUserId: str = Field(
         ..., description='User ID of the campaign owner', title='Owneruserid'
     )
     owner: Optional[UserSchema] = Field(
-        None, description='User Schema of the campaign owner', title='Owner'
+        default=None, description='User Schema of the campaign owner', title='Owner'
     )
 
 
 class CampaignSearchFilterBody(BaseModel):
     class Config:
         extra = Extra.forbid
 
     status: Optional[BasicEnumFilterCampaignStatus] = Field(
-        None,
+        default=None,
         description='Enum: "draft" "initializing" "running" "completed" "failed" "empty" "overdue"\n',
         title='Status',
     )
 
 
 class Ccm301(BaseModel):
     values: List[Ccm301Standard] = Field(..., description='Values')
-    id: Optional[str] = Field('ccm301', description='UniqueID', title='Id')
+    id: Optional[str] = Field(default='ccm301', description='UniqueID', title='Id')
     name: Optional[str] = Field(
-        'CSA STAR (CCM 3.0.1)', description='Name', title='Name'
+        default='CSA STAR (CCM 3.0.1)', description='Name', title='Name'
     )
 
 
 class Ccm402(BaseModel):
     values: List[Ccm402Standard] = Field(..., description='Values')
-    id: Optional[str] = Field('ccm402', description='UniqueID', title='Id')
+    id: Optional[str] = Field(default='ccm402', description='UniqueID', title='Id')
     name: Optional[str] = Field(
-        'CSA STAR (CCM 4.0.2)', description='Name', title='Name'
+        default='CSA STAR (CCM 4.0.2)', description='Name', title='Name'
     )
 
 
 class HTTPValidationError(BaseModel):
-    detail: Optional[List[ValidationError]] = Field(None, title='Detail')
+    detail: Optional[List[ValidationError]] = Field(default=None, title='Detail')
 
 
 class IncidentEntitiesSchema(BaseModel):
     id: str = Field(..., description='Unique id of entity.', title='Id')
-    name: Optional[str] = Field(None, description='Name of entity.', title='Name')
+    name: Optional[str] = Field(
+        default=None, description='Name of entity.', title='Name'
+    )
     object: Union[InventoryObjects, str] = Field(
         ..., description='Identity | Account | Asset', title='Object'
     )
-    email: Optional[str] = Field(None, description='Email', title='Email')
-    originId: Optional[str] = Field(None, description='Origin ID', title='Originid')
+    email: Optional[str] = Field(default=None, description='Email', title='Email')
+    originId: Optional[str] = Field(
+        default=None, description='Origin ID', title='Originid'
+    )
     originType: Optional[str] = Field(
-        None, description='Origin Type', title='Origintype'
+        default=None, description='Origin Type', title='Origintype'
     )
 
 
 class IsoIec27001(BaseModel):
     values: List[IsoIec27001Standard] = Field(..., description='Values')
-    id: Optional[str] = Field('isoIec27001', description='UniqueID', title='Id')
-    name: Optional[str] = Field('ISO/IEC 27001', description='Name', title='Name')
+    id: Optional[str] = Field(default='isoIec27001', description='UniqueID', title='Id')
+    name: Optional[str] = Field(
+        default='ISO/IEC 27001', description='Name', title='Name'
+    )
 
 
 class NonPaginatedResponseSchemaCampaignSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     data: CampaignSchema = Field(..., description='Actual Data', title='Data')
 
 
 class PaginatedResponseSchemaCampaignSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationResponseSchema] = Field(
-        None, description='Pagination Metadata', title='Pagination'
+        default=None, description='Pagination Metadata', title='Pagination'
     )
     data: List[CampaignSchema] = Field(
         ..., description='List of Actual Data', title='Data'
     )
 
 
 class ReviewerSchema(BaseModel):
@@ -552,100 +573,104 @@
         ..., description='Time of last activity', title='Lastactiveat'
     )
     reviewStatus: Union[ReviewStatus, str] = Field(
         ..., description='Review Status', title='Reviewstatus'
     )
     id: str = Field(..., description='Unique ID', title='Id')
     user: Optional[UserSchema] = Field(
-        None, description='User Schema of the reviewer', title='User'
+        default=None, description='User Schema of the reviewer', title='User'
     )
 
 
 class SearchCampaignPermissionsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationRequestSchema] = Field(
-        None, description='Pagination', title='Pagination'
+        default=None, description='Pagination', title='Pagination'
     )
     filter: Optional[CampaignPermissionsSearchFilterBody] = Field(
-        None, description='Filter by the reviewer decisions. \n', title='Filter'
+        default=None, description='Filter by the reviewer decisions. \n', title='Filter'
     )
     expand: Optional[List[PermissionsExpansion]] = Field(
-        None, description='Fields to expand.\n'
+        default=None, description='Fields to expand.\n'
     )
 
 
 class SearchCampaignsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     filter: Optional[CampaignSearchFilterBody] = Field(
-        None, description='Status filter', title='Filter'
+        default=None, description='Status filter', title='Filter'
+    )
+    expand: Optional[List[CampaignExpansion]] = Field(
+        default=None, description='Expand Fields'
     )
-    expand: Optional[List[CampaignExpansion]] = Field(None, description='Expand Fields')
     pagination: Optional[PaginationRequestSchema] = Field(
-        None, description='Pagination', title='Pagination'
+        default=None, description='Pagination', title='Pagination'
     )
     sort: Optional[List[SortSchemaFieldName]] = Field(
-        None, description='Sort', title='Sort'
+        default=None, description='Sort', title='Sort'
     )
 
 
 class SearchIncidentsFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     createdAt: Optional[BaseDateFilter] = Field(
-        None, description='Created At date', title='Createdat'
+        default=None, description='Created At date', title='Createdat'
     )
     updatedAt: Optional[BaseDateFilter] = Field(
-        None, description='Updated At date', title='Updatedat'
+        default=None, description='Updated At date', title='Updatedat'
     )
     severity: Optional[BasicEnumFilterIncidentSeverity] = Field(
-        None, description='Severity', title='Severity'
+        default=None, description='Severity', title='Severity'
     )
     status: Optional[BasicEnumFilterIncidentStatus] = Field(
-        None, description='Status', title='Status'
+        default=None, description='Status', title='Status'
     )
     policyId: Optional[BaseSingleValuedStringFilter] = Field(
-        None, description='Policy Id ', title='Policyid'
+        default=None, description='Policy Id ', title='Policyid'
     )
     policyTemplateId: Optional[BaseSingleValuedStringFilter] = Field(
-        None, description='Policy Template ID', title='Policytemplateid'
+        default=None, description='Policy Template ID', title='Policytemplateid'
     )
     isResolved: Optional[BaseBooleanFilter] = Field(
-        None, description='Is resolved?', title='Isresolved'
+        default=None, description='Is resolved?', title='Isresolved'
     )
 
 
 class SearchIncidentsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     filter: Optional[SearchIncidentsFilter] = Field(
-        None, description='Filter', title='Filter'
+        default=None, description='Filter', title='Filter'
+    )
+    expand: Optional[List[IncidentExpansion]] = Field(
+        default=None, description='Expend'
     )
-    expand: Optional[List[IncidentExpansion]] = Field(None, description='Expend')
     sort: Optional[List[SortSchemaSearchIncidentsSortFields]] = Field(
-        None, description='Sort', title='Sort'
+        default=None, description='Sort', title='Sort'
     )
     pagination: Optional[PaginationRequestSchema] = Field(
-        None, description='Pagination', title='Pagination'
+        default=None, description='Pagination', title='Pagination'
     )
 
 
 class CampaignsPermissionSchema(BaseModel):
     id: str = Field(..., description='Campaign ID (unique). \n', title='Id')
     campaignId: str = Field(
         ..., description='ID of the Campaign.\n', title='Campaignid'
     )
     reviewerId: str = Field(..., description='Reviewer ID', title='Reviewerid')
     reviewer: Optional[ReviewerSchema] = Field(
-        None, description='Details of the reviewer.\n', title='Reviewer'
+        default=None, description='Details of the reviewer.\n', title='Reviewer'
     )
     accessById: str = Field(
         ...,
         description='Access by ID (Account or Grouping ID) that their access was reviewed. \n',
         title='Accessbyid',
     )
     accessByType: AccessByType = Field(
@@ -656,71 +681,77 @@
         ...,
         description='Access to ID (Asset or Grouping ID) that the access to was reviewed, for example a database the access to was reviewed.  \n',
         title='Accesstoid',
     )
     accessToType: AccessToType = Field(
         ..., description='Assets or grouping that the access to was reviewed.  \n'
     )
-    privilegeId: str = Field(
-        ...,
+    privilegeId: Optional[str] = Field(
+        default=None,
         description='ID of the privileges that was reviewed. \n',
         title='Privilegeid',
     )
     decision: Optional[Selection] = Field(
-        None, description='Reviewer decisions (keep, revoke or null).\n'
+        default=None, description='Reviewer decisions (keep, revoke or null).\n'
     )
     decisionReason: Optional[str] = Field(
-        None,
+        default=None,
         description='Reviewer decision for keeping or revoking the reviewed access.  \n',
         title='Decisionreason',
     )
 
 
 class IncidentSchema(BaseModel):
     id: str = Field(..., description='Unique id', title='Id')
     createdAt: Optional[datetime] = Field(
-        None, description='The date the incident was first reported.', title='Createdat'
+        default=None,
+        description='The date the incident was first reported.',
+        title='Createdat',
     )
     updatedAt: Optional[datetime] = Field(
-        None, description='The date the incident was last updated.', title='Updatedat'
+        default=None,
+        description='The date the incident was last updated.',
+        title='Updatedat',
     )
     entities: Optional[List[IncidentEntitiesSchema]] = Field(
-        [], description='Entity', title='Entities'
+        default=[], description='Entity', title='Entities'
     )
     apps: Optional[List[SourceAppSchema]] = Field(
-        [], description='Applications', title='Apps'
+        default=[], description='Applications', title='Apps'
     )
-    category: Optional[AlertCategoryType] = Field(None, description='Category')
-    tactics: Optional[List[AttackTacticType]] = Field([], description='Tactics')
+    category: Optional[AlertCategoryType] = Field(default=None, description='Category')
+    tactics: Optional[List[AttackTacticType]] = Field(default=[], description='Tactics')
     compliance: Optional[
         List[Union[IsoIec27001, AicpaTsc2017, Ccm402, Ccm301, Cisv8]]
-    ] = Field([], description='Compliance', title='Compliance')
+    ] = Field(default=[], description='Compliance', title='Compliance')
     techniques: Optional[List[str]] = Field(
-        [], description='Techniques', title='Techniques'
+        default=[], description='Techniques', title='Techniques'
     )
     status: Optional[IncidentStatus] = Field(
-        None,
+        default=None,
         description='The status of the incident (Open, In Progress, Waiting for Input, or Closed)',
     )
     severity: IncidentSeverity = Field(
         ..., description='The severity of the incident (Low, Medium, High or Critical).'
     )
     policyId: str = Field(..., description='Unique id of policy.', title='Policyid')
-    policy: Optional[PolicySchema] = Field(None, description='Policy', title='Policy')
+    policy: Optional[PolicySchema] = Field(
+        default=None, description='Policy', title='Policy'
+    )
     assigneeId: Optional[str] = Field(
-        None, description='Unique id of assignee.', title='Assigneeid'
+        default=None, description='Unique id of assignee.', title='Assigneeid'
     )
     assignee: Optional[UserSchema] = Field(
-        None, description='Assignee', title='Assignee'
+        default=None, description='Assignee', title='Assignee'
     )
     recommendation: Optional[str] = Field(
-        None, description='Recommendation', title='Recommendation'
+        default=None, description='Recommendation', title='Recommendation'
     )
     description: Optional[str] = Field(
-        None, description='Description', title='Description'
+        default=None, description='Description', title='Description'
     )
     isResolved: bool = Field(..., description='Is Resolved?', title='Isresolved')
     url: str = Field(..., description='URL', title='Url')
 
 
 class NonPaginatedResponseSchemaIncidentSchema(BaseModel):
     class Config:
@@ -737,24 +768,24 @@
 
 
 class PaginatedResponseSchemaCampaignsPermissionSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationResponseSchema] = Field(
-        None, description='Pagination Metadata', title='Pagination'
+        default=None, description='Pagination Metadata', title='Pagination'
     )
     data: List[CampaignsPermissionSchema] = Field(
         ..., description='List of Actual Data', title='Data'
     )
 
 
 class PaginatedResponseSchemaIncidentSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationResponseSchema] = Field(
-        None, description='Pagination Metadata', title='Pagination'
+        default=None, description='Pagination Metadata', title='Pagination'
     )
     data: List[IncidentSchema] = Field(
         ..., description='List of Actual Data', title='Data'
     )
```

### Comparing `authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9872463830372645%*

 * *Differences: {"'components'": "{'schemas': {'GroupingSchema': {'properties': {'owner': {'description': 'The "*

 * *                 'uniqueId of the user who is the "owner" (or manager) of the group.\\n\'}}}, '*

 * *                 "'NewGroupingRequestSchema': {'properties': {'owner': {'description': 'The "*

 * *                 'uniqueId of the user who is the "owner" (or manager) of the group.\\n\'}}}, '*

 * *                 "'UpdateGroupingsRequestSchema': {'properties': {'owner': {'description': 'The "*

 * *                 'uniqueId of t […]*

```diff
@@ -452,15 +452,15 @@
                     },
                     "originType": {
                         "description": "The name of the type of grouping in the source system. The default is `Group`. Example: Group/Alias/AWS Role\n",
                         "title": "Origintype",
                         "type": "string"
                     },
                     "owner": {
-                        "description": "The owner ID",
+                        "description": "The uniqueId of the user who is the \"owner\" (or manager) of the group.\n",
                         "title": "Owner",
                         "type": "string"
                     },
                     "tags": {
                         "description": "Tags on the access grouping.\n",
                         "items": {
                             "minLength": 1,
@@ -1439,15 +1439,15 @@
                     },
                     "originType": {
                         "description": "The name of the type of grouping in the source system. The default is `Group`. Example: Group/Alias/AWS Role\n",
                         "title": "Origintype",
                         "type": "string"
                     },
                     "owner": {
-                        "description": "The owner ID",
+                        "description": "The uniqueId of the user who is the \"owner\" (or manager) of the group.\n",
                         "title": "Owner",
                         "type": "string"
                     },
                     "tags": {
                         "description": "Tags on the access grouping.\n",
                         "items": {
                             "minLength": 1,
@@ -3210,15 +3210,15 @@
                     },
                     "originType": {
                         "description": "The name of the type of grouping in the source system. The default is `Group`. Example: Group/Alias/AWS Role\n",
                         "title": "Origintype",
                         "type": "string"
                     },
                     "owner": {
-                        "description": "The owner ID",
+                        "description": "The uniqueId of the user who is the \"owner\" (or manager) of the group.\n",
                         "title": "Owner",
                         "type": "string"
                     },
                     "tags": {
                         "description": "Tags on the access grouping.\n",
                         "items": {
                             "minLength": 1,
@@ -3246,14 +3246,46 @@
                 "required": [
                     "uniqueId",
                     "name"
                 ],
                 "title": "UpdateGroupingsRequestSchema",
                 "type": "object"
             },
+            "UpdateGroupingsResponseSchema": {
+                "description": "Update user response schema",
+                "properties": {
+                    "acceptedTimestamp": {
+                        "description": "**The accepted time of the request**",
+                        "format": "date-time",
+                        "title": "Acceptedtimestamp",
+                        "type": "string"
+                    },
+                    "data": {
+                        "default": {},
+                        "description": "Response data.",
+                        "title": "Data"
+                    },
+                    "numberOfAcceptedEntities": {
+                        "description": "**The number of entities that pass validation and uploaded**",
+                        "title": "Numberofacceptedentities",
+                        "type": "integer"
+                    },
+                    "requestId": {
+                        "description": "**Request id**",
+                        "title": "Requestid",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "requestId",
+                    "numberOfAcceptedEntities"
+                ],
+                "title": "UpdateGroupingsResponseSchema",
+                "type": "object"
+            },
             "UpdateIdentitiesListRequestSchema": {
                 "description": "List of update requests request schema",
                 "properties": {
                     "data": {
                         "description": "List of update identity requests.\n",
                         "items": {
                             "$ref": "#/components/schemas/UpdateIdentityRequestSchema"
@@ -3669,15 +3701,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "3.1.4",
+        "version": "3.1.5",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
@@ -4510,15 +4542,15 @@
                     "required": true
                 },
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
-                                    "$ref": "#/components/schemas/NewGroupingResponseSchema"
+                                    "$ref": "#/components/schemas/UpdateGroupingsResponseSchema"
                                 }
                             }
                         },
                         "description": "Successful Response"
                     },
                     "422": {
                         "content": {
@@ -5418,15 +5450,15 @@
                         "schema": {
                             "title": "Appid",
                             "type": "string"
                         }
                     },
                     {
                         "description": "Delete all the app data lastly updated before the given date.",
-                        "example": "2023-04-11T05:48:47.081171+00:00",
+                        "example": "2023-04-19T21:27:04.123723+00:00",
                         "in": "query",
                         "name": "modifiedBefore",
                         "required": false,
                         "schema": {
                             "description": "Delete all the app data lastly updated before the given date.",
                             "format": "date-time",
                             "title": "Modifiedbefore",
```

### Comparing `authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9749960542929292%*

 * *Differences: {"'components'": "{'schemas': {'CampaignsPermissionSchema': {'required': {delete: [7]}}, "*

 * *                 "'MeResponse': {'properties': {'version': {'default': '3.1.5'}}}, "*

 * *                 "'PaginationResponseSchema': {'properties': {'limit': {'default': 20}}}}}",*

 * * "'info'": "{'description': 'Authomize enables users to integrate your applications with Authomize "*

 * *           'via custom connectors.\\n\\nYou can use the APIs described in this document to create '*

 * *           'your connector.\\n\\nOnce data […]*

```diff
@@ -426,16 +426,15 @@
                 "required": [
                     "id",
                     "campaignId",
                     "reviewerId",
                     "accessById",
                     "accessByType",
                     "accessToId",
-                    "accessToType",
-                    "privilegeId"
+                    "accessToType"
                 ],
                 "title": "CampaignsPermissionSchema",
                 "type": "object"
             },
             "Ccm301": {
                 "properties": {
                     "id": {
@@ -973,15 +972,15 @@
                     },
                     "tenant": {
                         "description": "**tenant**",
                         "title": "Tenant",
                         "type": "string"
                     },
                     "version": {
-                        "default": "3.1.2",
+                        "default": "3.1.5",
                         "description": "**version**",
                         "title": "Version",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
@@ -1170,15 +1169,15 @@
                 "properties": {
                     "hasMore": {
                         "description": "Has more? `true` or `false`.",
                         "title": "HasMore",
                         "type": "boolean"
                     },
                     "limit": {
-                        "default": -1,
+                        "default": 20,
                         "description": "Limit",
                         "title": "Limit",
                         "type": "integer"
                     },
                     "nextPage": {
                         "description": "Starting after",
                         "title": "NextPage",
@@ -1690,17 +1689,17 @@
                 "in": "header",
                 "name": "Authorization",
                 "type": "apiKey"
             }
         }
     },
     "info": {
-        "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n",
+        "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "3.1.2",
+        "version": "3.1.5",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
```

### Comparing `authomize-rest-api-client-3.1.5/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-3.1.6/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.5/setup.py` & `authomize-rest-api-client-3.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='3.1.5',
+        version='3.1.6',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

