# Comparing `tmp/mypy-boto3-s3control-1.26.90.tar.gz` & `tmp/mypy-boto3-s3control-1.26.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3control-1.26.90.tar", last modified: Mon Mar 13 19:32:22 2023, max compression
+gzip compressed data, was "mypy-boto3-s3control-1.26.92.tar", last modified: Wed Mar 15 19:32:09 2023, max compression
```

## Comparing `mypy-boto3-s3control-1.26.90.tar` & `mypy-boto3-s3control-1.26.92.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.895340 mypy-boto3-s3control-1.26.90/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-13 19:32:06.000000 mypy-boto3-s3control-1.26.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-03-13 19:32:22.895340 mypy-boto3-s3control-1.26.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-03-13 19:32:06.000000 mypy-boto3-s3control-1.26.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.895340 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-13 19:32:06.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-13 19:32:06.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-13 19:32:06.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43053 2023-03-13 19:32:06.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42981 2023-03-13 19:32:06.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13293 2023-03-13 19:32:07.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-03-13 19:32:07.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-13 19:32:07.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-03-13 19:32:07.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:06.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69710 2023-03-13 19:32:08.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69633 2023-03-13 19:32:08.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-13 19:32:06.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.895340 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-03-13 19:32:22.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-13 19:32:22.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 19:32:22.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 19:32:22.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-13 19:32:22.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-13 19:32:22.000000 mypy-boto3-s3control-1.26.90/mypy_boto3_s3control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 19:32:22.895340 mypy-boto3-s3control-1.26.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-13 19:32:06.000000 mypy-boto3-s3control-1.26.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 19:32:09.719555 mypy-boto3-s3control-1.26.92/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-03-15 19:32:09.719555 mypy-boto3-s3control-1.26.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21217 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 19:32:09.715555 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43053 2023-03-15 19:31:58.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42981 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-03-15 19:31:58.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13411 2023-03-15 19:31:58.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-15 19:31:58.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-03-15 19:31:58.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    70164 2023-03-15 19:32:00.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70087 2023-03-15 19:31:58.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 19:32:09.715555 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-03-15 19:32:09.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-15 19:32:09.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 19:32:09.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 19:32:09.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-15 19:32:09.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-15 19:32:09.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 19:32:09.719555 mypy-boto3-s3control-1.26.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/setup.py
```

### Comparing `mypy-boto3-s3control-1.26.90/LICENSE` & `mypy-boto3-s3control-1.26.92/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.26.90/PKG-INFO` & `mypy-boto3-s3control-1.26.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3control
-Version: 1.26.90
-Summary: Type annotations for boto3.S3Control 1.26.90 service generated with mypy-boto3-builder 7.13.0
+Version: 1.26.92
+Summary: Type annotations for boto3.S3Control 1.26.92 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3control?color=blue)](https://pypistats.org/packages/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.26.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -318,14 +318,15 @@
     JobStatusType,
     ListAccessPointsForObjectLambdaPaginatorName,
     MFADeleteStatusType,
     MFADeleteType,
     MetricsStatusType,
     MultiRegionAccessPointStatusType,
     NetworkOriginType,
+    ObjectLambdaAccessPointAliasStatusType,
     ObjectLambdaAllowedFeatureType,
     ObjectLambdaTransformationConfigurationActionType,
     OperationNameType,
     OutputSchemaVersionType,
     OwnerOverrideType,
     ReplicaModificationsStatusType,
     ReplicationRuleStatusType,
@@ -375,14 +376,15 @@
     AdvancedDataProtectionMetricsTypeDef,
     DetailedStatusCodesMetricsTypeDef,
     AsyncErrorDetailsTypeDef,
     DeleteMultiRegionAccessPointInputTypeDef,
     PutMultiRegionAccessPointPolicyInputTypeDef,
     AwsLambdaTransformationTypeDef,
     CloudWatchMetricsTypeDef,
+    ObjectLambdaAccessPointAliasTypeDef,
     ResponseMetadataTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     CreateBucketConfigurationTypeDef,
     JobReportTypeDef,
     S3TagTypeDef,
     RegionTypeDef,
     DeleteAccessPointForObjectLambdaRequestRequestTypeDef,
@@ -440,15 +442,14 @@
     JobTimersTypeDef,
     LifecycleExpirationTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
     PaginatorConfigTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
-    ObjectLambdaAccessPointTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
     ListStorageLensConfigurationEntryTypeDef,
     ListStorageLensConfigurationsRequestRequestTypeDef,
@@ -472,14 +473,15 @@
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
     AccessPointTypeDef,
     DeleteMultiRegionAccessPointRequestRequestTypeDef,
     PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
     ObjectLambdaContentTransformationTypeDef,
+    ObjectLambdaAccessPointTypeDef,
     CreateAccessPointForObjectLambdaResultTypeDef,
     CreateAccessPointResultTypeDef,
     CreateBucketResultTypeDef,
     CreateJobResultTypeDef,
     CreateMultiRegionAccessPointResultTypeDef,
     DeleteMultiRegionAccessPointResultTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -513,15 +515,14 @@
     SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
     PutStorageLensConfigurationTaggingRequestRequestTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
     ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
-    ListAccessPointsForObjectLambdaResultTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     MultiRegionAccessPointPolicyDocumentTypeDef,
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
@@ -530,14 +531,15 @@
     S3GrantTypeDef,
     S3SetObjectLegalHoldOperationTypeDef,
     S3SetObjectRetentionOperationTypeDef,
     StorageLensDataExportEncryptionTypeDef,
     SourceSelectionCriteriaTypeDef,
     ListAccessPointsResultTypeDef,
     ObjectLambdaTransformationConfigurationTypeDef,
+    ListAccessPointsForObjectLambdaResultTypeDef,
     LifecycleRuleFilterTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     AsyncRequestParametersTypeDef,
     CreateMultiRegionAccessPointRequestRequestTypeDef,
     S3ManifestOutputLocationTypeDef,
     JobListDescriptorTypeDef,
```

### Comparing `mypy-boto3-s3control-1.26.90/README.md` & `mypy-boto3-s3control-1.26.92/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3control?color=blue)](https://pypistats.org/packages/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.26.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -286,14 +286,15 @@
     JobStatusType,
     ListAccessPointsForObjectLambdaPaginatorName,
     MFADeleteStatusType,
     MFADeleteType,
     MetricsStatusType,
     MultiRegionAccessPointStatusType,
     NetworkOriginType,
+    ObjectLambdaAccessPointAliasStatusType,
     ObjectLambdaAllowedFeatureType,
     ObjectLambdaTransformationConfigurationActionType,
     OperationNameType,
     OutputSchemaVersionType,
     OwnerOverrideType,
     ReplicaModificationsStatusType,
     ReplicationRuleStatusType,
@@ -343,14 +344,15 @@
     AdvancedDataProtectionMetricsTypeDef,
     DetailedStatusCodesMetricsTypeDef,
     AsyncErrorDetailsTypeDef,
     DeleteMultiRegionAccessPointInputTypeDef,
     PutMultiRegionAccessPointPolicyInputTypeDef,
     AwsLambdaTransformationTypeDef,
     CloudWatchMetricsTypeDef,
+    ObjectLambdaAccessPointAliasTypeDef,
     ResponseMetadataTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     CreateBucketConfigurationTypeDef,
     JobReportTypeDef,
     S3TagTypeDef,
     RegionTypeDef,
     DeleteAccessPointForObjectLambdaRequestRequestTypeDef,
@@ -408,15 +410,14 @@
     JobTimersTypeDef,
     LifecycleExpirationTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
     PaginatorConfigTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
-    ObjectLambdaAccessPointTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
     ListStorageLensConfigurationEntryTypeDef,
     ListStorageLensConfigurationsRequestRequestTypeDef,
@@ -440,14 +441,15 @@
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
     AccessPointTypeDef,
     DeleteMultiRegionAccessPointRequestRequestTypeDef,
     PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
     ObjectLambdaContentTransformationTypeDef,
+    ObjectLambdaAccessPointTypeDef,
     CreateAccessPointForObjectLambdaResultTypeDef,
     CreateAccessPointResultTypeDef,
     CreateBucketResultTypeDef,
     CreateJobResultTypeDef,
     CreateMultiRegionAccessPointResultTypeDef,
     DeleteMultiRegionAccessPointResultTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -481,15 +483,14 @@
     SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
     PutStorageLensConfigurationTaggingRequestRequestTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
     ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
-    ListAccessPointsForObjectLambdaResultTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     MultiRegionAccessPointPolicyDocumentTypeDef,
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
@@ -498,14 +499,15 @@
     S3GrantTypeDef,
     S3SetObjectLegalHoldOperationTypeDef,
     S3SetObjectRetentionOperationTypeDef,
     StorageLensDataExportEncryptionTypeDef,
     SourceSelectionCriteriaTypeDef,
     ListAccessPointsResultTypeDef,
     ObjectLambdaTransformationConfigurationTypeDef,
+    ListAccessPointsForObjectLambdaResultTypeDef,
     LifecycleRuleFilterTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     AsyncRequestParametersTypeDef,
     CreateMultiRegionAccessPointRequestRequestTypeDef,
     S3ManifestOutputLocationTypeDef,
     JobListDescriptorTypeDef,
```

### Comparing `mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/__init__.py` & `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/__init__.pyi` & `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/__main__.py` & `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3Control 1.26.90\nVersion:         1.26.90\nBuilder version:"
+        "Type annotations for boto3.S3Control 1.26.92\nVersion:         1.26.92\nBuilder version:"
         " 7.13.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.90")
