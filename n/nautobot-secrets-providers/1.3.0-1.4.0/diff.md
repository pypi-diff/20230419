# Comparing `tmp/nautobot-secrets-providers-1.3.0.tar.gz` & `tmp/nautobot_secrets_providers-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot-secrets-providers-1.3.0.tar", max compression
+gzip compressed data, was "nautobot_secrets_providers-1.4.0.tar", max compression
```

## Comparing `nautobot-secrets-providers-1.3.0.tar` & `nautobot_secrets_providers-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      591 2022-08-30 18:25:51.045344 nautobot-secrets-providers-1.3.0/LICENSE
--rw-r--r--   0        0        0    28147 2022-08-30 18:25:51.045344 nautobot-secrets-providers-1.3.0/README.md
--rw-r--r--   0        0        0     1041 2022-08-30 18:25:51.049344 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/__init__.py
--rw-r--r--   0        0        0        0 2022-08-30 18:25:51.049344 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/migrations/__init__.py
--rw-r--r--   0        0        0      582 2022-08-30 18:25:51.049344 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/providers/__init__.py
--rw-r--r--   0        0        0     4656 2022-08-30 18:25:51.049344 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/providers/aws.py
--rw-r--r--   0        0        0      509 2022-08-30 18:25:51.049344 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/providers/choices.py
--rw-r--r--   0        0        0     9512 2022-08-30 18:25:51.049344 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/providers/delinea.py
--rw-r--r--   0        0        0     7667 2022-08-30 18:25:51.049344 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/providers/hashicorp.py
--rw-r--r--   0        0        0      758 2022-08-30 18:25:51.049344 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/secrets.py
--rw-r--r--   0        0        0     2745 2022-08-30 18:25:51.049344 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/templates/nautobot_secrets_providers/home.html
--rw-r--r--   0        0        0       56 2022-08-30 18:25:51.049344 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/tests/__init__.py
--rw-r--r--   0        0        0     2086 2022-08-30 18:25:51.049344 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/tests/nautobot_config.py
--rw-r--r--   0        0        0      621 2022-08-30 18:25:51.049344 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/tests/test_basic.py
--rw-r--r--   0        0        0    19880 2022-08-30 18:25:51.049344 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/tests/test_providers.py
--rw-r--r--   0        0        0      281 2022-08-30 18:25:51.049344 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/urls.py
--rw-r--r--   0        0        0      534 2022-08-30 18:25:51.053345 nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/views.py
--rw-r--r--   0        0        0     3087 2022-08-30 18:26:00.817629 nautobot-secrets-providers-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    30024 2022-08-30 18:26:02.159233 nautobot-secrets-providers-1.3.0/setup.py
--rw-r--r--   0        0        0    29347 2022-08-30 18:26:02.161625 nautobot-secrets-providers-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-04-19 20:54:25.659742 nautobot_secrets_providers-1.4.0/LICENSE
+-rw-r--r--   0        0        0    28981 2023-04-19 20:54:25.659742 nautobot_secrets_providers-1.4.0/README.md
+-rw-r--r--   0        0        0     1194 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/migrations/__init__.py
+-rw-r--r--   0        0        0      690 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/__init__.py
+-rw-r--r--   0        0        0     7245 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/aws.py
+-rw-r--r--   0        0        0      800 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/choices.py
+-rw-r--r--   0        0        0     9512 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/delinea.py
+-rw-r--r--   0        0        0     9120 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/hashicorp.py
+-rw-r--r--   0        0        0      758 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/secrets.py
+-rw-r--r--   0        0        0     3452 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/templates/nautobot_secrets_providers/home.html
+-rw-r--r--   0        0        0       56 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/tests/__init__.py
+-rw-r--r--   0        0        0     2086 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/tests/nautobot_config.py
+-rw-r--r--   0        0        0      621 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/tests/test_basic.py
+-rw-r--r--   0        0        0    26973 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/tests/test_providers.py
+-rw-r--r--   0        0        0      281 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/urls.py
+-rw-r--r--   0        0        0      534 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/views.py
+-rw-r--r--   0        0        0     3105 2023-04-19 20:54:35.383724 nautobot_secrets_providers-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    30235 1970-01-01 00:00:00.000000 nautobot_secrets_providers-1.4.0/PKG-INFO
```

### Comparing `nautobot-secrets-providers-1.3.0/LICENSE` & `nautobot_secrets_providers-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot-secrets-providers-1.3.0/README.md` & `nautobot_secrets_providers-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 ## Supported Secrets Backends
 
 This plugin supports the following popular secrets backends:
 
 | Secrets Backend                                              | Supported Secret Types                                       | Supported Authentication Methods                             |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
 | [AWS Secrets Manager](https://aws.amazon.com/secrets-manager/) | [Other: Key/value pairs](https://docs.aws.amazon.com/secretsmanager/latest/userguide/manage_create-basic-secret.html) | [AWS credentials](https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html) (see Usage section below) |
-| [HashiCorp Vault](https://www.vaultproject.io)               | [K/V Version 2](https://www.vaultproject.io/docs/secrets/kv/kv-v2) | [Token](https://www.vaultproject.io/docs/auth/token)<br/>[AppRole](https://www.vaultproject.io/docs/auth/approle)<br/>[AWS](https://www.vaultproject.io/docs/auth/aws)<br/>[Kubernetes](https://www.vaultproject.io/docs/auth/kubernetes)         |
+| [AWS Systems Manager Parameter Store](https://aws.amazon.com/secrets-manager/) | [Other: Key/value pairs](https://docs.aws.amazon.com/systems-manager/latest/userguide/systems-manager-parameter-store.html) | [AWS credentials](https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html) (see Usage section below) |
+| [HashiCorp Vault](https://www.vaultproject.io)               | [K/V Version 2](https://www.vaultproject.io/docs/secrets/kv/kv-v2)<br/>[K/V Version 1](https://developer.hashicorp.com/vault/docs/secrets/kv/kv-v1) | [Token](https://www.vaultproject.io/docs/auth/token)<br/>[AppRole](https://www.vaultproject.io/docs/auth/approle)<br/>[AWS](https://www.vaultproject.io/docs/auth/aws)<br/>[Kubernetes](https://www.vaultproject.io/docs/auth/kubernetes)         |
 | [Delinea/Thycotic Secret Server](https://delinea.com/products/secret-server)               | [Secret Server Cloud](https://github.com/DelineaXPM/python-tss-sdk#secret-server-cloud)<br/>[Secret Server (on-prem)](https://github.com/DelineaXPM/python-tss-sdk#initializing-secretserver)| [Access Token Authorization](https://github.com/DelineaXPM/python-tss-sdk#access-token-authorization)<br/>[Domain Authorization](https://github.com/DelineaXPM/python-tss-sdk#domain-authorization)<br/>[Password Authorization](https://github.com/DelineaXPM/python-tss-sdk#password-authorization)<br/>         |
 
 ## Screenshots
 
 ![Screenshot of installed plugins](https://raw.githubusercontent.com/nautobot/nautobot-plugin-secrets-providers/develop/docs/images/screenshot01.png "Plugin landing page")
 
 ---
@@ -36,15 +37,15 @@
 
 ---
 
 ![Screenshot of secret using Delinea/Thycotic Secret Server by Path](https://raw.githubusercontent.com/nautobot/nautobot-plugin-secrets-providers/develop/docs/images/screenshot06.png "Secret using Thycotic Secret Server by Path")
 
 ## Installation
 
-> Nautobot Secrets Providers is compatible with Nautobot 1.2.0 and higher. Support for Thycotic Secret Server requires Python 3.7 or later.
+> Nautobot Secrets Providers is compatible with Nautobot 1.4.0 and higher. Support for Thycotic Secret Server requires Python 3.7 or later.
 
 The package is available as a Python package in PyPI and can be installed with `pip`:
 
 ```no-highlight
 pip install nautobot-secrets-providers
 ```
 
@@ -56,17 +57,17 @@
 
 ### Dependencies
 
 For this plugin to operate you must install at least one of the dependent libraries required by the secrets providers.
 
 **You must install the dependencies for at least one of the supported secrets providers or a `RuntimeError` will be raised.**
 
-#### AWS Secrets Manager
+#### AWS
 
-The AWS Secrets Manager provider requires the `boto3` library. This can be easily installed along with the plugin using the following command:
+AWS Secrets Manager and Systems Manager Parameter Store are supported. Both providers require the `boto3` library. This can be easily installed along with the plugin using the following command:
 
 ```no-highlight
 pip install nautobot-secrets-providers[aws]
 ```
 
 #### HashiCorp Vault
 
@@ -107,15 +108,15 @@
 
 ## Usage
 
 Before you proceed, you must have **at least one** of the dependent libaries installed as detailed above.
 
 Please do not enable this plugin until you are able to install the dependencies, as it will block Nautobot from starting.
 
-### AWS Secrets Manager
+### AWS
 
 #### Authentication
 
 No configuration is needed within Nautobot for this provider to operate. Instead you must provide [AWS credentials in one of the methods supported by the `boto3` library](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html#configuring-credentials).
 
 Boto3 credentials can be configured in multiple ways (eight as of this writing) that are mirrored here:
 
@@ -124,15 +125,15 @@
 3. Environment variables
 4. Shared credential file (`~/.aws/credentials`)
 5. AWS config file (`~/.aws/config`)
 6. Assume Role provider
 7. Boto2 config file (`/etc/boto.cfg` and `~/.boto`)
 8. Instance metadata service on an Amazon EC2 instance that has an IAM role configured.
 
-**The AWS Secrets Manager provider only supports methods 3-8. Methods 1 and 2 ARE NOT SUPPORTED at this time.**
+**The AWS providers only support methods 3-8. Methods 1 and 2 ARE NOT SUPPORTED at this time.**
 
 We highly recommend you defer to using environment variables for your deployment as specified in the credentials documentation linked above. The values specified in the linked documentation should be [set within your `~.bashrc`](https://nautobot.readthedocs.io/en/latest/installation/nautobot/#update-the-nautobot-bashrc) (or similar profile) on your system.
 
 #### Configuration
 
 This is an example based on our recommended deployment pattern in the section above (item 3) that is using [environment variables](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html#environment-variables). You will need to set these in the environment prior to starting Nautobot:
 
@@ -161,21 +162,23 @@
 }
 ```
 
 - `url` - (required) The URL to the HashiCorp Vault instance (e.g. `http://localhost:8200`).
 - `auth_method` - (optional / defaults to "token") The method used to authenticate against the HashiCorp Vault instance. Either `"approle"`, `"aws"`, `"kubernetes"` or `"token"`.  For information on using AWS authentication with vault see the [authentication](#authentication) section above.
 - `ca_cert` - (optional) Path to a PEM formatted CA certificate to use when verifying the Vault connection.  Can alternatively be set to `False` to ignore SSL verification (not recommended) or `True` to use the system certificates.
 - `default_mount_point` - (optional / defaults to "secret") The default mount point of the K/V Version 2 secrets engine within Hashicorp Vault.
+- `kv_version` - (optional / defaults to "v2") The version of the KV engine to use, can be `v1` or `v2`
 - `k8s_token_path` - (optional) Path to the kubernetes service account token file.  Defaults to "/var/run/secrets/kubernetes.io/serviceaccount/token".
 - `token` - (optional) Required when `"auth_method": "token"` or `auth_method` is not supplied. The token for authenticating the client with the HashiCorp Vault instance. As with other sensitive service credentials, we recommend that you provide the token value as an environment variable and retrieve it with `{"token": os.getenv("NAUTOBOT_HASHICORP_VAULT_TOKEN")}` rather than hard-coding it in your `nautobot_config.py`.
 - `role_name` - (optional) Required when `"auth_method": "kubernetes"`, optional when `"auth_method": "aws"`.  The Vault Kubernetes role or Vault AWS role to assume which the pod's service account has access to.
 - `role_id` - (optional) Required when `"auth_method": "approle"`. As with other sensitive service credentials, we recommend that you provide the role_id value as an environment variable and retrieve it with `{"role_id": os.getenv("NAUTOBOT_HASHICORP_VAULT_ROLE_ID")}` rather than hard-coding it in your `nautobot_config.py`.
 - `secret_id` - (optional) Required when `"auth_method": "approle"`.As with other sensitive service credentials, we recommend that you provide the secret_id value as an environment variable and retrieve it with `{"secret_id": os.getenv("NAUTOBOT_HASHICORP_VAULT_SECRET_ID")}` rather than hard-coding it in your `nautobot_config.py`.
 - `login_kwargs` - (optional) Additional optional parameters to pass to the login method for [`approle`](https://hvac.readthedocs.io/en/stable/source/hvac_api_auth_methods.html#hvac.api.auth_methods.AppRole.login), [`aws`](https://hvac.readthedocs.io/en/stable/source/hvac_api_auth_methods.html#hvac.api.auth_methods.Aws.iam_login) and [`kubernetes`](https://hvac.readthedocs.io/en/stable/source/hvac_api_auth_methods.html#hvac.api.auth_methods.Kubernetes.login) authentication methods.
-
+- `namespace` - (optional) Namespace to use for the [`X-Vault-Namespace` header](https://github.com/hvac/hvac/blob/main/hvac/adapters.py#L287) on all hvac client requests. Required when the [`Namespaces`](https://developer.hashicorp.com/vault/docs/enterprise/namespaces#usage) feature is enabled in Vault Enterprise.
+ 
 ### Delinea/Thycotic Secret Server (TSS)
 
 The Delinea/Thycotic Secret Server plugin includes two providers:
 
 - **`Thycotic Secret Server by ID`**
 
     This provider uses the `Secret ID` to specifiy the secret that is selected. The `Secret ID` is displayed in the browser's URL field if you `Edit` the data in Thycotic Secret Server.
@@ -242,15 +245,15 @@
 
 Below is a quick start guide if you're already familiar with the development environment provided, but if you're not familiar, please read the [Getting Started Guide](GETTING_STARTED.md).
 
 #### Invoke
 
 The [PyInvoke](http://www.pyinvoke.org/) library is used to provide some helper commands based on the environment.  There are a few configuration parameters which can be passed to PyInvoke to override the default configuration:
 
-* `nautobot_ver`: the version of Nautobot to use as a base for any built docker containers (default: 1.2.0)
+* `nautobot_ver`: the version of Nautobot to use as a base for any built docker containers (default: 1.4.10)
 * `project_name`: the default docker compose project name (default: nautobot_secrets_providers)
 * `python_ver`: the version of Python to use as a base for any built docker containers (default: 3.7)
 * `local`: a boolean flag indicating if invoke tasks should be run on the host or inside the docker containers (default: False, commands will be run in docker containers)
 * `compose_dir`: the full path to a directory containing the project compose files
 * `compose_files`: a list of compose files applied in order (see [Multiple Compose files](https://docs.docker.com/compose/extends/#multiple-compose-files) for more information)
 
 Using **PyInvoke** these configuration options can be overridden using [several methods](http://docs.pyinvoke.org/en/stable/concepts/configuration.html).  Perhaps the simplest is simply setting an environment variable `INVOKE_NAUTOBOT_SECRETS_PROVIDERS_VARIABLE_NAME` where `VARIABLE_NAME` is the variable you are trying to override.  The only exception is `compose_files`, because it is a list it must be overridden in a yaml file.  There is an example `invoke.yml` (`invoke.example.yml`) in this directory which can be used as a starting point.
```

### Comparing `nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/__init__.py` & `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 from nautobot.extras.plugins import PluginConfig
 
 
 class NautobotSecretsProvidersConfig(PluginConfig):
     """Plugin configuration for the nautobot_secrets_providers plugin."""
 
     name = "nautobot_secrets_providers"
-    verbose_name = "Nautobot Secrets Providers"
+    verbose_name = "Secrets Management Extensions"
     version = __version__
     author = "Network to Code, LLC"
-    description = "Nautobot Secrets Providers Plugin."
+    description = "Nautobot App that provides direct integrations with Enterprise secrets management systems. Provides patterns to securely fetch secrets for use by other Nautobot Apps and Nautobot Jobs."
     base_url = "secrets"
     required_settings = []
-    min_version = "1.2.0"
+    min_version = "1.4.0"
     max_version = "1.9999"
     default_settings = {}
     caching_config = {}
 
     # URL reverse lookup names
     home_view_name = "plugins:nautobot_secrets_providers:home"
```

### Comparing `nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/providers/__init__.py` & `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Nautobot Secrets Providers."""
 
-from .aws import AWSSecretsManagerSecretsProvider
+from .aws import AWSSecretsManagerSecretsProvider, AWSSystemsManagerParameterStore
 from .hashicorp import HashiCorpVaultSecretsProvider
 from .delinea import ThycoticSecretServerSecretsProviderId, ThycoticSecretServerSecretsProviderPath
 
 __all__ = (  # type: ignore
     AWSSecretsManagerSecretsProvider,  # pylint: disable=invalid-all-object
+    AWSSystemsManagerParameterStore,  # pylint: disable=invalid-all-object
     HashiCorpVaultSecretsProvider,  # pylint: disable=invalid-all-object
     ThycoticSecretServerSecretsProviderId,  # pylint: disable=invalid-all-object
     ThycoticSecretServerSecretsProviderPath,  # pylint: disable=invalid-all-object
 )
```

### Comparing `nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/providers/aws.py` & `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/aws.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Secrets Provider for AWS Secrets Manager."""
+"""Secrets Provider for AWS Secrets Manager and Parameter Store."""
 
 import base64
 import json
 
 try:
     import boto3
     from botocore.exceptions import ClientError
@@ -11,15 +11,15 @@
 
 from django import forms
 
 from nautobot.utilities.forms import BootstrapMixin
 from nautobot.extras.secrets import exceptions, SecretsProvider
 
 
-__all__ = ("AWSSecretsManagerSecretsProvider",)
+__all__ = ("AWSSecretsManagerSecretsProvider", "AWSSystemsManagerParameterStore")
 
 
 class AWSSecretsManagerSecretsProvider(SecretsProvider):
     """A secrets provider for AWS Secrets Manager."""
 
     slug = "aws-secrets-manager"
     name = "AWS Secrets Manager"
@@ -95,7 +95,68 @@
 
         # Retrieve the value using the key or complain loudly.
         try:
             return data[secret_key]
         except KeyError as err:
             msg = f"The secret value could not be retrieved using key {err}"
             raise exceptions.SecretValueNotFoundError(secret, cls, msg) from err
+
+
+class AWSSystemsManagerParameterStore(SecretsProvider):
+    """
+    A secrets provider for AWS Systems Manager Parameter Store.
+
+    Documentation: https://docs.aws.amazon.com/systems-manager/latest/userguide/systems-manager-parameter-store.html
+    """
+
+    slug = "aws-sm-parameter-store"
+    name = "AWS Systems Manager Parameter Store"
+    is_available = boto3 is not None
+
+    class ParametersForm(BootstrapMixin, forms.Form):
+        """Required parameters for AWS Parameter Store."""
+
+        name = forms.CharField(
+            required=True,
+            help_text="The name of the AWS Parameter Store secret",
+        )
+        region = forms.CharField(
+            required=True,
+            help_text="The region name of the AWS Parameter Store secret",
+        )
+        key = forms.CharField(
+            required=True,
+            help_text="The key name to retrieve from AWS Parameter Store",
+        )
+
+    @classmethod
+    def get_value_for_secret(cls, secret, obj=None, **kwargs):
+        """Return the parameter value by name and region."""
+        # Extract the parameters from the Nautobot secret.
+        parameters = secret.rendered_parameters(obj=obj)
+
+        # Create a SSM client.
+        session = boto3.session.Session()
+        client = session.client(service_name="ssm", region_name=parameters.get("region"))
+        try:
+            get_secret_value_response = client.get_parameter(Name=parameters.get("name"), WithDecryption=True)
+        except ClientError as err:
+            if err.response["Error"]["Code"] == "ParameterNotFound":
+                raise exceptions.SecretParametersError(secret, cls, str(err))
+
+            if err.response["Error"]["Code"] == "ParameterVersionNotFound":
+                raise exceptions.SecretValueNotFoundError(secret, cls, str(err))
+
+            raise exceptions.SecretProviderError(secret, cls, str(err))
+        else:
+            try:
+                # Fetch the Value field from the parameter which must be a json field.
+                data = json.loads(get_secret_value_response["Parameter"]["Value"])
+            except ValueError as err:
+                msg = "InvalidJson"
+                raise exceptions.SecretValueNotFoundError(secret, cls, msg) from err
+        try:
+            # Return the value of the secret key configured in the nautobot secret.
+            return data[parameters.get("key")]
+        except KeyError as err:
+            msg = f"InvalidKeyName {err}"
+            raise exceptions.SecretParametersError(secret, cls, msg) from err
```

### Comparing `nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/providers/delinea.py` & `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/delinea.py`

 * *Files identical despite different names*

### Comparing `nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/providers/hashicorp.py` & `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/hashicorp.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,27 +12,36 @@
     import hvac
 except ImportError:
     hvac = None
 
 from nautobot.utilities.forms import BootstrapMixin
 from nautobot.extras.secrets import exceptions, SecretsProvider
 
+from .choices import HashicorpKVVersionChoices
+
 __all__ = ("HashiCorpVaultSecretsProvider",)
 
 K8S_TOKEN_DEFAULT_PATH = "/var/run/secrets/kubernetes.io/serviceaccount/token"  # nosec B105
 AUTH_METHOD_CHOICES = ["approle", "aws", "kubernetes", "token"]
 
 
 # Default mount point for the HVAC client
 try:
     plugins_config = settings.PLUGINS_CONFIG["nautobot_secrets_providers"]
     DEFAULT_MOUNT_POINT = plugins_config["hashicorp_vault"]["default_mount_point"]
 except KeyError:
     DEFAULT_MOUNT_POINT = "secret"
 
+# Default kv version for the HVAC client
+try:
+    plugins_config = settings.PLUGINS_CONFIG["nautobot_secrets_providers"]
+    DEFAULT_KV_VERSION = plugins_config["hashicorp_vault"]["default_kv_version"]
+except KeyError:
+    DEFAULT_KV_VERSION = HashicorpKVVersionChoices.KV_VERSION_2
+
 
 class HashiCorpVaultSecretsProvider(SecretsProvider):
     """A secrets provider for HashiCorp Vault."""
 
     slug = "hashicorp-vault"
     name = "HashiCorp Vault"
     is_available = hvac is not None
@@ -49,33 +58,43 @@
             help_text="The key of the HashiCorp Vault secret",
         )
         mount_point = forms.CharField(
             required=False,
             help_text=f"The path where the secret engine was mounted on (Default: <code>{DEFAULT_MOUNT_POINT}</code>)",
             initial=DEFAULT_MOUNT_POINT,
         )
+        kv_version = forms.ChoiceField(
+            required=False,
+            choices=HashicorpKVVersionChoices,
+            help_text=f"The version of the kv engine (either v1 or v2) (Default: <code>{DEFAULT_KV_VERSION}</code>)",
+            initial=DEFAULT_KV_VERSION,
+        )
 
     @classmethod
     def validate_vault_settings(cls, secret=None):
         """Validate the vault settings."""
         # This is only required for HashiCorp Vault therefore not defined in
         # `required_settings` for the plugin config.
         plugin_settings = settings.PLUGINS_CONFIG["nautobot_secrets_providers"]
         if "hashicorp_vault" not in plugin_settings:
             raise exceptions.SecretProviderError(secret, cls, "HashiCorp Vault is not configured!")
 
         vault_settings = plugin_settings.get("hashicorp_vault", {})
         auth_method = vault_settings.get("auth_method", "token")
+        kv_version = vault_settings.get("kv_version", HashicorpKVVersionChoices.KV_VERSION_2)
 
         if "url" not in vault_settings:
             raise exceptions.SecretProviderError(secret, cls, "HashiCorp Vault configuration is missing a url")
 
         if auth_method not in AUTH_METHOD_CHOICES:
             raise exceptions.SecretProviderError(secret, cls, f"HashiCorp Vault Auth Method {auth_method} is invalid!")
 
+        if kv_version not in HashicorpKVVersionChoices.as_dict():
+            raise exceptions.SecretProviderError(secret, cls, f"HashiCorp Vault KV version {kv_version} is invalid!")
+
         if auth_method == "aws":
             if not boto3:
                 raise exceptions.SecretProviderError(
                     secret, cls, "HashiCorp Vault AWS Authentication Method requires the boto3 library!"
                 )
         elif auth_method == "token":
             if "token" not in vault_settings:
@@ -105,20 +124,24 @@
         login_kwargs = vault_settings.get("login_kwargs", {})
 
         # According to the docs (https://hvac.readthedocs.io/en/stable/source/hvac_v1.html?highlight=verify#hvac.v1.Client.__init__)
         # the client verify parameter is either a boolean or a path to a ca certificate file to verify.  This is non-intuitive
         # so we use a parameter to specify the path to the ca_cert, if not provided we use the default of None
         ca_cert = vault_settings.get("ca_cert", None)
 
+        namespace = vault_settings.get("namespace", None)
+
         # Get the client and attempt to retrieve the secret.
         try:
             if auth_method == "token":
-                client = hvac.Client(url=vault_settings["url"], token=vault_settings["token"], verify=ca_cert)
+                client = hvac.Client(
+                    url=vault_settings["url"], token=vault_settings["token"], verify=ca_cert, namespace=namespace
+                )
             else:
-                client = hvac.Client(url=vault_settings["url"], verify=ca_cert)
+                client = hvac.Client(url=vault_settings["url"], verify=ca_cert, namespace=namespace)
                 if auth_method == "approle":
                     client.auth.approle.login(
                         role_id=vault_settings["role_id"],
                         secret_id=vault_settings["secret_id"],
                         **login_kwargs,
                     )
                 elif auth_method == "kubernetes":
@@ -152,24 +175,30 @@
         """Return the value stored under the secret’s key in the secret’s path."""
         # Try to get parameters and error out early.
         parameters = secret.rendered_parameters(obj=obj)
         try:
             secret_path = parameters["path"]
             secret_key = parameters["key"]
             secret_mount_point = parameters.get("mount_point", DEFAULT_MOUNT_POINT)
+            secret_kv_version = parameters.get("kv_version", DEFAULT_KV_VERSION)
         except KeyError as err:
             msg = f"The secret parameter could not be retrieved for field {err}"
             raise exceptions.SecretParametersError(secret, cls, msg) from err
 
         client = cls.get_client(secret)
 
         try:
-            response = client.secrets.kv.read_secret(path=secret_path, mount_point=secret_mount_point)
+            if secret_kv_version == HashicorpKVVersionChoices.KV_VERSION_1:
+                response = client.secrets.kv.v1.read_secret(path=secret_path, mount_point=secret_mount_point)
+            else:
+                response = client.secrets.kv.v2.read_secret(path=secret_path, mount_point=secret_mount_point)
         except hvac.exceptions.InvalidPath as err:
             raise exceptions.SecretValueNotFoundError(secret, cls, str(err)) from err
 
         # Retrieve the value using the key or complain loudly.
         try:
+            if secret_kv_version == HashicorpKVVersionChoices.KV_VERSION_1:
+                return response["data"][secret_key]
             return response["data"]["data"][secret_key]
         except KeyError as err:
             msg = f"The secret value could not be retrieved using key {err}"
             raise exceptions.SecretValueNotFoundError(secret, cls, msg) from err
```

### Comparing `nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/secrets.py` & `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/secrets.py`

 * *Files identical despite different names*

### Comparing `nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/templates/nautobot_secrets_providers/home.html` & `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/templates/nautobot_secrets_providers/home.html`

 * *Files 27% similar despite different names*

```diff
@@ -23,26 +23,32 @@
                 <tbody>
                     <tr>
                         <td><a href="https://aws.amazon.com/secrets-manager/" rel="nofollow">AWS Secrets Manager</a></td>
                         <td><a href="https://docs.aws.amazon.com/secretsmanager/latest/userguide/manage_create-basic-secret.html" rel="nofollow">Other: Key/value pairs</a></td>
                         <td><a href="https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html" rel="nofollow">AWS credentials</a></td>
                     </tr>
                     <tr>
+                        <td><a href="https://docs.aws.amazon.com/systems-manager/latest/userguide/systems-manager-parameter-store.html" rel="nofollow">AWS Systems Manager Parameter Store</a></td>
+                        <td><a href="https://docs.aws.amazon.com/systems-manager/latest/userguide/param-create-cli.html" rel="nofollow">Other: Key/value pairs</a></td>
+                        <td><a href="https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html" rel="nofollow">AWS credentials</a></td>
+                    </tr>
+                    <tr>
                         <td><a href="https://www.vaultproject.io" rel="nofollow">HashiCorp Vault</a></td>
-                        <td><a href="https://www.vaultproject.io/docs/secrets/kv/kv-v2" rel="nofollow">K/V Version 2</a></td>
+                        <td><a href="https://www.vaultproject.io/docs/secrets/kv/kv-v1" rel="nofollow">K/V Version 1</a><br />
+                            <a href="https://www.vaultproject.io/docs/secrets/kv/kv-v2" rel="nofollow">K/V Version 2</a></td>
                         <td><a href="https://www.vaultproject.io/docs/auth/token" rel="nofollow">Token</a><br/>
                             <a href="https://www.vaultproject.io/docs/auth/approle" rel="nofollow">AppRole</a></td>
                     </tr>
                     <tr>
-                        <td><a href="https://thycotic.com/" rel="nofollow">Thycotic Secret Server</a></td>
-                        <td><a href="https://github.com/thycotic/python-tss-sdk#secret-server-cloud" rel="nofollow">Secret Server Cloud</a><br/>
-                            <a href="https://github.com/thycotic/python-tss-sdk#secret-server" rel="nofollow">Secret Server (on-prem)</a></td>
-                        <td><a href="https://github.com/thycotic/python-tss-sdk#password-authorization" rel="nofollow">Password Authorization</a><br/>
-                            <a href="https://github.com/thycotic/python-tss-sdk#domain-authorization" rel="nofollow">Domain Authorization</a><br/>
-                            <a href="https://github.com/thycotic/python-tss-sdk#access-token-authorization" rel="nofollow">Access Token Authorization</a></td>
+                        <td><a href="https://delinea.com/" rel="nofollow">Delinea/Thycotic Secret Server</a></td>
+                        <td><a href="https://github.com/DelineaXPM/python-tss-sdk#secret-server-cloud" rel="nofollow">Secret Server Cloud</a><br/>
+                            <a href="https://github.com/DelineaXPM/python-tss-sdk#secret-server" rel="nofollow">Secret Server (on-prem)</a></td>
+                        <td><a href="https://github.com/DelineaXPM/python-tss-sdk#password-authorization" rel="nofollow">Password Authorization</a><br/>
+                            <a href="https://github.com/DelineaXPM/python-tss-sdk#domain-authorization" rel="nofollow">Domain Authorization</a><br/>
+                            <a href="https://github.com/DelineaXPM/python-tss-sdk#access-token-authorization" rel="nofollow">Access Token Authorization</a></td>
                     </tr>
                 </tbody>
             </table>
         </div>
     </div>
     </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,13 +1,16 @@
 {% extends 'base.html' %} {% load static %} {% load helpers %} {% block header
 %}
 ****** {% block title %}Secrets Providers Home{% endblock %} ******
 {% endblock header %} {% block content %}
 Enabled Secrets Providers
-Secrets Backend        Supported Secret Types  Supported Authentication Methods
-AWS_Secrets_Manager    Other:_Key/value_pairs  AWS_credentials
-HashiCorp_Vault        K/V_Version_2           Token
-                                               AppRole
-                       Secret_Server_Cloud     Password_Authorization
-Thycotic_Secret_Server Secret_Server_(on-prem) Domain_Authorization
-                                               Access_Token_Authorization
+Secrets Backend         Supported Secret Types  Supported Authentication
+                                                Methods
+AWS_Secrets_Manager     Other:_Key/value_pairs  AWS_credentials
+AWS_Systems_Manager     Other:_Key/value_pairs  AWS_credentials
+Parameter_Store
+HashiCorp_Vault         K/V_Version_1           Token
+                        K/V_Version_2           AppRole
+Delinea/Thycotic_Secret Secret_Server_Cloud     Password_Authorization
+Server                  Secret_Server_(on-prem) Domain_Authorization
+                                                Access_Token_Authorization
 {% endblock content %}
```

### Comparing `nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/tests/nautobot_config.py` & `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/tests/nautobot_config.py`

 * *Files identical despite different names*

### Comparing `nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/tests/test_basic.py` & `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/tests/test_providers.py` & `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/tests/test_providers.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,21 +3,26 @@
 from unittest.mock import patch, mock_open
 
 import boto3
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.test import Client, TestCase, tag
 from hvac import Client as HVACClient
-from moto import mock_secretsmanager
+from moto import mock_secretsmanager, mock_ssm
 import requests_mock
 
 from nautobot.extras.models import Secret
 from nautobot.extras.secrets import exceptions
-from nautobot_secrets_providers.providers import AWSSecretsManagerSecretsProvider, HashiCorpVaultSecretsProvider
+from nautobot_secrets_providers.providers import (
+    AWSSecretsManagerSecretsProvider,
+    AWSSystemsManagerParameterStore,
+    HashiCorpVaultSecretsProvider,
+)
 
+from nautobot_secrets_providers.providers.choices import HashicorpKVVersionChoices
 
 # Use the proper swappable User model
 User = get_user_model()
 
 
 @tag("unit")
 class SecretsProviderTestCase(TestCase):
@@ -174,27 +179,114 @@
         super().setUp()
 
         # The secret we be using.
         self.secret = Secret.objects.create(
             name="hello-hashicorp",
             slug="hello-hashicorp",
             provider=self.provider.slug,
-            parameters={"path": "hello", "key": "location"},
+            parameters={
+                "path": "hello",
+                "key": "location",
+                "kv_version": HashicorpKVVersionChoices.KV_VERSION_2,
+            },
         )
         # The secret with a mounting point we be using.
         self.secret_mounting_point = Secret.objects.create(
             name="hello-hashicorp-mntpnt",
             slug="hello-hashicorp-mntpnt",
             provider=self.provider.slug,
-            parameters={"path": "hello", "key": "location", "mount_point": "mymount"},
+            parameters={
+                "path": "hello",
+                "key": "location",
+                "mount_point": "mymount",
+                "kv_version": HashicorpKVVersionChoices.KV_VERSION_2,
+            },
         )
         self.test_path = "http://localhost:8200/v1/secret/data/hello"
         self.test_mountpoint_path = "http://localhost:8200/v1/mymount/data/hello"
 
     @requests_mock.Mocker()
+    def test_v1(self, requests_mocker):
+        mock_kv_v1_response = {
+            "request_id": "f0185257-af7a-f550-2d9a-ada457a70e17",
+            "lease_id": "",
+            "renewable": False,
+            "lease_duration": 0,
+            "data": {
+                "location": "world",
+            },
+            "wrap_info": None,
+            "warnings": None,
+            "auth": None,
+        }
+        kv_v1_test_path = "http://localhost:8200/v1/secret/hello"
+        kv_v1_test_mountpoint_path = "http://localhost:8200/v1/mymount/hello"
+        kv_v1_secret = Secret.objects.create(
+            name="hello-hashicorp-v1",
+            slug="hello-hashicorp-v1",
+            provider=self.provider.slug,
+            parameters={"path": "hello", "key": "location", "kv_version": HashicorpKVVersionChoices.KV_VERSION_1},
+        )
+        kv_v1_secret_mounting_point = Secret.objects.create(
+            name="hello-hashicorp-mntpnt-v1",
+            slug="hello-hashicorp-mntpnt-v1",
+            provider=self.provider.slug,
+            parameters={
+                "path": "hello",
+                "key": "location",
+                "mount_point": "mymount",
+                "kv_version": HashicorpKVVersionChoices.KV_VERSION_1,
+            },
+        )
+
+        with self.subTest("Test v1 retrieve success"):
+            requests_mocker.register_uri(method="GET", url=kv_v1_test_path, json=mock_kv_v1_response)
+
+            response = self.provider.get_value_for_secret(kv_v1_secret)
+            self.assertEqual(mock_kv_v1_response["data"]["location"], response)
+
+        with self.subTest("Test v1 retrieve success with mount point set"):
+            requests_mocker.register_uri(method="GET", url=kv_v1_test_mountpoint_path, json=mock_kv_v1_response)
+
+            response = self.provider.get_value_for_secret(kv_v1_secret_mounting_point)
+            self.assertEqual(mock_kv_v1_response["data"]["location"], response)
+
+    @requests_mock.Mocker()
+    def test_v2_fallback(self, requests_mocker):
+        """
+        Before https://github.com/nautobot/nautobot-plugin-secrets-providers/pull/53 was merged, the Hashicorp
+        provider would only support KV v2 and did not include a way to specify the KV version.
+        This test ensures that the provider will still work without the kv_version parameter.
+        """
+        kv_v2_fallback_secret = Secret.objects.create(
+            name="hello-hashicorp-v2-fallback",
+            slug="hello-hashicorp-v2-fallback",
+            provider=self.provider.slug,
+            parameters={"path": "hello", "key": "location"},
+        )
+        kv_v2_fallback_secret_mounting_point = Secret.objects.create(
+            name="hello-hashicorp-mntpnt-v2-fallback",
+            slug="hello-hashicorp-mntpnt-v2-fallback",
+            provider=self.provider.slug,
+            parameters={"path": "hello", "key": "location", "mount_point": "mymount"},
+        )
+
+        with self.subTest("Test v2 fallback retrieve success"):
+            requests_mocker.register_uri(method="GET", url=self.test_path, json=self.mock_response)
+
+            response = self.provider.get_value_for_secret(kv_v2_fallback_secret)
+            self.assertEqual(self.mock_response["data"]["data"]["location"], response)
+
+        with self.subTest("Test v2 fallback retrieve success with mount point set"):
+            requests_mocker.register_uri(method="GET", url=self.test_mountpoint_path, json=self.mock_response)
+
+            response = self.provider.get_value_for_secret(kv_v2_fallback_secret_mounting_point)
+            self.assertEqual(self.mock_response["data"]["data"]["location"], response)
+
+    @requests_mock.Mocker()
     def test_retrieve_success(self, requests_mocker):
         """Retrieve a secret successfully."""
         requests_mocker.register_uri(method="GET", url=self.test_path, json=self.mock_response)
 
         response = self.provider.get_value_for_secret(self.secret)
         self.assertEqual(self.mock_response["data"]["data"]["location"], response)
 
@@ -444,7 +536,75 @@
             requests_mocker.register_uri(method="POST", url=f"{vault_url}/v1/auth/aws/login", status_code=400)
             with self.assertRaises(exceptions.SecretProviderError) as err:
                 self.provider.get_client(self.secret)
             self.assertEqual(
                 str(err.exception),
                 'SecretProviderError: Secret "hello-hashicorp" (provider "HashiCorpVaultSecretsProvider"): HashiCorp Vault Login failed (auth_method: aws). Error: , on post http://localhost:8200/v1/auth/aws/login',
             )
+
+
+class AWSSystemsManagerParameterStoreTestCase(SecretsProviderTestCase):
+    """Tests for AWSSystemsManagerParameterStore."""
+
+    provider = AWSSystemsManagerParameterStore
+
+    def setUp(self):
+        super().setUp()
+        self.secret = Secret.objects.create(
+            name="hello-aws-parameterstore",
+            slug="hello-aws-parameterstore",
+            provider=self.provider.slug,
+            parameters={"name": "hello", "region": "eu-west-3", "key": "location"},
+        )
+
+    @mock_ssm
+    def test_retrieve_success(self):
+        """Retrieve a secret successfully."""
+        conn = boto3.client("ssm", region_name=self.secret.parameters["region"])
+        conn.put_parameter(Name="hello", Type="SecureString", Value='{"location":"world"}')
+        result = self.provider.get_value_for_secret(self.secret)
+        self.assertEqual(result, "world")
+
+    @mock_ssm
+    def test_retrieve_does_not_exist(self):
+        """Try and fail to retrieve a secret that doesn't exist."""
+        boto3.client("ssm", region_name=self.secret.parameters["region"])
+
+        with self.assertRaises(exceptions.SecretParametersError) as err:
+            self.provider.get_value_for_secret(self.secret)
+
+        exc = err.exception
+        self.assertIn("ParameterNotFound", exc.message)
+
+    @mock_ssm
+    def test_retrieve_invalid_key(self):
+        """Try and fail to retrieve a secret from an existing parameter but an invalid key."""
+        conn = boto3.client("ssm", region_name=self.secret.parameters["region"])
+        conn.put_parameter(Name="hello", Type="SecureString", Value='{"position":"world"}')
+        # Try to fetch the secret with key as locatio
+        with self.assertRaises(exceptions.SecretParametersError) as err:
+            self.provider.get_value_for_secret(self.secret)
+        exc = err.exception
+        self.assertIn(f"InvalidKeyName '{self.secret.parameters['key']}'", exc.message)
+
+    @mock_ssm
+    def test_retrieve_non_valid_json(self):
+        conn = boto3.client("ssm", region_name=self.secret.parameters["region"])
+        conn.put_parameter(Name="hello", Type="SecureString", Value="Non Valid JSON")
+
+        with self.assertRaises(exceptions.SecretValueNotFoundError) as err:
+            self.provider.get_value_for_secret(self.secret)
+
+        exc = err.exception
+        self.assertIn("InvalidJson", exc.message)
+
+    @mock_ssm
+    def test_retrieve_invalid_version(self):
+        """Try and fail to retrieve a parameter while specifying an invalid version|label."""
+        conn = boto3.client("ssm", region_name=self.secret.parameters["region"])
+        conn.put_parameter(Name="hello", Type="SecureString", Value='{"location":"world"}')
+        # add a non existing version to the Nautobot secret name and try to fetch it
+        self.secret.parameters["name"] += ":2"
+        with self.assertRaises(exceptions.SecretValueNotFoundError) as err:
+            self.provider.get_value_for_secret(self.secret)
+        exc = err.exception
+        self.assertIn("ParameterVersionNotFound", exc.message)
```

### Comparing `nautobot-secrets-providers-1.3.0/nautobot_secrets_providers/views.py` & `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/views.py`

 * *Files identical despite different names*

### Comparing `nautobot-secrets-providers-1.3.0/pyproject.toml` & `nautobot_secrets_providers-1.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-secrets-providers"
-version = "v1.3.0"
+version = "v1.4.0"
 description = "Nautobot Secrets Providers Plugin."
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-secrets-providers"
 repository = "https://github.com/nautobot/nautobot-plugin-secrets-providers"
 keywords = ["nautobot", "nautobot-plugin"]
@@ -15,36 +15,36 @@
 packages = [
     { include = "nautobot_secrets_providers" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 # Pin this to the lowest supported version of Nautobot
-nautobot = "~1.2.1"
+nautobot = "^1.4.0"
 
 #
 # Optional dependencies installed as extras
 # 
 
 # AWS SDK for Python (always keep in sync w/ dev dependency)
 boto3 = { version = "~1.19.5", optional = true }
 # HashiCorp Vault API Client (always keep in sync w/ dev dependency)
-hvac = { version = "~0.11.0", optional = true }
+hvac = { version = ">=0.11.0, <1.1.0", optional = true }
 # Thycotic Secret Server (always keep in sync w/ dev dependency)
 python-tss-sdk = {version = "~1.2.0", optional = true}
 
 
 [tool.poetry.dev-dependencies]
 bandit = "*"
 black = "*"
 boto3 = "~1.19.5"  # (always keep in sync w/ optional dependency)
 coverage = "~6.2"
 django-debug-toolbar = "*"
 flake8 = ">=3.9.2"
-hvac = "~0.11.0"  # (always keep in sync w/ optional dependency)
+hvac = ">=0.11.0, <1.1.0"  # (always keep in sync w/ optional dependency)
 invoke = "*"
 moto = "~2.2.11"
 mkdocs = "*"
 pydocstyle = "*"
 pylint = "*"
 pylint-django = "*"
 python-tss-sdk = "~1.2.0"  # (always keep in sync w/ optional dependency)
```

### Comparing `nautobot-secrets-providers-1.3.0/setup.py` & `nautobot_secrets_providers-1.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,624 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nautobot-secrets-providers
+Version: 1.4.0
+Summary: Nautobot Secrets Providers Plugin.
+Home-page: https://github.com/nautobot/nautobot-plugin-secrets-providers
+License: Apache-2.0
+Keywords: nautobot,nautobot-plugin
+Author: Network to Code, LLC
+Author-email: opensource@networktocode.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: aws
+Provides-Extra: hashicorp
+Provides-Extra: nautobot
+Provides-Extra: thycotic
+Requires-Dist: boto3 (>=1.19.5,<1.20.0) ; extra == "all" or extra == "aws"
+Requires-Dist: hvac (>=0.11.0,<1.1.0) ; extra == "all" or extra == "hashicorp"
+Requires-Dist: nautobot (>=1.4.0,<2.0.0) ; extra == "nautobot"
+Requires-Dist: python-tss-sdk (>=1.2.0,<1.3.0) ; extra == "all" or extra == "thycotic"
+Project-URL: Repository, https://github.com/nautobot/nautobot-plugin-secrets-providers
+Description-Content-Type: text/markdown
 
-packages = \
-['nautobot_secrets_providers',
- 'nautobot_secrets_providers.migrations',
- 'nautobot_secrets_providers.providers',
- 'nautobot_secrets_providers.tests']
-
-package_data = \
-{'': ['*'],
- 'nautobot_secrets_providers': ['templates/nautobot_secrets_providers/*']}
-
-extras_require = \
-{':extra == "nautobot"': ['nautobot>=1.2.1,<1.3.0'],
- 'all': ['boto3>=1.19.5,<1.20.0',
-         'hvac>=0.11.0,<0.12.0',
-         'python-tss-sdk>=1.2.0,<1.3.0'],
- 'aws': ['boto3>=1.19.5,<1.20.0'],
- 'hashicorp': ['hvac>=0.11.0,<0.12.0'],
- 'thycotic': ['python-tss-sdk>=1.2.0,<1.3.0']}
-
-setup_kwargs = {
-    'name': 'nautobot-secrets-providers',
-    'version': '1.3.0',
-    'description': 'Nautobot Secrets Providers Plugin.',
-    'long_description': '# Nautobot Secrets Providers\n\nNautobot Secrets Providers is a plugin for [Nautobot](https://github.com/nautobot/nautobot) 1.2.0 or higher that bundles Secrets Providers for integrating with popular secrets backends. Nautobot 1.2.0 added support for integrating with retrieving secrets from various secrets providers.\n\nThis plugin publishes secrets providers that are not included in the within the Nautobot core software package so that it will be easier to maintain and extend support for various secrets providers without waiting on Nautobot software releases.\n\n## Supported Secrets Backends\n\nThis plugin supports the following popular secrets backends:\n\n| Secrets Backend                                              | Supported Secret Types                                       | Supported Authentication Methods                             |\n| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |\n| [AWS Secrets Manager](https://aws.amazon.com/secrets-manager/) | [Other: Key/value pairs](https://docs.aws.amazon.com/secretsmanager/latest/userguide/manage_create-basic-secret.html) | [AWS credentials](https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html) (see Usage section below) |\n| [HashiCorp Vault](https://www.vaultproject.io)               | [K/V Version 2](https://www.vaultproject.io/docs/secrets/kv/kv-v2) | [Token](https://www.vaultproject.io/docs/auth/token)<br/>[AppRole](https://www.vaultproject.io/docs/auth/approle)<br/>[AWS](https://www.vaultproject.io/docs/auth/aws)<br/>[Kubernetes](https://www.vaultproject.io/docs/auth/kubernetes)         |\n| [Delinea/Thycotic Secret Server](https://delinea.com/products/secret-server)               | [Secret Server Cloud](https://github.com/DelineaXPM/python-tss-sdk#secret-server-cloud)<br/>[Secret Server (on-prem)](https://github.com/DelineaXPM/python-tss-sdk#initializing-secretserver)| [Access Token Authorization](https://github.com/DelineaXPM/python-tss-sdk#access-token-authorization)<br/>[Domain Authorization](https://github.com/DelineaXPM/python-tss-sdk#domain-authorization)<br/>[Password Authorization](https://github.com/DelineaXPM/python-tss-sdk#password-authorization)<br/>         |\n\n## Screenshots\n\n![Screenshot of installed plugins](https://raw.githubusercontent.com/nautobot/nautobot-plugin-secrets-providers/develop/docs/images/screenshot01.png "Plugin landing page")\n\n---\n\n![Screenshot of plugin home page](https://raw.githubusercontent.com/nautobot/nautobot-plugin-secrets-providers/develop/docs/images/screenshot02.png "Plugin Home page")\n\n---\n\n![Screenshot of secret using AWS Secrets Manager](https://raw.githubusercontent.com/nautobot/nautobot-plugin-secrets-providers/develop/docs/images/screenshot03.png "Secret using AWS Secrets Manager")\n\n---\n\n![Screenshot of secret using HashiCorp Vault](https://raw.githubusercontent.com/nautobot/nautobot-plugin-secrets-providers/develop/docs/images/screenshot04.png "Secret using HashiCorp Vault")\n\n---\n\n![Screenshot of secret using Delinea/Thycotic Secret Server by ID](https://raw.githubusercontent.com/nautobot/nautobot-plugin-secrets-providers/develop/docs/images/screenshot05.png "Secret using Thycotic Secret Server by ID")\n\n---\n\n![Screenshot of secret using Delinea/Thycotic Secret Server by Path](https://raw.githubusercontent.com/nautobot/nautobot-plugin-secrets-providers/develop/docs/images/screenshot06.png "Secret using Thycotic Secret Server by Path")\n\n## Installation\n\n> Nautobot Secrets Providers is compatible with Nautobot 1.2.0 and higher. Support for Thycotic Secret Server requires Python 3.7 or later.\n\nThe package is available as a Python package in PyPI and can be installed with `pip`:\n\n```no-highlight\npip install nautobot-secrets-providers\n```\n\nYou may quickly install all of the dependent libraries using the following command, however, this is *not recommended for production deployments* as it will install extras that you may not need:\n\n```no-highlight\npip install nautobot-secrets-providers[all]\n```\n\n### Dependencies\n\nFor this plugin to operate you must install at least one of the dependent libraries required by the secrets providers.\n\n**You must install the dependencies for at least one of the supported secrets providers or a `RuntimeError` will be raised.**\n\n#### AWS Secrets Manager\n\nThe AWS Secrets Manager provider requires the `boto3` library. This can be easily installed along with the plugin using the following command:\n\n```no-highlight\npip install nautobot-secrets-providers[aws]\n```\n\n#### HashiCorp Vault\n\nThe HashiCorp Vault provider requires the `hvac` library. This can easily be installed along with the plugin using the following command:\n\n```no-highlight\npip install nautobot-secrets-providers[hashicorp]\n```\n\n#### Delinea/Thycotic Secret Server\n\nThe Delinea/Thycotic Secret Server provider requires the `python-tss-sdk` library. This can easily be installed along with the plugin using the following command:\n\n```no-highlight\npip install nautobot-secrets-providers[thycotic]\n```\n\n### Enabling Secrets Providers\n\nTo ensure Nautobot Secrets Providers is automatically re-installed during future upgrades, create a file named `local_requirements.txt` (if not already existing) in the Nautobot root directory (alongside `requirements.txt`) and list the `secrets` package:\n\n```no-highlight\necho nautobot-secrets-providers >> local_requirements.txt\n```\n\nOnce installed, the plugin needs to be enabled in your `nautobot_config.py`:\n\n```python\n# In your nautobot_config.py\nPLUGINS = ["nautobot_secrets_providers"]\n\n# PLUGINS_CONFIG = {\n#   "nautobot_secrets_providers": {\n#      See below for how to configure Nautobot for each secrets provider!\n#   }\n# }\n```\n\n## Usage\n\nBefore you proceed, you must have **at least one** of the dependent libaries installed as detailed above.\n\nPlease do not enable this plugin until you are able to install the dependencies, as it will block Nautobot from starting.\n\n### AWS Secrets Manager\n\n#### Authentication\n\nNo configuration is needed within Nautobot for this provider to operate. Instead you must provide [AWS credentials in one of the methods supported by the `boto3` library](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html#configuring-credentials).\n\nBoto3 credentials can be configured in multiple ways (eight as of this writing) that are mirrored here:\n\n1. Passing credentials as parameters in the `boto.client()` method\n2. Passing credentials as parameters when creating a Session object\n3. Environment variables\n4. Shared credential file (`~/.aws/credentials`)\n5. AWS config file (`~/.aws/config`)\n6. Assume Role provider\n7. Boto2 config file (`/etc/boto.cfg` and `~/.boto`)\n8. Instance metadata service on an Amazon EC2 instance that has an IAM role configured.\n\n**The AWS Secrets Manager provider only supports methods 3-8. Methods 1 and 2 ARE NOT SUPPORTED at this time.**\n\nWe highly recommend you defer to using environment variables for your deployment as specified in the credentials documentation linked above. The values specified in the linked documentation should be [set within your `~.bashrc`](https://nautobot.readthedocs.io/en/latest/installation/nautobot/#update-the-nautobot-bashrc) (or similar profile) on your system.\n\n#### Configuration\n\nThis is an example based on our recommended deployment pattern in the section above (item 3) that is using [environment variables](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html#environment-variables). You will need to set these in the environment prior to starting Nautobot:\n\n```no-highlight\nexport AWS_ACCESS_KEY_ID=foo      # The access key for your AWS account.\nexport AWS_SECRET_ACCESS_KEY=bar  # The secret key for your AWS account.\n```\n\nPlease refer to the [Nautobot documentation on updating your `.bashrc`](https://nautobot.readthedocs.io/en/latest/installation/nautobot/#update-the-nautobot-bashrc) for how to do this for production Nautobot deployments.\n\n### HashiCorp Vault\n\n#### Configuration\n\nYou must provide a mapping in `PLUGINS_CONFIG` within your `nautobot_config.py`, for example:\n\n```python\nPLUGINS_CONFIG = {\n    "nautobot_secrets_providers": {\n        "hashicorp_vault": {\n            "url": "http://localhost:8200",\n            "auth_method": "token",\n            "token": os.getenv("NAUTOBOT_HASHICORP_VAULT_TOKEN"),\n        }\n    },\n}\n```\n\n- `url` - (required) The URL to the HashiCorp Vault instance (e.g. `http://localhost:8200`).\n- `auth_method` - (optional / defaults to "token") The method used to authenticate against the HashiCorp Vault instance. Either `"approle"`, `"aws"`, `"kubernetes"` or `"token"`.  For information on using AWS authentication with vault see the [authentication](#authentication) section above.\n- `ca_cert` - (optional) Path to a PEM formatted CA certificate to use when verifying the Vault connection.  Can alternatively be set to `False` to ignore SSL verification (not recommended) or `True` to use the system certificates.\n- `default_mount_point` - (optional / defaults to "secret") The default mount point of the K/V Version 2 secrets engine within Hashicorp Vault.\n- `k8s_token_path` - (optional) Path to the kubernetes service account token file.  Defaults to "/var/run/secrets/kubernetes.io/serviceaccount/token".\n- `token` - (optional) Required when `"auth_method": "token"` or `auth_method` is not supplied. The token for authenticating the client with the HashiCorp Vault instance. As with other sensitive service credentials, we recommend that you provide the token value as an environment variable and retrieve it with `{"token": os.getenv("NAUTOBOT_HASHICORP_VAULT_TOKEN")}` rather than hard-coding it in your `nautobot_config.py`.\n- `role_name` - (optional) Required when `"auth_method": "kubernetes"`, optional when `"auth_method": "aws"`.  The Vault Kubernetes role or Vault AWS role to assume which the pod\'s service account has access to.\n- `role_id` - (optional) Required when `"auth_method": "approle"`. As with other sensitive service credentials, we recommend that you provide the role_id value as an environment variable and retrieve it with `{"role_id": os.getenv("NAUTOBOT_HASHICORP_VAULT_ROLE_ID")}` rather than hard-coding it in your `nautobot_config.py`.\n- `secret_id` - (optional) Required when `"auth_method": "approle"`.As with other sensitive service credentials, we recommend that you provide the secret_id value as an environment variable and retrieve it with `{"secret_id": os.getenv("NAUTOBOT_HASHICORP_VAULT_SECRET_ID")}` rather than hard-coding it in your `nautobot_config.py`.\n- `login_kwargs` - (optional) Additional optional parameters to pass to the login method for [`approle`](https://hvac.readthedocs.io/en/stable/source/hvac_api_auth_methods.html#hvac.api.auth_methods.AppRole.login), [`aws`](https://hvac.readthedocs.io/en/stable/source/hvac_api_auth_methods.html#hvac.api.auth_methods.Aws.iam_login) and [`kubernetes`](https://hvac.readthedocs.io/en/stable/source/hvac_api_auth_methods.html#hvac.api.auth_methods.Kubernetes.login) authentication methods.\n\n### Delinea/Thycotic Secret Server (TSS)\n\nThe Delinea/Thycotic Secret Server plugin includes two providers:\n\n- **`Thycotic Secret Server by ID`**\n\n    This provider uses the `Secret ID` to specifiy the secret that is selected. The `Secret ID` is displayed in the browser\'s URL field if you `Edit` the data in Thycotic Secret Server.\n\n    - Example:\n\n        The url is: _https://pw.example.local/SecretServer/app/#/secret/**1234**/general_\n\n        In this example the value for `Secret ID` is **1234**.\n\n- **`Thycotic Secret Server by Path`**\n\n    This provider allows to select the secret by folder-path and secret-name. The path delimiter is a \'\\\\\'.\n\n    The `Secret path` is displayed as page header when `Edit` a secret.\n\n    - Example:\n\n        The header is: **NET-Automation > Nautobot > My-Secret**\n\n        In this example the value for `Secret path` is **`\\NET-Automation\\Nautobot\\My-Secret`**.\n\n#### Configuration\n\n```python\nPLUGINS_CONFIG = {\n    "nautobot_secrets_providers": {\n        "thycotic": {  # https://github.com/thycotic/python-tss-sdk\n            "base_url": os.getenv("SECRET_SERVER_BASE_URL", None),\n            "ca_bundle_path": os.getenv("REQUESTS_CA_BUNDLE", None),\n            "cloud_based": is_truthy(os.getenv("SECRET_SERVER_IS_CLOUD_BASED", "False")),\n            "domain": os.getenv("SECRET_SERVER_DOMAIN", None),\n            "password": os.getenv("SECRET_SERVER_PASSWORD", None),\n            "tenant": os.getenv("SECRET_SERVER_TENANT", None),\n            "token": os.getenv("SECRET_SERVER_TOKEN", None),\n            "username": os.getenv("SECRET_SERVER_USERNAME", None),\n        },\n    }\n}\n```\n- `base_url` - (required) The Secret Server base_url. _e.g.\'https://pw.example.local/SecretServer\'_\n- `ca_bundle_path` - (optional) When using self-signed certificates this variable must be set to a file containing the trusted certificates (in .pem format). _e.g. \'/etc/ssl/certs/ca-bundle.trust.crt\'_.\n- `cloud_based` - (optional) Set to "True" if Secret Server Cloud should be used. (Default: "False").\n- `domain` - (optional) Required for \'Domain Authorization\'\n- `password` - (optional) Required for \'Secret Server Cloud\', \'Password Authorization\', \'Domain Authorization\'.\n- `tenant` - (optional) Required for \'Domain Authorization\'.\n- `token` - (optional) Required for \'Access Token Authorization\'.\n- `username` - (optional) Required for \'Secret Server Cloud\', \'Password Authorization\', \'Domain Authorization\'.\n\n## Contributing\n\nPull requests are welcomed and automatically built and tested against multiple version of Python and multiple version of Nautobot through GitHub Actions.\n\nThe project is packaged with a light development environment based on `docker-compose` to help with the local development of the project and to run the tests within GitHub Actions.\n\nThe project is following Network to Code software development guidelines and is leveraging:\n\n- Black, Pylint, Bandit and pydocstyle for Python linting and formatting.\n- Django unit test to ensure the plugin is working properly.\n\n### Development Environment\n\nThe development environment can be used in 2 ways. First, with a local poetry environment if you wish to develop outside of Docker with the caveat of using external services provided by Docker for PostgreSQL and Redis. Second, all services are spun up using Docker and a local mount so you can develop locally, but Nautobot is spun up within the Docker container.\n\nBelow is a quick start guide if you\'re already familiar with the development environment provided, but if you\'re not familiar, please read the [Getting Started Guide](GETTING_STARTED.md).\n\n#### Invoke\n\nThe [PyInvoke](http://www.pyinvoke.org/) library is used to provide some helper commands based on the environment.  There are a few configuration parameters which can be passed to PyInvoke to override the default configuration:\n\n* `nautobot_ver`: the version of Nautobot to use as a base for any built docker containers (default: 1.2.0)\n* `project_name`: the default docker compose project name (default: nautobot_secrets_providers)\n* `python_ver`: the version of Python to use as a base for any built docker containers (default: 3.7)\n* `local`: a boolean flag indicating if invoke tasks should be run on the host or inside the docker containers (default: False, commands will be run in docker containers)\n* `compose_dir`: the full path to a directory containing the project compose files\n* `compose_files`: a list of compose files applied in order (see [Multiple Compose files](https://docs.docker.com/compose/extends/#multiple-compose-files) for more information)\n\nUsing **PyInvoke** these configuration options can be overridden using [several methods](http://docs.pyinvoke.org/en/stable/concepts/configuration.html).  Perhaps the simplest is simply setting an environment variable `INVOKE_NAUTOBOT_SECRETS_PROVIDERS_VARIABLE_NAME` where `VARIABLE_NAME` is the variable you are trying to override.  The only exception is `compose_files`, because it is a list it must be overridden in a yaml file.  There is an example `invoke.yml` (`invoke.example.yml`) in this directory which can be used as a starting point.\n\n#### Local Poetry Development Environment\n\n1. Copy `development/creds.example.env` to `development/creds.env` (This file will be ignored by Git and Docker)\n2. Uncomment the `POSTGRES_HOST`, `REDIS_HOST`, and `NAUTOBOT_ROOT` variables in `development/creds.env`\n3. Create an `invoke.yml` file with the following contents at the root of the repo (you can also `cp invoke.example.yml invoke.yml` and edit as necessary):\n\n```yaml\n---\nnautobot_secrets_providers:\n  local: true\n  compose_files:\n    - "docker-compose.requirements.yml"\n```\n\n3. Run the following commands:\n\n```shell\npoetry shell\npoetry install --extras nautobot\nexport $(cat development/dev.env | xargs)\nexport $(cat development/creds.env | xargs)\ninvoke start && sleep 5\nnautobot-server migrate\n```\n\n> If you want to develop on the latest develop branch of Nautobot, run the following command: `poetry add --optional git+https://github.com/nautobot/nautobot@develop`. After the `@` symbol must match either a branch or a tag.\n\n4. You can now run nautobot-server commands as you would from the [Nautobot documentation](https://nautobot.readthedocs.io/en/latest/) for example to start the development server:\n\n```shell\nnautobot-server runserver 0.0.0.0:8080 --insecure\n```\n\nNautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).\n\nIt is typically recommended to launch the Nautobot **runserver** command in a separate shell so you can keep developing and manage the webserver separately.\n\n#### Docker Development Environment\n\nThis project is managed by [Python Poetry](https://python-poetry.org/) and has a few requirements to setup your development environment:\n\n1. Install Poetry, see the [Poetry Documentation](https://python-poetry.org/docs/#installation) for your operating system.\n2. Install Docker, see the [Docker documentation](https://docs.docker.com/get-docker/) for your operating system.\n\nOnce you have Poetry and Docker installed you can run the following commands to install all other development dependencies in an isolated python virtual environment:\n\n```shell\npoetry shell\npoetry install\ninvoke start\n```\n\nNautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).\n\nTo either stop or destroy the development environment use the following options.\n\n- **invoke stop** - Stop the containers, but keep all underlying systems intact\n- **invoke destroy** - Stop and remove all containers, volumes, etc. (This results in data loss due to the volume being deleted)\n\n### CLI Helper Commands\n\nThe project is coming with a CLI helper based on [invoke](http://www.pyinvoke.org/) to help setup the development environment. The commands are listed below in 3 categories `dev environment`, `utility` and `testing`.\n\nEach command can be executed with `invoke <command>`. Environment variables `INVOKE_NAUTOBOT_SECRETS_PROVIDERS_PYTHON_VER` and `INVOKE_NAUTOBOT_SECRETS_PROVIDERS_NAUTOBOT_VER` may be specified to override the default versions. Each command also has its own help `invoke <command> --help`\n\n#### Docker dev environment\n\n```no-highlight\n  build            Build all docker images.\n  debug            Start Nautobot and its dependencies in debug mode.\n  destroy          Destroy all containers and volumes.\n  restart          Restart Nautobot and its dependencies.\n  start            Start Nautobot and its dependencies in detached mode.\n  stop             Stop Nautobot and its dependencies.\n```\n\n#### Utility\n\n```no-highlight\n  cli              Launch a bash shell inside the running Nautobot container.\n  create-user      Create a new user in django (default: admin), will prompt for password.\n  makemigrations   Run Make Migration in Django.\n  nbshell          Launch a nbshell session.\n```\n\n#### Testing\n\n```no-highlight\n  bandit           Run bandit to validate basic static code security analysis.\n  black            Run black to check that Python files adhere to its style standards.\n  flake8           This will run flake8 for the specified name and Python version.\n  pydocstyle       Run pydocstyle to validate docstring formatting adheres to NTC defined standards.\n  pylint           Run pylint code analysis.\n  tests            Run all tests for this plugin.\n  unittest         Run Django unit tests for the plugin.\n```\n\n### Project Documentation\n\nProject documentation is generated by [mkdocs](https://www.mkdocs.org/) from the documentation located in the docs folder.  You can configure [readthedocs.io](https://readthedocs.io/) to point at this folder in your repo.  For development purposes a `docker-compose.docs.yml` is also included.  A container hosting the docs will be started using the invoke commands on [http://localhost:8001](http://localhost:8001), as changes are saved the docs will be automatically reloaded.\n\n### Developing Against Secrets Backends\n\n#### AWS Secrets Manager\n\nThis assumes you are logged into the AWS Console.\n\n- Navigate to AWS Console\n- Navigate to AWS Secrets Manager\n- Click "Store a new secret"\n  - Select “Other type of secrets”\n  - Use Secret key/value\n  - Enter `hello=world`\n  - Use "DefaultEncryptionKey" for now\n  - Click "Next"\n  - Under "Secret name" fill out `hello`\n  - Click "Next"\n  - Under "Configure automatic rotation"\n    - Leave it as "Disable automatic rotation"\n  - On "Store a new secret"\n    - Copy the sample code (see below)\n  - Click "Store"\n- END\n\n##### Install the AWS CLI\n\nNext, install the [AWS CLI](https://aws.amazon.com/cli/).\n\nOn MacOS, this can be done using `brew install awscli`:\n\n```\nbrew install awscli\n```\n\nOn Linux, you will need to run a `curl` command (This assumes x86. Please see the docs for [AWS CLI on\nLinux](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2-linux.html) for ARM and other options):\n\n```\ncurl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"\nunzip awscliv2.zip\nsudo ./aws/install\n```\n\n##### Configure the AWS CLI\n\nAfter installing the AWS CLI, you will need to configure it for authentication.\n\nYou may use an existing AWS access key or create a new one. For these instructions we cover the need to create a new access key that can be used for this.\n\n- Navigate to AWS Console\n- Click your username\n  - Click "My security credentials"\n  - Click "create access key"\n- Save your "Access key ID" and "Secret access key" for use when configuring the AWS CLI\n\nNow configure the CLI:\n\n- Run `aws configure`\n- Enter your credentials from above\n- Choose your region\n- Use output format: `json`\n\nExample:\n\n```no-highlight\n$ aws configure\nAWS Access Key ID [None]: AKIAIOSFODNN7EXAMPLE\nAWS Secret Access Key [None]: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY\nDefault region name [None]: us-east-2\nDefault output format [None]: json\n```\n\nNow you are ready to use the sample code to retrieve your secret from AWS Secrets Manager!\n\n##### Sample Code\n\nMake sure that the `boto3` client is installed:\n\n```no-highlight\npoetry install --extras aws\n```\n\nNext, save this as `aws_secrets.py`:\n\n```python\n# Use this code snippet in your app.\n# If you need more information about configurations or implementing the sample code, visit the AWS docs:\n# https://aws.amazon.com/developers/getting-started/python/\n\nimport boto3\nimport base64\nfrom botocore.exceptions import ClientError\n\n\ndef get_secret():\n\n    secret_name = "hello"\n    region_name = "us-east-2"\n\n    # Create a Secrets Manager client\n    session = boto3.session.Session()\n    client = session.client(\n        service_name=\'secretsmanager\',\n        region_name=region_name\n    )\n\n    # In this sample we only handle the specific exceptions for the \'GetSecretValue\' API.\n    # See https://docs.aws.amazon.com/secretsmanager/latest/apireference/API_GetSecretValue.html\n    # We rethrow the exception by default.\n\n    try:\n        get_secret_value_response = client.get_secret_value(\n            SecretId=secret_name\n        )\n    except ClientError as e:\n        if e.response[\'Error\'][\'Code\'] == \'DecryptionFailureException\':\n            # Secrets Manager can\'t decrypt the protected secret text using the provided KMS key.\n            # Deal with the exception here, and/or rethrow at your discretion.\n            raise e\n        elif e.response[\'Error\'][\'Code\'] == \'InternalServiceErrorException\':\n            # An error occurred on the server side.\n            # Deal with the exception here, and/or rethrow at your discretion.\n            raise e\n        elif e.response[\'Error\'][\'Code\'] == \'InvalidParameterException\':\n            # You provided an invalid value for a parameter.\n            # Deal with the exception here, and/or rethrow at your discretion.\n            raise e\n        elif e.response[\'Error\'][\'Code\'] == \'InvalidRequestException\':\n            # You provided a parameter value that is not valid for the current state of the resource.\n            # Deal with the exception here, and/or rethrow at your discretion.\n            raise e\n        elif e.response[\'Error\'][\'Code\'] == \'ResourceNotFoundException\':\n            # We can\'t find the resource that you asked for.\n            # Deal with the exception here, and/or rethrow at your discretion.\n            raise e\n    else:\n        # Decrypts secret using the associated KMS CMK.\n        # Depending on whether the secret is a string or binary, one of these fields will be populated.\n        if \'SecretString\' in get_secret_value_response:\n            secret = get_secret_value_response[\'SecretString\']\n        else:\n            decoded_binary_secret = base64.b64decode(get_secret_value_response[\'SecretBinary\'])\n\n    # Your code goes here.\n\n# ^ Above was generated by AWS.\n\n# This was added by us so you can run this as a script:\nif __name__ == "__main__":\n    secret = get_secret()\n    print(f"Secret = {secret}")\n```\n\nRun it with `python aws_secrets.py`:\n\n```\n$ python aws_secrets.py\nSecret = {"hello":"world"}.\n```\n\nNote that this blob is JSON and will also need to be decoded if you want to extract the value.\n\n#### HashiCorp Vault\n\nMake sure that the `hvac` client is installed:\n\n```no-highlight\npoetry install --extras hashicorp\n```\n\n##### Start Services with Docker\n\n```no-highlight\ninvoke start\n```\n\n##### Set an alias to work with `vault`\n\nThis will allow you to easily run the CLI command from within the container:\n\n```no-highlight\nalias vault="docker exec -it nautobot_secrets_providers_vault_1 vault"\n```\n\nInteract with the Vault vi CLI (via `docker exec` into the container from localhost):\n\n```no-highlight\n$ vault status\nKey             Value\n---             -----\nSeal Type       shamir\nInitialized     true\nSealed          false\nTotal Shares    1\nThreshold       1\nVersion         1.8.2\nStorage Type    inmem\nCluster Name    vault-cluster-35c5d319\nCluster ID      2611f99c-a6de-a883-1fcc-bfffdc0217bc\nHA Enabled      false\n```\n\n##### Using the Python `hvac` Library\n\nThis establishes a client, creates a basic key/value secret (`hello=world`) at the path `hello`, and then retrieves the data from the `hello` key at the secret path `hello`.\n\n> This is equivalent to the command `vault kv get -field hello secret/hello`.\n\n```python\nIn [1]: import hvac\n\nIn [2]: client = hvac.Client(url="http://localhost:8200", token="nautobot")\n\nIn [3]: client.secrets.kv.create_or_update_secret(path="hello", secret=dict(hello="world"))\nOut[3]:\n{\'request_id\': \'c4709868-c08f-4cb1-ab8c-605c58b82f3f\',\n \'lease_id\': \'\',\n \'renewable\': False,\n \'lease_duration\': 0,\n \'data\': {\'created_time\': \'2021-09-16T23:21:07.5564132Z\',\n  \'deletion_time\': \'\',\n  \'destroyed\': False,\n  \'version\': 2},\n \'wrap_info\': None,\n \'warnings\': None,\n \'auth\': None}\n\nIn [4]: client.secrets.kv.read_secret(path="hello")["data"]["data"]["hello"]\nOut[4]: \'world\'\n```\n\n## Questions\n\nFor any questions or comments, please check the [FAQ](FAQ.md) first and feel free to swing by the [Network to Code Slack workspace](https://networktocode.slack.com/) (channel `#networktocode`).\n',
-    'author': 'Network to Code, LLC',
-    'author_email': 'opensource@networktocode.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/nautobot/nautobot-plugin-secrets-providers',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
+# Nautobot Secrets Providers
+
+Nautobot Secrets Providers is a plugin for [Nautobot](https://github.com/nautobot/nautobot) 1.2.0 or higher that bundles Secrets Providers for integrating with popular secrets backends. Nautobot 1.2.0 added support for integrating with retrieving secrets from various secrets providers.
+
+This plugin publishes secrets providers that are not included in the within the Nautobot core software package so that it will be easier to maintain and extend support for various secrets providers without waiting on Nautobot software releases.
+
+## Supported Secrets Backends
+
+This plugin supports the following popular secrets backends:
+
+| Secrets Backend                                              | Supported Secret Types                                       | Supported Authentication Methods                             |
+| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
+| [AWS Secrets Manager](https://aws.amazon.com/secrets-manager/) | [Other: Key/value pairs](https://docs.aws.amazon.com/secretsmanager/latest/userguide/manage_create-basic-secret.html) | [AWS credentials](https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html) (see Usage section below) |
+| [AWS Systems Manager Parameter Store](https://aws.amazon.com/secrets-manager/) | [Other: Key/value pairs](https://docs.aws.amazon.com/systems-manager/latest/userguide/systems-manager-parameter-store.html) | [AWS credentials](https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html) (see Usage section below) |
+| [HashiCorp Vault](https://www.vaultproject.io)               | [K/V Version 2](https://www.vaultproject.io/docs/secrets/kv/kv-v2)<br/>[K/V Version 1](https://developer.hashicorp.com/vault/docs/secrets/kv/kv-v1) | [Token](https://www.vaultproject.io/docs/auth/token)<br/>[AppRole](https://www.vaultproject.io/docs/auth/approle)<br/>[AWS](https://www.vaultproject.io/docs/auth/aws)<br/>[Kubernetes](https://www.vaultproject.io/docs/auth/kubernetes)         |
+| [Delinea/Thycotic Secret Server](https://delinea.com/products/secret-server)               | [Secret Server Cloud](https://github.com/DelineaXPM/python-tss-sdk#secret-server-cloud)<br/>[Secret Server (on-prem)](https://github.com/DelineaXPM/python-tss-sdk#initializing-secretserver)| [Access Token Authorization](https://github.com/DelineaXPM/python-tss-sdk#access-token-authorization)<br/>[Domain Authorization](https://github.com/DelineaXPM/python-tss-sdk#domain-authorization)<br/>[Password Authorization](https://github.com/DelineaXPM/python-tss-sdk#password-authorization)<br/>         |
+
+## Screenshots
+
+![Screenshot of installed plugins](https://raw.githubusercontent.com/nautobot/nautobot-plugin-secrets-providers/develop/docs/images/screenshot01.png "Plugin landing page")
+
+---
+
+![Screenshot of plugin home page](https://raw.githubusercontent.com/nautobot/nautobot-plugin-secrets-providers/develop/docs/images/screenshot02.png "Plugin Home page")
+
+---
+
+![Screenshot of secret using AWS Secrets Manager](https://raw.githubusercontent.com/nautobot/nautobot-plugin-secrets-providers/develop/docs/images/screenshot03.png "Secret using AWS Secrets Manager")
+
+---
+
+![Screenshot of secret using HashiCorp Vault](https://raw.githubusercontent.com/nautobot/nautobot-plugin-secrets-providers/develop/docs/images/screenshot04.png "Secret using HashiCorp Vault")
+
+---
+
+![Screenshot of secret using Delinea/Thycotic Secret Server by ID](https://raw.githubusercontent.com/nautobot/nautobot-plugin-secrets-providers/develop/docs/images/screenshot05.png "Secret using Thycotic Secret Server by ID")
+
+---
+
+![Screenshot of secret using Delinea/Thycotic Secret Server by Path](https://raw.githubusercontent.com/nautobot/nautobot-plugin-secrets-providers/develop/docs/images/screenshot06.png "Secret using Thycotic Secret Server by Path")
+
+## Installation
+
+> Nautobot Secrets Providers is compatible with Nautobot 1.4.0 and higher. Support for Thycotic Secret Server requires Python 3.7 or later.
+
+The package is available as a Python package in PyPI and can be installed with `pip`:
+
+```no-highlight
+pip install nautobot-secrets-providers
+```
+
+You may quickly install all of the dependent libraries using the following command, however, this is *not recommended for production deployments* as it will install extras that you may not need:
+
+```no-highlight
+pip install nautobot-secrets-providers[all]
+```
+
+### Dependencies
+
+For this plugin to operate you must install at least one of the dependent libraries required by the secrets providers.
+
+**You must install the dependencies for at least one of the supported secrets providers or a `RuntimeError` will be raised.**
+
+#### AWS
+
+AWS Secrets Manager and Systems Manager Parameter Store are supported. Both providers require the `boto3` library. This can be easily installed along with the plugin using the following command:
+
+```no-highlight
+pip install nautobot-secrets-providers[aws]
+```
+
+#### HashiCorp Vault
+
+The HashiCorp Vault provider requires the `hvac` library. This can easily be installed along with the plugin using the following command:
+
+```no-highlight
+pip install nautobot-secrets-providers[hashicorp]
+```
+
+#### Delinea/Thycotic Secret Server
+
+The Delinea/Thycotic Secret Server provider requires the `python-tss-sdk` library. This can easily be installed along with the plugin using the following command:
+
+```no-highlight
+pip install nautobot-secrets-providers[thycotic]
+```
+
+### Enabling Secrets Providers
+
+To ensure Nautobot Secrets Providers is automatically re-installed during future upgrades, create a file named `local_requirements.txt` (if not already existing) in the Nautobot root directory (alongside `requirements.txt`) and list the `secrets` package:
+
+```no-highlight
+echo nautobot-secrets-providers >> local_requirements.txt
+```
+
+Once installed, the plugin needs to be enabled in your `nautobot_config.py`:
+
+```python
+# In your nautobot_config.py
+PLUGINS = ["nautobot_secrets_providers"]
+
+# PLUGINS_CONFIG = {
+#   "nautobot_secrets_providers": {
+#      See below for how to configure Nautobot for each secrets provider!
+#   }
+# }
+```
+
+## Usage
+
+Before you proceed, you must have **at least one** of the dependent libaries installed as detailed above.
+
+Please do not enable this plugin until you are able to install the dependencies, as it will block Nautobot from starting.
+
+### AWS
+
+#### Authentication
+
+No configuration is needed within Nautobot for this provider to operate. Instead you must provide [AWS credentials in one of the methods supported by the `boto3` library](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html#configuring-credentials).
+
+Boto3 credentials can be configured in multiple ways (eight as of this writing) that are mirrored here:
+
+1. Passing credentials as parameters in the `boto.client()` method
+2. Passing credentials as parameters when creating a Session object
+3. Environment variables
+4. Shared credential file (`~/.aws/credentials`)
+5. AWS config file (`~/.aws/config`)
+6. Assume Role provider
+7. Boto2 config file (`/etc/boto.cfg` and `~/.boto`)
+8. Instance metadata service on an Amazon EC2 instance that has an IAM role configured.
+
+**The AWS providers only support methods 3-8. Methods 1 and 2 ARE NOT SUPPORTED at this time.**
+
+We highly recommend you defer to using environment variables for your deployment as specified in the credentials documentation linked above. The values specified in the linked documentation should be [set within your `~.bashrc`](https://nautobot.readthedocs.io/en/latest/installation/nautobot/#update-the-nautobot-bashrc) (or similar profile) on your system.
+
+#### Configuration
+
+This is an example based on our recommended deployment pattern in the section above (item 3) that is using [environment variables](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html#environment-variables). You will need to set these in the environment prior to starting Nautobot:
+
+```no-highlight
+export AWS_ACCESS_KEY_ID=foo      # The access key for your AWS account.
+export AWS_SECRET_ACCESS_KEY=bar  # The secret key for your AWS account.
+```
+
+Please refer to the [Nautobot documentation on updating your `.bashrc`](https://nautobot.readthedocs.io/en/latest/installation/nautobot/#update-the-nautobot-bashrc) for how to do this for production Nautobot deployments.
+
+### HashiCorp Vault
+
+#### Configuration
+
+You must provide a mapping in `PLUGINS_CONFIG` within your `nautobot_config.py`, for example:
+
+```python
+PLUGINS_CONFIG = {
+    "nautobot_secrets_providers": {
+        "hashicorp_vault": {
+            "url": "http://localhost:8200",
+            "auth_method": "token",
+            "token": os.getenv("NAUTOBOT_HASHICORP_VAULT_TOKEN"),
+        }
+    },
 }
+```
+
+- `url` - (required) The URL to the HashiCorp Vault instance (e.g. `http://localhost:8200`).
+- `auth_method` - (optional / defaults to "token") The method used to authenticate against the HashiCorp Vault instance. Either `"approle"`, `"aws"`, `"kubernetes"` or `"token"`.  For information on using AWS authentication with vault see the [authentication](#authentication) section above.
+- `ca_cert` - (optional) Path to a PEM formatted CA certificate to use when verifying the Vault connection.  Can alternatively be set to `False` to ignore SSL verification (not recommended) or `True` to use the system certificates.
+- `default_mount_point` - (optional / defaults to "secret") The default mount point of the K/V Version 2 secrets engine within Hashicorp Vault.
+- `kv_version` - (optional / defaults to "v2") The version of the KV engine to use, can be `v1` or `v2`
+- `k8s_token_path` - (optional) Path to the kubernetes service account token file.  Defaults to "/var/run/secrets/kubernetes.io/serviceaccount/token".
+- `token` - (optional) Required when `"auth_method": "token"` or `auth_method` is not supplied. The token for authenticating the client with the HashiCorp Vault instance. As with other sensitive service credentials, we recommend that you provide the token value as an environment variable and retrieve it with `{"token": os.getenv("NAUTOBOT_HASHICORP_VAULT_TOKEN")}` rather than hard-coding it in your `nautobot_config.py`.
+- `role_name` - (optional) Required when `"auth_method": "kubernetes"`, optional when `"auth_method": "aws"`.  The Vault Kubernetes role or Vault AWS role to assume which the pod's service account has access to.
+- `role_id` - (optional) Required when `"auth_method": "approle"`. As with other sensitive service credentials, we recommend that you provide the role_id value as an environment variable and retrieve it with `{"role_id": os.getenv("NAUTOBOT_HASHICORP_VAULT_ROLE_ID")}` rather than hard-coding it in your `nautobot_config.py`.
+- `secret_id` - (optional) Required when `"auth_method": "approle"`.As with other sensitive service credentials, we recommend that you provide the secret_id value as an environment variable and retrieve it with `{"secret_id": os.getenv("NAUTOBOT_HASHICORP_VAULT_SECRET_ID")}` rather than hard-coding it in your `nautobot_config.py`.
+- `login_kwargs` - (optional) Additional optional parameters to pass to the login method for [`approle`](https://hvac.readthedocs.io/en/stable/source/hvac_api_auth_methods.html#hvac.api.auth_methods.AppRole.login), [`aws`](https://hvac.readthedocs.io/en/stable/source/hvac_api_auth_methods.html#hvac.api.auth_methods.Aws.iam_login) and [`kubernetes`](https://hvac.readthedocs.io/en/stable/source/hvac_api_auth_methods.html#hvac.api.auth_methods.Kubernetes.login) authentication methods.
+- `namespace` - (optional) Namespace to use for the [`X-Vault-Namespace` header](https://github.com/hvac/hvac/blob/main/hvac/adapters.py#L287) on all hvac client requests. Required when the [`Namespaces`](https://developer.hashicorp.com/vault/docs/enterprise/namespaces#usage) feature is enabled in Vault Enterprise.
+ 
+### Delinea/Thycotic Secret Server (TSS)
+
+The Delinea/Thycotic Secret Server plugin includes two providers:
+
+- **`Thycotic Secret Server by ID`**
+
+    This provider uses the `Secret ID` to specifiy the secret that is selected. The `Secret ID` is displayed in the browser's URL field if you `Edit` the data in Thycotic Secret Server.
+
+    - Example:
+
+        The url is: _https://pw.example.local/SecretServer/app/#/secret/**1234**/general_
+
+        In this example the value for `Secret ID` is **1234**.
+
+- **`Thycotic Secret Server by Path`**
+
+    This provider allows to select the secret by folder-path and secret-name. The path delimiter is a '\\'.
+
+    The `Secret path` is displayed as page header when `Edit` a secret.
+
+    - Example:
+
+        The header is: **NET-Automation > Nautobot > My-Secret**
+
+        In this example the value for `Secret path` is **`\NET-Automation\Nautobot\My-Secret`**.
+
+#### Configuration
+
+```python
+PLUGINS_CONFIG = {
+    "nautobot_secrets_providers": {
+        "thycotic": {  # https://github.com/thycotic/python-tss-sdk
+            "base_url": os.getenv("SECRET_SERVER_BASE_URL", None),
+            "ca_bundle_path": os.getenv("REQUESTS_CA_BUNDLE", None),
+            "cloud_based": is_truthy(os.getenv("SECRET_SERVER_IS_CLOUD_BASED", "False")),
+            "domain": os.getenv("SECRET_SERVER_DOMAIN", None),
+            "password": os.getenv("SECRET_SERVER_PASSWORD", None),
+            "tenant": os.getenv("SECRET_SERVER_TENANT", None),
+            "token": os.getenv("SECRET_SERVER_TOKEN", None),
+            "username": os.getenv("SECRET_SERVER_USERNAME", None),
+        },
+    }
+}
+```
+- `base_url` - (required) The Secret Server base_url. _e.g.'https://pw.example.local/SecretServer'_
+- `ca_bundle_path` - (optional) When using self-signed certificates this variable must be set to a file containing the trusted certificates (in .pem format). _e.g. '/etc/ssl/certs/ca-bundle.trust.crt'_.
+- `cloud_based` - (optional) Set to "True" if Secret Server Cloud should be used. (Default: "False").
+- `domain` - (optional) Required for 'Domain Authorization'
+- `password` - (optional) Required for 'Secret Server Cloud', 'Password Authorization', 'Domain Authorization'.
+- `tenant` - (optional) Required for 'Domain Authorization'.
+- `token` - (optional) Required for 'Access Token Authorization'.
+- `username` - (optional) Required for 'Secret Server Cloud', 'Password Authorization', 'Domain Authorization'.
+
+## Contributing
+
+Pull requests are welcomed and automatically built and tested against multiple version of Python and multiple version of Nautobot through GitHub Actions.
+
+The project is packaged with a light development environment based on `docker-compose` to help with the local development of the project and to run the tests within GitHub Actions.
+
+The project is following Network to Code software development guidelines and is leveraging:
+
+- Black, Pylint, Bandit and pydocstyle for Python linting and formatting.
+- Django unit test to ensure the plugin is working properly.
+
+### Development Environment
+
+The development environment can be used in 2 ways. First, with a local poetry environment if you wish to develop outside of Docker with the caveat of using external services provided by Docker for PostgreSQL and Redis. Second, all services are spun up using Docker and a local mount so you can develop locally, but Nautobot is spun up within the Docker container.
+
+Below is a quick start guide if you're already familiar with the development environment provided, but if you're not familiar, please read the [Getting Started Guide](GETTING_STARTED.md).
+
+#### Invoke
+
+The [PyInvoke](http://www.pyinvoke.org/) library is used to provide some helper commands based on the environment.  There are a few configuration parameters which can be passed to PyInvoke to override the default configuration:
+
+* `nautobot_ver`: the version of Nautobot to use as a base for any built docker containers (default: 1.4.10)
+* `project_name`: the default docker compose project name (default: nautobot_secrets_providers)
+* `python_ver`: the version of Python to use as a base for any built docker containers (default: 3.7)
+* `local`: a boolean flag indicating if invoke tasks should be run on the host or inside the docker containers (default: False, commands will be run in docker containers)
+* `compose_dir`: the full path to a directory containing the project compose files
+* `compose_files`: a list of compose files applied in order (see [Multiple Compose files](https://docs.docker.com/compose/extends/#multiple-compose-files) for more information)
+
+Using **PyInvoke** these configuration options can be overridden using [several methods](http://docs.pyinvoke.org/en/stable/concepts/configuration.html).  Perhaps the simplest is simply setting an environment variable `INVOKE_NAUTOBOT_SECRETS_PROVIDERS_VARIABLE_NAME` where `VARIABLE_NAME` is the variable you are trying to override.  The only exception is `compose_files`, because it is a list it must be overridden in a yaml file.  There is an example `invoke.yml` (`invoke.example.yml`) in this directory which can be used as a starting point.
+
+#### Local Poetry Development Environment
+
+1. Copy `development/creds.example.env` to `development/creds.env` (This file will be ignored by Git and Docker)
+2. Uncomment the `POSTGRES_HOST`, `REDIS_HOST`, and `NAUTOBOT_ROOT` variables in `development/creds.env`
+3. Create an `invoke.yml` file with the following contents at the root of the repo (you can also `cp invoke.example.yml invoke.yml` and edit as necessary):
+
+```yaml
+---
+nautobot_secrets_providers:
+  local: true
+  compose_files:
+    - "docker-compose.requirements.yml"
+```
+
+3. Run the following commands:
+
+```shell
+poetry shell
+poetry install --extras nautobot
+export $(cat development/dev.env | xargs)
+export $(cat development/creds.env | xargs)
+invoke start && sleep 5
+nautobot-server migrate
+```
+
+> If you want to develop on the latest develop branch of Nautobot, run the following command: `poetry add --optional git+https://github.com/nautobot/nautobot@develop`. After the `@` symbol must match either a branch or a tag.
+
+4. You can now run nautobot-server commands as you would from the [Nautobot documentation](https://nautobot.readthedocs.io/en/latest/) for example to start the development server:
+
+```shell
+nautobot-server runserver 0.0.0.0:8080 --insecure
+```
+
+Nautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).
+
+It is typically recommended to launch the Nautobot **runserver** command in a separate shell so you can keep developing and manage the webserver separately.
+
+#### Docker Development Environment
+
+This project is managed by [Python Poetry](https://python-poetry.org/) and has a few requirements to setup your development environment:
+
+1. Install Poetry, see the [Poetry Documentation](https://python-poetry.org/docs/#installation) for your operating system.
+2. Install Docker, see the [Docker documentation](https://docs.docker.com/get-docker/) for your operating system.
+
+Once you have Poetry and Docker installed you can run the following commands to install all other development dependencies in an isolated python virtual environment:
+
+```shell
+poetry shell
+poetry install
+invoke start
+```
+
+Nautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).
+
+To either stop or destroy the development environment use the following options.
+
+- **invoke stop** - Stop the containers, but keep all underlying systems intact
+- **invoke destroy** - Stop and remove all containers, volumes, etc. (This results in data loss due to the volume being deleted)
+
+### CLI Helper Commands
+
+The project is coming with a CLI helper based on [invoke](http://www.pyinvoke.org/) to help setup the development environment. The commands are listed below in 3 categories `dev environment`, `utility` and `testing`.
+
+Each command can be executed with `invoke <command>`. Environment variables `INVOKE_NAUTOBOT_SECRETS_PROVIDERS_PYTHON_VER` and `INVOKE_NAUTOBOT_SECRETS_PROVIDERS_NAUTOBOT_VER` may be specified to override the default versions. Each command also has its own help `invoke <command> --help`
+
+#### Docker dev environment
+
+```no-highlight
+  build            Build all docker images.
+  debug            Start Nautobot and its dependencies in debug mode.
+  destroy          Destroy all containers and volumes.
+  restart          Restart Nautobot and its dependencies.
+  start            Start Nautobot and its dependencies in detached mode.
+  stop             Stop Nautobot and its dependencies.
+```
+
+#### Utility
+
+```no-highlight
+  cli              Launch a bash shell inside the running Nautobot container.
+  create-user      Create a new user in django (default: admin), will prompt for password.
+  makemigrations   Run Make Migration in Django.
+  nbshell          Launch a nbshell session.
+```
+
+#### Testing
+
+```no-highlight
+  bandit           Run bandit to validate basic static code security analysis.
+  black            Run black to check that Python files adhere to its style standards.
+  flake8           This will run flake8 for the specified name and Python version.
+  pydocstyle       Run pydocstyle to validate docstring formatting adheres to NTC defined standards.
+  pylint           Run pylint code analysis.
+  tests            Run all tests for this plugin.
+  unittest         Run Django unit tests for the plugin.
+```
+
+### Project Documentation
+
+Project documentation is generated by [mkdocs](https://www.mkdocs.org/) from the documentation located in the docs folder.  You can configure [readthedocs.io](https://readthedocs.io/) to point at this folder in your repo.  For development purposes a `docker-compose.docs.yml` is also included.  A container hosting the docs will be started using the invoke commands on [http://localhost:8001](http://localhost:8001), as changes are saved the docs will be automatically reloaded.
+
+### Developing Against Secrets Backends
+
+#### AWS Secrets Manager
+
+This assumes you are logged into the AWS Console.
+
+- Navigate to AWS Console
+- Navigate to AWS Secrets Manager
+- Click "Store a new secret"
+  - Select “Other type of secrets”
+  - Use Secret key/value
+  - Enter `hello=world`
+  - Use "DefaultEncryptionKey" for now
+  - Click "Next"
+  - Under "Secret name" fill out `hello`
+  - Click "Next"
+  - Under "Configure automatic rotation"
+    - Leave it as "Disable automatic rotation"
+  - On "Store a new secret"
+    - Copy the sample code (see below)
+  - Click "Store"
+- END
+
+##### Install the AWS CLI
+
+Next, install the [AWS CLI](https://aws.amazon.com/cli/).
+
+On MacOS, this can be done using `brew install awscli`:
+
+```
+brew install awscli
+```
+
+On Linux, you will need to run a `curl` command (This assumes x86. Please see the docs for [AWS CLI on
+Linux](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2-linux.html) for ARM and other options):
+
+```
+curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
+unzip awscliv2.zip
+sudo ./aws/install
+```
+
+##### Configure the AWS CLI
+
+After installing the AWS CLI, you will need to configure it for authentication.
+
+You may use an existing AWS access key or create a new one. For these instructions we cover the need to create a new access key that can be used for this.
+
+- Navigate to AWS Console
+- Click your username
+  - Click "My security credentials"
+  - Click "create access key"
+- Save your "Access key ID" and "Secret access key" for use when configuring the AWS CLI
+
+Now configure the CLI:
+
+- Run `aws configure`
+- Enter your credentials from above
+- Choose your region
+- Use output format: `json`
+
+Example:
+
+```no-highlight
+$ aws configure
+AWS Access Key ID [None]: AKIAIOSFODNN7EXAMPLE
+AWS Secret Access Key [None]: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
+Default region name [None]: us-east-2
+Default output format [None]: json
+```
+
+Now you are ready to use the sample code to retrieve your secret from AWS Secrets Manager!
+
+##### Sample Code
+
+Make sure that the `boto3` client is installed:
+
+```no-highlight
+poetry install --extras aws
+```
+
+Next, save this as `aws_secrets.py`:
+
+```python
+# Use this code snippet in your app.
+# If you need more information about configurations or implementing the sample code, visit the AWS docs:
+# https://aws.amazon.com/developers/getting-started/python/
+
+import boto3
+import base64
+from botocore.exceptions import ClientError
+
+
+def get_secret():
+
+    secret_name = "hello"
+    region_name = "us-east-2"
+
+    # Create a Secrets Manager client
+    session = boto3.session.Session()
+    client = session.client(
+        service_name='secretsmanager',
+        region_name=region_name
+    )
+
+    # In this sample we only handle the specific exceptions for the 'GetSecretValue' API.
+    # See https://docs.aws.amazon.com/secretsmanager/latest/apireference/API_GetSecretValue.html
+    # We rethrow the exception by default.
+
+    try:
+        get_secret_value_response = client.get_secret_value(
+            SecretId=secret_name
+        )
+    except ClientError as e:
+        if e.response['Error']['Code'] == 'DecryptionFailureException':
+            # Secrets Manager can't decrypt the protected secret text using the provided KMS key.
+            # Deal with the exception here, and/or rethrow at your discretion.
+            raise e
+        elif e.response['Error']['Code'] == 'InternalServiceErrorException':
+            # An error occurred on the server side.
+            # Deal with the exception here, and/or rethrow at your discretion.
+            raise e
+        elif e.response['Error']['Code'] == 'InvalidParameterException':
+            # You provided an invalid value for a parameter.
+            # Deal with the exception here, and/or rethrow at your discretion.
+            raise e
+        elif e.response['Error']['Code'] == 'InvalidRequestException':
+            # You provided a parameter value that is not valid for the current state of the resource.
+            # Deal with the exception here, and/or rethrow at your discretion.
+            raise e
+        elif e.response['Error']['Code'] == 'ResourceNotFoundException':
+            # We can't find the resource that you asked for.
+            # Deal with the exception here, and/or rethrow at your discretion.
+            raise e
+    else:
+        # Decrypts secret using the associated KMS CMK.
+        # Depending on whether the secret is a string or binary, one of these fields will be populated.
+        if 'SecretString' in get_secret_value_response:
+            secret = get_secret_value_response['SecretString']
+        else:
+            decoded_binary_secret = base64.b64decode(get_secret_value_response['SecretBinary'])
+
+    # Your code goes here.
+
+# ^ Above was generated by AWS.
+
+# This was added by us so you can run this as a script:
+if __name__ == "__main__":
+    secret = get_secret()
+    print(f"Secret = {secret}")
+```
+
+Run it with `python aws_secrets.py`:
+
+```
+$ python aws_secrets.py
+Secret = {"hello":"world"}.
+```
+
+Note that this blob is JSON and will also need to be decoded if you want to extract the value.
+
+#### HashiCorp Vault
+
+Make sure that the `hvac` client is installed:
+
+```no-highlight
+poetry install --extras hashicorp
+```
+
+##### Start Services with Docker
+
+```no-highlight
+invoke start
+```
+
+##### Set an alias to work with `vault`
+
+This will allow you to easily run the CLI command from within the container:
+
+```no-highlight
+alias vault="docker exec -it nautobot_secrets_providers_vault_1 vault"
+```
+
+Interact with the Vault vi CLI (via `docker exec` into the container from localhost):
+
+```no-highlight
+$ vault status
+Key             Value
+---             -----
+Seal Type       shamir
+Initialized     true
+Sealed          false
+Total Shares    1
+Threshold       1
+Version         1.8.2
+Storage Type    inmem
+Cluster Name    vault-cluster-35c5d319
+Cluster ID      2611f99c-a6de-a883-1fcc-bfffdc0217bc
+HA Enabled      false
+```
+
+##### Using the Python `hvac` Library
+
+This establishes a client, creates a basic key/value secret (`hello=world`) at the path `hello`, and then retrieves the data from the `hello` key at the secret path `hello`.
+
+> This is equivalent to the command `vault kv get -field hello secret/hello`.
+
+```python
+In [1]: import hvac
+
+In [2]: client = hvac.Client(url="http://localhost:8200", token="nautobot")
+
+In [3]: client.secrets.kv.create_or_update_secret(path="hello", secret=dict(hello="world"))
+Out[3]:
+{'request_id': 'c4709868-c08f-4cb1-ab8c-605c58b82f3f',
+ 'lease_id': '',
+ 'renewable': False,
+ 'lease_duration': 0,
+ 'data': {'created_time': '2021-09-16T23:21:07.5564132Z',
+  'deletion_time': '',
+  'destroyed': False,
+  'version': 2},
+ 'wrap_info': None,
+ 'warnings': None,
+ 'auth': None}
+
+In [4]: client.secrets.kv.read_secret(path="hello")["data"]["data"]["hello"]
+Out[4]: 'world'
+```
+
+## Questions
 
+For any questions or comments, please check the [FAQ](FAQ.md) first and feel free to swing by the [Network to Code Slack workspace](https://networktocode.slack.com/) (channel `#networktocode`).
 
-setup(**setup_kwargs)
```

