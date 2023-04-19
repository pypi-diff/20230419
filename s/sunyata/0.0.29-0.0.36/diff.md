# Comparing `tmp/sunyata-0.0.29.tar.gz` & `tmp/sunyata-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sunyata-0.0.29.tar", last modified: Wed Mar  1 03:16:44 2023, max compression
+gzip compressed data, was "dist/sunyata-0.0.36.tar", last modified: Wed Apr 19 07:54:30 2023, max compression
```

## Comparing `sunyata-0.0.29.tar` & `sunyata-0.0.36.tar`

### file list

```diff
@@ -1,57 +1,66 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-01 03:16:44.000000 sunyata-0.0.29/
--rw-r--r--   0 root         (0) staff       (20)      636 2023-03-01 03:16:44.000000 sunyata-0.0.29/PKG-INFO
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      636 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1112 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)       52 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       57 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       63 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata.egg-info/dependency_links.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata/
--rw-r--r--   0 root         (0) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/db.py
--rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/log.py
--rw-r--r--   0 root         (0) staff       (20)      265 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/util.py
--rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/orm.py
--rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/eventloop.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata/cli/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/cli/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/cli/cli.py
--rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/cli/entry.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata/algorithm/
--rw-r--r--   0 root         (0) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/algorithm/bloomfilter.py
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/algorithm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/algorithm/lru.py
--rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/algorithm/trie.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/algorithm/hashtable.py
--rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/redislock.py
--rw-r--r--   0 root         (0) staff       (20)     3903 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/consul.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata/http/
--rw-r--r--   0 root         (0) staff       (20)     5416 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/http/server.py
--rw-r--r--   0 root         (0) staff       (20)     2375 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/http/transport.py
--rw-r--r--   0 root         (0) staff       (20)      368 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/http/request.py
--rw-r--r--   0 root         (0) staff       (20)       68 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/http/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      938 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/http/response.py
--rw-r--r--   0 root         (0) staff       (20)     3670 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/http/factory.py
--rw-r--r--   0 root         (0) staff       (20)      256 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/http/router.py
--rw-r--r--   0 root         (0) staff       (20)      663 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/http/status.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/cache_wrap.py
--rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/compress.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata/rpc/
--rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/encrypt.py
--rw-r--r--   0 root         (0) staff       (20)      699 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/rpc/serialize.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/rpc/exception.py
--rw-r--r--   0 root         (0) staff       (20)    11596 2023-03-01 03:14:41.000000 sunyata-0.0.29/sunyata/rpc/server.py
--rw-r--r--   0 root         (0) staff       (20)     2177 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/discovery.py
--rw-r--r--   0 root         (0) staff       (20)     8307 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/transport.py
--rw-r--r--   0 root         (0) staff       (20)     8370 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/client.py
--rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/compress.py
--rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/method.py
--rw-r--r--   0 root         (0) staff       (20)     2840 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/protocal.py
--rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/rpc/const.py
--rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/table_writer.py
--rw-r--r--   0 root         (0) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/wrap.py
--rw-r--r--   0 root         (0) staff       (20)     9004 2023-03-01 03:14:12.000000 sunyata-0.0.29/README.md
--rwxr-xr-x   0 root         (0) staff       (20)     1110 2023-03-01 03:10:59.000000 sunyata-0.0.29/setup.py
--rw-r--r--   0 root         (0) staff       (20)       38 2023-03-01 03:16:44.000000 sunyata-0.0.29/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-19 07:54:30.000000 sunyata-0.0.36/
+-rw-r--r--   0 root         (0) staff       (20)      486 2023-04-19 07:54:30.000000 sunyata-0.0.36/PKG-INFO
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-19 07:54:30.000000 sunyata-0.0.36/sunyata.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      486 2023-04-19 07:54:30.000000 sunyata-0.0.36/sunyata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1383 2023-04-19 07:54:30.000000 sunyata-0.0.36/sunyata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)       52 2023-04-19 07:54:30.000000 sunyata-0.0.36/sunyata.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)       70 2023-04-19 07:54:30.000000 sunyata-0.0.36/sunyata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       63 2023-04-19 07:54:30.000000 sunyata-0.0.36/sunyata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-04-19 07:54:30.000000 sunyata-0.0.36/sunyata.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-19 07:54:30.000000 sunyata-0.0.36/sunyata/
+-rw-r--r--   0 root         (0) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.36/sunyata/db.py
+-rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.36/sunyata/log.py
+-rw-r--r--   0 root         (0) staff       (20)      265 2023-02-28 12:29:05.000000 sunyata-0.0.36/sunyata/util.py
+-rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.36/sunyata/orm.py
+-rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.36/sunyata/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.36/sunyata/eventloop.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-19 07:54:30.000000 sunyata-0.0.36/sunyata/cli/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.36/sunyata/cli/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.36/sunyata/cli/cli.py
+-rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.36/sunyata/cli/entry.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-19 07:54:30.000000 sunyata-0.0.36/sunyata/algorithm/
+-rw-r--r--   0 root         (0) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.36/sunyata/algorithm/bloomfilter.py
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.36/sunyata/algorithm/binsearchtree.py
+-rw-r--r--   0 root         (0) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.36/sunyata/algorithm/rbtree.py
+-rw-r--r--   0 root         (0) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.36/sunyata/algorithm/avltree.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.36/sunyata/algorithm/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.36/sunyata/algorithm/bplustree.py
+-rw-r--r--   0 root         (0) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.36/sunyata/algorithm/btree.py
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.36/sunyata/algorithm/bintree.py
+-rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.36/sunyata/algorithm/lru.py
+-rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.36/sunyata/algorithm/trie.py
+-rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.36/sunyata/algorithm/hashtable.py
+-rw-r--r--   0 root         (0) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.36/sunyata/algorithm/avlsearchtree.py
+-rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.36/sunyata/redislock.py
+-rw-r--r--   0 root         (0) staff       (20)     3903 2023-03-01 03:10:44.000000 sunyata-0.0.36/sunyata/consul.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-19 07:54:30.000000 sunyata-0.0.36/sunyata/http/
+-rw-r--r--   0 root         (0) staff       (20)     3103 2023-04-14 09:55:44.000000 sunyata-0.0.36/sunyata/http/server.py
+-rw-r--r--   0 root         (0) staff       (20)      182 2023-04-12 02:31:22.000000 sunyata-0.0.36/sunyata/http/request_stream.py
+-rw-r--r--   0 root         (0) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.36/sunyata/http/transport.py
+-rw-r--r--   0 root         (0) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.36/sunyata/http/request.py
+-rw-r--r--   0 root         (0) staff       (20)       68 2023-04-13 06:36:26.000000 sunyata-0.0.36/sunyata/http/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1639 2023-04-14 10:00:43.000000 sunyata-0.0.36/sunyata/http/response.py
+-rw-r--r--   0 root         (0) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.36/sunyata/http/factory.py
+-rw-r--r--   0 root         (0) staff       (20)     3394 2023-04-14 10:00:50.000000 sunyata-0.0.36/sunyata/http/rawserver.py
+-rw-r--r--   0 root         (0) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.36/sunyata/http/router.py
+-rw-r--r--   0 root         (0) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.36/sunyata/http/status.py
+-rw-r--r--   0 root         (0) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.36/sunyata/cache_wrap.py
+-rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.36/sunyata/compress.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-19 07:54:30.000000 sunyata-0.0.36/sunyata/rpc/
+-rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.36/sunyata/rpc/encrypt.py
+-rw-r--r--   0 root         (0) staff       (20)      699 2023-02-28 12:29:05.000000 sunyata-0.0.36/sunyata/rpc/serialize.py
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.36/sunyata/rpc/exception.py
+-rw-r--r--   0 root         (0) staff       (20)    11673 2023-04-14 09:46:23.000000 sunyata-0.0.36/sunyata/rpc/server.py
+-rw-r--r--   0 root         (0) staff       (20)     2178 2023-04-14 09:41:36.000000 sunyata-0.0.36/sunyata/rpc/discovery.py
+-rw-r--r--   0 root         (0) staff       (20)     8307 2023-04-12 02:48:07.000000 sunyata-0.0.36/sunyata/rpc/transport.py
+-rw-r--r--   0 root         (0) staff       (20)     8110 2023-04-13 06:16:39.000000 sunyata-0.0.36/sunyata/rpc/client.py
+-rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.36/sunyata/rpc/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.36/sunyata/rpc/compress.py
+-rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.36/sunyata/rpc/method.py
+-rw-r--r--   0 root         (0) staff       (20)     2840 2023-04-13 06:02:14.000000 sunyata-0.0.36/sunyata/rpc/protocal.py
+-rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.36/sunyata/rpc/const.py
+-rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.36/sunyata/table_writer.py
+-rw-r--r--   0 root         (0) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.36/sunyata/wrap.py
+-rw-r--r--   0 root         (0) staff       (20)     9004 2023-04-13 06:19:43.000000 sunyata-0.0.36/README.md
+-rwxr-xr-x   0 root         (0) staff       (20)     1026 2023-04-17 06:36:31.000000 sunyata-0.0.36/setup.py
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-04-19 07:54:30.000000 sunyata-0.0.36/setup.cfg
```

### Comparing `sunyata-0.0.29/sunyata.egg-info/SOURCES.txt` & `sunyata-0.0.36/sunyata.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -15,24 +15,33 @@
 sunyata.egg-info/PKG-INFO
 sunyata.egg-info/SOURCES.txt
 sunyata.egg-info/dependency_links.txt
 sunyata.egg-info/entry_points.txt
 sunyata.egg-info/requires.txt
 sunyata.egg-info/top_level.txt
 sunyata/algorithm/__init__.py
