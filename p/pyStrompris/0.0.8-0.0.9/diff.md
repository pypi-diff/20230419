# Comparing `tmp/pyStrompris-0.0.8.tar.gz` & `tmp/pyStrompris-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyStrompris-0.0.8.tar", last modified: Sat Dec  3 15:27:10 2022, max compression
+gzip compressed data, was "pyStrompris-0.0.9.tar", last modified: Sat Dec  3 23:43:43 2022, max compression
```

## Comparing `pyStrompris-0.0.8.tar` & `pyStrompris-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 15:27:10.876523 pyStrompris-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-03 15:26:58.000000 pyStrompris-0.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2022-12-03 15:27:10.876523 pyStrompris-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2022-12-03 15:26:58.000000 pyStrompris-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 15:27:10.876523 pyStrompris-0.0.8/pyStrompris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2022-12-03 15:27:10.000000 pyStrompris-0.0.8/pyStrompris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-03 15:27:10.000000 pyStrompris-0.0.8/pyStrompris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-03 15:27:10.000000 pyStrompris-0.0.8/pyStrompris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-03 15:27:10.000000 pyStrompris-0.0.8/pyStrompris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-03 15:27:10.000000 pyStrompris-0.0.8/pyStrompris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-03 15:27:10.876523 pyStrompris-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2022-12-03 15:26:58.000000 pyStrompris-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 15:27:10.876523 pyStrompris-0.0.8/strompris/
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2022-12-03 15:26:58.000000 pyStrompris-0.0.8/strompris/PriceSource.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 15:26:58.000000 pyStrompris-0.0.8/strompris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2022-12-03 15:26:58.000000 pyStrompris-0.0.8/strompris/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-03 15:26:58.000000 pyStrompris-0.0.8/strompris/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2022-12-03 15:26:58.000000 pyStrompris-0.0.8/strompris/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2022-12-03 15:26:58.000000 pyStrompris-0.0.8/strompris/strompris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 23:43:43.916939 pyStrompris-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-03 23:43:27.000000 pyStrompris-0.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2022-12-03 23:43:43.916939 pyStrompris-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2022-12-03 23:43:27.000000 pyStrompris-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 23:43:43.912939 pyStrompris-0.0.9/pyStrompris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2022-12-03 23:43:43.000000 pyStrompris-0.0.9/pyStrompris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-03 23:43:43.000000 pyStrompris-0.0.9/pyStrompris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-03 23:43:43.000000 pyStrompris-0.0.9/pyStrompris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-03 23:43:43.000000 pyStrompris-0.0.9/pyStrompris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-03 23:43:43.000000 pyStrompris-0.0.9/pyStrompris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-03 23:43:43.916939 pyStrompris-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2022-12-03 23:43:27.000000 pyStrompris-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 23:43:43.912939 pyStrompris-0.0.9/strompris/
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2022-12-03 23:43:27.000000 pyStrompris-0.0.9/strompris/PriceSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 23:43:27.000000 pyStrompris-0.0.9/strompris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2022-12-03 23:43:27.000000 pyStrompris-0.0.9/strompris/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-03 23:43:27.000000 pyStrompris-0.0.9/strompris/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2022-12-03 23:43:27.000000 pyStrompris-0.0.9/strompris/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2022-12-03 23:43:27.000000 pyStrompris-0.0.9/strompris/strompris.py
```

### Comparing `pyStrompris-0.0.8/LICENSE.md` & `pyStrompris-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyStrompris-0.0.8/PKG-INFO` & `pyStrompris-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyStrompris
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python3 library to read electricity price
 Home-page: https://github.com/bskjon/pyStrompris
 Author: Brage Skjønborg
 Author-email: bskjon@outlook.com
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `pyStrompris-0.0.8/README.md` & `pyStrompris-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyStrompris-0.0.8/pyStrompris.egg-info/PKG-INFO` & `pyStrompris-0.0.9/pyStrompris.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyStrompris
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python3 library to read electricity price
 Home-page: https://github.com/bskjon/pyStrompris
 Author: Brage Skjønborg
 Author-email: bskjon@outlook.com
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `pyStrompris-0.0.8/setup.py` & `pyStrompris-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyStrompris-0.0.8/strompris/PriceSource.py` & `pyStrompris-0.0.9/strompris/PriceSource.py`

 * *Files identical despite different names*

### Comparing `pyStrompris-0.0.8/strompris/common.py` & `pyStrompris-0.0.9/strompris/common.py`

 * *Files identical despite different names*

### Comparing `pyStrompris-0.0.8/strompris/schemas.py` & `pyStrompris-0.0.9/strompris/schemas.py`

 * *Files identical despite different names*

### Comparing `pyStrompris-0.0.8/strompris/strompris.py` & `pyStrompris-0.0.9/strompris/strompris.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,53 +76,57 @@
         today = self.get_prices_for_today()
         tomorrow = self.get_prices_for_tomorrow()
         return (today + tomorrow)
     
     async def async_get_current_price(self) -> Optional[Pris]:
         if (not self.priceSource._price_today or len(self.priceSource._price_today) == 0):
             await self.async_get_prices_for_today()
