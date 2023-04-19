# Comparing `tmp/multiversx_sdk_network_providers-0.6.9.tar.gz` & `tmp/multiversx_sdk_network_providers-0.7.0.tar.gz`

## Comparing `multiversx_sdk_network_providers-0.6.9.tar` & `multiversx_sdk_network_providers-0.7.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/.flake8
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/py.typed
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/pyrightconfig.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/requirements-dev.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/requirements.txt
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/.github/workflows/linter-flake8.yml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/.github/workflows/linter-pyright.yml
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/.github/workflows/test.yml
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/__init__.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/accounts.py
--rw-r--r--   0        0        0     9394 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/api_network_provider.py
--rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/api_network_provider_test.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/config.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/constants.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/contract_query_requests.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/contract_query_response.py
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/contract_results.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/errors.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/interface.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/network_config.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/network_general_statistics.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/network_stake.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/network_status.py
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/proxy_network_provider.py
--rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/proxy_network_provider_test.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/resources.py
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/token_definitions.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/tokens.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/transaction_completion_strategy.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/transaction_events.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/transaction_logs.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/transaction_receipt.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/transaction_status.py
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/transactions.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/utils.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/LICENSE
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/pyproject.toml
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/.flake8
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/py.typed
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/pyrightconfig.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/requirements-dev.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/requirements.txt
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/.github/workflows/linter-flake8.yml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/.github/workflows/linter-pyright.yml
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/__init__.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/accounts.py
+-rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/api_network_provider.py
+-rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/api_network_provider_test.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/config.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/constants.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/contract_query_requests.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/contract_query_response.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/contract_results.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/errors.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/interface.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_config.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_general_statistics.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_stake.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_status.py
+-rw-r--r--   0        0        0    10488 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/proxy_network_provider.py
+-rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/proxy_network_provider_test.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/resources.py
+-rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/token_definitions.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/tokens.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_completion_strategy.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_events.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_logs.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_receipt.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_status.py
+-rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transactions.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/utils.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/PKG-INFO
```

### Comparing `multiversx_sdk_network_providers-0.6.9/.github/workflows/linter-flake8.yml` & `multiversx_sdk_network_providers-0.7.0/.github/workflows/linter-flake8.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/.github/workflows/linter-pyright.yml` & `multiversx_sdk_network_providers-0.7.0/.github/workflows/linter-pyright.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/.github/workflows/python-publish.yml` & `multiversx_sdk_network_providers-0.7.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/.github/workflows/test.yml` & `multiversx_sdk_network_providers-0.7.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/api_network_provider.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/api_network_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict, List, Tuple, Union, cast
 
 import requests
 from requests.auth import AuthBase
 
-from multiversx_sdk_network_providers.accounts import AccountOnNetwork
+from multiversx_sdk_network_providers.accounts import AccountOnNetwork, GuardianData
 from multiversx_sdk_network_providers.config import DefaultPagination
 from multiversx_sdk_network_providers.constants import DEFAULT_ADDRESS_HRP
 from multiversx_sdk_network_providers.contract_query_requests import ContractQueryRequest
 from multiversx_sdk_network_providers.contract_query_response import ContractQueryResponse
 from multiversx_sdk_network_providers.errors import GenericError
 from multiversx_sdk_network_providers.interface import (IAddress, IContractQuery, IPagination,
                                                         ITransaction)
@@ -33,14 +33,17 @@
 
     def get_network_config(self) -> NetworkConfig:
         return self.backing_proxy.get_network_config()
 
     def get_network_status(self) -> NetworkStatus:
         return self.backing_proxy.get_network_status()
 
+    def get_guardian_data(self, address: IAddress) -> GuardianData:
+        return self.backing_proxy.get_guardian_data(address)
+
     def get_network_stake_statistics(self) -> NetworkStake:
         response = self.do_get_generic('stake')
         network_stake = NetworkStake.from_http_response(response)
 
         return network_stake
 
     def get_network_general_statistics(self) -> NetworkGeneralStatistics:
```

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/api_network_provider_test.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/api_network_provider_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         assert len(result.return_data) == 1
 
     def test_get_definition_of_fungible_token(self):
         result = self.api.get_definition_of_fungible_token('ABC-10df96')
 
         assert result.identifier == 'ABC-10df96'
         assert result.owner.bech32() == 'erd1testnlersh4z0wsv8kjx39me4rmnvjkwu8dsaea7ukdvvc9z396qykv7z7'
-        assert result.can_upgrade
+        assert not result.can_upgrade
         assert not result.can_freeze
         assert result.decimals == 1
         assert result.supply == 5
 
     def test_get_definition_of_token_collection(self):
         result = self.api.get_definition_of_token_collection('ASDASD-510041')
```

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/contract_query_requests.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/contract_query_requests.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/contract_query_response.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/contract_query_response.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/contract_results.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/contract_results.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/interface.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/interface.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/network_config.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/network_general_statistics.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_general_statistics.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/network_stake.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_stake.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/network_status.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_status.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/proxy_network_provider.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/proxy_network_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import requests
 from requests.auth import AuthBase
 
-from multiversx_sdk_network_providers.accounts import AccountOnNetwork
+from multiversx_sdk_network_providers.accounts import AccountOnNetwork, GuardianData
 from multiversx_sdk_network_providers.constants import (DEFAULT_ADDRESS_HRP,
                                                         ESDT_CONTRACT_ADDRESS, METACHAIN_ID)
 from multiversx_sdk_network_providers.contract_query_requests import ContractQueryRequest
 from multiversx_sdk_network_providers.contract_query_response import ContractQueryResponse
 from multiversx_sdk_network_providers.errors import GenericError
 from multiversx_sdk_network_providers.interface import IAddress, IContractQuery, ITransaction
 from multiversx_sdk_network_providers.network_config import NetworkConfig
@@ -41,14 +41,20 @@
 
     def get_account(self, address: IAddress) -> AccountOnNetwork:
         response = self.do_get_generic(f'address/{address.bech32()}')
         account = AccountOnNetwork.from_http_response(response.get('account', ''))
 
         return account
 
+    def get_guardian_data(self, address: IAddress) -> GuardianData:
+        response = self.do_get_generic(f'address/{address.bech32()}/guardian-data')
+        account_guardian = GuardianData.from_http_response(response.get('guardianData', ''))
+
+        return account_guardian
+
     def get_fungible_tokens_of_account(self, address: IAddress) -> List[FungibleTokenOfAccountOnNetwork]:
         url = f'address/{address.bech32()}/esdt'
         response = self.do_get_generic(url)
         items = response.get('esdts')
         esdts = [items[key] for key in items.keys() if items[key].get('nonce', '') == '']
         tokens = map(FungibleTokenOfAccountOnNetwork.from_http_response, esdts)
```

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/proxy_network_provider_test.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/proxy_network_provider_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/resources.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/resources.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/token_definitions.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/token_definitions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/tokens.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/tokens.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/transaction_completion_strategy.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_completion_strategy.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/transaction_events.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_events.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/transaction_logs.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_logs.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/transaction_receipt.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_receipt.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/transaction_status.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_status.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/multiversx_sdk_network_providers/transactions.py` & `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transactions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/.gitignore` & `multiversx_sdk_network_providers-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/LICENSE` & `multiversx_sdk_network_providers-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/README.md` & `multiversx_sdk_network_providers-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.6.9/pyproject.toml` & `multiversx_sdk_network_providers-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "multiversx-sdk-network-providers"
-version = "0.6.9"
+version = "0.7.0"
 authors = [
   { name="MultiversX" },
 ]
 license = "MIT"
 description = "Network providers for MultiversX Python SDK."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `multiversx_sdk_network_providers-0.6.9/PKG-INFO` & `multiversx_sdk_network_providers-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiversx-sdk-network-providers
-Version: 0.6.9
+Version: 0.7.0
 Summary: Network providers for MultiversX Python SDK.
 Project-URL: Homepage, https://github.com/multiversx/mx-sdk-py-network-providers
 Author: MultiversX
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