+sunyata/algorithm/avlsearchtree.py
+sunyata/algorithm/avltree.py
+sunyata/algorithm/binsearchtree.py
+sunyata/algorithm/bintree.py
 sunyata/algorithm/bloomfilter.py
+sunyata/algorithm/bplustree.py
+sunyata/algorithm/btree.py
 sunyata/algorithm/hashtable.py
 sunyata/algorithm/lru.py
+sunyata/algorithm/rbtree.py
 sunyata/algorithm/trie.py
 sunyata/cli/__init__.py
 sunyata/cli/cli.py
 sunyata/cli/entry.py
 sunyata/http/__init__.py
 sunyata/http/factory.py
+sunyata/http/rawserver.py
 sunyata/http/request.py
+sunyata/http/request_stream.py
 sunyata/http/response.py
 sunyata/http/router.py
 sunyata/http/server.py
 sunyata/http/status.py
 sunyata/http/transport.py
 sunyata/rpc/__init__.py
 sunyata/rpc/client.py
```

### Comparing `sunyata-0.0.29/sunyata/db.py` & `sunyata-0.0.36/sunyata/db.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/log.py` & `sunyata-0.0.36/sunyata/log.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/orm.py` & `sunyata-0.0.36/sunyata/orm.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/cli/cli.py` & `sunyata-0.0.36/sunyata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/algorithm/bloomfilter.py` & `sunyata-0.0.36/sunyata/algorithm/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/algorithm/lru.py` & `sunyata-0.0.36/sunyata/algorithm/lru.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/algorithm/trie.py` & `sunyata-0.0.36/sunyata/algorithm/trie.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/algorithm/hashtable.py` & `sunyata-0.0.36/sunyata/algorithm/hashtable.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/redislock.py` & `sunyata-0.0.36/sunyata/redislock.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/consul.py` & `sunyata-0.0.36/sunyata/consul.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/http/transport.py` & `sunyata-0.0.36/sunyata/http/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/http/factory.py` & `sunyata-0.0.36/sunyata/http/factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from datetime import date
 from sunyata.http.request import HttpRequest
 from sunyata.http.response import HttpResponse
 from sunyata.http.router import HttpRouter
 from sunyata.util import bytes2str