-        return next((x for x in self.priceSource._price_today if x.start.hour == getNorwayTime().hour), [None])
+        return next((x for x in self.priceSource._price_today if x.start.hour == getNorwayTime().hour), None)
         
     def get_current_price(self) -> Optional[Pris]:
         return self.sync(self.async_get_current_price())
                 
-    async def async_get_current_price_attrs(self) -> dict[str, Any]:
-        now = await self.async_get_current_price()
+    async def async_get_price_attrs(self, price: Pris = None, prices: List[Pris] = None) -> dict[str, Any]:
+        if (price is None):
+            price = await self.async_get_current_price()
+        if (prices is None or len(prices) == 0):
+            prices = self.priceSource._price_today
+        
         common = Common()
         max = common.getMax(self.priceSource._price_today)
         avg = common.getAverage(self.priceSource._price_today)
         min =  common.getMin(self.priceSource._price_today)
         return {
-            "start": now.start.isoformat(),
-            "end": now.slutt.isoformat(),
-            "kwh": now.kwh,
-            "tax": now.tax,
-            "total": now.total,
+            "start": price.start.isoformat(),
+            "end": price.slutt.isoformat(),
+            "kwh": price.kwh,
+            "tax": price.tax,
+            "total": price.total,
             "max": max + common.getTax(max, self.getTaxPercentage()),
             "avg": avg + common.getTax(avg, self.getTaxPercentage()),
             "min": min + common.getTax(min, self.getTaxPercentage()),
-            "price_level": common.getPriceLevel(now, self.priceSource._price_today)
+            "price_level": common.getPriceLevel(price, self.priceSource._price_today)
         }
      
     async def async_get_price_tomorrow_attrs(self) -> dict[str, Any]:
         common = Common()
         max = common.getMax(self.priceSource._price_tomorrow)
         avg = common.getAverage(self.priceSource._price_tomorrow)
         min = common.getMin(self.priceSource._price_tomorrow)
         return {
             "max": max + common.getTax(max, self.getTaxPercentage()),
             "avg": avg + common.getTax(avg, self.getTaxPercentage()),
             "min": min + common.getTax(min, self.getTaxPercentage())
         }
     
     def get_current_price_attrs(self) -> dict[str, Any]:
-        return self.sync(self.async_get_current_price_attrs())
+        return self.sync(self.async_get_price_attrs())
     
-    def get_price_attrs(self, price: Pris) -> dict[str, Any]:
-        return self.sync(self.async_get_price_attrs(price))
+    def get_price_attrs(self, price: Pris, prices: List[Pris]) -> dict[str, Any]:
+        return self.sync(self.async_get_price_attrs(price, prices))
     
     
     def __get_avg(self, prices: List[Pris]) -> float:
         common = Common()
         avg = common.getAverage(prices)
         #avg = avg + common.getTax(avg, self.getTaxPercentage())
         return avg
```

