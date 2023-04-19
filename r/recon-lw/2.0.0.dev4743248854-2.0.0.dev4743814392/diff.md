# Comparing `tmp/recon_lw-2.0.0.dev4743248854.tar.gz` & `tmp/recon_lw-2.0.0.dev4743814392.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4743248854.tar", last modified: Wed Apr 19 12:25:48 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4743814392.tar", last modified: Wed Apr 19 13:21:15 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4743248854.tar` & `recon_lw-2.0.0.dev4743814392.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-19 12:25:32.000000 recon_lw-2.0.0.dev4743248854/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    13766 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/recon_lw/recon_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:21:15.000000 recon_lw-2.0.0.dev4743814392/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-19 13:20:48.000000 recon_lw-2.0.0.dev4743814392/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-19 13:21:15.000000 recon_lw-2.0.0.dev4743814392/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-19 13:20:48.000000 recon_lw-2.0.0.dev4743814392/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-19 13:20:56.000000 recon_lw-2.0.0.dev4743814392/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:21:15.000000 recon_lw-2.0.0.dev4743814392/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-04-19 13:20:48.000000 recon_lw-2.0.0.dev4743814392/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-19 13:20:48.000000 recon_lw-2.0.0.dev4743814392/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-19 13:20:48.000000 recon_lw-2.0.0.dev4743814392/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13794 2023-04-19 13:20:48.000000 recon_lw-2.0.0.dev4743814392/recon_lw/recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:21:15.000000 recon_lw-2.0.0.dev4743814392/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-19 13:21:15.000000 recon_lw-2.0.0.dev4743814392/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-19 13:21:15.000000 recon_lw-2.0.0.dev4743814392/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 13:21:15.000000 recon_lw-2.0.0.dev4743814392/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-19 13:21:15.000000 recon_lw-2.0.0.dev4743814392/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-19 13:21:15.000000 recon_lw-2.0.0.dev4743814392/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-19 13:20:48.000000 recon_lw-2.0.0.dev4743814392/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 13:21:15.000000 recon_lw-2.0.0.dev4743814392/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-19 13:20:48.000000 recon_lw-2.0.0.dev4743814392/setup.py
```

### Comparing `recon_lw-2.0.0.dev4743248854/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4743814392/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4743248854/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4743814392/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4743248854/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4743814392/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,14 +244,15 @@
     return {}
 
 
 def ob_clean_book(order_book):
     for side_key in ["ask", "bid"]:
         if side_key in order_book:
             order_book[side_key].clear()
+    return {}
 
 
 def ob_change_status(new_status, order_book):
     order_book["status"] = new_status
     return {}
 
 
@@ -318,14 +319,15 @@
     return {}
 
 
 def ob_aggr_clean_book(order_book):
     for side_key in ["ask_aggr", "bid_aggr"]:
         if side_key in order_book:
             order_book[side_key].clear()
+    return {}
 
 
 def ob_top_update(ask_price, ask_real_qty, ask_impl_qty, ask_real_n_orders, ask_impl_n_orders,
                   bid_price, bid_real_qty, bid_impl_qty, bid_real_n_orders, bid_impl_n_orders,
                   order_book):
     order_book["ask_price"] = ask_price
     order_book["ask_real_qty"] = ask_real_qty
```

### Comparing `recon_lw-2.0.0.dev4743248854/setup.py` & `recon_lw-2.0.0.dev4743814392/setup.py`

 * *Files identical despite different names*