+import ujson
 
 class HttpFactory(object):
 
-    maxContentLength = 1 * 1024 * 1024 #1M限制
-
     def __init__(self) -> None:
         super().__init__()
 
     @classmethod
     def genLineHeaderBody(self, lines):
         getHeader = 1
         reqHeaders = []
@@ -21,84 +19,59 @@
             if not l:
                 getHeader = 0
             if getHeader:
                 reqHeaders.append(l)
             else:
                 reqBody = reqBody + l
         return reqLine, reqHeaders, reqBody
-        '''
-        reqHeaders = []
-        reqLine = lines[0]
-        for l in lines[1:]:
-            if l and b': ' in l:
-                reqHeaders.append(l)
-            else:
-                reqHeaders = [l for l in lines[1:-2] if l != b'' and b': ' in l]
-        '''
-            
-        #reqBody = lines[-1]
-        #reqHeaders = [l for l in lines[1:-2] if l != b'' and b': ' in l]
-        return reqLine, reqHeaders, reqBody
-        '''
-        reqLine = b''
-        reqHeaders = []
-        reqBody = b''
-        lenLines = len(lines)
-        for index, line in enumerate(lines):
-            if index == 0: 
-                reqLine = line
-            elif index == lenLines - 1:
-                reqBody = line
-            elif index > 0 and line != b'':
-                reqHeaders.append(line)
-        return reqLine, reqHeaders, reqBody
-        '''
+
+    @classmethod
+    def parseRequestData(cls, uri, body):
+        requestData = {}
+        if uri:
+            try:
+                kvPairs = uri.split(b'?')[1].split(b'&')
+                for kvPair in kvPairs:
+                    k, v = kvPair.split(b'=')
+                    requestData[bytes2str(k)] = bytes2str(v)
+            except:
+                pass
+        if body:
+            try:
+                bodydic = ujson.decode(body)
+                requestData.update(bodydic)
+            except:
+                pass
+        return requestData
         
     @classmethod