+    print("1.26.92")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/client.py` & `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/client.pyi` & `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/literals.py` & `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     "JobStatusType",
     "ListAccessPointsForObjectLambdaPaginatorName",
     "MFADeleteStatusType",
     "MFADeleteType",
     "MetricsStatusType",
     "MultiRegionAccessPointStatusType",
     "NetworkOriginType",
+    "ObjectLambdaAccessPointAliasStatusType",
     "ObjectLambdaAllowedFeatureType",
     "ObjectLambdaTransformationConfigurationActionType",
     "OperationNameType",
     "OutputSchemaVersionType",
     "OwnerOverrideType",
     "ReplicaModificationsStatusType",
     "ReplicationRuleStatusType",
@@ -125,14 +126,15 @@
     "DELETING",
     "INCONSISTENT_ACROSS_REGIONS",
     "PARTIALLY_CREATED",
     "PARTIALLY_DELETED",
     "READY",
 ]
 NetworkOriginType = Literal["Internet", "VPC"]
+ObjectLambdaAccessPointAliasStatusType = Literal["PROVISIONING", "READY"]
 ObjectLambdaAllowedFeatureType = Literal[
     "GetObject-PartNumber", "GetObject-Range", "HeadObject-PartNumber", "HeadObject-Range"
 ]
 ObjectLambdaTransformationConfigurationActionType = Literal[
     "GetObject", "HeadObject", "ListObjects", "ListObjectsV2"
 ]
 OperationNameType = Literal[
```

### Comparing `mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/literals.pyi` & `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     "JobStatusType",
     "ListAccessPointsForObjectLambdaPaginatorName",
     "MFADeleteStatusType",
     "MFADeleteType",
     "MetricsStatusType",
     "MultiRegionAccessPointStatusType",
     "NetworkOriginType",
+    "ObjectLambdaAccessPointAliasStatusType",
     "ObjectLambdaAllowedFeatureType",
     "ObjectLambdaTransformationConfigurationActionType",
     "OperationNameType",
     "OutputSchemaVersionType",
     "OwnerOverrideType",
     "ReplicaModificationsStatusType",
     "ReplicationRuleStatusType",
@@ -123,14 +124,15 @@
     "DELETING",
     "INCONSISTENT_ACROSS_REGIONS",
     "PARTIALLY_CREATED",
     "PARTIALLY_DELETED",
     "READY",
 ]
 NetworkOriginType = Literal["Internet", "VPC"]
