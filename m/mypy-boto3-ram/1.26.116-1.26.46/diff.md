# Comparing `tmp/mypy-boto3-ram-1.26.116.tar.gz` & `tmp/mypy-boto3-ram-1.26.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ram-1.26.116.tar", last modified: Wed Apr 19 19:32:44 2023, max compression
+gzip compressed data, was "mypy-boto3-ram-1.26.46.tar", last modified: Mon Jan  9 20:27:39 2023, max compression
```

## Comparing `mypy-boto3-ram-1.26.116.tar` & `mypy-boto3-ram-1.26.46.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:32:44.093006 mypy-boto3-ram-1.26.116/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-19 19:32:07.000000 mypy-boto3-ram-1.26.116/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-04-19 19:32:44.093006 mypy-boto3-ram-1.26.116/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-04-19 19:32:07.000000 mypy-boto3-ram-1.26.116/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:32:44.089006 mypy-boto3-ram-1.26.116/mypy_boto3_ram/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-19 19:32:07.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-19 19:32:07.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-19 19:32:07.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31754 2023-04-19 19:32:07.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31707 2023-04-19 19:32:07.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-04-19 19:32:08.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-04-19 19:32:08.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-04-19 19:32:07.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-04-19 19:32:07.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:32:07.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40995 2023-04-19 19:32:09.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40930 2023-04-19 19:32:08.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-19 19:32:07.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:32:44.089006 mypy-boto3-ram-1.26.116/mypy_boto3_ram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-04-19 19:32:43.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-19 19:32:43.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:32:43.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:32:43.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-19 19:32:43.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 19:32:43.000000 mypy-boto3-ram-1.26.116/mypy_boto3_ram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:32:44.093006 mypy-boto3-ram-1.26.116/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-19 19:32:07.000000 mypy-boto3-ram-1.26.116/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.372431 mypy-boto3-ram-1.26.46/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16555 2023-01-09 20:27:39.372431 mypy-boto3-ram-1.26.46/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.372431 mypy-boto3-ram-1.26.46/mypy_boto3_ram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24209 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30603 2023-01-09 20:27:29.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30556 2023-01-09 20:27:29.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.372431 mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16555 2023-01-09 20:27:39.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-09 20:27:39.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:27:39.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:27:39.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-09 20:27:39.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-09 20:27:39.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 20:27:39.372431 mypy-boto3-ram-1.26.46/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/setup.py
```

### Comparing `mypy-boto3-ram-1.26.116/LICENSE` & `mypy-boto3-ram-1.26.46/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-ram-1.26.116/PKG-INFO` & `mypy-boto3-ram-1.26.46/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ram
-Version: 1.26.116
-Summary: Type annotations for boto3.RAM 1.26.116 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.46
+Summary: Type annotations for boto3.RAM 1.26.46 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ram"></a>
 
 # mypy-boto3-ram
 
 [![PyPI - mypy-boto3-ram](https://img.shields.io/pypi/v/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ram?color=blue)](https://pypistats.org/packages/mypy-boto3-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RAM 1.26.116](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[boto3.RAM 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ram docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,19 +321,14 @@
 from mypy_boto3_ram.literals import (
     GetResourcePoliciesPaginatorName,
     GetResourceShareAssociationsPaginatorName,
     GetResourceShareInvitationsPaginatorName,
     GetResourceSharesPaginatorName,
     ListPrincipalsPaginatorName,
     ListResourcesPaginatorName,
-    PermissionFeatureSetType,
-    PermissionStatusType,
-    PermissionTypeFilterType,
-    PermissionTypeType,
-    ReplacePermissionAssociationsWorkStatusType,
     ResourceOwnerType,
     ResourceRegionScopeFilterType,
     ResourceRegionScopeType,
     ResourceShareAssociationStatusType,
     ResourceShareAssociationTypeType,
     ResourceShareFeatureSetType,
     ResourceShareInvitationStatusType,
@@ -361,91 +356,71 @@
 ```python
 from mypy_boto3_ram.type_defs import (
     AcceptResourceShareInvitationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateResourceSharePermissionRequestRequestTypeDef,
     AssociateResourceShareRequestRequestTypeDef,
     ResourceShareAssociationTypeDef,
-    AssociatedPermissionTypeDef,
     TagTypeDef,
-    CreatePermissionVersionRequestRequestTypeDef,
-    DeletePermissionRequestRequestTypeDef,
-    DeletePermissionVersionRequestRequestTypeDef,
     DeleteResourceShareRequestRequestTypeDef,
     DisassociateResourceSharePermissionRequestRequestTypeDef,
     DisassociateResourceShareRequestRequestTypeDef,
     GetPermissionRequestRequestTypeDef,
+    ResourceSharePermissionDetailTypeDef,
     PaginatorConfigTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourceShareAssociationsRequestRequestTypeDef,
     GetResourceShareInvitationsRequestRequestTypeDef,
     TagFilterTypeDef,
     ListPendingInvitationResourcesRequestRequestTypeDef,
     ResourceTypeDef,
-    ListPermissionAssociationsRequestRequestTypeDef,
     ListPermissionVersionsRequestRequestTypeDef,
+    ResourceSharePermissionSummaryTypeDef,
     ListPermissionsRequestRequestTypeDef,
     ListPrincipalsRequestRequestTypeDef,
     PrincipalTypeDef,
-    ListReplacePermissionAssociationsWorkRequestRequestTypeDef,
-    ReplacePermissionAssociationsWorkTypeDef,
     ListResourceSharePermissionsRequestRequestTypeDef,
     ListResourceTypesRequestRequestTypeDef,
     ServiceNameAndResourceTypeTypeDef,
     ListResourcesRequestRequestTypeDef,
-    PromotePermissionCreatedFromPolicyRequestRequestTypeDef,
     PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef,
     RejectResourceShareInvitationRequestRequestTypeDef,
-    ReplacePermissionAssociationsRequestRequestTypeDef,
-    SetDefaultPermissionVersionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateResourceShareRequestRequestTypeDef,
     AssociateResourceSharePermissionResponseTypeDef,
-    DeletePermissionResponseTypeDef,
-    DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareResponseTypeDef,
     DisassociateResourceSharePermissionResponseTypeDef,
     EnableSharingWithAwsOrganizationResponseTypeDef,
     GetResourcePoliciesResponseTypeDef,
     PromoteResourceShareCreatedFromPolicyResponseTypeDef,
-    SetDefaultPermissionVersionResponseTypeDef,
     AssociateResourceShareResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     ResourceShareInvitationTypeDef,
-    ListPermissionAssociationsResponseTypeDef,
-    CreatePermissionRequestRequestTypeDef,
     CreateResourceShareRequestRequestTypeDef,
-    ResourceSharePermissionDetailTypeDef,
-    ResourceSharePermissionSummaryTypeDef,
     ResourceShareTypeDef,
     TagResourceRequestRequestTypeDef,
+    GetPermissionResponseTypeDef,
     GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
     GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
     ListPrincipalsRequestListPrincipalsPaginateTypeDef,
     ListResourcesRequestListResourcesPaginateTypeDef,
     GetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     GetResourceSharesRequestRequestTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
     ListResourcesResponseTypeDef,
+    ListPermissionVersionsResponseTypeDef,
+    ListPermissionsResponseTypeDef,
+    ListResourceSharePermissionsResponseTypeDef,
     ListPrincipalsResponseTypeDef,
-    ListReplacePermissionAssociationsWorkResponseTypeDef,
-    ReplacePermissionAssociationsResponseTypeDef,
     ListResourceTypesResponseTypeDef,
     AcceptResourceShareInvitationResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
-    CreatePermissionVersionResponseTypeDef,
-    GetPermissionResponseTypeDef,
-    CreatePermissionResponseTypeDef,
-    ListPermissionVersionsResponseTypeDef,
-    ListPermissionsResponseTypeDef,
-    ListResourceSharePermissionsResponseTypeDef,
-    PromotePermissionCreatedFromPolicyResponseTypeDef,
     CreateResourceShareResponseTypeDef,
     GetResourceSharesResponseTypeDef,
     UpdateResourceShareResponseTypeDef,
 )
 
 
 def get_structure() -> AcceptResourceShareInvitationRequestRequestTypeDef:
@@ -455,42 +430,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-ram-1.26.116/README.md` & `mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-ram
+Version: 1.26.46
+Summary: Type annotations for boto3.RAM 1.26.46 service generated with mypy-boto3-builder 7.12.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 ram type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-ram"></a>
 
 # mypy-boto3-ram
 
 [![PyPI - mypy-boto3-ram](https://img.shields.io/pypi/v/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ram?color=blue)](https://pypistats.org/packages/mypy-boto3-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RAM 1.26.116](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[boto3.RAM 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ram docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,19 +321,14 @@
 from mypy_boto3_ram.literals import (
     GetResourcePoliciesPaginatorName,
     GetResourceShareAssociationsPaginatorName,
     GetResourceShareInvitationsPaginatorName,
     GetResourceSharesPaginatorName,
     ListPrincipalsPaginatorName,
     ListResourcesPaginatorName,
-    PermissionFeatureSetType,
-    PermissionStatusType,
-    PermissionTypeFilterType,
-    PermissionTypeType,
-    ReplacePermissionAssociationsWorkStatusType,
     ResourceOwnerType,
     ResourceRegionScopeFilterType,
     ResourceRegionScopeType,
     ResourceShareAssociationStatusType,
     ResourceShareAssociationTypeType,
     ResourceShareFeatureSetType,
     ResourceShareInvitationStatusType,
@@ -329,91 +356,71 @@
 ```python
 from mypy_boto3_ram.type_defs import (
     AcceptResourceShareInvitationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateResourceSharePermissionRequestRequestTypeDef,
     AssociateResourceShareRequestRequestTypeDef,
     ResourceShareAssociationTypeDef,
-    AssociatedPermissionTypeDef,
     TagTypeDef,
-    CreatePermissionVersionRequestRequestTypeDef,
-    DeletePermissionRequestRequestTypeDef,
-    DeletePermissionVersionRequestRequestTypeDef,
     DeleteResourceShareRequestRequestTypeDef,
     DisassociateResourceSharePermissionRequestRequestTypeDef,
     DisassociateResourceShareRequestRequestTypeDef,
     GetPermissionRequestRequestTypeDef,
+    ResourceSharePermissionDetailTypeDef,
     PaginatorConfigTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourceShareAssociationsRequestRequestTypeDef,
     GetResourceShareInvitationsRequestRequestTypeDef,
     TagFilterTypeDef,
     ListPendingInvitationResourcesRequestRequestTypeDef,
     ResourceTypeDef,
-    ListPermissionAssociationsRequestRequestTypeDef,
     ListPermissionVersionsRequestRequestTypeDef,
+    ResourceSharePermissionSummaryTypeDef,
     ListPermissionsRequestRequestTypeDef,
     ListPrincipalsRequestRequestTypeDef,
     PrincipalTypeDef,
-    ListReplacePermissionAssociationsWorkRequestRequestTypeDef,
-    ReplacePermissionAssociationsWorkTypeDef,
     ListResourceSharePermissionsRequestRequestTypeDef,
     ListResourceTypesRequestRequestTypeDef,
     ServiceNameAndResourceTypeTypeDef,
     ListResourcesRequestRequestTypeDef,
-    PromotePermissionCreatedFromPolicyRequestRequestTypeDef,
     PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef,
     RejectResourceShareInvitationRequestRequestTypeDef,
-    ReplacePermissionAssociationsRequestRequestTypeDef,
-    SetDefaultPermissionVersionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateResourceShareRequestRequestTypeDef,
     AssociateResourceSharePermissionResponseTypeDef,
-    DeletePermissionResponseTypeDef,
-    DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareResponseTypeDef,
     DisassociateResourceSharePermissionResponseTypeDef,
     EnableSharingWithAwsOrganizationResponseTypeDef,
     GetResourcePoliciesResponseTypeDef,
     PromoteResourceShareCreatedFromPolicyResponseTypeDef,
-    SetDefaultPermissionVersionResponseTypeDef,
     AssociateResourceShareResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     ResourceShareInvitationTypeDef,
-    ListPermissionAssociationsResponseTypeDef,
-    CreatePermissionRequestRequestTypeDef,
     CreateResourceShareRequestRequestTypeDef,
-    ResourceSharePermissionDetailTypeDef,
-    ResourceSharePermissionSummaryTypeDef,
     ResourceShareTypeDef,
     TagResourceRequestRequestTypeDef,
+    GetPermissionResponseTypeDef,
     GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
     GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
     ListPrincipalsRequestListPrincipalsPaginateTypeDef,
     ListResourcesRequestListResourcesPaginateTypeDef,
     GetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     GetResourceSharesRequestRequestTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
     ListResourcesResponseTypeDef,
+    ListPermissionVersionsResponseTypeDef,
+    ListPermissionsResponseTypeDef,
+    ListResourceSharePermissionsResponseTypeDef,
     ListPrincipalsResponseTypeDef,
-    ListReplacePermissionAssociationsWorkResponseTypeDef,
-    ReplacePermissionAssociationsResponseTypeDef,
     ListResourceTypesResponseTypeDef,
     AcceptResourceShareInvitationResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
-    CreatePermissionVersionResponseTypeDef,
-    GetPermissionResponseTypeDef,
-    CreatePermissionResponseTypeDef,
-    ListPermissionVersionsResponseTypeDef,
-    ListPermissionsResponseTypeDef,
-    ListResourceSharePermissionsResponseTypeDef,
-    PromotePermissionCreatedFromPolicyResponseTypeDef,
     CreateResourceShareResponseTypeDef,
     GetResourceSharesResponseTypeDef,
     UpdateResourceShareResponseTypeDef,
 )
 
 
 def get_structure() -> AcceptResourceShareInvitationRequestRequestTypeDef:
@@ -423,42 +430,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-ram-1.26.116/mypy_boto3_ram/__init__.py` & `mypy-boto3-ram-1.26.46/mypy_boto3_ram/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.26.116/mypy_boto3_ram/__init__.pyi` & `mypy-boto3-ram-1.26.46/mypy_boto3_ram/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.26.116/mypy_boto3_ram/__main__.py` & `mypy-boto3-ram-1.26.46/mypy_boto3_ram/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RAM 1.26.116\nVersion:         1.26.116\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.RAM 1.26.46\nVersion:         1.26.46\nBuilder version:"
+        " 7.12.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.116")
+    print("1.26.46")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ram-1.26.116/mypy_boto3_ram/client.py` & `mypy-boto3-ram-1.26.46/mypy_boto3_ram/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
-    PermissionFeatureSetType,
-    PermissionTypeFilterType,
-    ReplacePermissionAssociationsWorkStatusType,
     ResourceOwnerType,
     ResourceRegionScopeFilterType,
     ResourceShareAssociationStatusType,
     ResourceShareAssociationTypeType,
     ResourceShareStatusType,
 )
 from .paginator import (
@@ -36,42 +33,33 @@
     ListPrincipalsPaginator,
     ListResourcesPaginator,
 )
 from .type_defs import (
     AcceptResourceShareInvitationResponseTypeDef,
     AssociateResourceSharePermissionResponseTypeDef,
     AssociateResourceShareResponseTypeDef,
-    CreatePermissionResponseTypeDef,
-    CreatePermissionVersionResponseTypeDef,
     CreateResourceShareResponseTypeDef,
-    DeletePermissionResponseTypeDef,
-    DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareResponseTypeDef,
     DisassociateResourceSharePermissionResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     EnableSharingWithAwsOrganizationResponseTypeDef,
     GetPermissionResponseTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     GetResourceSharesResponseTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
-    ListPermissionAssociationsResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListPermissionVersionsResponseTypeDef,
     ListPrincipalsResponseTypeDef,
-    ListReplacePermissionAssociationsWorkResponseTypeDef,
     ListResourceSharePermissionsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListResourceTypesResponseTypeDef,
-    PromotePermissionCreatedFromPolicyResponseTypeDef,
     PromoteResourceShareCreatedFromPolicyResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
-    ReplacePermissionAssociationsResponseTypeDef,
-    SetDefaultPermissionVersionResponseTypeDef,
     TagFilterTypeDef,
     TagTypeDef,
     UpdateResourceShareResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -93,37 +81,31 @@
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     InvalidClientTokenException: Type[BotocoreClientError]
     InvalidMaxResultsException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
-    InvalidPolicyException: Type[BotocoreClientError]
     InvalidResourceTypeException: Type[BotocoreClientError]
     InvalidStateTransitionException: Type[BotocoreClientError]
     MalformedArnException: Type[BotocoreClientError]
-    MalformedPolicyTemplateException: Type[BotocoreClientError]
     MissingRequiredParameterException: Type[BotocoreClientError]
     OperationNotPermittedException: Type[BotocoreClientError]
-    PermissionAlreadyExistsException: Type[BotocoreClientError]
-    PermissionLimitExceededException: Type[BotocoreClientError]
-    PermissionVersionsLimitExceededException: Type[BotocoreClientError]
     ResourceArnNotFoundException: Type[BotocoreClientError]
     ResourceShareInvitationAlreadyAcceptedException: Type[BotocoreClientError]
     ResourceShareInvitationAlreadyRejectedException: Type[BotocoreClientError]
     ResourceShareInvitationArnNotFoundException: Type[BotocoreClientError]
     ResourceShareInvitationExpiredException: Type[BotocoreClientError]
     ResourceShareLimitExceededException: Type[BotocoreClientError]
     ServerInternalException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     TagLimitExceededException: Type[BotocoreClientError]
     TagPolicyViolationException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnknownResourceException: Type[BotocoreClientError]
-    UnmatchedPolicyPermissionException: Type[BotocoreClientError]
 
 
 class RAMClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/)
     """
@@ -194,41 +176,14 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#close)
         """
 
-    def create_permission(
-        self,
-        *,
-        name: str,
-        resourceType: str,
-        policyTemplate: str,
-        clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
-    ) -> CreatePermissionResponseTypeDef:
-        """
-        Creates a customer managed permission for a specified resource type that you can
-        attach to resource shares.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_permission)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#create_permission)
-        """
-
-    def create_permission_version(
-        self, *, permissionArn: str, policyTemplate: str, clientToken: str = ...
-    ) -> CreatePermissionVersionResponseTypeDef:
-        """
-        Creates a new version of the specified customer managed permission.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_permission_version)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#create_permission_version)
-        """
-
     def create_resource_share(
         self,
         *,
         name: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         tags: Sequence[TagTypeDef] = ...,
@@ -239,35 +194,14 @@
         """
         Creates a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#create_resource_share)
         """
 
-    def delete_permission(
-        self, *, permissionArn: str, clientToken: str = ...
-    ) -> DeletePermissionResponseTypeDef:
-        """
-        Deletes the specified customer managed permission in the Amazon Web Services
-        Region in which you call this operation.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_permission)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#delete_permission)
-        """
-
-    def delete_permission_version(
-        self, *, permissionArn: str, permissionVersion: int, clientToken: str = ...
-    ) -> DeletePermissionVersionResponseTypeDef:
-        """
-        Deletes one version of a customer managed permission.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_permission_version)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#delete_permission_version)
-        """
-
     def delete_resource_share(
         self, *, resourceShareArn: str, clientToken: str = ...
     ) -> DeleteResourceShareResponseTypeDef:
         """
         Deletes the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_resource_share)
@@ -279,26 +213,26 @@
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         clientToken: str = ...
     ) -> DisassociateResourceShareResponseTypeDef:
         """
-        Removes the specified principals or resources from participating in the
-        specified resource share.
+        Disassociates the specified principals or resources from the specified resource
+        share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#disassociate_resource_share)
         """
 
     def disassociate_resource_share_permission(
         self, *, resourceShareArn: str, permissionArn: str, clientToken: str = ...
     ) -> DisassociateResourceSharePermissionResponseTypeDef:
         """
-        Removes a managed permission from a resource share.
+        Disassociates an RAM permission from a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#disassociate_resource_share_permission)
         """
 
     def enable_sharing_with_aws_organization(
         self,
@@ -324,15 +258,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#generate_presigned_url)
         """
 
     def get_permission(
         self, *, permissionArn: str, permissionVersion: int = ...
     ) -> GetPermissionResponseTypeDef:
         """
-        Retrieves the contents of a managed permission in JSON format.
+        Gets the contents of an RAM permission in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_permission)
         """
 
     def get_resource_policies(
         self,
@@ -358,16 +292,16 @@
         resourceArn: str = ...,
         principal: str = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetResourceShareAssociationsResponseTypeDef:
         """
-        Retrieves the lists of resources and principals that associated for resource
-        shares that you own.
+        Retrieves the resource and principal associations for resource shares that you
+        own.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_share_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_resource_share_associations)
         """
 
     def get_resource_share_invitations(
         self,
@@ -390,16 +324,15 @@
         resourceOwner: ResourceOwnerType,
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        permissionArn: str = ...,
-        permissionVersion: int = ...
+        permissionArn: str = ...
     ) -> GetResourceSharesResponseTypeDef:
         """
         Retrieves details about the resource shares that you own or that are shared with
         you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_resource_shares)
@@ -417,51 +350,26 @@
         Lists the resources in a resource share that is shared with you but for which
         the invitation is still `PENDING`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_pending_invitation_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_pending_invitation_resources)
         """
 
-    def list_permission_associations(
-        self,
-        *,
-        permissionArn: str = ...,
-        permissionVersion: int = ...,
-        associationStatus: ResourceShareAssociationStatusType = ...,
-        resourceType: str = ...,
-        featureSet: PermissionFeatureSetType = ...,
-        defaultVersion: bool = ...,
-        nextToken: str = ...,
-        maxResults: int = ...
-    ) -> ListPermissionAssociationsResponseTypeDef:
-        """
-        Lists information about the managed permission and its associations to any
-        resource shares that use this managed permission.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permission_associations)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_permission_associations)
-        """
-
     def list_permission_versions(
         self, *, permissionArn: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListPermissionVersionsResponseTypeDef:
         """
         Lists the available versions of the specified RAM permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permission_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_permission_versions)
         """
 
     def list_permissions(
-        self,
-        *,
-        resourceType: str = ...,
-        nextToken: str = ...,
-        maxResults: int = ...,
-        permissionType: PermissionTypeFilterType = ...
+        self, *, resourceType: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> ListPermissionsResponseTypeDef:
         """
         Retrieves a list of available RAM permissions that you can use for the supported
         resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_permissions)
@@ -482,30 +390,14 @@
         Lists the principals that you are sharing resources with or that are sharing
         resources with you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_principals)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_principals)
         """
 
-    def list_replace_permission_associations_work(
-        self,
-        *,
-        workIds: Sequence[str] = ...,
-        status: ReplacePermissionAssociationsWorkStatusType = ...,
-        nextToken: str = ...,
-        maxResults: int = ...
-    ) -> ListReplacePermissionAssociationsWorkResponseTypeDef:
-        """
-        Retrieves the current status of the asynchronous tasks performed by RAM when you
-        perform the  ReplacePermissionAssociationsWork operation.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_replace_permission_associations_work)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_replace_permission_associations_work)
-        """
-
     def list_resource_share_permissions(
         self, *, resourceShareArn: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListResourceSharePermissionsResponseTypeDef:
         """
         Lists the RAM permissions that are associated with a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resource_share_permissions)
@@ -542,35 +434,20 @@
         Lists the resources that you added to a resource share or the resources that are
         shared with you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_resources)
         """
 
-    def promote_permission_created_from_policy(
-        self, *, permissionArn: str, name: str, clientToken: str = ...
-    ) -> PromotePermissionCreatedFromPolicyResponseTypeDef:
-        """
-        When you attach a resource-based policy to a resource, RAM automatically creates
-        a resource share of `featureSet`= `CREATED_FROM_POLICY` with a managed
-        permission that has the same IAM permissions as the original resource-based
-        policy.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.promote_permission_created_from_policy)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#promote_permission_created_from_policy)
-        """
-
     def promote_resource_share_created_from_policy(
         self, *, resourceShareArn: str
     ) -> PromoteResourceShareCreatedFromPolicyResponseTypeDef:
         """
-        When you attach a resource-based policy to a resource, RAM automatically creates
-        a resource share of `featureSet`= `CREATED_FROM_POLICY` with a managed
-        permission that has the same IAM permissions as the original resource-based
-        policy.
+        When you attach a resource-based permission policy to a resource, it
+        automatically creates a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.promote_resource_share_created_from_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#promote_resource_share_created_from_policy)
         """
 
     def reject_resource_share_invitation(
         self, *, resourceShareInvitationArn: str, clientToken: str = ...
@@ -579,58 +456,25 @@
         Rejects an invitation to a resource share from another Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.reject_resource_share_invitation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#reject_resource_share_invitation)
         """
 
-    def replace_permission_associations(
-        self,
-        *,
-        fromPermissionArn: str,
-        toPermissionArn: str,
-        fromPermissionVersion: int = ...,
-        clientToken: str = ...
-    ) -> ReplacePermissionAssociationsResponseTypeDef:
-        """
-        Updates all resource shares that use a managed permission to a different managed
-        permission.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.replace_permission_associations)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#replace_permission_associations)
-        """
-
-    def set_default_permission_version(
-        self, *, permissionArn: str, permissionVersion: int, clientToken: str = ...
-    ) -> SetDefaultPermissionVersionResponseTypeDef:
-        """
-        Designates the specified version number as the default version for the specified
-        customer managed permission.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.set_default_permission_version)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#set_default_permission_version)
-        """
-
-    def tag_resource(
-        self, *, tags: Sequence[TagTypeDef], resourceShareArn: str = ..., resourceArn: str = ...
-    ) -> Dict[str, Any]:
+    def tag_resource(self, *, resourceShareArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
-        Adds the specified tag keys and values to a resource share or managed
-        permission.
+        Adds the specified tag keys and values to the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#tag_resource)
         """
 
-    def untag_resource(
-        self, *, tagKeys: Sequence[str], resourceShareArn: str = ..., resourceArn: str = ...
-    ) -> Dict[str, Any]:
+    def untag_resource(self, *, resourceShareArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes the specified tag key and value pairs from the specified resource share
-        or managed permission.
+        Removes the specified tag key and value pairs from the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#untag_resource)
         """
 
     def update_resource_share(
         self,
```

### Comparing `mypy-boto3-ram-1.26.116/mypy_boto3_ram/client.pyi` & `mypy-boto3-ram-1.26.46/mypy_boto3_ram/client.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
-    PermissionFeatureSetType,
-    PermissionTypeFilterType,
-    ReplacePermissionAssociationsWorkStatusType,
     ResourceOwnerType,
     ResourceRegionScopeFilterType,
     ResourceShareAssociationStatusType,
     ResourceShareAssociationTypeType,
     ResourceShareStatusType,
 )
 from .paginator import (
@@ -36,42 +33,33 @@
     ListPrincipalsPaginator,
     ListResourcesPaginator,
 )
 from .type_defs import (
     AcceptResourceShareInvitationResponseTypeDef,
     AssociateResourceSharePermissionResponseTypeDef,
     AssociateResourceShareResponseTypeDef,
-    CreatePermissionResponseTypeDef,
-    CreatePermissionVersionResponseTypeDef,
     CreateResourceShareResponseTypeDef,
-    DeletePermissionResponseTypeDef,
-    DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareResponseTypeDef,
     DisassociateResourceSharePermissionResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     EnableSharingWithAwsOrganizationResponseTypeDef,
     GetPermissionResponseTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     GetResourceSharesResponseTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
-    ListPermissionAssociationsResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListPermissionVersionsResponseTypeDef,
     ListPrincipalsResponseTypeDef,
-    ListReplacePermissionAssociationsWorkResponseTypeDef,
     ListResourceSharePermissionsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListResourceTypesResponseTypeDef,
-    PromotePermissionCreatedFromPolicyResponseTypeDef,
     PromoteResourceShareCreatedFromPolicyResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
-    ReplacePermissionAssociationsResponseTypeDef,
-    SetDefaultPermissionVersionResponseTypeDef,
     TagFilterTypeDef,
     TagTypeDef,
     UpdateResourceShareResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -90,37 +78,31 @@
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     InvalidClientTokenException: Type[BotocoreClientError]
     InvalidMaxResultsException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
-    InvalidPolicyException: Type[BotocoreClientError]
     InvalidResourceTypeException: Type[BotocoreClientError]
     InvalidStateTransitionException: Type[BotocoreClientError]
     MalformedArnException: Type[BotocoreClientError]
-    MalformedPolicyTemplateException: Type[BotocoreClientError]
     MissingRequiredParameterException: Type[BotocoreClientError]
     OperationNotPermittedException: Type[BotocoreClientError]
-    PermissionAlreadyExistsException: Type[BotocoreClientError]
-    PermissionLimitExceededException: Type[BotocoreClientError]
-    PermissionVersionsLimitExceededException: Type[BotocoreClientError]
     ResourceArnNotFoundException: Type[BotocoreClientError]
     ResourceShareInvitationAlreadyAcceptedException: Type[BotocoreClientError]
     ResourceShareInvitationAlreadyRejectedException: Type[BotocoreClientError]
     ResourceShareInvitationArnNotFoundException: Type[BotocoreClientError]
     ResourceShareInvitationExpiredException: Type[BotocoreClientError]
     ResourceShareLimitExceededException: Type[BotocoreClientError]
     ServerInternalException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     TagLimitExceededException: Type[BotocoreClientError]
     TagPolicyViolationException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnknownResourceException: Type[BotocoreClientError]
-    UnmatchedPolicyPermissionException: Type[BotocoreClientError]
 
 class RAMClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/)
     """
 
@@ -184,39 +166,14 @@
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#close)
         """
-    def create_permission(
-        self,
-        *,
-        name: str,
-        resourceType: str,
-        policyTemplate: str,
-        clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
-    ) -> CreatePermissionResponseTypeDef:
-        """
-        Creates a customer managed permission for a specified resource type that you can
-        attach to resource shares.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_permission)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#create_permission)
-        """
-    def create_permission_version(
-        self, *, permissionArn: str, policyTemplate: str, clientToken: str = ...
-    ) -> CreatePermissionVersionResponseTypeDef:
-        """
-        Creates a new version of the specified customer managed permission.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_permission_version)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#create_permission_version)
-        """
     def create_resource_share(
         self,
         *,
         name: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         tags: Sequence[TagTypeDef] = ...,
@@ -226,33 +183,14 @@
     ) -> CreateResourceShareResponseTypeDef:
         """
         Creates a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#create_resource_share)
         """
-    def delete_permission(
-        self, *, permissionArn: str, clientToken: str = ...
-    ) -> DeletePermissionResponseTypeDef:
-        """
-        Deletes the specified customer managed permission in the Amazon Web Services
-        Region in which you call this operation.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_permission)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#delete_permission)
-        """
-    def delete_permission_version(
-        self, *, permissionArn: str, permissionVersion: int, clientToken: str = ...
-    ) -> DeletePermissionVersionResponseTypeDef:
-        """
-        Deletes one version of a customer managed permission.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_permission_version)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#delete_permission_version)
-        """
     def delete_resource_share(
         self, *, resourceShareArn: str, clientToken: str = ...
     ) -> DeleteResourceShareResponseTypeDef:
         """
         Deletes the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_resource_share)
@@ -263,25 +201,25 @@
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         clientToken: str = ...
     ) -> DisassociateResourceShareResponseTypeDef:
         """
-        Removes the specified principals or resources from participating in the
-        specified resource share.
+        Disassociates the specified principals or resources from the specified resource
+        share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#disassociate_resource_share)
         """
     def disassociate_resource_share_permission(
         self, *, resourceShareArn: str, permissionArn: str, clientToken: str = ...
     ) -> DisassociateResourceSharePermissionResponseTypeDef:
         """
-        Removes a managed permission from a resource share.
+        Disassociates an RAM permission from a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#disassociate_resource_share_permission)
         """
     def enable_sharing_with_aws_organization(
         self,
     ) -> EnableSharingWithAwsOrganizationResponseTypeDef:
@@ -304,15 +242,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#generate_presigned_url)
         """
     def get_permission(
         self, *, permissionArn: str, permissionVersion: int = ...
     ) -> GetPermissionResponseTypeDef:
         """
-        Retrieves the contents of a managed permission in JSON format.
+        Gets the contents of an RAM permission in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_permission)
         """
     def get_resource_policies(
         self,
         *,
@@ -336,16 +274,16 @@
         resourceArn: str = ...,
         principal: str = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetResourceShareAssociationsResponseTypeDef:
         """
-        Retrieves the lists of resources and principals that associated for resource
-        shares that you own.
+        Retrieves the resource and principal associations for resource shares that you
+        own.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_share_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_resource_share_associations)
         """
     def get_resource_share_invitations(
         self,
         *,
@@ -366,16 +304,15 @@
         resourceOwner: ResourceOwnerType,
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        permissionArn: str = ...,
-        permissionVersion: int = ...
+        permissionArn: str = ...
     ) -> GetResourceSharesResponseTypeDef:
         """
         Retrieves details about the resource shares that you own or that are shared with
         you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_resource_shares)
@@ -391,49 +328,25 @@
         """
         Lists the resources in a resource share that is shared with you but for which
         the invitation is still `PENDING`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_pending_invitation_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_pending_invitation_resources)
         """