-    def genHttpRequest(cls, linesStr, conn):
+    async def genHttpRequest(cls, requestStream):
+        linesStr = await requestStream.reader.read(requestStream.bufsize)
         req = HttpRequest()
         lines = linesStr.split(b"\r\n")
         reqLine, reqHeaders, reqBody = cls.genLineHeaderBody(lines)
-    
         method, uri, httpVersion = reqLine.split(b' ')
         req.method = bytes2str(method)
         req.httpVersion = bytes2str(httpVersion)
         req.uri = bytes2str( uri.split(b'?')[0] )
         req.body = reqBody
         for header in reqHeaders:
             if header == b'':
                 continue
             k, v = header.split(b': ')
             try:
                 req.headers[bytes2str(k)] = bytes2str(v)
             except:
                 req.headers[str(k)] = str(v)
-        if req.body:
-            try:
-                for kvPair in req.body.split(b'&'):
-                    k, v = kvPair.split(b'=')
-                    req.data[bytes2str(k)] = bytes2str(v)
-            except:
-                pass
-        else:
-            try:
-                kvPairs = uri.split(b'?')[1].split(b'&')
-                for kvPair in kvPairs:
-                    k, v = kvPair.split(b'=')
-                    req.data[bytes2str(k)] = bytes2str(v)
-            except:
-                pass
-        contentLength = int(req.headers.get('Content-Length'))
-        #if contentLength > cls.maxContentLength:
-        #    raise Exception('content-length over')
+        req.data = cls.parseRequestData(uri, req.body)
+        contentLength = int(req.headers.get('Content-Length', 0))
         hasRead = len(req.body)
         toRead = contentLength - hasRead
-        bufsize = 1024 
         while toRead:
-            rdata = conn.recv(bufsize)
+            rdata = requestStream.reader.read(toRead)
             if not rdata:
                 raise Exception('peer closed')
             req.body = req.body + rdata
             hasRead = hasRead + len(rdata)
             toRead = contentLength - hasRead
         return req
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sunyata-0.0.29/sunyata/http/status.py` & `sunyata-0.0.36/sunyata/http/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class HttpStatus403(HttpStatus):
     code = 403
     msg = 'Forbidden'
 
 
 class HttpStatus404(HttpStatus):
-    code = 403
+    code = 404
     msg = 'Not Found'
 
 
 class HttpStatus405(HttpStatus):
     code = 405
     msg = 'Method Not Allowed'
```

### Comparing `sunyata-0.0.29/sunyata/cache_wrap.py` & `sunyata-0.0.36/sunyata/cache_wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/rpc/serialize.py` & `sunyata-0.0.36/sunyata/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/rpc/server.py` & `sunyata-0.0.36/sunyata/rpc/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 import socket
 from sunyata.rpc.discovery import DiscoveryConfig, ConsulRpcDiscovery
 import struct
 from sunyata.rpc.compress import RpcCompress
 from types import FunctionType
 from sunyata.rpc.method import RpcMethod
 import asyncio
+import uvloop
 import inspect
 from sunyata.http.server import HttpServer
-import traceback
+asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+
 
 class RpcServer(object):
 
     __slots__ = ('discoveryConfig', 'discovery', 'protocal')
 
     funcMap = {}
     funcList = []
@@ -160,15 +162,15 @@
         return resp
 
     def serve(self):
         tRegist = None
         if self.discovery and self.discoveryConfig:
             self.discovery.regist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True)
         self.printLogo()
-        print(' HTTP rpc serving on %s:%s' % (self.host, self.port) )
+        print('http rpc running on http://%s:%s' % (self.host, self.port) )
         self.app.serve()
 
 
 class TcpRpcServer(BlockTcpRpcServer):
 
     def __init__(self, host, port):
         BlockTcpRpcServer.__init__(self, host, port)
@@ -215,15 +217,15 @@
                 writer.close()
                 return
 
     async def main(self):
         loop = asyncio.get_event_loop()
         coro = asyncio.start_server(self.handle, self.host, self.port, loop=loop)
         server = loop.run_until_complete(coro)