+ObjectLambdaAccessPointAliasStatusType = Literal["PROVISIONING", "READY"]
 ObjectLambdaAllowedFeatureType = Literal[
     "GetObject-PartNumber", "GetObject-Range", "HeadObject-PartNumber", "HeadObject-Range"
 ]
 ObjectLambdaTransformationConfigurationActionType = Literal[
     "GetObject", "HeadObject", "ListObjects", "ListObjectsV2"
 ]
 OperationNameType = Literal[
```

### Comparing `mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/paginator.py` & `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/paginator.pyi` & `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/type_defs.py` & `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     JobReportScopeType,
     JobStatusType,
     MetricsStatusType,
     MFADeleteStatusType,
     MFADeleteType,
     MultiRegionAccessPointStatusType,
     NetworkOriginType,
+    ObjectLambdaAccessPointAliasStatusType,
     ObjectLambdaAllowedFeatureType,
     ObjectLambdaTransformationConfigurationActionType,
     OperationNameType,
     ReplicaModificationsStatusType,
     ReplicationRuleStatusType,
     ReplicationStatusType,
     ReplicationStorageClassType,
@@ -76,14 +77,15 @@
     "AdvancedDataProtectionMetricsTypeDef",
     "DetailedStatusCodesMetricsTypeDef",
     "AsyncErrorDetailsTypeDef",
     "DeleteMultiRegionAccessPointInputTypeDef",
     "PutMultiRegionAccessPointPolicyInputTypeDef",
     "AwsLambdaTransformationTypeDef",
     "CloudWatchMetricsTypeDef",
+    "ObjectLambdaAccessPointAliasTypeDef",
     "ResponseMetadataTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
     "CreateBucketConfigurationTypeDef",
     "JobReportTypeDef",
     "S3TagTypeDef",
     "RegionTypeDef",
     "DeleteAccessPointForObjectLambdaRequestRequestTypeDef",
@@ -141,15 +143,14 @@
     "JobTimersTypeDef",
     "LifecycleExpirationTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
     "TransitionTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessPointsForObjectLambdaRequestRequestTypeDef",
-    "ObjectLambdaAccessPointTypeDef",
     "ListAccessPointsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListMultiRegionAccessPointsRequestRequestTypeDef",
     "ListRegionalBucketsRequestRequestTypeDef",
     "RegionalBucketTypeDef",
     "ListStorageLensConfigurationEntryTypeDef",
     "ListStorageLensConfigurationsRequestRequestTypeDef",
@@ -173,14 +174,15 @@
     "StorageLensAwsOrgTypeDef",
     "UpdateJobPriorityRequestRequestTypeDef",
     "UpdateJobStatusRequestRequestTypeDef",
     "AccessPointTypeDef",
     "DeleteMultiRegionAccessPointRequestRequestTypeDef",
     "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
     "ObjectLambdaContentTransformationTypeDef",
+    "ObjectLambdaAccessPointTypeDef",
     "CreateAccessPointForObjectLambdaResultTypeDef",
     "CreateAccessPointResultTypeDef",
     "CreateBucketResultTypeDef",
     "CreateJobResultTypeDef",
     "CreateMultiRegionAccessPointResultTypeDef",
     "DeleteMultiRegionAccessPointResultTypeDef",
     "EmptyResponseMetadataTypeDef",
@@ -214,15 +216,14 @@
     "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingResultTypeDef",
     "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
     "S3GeneratedManifestDescriptorTypeDef",
     "JobManifestTypeDef",
     "JobProgressSummaryTypeDef",
     "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
-    "ListAccessPointsForObjectLambdaResultTypeDef",
     "ListRegionalBucketsResultTypeDef",
     "ListStorageLensConfigurationsResultTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "MultiRegionAccessPointPolicyDocumentTypeDef",
     "MultiRegionAccessPointsAsyncResponseTypeDef",
     "MultiRegionAccessPointReportTypeDef",
@@ -231,14 +232,15 @@
     "S3GrantTypeDef",
     "S3SetObjectLegalHoldOperationTypeDef",
     "S3SetObjectRetentionOperationTypeDef",
     "StorageLensDataExportEncryptionTypeDef",
     "SourceSelectionCriteriaTypeDef",
     "ListAccessPointsResultTypeDef",
     "ObjectLambdaTransformationConfigurationTypeDef",
+    "ListAccessPointsForObjectLambdaResultTypeDef",
     "LifecycleRuleFilterTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "AsyncRequestParametersTypeDef",
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
     "S3ManifestOutputLocationTypeDef",
     "JobListDescriptorTypeDef",
@@ -386,14 +388,23 @@
 CloudWatchMetricsTypeDef = TypedDict(
     "CloudWatchMetricsTypeDef",
     {
         "IsEnabled": bool,
     },
 )
 
+ObjectLambdaAccessPointAliasTypeDef = TypedDict(
+    "ObjectLambdaAccessPointAliasTypeDef",
+    {
+        "Value": str,
+        "Status": ObjectLambdaAccessPointAliasStatusType,
+    },
+    total=False,
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -1001,35 +1012,14 @@
 class ListAccessPointsForObjectLambdaRequestRequestTypeDef(
     _RequiredListAccessPointsForObjectLambdaRequestRequestTypeDef,
     _OptionalListAccessPointsForObjectLambdaRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredObjectLambdaAccessPointTypeDef = TypedDict(
-    "_RequiredObjectLambdaAccessPointTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalObjectLambdaAccessPointTypeDef = TypedDict(
-    "_OptionalObjectLambdaAccessPointTypeDef",
-    {
-        "ObjectLambdaAccessPointArn": str,
-    },
-    total=False,
-)
-
-
-class ObjectLambdaAccessPointTypeDef(
-    _RequiredObjectLambdaAccessPointTypeDef, _OptionalObjectLambdaAccessPointTypeDef
-):
-    pass
-
-
 _RequiredListAccessPointsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessPointsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListAccessPointsRequestRequestTypeDef = TypedDict(
@@ -1441,18 +1431,41 @@
     "ObjectLambdaContentTransformationTypeDef",
     {
         "AwsLambda": AwsLambdaTransformationTypeDef,
     },
     total=False,
 )
 
+_RequiredObjectLambdaAccessPointTypeDef = TypedDict(
+    "_RequiredObjectLambdaAccessPointTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalObjectLambdaAccessPointTypeDef = TypedDict(
+    "_OptionalObjectLambdaAccessPointTypeDef",
+    {
+        "ObjectLambdaAccessPointArn": str,
+        "Alias": ObjectLambdaAccessPointAliasTypeDef,
+    },
+    total=False,
+)
+
+
+class ObjectLambdaAccessPointTypeDef(
+    _RequiredObjectLambdaAccessPointTypeDef, _OptionalObjectLambdaAccessPointTypeDef
+):
+    pass
+
+
 CreateAccessPointForObjectLambdaResultTypeDef = TypedDict(
     "CreateAccessPointForObjectLambdaResultTypeDef",
     {
         "ObjectLambdaAccessPointArn": str,
+        "Alias": ObjectLambdaAccessPointAliasTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAccessPointResultTypeDef = TypedDict(
     "CreateAccessPointResultTypeDef",
     {
@@ -1599,14 +1612,15 @@
 
 GetAccessPointForObjectLambdaResultTypeDef = TypedDict(
     "GetAccessPointForObjectLambdaResultTypeDef",
     {
         "Name": str,
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "CreationDate": datetime,
+        "Alias": ObjectLambdaAccessPointAliasTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccessPointResultTypeDef = TypedDict(
     "GetAccessPointResultTypeDef",
     {
@@ -1866,23 +1880,14 @@
 class ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef(
     _RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     _OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
 ):
     pass
 
 
-ListAccessPointsForObjectLambdaResultTypeDef = TypedDict(
-    "ListAccessPointsForObjectLambdaResultTypeDef",
-    {
-        "ObjectLambdaAccessPointList": List[ObjectLambdaAccessPointTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListRegionalBucketsResultTypeDef = TypedDict(
     "ListRegionalBucketsResultTypeDef",
     {
         "RegionalBucketList": List[RegionalBucketTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2055,14 +2060,23 @@
     "ObjectLambdaTransformationConfigurationTypeDef",
     {
         "Actions": Sequence[ObjectLambdaTransformationConfigurationActionType],
         "ContentTransformation": ObjectLambdaContentTransformationTypeDef,
     },
 )
 
+ListAccessPointsForObjectLambdaResultTypeDef = TypedDict(
+    "ListAccessPointsForObjectLambdaResultTypeDef",
+    {
+        "ObjectLambdaAccessPointList": List[ObjectLambdaAccessPointTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": S3TagTypeDef,
         "And": LifecycleRuleAndOperatorTypeDef,
         "ObjectSizeGreaterThan": int,
```

### Comparing `mypy-boto3-s3control-1.26.90/mypy_boto3_s3control/type_defs.pyi` & `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     JobReportScopeType,
     JobStatusType,
     MetricsStatusType,
     MFADeleteStatusType,
     MFADeleteType,
     MultiRegionAccessPointStatusType,
     NetworkOriginType,
+    ObjectLambdaAccessPointAliasStatusType,
     ObjectLambdaAllowedFeatureType,
     ObjectLambdaTransformationConfigurationActionType,
     OperationNameType,
     ReplicaModificationsStatusType,
     ReplicationRuleStatusType,
     ReplicationStatusType,
     ReplicationStorageClassType,
@@ -75,14 +76,15 @@
     "AdvancedDataProtectionMetricsTypeDef",
     "DetailedStatusCodesMetricsTypeDef",
     "AsyncErrorDetailsTypeDef",
     "DeleteMultiRegionAccessPointInputTypeDef",
     "PutMultiRegionAccessPointPolicyInputTypeDef",
     "AwsLambdaTransformationTypeDef",
     "CloudWatchMetricsTypeDef",
+    "ObjectLambdaAccessPointAliasTypeDef",
     "ResponseMetadataTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
     "CreateBucketConfigurationTypeDef",
     "JobReportTypeDef",
     "S3TagTypeDef",
     "RegionTypeDef",
     "DeleteAccessPointForObjectLambdaRequestRequestTypeDef",
@@ -140,15 +142,14 @@
     "JobTimersTypeDef",
     "LifecycleExpirationTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
     "TransitionTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessPointsForObjectLambdaRequestRequestTypeDef",
-    "ObjectLambdaAccessPointTypeDef",
     "ListAccessPointsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListMultiRegionAccessPointsRequestRequestTypeDef",
     "ListRegionalBucketsRequestRequestTypeDef",
     "RegionalBucketTypeDef",
     "ListStorageLensConfigurationEntryTypeDef",
     "ListStorageLensConfigurationsRequestRequestTypeDef",
@@ -172,14 +173,15 @@
     "StorageLensAwsOrgTypeDef",
     "UpdateJobPriorityRequestRequestTypeDef",
     "UpdateJobStatusRequestRequestTypeDef",
     "AccessPointTypeDef",
     "DeleteMultiRegionAccessPointRequestRequestTypeDef",
     "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
     "ObjectLambdaContentTransformationTypeDef",
+    "ObjectLambdaAccessPointTypeDef",
     "CreateAccessPointForObjectLambdaResultTypeDef",
     "CreateAccessPointResultTypeDef",
     "CreateBucketResultTypeDef",
     "CreateJobResultTypeDef",
     "CreateMultiRegionAccessPointResultTypeDef",
     "DeleteMultiRegionAccessPointResultTypeDef",
     "EmptyResponseMetadataTypeDef",
@@ -213,15 +215,14 @@
     "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingResultTypeDef",
     "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
     "S3GeneratedManifestDescriptorTypeDef",
     "JobManifestTypeDef",
     "JobProgressSummaryTypeDef",
     "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
-    "ListAccessPointsForObjectLambdaResultTypeDef",
     "ListRegionalBucketsResultTypeDef",
     "ListStorageLensConfigurationsResultTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "MultiRegionAccessPointPolicyDocumentTypeDef",
     "MultiRegionAccessPointsAsyncResponseTypeDef",
     "MultiRegionAccessPointReportTypeDef",
@@ -230,14 +231,15 @@
     "S3GrantTypeDef",
     "S3SetObjectLegalHoldOperationTypeDef",
     "S3SetObjectRetentionOperationTypeDef",
     "StorageLensDataExportEncryptionTypeDef",
     "SourceSelectionCriteriaTypeDef",
     "ListAccessPointsResultTypeDef",
     "ObjectLambdaTransformationConfigurationTypeDef",
+    "ListAccessPointsForObjectLambdaResultTypeDef",
     "LifecycleRuleFilterTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "AsyncRequestParametersTypeDef",
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
     "S3ManifestOutputLocationTypeDef",
     "JobListDescriptorTypeDef",
@@ -383,14 +385,23 @@
 CloudWatchMetricsTypeDef = TypedDict(
     "CloudWatchMetricsTypeDef",
     {
         "IsEnabled": bool,
     },
 )
 
+ObjectLambdaAccessPointAliasTypeDef = TypedDict(
+    "ObjectLambdaAccessPointAliasTypeDef",
+    {
+        "Value": str,
+        "Status": ObjectLambdaAccessPointAliasStatusType,
+    },
+    total=False,
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -986,33 +997,14 @@
 
 class ListAccessPointsForObjectLambdaRequestRequestTypeDef(
     _RequiredListAccessPointsForObjectLambdaRequestRequestTypeDef,
     _OptionalListAccessPointsForObjectLambdaRequestRequestTypeDef,
 ):
     pass
 
-_RequiredObjectLambdaAccessPointTypeDef = TypedDict(
-    "_RequiredObjectLambdaAccessPointTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalObjectLambdaAccessPointTypeDef = TypedDict(
-    "_OptionalObjectLambdaAccessPointTypeDef",
-    {
-        "ObjectLambdaAccessPointArn": str,
-    },
-    total=False,
-)
-
-class ObjectLambdaAccessPointTypeDef(
-    _RequiredObjectLambdaAccessPointTypeDef, _OptionalObjectLambdaAccessPointTypeDef
-):
-    pass
-
 _RequiredListAccessPointsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessPointsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListAccessPointsRequestRequestTypeDef = TypedDict(
@@ -1404,18 +1396,39 @@
     "ObjectLambdaContentTransformationTypeDef",
     {
         "AwsLambda": AwsLambdaTransformationTypeDef,
     },
     total=False,
 )
 
+_RequiredObjectLambdaAccessPointTypeDef = TypedDict(
+    "_RequiredObjectLambdaAccessPointTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalObjectLambdaAccessPointTypeDef = TypedDict(
+    "_OptionalObjectLambdaAccessPointTypeDef",
+    {
+        "ObjectLambdaAccessPointArn": str,
+        "Alias": ObjectLambdaAccessPointAliasTypeDef,
+    },
+    total=False,
+)
+
+class ObjectLambdaAccessPointTypeDef(
+    _RequiredObjectLambdaAccessPointTypeDef, _OptionalObjectLambdaAccessPointTypeDef
+):
+    pass
+
 CreateAccessPointForObjectLambdaResultTypeDef = TypedDict(
     "CreateAccessPointForObjectLambdaResultTypeDef",
     {
         "ObjectLambdaAccessPointArn": str,
+        "Alias": ObjectLambdaAccessPointAliasTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAccessPointResultTypeDef = TypedDict(
     "CreateAccessPointResultTypeDef",
     {
@@ -1560,14 +1573,15 @@
 
 GetAccessPointForObjectLambdaResultTypeDef = TypedDict(
     "GetAccessPointForObjectLambdaResultTypeDef",
     {
         "Name": str,
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "CreationDate": datetime,
+        "Alias": ObjectLambdaAccessPointAliasTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccessPointResultTypeDef = TypedDict(
     "GetAccessPointResultTypeDef",
     {
@@ -1821,23 +1835,14 @@
 
 class ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef(
     _RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     _OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
 ):
     pass
 
-ListAccessPointsForObjectLambdaResultTypeDef = TypedDict(
-    "ListAccessPointsForObjectLambdaResultTypeDef",
-    {
-        "ObjectLambdaAccessPointList": List[ObjectLambdaAccessPointTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListRegionalBucketsResultTypeDef = TypedDict(
     "ListRegionalBucketsResultTypeDef",
     {
         "RegionalBucketList": List[RegionalBucketTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2004,14 +2009,23 @@
     "ObjectLambdaTransformationConfigurationTypeDef",
     {
         "Actions": Sequence[ObjectLambdaTransformationConfigurationActionType],
         "ContentTransformation": ObjectLambdaContentTransformationTypeDef,
     },
 )
 
+ListAccessPointsForObjectLambdaResultTypeDef = TypedDict(
+    "ListAccessPointsForObjectLambdaResultTypeDef",
+    {
+        "ObjectLambdaAccessPointList": List[ObjectLambdaAccessPointTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": S3TagTypeDef,
         "And": LifecycleRuleAndOperatorTypeDef,
         "ObjectSizeGreaterThan": int,
```

### Comparing `mypy-boto3-s3control-1.26.90/mypy_boto3_s3control.egg-info/PKG-INFO` & `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3control
-Version: 1.26.90
-Summary: Type annotations for boto3.S3Control 1.26.90 service generated with mypy-boto3-builder 7.13.0
+Version: 1.26.92
+Summary: Type annotations for boto3.S3Control 1.26.92 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3control?color=blue)](https://pypistats.org/packages/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.26.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -318,14 +318,15 @@
     JobStatusType,
     ListAccessPointsForObjectLambdaPaginatorName,
     MFADeleteStatusType,
     MFADeleteType,
     MetricsStatusType,
     MultiRegionAccessPointStatusType,
     NetworkOriginType,
+    ObjectLambdaAccessPointAliasStatusType,
     ObjectLambdaAllowedFeatureType,
     ObjectLambdaTransformationConfigurationActionType,
     OperationNameType,
     OutputSchemaVersionType,
     OwnerOverrideType,
     ReplicaModificationsStatusType,
     ReplicationRuleStatusType,
@@ -375,14 +376,15 @@
     AdvancedDataProtectionMetricsTypeDef,
     DetailedStatusCodesMetricsTypeDef,
     AsyncErrorDetailsTypeDef,
     DeleteMultiRegionAccessPointInputTypeDef,
     PutMultiRegionAccessPointPolicyInputTypeDef,
     AwsLambdaTransformationTypeDef,
     CloudWatchMetricsTypeDef,
+    ObjectLambdaAccessPointAliasTypeDef,
     ResponseMetadataTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     CreateBucketConfigurationTypeDef,
     JobReportTypeDef,
     S3TagTypeDef,
     RegionTypeDef,
     DeleteAccessPointForObjectLambdaRequestRequestTypeDef,
@@ -440,15 +442,14 @@
     JobTimersTypeDef,
     LifecycleExpirationTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
     PaginatorConfigTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
-    ObjectLambdaAccessPointTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
     ListStorageLensConfigurationEntryTypeDef,
     ListStorageLensConfigurationsRequestRequestTypeDef,
@@ -472,14 +473,15 @@
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
     AccessPointTypeDef,
     DeleteMultiRegionAccessPointRequestRequestTypeDef,
     PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
     ObjectLambdaContentTransformationTypeDef,
+    ObjectLambdaAccessPointTypeDef,
     CreateAccessPointForObjectLambdaResultTypeDef,
     CreateAccessPointResultTypeDef,
     CreateBucketResultTypeDef,
     CreateJobResultTypeDef,
     CreateMultiRegionAccessPointResultTypeDef,
     DeleteMultiRegionAccessPointResultTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -513,15 +515,14 @@
     SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
     PutStorageLensConfigurationTaggingRequestRequestTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
     ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
-    ListAccessPointsForObjectLambdaResultTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     MultiRegionAccessPointPolicyDocumentTypeDef,
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
@@ -530,14 +531,15 @@
     S3GrantTypeDef,
     S3SetObjectLegalHoldOperationTypeDef,
     S3SetObjectRetentionOperationTypeDef,
     StorageLensDataExportEncryptionTypeDef,
     SourceSelectionCriteriaTypeDef,
     ListAccessPointsResultTypeDef,
     ObjectLambdaTransformationConfigurationTypeDef,
+    ListAccessPointsForObjectLambdaResultTypeDef,
     LifecycleRuleFilterTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     AsyncRequestParametersTypeDef,
     CreateMultiRegionAccessPointRequestRequestTypeDef,
     S3ManifestOutputLocationTypeDef,
     JobListDescriptorTypeDef,
```

### Comparing `mypy-boto3-s3control-1.26.90/mypy_boto3_s3control.egg-info/SOURCES.txt` & `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.26.90/setup.py` & `mypy-boto3-s3control-1.26.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-s3control",
-    version="1.26.90",
+    version="1.26.92",
     packages=["mypy_boto3_s3control"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.S3Control 1.26.90 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.S3Control 1.26.92 service generated with mypy-boto3-builder"
         " 7.13.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