-    def list_permission_associations(
-        self,
-        *,
-        permissionArn: str = ...,
-        permissionVersion: int = ...,
-        associationStatus: ResourceShareAssociationStatusType = ...,
-        resourceType: str = ...,
-        featureSet: PermissionFeatureSetType = ...,
-        defaultVersion: bool = ...,
-        nextToken: str = ...,
-        maxResults: int = ...
-    ) -> ListPermissionAssociationsResponseTypeDef:
-        """
-        Lists information about the managed permission and its associations to any
-        resource shares that use this managed permission.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permission_associations)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_permission_associations)
-        """
     def list_permission_versions(
         self, *, permissionArn: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListPermissionVersionsResponseTypeDef:
         """
         Lists the available versions of the specified RAM permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permission_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_permission_versions)
         """
     def list_permissions(
-        self,
-        *,
-        resourceType: str = ...,
-        nextToken: str = ...,
-        maxResults: int = ...,
-        permissionType: PermissionTypeFilterType = ...
+        self, *, resourceType: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> ListPermissionsResponseTypeDef:
         """
         Retrieves a list of available RAM permissions that you can use for the supported
         resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_permissions)
@@ -452,29 +365,14 @@
         """
         Lists the principals that you are sharing resources with or that are sharing
         resources with you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_principals)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_principals)
         """
-    def list_replace_permission_associations_work(
-        self,
-        *,
-        workIds: Sequence[str] = ...,
-        status: ReplacePermissionAssociationsWorkStatusType = ...,
-        nextToken: str = ...,
-        maxResults: int = ...
-    ) -> ListReplacePermissionAssociationsWorkResponseTypeDef:
-        """
-        Retrieves the current status of the asynchronous tasks performed by RAM when you
-        perform the  ReplacePermissionAssociationsWork operation.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_replace_permission_associations_work)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_replace_permission_associations_work)
-        """
     def list_resource_share_permissions(
         self, *, resourceShareArn: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListResourceSharePermissionsResponseTypeDef:
         """
         Lists the RAM permissions that are associated with a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resource_share_permissions)
