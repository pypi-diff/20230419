# Comparing `tmp/python_seller_active-0.0.3.tar.gz` & `tmp/python_seller_active-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_seller_active-0.0.3.tar", last modified: Thu Feb 16 18:18:10 2023, max compression
+gzip compressed data, was "python_seller_active-0.0.4.tar", last modified: Wed Apr 19 07:16:08 2023, max compression
```

## Comparing `python_seller_active-0.0.3.tar` & `python_seller_active-0.0.4.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:18:10.933637 python_seller_active-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-02-16 18:18:10.933637 python_seller_active-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:18:10.933637 python_seller_active-0.0.3/python_seller_active.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-02-16 18:18:10.000000 python_seller_active-0.0.3/python_seller_active.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-02-16 18:18:10.000000 python_seller_active-0.0.3/python_seller_active.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 18:18:10.000000 python_seller_active-0.0.3/python_seller_active.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-16 18:18:10.000000 python_seller_active-0.0.3/python_seller_active.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-16 18:18:10.000000 python_seller_active-0.0.3/python_seller_active.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:18:10.933637 python_seller_active-0.0.3/seller_active/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/__info__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:18:10.933637 python_seller_active-0.0.3/seller_active/api/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:18:10.933637 python_seller_active-0.0.3/seller_active/api/bundles/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/api/bundles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/api/bundles/bundles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:18:10.933637 python_seller_active-0.0.3/seller_active/api/inventory/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/api/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/api/inventory/inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:18:10.933637 python_seller_active-0.0.3/seller_active/api/locations/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/api/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/api/locations/locations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:18:10.933637 python_seller_active-0.0.3/seller_active/api/orders/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/api/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/api/orders/orders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:18:10.933637 python_seller_active-0.0.3/seller_active/api/rate_limit_status/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/api/rate_limit_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/api/rate_limit_status/rate_limit_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:18:10.933637 python_seller_active-0.0.3/seller_active/base/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/base/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/seller_active/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-16 18:18:10.933637 python_seller_active-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-02-16 18:17:54.000000 python_seller_active-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.658428 python_seller_active-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-19 07:16:08.658428 python_seller_active-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/python_seller_active.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-19 07:16:08.000000 python_seller_active-0.0.4/python_seller_active.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-19 07:16:08.000000 python_seller_active-0.0.4/python_seller_active.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 07:16:08.000000 python_seller_active-0.0.4/python_seller_active.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 07:16:08.000000 python_seller_active-0.0.4/python_seller_active.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 07:16:08.000000 python_seller_active-0.0.4/python_seller_active.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/seller_active/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/seller_active/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/seller_active/api/bundles/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/bundles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/bundles/bundles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/seller_active/api/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/inventory/inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/seller_active/api/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/locations/locations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/seller_active/api/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/orders/orders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/seller_active/api/rate_limit_status/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/rate_limit_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/rate_limit_status/rate_limit_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.658428 python_seller_active-0.0.4/seller_active/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/base/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-19 07:16:08.658428 python_seller_active-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/setup.py
```

### Comparing `python_seller_active-0.0.3/LICENSE` & `python_seller_active-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_seller_active-0.0.3/PKG-INFO` & `python_seller_active-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: python_seller_active
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wrapper around SellerActive.com API
 Home-page: https://github.com/yberezkin/python_seller_active
 Author: Yan Berezkin
 Author-email: yan.berezkin@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yberezkin/python_seller_active/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SELLER-ACTIVE-API Python Wrapper
 
