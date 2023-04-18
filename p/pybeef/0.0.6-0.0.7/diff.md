# Comparing `tmp/pybeef-0.0.6-py3-none-any.whl.zip` & `tmp/pybeef-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6844 bytes, number of entries: 7
+Zip file size: 6838 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      350 b- defN 20-Feb-02 00:00 beef/__init__.py
--rw-r--r--  2.0 unx    11944 b- defN 20-Feb-02 00:00 beef/beef.py
+-rw-r--r--  2.0 unx    11937 b- defN 20-Feb-02 00:00 beef/beef.py
 -rw-r--r--  2.0 unx     1825 b- defN 20-Feb-02 00:00 beef/pool.py
-?rw-r--r--  2.0 unx     2515 b- defN 20-Feb-02 00:00 pybeef-0.0.6.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pybeef-0.0.6.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1070 b- defN 20-Feb-02 00:00 pybeef-0.0.6.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      510 b- defN 20-Feb-02 00:00 pybeef-0.0.6.dist-info/RECORD
-7 files, 18301 bytes uncompressed, 5956 bytes compressed:  67.5%
+?rw-r--r--  2.0 unx     2515 b- defN 20-Feb-02 00:00 pybeef-0.0.7.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pybeef-0.0.7.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1070 b- defN 20-Feb-02 00:00 pybeef-0.0.7.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      510 b- defN 20-Feb-02 00:00 pybeef-0.0.7.dist-info/RECORD
+7 files, 18294 bytes uncompressed, 5950 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: beef/beef.py
 Comment: 
 
 Filename: beef/pool.py
 Comment: 
 
-Filename: pybeef-0.0.6.dist-info/METADATA
+Filename: pybeef-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: pybeef-0.0.6.dist-info/WHEEL
+Filename: pybeef-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: pybeef-0.0.6.dist-info/licenses/LICENSE
+Filename: pybeef-0.0.7.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: pybeef-0.0.6.dist-info/RECORD
+Filename: pybeef-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beef/beef.py

```diff
@@ -245,15 +245,15 @@
                     await msg.ack()
 
     @contextlib.asynccontextmanager
     async def connect(self, url: str, max_channels=10) -> Pool:
         '''
         Opens a (single) connection to AMQP server at :url: and creates a pool of channels
         '''
-        connection = await aio_pika.connect_robust(url)
+        connection = await aio_pika.connect(url)
         async with connection:
             pool = Pool(connection, max_items=max_channels)
             async with pool:
                 self._pool.set(pool)
                 try:
                     yield pool
                 finally:
```

## Comparing `pybeef-0.0.6.dist-info/METADATA` & `pybeef-0.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybeef
-Version: 0.0.6
+Version: 0.0.7
 Summary: Opinionated distributed RPC using AMQP workers
 Project-URL: Homepage, https://github.com/innodatalabs/beef
 Project-URL: Bug Tracker, https://github.com/pypa/innodatalabs/beef
 Author-email: Mike Kroutikov <mkroutikov@innodata.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `pybeef-0.0.6.dist-info/licenses/LICENSE` & `pybeef-0.0.7.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

