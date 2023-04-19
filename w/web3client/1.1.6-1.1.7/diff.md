# Comparing `tmp/web3client-1.1.6.tar.gz` & `tmp/web3client-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3client-1.1.6.tar", last modified: Mon Apr 17 17:03:14 2023, max compression
+gzip compressed data, was "web3client-1.1.7.tar", last modified: Wed Apr 19 13:32:38 2023, max compression
```

## Comparing `web3client-1.1.6.tar` & `web3client-1.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1069 2022-10-13 15:30:24.076003 web3client-1.1.6/LICENSE
--rw-r--r--   0        0        0     2757 2023-04-17 14:56:39.469040 web3client-1.1.6/README.md
--rw-r--r--   0        0        0     1983 2023-04-17 17:03:00.093123 web3client-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.879656 web3client-1.1.6/src/.DS_Store
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:28.884980 web3client-1.1.6/src/web3client/.DS_Store
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.603558 web3client-1.1.6/src/web3client/__init__.py
--rw-r--r--   0        0        0    11117 2022-10-18 14:47:37.604295 web3client-1.1.6/src/web3client/abi/erc20.json
--rw-r--r--   0        0        0    24512 2023-04-17 17:02:11.554007 web3client-1.1.6/src/web3client/base_client.py
--rw-r--r--   0        0        0     3320 2023-04-05 16:33:33.363845 web3client-1.1.6/src/web3client/erc20_client.py
--rw-r--r--   0        0        0      342 2022-10-19 17:40:52.208885 web3client-1.1.6/src/web3client/exceptions.py
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.604873 web3client-1.1.6/src/web3client/helpers/__init__.py
--rw-r--r--   0        0        0     1732 2023-02-13 20:06:35.817499 web3client-1.1.6/src/web3client/helpers/debug.py
--rw-r--r--   0        0        0     2438 2022-10-18 14:47:37.605628 web3client-1.1.6/src/web3client/helpers/general.py
--rw-r--r--   0        0        0     1909 2023-04-10 15:26:30.878490 web3client-1.1.6/src/web3client/helpers/websockets.py
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.601242 web3client-1.1.6/src/web3factory/__init__.py
--rw-r--r--   0        0        0     2190 2023-04-05 13:58:18.268337 web3client-1.1.6/src/web3factory/erc20_tokens.py
--rw-r--r--   0        0        0     1431 2023-02-13 20:30:39.832108 web3client-1.1.6/src/web3factory/factory.py
--rw-r--r--   0        0        0     2770 2023-04-17 14:56:39.482576 web3client-1.1.6/src/web3factory/networks.py
--rw-r--r--   0        0        0      621 2023-02-13 19:47:49.818983 web3client-1.1.6/src/web3factory/types.py
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.878800 web3client-1.1.6/tests/.DS_Store
--rw-r--r--   0        0        0        0 2023-02-23 10:04:23.399090 web3client-1.1.6/tests/__init__.py
--rw-r--r--   0        0        0     6148 2023-04-05 16:39:49.642961 web3client-1.1.6/tests/ape/.DS_Store
--rw-r--r--   0        0        0      779 2023-04-06 10:47:11.288879 web3client-1.1.6/tests/ape/.build/SafeMath.json
--rw-r--r--   0        0        0    14895 2023-04-06 10:47:11.290250 web3client-1.1.6/tests/ape/.build/Token.json
--rw-r--r--   0        0        0    20923 2023-04-17 17:03:05.043749 web3client-1.1.6/tests/ape/.build/__local__.json
--rw-r--r--   0        0        0      600 2023-02-23 10:18:28.269673 web3client-1.1.6/tests/ape/contracts/token/SafeMath.sol
--rw-r--r--   0        0        0     4082 2023-02-23 10:18:28.283242 web3client-1.1.6/tests/ape/contracts/token/Token.sol
--rw-r--r--   0        0        0     3529 2023-04-05 16:42:52.576613 web3client-1.1.6/tests/ape/fixtures.py
--rw-r--r--   0        0        0        0 2023-04-05 15:27:07.832128 web3client-1.1.6/tests/ape/scripts/__init__.py
--rw-r--r--   0        0        0      123 2023-04-05 14:37:05.616337 web3client-1.1.6/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-02-23 10:04:38.139397 web3client-1.1.6/tests/web3client/__init__.py
--rw-r--r--   0        0        0     1300 2023-04-06 11:08:05.647477 web3client-1.1.6/tests/web3client/fixtures.py
--rw-r--r--   0        0        0     1417 2023-02-13 20:04:46.649348 web3client-1.1.6/tests/web3client/test_networks.py
--rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 web3client-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-13 15:30:24.076003 web3client-1.1.7/LICENSE
+-rw-r--r--   0        0        0     2757 2023-04-17 14:56:39.469040 web3client-1.1.7/README.md
+-rw-r--r--   0        0        0     1983 2023-04-19 13:32:03.882839 web3client-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.879656 web3client-1.1.7/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:28.884980 web3client-1.1.7/src/web3client/.DS_Store
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.603558 web3client-1.1.7/src/web3client/__init__.py
+-rw-r--r--   0        0        0    11117 2022-10-18 14:47:37.604295 web3client-1.1.7/src/web3client/abi/erc20.json
+-rw-r--r--   0        0        0    24640 2023-04-19 12:54:16.926188 web3client-1.1.7/src/web3client/base_client.py
+-rw-r--r--   0        0        0     4436 2023-04-19 12:51:51.450776 web3client-1.1.7/src/web3client/erc20_client.py
+-rw-r--r--   0        0        0      342 2022-10-19 17:40:52.208885 web3client-1.1.7/src/web3client/exceptions.py
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.604873 web3client-1.1.7/src/web3client/helpers/__init__.py
+-rw-r--r--   0        0        0     1732 2023-02-13 20:06:35.817499 web3client-1.1.7/src/web3client/helpers/debug.py
+-rw-r--r--   0        0        0     2438 2022-10-18 14:47:37.605628 web3client-1.1.7/src/web3client/helpers/general.py
+-rw-r--r--   0        0        0     1909 2023-04-10 15:26:30.878490 web3client-1.1.7/src/web3client/helpers/websockets.py
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.601242 web3client-1.1.7/src/web3factory/__init__.py
+-rw-r--r--   0        0        0     2190 2023-04-05 13:58:18.268337 web3client-1.1.7/src/web3factory/erc20_tokens.py
+-rw-r--r--   0        0        0     1431 2023-02-13 20:30:39.832108 web3client-1.1.7/src/web3factory/factory.py
+-rw-r--r--   0        0        0     2770 2023-04-17 14:56:39.482576 web3client-1.1.7/src/web3factory/networks.py
+-rw-r--r--   0        0        0      621 2023-02-13 19:47:49.818983 web3client-1.1.7/src/web3factory/types.py
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.878800 web3client-1.1.7/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2023-02-23 10:04:23.399090 web3client-1.1.7/tests/__init__.py
+-rw-r--r--   0        0        0     6148 2023-04-05 16:39:49.642961 web3client-1.1.7/tests/ape/.DS_Store
+-rw-r--r--   0        0        0      779 2023-04-06 10:47:11.288879 web3client-1.1.7/tests/ape/.build/SafeMath.json
+-rw-r--r--   0        0        0    14895 2023-04-06 10:47:11.290250 web3client-1.1.7/tests/ape/.build/Token.json
+-rw-r--r--   0        0        0    20923 2023-04-19 13:32:09.817791 web3client-1.1.7/tests/ape/.build/__local__.json
+-rw-r--r--   0        0        0      600 2023-02-23 10:18:28.269673 web3client-1.1.7/tests/ape/contracts/token/SafeMath.sol
+-rw-r--r--   0        0        0     4082 2023-02-23 10:18:28.283242 web3client-1.1.7/tests/ape/contracts/token/Token.sol
+-rw-r--r--   0        0        0     3529 2023-04-05 16:42:52.576613 web3client-1.1.7/tests/ape/fixtures.py
+-rw-r--r--   0        0        0        0 2023-04-05 15:27:07.832128 web3client-1.1.7/tests/ape/scripts/__init__.py
+-rw-r--r--   0        0        0      123 2023-04-05 14:37:05.616337 web3client-1.1.7/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-02-23 10:04:38.139397 web3client-1.1.7/tests/web3client/__init__.py
+-rw-r--r--   0        0        0     1300 2023-04-06 11:08:05.647477 web3client-1.1.7/tests/web3client/fixtures.py
+-rw-r--r--   0        0        0     1417 2023-02-13 20:04:46.649348 web3client-1.1.7/tests/web3client/test_networks.py
+-rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 web3client-1.1.7/PKG-INFO
```

### Comparing `web3client-1.1.6/LICENSE` & `web3client-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/README.md` & `web3client-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/pyproject.toml` & `web3client-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "web3client"
-version = "1.1.6"
+version = "1.1.7"
 description = "Batteries-included client to interact with blockchains and smart contracts"
 authors = [
     { name = "coccoinomane", email = "coccoinomane@gmail.com" },
 ]
 readme = "README.md"
 keywords = [
     "web3",
```

### Comparing `web3client-1.1.6/src/.DS_Store` & `web3client-1.1.7/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/src/web3client/.DS_Store` & `web3client-1.1.7/src/web3client/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/src/web3client/abi/erc20.json` & `web3client-1.1.7/src/web3client/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/src/web3client/base_client.py` & `web3client-1.1.7/src/web3client/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -557,17 +557,21 @@
                 "from": self.user_address,
                 "to": to,
                 "value": value_in_wei,
             }
         )
 
     def get_balance_in_wei(self, address: Address = None) -> Wei:
+        if not address:
+            address = self.user_address
         return self.w3.eth.get_balance(Web3.to_checksum_address(address))
 
     def get_balance_in_eth(self, address: Address = None) -> float:
+        if not address:
+            address = self.user_address
         return float(Web3.from_wei(self.get_balance_in_wei(address), "ether"))
 
     ####################
     # Contract
     ####################
 
     def call(
```

### Comparing `web3client-1.1.6/src/web3client/erc20_client.py` & `web3client-1.1.7/src/web3client/erc20_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 import os
+from functools import cached_property
 
 from eth_typing import Address, HexStr
 from web3 import Web3
-from web3.types import Nonce, TxParams, Wei
+from web3.types import Nonce, Wei
 
 from web3client.base_client import BaseClient
 
 
 class Erc20Client(BaseClient):
     """
     Client that comes with the ERC20 ABI preloaded.
 
-    Call the contract functions directly: transfer, balanceOf, name,
-    etc.
+    It allows you to call the contract functions as class methods:
+    transfer, balanceOf, name, etc.
+
+    If you pass  a private key, it will allow you to call the
+    write functions (transfer, approve, etc.)
+
+    The token properties (name, symbol, total_supply, decimals) can be
+    accessed as attributes, and will be fetched from the blockchain only
+    once.
 
     AMOUNTS
     =======
 
     Whenever we will refer to an "amount" of the token, we really mean an
-    "amount in token units". A token unit is the smallest subdivision of
-    the token. For example:
-    - If the token has 6 digits (like most stablecoins) an amount of 1
+    amount in the smallest subdivision of the token (e.g. wei). For example:
+    - If the token has 6 decimals (like most stablecoins) an amount of 1
       corresponds to one millionth of the token.
-    - For tokens with 18 digits (like most non-stablecoins) an amount
+    - For tokens with 18 decimals (like most non-stablecoins) an amount
       of 1 is equal to 1/10^18 of the token (a single wei).
     """
 
     abiDir = os.path.dirname(os.path.realpath(__file__)) + "/abi"
     abi = BaseClient.get_contract_abi_from_file(abiDir + "/erc20.json")
 
     def __init__(
@@ -35,14 +42,16 @@
         chain_id: int = None,
         tx_type: int = 2,
         private_key: str = None,
         max_priority_fee_in_gwei: float = 1,
         upper_limit_for_base_fee_in_gwei: float = float("inf"),
         contract_address: Address = None,
     ) -> None:
+        if not contract_address:
+            raise ValueError("You must specify a contract address")
         super().__init__(
             node_uri,
             chain_id,
             tx_type,
             private_key,
             max_priority_fee_in_gwei,
             upper_limit_for_base_fee_in_gwei,
@@ -58,61 +67,87 @@
         """
         Return the amount held by the given address
         """
         return self.contract.functions.balanceOf(
             Web3.to_checksum_address(address)
         ).call()
 
+    @cached_property
     def name(self) -> str:
         """
         Return the name/label of the token
         """
         return self.contract.functions.name().call()
 
+    @cached_property
     def symbol(self) -> str:
         """
         Return the symbol/ticker of the token
         """
         return self.contract.functions.symbol().call()
 
+    @cached_property
     def totalSupply(self) -> int:
         """
         Return the total supply of the token
         """
         return self.contract.functions.totalSupply().call()
 
+    @cached_property
     def decimals(self) -> int:
         """
         Return the number of digits of the token
         """
         return self.contract.functions.decimals().call()
 
     ####################
     # Write
     ####################
 
     def transfer(
-        self, to: Address, amount: int, nonce: Nonce = None, value_in_wei: Wei = Wei(0)
+        self,
+        to: Address,
+        amount: int,
+        value_in_wei: Wei = None,
+        nonce: Nonce = None,
+        gas_limit: int = None,
+        max_priority_fee_in_gwei: int = None,
     ) -> HexStr:
         """
         Transfer some amount of the token to an address; does not
         require approval.
         """
-
-        tx: TxParams = self.build_contract_tx(
-            self.contract.functions.transfer(Web3.to_checksum_address(to), amount)
+        return self.transact(
+            self.contract.functions.transfer(Web3.to_checksum_address(to), amount),
+            value_in_wei,
+            nonce,
+            gas_limit,
+            max_priority_fee_in_gwei,
         )
 
-        if nonce:
-            tx["nonce"] = nonce
-
-        if value_in_wei:
-            tx["value"] = value_in_wei
-
-        return self.sign_and_send_tx(tx)
+    def approve(
+        self,
+        spender: Address,
+        amount: int,
+        value_in_wei: Wei = None,
+        nonce: Nonce = None,
+        gas_limit: int = None,
+        max_priority_fee_in_gwei: int = None,
+    ) -> HexStr:
+        """
+        Approve the given address to spend some amount of the token
+        on behalf of the sender.
+        """
+        return self.transact(
+            self.contract.functions.approve(Web3.to_checksum_address(spender), amount),
+            value_in_wei,
+            nonce,
+            gas_limit,
+            max_priority_fee_in_gwei,
+        )
 
     ####################
     # Static
     ####################
 
     @staticmethod
     def from_wei(amount: int, decimals: int) -> float:
```

### Comparing `web3client-1.1.6/src/web3client/helpers/debug.py` & `web3client-1.1.7/src/web3client/helpers/debug.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/src/web3client/helpers/general.py` & `web3client-1.1.7/src/web3client/helpers/general.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/src/web3client/helpers/websockets.py` & `web3client-1.1.7/src/web3client/helpers/websockets.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/src/web3factory/erc20_tokens.py` & `web3client-1.1.7/src/web3factory/erc20_tokens.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/src/web3factory/factory.py` & `web3client-1.1.7/src/web3factory/factory.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/src/web3factory/networks.py` & `web3client-1.1.7/src/web3factory/networks.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/src/web3factory/types.py` & `web3client-1.1.7/src/web3factory/types.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/tests/.DS_Store` & `web3client-1.1.7/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/tests/ape/.DS_Store` & `web3client-1.1.7/tests/ape/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/tests/ape/.build/SafeMath.json` & `web3client-1.1.7/tests/ape/.build/SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/tests/ape/.build/Token.json` & `web3client-1.1.7/tests/ape/.build/Token.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/tests/ape/.build/__local__.json` & `web3client-1.1.7/tests/ape/.build/__local__.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/tests/ape/contracts/token/SafeMath.sol` & `web3client-1.1.7/tests/ape/contracts/token/SafeMath.sol`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/tests/ape/contracts/token/Token.sol` & `web3client-1.1.7/tests/ape/contracts/token/Token.sol`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/tests/ape/fixtures.py` & `web3client-1.1.7/tests/ape/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/tests/web3client/fixtures.py` & `web3client-1.1.7/tests/web3client/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/tests/web3client/test_networks.py` & `web3client-1.1.7/tests/web3client/test_networks.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.6/PKG-INFO` & `web3client-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3client
-Version: 1.1.6
+Version: 1.1.7
 Summary: Batteries-included client to interact with blockchains and smart contracts
 License: MIT
 Keywords: web3,blockchain,ethereum,evm
 Author-email: coccoinomane <coccoinomane@gmail.com>
 Requires-Python: >=3.9,<3.11
 Project-URL: homepage, https://github.com/coccoinomane/web3client
 Project-URL: repository, https://github.com/coccoinomane/web3client
```