@@ -508,89 +406,44 @@
         """
         Lists the resources that you added to a resource share or the resources that are
         shared with you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_resources)
         """
-    def promote_permission_created_from_policy(
-        self, *, permissionArn: str, name: str, clientToken: str = ...
-    ) -> PromotePermissionCreatedFromPolicyResponseTypeDef:
-        """
-        When you attach a resource-based policy to a resource, RAM automatically creates
-        a resource share of `featureSet`= `CREATED_FROM_POLICY` with a managed
-        permission that has the same IAM permissions as the original resource-based
-        policy.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.promote_permission_created_from_policy)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#promote_permission_created_from_policy)
-        """
     def promote_resource_share_created_from_policy(
         self, *, resourceShareArn: str
     ) -> PromoteResourceShareCreatedFromPolicyResponseTypeDef:
         """
-        When you attach a resource-based policy to a resource, RAM automatically creates
-        a resource share of `featureSet`= `CREATED_FROM_POLICY` with a managed
-        permission that has the same IAM permissions as the original resource-based
-        policy.
+        When you attach a resource-based permission policy to a resource, it
+        automatically creates a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.promote_resource_share_created_from_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#promote_resource_share_created_from_policy)
         """
     def reject_resource_share_invitation(
         self, *, resourceShareInvitationArn: str, clientToken: str = ...
     ) -> RejectResourceShareInvitationResponseTypeDef:
         """
         Rejects an invitation to a resource share from another Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.reject_resource_share_invitation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#reject_resource_share_invitation)
         """
-    def replace_permission_associations(
-        self,
-        *,
-        fromPermissionArn: str,
-        toPermissionArn: str,
-        fromPermissionVersion: int = ...,
-        clientToken: str = ...
-    ) -> ReplacePermissionAssociationsResponseTypeDef:
-        """
-        Updates all resource shares that use a managed permission to a different managed
-        permission.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.replace_permission_associations)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#replace_permission_associations)
-        """
-    def set_default_permission_version(
-        self, *, permissionArn: str, permissionVersion: int, clientToken: str = ...
-    ) -> SetDefaultPermissionVersionResponseTypeDef:
-        """
-        Designates the specified version number as the default version for the specified
-        customer managed permission.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.set_default_permission_version)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#set_default_permission_version)
-        """
-    def tag_resource(
-        self, *, tags: Sequence[TagTypeDef], resourceShareArn: str = ..., resourceArn: str = ...
-    ) -> Dict[str, Any]:
+    def tag_resource(self, *, resourceShareArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
-        Adds the specified tag keys and values to a resource share or managed
-        permission.
+        Adds the specified tag keys and values to the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#tag_resource)
         """
-    def untag_resource(
-        self, *, tagKeys: Sequence[str], resourceShareArn: str = ..., resourceArn: str = ...
-    ) -> Dict[str, Any]:
+    def untag_resource(self, *, resourceShareArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes the specified tag key and value pairs from the specified resource share
-        or managed permission.
+        Removes the specified tag key and value pairs from the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#untag_resource)
         """
     def update_resource_share(
         self,
         *,
```

### Comparing `mypy-boto3-ram-1.26.116/mypy_boto3_ram/literals.py` & `mypy-boto3-ram-1.26.46/mypy_boto3_ram/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,27 +14,21 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "GetResourcePoliciesPaginatorName",
     "GetResourceShareAssociationsPaginatorName",
     "GetResourceShareInvitationsPaginatorName",
     "GetResourceSharesPaginatorName",
     "ListPrincipalsPaginatorName",
     "ListResourcesPaginatorName",
-    "PermissionFeatureSetType",
-    "PermissionStatusType",
-    "PermissionTypeFilterType",
-    "PermissionTypeType",
-    "ReplacePermissionAssociationsWorkStatusType",
     "ResourceOwnerType",
     "ResourceRegionScopeFilterType",
     "ResourceRegionScopeType",
     "ResourceShareAssociationStatusType",
     "ResourceShareAssociationTypeType",
     "ResourceShareFeatureSetType",
     "ResourceShareInvitationStatusType",
@@ -43,26 +37,20 @@
     "RAMServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 GetResourcePoliciesPaginatorName = Literal["get_resource_policies"]
 GetResourceShareAssociationsPaginatorName = Literal["get_resource_share_associations"]
 GetResourceShareInvitationsPaginatorName = Literal["get_resource_share_invitations"]
 GetResourceSharesPaginatorName = Literal["get_resource_shares"]
 ListPrincipalsPaginatorName = Literal["list_principals"]
 ListResourcesPaginatorName = Literal["list_resources"]
-PermissionFeatureSetType = Literal["CREATED_FROM_POLICY", "PROMOTING_TO_STANDARD", "STANDARD"]
-PermissionStatusType = Literal["ATTACHABLE", "DELETED", "DELETING", "UNATTACHABLE"]
-PermissionTypeFilterType = Literal["ALL", "AWS_MANAGED", "CUSTOMER_MANAGED"]
-PermissionTypeType = Literal["AWS_MANAGED", "CUSTOMER_MANAGED"]
-ReplacePermissionAssociationsWorkStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS"]
 ResourceOwnerType = Literal["OTHER-ACCOUNTS", "SELF"]
 ResourceRegionScopeFilterType = Literal["ALL", "GLOBAL", "REGIONAL"]
 ResourceRegionScopeType = Literal["GLOBAL", "REGIONAL"]
 ResourceShareAssociationStatusType = Literal[
     "ASSOCIATED", "ASSOCIATING", "DISASSOCIATED", "DISASSOCIATING", "FAILED"
 ]
 ResourceShareAssociationTypeType = Literal["PRINCIPAL", "RESOURCE"]
@@ -112,26 +100,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -217,15 +203,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -236,15 +221,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -395,20 +379,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -445,15 +427,14 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
-    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-ram-1.26.116/mypy_boto3_ram/literals.pyi` & `mypy-boto3-ram-1.26.46/mypy_boto3_ram/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,22 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "GetResourcePoliciesPaginatorName",
     "GetResourceShareAssociationsPaginatorName",
     "GetResourceShareInvitationsPaginatorName",
     "GetResourceSharesPaginatorName",
     "ListPrincipalsPaginatorName",
     "ListResourcesPaginatorName",
-    "PermissionFeatureSetType",
-    "PermissionStatusType",
-    "PermissionTypeFilterType",
-    "PermissionTypeType",
-    "ReplacePermissionAssociationsWorkStatusType",
     "ResourceOwnerType",
     "ResourceRegionScopeFilterType",
     "ResourceRegionScopeType",
     "ResourceShareAssociationStatusType",
     "ResourceShareAssociationTypeType",
     "ResourceShareFeatureSetType",
     "ResourceShareInvitationStatusType",
@@ -42,25 +38,21 @@
     "RAMServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 GetResourcePoliciesPaginatorName = Literal["get_resource_policies"]
 GetResourceShareAssociationsPaginatorName = Literal["get_resource_share_associations"]
 GetResourceShareInvitationsPaginatorName = Literal["get_resource_share_invitations"]
 GetResourceSharesPaginatorName = Literal["get_resource_shares"]
 ListPrincipalsPaginatorName = Literal["list_principals"]
 ListResourcesPaginatorName = Literal["list_resources"]
-PermissionFeatureSetType = Literal["CREATED_FROM_POLICY", "PROMOTING_TO_STANDARD", "STANDARD"]
-PermissionStatusType = Literal["ATTACHABLE", "DELETED", "DELETING", "UNATTACHABLE"]
-PermissionTypeFilterType = Literal["ALL", "AWS_MANAGED", "CUSTOMER_MANAGED"]
-PermissionTypeType = Literal["AWS_MANAGED", "CUSTOMER_MANAGED"]
-ReplacePermissionAssociationsWorkStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS"]
 ResourceOwnerType = Literal["OTHER-ACCOUNTS", "SELF"]
 ResourceRegionScopeFilterType = Literal["ALL", "GLOBAL", "REGIONAL"]
 ResourceRegionScopeType = Literal["GLOBAL", "REGIONAL"]
 ResourceShareAssociationStatusType = Literal[
     "ASSOCIATED", "ASSOCIATING", "DISASSOCIATED", "DISASSOCIATING", "FAILED"
 ]
 ResourceShareAssociationTypeType = Literal["PRINCIPAL", "RESOURCE"]
@@ -110,26 +102,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -215,15 +205,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -234,15 +223,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -393,20 +381,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -443,15 +429,14 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
-    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-ram-1.26.116/mypy_boto3_ram/paginator.py` & `mypy-boto3-ram-1.26.46/mypy_boto3_ram/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,14 @@
         *,
         resourceOwner: ResourceOwnerType,
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
         permissionArn: str = ...,
-        permissionVersion: int = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourceSharesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourcesharespaginator)
         """
```

### Comparing `mypy-boto3-ram-1.26.116/mypy_boto3_ram/paginator.pyi` & `mypy-boto3-ram-1.26.46/mypy_boto3_ram/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,14 @@
         *,
         resourceOwner: ResourceOwnerType,
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
         permissionArn: str = ...,
-        permissionVersion: int = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourceSharesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourcesharespaginator)
         """
```

### Comparing `mypy-boto3-ram-1.26.116/mypy_boto3_ram/type_defs.py` & `mypy-boto3-ram-1.26.46/mypy_boto3_ram/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,19 +12,14 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
-    PermissionFeatureSetType,
-    PermissionStatusType,
-    PermissionTypeFilterType,
-    PermissionTypeType,
-    ReplacePermissionAssociationsWorkStatusType,
     ResourceOwnerType,
     ResourceRegionScopeFilterType,
     ResourceRegionScopeType,
     ResourceShareAssociationStatusType,
     ResourceShareAssociationTypeType,
     ResourceShareFeatureSetType,
     ResourceShareInvitationStatusType,
@@ -40,91 +35,71 @@
 
 __all__ = (
     "AcceptResourceShareInvitationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateResourceSharePermissionRequestRequestTypeDef",
     "AssociateResourceShareRequestRequestTypeDef",
     "ResourceShareAssociationTypeDef",
-    "AssociatedPermissionTypeDef",
     "TagTypeDef",
-    "CreatePermissionVersionRequestRequestTypeDef",
-    "DeletePermissionRequestRequestTypeDef",
-    "DeletePermissionVersionRequestRequestTypeDef",
     "DeleteResourceShareRequestRequestTypeDef",
     "DisassociateResourceSharePermissionRequestRequestTypeDef",
     "DisassociateResourceShareRequestRequestTypeDef",
     "GetPermissionRequestRequestTypeDef",
+    "ResourceSharePermissionDetailTypeDef",
     "PaginatorConfigTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourceShareAssociationsRequestRequestTypeDef",
     "GetResourceShareInvitationsRequestRequestTypeDef",
     "TagFilterTypeDef",
     "ListPendingInvitationResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
-    "ListPermissionAssociationsRequestRequestTypeDef",
     "ListPermissionVersionsRequestRequestTypeDef",
+    "ResourceSharePermissionSummaryTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "ListPrincipalsRequestRequestTypeDef",
     "PrincipalTypeDef",
-    "ListReplacePermissionAssociationsWorkRequestRequestTypeDef",
-    "ReplacePermissionAssociationsWorkTypeDef",
     "ListResourceSharePermissionsRequestRequestTypeDef",
     "ListResourceTypesRequestRequestTypeDef",
     "ServiceNameAndResourceTypeTypeDef",
     "ListResourcesRequestRequestTypeDef",
-    "PromotePermissionCreatedFromPolicyRequestRequestTypeDef",
     "PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef",
     "RejectResourceShareInvitationRequestRequestTypeDef",
-    "ReplacePermissionAssociationsRequestRequestTypeDef",
-    "SetDefaultPermissionVersionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateResourceShareRequestRequestTypeDef",
     "AssociateResourceSharePermissionResponseTypeDef",
-    "DeletePermissionResponseTypeDef",
-    "DeletePermissionVersionResponseTypeDef",
     "DeleteResourceShareResponseTypeDef",
     "DisassociateResourceSharePermissionResponseTypeDef",
     "EnableSharingWithAwsOrganizationResponseTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
-    "SetDefaultPermissionVersionResponseTypeDef",
     "AssociateResourceShareResponseTypeDef",
     "DisassociateResourceShareResponseTypeDef",
     "GetResourceShareAssociationsResponseTypeDef",
     "ResourceShareInvitationTypeDef",
-    "ListPermissionAssociationsResponseTypeDef",
-    "CreatePermissionRequestRequestTypeDef",
     "CreateResourceShareRequestRequestTypeDef",
-    "ResourceSharePermissionDetailTypeDef",
-    "ResourceSharePermissionSummaryTypeDef",
     "ResourceShareTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "GetPermissionResponseTypeDef",
     "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     "GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
     "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
     "ListPrincipalsRequestListPrincipalsPaginateTypeDef",
     "ListResourcesRequestListResourcesPaginateTypeDef",
     "GetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     "GetResourceSharesRequestRequestTypeDef",
     "ListPendingInvitationResourcesResponseTypeDef",
     "ListResourcesResponseTypeDef",
+    "ListPermissionVersionsResponseTypeDef",
+    "ListPermissionsResponseTypeDef",
+    "ListResourceSharePermissionsResponseTypeDef",
     "ListPrincipalsResponseTypeDef",
-    "ListReplacePermissionAssociationsWorkResponseTypeDef",
-    "ReplacePermissionAssociationsResponseTypeDef",
     "ListResourceTypesResponseTypeDef",
     "AcceptResourceShareInvitationResponseTypeDef",
     "GetResourceShareInvitationsResponseTypeDef",
     "RejectResourceShareInvitationResponseTypeDef",
-    "CreatePermissionVersionResponseTypeDef",
-    "GetPermissionResponseTypeDef",
-    "CreatePermissionResponseTypeDef",
-    "ListPermissionVersionsResponseTypeDef",
-    "ListPermissionsResponseTypeDef",
-    "ListResourceSharePermissionsResponseTypeDef",
-    "PromotePermissionCreatedFromPolicyResponseTypeDef",
     "CreateResourceShareResponseTypeDef",
     "GetResourceSharesResponseTypeDef",
     "UpdateResourceShareResponseTypeDef",
 )
 
 _RequiredAcceptResourceShareInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptResourceShareInvitationRequestRequestTypeDef",
@@ -220,105 +195,23 @@
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
         "external": bool,
     },
     total=False,
 )
 