+[![CodeFactor](https://www.codefactor.io/repository/github/yberezkin/python_seller_active/badge)](https://www.codefactor.io/repository/github/yberezkin/python_seller_active)
+
 This project provides a Python wrapper for interacting with the [rest.selleractive.com](https://rest.selleractive.com/) API, allowing developers to easily integrate the API's functionality into their Python applications.
 
 ## Getting Started
 
 These instructions will give you a copy of the project up and running on
 your local machine for development and testing purposes. See deployment
 for notes on deploying the project on a live system.
 
 ### Installing
 
-[//]: # ([![Badge]&#40;https://img.shields.io/pypi/v/pytho?style=for-the-badge&#41;]&#40;https://pypi.org/project/xsellco-api/&#41;)
+[![Badge](https://img.shields.io/pypi/v/python_seller_active?style=for-the-badge)](https://pypi.org/project/python-seller-active/)
 
 
     pip install python_seller_active
 
 
 ---
```

### Comparing `python_seller_active-0.0.3/README.md` & `python_seller_active-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # SELLER-ACTIVE-API Python Wrapper
 
+[![CodeFactor](https://www.codefactor.io/repository/github/yberezkin/python_seller_active/badge)](https://www.codefactor.io/repository/github/yberezkin/python_seller_active)
+
 This project provides a Python wrapper for interacting with the [rest.selleractive.com](https://rest.selleractive.com/) API, allowing developers to easily integrate the API's functionality into their Python applications.
 
 ## Getting Started
 
 These instructions will give you a copy of the project up and running on
 your local machine for development and testing purposes. See deployment
 for notes on deploying the project on a live system.
 
 ### Installing
 
-[//]: # ([![Badge]&#40;https://img.shields.io/pypi/v/pytho?style=for-the-badge&#41;]&#40;https://pypi.org/project/xsellco-api/&#41;)
+[![Badge](https://img.shields.io/pypi/v/python_seller_active?style=for-the-badge)](https://pypi.org/project/python-seller-active/)
 
 
     pip install python_seller_active
 
 
 ---
```

### Comparing `python_seller_active-0.0.3/python_seller_active.egg-info/PKG-INFO` & `python_seller_active-0.0.4/python_seller_active.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: python-seller-active
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wrapper around SellerActive.com API
 Home-page: https://github.com/yberezkin/python_seller_active
 Author: Yan Berezkin
 Author-email: yan.berezkin@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yberezkin/python_seller_active/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SELLER-ACTIVE-API Python Wrapper
 
+[![CodeFactor](https://www.codefactor.io/repository/github/yberezkin/python_seller_active/badge)](https://www.codefactor.io/repository/github/yberezkin/python_seller_active)
+
 This project provides a Python wrapper for interacting with the [rest.selleractive.com](https://rest.selleractive.com/) API, allowing developers to easily integrate the API's functionality into their Python applications.
 
 ## Getting Started
 
 These instructions will give you a copy of the project up and running on
 your local machine for development and testing purposes. See deployment
 for notes on deploying the project on a live system.
 
 ### Installing
 
-[//]: # ([![Badge]&#40;https://img.shields.io/pypi/v/pytho?style=for-the-badge&#41;]&#40;https://pypi.org/project/xsellco-api/&#41;)
+[![Badge](https://img.shields.io/pypi/v/python_seller_active?style=for-the-badge)](https://pypi.org/project/python-seller-active/)
 
 
     pip install python_seller_active
 
 
 ---
```

### Comparing `python_seller_active-0.0.3/python_seller_active.egg-info/SOURCES.txt` & `python_seller_active-0.0.4/python_seller_active.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -19,9 +19,10 @@
 seller_active/api/locations/__init__.py
 seller_active/api/locations/locations.py
 seller_active/api/orders/__init__.py
 seller_active/api/orders/orders.py
 seller_active/api/rate_limit_status/__init__.py
 seller_active/api/rate_limit_status/rate_limit_status.py
 seller_active/base/__init__.py
+seller_active/base/api_response.py
 seller_active/base/base.py
 seller_active/base/helpers.py
```

### Comparing `python_seller_active-0.0.3/seller_active/api/bundles/bundles.py` & `python_seller_active-0.0.4/seller_active/api/bundles/bundles.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,14 +36,31 @@
                 "updated_before": updated_before,
             }.items()
             if v is not None
         }
 
         return self._request("GET", params=params)
 
+    def get_all_bundles(self):
+        """
+        Retrieve list of all inventory items
+        """
+        page = 1
+        inventory = []
+        while True:
+            if page >= 1000:
+                break
+            resp = self.get_bundles(page=page)
+            inventory.extend(resp.data)
+            if len(resp.data) < 100:
+                break
+            else:
+                page += 1
+        return inventory
+
     def update_bundle(self, data: Dict):
         """
         Modifies an existing inventory bundle, all SKUs and relationships must exist prior. Quantity and price values
         are adjusted through the 'Inventory' POST API operations, 'Bundle' POST API operations modify the
         relationship amounts of individual SKUs in each bundle.
         data = {
           "BundleSKU": "string",
```

### Comparing `python_seller_active-0.0.3/seller_active/api/inventory/inventory.py` & `python_seller_active-0.0.4/seller_active/api/inventory/inventory.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,31 @@
                 "updated_before": updated_before,
             }.items()
             if v is not None
         }
 
         return self._request("GET", params=params)
 
+    def get_all_inventory(self):
+        """
+        Retrieve list of all inventory items
+        """
+        page = 1
+        inventory = []
+        while True:
+            if page >= 1000:
+                break
+            resp = self.get_inventory(page=page)
+            inventory.extend(resp.data)
+            if len(resp.data) < 100:
+                break
+            else:
+                page += 1
+        return inventory
+
     def update_inventory(self, data: Dict):
         """
         Modifies an existing inventory item, inventory is identified using required attribute 'SKU'.
         """
         if "SKU" not in data.keys():
             raise ValueError(
                 "'SKU' attribute was not found in `data`."
```

### Comparing `python_seller_active-0.0.3/seller_active/api/locations/locations.py` & `python_seller_active-0.0.4/seller_active/api/locations/locations.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,14 +36,31 @@
                 "updated_before": updated_before,
             }.items()
             if v is not None
         }
 
         return self._request("GET", params=params)
 
+    def get_all_locations(self):
+        """
+        Retrieve list of all inventory items
+        """
+        page = 1
+        inventory = []
+        while True:
+            if page >= 1000:
+                break
+            resp = self.get_locations(page=page)
+            inventory.extend(resp.data)
+            if len(resp.data) < 100:
+                break
+            else:
+                page += 1
+        return inventory
+
     def update_location(self, data: Dict):
         """
         Modify an existing inventory location, must specify the location by both
         required attributes 'SKU' and 'LocationName'.
         data = {
           "SKU": "string",
           "LocationName": "string",
```

### Comparing `python_seller_active-0.0.3/seller_active/api/orders/orders.py` & `python_seller_active-0.0.4/seller_active/api/orders/orders.py`

 * *Files identical despite different names*

### Comparing `python_seller_active-0.0.3/setup.py` & `python_seller_active-0.0.4/setup.py`

 * *Files identical despite different names*

