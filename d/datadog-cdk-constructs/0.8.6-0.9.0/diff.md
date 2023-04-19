# Comparing `tmp/datadog-cdk-constructs-0.8.6.tar.gz` & `tmp/datadog-cdk-constructs-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog-cdk-constructs-0.8.6.tar", last modified: Thu Mar 30 20:15:05 2023, max compression
+gzip compressed data, was "datadog-cdk-constructs-0.9.0.tar", last modified: Wed Apr 19 17:00:52 2023, max compression
```

## Comparing `datadog-cdk-constructs-0.8.6.tar` & `datadog-cdk-constructs-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-03-30 20:15:05.281193 datadog-cdk-constructs-0.8.6/
--rw-r--r--   0 david.lee   (503) staff       (20)    11358 2023-03-30 20:15:01.000000 datadog-cdk-constructs-0.8.6/LICENSE
--rw-r--r--   0 david.lee   (503) staff       (20)       23 2023-03-30 20:15:01.000000 datadog-cdk-constructs-0.8.6/MANIFEST.in
--rw-r--r--   0 david.lee   (503) staff       (20)    21958 2023-03-30 20:15:05.281046 datadog-cdk-constructs-0.8.6/PKG-INFO
--rw-r--r--   0 david.lee   (503) staff       (20)    20999 2023-03-30 20:15:01.000000 datadog-cdk-constructs-0.8.6/README.md
--rw-r--r--   0 david.lee   (503) staff       (20)      106 2023-03-30 20:15:01.000000 datadog-cdk-constructs-0.8.6/pyproject.toml
--rw-r--r--   0 david.lee   (503) staff       (20)       38 2023-03-30 20:15:05.281253 datadog-cdk-constructs-0.8.6/setup.cfg
--rw-r--r--   0 david.lee   (503) staff       (20)     2104 2023-03-30 20:15:01.000000 datadog-cdk-constructs-0.8.6/setup.py
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-03-30 20:15:05.278180 datadog-cdk-constructs-0.8.6/src/
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-03-30 20:15:05.279500 datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs/
--rw-r--r--   0 david.lee   (503) staff       (20)    60325 2023-03-30 20:15:01.000000 datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs/__init__.py
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-03-30 20:15:05.280726 datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs/_jsii/
--rw-r--r--   0 david.lee   (503) staff       (20)      614 2023-03-30 20:15:01.000000 datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 david.lee   (503) staff       (20)   126892 2023-03-30 20:15:01.000000 datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs/_jsii/datadog-cdk-constructs@0.8.6.jsii.tgz
--rw-r--r--   0 david.lee   (503) staff       (20)        1 2023-03-30 20:15:01.000000 datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs/py.typed
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-03-30 20:15:05.280382 datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs.egg-info/
--rw-r--r--   0 david.lee   (503) staff       (20)    21958 2023-03-30 20:15:05.000000 datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 david.lee   (503) staff       (20)      493 2023-03-30 20:15:05.000000 datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 david.lee   (503) staff       (20)        1 2023-03-30 20:15:05.000000 datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 david.lee   (503) staff       (20)      331 2023-03-30 20:15:05.000000 datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 david.lee   (503) staff       (20)       23 2023-03-30 20:15:05.000000 datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 17:00:52.123770 datadog-cdk-constructs-0.9.0/
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    11358 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/LICENSE
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)       23 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/MANIFEST.in
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    22767 2023-04-19 17:00:52.123619 datadog-cdk-constructs-0.9.0/PKG-INFO
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    21808 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/README.md
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)      106 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/pyproject.toml
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)       38 2023-04-19 17:00:52.123808 datadog-cdk-constructs-0.9.0/setup.cfg
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)     2104 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/setup.py
+drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 17:00:52.120953 datadog-cdk-constructs-0.9.0/src/
+drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 17:00:52.122075 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    61134 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/__init__.py
+drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 17:00:52.123325 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/_jsii/
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)      614 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)   102261 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/_jsii/datadog-cdk-constructs@0.9.0.jsii.tgz
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)        1 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/py.typed
+drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 17:00:52.122972 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs.egg-info/
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    22767 2023-04-19 17:00:52.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)      493 2023-04-19 17:00:52.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)        1 2023-04-19 17:00:52.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)      331 2023-04-19 17:00:52.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)       23 2023-04-19 17:00:52.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs.egg-info/top_level.txt
```

### Comparing `datadog-cdk-constructs-0.8.6/LICENSE` & `datadog-cdk-constructs-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog-cdk-constructs-0.8.6/PKG-INFO` & `datadog-cdk-constructs-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-cdk-constructs
-Version: 0.8.6
+Version: 0.9.0
 Summary: CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog
 Home-page: https://github.com/DataDog/datadog-cdk-constructs
 Author: Datadog
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataDog/datadog-cdk-constructs
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -30,15 +30,15 @@
 [![PyPI](https://img.shields.io/pypi/v/datadog-cdk-constructs-v2?color=39a356&label=pypi+cdk+v2)](https://pypi.org/project/datadog-cdk-constructs-v2/)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-cdk-constructs/blob/main/LICENSE)
 
 Use this Datadog CDK Construct Library to deploy serverless applications using AWS CDK .
 
 This CDK library automatically configures ingestion of metrics, traces, and logs from your serverless applications by:
 
-* Installing and configuring the Datadog Lambda library for your [Python](https://github.com/DataDog/datadog-lambda-layer-python) and [Node.js](https://github.com/DataDog/datadog-lambda-layer-js) Lambda functions.
+* Installing and configuring the Datadog Lambda layers for your [Python](https://github.com/DataDog/datadog-lambda-layer-python), [Node.js](https://github.com/DataDog/datadog-lambda-layer-js), and [Java](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk) Lambda functions.
 * Enabling the collection of traces and custom metrics from your Lambda functions.
 * Managing subscriptions from the Datadog Forwarder to your Lambda and non-Lambda log groups.
 
 ## AWS CDK v1 vs AWS CDK v2
 
 Two separate versions of Datadog CDK Constructs exist; `datadog-cdk-constructs` and `datadog-cdk-constructs-v2`. These are designed to work with `AWS CDK v1` and `AWS CDK v2` respectively.
 
@@ -93,14 +93,15 @@
 ```python
 # Example automatically generated from non-compiling source. May contain errors.
 from datadog_cdk_constructs_v2 import Datadog
 
 datadog = Datadog(self, "Datadog",
     node_layer_version=<LAYER_VERSION>,
     python_layer_version=<LAYER_VERSION>,
+    java_layer_version=<LAYER_VERSION>,
     add_layers=<BOOLEAN>,
     extension_layer_version="<EXTENSION_VERSION>",
     forwarder_arn="<FORWARDER_ARN>",
     create_forwarder_permissions=<BOOLEAN>,
     flush_metrics_to_logs=<BOOLEAN>,
     site="<SITE>",
     api_key="{Datadog_API_Key}",
@@ -195,19 +196,20 @@
 *Note*: The descriptions use the npm package parameters, but they also apply to the PyPI package parameters.
 
 | npm package parameter | PyPI package parameter | Description |
 | --- | --- | --- |
 | `addLayers` | `add_layers` | Whether to add the Lambda Layers or expect the user to bring their own. Defaults to true. When true, the Lambda Library version variables are also required. When false, you must include the Datadog Lambda library in your functions' deployment packages. |
 | `pythonLayerVersion` | `python_layer_version` | Version of the Python Lambda layer to install, such as 21. Required if you are deploying at least one Lambda function written in Python and `addLayers` is true. Find the latest version number [here](https://github.com/DataDog/datadog-lambda-python/releases). |
 | `nodeLayerVersion` | `node_layer_version` | Version of the Node.js Lambda layer to install, such as 29. Required if you are deploying at least one Lambda function written in Node.js and `addLayers` is true. Find the latest version number from [here](https://github.com/DataDog/datadog-lambda-js/releases). |
+| `javaLayerVersion` | `java_layer_version` | Version of the Java layer to install, such as 8. Required if you are deploying at least one Lambda function written in Java and `addLayers` is true. Find the latest version number in the [Serverless Java installation documentation](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk). **Note**: `extensionLayerVersion >= 25` and `javaLayerVersion >= 5` are required for the Datadog construct to instrument your Java functions properly. |
 | `extensionLayerVersion` | `extension_layer_version` | Version of the Datadog Lambda Extension layer to install, such as 5. When `extensionLayerVersion` is set, `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`) needs to be set as well. When enabled, lambda function log groups will not be subscribed by the forwarder. Learn more about the Lambda extension [here](https://docs.datadoghq.com/serverless/datadog_lambda_library/extension/). |
 | `forwarderArn` | `forwarder_arn` | When set, the plugin will automatically subscribe the Datadog Forwarder to the functions' log groups. Do not set `forwarderArn` when `extensionLayerVersion` is set. |
 | `createForwarderPermissions` | `createForwarderPermissions` | When set to `true`, creates a Lambda permission on the the Datadog Forwarder per log group. Since the Datadog Forwarder has permissions configured by default, this is unnecessary in most use cases. |
 | `flushMetricsToLogs` | `flush_metrics_to_logs` | Send custom metrics using CloudWatch logs with the Datadog Forwarder Lambda function (recommended). Defaults to `true` . If you disable this parameter, it's required to set `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`). |
-| `site` | `site` | Set which Datadog site to send data. This is only used when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. Possible values are `datadoghq.com`, `datadoghq.eu`, `us3.datadoghq.com`, `us5.datadoghq.com`, and `ddog-gov.com`. The default is `datadoghq.com`. |
+| `site` | `site` | Set which Datadog site to send data. This is only used when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. Possible values are `datadoghq.com`, `datadoghq.eu`, `us3.datadoghq.com`, `us5.datadoghq.com`, `ap1.datadoghq.com`, and `ddog-gov.com`. The default is `datadoghq.com`. |
 | `apiKey` | `api_key` | Datadog API Key, only needed when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. For more information about getting a Datadog API key, see the [API key documentation](https://docs.datadoghq.com/account_management/api-app-keys/#api-keys). |
 | `apiKeySecretArn` | `api_key_secret_arn` | The ARN of the secret storing the Datadog API key in AWS Secrets Manager. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayer` is set. Remember to add the `secretsmanager:GetSecretValue` permission to the Lambda execution role. |
 | `apiKmsKey` | `api_kms_key` | Datadog API Key encrypted using KMS. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set, and you are using KMS encryption. |
 | `enableDatadogTracing` | `enable_datadog_tracing` | Enable Datadog tracing on your Lambda functions. Defaults to `true`. |
 | `enableMergeXrayTraces` | `enable_merge_xray_traces` | Enable merging X-Ray traces on your Lambda functions. Defaults to `false`. |
 | `enableDatadogLogs` | `enable_datadog_logs` | Send Lambda function logs to Datadog via the Datadog Lambda Extension.  Defaults to `true`. Note: This setting has no effect on logs sent via the Datadog Forwarder. |
 | `enableSourceCodeIntegration` | `enable_source_code_integration` | Enable Datadog Source Code Integration, connecting your telemetry with application code in your Git repositories. This requires the Datadog Github Integration to work, otherwise please follow the [alternative method](#alternative-methods-to-enable-source-code-integration). Learn more [here](https://docs.datadoghq.com/integrations/guide/source-code-integration/). Defaults to `true`. |
@@ -219,15 +221,15 @@
 | `tags` | `tags` | A comma separated list of key:value pairs as a single string. When set along with `extensionLayerVersion`, a `DD_TAGS` environment variable is added to all Lambda functions with the provided value. When set along with `forwarderArn`, the cdk parses the string and sets each key:value pair as a tag to all Lambda functions. |
 | `enableColdStartTracing`      | `enable_cold_start_tracing` | Set to `false` to disable Cold Start Tracing. Used in NodeJS and Python. Defaults to `true`. |
 | `coldStartTraceMinDuration`   | `min_cold_start_trace_duration` | Sets the minimum duration (in milliseconds) for a module load event to be traced via Cold Start Tracing. Number. Defaults to `3`. |
 | `coldStartTraceSkipLibs`      | `cold_start_trace_skip_libs`| Optionally skip creating Cold Start Spans for a comma-separated list of libraries. Useful to limit depth or skip known libraries. Default depends on runtime. |
 | `enableProfiling`             | `enable_profiling` | Enable the Datadog Continuous Profiler with `true`. Supported in Beta for NodeJS and Python. Defaults to `false`. |
 | `encodeAuthorizerContext`     |`encode_authorizer_context` | When set to `true` for Lambda authorizers, the tracing context will be encoded into the response for propagation. Supported for NodeJS and Python. Defaults to `true`. |
 | `decodeAuthorizerContext`     |`decode_authorizer_context` | When set to `true` for Lambdas that are authorized via Lambda authorizers, it will parse and use the encoded tracing context (if found). Supported for NodeJS and Python. Defaults to `true`.                         |
-| `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set. The tracer will attempt to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
+| `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set, the tracer attempts to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
 
 **Note**: Using the parameters above may override corresponding function level `DD_XXX` environment variables.
 
 ### Tracing
 
 Enable X-Ray Tracing on your Lambda functions. For more information, see [CDK documentation](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-lambda.Tracing.html).
 
@@ -257,14 +259,15 @@
     def __init__(self, scope, id, props=None):
         super().__init__(scope, id, props)
         NestedStack(self, "NestedStack")
 
         datadog = Datadog(self, "Datadog",
             node_layer_version=<LAYER_VERSION>,
             python_layer_version=<LAYER_VERSION>,
+            java_layer_version=<LAYER_VERSION>,
             add_layers=<BOOLEAN>,
             forwarder_arn="<FORWARDER_ARN>",
             flush_metrics_to_logs=<BOOLEAN>,
             site="<SITE>",
             api_key="{Datadog_API_Key}",
             api_key_secret_arn="{Secret_ARN_Datadog_API_Key}",
             api_kms_key="{Encrypted_Datadog_API_Key}",
@@ -278,14 +281,15 @@
 class NestedStack(cdk.NestedStack):
     def __init__(self, scope, id, props=None):
         super().__init__(scope, id, props)
 
         datadog = Datadog(self, "Datadog",
             node_layer_version=<LAYER_VERSION>,
             python_layer_version=<LAYER_VERSION>,
+            java_layer_version=<LAYER_VERSION>,
             add_layers=<BOOLEAN>,
             forwarder_arn="<FORWARDER_ARN>",
             flush_metrics_to_logs=<BOOLEAN>,
             site="<SITE>",
             api_key="{Datadog_API_Key}",
             api_key_secret_arn="{Secret_ARN_Datadog_API_Key}",
             api_kms_key="{Encrypted_Datadog_API_Key}",
@@ -299,15 +303,15 @@
 
 ### Tags
 
 Add tags to your constructs. We recommend setting an `env` and `service` tag to tie Datadog telemetry together. For more information see [official AWS documentation](https://docs.aws.amazon.com/cdk/latest/guide/tagging.html) and [CDK documentation](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.Tags.html).
 
 ## How it works
 
-The Datadog CDK construct takes in a list of lambda functions and installs the Datadog Lambda Library by attaching the Lambda Layers for [Node.js](https://github.com/DataDog/datadog-lambda-layer-js) and [Python](https://github.com/DataDog/datadog-lambda-layer-python) to your functions. It redirects to a replacement handler that initializes the Lambda Library without any required code changes. Additional configurations added to the Datadog CDK construct will also translate into their respective environment variables under each lambda function (if applicable / required).
+The Datadog CDK construct takes in a list of lambda functions and installs the Datadog Lambda Library by attaching the Lambda Layers for [Java](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk), [Node.js](https://github.com/DataDog/datadog-lambda-layer-js), and [Python](https://github.com/DataDog/datadog-lambda-layer-python) to your functions. It redirects to a replacement handler that initializes the Lambda Library without any required code changes. Additional configurations added to the Datadog CDK construct will also translate into their respective environment variables under each lambda function (if applicable / required).
 
 While Lambda function based log groups are handled by the `addLambdaFunctions` method automatically, the construct has an additional function `addForwarderToNonLambdaLogGroups` which subscribes the forwarder to any additional log groups of your choosing.
 
 ## Resources to learn about CDK
 
 * [CDK TypeScript Workshop](https://cdkworkshop.com/20-typescript.html)
 * [Video Introducing CDK by AWS with Demo](https://youtu.be/ZWCvNFUN-sU)
```

### Comparing `datadog-cdk-constructs-0.8.6/README.md` & `datadog-cdk-constructs-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI](https://img.shields.io/pypi/v/datadog-cdk-constructs-v2?color=39a356&label=pypi+cdk+v2)](https://pypi.org/project/datadog-cdk-constructs-v2/)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-cdk-constructs/blob/main/LICENSE)
 
 Use this Datadog CDK Construct Library to deploy serverless applications using AWS CDK .
 
 This CDK library automatically configures ingestion of metrics, traces, and logs from your serverless applications by:
 
-* Installing and configuring the Datadog Lambda library for your [Python](https://github.com/DataDog/datadog-lambda-layer-python) and [Node.js](https://github.com/DataDog/datadog-lambda-layer-js) Lambda functions.
+* Installing and configuring the Datadog Lambda layers for your [Python](https://github.com/DataDog/datadog-lambda-layer-python), [Node.js](https://github.com/DataDog/datadog-lambda-layer-js), and [Java](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk) Lambda functions.
 * Enabling the collection of traces and custom metrics from your Lambda functions.
 * Managing subscriptions from the Datadog Forwarder to your Lambda and non-Lambda log groups.
 
 ## AWS CDK v1 vs AWS CDK v2
 
 Two separate versions of Datadog CDK Constructs exist; `datadog-cdk-constructs` and `datadog-cdk-constructs-v2`. These are designed to work with `AWS CDK v1` and `AWS CDK v2` respectively.
 
@@ -69,14 +69,15 @@
 ```python
 # Example automatically generated from non-compiling source. May contain errors.
 from datadog_cdk_constructs_v2 import Datadog
 
 datadog = Datadog(self, "Datadog",
     node_layer_version=<LAYER_VERSION>,
     python_layer_version=<LAYER_VERSION>,
+    java_layer_version=<LAYER_VERSION>,
     add_layers=<BOOLEAN>,
     extension_layer_version="<EXTENSION_VERSION>",
     forwarder_arn="<FORWARDER_ARN>",
     create_forwarder_permissions=<BOOLEAN>,
     flush_metrics_to_logs=<BOOLEAN>,
     site="<SITE>",
     api_key="{Datadog_API_Key}",
@@ -171,19 +172,20 @@
 *Note*: The descriptions use the npm package parameters, but they also apply to the PyPI package parameters.
 
 | npm package parameter | PyPI package parameter | Description |
 | --- | --- | --- |
 | `addLayers` | `add_layers` | Whether to add the Lambda Layers or expect the user to bring their own. Defaults to true. When true, the Lambda Library version variables are also required. When false, you must include the Datadog Lambda library in your functions' deployment packages. |
 | `pythonLayerVersion` | `python_layer_version` | Version of the Python Lambda layer to install, such as 21. Required if you are deploying at least one Lambda function written in Python and `addLayers` is true. Find the latest version number [here](https://github.com/DataDog/datadog-lambda-python/releases). |
 | `nodeLayerVersion` | `node_layer_version` | Version of the Node.js Lambda layer to install, such as 29. Required if you are deploying at least one Lambda function written in Node.js and `addLayers` is true. Find the latest version number from [here](https://github.com/DataDog/datadog-lambda-js/releases). |
+| `javaLayerVersion` | `java_layer_version` | Version of the Java layer to install, such as 8. Required if you are deploying at least one Lambda function written in Java and `addLayers` is true. Find the latest version number in the [Serverless Java installation documentation](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk). **Note**: `extensionLayerVersion >= 25` and `javaLayerVersion >= 5` are required for the Datadog construct to instrument your Java functions properly. |
 | `extensionLayerVersion` | `extension_layer_version` | Version of the Datadog Lambda Extension layer to install, such as 5. When `extensionLayerVersion` is set, `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`) needs to be set as well. When enabled, lambda function log groups will not be subscribed by the forwarder. Learn more about the Lambda extension [here](https://docs.datadoghq.com/serverless/datadog_lambda_library/extension/). |
 | `forwarderArn` | `forwarder_arn` | When set, the plugin will automatically subscribe the Datadog Forwarder to the functions' log groups. Do not set `forwarderArn` when `extensionLayerVersion` is set. |
 | `createForwarderPermissions` | `createForwarderPermissions` | When set to `true`, creates a Lambda permission on the the Datadog Forwarder per log group. Since the Datadog Forwarder has permissions configured by default, this is unnecessary in most use cases. |
 | `flushMetricsToLogs` | `flush_metrics_to_logs` | Send custom metrics using CloudWatch logs with the Datadog Forwarder Lambda function (recommended). Defaults to `true` . If you disable this parameter, it's required to set `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`). |
-| `site` | `site` | Set which Datadog site to send data. This is only used when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. Possible values are `datadoghq.com`, `datadoghq.eu`, `us3.datadoghq.com`, `us5.datadoghq.com`, and `ddog-gov.com`. The default is `datadoghq.com`. |
+| `site` | `site` | Set which Datadog site to send data. This is only used when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. Possible values are `datadoghq.com`, `datadoghq.eu`, `us3.datadoghq.com`, `us5.datadoghq.com`, `ap1.datadoghq.com`, and `ddog-gov.com`. The default is `datadoghq.com`. |
 | `apiKey` | `api_key` | Datadog API Key, only needed when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. For more information about getting a Datadog API key, see the [API key documentation](https://docs.datadoghq.com/account_management/api-app-keys/#api-keys). |
 | `apiKeySecretArn` | `api_key_secret_arn` | The ARN of the secret storing the Datadog API key in AWS Secrets Manager. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayer` is set. Remember to add the `secretsmanager:GetSecretValue` permission to the Lambda execution role. |
 | `apiKmsKey` | `api_kms_key` | Datadog API Key encrypted using KMS. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set, and you are using KMS encryption. |
 | `enableDatadogTracing` | `enable_datadog_tracing` | Enable Datadog tracing on your Lambda functions. Defaults to `true`. |
 | `enableMergeXrayTraces` | `enable_merge_xray_traces` | Enable merging X-Ray traces on your Lambda functions. Defaults to `false`. |
 | `enableDatadogLogs` | `enable_datadog_logs` | Send Lambda function logs to Datadog via the Datadog Lambda Extension.  Defaults to `true`. Note: This setting has no effect on logs sent via the Datadog Forwarder. |
 | `enableSourceCodeIntegration` | `enable_source_code_integration` | Enable Datadog Source Code Integration, connecting your telemetry with application code in your Git repositories. This requires the Datadog Github Integration to work, otherwise please follow the [alternative method](#alternative-methods-to-enable-source-code-integration). Learn more [here](https://docs.datadoghq.com/integrations/guide/source-code-integration/). Defaults to `true`. |
@@ -195,15 +197,15 @@
 | `tags` | `tags` | A comma separated list of key:value pairs as a single string. When set along with `extensionLayerVersion`, a `DD_TAGS` environment variable is added to all Lambda functions with the provided value. When set along with `forwarderArn`, the cdk parses the string and sets each key:value pair as a tag to all Lambda functions. |
 | `enableColdStartTracing`      | `enable_cold_start_tracing` | Set to `false` to disable Cold Start Tracing. Used in NodeJS and Python. Defaults to `true`. |
 | `coldStartTraceMinDuration`   | `min_cold_start_trace_duration` | Sets the minimum duration (in milliseconds) for a module load event to be traced via Cold Start Tracing. Number. Defaults to `3`. |
 | `coldStartTraceSkipLibs`      | `cold_start_trace_skip_libs`| Optionally skip creating Cold Start Spans for a comma-separated list of libraries. Useful to limit depth or skip known libraries. Default depends on runtime. |
 | `enableProfiling`             | `enable_profiling` | Enable the Datadog Continuous Profiler with `true`. Supported in Beta for NodeJS and Python. Defaults to `false`. |
 | `encodeAuthorizerContext`     |`encode_authorizer_context` | When set to `true` for Lambda authorizers, the tracing context will be encoded into the response for propagation. Supported for NodeJS and Python. Defaults to `true`. |
 | `decodeAuthorizerContext`     |`decode_authorizer_context` | When set to `true` for Lambdas that are authorized via Lambda authorizers, it will parse and use the encoded tracing context (if found). Supported for NodeJS and Python. Defaults to `true`.                         |
-| `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set. The tracer will attempt to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
+| `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set, the tracer attempts to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
 
 **Note**: Using the parameters above may override corresponding function level `DD_XXX` environment variables.
 
 ### Tracing
 
 Enable X-Ray Tracing on your Lambda functions. For more information, see [CDK documentation](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-lambda.Tracing.html).
 
@@ -233,14 +235,15 @@
     def __init__(self, scope, id, props=None):
         super().__init__(scope, id, props)
         NestedStack(self, "NestedStack")
 
         datadog = Datadog(self, "Datadog",
             node_layer_version=<LAYER_VERSION>,
             python_layer_version=<LAYER_VERSION>,
+            java_layer_version=<LAYER_VERSION>,
             add_layers=<BOOLEAN>,
             forwarder_arn="<FORWARDER_ARN>",
             flush_metrics_to_logs=<BOOLEAN>,
             site="<SITE>",
             api_key="{Datadog_API_Key}",
             api_key_secret_arn="{Secret_ARN_Datadog_API_Key}",
             api_kms_key="{Encrypted_Datadog_API_Key}",
@@ -254,14 +257,15 @@
 class NestedStack(cdk.NestedStack):
     def __init__(self, scope, id, props=None):
         super().__init__(scope, id, props)
 
         datadog = Datadog(self, "Datadog",
             node_layer_version=<LAYER_VERSION>,
             python_layer_version=<LAYER_VERSION>,
+            java_layer_version=<LAYER_VERSION>,
             add_layers=<BOOLEAN>,
             forwarder_arn="<FORWARDER_ARN>",
             flush_metrics_to_logs=<BOOLEAN>,
             site="<SITE>",
             api_key="{Datadog_API_Key}",
             api_key_secret_arn="{Secret_ARN_Datadog_API_Key}",
             api_kms_key="{Encrypted_Datadog_API_Key}",
@@ -275,15 +279,15 @@
 
 ### Tags
 
 Add tags to your constructs. We recommend setting an `env` and `service` tag to tie Datadog telemetry together. For more information see [official AWS documentation](https://docs.aws.amazon.com/cdk/latest/guide/tagging.html) and [CDK documentation](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.Tags.html).
 
 ## How it works
 
-The Datadog CDK construct takes in a list of lambda functions and installs the Datadog Lambda Library by attaching the Lambda Layers for [Node.js](https://github.com/DataDog/datadog-lambda-layer-js) and [Python](https://github.com/DataDog/datadog-lambda-layer-python) to your functions. It redirects to a replacement handler that initializes the Lambda Library without any required code changes. Additional configurations added to the Datadog CDK construct will also translate into their respective environment variables under each lambda function (if applicable / required).
+The Datadog CDK construct takes in a list of lambda functions and installs the Datadog Lambda Library by attaching the Lambda Layers for [Java](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk), [Node.js](https://github.com/DataDog/datadog-lambda-layer-js), and [Python](https://github.com/DataDog/datadog-lambda-layer-python) to your functions. It redirects to a replacement handler that initializes the Lambda Library without any required code changes. Additional configurations added to the Datadog CDK construct will also translate into their respective environment variables under each lambda function (if applicable / required).
 
 While Lambda function based log groups are handled by the `addLambdaFunctions` method automatically, the construct has an additional function `addForwarderToNonLambdaLogGroups` which subscribes the forwarder to any additional log groups of your choosing.
 
 ## Resources to learn about CDK
 
 * [CDK TypeScript Workshop](https://cdkworkshop.com/20-typescript.html)
 * [Video Introducing CDK by AWS with Demo](https://youtu.be/ZWCvNFUN-sU)
```

### Comparing `datadog-cdk-constructs-0.8.6/setup.py` & `datadog-cdk-constructs-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "datadog-cdk-constructs",
-    "version": "0.8.6",
+    "version": "0.9.0",
     "description": "CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog",
     "license": "Apache-2.0",
     "url": "https://github.com/DataDog/datadog-cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "Datadog",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "datadog_cdk_constructs",
         "datadog_cdk_constructs._jsii"
     ],
     "package_data": {
         "datadog_cdk_constructs._jsii": [
-            "datadog-cdk-constructs@0.8.6.jsii.tgz"
+            "datadog-cdk-constructs@0.9.0.jsii.tgz"
         ],
         "datadog_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
```

### Comparing `datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs/__init__.py` & `datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![PyPI](https://img.shields.io/pypi/v/datadog-cdk-constructs-v2?color=39a356&label=pypi+cdk+v2)](https://pypi.org/project/datadog-cdk-constructs-v2/)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-cdk-constructs/blob/main/LICENSE)
 
 Use this Datadog CDK Construct Library to deploy serverless applications using AWS CDK .
 
 This CDK library automatically configures ingestion of metrics, traces, and logs from your serverless applications by:
 
-* Installing and configuring the Datadog Lambda library for your [Python](https://github.com/DataDog/datadog-lambda-layer-python) and [Node.js](https://github.com/DataDog/datadog-lambda-layer-js) Lambda functions.
+* Installing and configuring the Datadog Lambda layers for your [Python](https://github.com/DataDog/datadog-lambda-layer-python), [Node.js](https://github.com/DataDog/datadog-lambda-layer-js), and [Java](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk) Lambda functions.
 * Enabling the collection of traces and custom metrics from your Lambda functions.
 * Managing subscriptions from the Datadog Forwarder to your Lambda and non-Lambda log groups.
 
 ## AWS CDK v1 vs AWS CDK v2
 
 Two separate versions of Datadog CDK Constructs exist; `datadog-cdk-constructs` and `datadog-cdk-constructs-v2`. These are designed to work with `AWS CDK v1` and `AWS CDK v2` respectively.
 
@@ -70,14 +70,15 @@
 ```python
 # Example automatically generated from non-compiling source. May contain errors.
 from datadog_cdk_constructs_v2 import Datadog
 
 datadog = Datadog(self, "Datadog",
     node_layer_version=<LAYER_VERSION>,
     python_layer_version=<LAYER_VERSION>,
+    java_layer_version=<LAYER_VERSION>,
     add_layers=<BOOLEAN>,
     extension_layer_version="<EXTENSION_VERSION>",
     forwarder_arn="<FORWARDER_ARN>",
     create_forwarder_permissions=<BOOLEAN>,
     flush_metrics_to_logs=<BOOLEAN>,
     site="<SITE>",
     api_key="{Datadog_API_Key}",
@@ -172,19 +173,20 @@
 *Note*: The descriptions use the npm package parameters, but they also apply to the PyPI package parameters.
 
 | npm package parameter | PyPI package parameter | Description |
 | --- | --- | --- |
 | `addLayers` | `add_layers` | Whether to add the Lambda Layers or expect the user to bring their own. Defaults to true. When true, the Lambda Library version variables are also required. When false, you must include the Datadog Lambda library in your functions' deployment packages. |
 | `pythonLayerVersion` | `python_layer_version` | Version of the Python Lambda layer to install, such as 21. Required if you are deploying at least one Lambda function written in Python and `addLayers` is true. Find the latest version number [here](https://github.com/DataDog/datadog-lambda-python/releases). |
 | `nodeLayerVersion` | `node_layer_version` | Version of the Node.js Lambda layer to install, such as 29. Required if you are deploying at least one Lambda function written in Node.js and `addLayers` is true. Find the latest version number from [here](https://github.com/DataDog/datadog-lambda-js/releases). |
+| `javaLayerVersion` | `java_layer_version` | Version of the Java layer to install, such as 8. Required if you are deploying at least one Lambda function written in Java and `addLayers` is true. Find the latest version number in the [Serverless Java installation documentation](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk). **Note**: `extensionLayerVersion >= 25` and `javaLayerVersion >= 5` are required for the Datadog construct to instrument your Java functions properly. |
 | `extensionLayerVersion` | `extension_layer_version` | Version of the Datadog Lambda Extension layer to install, such as 5. When `extensionLayerVersion` is set, `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`) needs to be set as well. When enabled, lambda function log groups will not be subscribed by the forwarder. Learn more about the Lambda extension [here](https://docs.datadoghq.com/serverless/datadog_lambda_library/extension/). |
 | `forwarderArn` | `forwarder_arn` | When set, the plugin will automatically subscribe the Datadog Forwarder to the functions' log groups. Do not set `forwarderArn` when `extensionLayerVersion` is set. |
 | `createForwarderPermissions` | `createForwarderPermissions` | When set to `true`, creates a Lambda permission on the the Datadog Forwarder per log group. Since the Datadog Forwarder has permissions configured by default, this is unnecessary in most use cases. |
 | `flushMetricsToLogs` | `flush_metrics_to_logs` | Send custom metrics using CloudWatch logs with the Datadog Forwarder Lambda function (recommended). Defaults to `true` . If you disable this parameter, it's required to set `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`). |
-| `site` | `site` | Set which Datadog site to send data. This is only used when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. Possible values are `datadoghq.com`, `datadoghq.eu`, `us3.datadoghq.com`, `us5.datadoghq.com`, and `ddog-gov.com`. The default is `datadoghq.com`. |
+| `site` | `site` | Set which Datadog site to send data. This is only used when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. Possible values are `datadoghq.com`, `datadoghq.eu`, `us3.datadoghq.com`, `us5.datadoghq.com`, `ap1.datadoghq.com`, and `ddog-gov.com`. The default is `datadoghq.com`. |
 | `apiKey` | `api_key` | Datadog API Key, only needed when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. For more information about getting a Datadog API key, see the [API key documentation](https://docs.datadoghq.com/account_management/api-app-keys/#api-keys). |
 | `apiKeySecretArn` | `api_key_secret_arn` | The ARN of the secret storing the Datadog API key in AWS Secrets Manager. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayer` is set. Remember to add the `secretsmanager:GetSecretValue` permission to the Lambda execution role. |
 | `apiKmsKey` | `api_kms_key` | Datadog API Key encrypted using KMS. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set, and you are using KMS encryption. |
 | `enableDatadogTracing` | `enable_datadog_tracing` | Enable Datadog tracing on your Lambda functions. Defaults to `true`. |
 | `enableMergeXrayTraces` | `enable_merge_xray_traces` | Enable merging X-Ray traces on your Lambda functions. Defaults to `false`. |
 | `enableDatadogLogs` | `enable_datadog_logs` | Send Lambda function logs to Datadog via the Datadog Lambda Extension.  Defaults to `true`. Note: This setting has no effect on logs sent via the Datadog Forwarder. |
 | `enableSourceCodeIntegration` | `enable_source_code_integration` | Enable Datadog Source Code Integration, connecting your telemetry with application code in your Git repositories. This requires the Datadog Github Integration to work, otherwise please follow the [alternative method](#alternative-methods-to-enable-source-code-integration). Learn more [here](https://docs.datadoghq.com/integrations/guide/source-code-integration/). Defaults to `true`. |
@@ -196,15 +198,15 @@
 | `tags` | `tags` | A comma separated list of key:value pairs as a single string. When set along with `extensionLayerVersion`, a `DD_TAGS` environment variable is added to all Lambda functions with the provided value. When set along with `forwarderArn`, the cdk parses the string and sets each key:value pair as a tag to all Lambda functions. |
 | `enableColdStartTracing`      | `enable_cold_start_tracing` | Set to `false` to disable Cold Start Tracing. Used in NodeJS and Python. Defaults to `true`. |
 | `coldStartTraceMinDuration`   | `min_cold_start_trace_duration` | Sets the minimum duration (in milliseconds) for a module load event to be traced via Cold Start Tracing. Number. Defaults to `3`. |
 | `coldStartTraceSkipLibs`      | `cold_start_trace_skip_libs`| Optionally skip creating Cold Start Spans for a comma-separated list of libraries. Useful to limit depth or skip known libraries. Default depends on runtime. |
 | `enableProfiling`             | `enable_profiling` | Enable the Datadog Continuous Profiler with `true`. Supported in Beta for NodeJS and Python. Defaults to `false`. |
 | `encodeAuthorizerContext`     |`encode_authorizer_context` | When set to `true` for Lambda authorizers, the tracing context will be encoded into the response for propagation. Supported for NodeJS and Python. Defaults to `true`. |
 | `decodeAuthorizerContext`     |`decode_authorizer_context` | When set to `true` for Lambdas that are authorized via Lambda authorizers, it will parse and use the encoded tracing context (if found). Supported for NodeJS and Python. Defaults to `true`.                         |
-| `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set. The tracer will attempt to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
+| `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set, the tracer attempts to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
 
 **Note**: Using the parameters above may override corresponding function level `DD_XXX` environment variables.
 
 ### Tracing
 
 Enable X-Ray Tracing on your Lambda functions. For more information, see [CDK documentation](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-lambda.Tracing.html).
 
@@ -234,14 +236,15 @@
     def __init__(self, scope, id, props=None):
         super().__init__(scope, id, props)
         NestedStack(self, "NestedStack")
 
         datadog = Datadog(self, "Datadog",
             node_layer_version=<LAYER_VERSION>,
             python_layer_version=<LAYER_VERSION>,
+            java_layer_version=<LAYER_VERSION>,
             add_layers=<BOOLEAN>,
             forwarder_arn="<FORWARDER_ARN>",
             flush_metrics_to_logs=<BOOLEAN>,
             site="<SITE>",
             api_key="{Datadog_API_Key}",
             api_key_secret_arn="{Secret_ARN_Datadog_API_Key}",
             api_kms_key="{Encrypted_Datadog_API_Key}",
@@ -255,14 +258,15 @@
 class NestedStack(cdk.NestedStack):
     def __init__(self, scope, id, props=None):
         super().__init__(scope, id, props)
 
         datadog = Datadog(self, "Datadog",
             node_layer_version=<LAYER_VERSION>,
             python_layer_version=<LAYER_VERSION>,
+            java_layer_version=<LAYER_VERSION>,
             add_layers=<BOOLEAN>,
             forwarder_arn="<FORWARDER_ARN>",
             flush_metrics_to_logs=<BOOLEAN>,
             site="<SITE>",
             api_key="{Datadog_API_Key}",
             api_key_secret_arn="{Secret_ARN_Datadog_API_Key}",
             api_kms_key="{Encrypted_Datadog_API_Key}",
@@ -276,15 +280,15 @@
 
 ### Tags
 
 Add tags to your constructs. We recommend setting an `env` and `service` tag to tie Datadog telemetry together. For more information see [official AWS documentation](https://docs.aws.amazon.com/cdk/latest/guide/tagging.html) and [CDK documentation](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.Tags.html).
 
 ## How it works
 
-The Datadog CDK construct takes in a list of lambda functions and installs the Datadog Lambda Library by attaching the Lambda Layers for [Node.js](https://github.com/DataDog/datadog-lambda-layer-js) and [Python](https://github.com/DataDog/datadog-lambda-layer-python) to your functions. It redirects to a replacement handler that initializes the Lambda Library without any required code changes. Additional configurations added to the Datadog CDK construct will also translate into their respective environment variables under each lambda function (if applicable / required).
+The Datadog CDK construct takes in a list of lambda functions and installs the Datadog Lambda Library by attaching the Lambda Layers for [Java](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk), [Node.js](https://github.com/DataDog/datadog-lambda-layer-js), and [Python](https://github.com/DataDog/datadog-lambda-layer-python) to your functions. It redirects to a replacement handler that initializes the Lambda Library without any required code changes. Additional configurations added to the Datadog CDK construct will also translate into their respective environment variables under each lambda function (if applicable / required).
 
 While Lambda function based log groups are handled by the `addLambdaFunctions` method automatically, the construct has an additional function `addForwarderToNonLambdaLogGroups` which subscribes the forwarder to any additional log groups of your choosing.
 
 ## Resources to learn about CDK
 
 * [CDK TypeScript Workshop](https://cdkworkshop.com/20-typescript.html)
 * [Video Introducing CDK by AWS with Demo](https://youtu.be/ZWCvNFUN-sU)
```

### Comparing `datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs/_jsii/__init__.py` & `datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 import aws_cdk.aws_logs._jsii
 import aws_cdk.aws_logs_destinations._jsii
 import aws_cdk.core._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "datadog-cdk-constructs",
-    "0.8.6",
+    "0.9.0",
     __name__[0:-6],
-    "datadog-cdk-constructs@0.8.6.jsii.tgz",
+    "datadog-cdk-constructs@0.9.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `datadog-cdk-constructs-0.8.6/src/datadog_cdk_constructs.egg-info/PKG-INFO` & `datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-cdk-constructs
-Version: 0.8.6
+Version: 0.9.0
 Summary: CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog
 Home-page: https://github.com/DataDog/datadog-cdk-constructs
 Author: Datadog
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataDog/datadog-cdk-constructs
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -30,15 +30,15 @@
 [![PyPI](https://img.shields.io/pypi/v/datadog-cdk-constructs-v2?color=39a356&label=pypi+cdk+v2)](https://pypi.org/project/datadog-cdk-constructs-v2/)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-cdk-constructs/blob/main/LICENSE)
 
 Use this Datadog CDK Construct Library to deploy serverless applications using AWS CDK .
 
 This CDK library automatically configures ingestion of metrics, traces, and logs from your serverless applications by:
 
-* Installing and configuring the Datadog Lambda library for your [Python](https://github.com/DataDog/datadog-lambda-layer-python) and [Node.js](https://github.com/DataDog/datadog-lambda-layer-js) Lambda functions.
+* Installing and configuring the Datadog Lambda layers for your [Python](https://github.com/DataDog/datadog-lambda-layer-python), [Node.js](https://github.com/DataDog/datadog-lambda-layer-js), and [Java](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk) Lambda functions.
 * Enabling the collection of traces and custom metrics from your Lambda functions.
 * Managing subscriptions from the Datadog Forwarder to your Lambda and non-Lambda log groups.
 
 ## AWS CDK v1 vs AWS CDK v2
 
 Two separate versions of Datadog CDK Constructs exist; `datadog-cdk-constructs` and `datadog-cdk-constructs-v2`. These are designed to work with `AWS CDK v1` and `AWS CDK v2` respectively.
 
@@ -93,14 +93,15 @@
 ```python
 # Example automatically generated from non-compiling source. May contain errors.
 from datadog_cdk_constructs_v2 import Datadog
 
 datadog = Datadog(self, "Datadog",
     node_layer_version=<LAYER_VERSION>,
     python_layer_version=<LAYER_VERSION>,
+    java_layer_version=<LAYER_VERSION>,
     add_layers=<BOOLEAN>,
     extension_layer_version="<EXTENSION_VERSION>",
     forwarder_arn="<FORWARDER_ARN>",
     create_forwarder_permissions=<BOOLEAN>,
     flush_metrics_to_logs=<BOOLEAN>,
     site="<SITE>",
     api_key="{Datadog_API_Key}",
@@ -195,19 +196,20 @@
 *Note*: The descriptions use the npm package parameters, but they also apply to the PyPI package parameters.
 
 | npm package parameter | PyPI package parameter | Description |
 | --- | --- | --- |
 | `addLayers` | `add_layers` | Whether to add the Lambda Layers or expect the user to bring their own. Defaults to true. When true, the Lambda Library version variables are also required. When false, you must include the Datadog Lambda library in your functions' deployment packages. |
 | `pythonLayerVersion` | `python_layer_version` | Version of the Python Lambda layer to install, such as 21. Required if you are deploying at least one Lambda function written in Python and `addLayers` is true. Find the latest version number [here](https://github.com/DataDog/datadog-lambda-python/releases). |
 | `nodeLayerVersion` | `node_layer_version` | Version of the Node.js Lambda layer to install, such as 29. Required if you are deploying at least one Lambda function written in Node.js and `addLayers` is true. Find the latest version number from [here](https://github.com/DataDog/datadog-lambda-js/releases). |
+| `javaLayerVersion` | `java_layer_version` | Version of the Java layer to install, such as 8. Required if you are deploying at least one Lambda function written in Java and `addLayers` is true. Find the latest version number in the [Serverless Java installation documentation](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk). **Note**: `extensionLayerVersion >= 25` and `javaLayerVersion >= 5` are required for the Datadog construct to instrument your Java functions properly. |
 | `extensionLayerVersion` | `extension_layer_version` | Version of the Datadog Lambda Extension layer to install, such as 5. When `extensionLayerVersion` is set, `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`) needs to be set as well. When enabled, lambda function log groups will not be subscribed by the forwarder. Learn more about the Lambda extension [here](https://docs.datadoghq.com/serverless/datadog_lambda_library/extension/). |
 | `forwarderArn` | `forwarder_arn` | When set, the plugin will automatically subscribe the Datadog Forwarder to the functions' log groups. Do not set `forwarderArn` when `extensionLayerVersion` is set. |
 | `createForwarderPermissions` | `createForwarderPermissions` | When set to `true`, creates a Lambda permission on the the Datadog Forwarder per log group. Since the Datadog Forwarder has permissions configured by default, this is unnecessary in most use cases. |
 | `flushMetricsToLogs` | `flush_metrics_to_logs` | Send custom metrics using CloudWatch logs with the Datadog Forwarder Lambda function (recommended). Defaults to `true` . If you disable this parameter, it's required to set `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`). |
-| `site` | `site` | Set which Datadog site to send data. This is only used when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. Possible values are `datadoghq.com`, `datadoghq.eu`, `us3.datadoghq.com`, `us5.datadoghq.com`, and `ddog-gov.com`. The default is `datadoghq.com`. |
+| `site` | `site` | Set which Datadog site to send data. This is only used when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. Possible values are `datadoghq.com`, `datadoghq.eu`, `us3.datadoghq.com`, `us5.datadoghq.com`, `ap1.datadoghq.com`, and `ddog-gov.com`. The default is `datadoghq.com`. |
 | `apiKey` | `api_key` | Datadog API Key, only needed when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. For more information about getting a Datadog API key, see the [API key documentation](https://docs.datadoghq.com/account_management/api-app-keys/#api-keys). |
 | `apiKeySecretArn` | `api_key_secret_arn` | The ARN of the secret storing the Datadog API key in AWS Secrets Manager. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayer` is set. Remember to add the `secretsmanager:GetSecretValue` permission to the Lambda execution role. |
 | `apiKmsKey` | `api_kms_key` | Datadog API Key encrypted using KMS. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set, and you are using KMS encryption. |
 | `enableDatadogTracing` | `enable_datadog_tracing` | Enable Datadog tracing on your Lambda functions. Defaults to `true`. |
 | `enableMergeXrayTraces` | `enable_merge_xray_traces` | Enable merging X-Ray traces on your Lambda functions. Defaults to `false`. |
 | `enableDatadogLogs` | `enable_datadog_logs` | Send Lambda function logs to Datadog via the Datadog Lambda Extension.  Defaults to `true`. Note: This setting has no effect on logs sent via the Datadog Forwarder. |
 | `enableSourceCodeIntegration` | `enable_source_code_integration` | Enable Datadog Source Code Integration, connecting your telemetry with application code in your Git repositories. This requires the Datadog Github Integration to work, otherwise please follow the [alternative method](#alternative-methods-to-enable-source-code-integration). Learn more [here](https://docs.datadoghq.com/integrations/guide/source-code-integration/). Defaults to `true`. |
@@ -219,15 +221,15 @@
 | `tags` | `tags` | A comma separated list of key:value pairs as a single string. When set along with `extensionLayerVersion`, a `DD_TAGS` environment variable is added to all Lambda functions with the provided value. When set along with `forwarderArn`, the cdk parses the string and sets each key:value pair as a tag to all Lambda functions. |
 | `enableColdStartTracing`      | `enable_cold_start_tracing` | Set to `false` to disable Cold Start Tracing. Used in NodeJS and Python. Defaults to `true`. |
 | `coldStartTraceMinDuration`   | `min_cold_start_trace_duration` | Sets the minimum duration (in milliseconds) for a module load event to be traced via Cold Start Tracing. Number. Defaults to `3`. |
 | `coldStartTraceSkipLibs`      | `cold_start_trace_skip_libs`| Optionally skip creating Cold Start Spans for a comma-separated list of libraries. Useful to limit depth or skip known libraries. Default depends on runtime. |
 | `enableProfiling`             | `enable_profiling` | Enable the Datadog Continuous Profiler with `true`. Supported in Beta for NodeJS and Python. Defaults to `false`. |
 | `encodeAuthorizerContext`     |`encode_authorizer_context` | When set to `true` for Lambda authorizers, the tracing context will be encoded into the response for propagation. Supported for NodeJS and Python. Defaults to `true`. |
 | `decodeAuthorizerContext`     |`decode_authorizer_context` | When set to `true` for Lambdas that are authorized via Lambda authorizers, it will parse and use the encoded tracing context (if found). Supported for NodeJS and Python. Defaults to `true`.                         |
-| `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set. The tracer will attempt to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
+| `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set, the tracer attempts to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
 
 **Note**: Using the parameters above may override corresponding function level `DD_XXX` environment variables.
 
 ### Tracing
 
 Enable X-Ray Tracing on your Lambda functions. For more information, see [CDK documentation](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-lambda.Tracing.html).
 
@@ -257,14 +259,15 @@
     def __init__(self, scope, id, props=None):
         super().__init__(scope, id, props)
         NestedStack(self, "NestedStack")
 
         datadog = Datadog(self, "Datadog",
             node_layer_version=<LAYER_VERSION>,
             python_layer_version=<LAYER_VERSION>,
+            java_layer_version=<LAYER_VERSION>,
             add_layers=<BOOLEAN>,
             forwarder_arn="<FORWARDER_ARN>",
             flush_metrics_to_logs=<BOOLEAN>,
             site="<SITE>",
             api_key="{Datadog_API_Key}",
             api_key_secret_arn="{Secret_ARN_Datadog_API_Key}",
             api_kms_key="{Encrypted_Datadog_API_Key}",
@@ -278,14 +281,15 @@
 class NestedStack(cdk.NestedStack):
     def __init__(self, scope, id, props=None):
         super().__init__(scope, id, props)
 
         datadog = Datadog(self, "Datadog",
             node_layer_version=<LAYER_VERSION>,
             python_layer_version=<LAYER_VERSION>,
+            java_layer_version=<LAYER_VERSION>,
             add_layers=<BOOLEAN>,
             forwarder_arn="<FORWARDER_ARN>",
             flush_metrics_to_logs=<BOOLEAN>,
             site="<SITE>",
             api_key="{Datadog_API_Key}",
             api_key_secret_arn="{Secret_ARN_Datadog_API_Key}",
             api_kms_key="{Encrypted_Datadog_API_Key}",
@@ -299,15 +303,15 @@
 
 ### Tags
 
 Add tags to your constructs. We recommend setting an `env` and `service` tag to tie Datadog telemetry together. For more information see [official AWS documentation](https://docs.aws.amazon.com/cdk/latest/guide/tagging.html) and [CDK documentation](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.Tags.html).
 
 ## How it works
 
-The Datadog CDK construct takes in a list of lambda functions and installs the Datadog Lambda Library by attaching the Lambda Layers for [Node.js](https://github.com/DataDog/datadog-lambda-layer-js) and [Python](https://github.com/DataDog/datadog-lambda-layer-python) to your functions. It redirects to a replacement handler that initializes the Lambda Library without any required code changes. Additional configurations added to the Datadog CDK construct will also translate into their respective environment variables under each lambda function (if applicable / required).
+The Datadog CDK construct takes in a list of lambda functions and installs the Datadog Lambda Library by attaching the Lambda Layers for [Java](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk), [Node.js](https://github.com/DataDog/datadog-lambda-layer-js), and [Python](https://github.com/DataDog/datadog-lambda-layer-python) to your functions. It redirects to a replacement handler that initializes the Lambda Library without any required code changes. Additional configurations added to the Datadog CDK construct will also translate into their respective environment variables under each lambda function (if applicable / required).
 
 While Lambda function based log groups are handled by the `addLambdaFunctions` method automatically, the construct has an additional function `addForwarderToNonLambdaLogGroups` which subscribes the forwarder to any additional log groups of your choosing.
 
 ## Resources to learn about CDK
 
 * [CDK TypeScript Workshop](https://cdkworkshop.com/20-typescript.html)
 * [Video Introducing CDK by AWS with Demo](https://youtu.be/ZWCvNFUN-sU)
```