-AssociatedPermissionTypeDef = TypedDict(
-    "AssociatedPermissionTypeDef",
-    {
-        "arn": str,
-        "permissionVersion": str,
-        "defaultVersion": bool,
-        "resourceType": str,
-        "status": str,
-        "featureSet": PermissionFeatureSetType,
-        "lastUpdatedTime": datetime,
-        "resourceShareArn": str,
-    },
-    total=False,
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-_RequiredCreatePermissionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePermissionVersionRequestRequestTypeDef",
-    {
-        "permissionArn": str,
-        "policyTemplate": str,
-    },
-)
-_OptionalCreatePermissionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePermissionVersionRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class CreatePermissionVersionRequestRequestTypeDef(
-    _RequiredCreatePermissionVersionRequestRequestTypeDef,
-    _OptionalCreatePermissionVersionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredDeletePermissionRequestRequestTypeDef = TypedDict(
-    "_RequiredDeletePermissionRequestRequestTypeDef",
-    {
-        "permissionArn": str,
-    },
-)
-_OptionalDeletePermissionRequestRequestTypeDef = TypedDict(
-    "_OptionalDeletePermissionRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class DeletePermissionRequestRequestTypeDef(
-    _RequiredDeletePermissionRequestRequestTypeDef, _OptionalDeletePermissionRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredDeletePermissionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredDeletePermissionVersionRequestRequestTypeDef",
-    {
-        "permissionArn": str,
-        "permissionVersion": int,
-    },
-)
-_OptionalDeletePermissionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalDeletePermissionVersionRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class DeletePermissionVersionRequestRequestTypeDef(
-    _RequiredDeletePermissionVersionRequestRequestTypeDef,
-    _OptionalDeletePermissionVersionRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredDeleteResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalDeleteResourceShareRequestRequestTypeDef = TypedDict(
@@ -401,14 +294,30 @@
 
 class GetPermissionRequestRequestTypeDef(
     _RequiredGetPermissionRequestRequestTypeDef, _OptionalGetPermissionRequestRequestTypeDef
 ):
     pass
 
 
+ResourceSharePermissionDetailTypeDef = TypedDict(
+    "ResourceSharePermissionDetailTypeDef",
+    {
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
+        "name": str,
+        "resourceType": str,
+        "permission": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "isResourceTypeDefault": bool,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -522,29 +431,14 @@
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
         "resourceRegionScope": ResourceRegionScopeType,
     },
     total=False,
 )
 
-ListPermissionAssociationsRequestRequestTypeDef = TypedDict(
-    "ListPermissionAssociationsRequestRequestTypeDef",
-    {
-        "permissionArn": str,
-        "permissionVersion": int,
-        "associationStatus": ResourceShareAssociationStatusType,
-        "resourceType": str,
-        "featureSet": PermissionFeatureSetType,
-        "defaultVersion": bool,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
 _RequiredListPermissionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionVersionsRequestRequestTypeDef",
     {
         "permissionArn": str,
     },
 )
 _OptionalListPermissionVersionsRequestRequestTypeDef = TypedDict(
@@ -560,21 +454,36 @@
 class ListPermissionVersionsRequestRequestTypeDef(
     _RequiredListPermissionVersionsRequestRequestTypeDef,
     _OptionalListPermissionVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+ResourceSharePermissionSummaryTypeDef = TypedDict(
+    "ResourceSharePermissionSummaryTypeDef",
+    {
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
+        "name": str,
+        "resourceType": str,
+        "status": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "isResourceTypeDefault": bool,
+    },
+    total=False,
+)
+
 ListPermissionsRequestRequestTypeDef = TypedDict(
     "ListPermissionsRequestRequestTypeDef",
     {
         "resourceType": str,
         "nextToken": str,
         "maxResults": int,
-        "permissionType": PermissionTypeFilterType,
     },
     total=False,
 )
 
 _RequiredListPrincipalsRequestRequestTypeDef = TypedDict(
     "_RequiredListPrincipalsRequestRequestTypeDef",
     {
@@ -609,41 +518,14 @@
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
         "external": bool,
     },
     total=False,
 )
 
-ListReplacePermissionAssociationsWorkRequestRequestTypeDef = TypedDict(
-    "ListReplacePermissionAssociationsWorkRequestRequestTypeDef",
-    {
-        "workIds": Sequence[str],
-        "status": ReplacePermissionAssociationsWorkStatusType,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-ReplacePermissionAssociationsWorkTypeDef = TypedDict(
-    "ReplacePermissionAssociationsWorkTypeDef",
-    {
-        "id": str,
-        "fromPermissionArn": str,
-        "fromPermissionVersion": str,
-        "toPermissionArn": str,
-        "toPermissionVersion": str,
-        "status": ReplacePermissionAssociationsWorkStatusType,
-        "statusMessage": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredListResourceSharePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceSharePermissionsRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalListResourceSharePermissionsRequestRequestTypeDef = TypedDict(
@@ -706,37 +588,14 @@
 
 class ListResourcesRequestRequestTypeDef(
     _RequiredListResourcesRequestRequestTypeDef, _OptionalListResourcesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef",
-    {
-        "permissionArn": str,
-        "name": str,
-    },
-)
-_OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class PromotePermissionCreatedFromPolicyRequestRequestTypeDef(
-    _RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef,
-    _OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef,
-):
-    pass
-
-
 PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef = TypedDict(
     "PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 
@@ -758,83 +617,22 @@
 class RejectResourceShareInvitationRequestRequestTypeDef(
     _RequiredRejectResourceShareInvitationRequestRequestTypeDef,
     _OptionalRejectResourceShareInvitationRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredReplacePermissionAssociationsRequestRequestTypeDef = TypedDict(
-    "_RequiredReplacePermissionAssociationsRequestRequestTypeDef",
-    {
-        "fromPermissionArn": str,
-        "toPermissionArn": str,
-    },
-)
-_OptionalReplacePermissionAssociationsRequestRequestTypeDef = TypedDict(
-    "_OptionalReplacePermissionAssociationsRequestRequestTypeDef",
-    {
-        "fromPermissionVersion": int,
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class ReplacePermissionAssociationsRequestRequestTypeDef(
-    _RequiredReplacePermissionAssociationsRequestRequestTypeDef,
-    _OptionalReplacePermissionAssociationsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredSetDefaultPermissionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredSetDefaultPermissionVersionRequestRequestTypeDef",
-    {
-        "permissionArn": str,
-        "permissionVersion": int,
-    },
-)
-_OptionalSetDefaultPermissionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalSetDefaultPermissionVersionRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class SetDefaultPermissionVersionRequestRequestTypeDef(
-    _RequiredSetDefaultPermissionVersionRequestRequestTypeDef,
-    _OptionalSetDefaultPermissionVersionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUntagResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredUntagResourceRequestRequestTypeDef",
-    {
-        "tagKeys": Sequence[str],
-    },
-)
-_OptionalUntagResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalUntagResourceRequestRequestTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
         "resourceShareArn": str,
-        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
-    total=False,
 )
 
-
-class UntagResourceRequestRequestTypeDef(
-    _RequiredUntagResourceRequestRequestTypeDef, _OptionalUntagResourceRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredUpdateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalUpdateResourceShareRequestRequestTypeDef = TypedDict(
@@ -860,34 +658,14 @@
     {
         "returnValue": bool,
         "clientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeletePermissionResponseTypeDef = TypedDict(
-    "DeletePermissionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "permissionStatus": PermissionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePermissionVersionResponseTypeDef = TypedDict(
-    "DeletePermissionVersionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "permissionStatus": PermissionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeleteResourceShareResponseTypeDef = TypedDict(
     "DeleteResourceShareResponseTypeDef",
     {
         "returnValue": bool,
         "clientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -923,23 +701,14 @@
     "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
     {
         "returnValue": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SetDefaultPermissionVersionResponseTypeDef = TypedDict(
-    "SetDefaultPermissionVersionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AssociateResourceShareResponseTypeDef = TypedDict(
     "AssociateResourceShareResponseTypeDef",
     {
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "clientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -975,47 +744,14 @@
         "status": ResourceShareInvitationStatusType,
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "receiverArn": str,
     },
     total=False,
 )
 
-ListPermissionAssociationsResponseTypeDef = TypedDict(
-    "ListPermissionAssociationsResponseTypeDef",
-    {
-        "permissions": List[AssociatedPermissionTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreatePermissionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePermissionRequestRequestTypeDef",
-    {
-        "name": str,
-        "resourceType": str,
-        "policyTemplate": str,
-    },
-)
-_OptionalCreatePermissionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePermissionRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreatePermissionRequestRequestTypeDef(
-    _RequiredCreatePermissionRequestRequestTypeDef, _OptionalCreatePermissionRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredCreateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceShareRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateResourceShareRequestRequestTypeDef = TypedDict(
@@ -1035,53 +771,14 @@
 class CreateResourceShareRequestRequestTypeDef(
     _RequiredCreateResourceShareRequestRequestTypeDef,
     _OptionalCreateResourceShareRequestRequestTypeDef,
 ):
     pass
 
 
-ResourceSharePermissionDetailTypeDef = TypedDict(
-    "ResourceSharePermissionDetailTypeDef",
-    {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
-        "resourceType": str,
-        "permission": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
-        "permissionType": PermissionTypeType,
-        "featureSet": PermissionFeatureSetType,
-        "status": PermissionStatusType,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-ResourceSharePermissionSummaryTypeDef = TypedDict(
-    "ResourceSharePermissionSummaryTypeDef",
-    {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
-        "resourceType": str,
-        "status": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
-        "permissionType": PermissionTypeType,
-        "featureSet": PermissionFeatureSetType,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 ResourceShareTypeDef = TypedDict(
     "ResourceShareTypeDef",
     {
         "resourceShareArn": str,
         "name": str,
         "owningAccountId": str,
         "allowExternalPrincipals": bool,
@@ -1091,36 +788,30 @@
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
         "featureSet": ResourceShareFeatureSetType,
     },
     total=False,
 )
 
-_RequiredTagResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredTagResourceRequestRequestTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
+        "resourceShareArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
-_OptionalTagResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalTagResourceRequestRequestTypeDef",
+
+GetPermissionResponseTypeDef = TypedDict(
+    "GetPermissionResponseTypeDef",
     {
-        "resourceShareArn": str,
-        "resourceArn": str,
+        "permission": ResourceSharePermissionDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class TagResourceRequestRequestTypeDef(
-    _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "resourceArns": Sequence[str],
     },
 )
 _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
@@ -1239,15 +930,14 @@
     "_OptionalGetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     {
         "resourceShareArns": Sequence[str],
         "resourceShareStatus": ResourceShareStatusType,
         "name": str,
         "tagFilters": Sequence[TagFilterTypeDef],
         "permissionArn": str,
-        "permissionVersion": int,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class GetResourceSharesRequestGetResourceSharesPaginateTypeDef(
@@ -1269,15 +959,14 @@
         "resourceShareArns": Sequence[str],
         "resourceShareStatus": ResourceShareStatusType,
         "name": str,
         "tagFilters": Sequence[TagFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
         "permissionArn": str,
-        "permissionVersion": int,
     },
     total=False,
 )
 
 
 class GetResourceSharesRequestRequestTypeDef(
     _RequiredGetResourceSharesRequestRequestTypeDef, _OptionalGetResourceSharesRequestRequestTypeDef
@@ -1299,37 +988,46 @@
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListPrincipalsResponseTypeDef = TypedDict(
-    "ListPrincipalsResponseTypeDef",
+ListPermissionVersionsResponseTypeDef = TypedDict(
+    "ListPermissionVersionsResponseTypeDef",
     {
-        "principals": List[PrincipalTypeDef],
+        "permissions": List[ResourceSharePermissionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListReplacePermissionAssociationsWorkResponseTypeDef = TypedDict(
-    "ListReplacePermissionAssociationsWorkResponseTypeDef",
+ListPermissionsResponseTypeDef = TypedDict(
+    "ListPermissionsResponseTypeDef",
     {
-        "replacePermissionAssociationsWorks": List[ReplacePermissionAssociationsWorkTypeDef],
+        "permissions": List[ResourceSharePermissionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReplacePermissionAssociationsResponseTypeDef = TypedDict(
-    "ReplacePermissionAssociationsResponseTypeDef",
+ListResourceSharePermissionsResponseTypeDef = TypedDict(
+    "ListResourceSharePermissionsResponseTypeDef",
     {
-        "replacePermissionAssociationsWork": ReplacePermissionAssociationsWorkTypeDef,
-        "clientToken": str,
+        "permissions": List[ResourceSharePermissionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPrincipalsResponseTypeDef = TypedDict(
+    "ListPrincipalsResponseTypeDef",
+    {
+        "principals": List[PrincipalTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceTypesResponseTypeDef = TypedDict(
     "ListResourceTypesResponseTypeDef",
     {
@@ -1362,76 +1060,14 @@
     {
         "resourceShareInvitation": ResourceShareInvitationTypeDef,
         "clientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreatePermissionVersionResponseTypeDef = TypedDict(
-    "CreatePermissionVersionResponseTypeDef",
-    {
-        "permission": ResourceSharePermissionDetailTypeDef,
-        "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPermissionResponseTypeDef = TypedDict(
-    "GetPermissionResponseTypeDef",
-    {
-        "permission": ResourceSharePermissionDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePermissionResponseTypeDef = TypedDict(
-    "CreatePermissionResponseTypeDef",
-    {
-        "permission": ResourceSharePermissionSummaryTypeDef,
-        "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPermissionVersionsResponseTypeDef = TypedDict(
-    "ListPermissionVersionsResponseTypeDef",
-    {
-        "permissions": List[ResourceSharePermissionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPermissionsResponseTypeDef = TypedDict(
-    "ListPermissionsResponseTypeDef",
-    {
-        "permissions": List[ResourceSharePermissionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListResourceSharePermissionsResponseTypeDef = TypedDict(
-    "ListResourceSharePermissionsResponseTypeDef",
-    {
-        "permissions": List[ResourceSharePermissionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PromotePermissionCreatedFromPolicyResponseTypeDef = TypedDict(
-    "PromotePermissionCreatedFromPolicyResponseTypeDef",
-    {
-        "permission": ResourceSharePermissionSummaryTypeDef,
-        "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateResourceShareResponseTypeDef = TypedDict(
     "CreateResourceShareResponseTypeDef",
     {
         "resourceShare": ResourceShareTypeDef,
         "clientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-ram-1.26.116/mypy_boto3_ram/type_defs.pyi` & `mypy-boto3-ram-1.26.46/mypy_boto3_ram/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -12,19 +12,14 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
-    PermissionFeatureSetType,
-    PermissionStatusType,
-    PermissionTypeFilterType,
-    PermissionTypeType,
-    ReplacePermissionAssociationsWorkStatusType,
     ResourceOwnerType,
     ResourceRegionScopeFilterType,
     ResourceRegionScopeType,
     ResourceShareAssociationStatusType,
     ResourceShareAssociationTypeType,
     ResourceShareFeatureSetType,
     ResourceShareInvitationStatusType,
@@ -39,91 +34,71 @@
 
 __all__ = (
     "AcceptResourceShareInvitationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateResourceSharePermissionRequestRequestTypeDef",
     "AssociateResourceShareRequestRequestTypeDef",
     "ResourceShareAssociationTypeDef",
-    "AssociatedPermissionTypeDef",
     "TagTypeDef",
-    "CreatePermissionVersionRequestRequestTypeDef",
-    "DeletePermissionRequestRequestTypeDef",
-    "DeletePermissionVersionRequestRequestTypeDef",
     "DeleteResourceShareRequestRequestTypeDef",
     "DisassociateResourceSharePermissionRequestRequestTypeDef",
     "DisassociateResourceShareRequestRequestTypeDef",
     "GetPermissionRequestRequestTypeDef",
+    "ResourceSharePermissionDetailTypeDef",
     "PaginatorConfigTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourceShareAssociationsRequestRequestTypeDef",
     "GetResourceShareInvitationsRequestRequestTypeDef",
     "TagFilterTypeDef",
     "ListPendingInvitationResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
-    "ListPermissionAssociationsRequestRequestTypeDef",
     "ListPermissionVersionsRequestRequestTypeDef",
+    "ResourceSharePermissionSummaryTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "ListPrincipalsRequestRequestTypeDef",
     "PrincipalTypeDef",
-    "ListReplacePermissionAssociationsWorkRequestRequestTypeDef",
-    "ReplacePermissionAssociationsWorkTypeDef",
     "ListResourceSharePermissionsRequestRequestTypeDef",
     "ListResourceTypesRequestRequestTypeDef",
     "ServiceNameAndResourceTypeTypeDef",
     "ListResourcesRequestRequestTypeDef",
-    "PromotePermissionCreatedFromPolicyRequestRequestTypeDef",
     "PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef",
     "RejectResourceShareInvitationRequestRequestTypeDef",
-    "ReplacePermissionAssociationsRequestRequestTypeDef",
-    "SetDefaultPermissionVersionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateResourceShareRequestRequestTypeDef",
     "AssociateResourceSharePermissionResponseTypeDef",
-    "DeletePermissionResponseTypeDef",
-    "DeletePermissionVersionResponseTypeDef",
     "DeleteResourceShareResponseTypeDef",
     "DisassociateResourceSharePermissionResponseTypeDef",
     "EnableSharingWithAwsOrganizationResponseTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
-    "SetDefaultPermissionVersionResponseTypeDef",
     "AssociateResourceShareResponseTypeDef",
     "DisassociateResourceShareResponseTypeDef",
     "GetResourceShareAssociationsResponseTypeDef",
     "ResourceShareInvitationTypeDef",
-    "ListPermissionAssociationsResponseTypeDef",
-    "CreatePermissionRequestRequestTypeDef",
     "CreateResourceShareRequestRequestTypeDef",
-    "ResourceSharePermissionDetailTypeDef",
-    "ResourceSharePermissionSummaryTypeDef",
     "ResourceShareTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "GetPermissionResponseTypeDef",
     "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     "GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
     "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
     "ListPrincipalsRequestListPrincipalsPaginateTypeDef",
     "ListResourcesRequestListResourcesPaginateTypeDef",
     "GetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     "GetResourceSharesRequestRequestTypeDef",
     "ListPendingInvitationResourcesResponseTypeDef",
     "ListResourcesResponseTypeDef",
+    "ListPermissionVersionsResponseTypeDef",
+    "ListPermissionsResponseTypeDef",
+    "ListResourceSharePermissionsResponseTypeDef",
     "ListPrincipalsResponseTypeDef",
-    "ListReplacePermissionAssociationsWorkResponseTypeDef",
-    "ReplacePermissionAssociationsResponseTypeDef",
     "ListResourceTypesResponseTypeDef",
     "AcceptResourceShareInvitationResponseTypeDef",
     "GetResourceShareInvitationsResponseTypeDef",
     "RejectResourceShareInvitationResponseTypeDef",
-    "CreatePermissionVersionResponseTypeDef",
-    "GetPermissionResponseTypeDef",
-    "CreatePermissionResponseTypeDef",
-    "ListPermissionVersionsResponseTypeDef",
-    "ListPermissionsResponseTypeDef",
-    "ListResourceSharePermissionsResponseTypeDef",
-    "PromotePermissionCreatedFromPolicyResponseTypeDef",
     "CreateResourceShareResponseTypeDef",
     "GetResourceSharesResponseTypeDef",
     "UpdateResourceShareResponseTypeDef",
 )
 
 _RequiredAcceptResourceShareInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptResourceShareInvitationRequestRequestTypeDef",
@@ -213,99 +188,23 @@
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
         "external": bool,
     },
     total=False,
 )
 
-AssociatedPermissionTypeDef = TypedDict(
-    "AssociatedPermissionTypeDef",
-    {
-        "arn": str,
-        "permissionVersion": str,
-        "defaultVersion": bool,
-        "resourceType": str,
-        "status": str,
-        "featureSet": PermissionFeatureSetType,
-        "lastUpdatedTime": datetime,
-        "resourceShareArn": str,
-    },
-    total=False,
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-_RequiredCreatePermissionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePermissionVersionRequestRequestTypeDef",
-    {
-        "permissionArn": str,
-        "policyTemplate": str,
-    },
-)
-_OptionalCreatePermissionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePermissionVersionRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class CreatePermissionVersionRequestRequestTypeDef(
-    _RequiredCreatePermissionVersionRequestRequestTypeDef,
-    _OptionalCreatePermissionVersionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredDeletePermissionRequestRequestTypeDef = TypedDict(
-    "_RequiredDeletePermissionRequestRequestTypeDef",
-    {
-        "permissionArn": str,
-    },
-)
-_OptionalDeletePermissionRequestRequestTypeDef = TypedDict(
-    "_OptionalDeletePermissionRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class DeletePermissionRequestRequestTypeDef(
-    _RequiredDeletePermissionRequestRequestTypeDef, _OptionalDeletePermissionRequestRequestTypeDef
-):
-    pass
-
-_RequiredDeletePermissionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredDeletePermissionVersionRequestRequestTypeDef",
-    {
-        "permissionArn": str,
-        "permissionVersion": int,
-    },
-)
-_OptionalDeletePermissionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalDeletePermissionVersionRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class DeletePermissionVersionRequestRequestTypeDef(
-    _RequiredDeletePermissionVersionRequestRequestTypeDef,
-    _OptionalDeletePermissionVersionRequestRequestTypeDef,
-):
-    pass
-
 _RequiredDeleteResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalDeleteResourceShareRequestRequestTypeDef = TypedDict(
@@ -380,14 +279,30 @@
 )
 
 class GetPermissionRequestRequestTypeDef(
     _RequiredGetPermissionRequestRequestTypeDef, _OptionalGetPermissionRequestRequestTypeDef
 ):
     pass
 
+ResourceSharePermissionDetailTypeDef = TypedDict(
+    "ResourceSharePermissionDetailTypeDef",
+    {
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
+        "name": str,
+        "resourceType": str,
+        "permission": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "isResourceTypeDefault": bool,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -495,29 +410,14 @@
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
         "resourceRegionScope": ResourceRegionScopeType,
     },
     total=False,
 )
 
-ListPermissionAssociationsRequestRequestTypeDef = TypedDict(
-    "ListPermissionAssociationsRequestRequestTypeDef",
-    {
-        "permissionArn": str,
-        "permissionVersion": int,
-        "associationStatus": ResourceShareAssociationStatusType,
-        "resourceType": str,
-        "featureSet": PermissionFeatureSetType,
-        "defaultVersion": bool,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
 _RequiredListPermissionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionVersionsRequestRequestTypeDef",
     {
         "permissionArn": str,
     },
 )
 _OptionalListPermissionVersionsRequestRequestTypeDef = TypedDict(
@@ -531,21 +431,36 @@
 
 class ListPermissionVersionsRequestRequestTypeDef(
     _RequiredListPermissionVersionsRequestRequestTypeDef,
     _OptionalListPermissionVersionsRequestRequestTypeDef,
 ):
     pass
 
+ResourceSharePermissionSummaryTypeDef = TypedDict(
+    "ResourceSharePermissionSummaryTypeDef",
+    {
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
+        "name": str,
+        "resourceType": str,
+        "status": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "isResourceTypeDefault": bool,
+    },
+    total=False,
+)
+
 ListPermissionsRequestRequestTypeDef = TypedDict(
     "ListPermissionsRequestRequestTypeDef",
     {
         "resourceType": str,
         "nextToken": str,
         "maxResults": int,
-        "permissionType": PermissionTypeFilterType,
     },
     total=False,
 )
 
 _RequiredListPrincipalsRequestRequestTypeDef = TypedDict(
     "_RequiredListPrincipalsRequestRequestTypeDef",
     {
@@ -578,41 +493,14 @@
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
         "external": bool,
     },
     total=False,
 )
 
-ListReplacePermissionAssociationsWorkRequestRequestTypeDef = TypedDict(
-    "ListReplacePermissionAssociationsWorkRequestRequestTypeDef",
-    {
-        "workIds": Sequence[str],
-        "status": ReplacePermissionAssociationsWorkStatusType,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-ReplacePermissionAssociationsWorkTypeDef = TypedDict(
-    "ReplacePermissionAssociationsWorkTypeDef",
-    {
-        "id": str,
-        "fromPermissionArn": str,
-        "fromPermissionVersion": str,
-        "toPermissionArn": str,
-        "toPermissionVersion": str,
-        "status": ReplacePermissionAssociationsWorkStatusType,
-        "statusMessage": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredListResourceSharePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceSharePermissionsRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalListResourceSharePermissionsRequestRequestTypeDef = TypedDict(
@@ -671,35 +559,14 @@
 )
 
 class ListResourcesRequestRequestTypeDef(
     _RequiredListResourcesRequestRequestTypeDef, _OptionalListResourcesRequestRequestTypeDef
 ):
     pass
 
-_RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef",
-    {
-        "permissionArn": str,
-        "name": str,
-    },
-)
-_OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class PromotePermissionCreatedFromPolicyRequestRequestTypeDef(
-    _RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef,
-    _OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef,
-):
-    pass
-
 PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef = TypedDict(
     "PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 
@@ -719,77 +586,22 @@
 
 class RejectResourceShareInvitationRequestRequestTypeDef(
     _RequiredRejectResourceShareInvitationRequestRequestTypeDef,
     _OptionalRejectResourceShareInvitationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredReplacePermissionAssociationsRequestRequestTypeDef = TypedDict(
-    "_RequiredReplacePermissionAssociationsRequestRequestTypeDef",
-    {
-        "fromPermissionArn": str,
-        "toPermissionArn": str,
-    },
-)
-_OptionalReplacePermissionAssociationsRequestRequestTypeDef = TypedDict(
-    "_OptionalReplacePermissionAssociationsRequestRequestTypeDef",
-    {
-        "fromPermissionVersion": int,
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class ReplacePermissionAssociationsRequestRequestTypeDef(
-    _RequiredReplacePermissionAssociationsRequestRequestTypeDef,
-    _OptionalReplacePermissionAssociationsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredSetDefaultPermissionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredSetDefaultPermissionVersionRequestRequestTypeDef",
-    {
-        "permissionArn": str,
-        "permissionVersion": int,
-    },
-)
-_OptionalSetDefaultPermissionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalSetDefaultPermissionVersionRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class SetDefaultPermissionVersionRequestRequestTypeDef(
-    _RequiredSetDefaultPermissionVersionRequestRequestTypeDef,
-    _OptionalSetDefaultPermissionVersionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUntagResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredUntagResourceRequestRequestTypeDef",
-    {
-        "tagKeys": Sequence[str],
-    },
-)
-_OptionalUntagResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalUntagResourceRequestRequestTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
         "resourceShareArn": str,
-        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
-    total=False,
 )
 
-class UntagResourceRequestRequestTypeDef(
-    _RequiredUntagResourceRequestRequestTypeDef, _OptionalUntagResourceRequestRequestTypeDef
-):
-    pass
-
 _RequiredUpdateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalUpdateResourceShareRequestRequestTypeDef = TypedDict(
@@ -813,34 +625,14 @@
     {
         "returnValue": bool,
         "clientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeletePermissionResponseTypeDef = TypedDict(
-    "DeletePermissionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "permissionStatus": PermissionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePermissionVersionResponseTypeDef = TypedDict(
-    "DeletePermissionVersionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "permissionStatus": PermissionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeleteResourceShareResponseTypeDef = TypedDict(
     "DeleteResourceShareResponseTypeDef",
     {
         "returnValue": bool,
         "clientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -876,23 +668,14 @@
     "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
     {
         "returnValue": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SetDefaultPermissionVersionResponseTypeDef = TypedDict(
-    "SetDefaultPermissionVersionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AssociateResourceShareResponseTypeDef = TypedDict(
     "AssociateResourceShareResponseTypeDef",
     {
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "clientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -928,45 +711,14 @@
         "status": ResourceShareInvitationStatusType,
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "receiverArn": str,
     },
     total=False,
 )
 
-ListPermissionAssociationsResponseTypeDef = TypedDict(
-    "ListPermissionAssociationsResponseTypeDef",
-    {
-        "permissions": List[AssociatedPermissionTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreatePermissionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePermissionRequestRequestTypeDef",
-    {
-        "name": str,
-        "resourceType": str,
-        "policyTemplate": str,
-    },
-)
-_OptionalCreatePermissionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePermissionRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreatePermissionRequestRequestTypeDef(
-    _RequiredCreatePermissionRequestRequestTypeDef, _OptionalCreatePermissionRequestRequestTypeDef
-):
-    pass
-
 _RequiredCreateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceShareRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateResourceShareRequestRequestTypeDef = TypedDict(
@@ -984,53 +736,14 @@
 
 class CreateResourceShareRequestRequestTypeDef(
     _RequiredCreateResourceShareRequestRequestTypeDef,
     _OptionalCreateResourceShareRequestRequestTypeDef,
 ):
     pass
 
-ResourceSharePermissionDetailTypeDef = TypedDict(
-    "ResourceSharePermissionDetailTypeDef",
-    {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
-        "resourceType": str,
-        "permission": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
-        "permissionType": PermissionTypeType,
-        "featureSet": PermissionFeatureSetType,
-        "status": PermissionStatusType,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-ResourceSharePermissionSummaryTypeDef = TypedDict(
-    "ResourceSharePermissionSummaryTypeDef",
-    {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
-        "resourceType": str,
-        "status": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
-        "permissionType": PermissionTypeType,
-        "featureSet": PermissionFeatureSetType,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 ResourceShareTypeDef = TypedDict(
     "ResourceShareTypeDef",
     {
         "resourceShareArn": str,
         "name": str,
         "owningAccountId": str,
         "allowExternalPrincipals": bool,
@@ -1040,34 +753,30 @@
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
         "featureSet": ResourceShareFeatureSetType,
     },
     total=False,
 )
 
-_RequiredTagResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredTagResourceRequestRequestTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
+        "resourceShareArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
-_OptionalTagResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalTagResourceRequestRequestTypeDef",
+
+GetPermissionResponseTypeDef = TypedDict(
+    "GetPermissionResponseTypeDef",
     {
-        "resourceShareArn": str,
-        "resourceArn": str,
+        "permission": ResourceSharePermissionDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class TagResourceRequestRequestTypeDef(
-    _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
-):
-    pass
-
 _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "resourceArns": Sequence[str],
     },
 )
 _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
@@ -1178,15 +887,14 @@
     "_OptionalGetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     {
         "resourceShareArns": Sequence[str],
         "resourceShareStatus": ResourceShareStatusType,
         "name": str,
         "tagFilters": Sequence[TagFilterTypeDef],
         "permissionArn": str,
-        "permissionVersion": int,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class GetResourceSharesRequestGetResourceSharesPaginateTypeDef(
     _RequiredGetResourceSharesRequestGetResourceSharesPaginateTypeDef,
@@ -1206,15 +914,14 @@
         "resourceShareArns": Sequence[str],
         "resourceShareStatus": ResourceShareStatusType,
         "name": str,
         "tagFilters": Sequence[TagFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
         "permissionArn": str,
-        "permissionVersion": int,
     },
     total=False,
 )
 
 class GetResourceSharesRequestRequestTypeDef(
     _RequiredGetResourceSharesRequestRequestTypeDef, _OptionalGetResourceSharesRequestRequestTypeDef
 ):
@@ -1234,37 +941,46 @@
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListPrincipalsResponseTypeDef = TypedDict(
-    "ListPrincipalsResponseTypeDef",
+ListPermissionVersionsResponseTypeDef = TypedDict(
+    "ListPermissionVersionsResponseTypeDef",
     {
-        "principals": List[PrincipalTypeDef],
+        "permissions": List[ResourceSharePermissionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListReplacePermissionAssociationsWorkResponseTypeDef = TypedDict(
-    "ListReplacePermissionAssociationsWorkResponseTypeDef",
+ListPermissionsResponseTypeDef = TypedDict(
+    "ListPermissionsResponseTypeDef",
     {
-        "replacePermissionAssociationsWorks": List[ReplacePermissionAssociationsWorkTypeDef],
+        "permissions": List[ResourceSharePermissionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReplacePermissionAssociationsResponseTypeDef = TypedDict(
-    "ReplacePermissionAssociationsResponseTypeDef",
+ListResourceSharePermissionsResponseTypeDef = TypedDict(
+    "ListResourceSharePermissionsResponseTypeDef",
     {
-        "replacePermissionAssociationsWork": ReplacePermissionAssociationsWorkTypeDef,
-        "clientToken": str,
+        "permissions": List[ResourceSharePermissionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPrincipalsResponseTypeDef = TypedDict(
+    "ListPrincipalsResponseTypeDef",
+    {
+        "principals": List[PrincipalTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceTypesResponseTypeDef = TypedDict(
     "ListResourceTypesResponseTypeDef",
     {
@@ -1297,76 +1013,14 @@
     {
         "resourceShareInvitation": ResourceShareInvitationTypeDef,
         "clientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreatePermissionVersionResponseTypeDef = TypedDict(
-    "CreatePermissionVersionResponseTypeDef",
-    {
-        "permission": ResourceSharePermissionDetailTypeDef,
-        "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPermissionResponseTypeDef = TypedDict(
-    "GetPermissionResponseTypeDef",
-    {
-        "permission": ResourceSharePermissionDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePermissionResponseTypeDef = TypedDict(
-    "CreatePermissionResponseTypeDef",
-    {
-        "permission": ResourceSharePermissionSummaryTypeDef,
-        "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPermissionVersionsResponseTypeDef = TypedDict(
-    "ListPermissionVersionsResponseTypeDef",
-    {
-        "permissions": List[ResourceSharePermissionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPermissionsResponseTypeDef = TypedDict(
-    "ListPermissionsResponseTypeDef",
-    {
-        "permissions": List[ResourceSharePermissionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListResourceSharePermissionsResponseTypeDef = TypedDict(
-    "ListResourceSharePermissionsResponseTypeDef",
-    {
-        "permissions": List[ResourceSharePermissionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PromotePermissionCreatedFromPolicyResponseTypeDef = TypedDict(
-    "PromotePermissionCreatedFromPolicyResponseTypeDef",
-    {
-        "permission": ResourceSharePermissionSummaryTypeDef,
-        "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateResourceShareResponseTypeDef = TypedDict(
     "CreateResourceShareResponseTypeDef",
     {
         "resourceShare": ResourceShareTypeDef,
         "clientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-ram-1.26.116/mypy_boto3_ram.egg-info/PKG-INFO` & `mypy-boto3-ram-1.26.46/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-ram
-Version: 1.26.116
-Summary: Type annotations for boto3.RAM 1.26.116 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ram type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-ram"></a>
 
 # mypy-boto3-ram
 
 [![PyPI - mypy-boto3-ram](https://img.shields.io/pypi/v/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ram?color=blue)](https://pypistats.org/packages/mypy-boto3-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RAM 1.26.116](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[boto3.RAM 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ram docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,19 +289,14 @@
 from mypy_boto3_ram.literals import (
     GetResourcePoliciesPaginatorName,
     GetResourceShareAssociationsPaginatorName,
     GetResourceShareInvitationsPaginatorName,
     GetResourceSharesPaginatorName,
     ListPrincipalsPaginatorName,
     ListResourcesPaginatorName,
-    PermissionFeatureSetType,
-    PermissionStatusType,
-    PermissionTypeFilterType,
-    PermissionTypeType,
-    ReplacePermissionAssociationsWorkStatusType,
     ResourceOwnerType,
     ResourceRegionScopeFilterType,
     ResourceRegionScopeType,
     ResourceShareAssociationStatusType,
     ResourceShareAssociationTypeType,
     ResourceShareFeatureSetType,
     ResourceShareInvitationStatusType,
@@ -361,91 +324,71 @@
 ```python
 from mypy_boto3_ram.type_defs import (
     AcceptResourceShareInvitationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateResourceSharePermissionRequestRequestTypeDef,
     AssociateResourceShareRequestRequestTypeDef,
     ResourceShareAssociationTypeDef,
-    AssociatedPermissionTypeDef,
     TagTypeDef,
-    CreatePermissionVersionRequestRequestTypeDef,
-    DeletePermissionRequestRequestTypeDef,
-    DeletePermissionVersionRequestRequestTypeDef,
     DeleteResourceShareRequestRequestTypeDef,
     DisassociateResourceSharePermissionRequestRequestTypeDef,
     DisassociateResourceShareRequestRequestTypeDef,
     GetPermissionRequestRequestTypeDef,
+    ResourceSharePermissionDetailTypeDef,
     PaginatorConfigTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourceShareAssociationsRequestRequestTypeDef,
     GetResourceShareInvitationsRequestRequestTypeDef,
     TagFilterTypeDef,
     ListPendingInvitationResourcesRequestRequestTypeDef,
     ResourceTypeDef,
-    ListPermissionAssociationsRequestRequestTypeDef,
     ListPermissionVersionsRequestRequestTypeDef,
+    ResourceSharePermissionSummaryTypeDef,
     ListPermissionsRequestRequestTypeDef,
     ListPrincipalsRequestRequestTypeDef,
     PrincipalTypeDef,
-    ListReplacePermissionAssociationsWorkRequestRequestTypeDef,
-    ReplacePermissionAssociationsWorkTypeDef,
     ListResourceSharePermissionsRequestRequestTypeDef,
     ListResourceTypesRequestRequestTypeDef,
     ServiceNameAndResourceTypeTypeDef,
     ListResourcesRequestRequestTypeDef,
-    PromotePermissionCreatedFromPolicyRequestRequestTypeDef,
     PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef,
     RejectResourceShareInvitationRequestRequestTypeDef,
-    ReplacePermissionAssociationsRequestRequestTypeDef,
-    SetDefaultPermissionVersionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateResourceShareRequestRequestTypeDef,
     AssociateResourceSharePermissionResponseTypeDef,
-    DeletePermissionResponseTypeDef,
-    DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareResponseTypeDef,
     DisassociateResourceSharePermissionResponseTypeDef,
     EnableSharingWithAwsOrganizationResponseTypeDef,
     GetResourcePoliciesResponseTypeDef,
     PromoteResourceShareCreatedFromPolicyResponseTypeDef,
-    SetDefaultPermissionVersionResponseTypeDef,
     AssociateResourceShareResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     ResourceShareInvitationTypeDef,
-    ListPermissionAssociationsResponseTypeDef,
-    CreatePermissionRequestRequestTypeDef,
     CreateResourceShareRequestRequestTypeDef,
-    ResourceSharePermissionDetailTypeDef,
-    ResourceSharePermissionSummaryTypeDef,
     ResourceShareTypeDef,
     TagResourceRequestRequestTypeDef,
+    GetPermissionResponseTypeDef,
     GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
     GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
     ListPrincipalsRequestListPrincipalsPaginateTypeDef,
     ListResourcesRequestListResourcesPaginateTypeDef,
     GetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     GetResourceSharesRequestRequestTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
     ListResourcesResponseTypeDef,
+    ListPermissionVersionsResponseTypeDef,
+    ListPermissionsResponseTypeDef,
+    ListResourceSharePermissionsResponseTypeDef,
     ListPrincipalsResponseTypeDef,
-    ListReplacePermissionAssociationsWorkResponseTypeDef,
-    ReplacePermissionAssociationsResponseTypeDef,
     ListResourceTypesResponseTypeDef,
     AcceptResourceShareInvitationResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
-    CreatePermissionVersionResponseTypeDef,
-    GetPermissionResponseTypeDef,
-    CreatePermissionResponseTypeDef,
-    ListPermissionVersionsResponseTypeDef,
-    ListPermissionsResponseTypeDef,
-    ListResourceSharePermissionsResponseTypeDef,
-    PromotePermissionCreatedFromPolicyResponseTypeDef,
     CreateResourceShareResponseTypeDef,
     GetResourceSharesResponseTypeDef,
     UpdateResourceShareResponseTypeDef,
 )
 
 
 def get_structure() -> AcceptResourceShareInvitationRequestRequestTypeDef:
@@ -455,42 +398,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-ram-1.26.116/mypy_boto3_ram.egg-info/SOURCES.txt` & `mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.26.116/setup.py` & `mypy-boto3-ram-1.26.46/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-ram.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-ram",
-    version="1.26.116",
+    version="1.26.46",
     packages=["mypy_boto3_ram"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RAM 1.26.116 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.RAM 1.26.46 service generated with mypy-boto3-builder 7.12.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -44,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

