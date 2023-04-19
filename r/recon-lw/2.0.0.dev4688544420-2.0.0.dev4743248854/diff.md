# Comparing `tmp/recon_lw-2.0.0.dev4688544420.tar.gz` & `tmp/recon_lw-2.0.0.dev4743248854.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4688544420.tar", last modified: Thu Apr 13 11:11:09 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4743248854.tar", last modified: Wed Apr 19 12:25:48 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4688544420.tar` & `recon_lw-2.0.0.dev4743248854.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-13 11:10:43.000000 recon_lw-2.0.0.dev4688544420/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-13 11:10:43.000000 recon_lw-2.0.0.dev4688544420/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-13 11:10:50.000000 recon_lw-2.0.0.dev4688544420/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-13 11:10:43.000000 recon_lw-2.0.0.dev4688544420/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-13 11:10:43.000000 recon_lw-2.0.0.dev4688544420/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    13351 2023-04-13 11:10:43.000000 recon_lw-2.0.0.dev4688544420/recon_lw/recon_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-13 11:10:43.000000 recon_lw-2.0.0.dev4688544420/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-13 11:10:43.000000 recon_lw-2.0.0.dev4688544420/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-19 12:25:32.000000 recon_lw-2.0.0.dev4743248854/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13766 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/recon_lw/recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 12:25:48.000000 recon_lw-2.0.0.dev4743248854/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-19 12:25:24.000000 recon_lw-2.0.0.dev4743248854/setup.py
```

### Comparing `recon_lw-2.0.0.dev4688544420/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4743248854/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4688544420/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4743248854/recon_lw/recon_ob.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,32 +181,33 @@
         d_ev["attachedMessageIds"] = [item[1], item[2]]
         dupl_events.append(d_ev)
     save_events_func(dupl_events)
     duplicates.clear()
     flush_sequence_clear_cache(n_processed,rule_settings["sequence_cache"])
 
 
+def init_aggr_seq(order_book):
+    order_book["aggr_seq"] = {"top_v": 0, "top_delta": 0, "limit_v": 0, "limit_delta": 0}
+
+
 def ob_add_order(order_id, price, size, side, order_book):
-    result_body = {}
     if find_order_position(order_id, order_book)[0] is not None:
-        result_body["error"] = order_id + " already exists"
-        return result_body
+        return {"error": order_id + " already exists"}
     if price not in order_book[side]:
         order_book[side][price] = {order_id: size}
-        return result_body
+        return {}
+
     order_book[side][price][order_id] = size
     return {}
 
 
 def ob_update_order(order_id, price, size, order_book):
-    result_body = {}
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     if old_side is None:
-        result_body["error"] = order_id + " not found"
-        return result_body
+        return {"error": order_id + " not found"}
 
     if price == old_price:
         order_book[old_side][old_price][order_id] = size
     else:
         order_book[old_side][old_price].pop(order_id)
         if len(order_book[old_side][old_price]) == 0:
             order_book[old_side].pop(old_price)
@@ -214,57 +215,66 @@
             order_book[old_side][price] = {}
         order_book[old_side][price][order_id] = size
 
     return {}
 
 
 def ob_delete_order(order_id, order_book):
-    result_body = {}
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     if old_side is None:
-        result_body["error"] = order_id + " not found"
-        return result_body
+        return {"error": order_id + " not found"}
 
     order_book[old_side][old_price].pop(order_id)
     if len(order_book[old_side][old_price]) == 0:
         order_book[old_side].pop(old_price)
     return {}
 
 
 def ob_trade_order(order_id, traded_size ,order_book):
-    result_body = {}
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     if old_side is None:
-        result_body["error"] = order_id + " not found"
-        return result_body
+        return {"error": order_id + " not found"}
     if traded_size > old_size:
-        result_body["error"] = "traded size > resting size"
-        return result_body
+        return {"error": "traded size > resting size"}
     elif traded_size == old_size:
         order_book[old_side][old_price].pop(order_id)
         if len(order_book[old_side][old_price]) == 0:
             order_book[old_side].pop(old_price)
     else:
         order_book[old_side][old_price][order_id] -= traded_size
     return {}
 
 
+def ob_clean_book(order_book):
+    for side_key in ["ask", "bid"]:
+        if side_key in order_book:
+            order_book[side_key].clear()
+
+
 def ob_change_status(new_status, order_book):
     order_book["status"] = new_status
     return {}
 
 
 def find_order_position(order_id, order_book):
-    for side in ["ask","bid"]:
+    for side in ["ask", "bid"]:
         for pr,orders in order_book[side].items():
             if order_id in orders:
                 return side, pr, orders[order_id]
     return None, None, None
 
 
+def get_price_level(side, p, order_book):
+    if p not in order_book[side]:
+        return -1
+    levels = list(order_book[side].keys())
+    levels.sort()
+    return levels.index(p)+1 if side == "ask" else len(levels)-levels.index(p)
+
+
 def ob_aggr_add_level(side, level, price, real_qty, real_num_orders, impl_qty, impl_num_orders, order_book):
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
     side_key = side+"_aggr"
     new_index = level - 1
     if not 0 <= new_index <= len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
@@ -304,22 +314,29 @@
     upd_level = {"price": price, "real_qty": real_qty, "real_num_orders": real_num_orders, 
                  "impl_qty" : impl_qty, "impl_num_orders": impl_num_orders}
     order_book[side_key][update_index].update(upd_level)
 
     return {}
 
 
+def ob_aggr_clean_book(order_book):
+    for side_key in ["ask_aggr", "bid_aggr"]:
+        if side_key in order_book:
+            order_book[side_key].clear()
+
+
 def ob_top_update(ask_price, ask_real_qty, ask_impl_qty, ask_real_n_orders, ask_impl_n_orders,
                   bid_price, bid_real_qty, bid_impl_qty, bid_real_n_orders, bid_impl_n_orders,
                   order_book):
     order_book["ask_price"] = ask_price
     order_book["ask_real_qty"] = ask_real_qty
     order_book["ask_impl_qty"] = ask_impl_qty
     order_book["ask_real_n_orders"] = ask_real_n_orders
     order_book["ask_impl_n_orders"] = ask_impl_n_orders
     order_book["bid_price"] = bid_price
     order_book["bid_real_qty"] = bid_real_qty
     order_book["bid_impl_qty"] = bid_impl_qty
     order_book["bid_real_n_orders"] = bid_real_n_orders
     order_book["bid_impl_n_orders"] = bid_impl_n_orders
 
-    return {}
+    return {}
+
```

### Comparing `recon_lw-2.0.0.dev4688544420/setup.py` & `recon_lw-2.0.0.dev4743248854/setup.py`

 * *Files identical despite different names*