-        print('TCP rpc serving on %s:%s' % (self.host, self.port))
+        print('tcp rpc running on tcp://%s:%s' % (self.host, self.port))
         try:
             loop.run_forever()
         except KeyboardInterrupt:
             pass
         # Close the server
         server.close()
         loop.run_until_complete(server.wait_closed())
@@ -250,15 +252,15 @@
         if self.discovery and self.discoveryConfig:
             tRegist = self.discovery.asyncRegist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True)
             tasks.append(tRegist)
         coro = asyncio.start_server(self.handle, self.host, self.port, loop=loop)
         tasks.append(coro)
         rs = loop.run_until_complete(asyncio.gather(*tasks))
         self.printLogo()
-        print('TCP rpc serving on %s:%s' % (self.host, self.port) )
+        print('tcp rpc running on tcp://%s:%s' % (self.host, self.port) )
         try:
             loop.run_forever()
         except KeyboardInterrupt:
             pass
         server = rs[-1]
         # Close the server
         server.close()
@@ -295,15 +297,15 @@
             except Exception as ex:
                 print('UDP handler exception:', ex)
     
     def serve(self):
         self.startWorkers()
         self.protocal.transport.bind()
         self.printLogo()
-        print(' UDP rpc serving on %s:%s' % (self.host, self.port))
+        print('udp rpc running on udp://%s:%s' % (self.host, self.port))
         if self.discovery and self.discoveryConfig:
             self.discovery.regist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True)
         while 1:
             try:
                 msg, cliAddr = self.protocal.transport.recv()
                 self.queue.put({'msg' : msg, 'addr' : cliAddr})
             except socket.timeout:
```

### Comparing `sunyata-0.0.29/sunyata/rpc/discovery.py` & `sunyata-0.0.36/sunyata/rpc/discovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from sunyata.consul import ConsulApi, Instance
 import time
 import threading
 import asyncio
 
 
+
 class RpcDiscovery(object):
     pass
 
 
 class DiscoveryConfig(object):
 
     __slots__ = ('consulHost', 'consulPort', 'serviceName', 'serviceHost', 'servicePort', 'consulToken')
```

### Comparing `sunyata-0.0.29/sunyata/rpc/transport.py` & `sunyata-0.0.36/sunyata/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/rpc/client.py` & `sunyata-0.0.36/sunyata/rpc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,19 +91,14 @@
         return self.lastServer
 
     @retryTimes(retryTimes=3)
     def call(self, func, *args, **kwargs):
         pass
 
     def __getattr__(self, key):
-        #def remote_attr(*args, **kwargs):
-        #    print(f'{key}方法不存在, 参数为:{args}, {kwargs}')
-        #    return self.call(f'{key}', *args, **kwargs)
-        #def remote_attr(*args, **kwargs):
-        #    return Callable(self, f"{key}")
         if key in dir(self):
             return getattr(self, key)
         return Callable(self, f"{key}")
 
 
 class TcpRpcClient(RpcClient):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sunyata-0.0.29/sunyata/rpc/method.py` & `sunyata-0.0.36/sunyata/rpc/method.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/rpc/protocal.py` & `sunyata-0.0.36/sunyata/rpc/protocal.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/table_writer.py` & `sunyata-0.0.36/sunyata/table_writer.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/wrap.py` & `sunyata-0.0.36/sunyata/wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/README.md` & `sunyata-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/setup.py` & `sunyata-0.0.36/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-DEFINE_VERSION = '0.0.29'
+DEFINE_VERSION = '0.0.36'
 from setuptools import setup
 
 requireList = [
     'lz4==3.1.3',
     'requests==2.25.1',
-    'PyMySQL==0.10.1',
-    'DBUtils==1.3',
+    'ujson==1.35',
+    'uvloop==0.19.0'
+    'uvicorn==0.18.0'
+    #'PyMySQL==0.10.1',
+    #'DBUtils==1.3',
 ]
 
 setup(
     name='sunyata',
     version=DEFINE_VERSION,
     description='Light, simple, asynchronous RPC framework for Python',
     author='tank',
     license='MIT',
     platforms="any",
     install_requires=requireList,
     classifiers=[
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     keywords='sunyata',
@@ -36,8 +36,8 @@
     ],
     include_package_data=True,
     entry_points = {
         'console_scripts' : [
             'sunyata=sunyata.cli.entry:main'
         ]
     }
-)
+)
```

