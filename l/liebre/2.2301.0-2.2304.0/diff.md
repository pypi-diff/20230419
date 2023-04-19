# Comparing `tmp/liebre-2.2301.0-py3-none-any.whl.zip` & `tmp/liebre-2.2304.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 19924 bytes, number of entries: 13
--rw-rw-r--  2.0 unx      222 b- defN 23-Jan-13 01:26 liebre/__init__.py
+Zip file size: 19920 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      222 b- defN 23-Apr-19 20:13 liebre/__init__.py
 -rw-rw-r--  2.0 unx     8140 b- defN 23-Jan-13 01:26 liebre/consumer.py
 -rw-rw-r--  2.0 unx       46 b- defN 22-Dec-07 11:43 liebre/liebre.py
 -rw-rw-r--  2.0 unx       69 b- defN 22-Dec-07 11:44 liebre/logger.py
 -rw-rw-r--  2.0 unx      393 b- defN 23-Jan-12 22:45 liebre/message.py
--rw-rw-r--  2.0 unx     2535 b- defN 23-Jan-13 01:13 liebre/producer.py
--rw-rw-r--  2.0 unx     7250 b- defN 23-Jan-13 01:26 liebre/rabbit_store.py
--rw-rw-r--  2.0 unx     1121 b- defN 23-Jan-12 23:00 liebre/utils.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-Jan-13 01:30 liebre-2.2301.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      730 b- defN 23-Jan-13 01:30 liebre-2.2301.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-13 01:30 liebre-2.2301.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jan-13 01:30 liebre-2.2301.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      985 b- defN 23-Jan-13 01:30 liebre-2.2301.0.dist-info/RECORD
-13 files, 56739 bytes uncompressed, 18296 bytes compressed:  67.8%
+-rw-rw-r--  2.0 unx     2535 b- defN 23-Jan-17 11:16 liebre/producer.py
+-rw-rw-r--  2.0 unx     7402 b- defN 23-Jan-30 23:35 liebre/rabbit_store.py
+-rw-rw-r--  2.0 unx     1195 b- defN 23-Jan-17 18:06 liebre/utils.py
+-rw-rw-r--  2.0 unx    35149 b- defN 23-Apr-19 20:14 liebre-2.2304.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      730 b- defN 23-Apr-19 20:14 liebre-2.2304.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 20:14 liebre-2.2304.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-19 20:14 liebre-2.2304.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      985 b- defN 23-Apr-19 20:14 liebre-2.2304.0.dist-info/RECORD
+13 files, 56965 bytes uncompressed, 18292 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: liebre/rabbit_store.py
 Comment: 
 
 Filename: liebre/utils.py
 Comment: 
 
-Filename: liebre-2.2301.0.dist-info/LICENSE
+Filename: liebre-2.2304.0.dist-info/LICENSE
 Comment: 
 
-Filename: liebre-2.2301.0.dist-info/METADATA
+Filename: liebre-2.2304.0.dist-info/METADATA
 Comment: 
 
-Filename: liebre-2.2301.0.dist-info/WHEEL
+Filename: liebre-2.2304.0.dist-info/WHEEL
 Comment: 
 
-Filename: liebre-2.2301.0.dist-info/top_level.txt
+Filename: liebre-2.2304.0.dist-info/top_level.txt
 Comment: 
 
-Filename: liebre-2.2301.0.dist-info/RECORD
+Filename: liebre-2.2304.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## liebre/__init__.py

```diff
@@ -2,10 +2,10 @@
 # -*- coding: utf-8 -*-
 
 from .consumer import Consumer  # noqa F401
 from .producer import Producer  # noqa F401
 
 import logging
 
-__version__ = '2.2301.0'
+__version__ = '2.2304.0'
 
 logging.getLogger('pika').propagate = False
```

## liebre/rabbit_store.py

```diff
@@ -48,144 +48,143 @@
 
         self._user = user or 'guest'
         self._password = password or 'guest'
         self._host = host or 'localhost'
         self._port = port or 5672
         self._vhost = vhost or '/'
         self._exchange = exchange
-        self._max_retry_seconds = max_retry_seconds or 0
+        self._max_retry_seconds = (
+            max_retry_seconds
+            if max_retry_seconds and max_retry_seconds > 0 else 0
+        )
 
-        self._sleep_seconds_on_retry = sleep_seconds_on_retry or 1
+        self._sleep_seconds_on_retry = (
+            sleep_seconds_on_retry
+            if sleep_seconds_on_retry and sleep_seconds_on_retry > 0 else 1
+        )
 
         self._max_retries = max_retries or (
-            self._max_retry_seconds / self._sleep_seconds_on_retry
+            self._max_retry_seconds // self._sleep_seconds_on_retry
         )
 
         self._auto_ack = auto_ack
-        self._prefetch = prefetch or 10
-        self._partitions = partitions or 1
+        self._prefetch = prefetch if prefetch and prefetch >= 0 else 10
+        self._partitions = partitions if partitions and partitions >= 1 else 1
 
         self._exchange_options = self.__class__.EXCHANGE_OPTIONS.copy()
         if exchange_options:
             self._exchange_options = self._exchange_options | exchange_options
 
         self._queue_options = self.__class__.QUEUE_OPTIONS.copy()
         if queue_options:
             self._queue_options = self._queue_options | queue_options
 
-        self._rabbit_url = (
-            f'amqp://{self._user}:{self._password }@{self._host}:{self._port}'
-        )
-
+        self._declared_queues = set()
         self._declared_logical_queues = set()
+
         self._message_retries = {}
         self._lock = Lock()
 
-        self._connect()
-
-    def is_rabbitmq_alive(self):
-        connection = self._get_connection()
-        try:
-            # Provide a connection object so it can be closed
-            self._get_channel(connection=connection)
-            return True
-        except Exception:
-            return False
-        finally:
-            try:
-                connection.close()
-            except Exception:
-                pass
-
-    def _get_connection(self):
-        return pika.BlockingConnection(
-            pika.ConnectionParameters(
-                self._host,
-                self._port,
-                self._vhost,
-                pika.PlainCredentials(
-                    self._user,
-                    self._password,
-                ),
-            )
-        )
-
-    def thread_safe(function):
-
-        def _(*args, **kwargs):
-            instance = args[0]
-            with instance._lock:
-                return function(*args, **kwargs)
-
-        return _
+        self._initialized = False
 
     def reconnect(function):
 
         def _(*args, **kwargs):
             retries = 0
 
             while True:
                 try:
                     return function(*args, **kwargs)
 
                 except Exception as error:
                     instance = args[0]
+                    time.sleep(instance._sleep_seconds_on_retry)
+
                     retries += 1
                     if (not instance._max_retries
                             or retries >= instance._max_retries):
                         raise error
 
                     logger.warning(
                         'Reconnecting... '
                         f'({retries}/{instance._max_retries})',
                         error=error
                     )
 
                     try:
-                        instance._channel = instance._get_channel()
+                        instance.connect()
                     except Exception:
-                        pass
-                    time.sleep(instance._sleep_seconds_on_retry)
+                        logger.exception(
+                            'Reconnecting... '
+                            f'({retries}/{instance._max_retries})',
+                        )
+
+        return _
+
+    def connect(self):
+        if self._initialized:
+            return
+
+        self._channel = self._get_channel()
+        self._declare_exchange()
+
+        self._initialized = True
+
+    def thread_safe(function):
+
+        def _(*args, **kwargs):
+            instance = args[0]
+            with instance._lock:
+                return function(*args, **kwargs)
 
         return _
 
-    @reconnect
     @thread_safe
     def _declare_exchange(self):
         self._channel.exchange_declare(
             exchange=self._exchange,
             exchange_type=self._exchange_options['type'],
             durable=self._exchange_options['durable'],
             auto_delete=self._exchange_options['auto_delete'],
         )
 
-    @reconnect
-    def _connect(self):
-        self._channel = self._get_channel()
-        self._declare_exchange()
-
-    def _get_channel(
-        self,
-        prefetch=None,
-        connection=None,
-    ):
+    def _get_channel(self, prefetch=None):
         if prefetch is None:
             prefetch = self._prefetch
 
         # Pika's connection is not thread-safe, can't be reused.
         # Thus, neither the channels belonging to it.
-        if connection is None:
-            connection = self._get_connection()
+        connection = pika.BlockingConnection(
+            pika.ConnectionParameters(
+                self._host,
+                self._port,
+                self._vhost,
+                pika.PlainCredentials(
+                    self._user,
+                    self._password,
+                ),
+            )
+        )
 
         channel = connection.channel()
         channel.confirm_delivery()
         channel.basic_qos(prefetch_count=prefetch)
 
         return channel
 
+    # TODO same result as with liebre-js
+    def get_info(self):
+        try:
+            # Provide a connection object so it can be closed
+            channel = self._get_channel()
+            channel.connection.close()
+            return True
+        except Exception:
+            return False
+
     def _declare_queue(
         self,
         queue,
         options,
         partition=None,
         dead_letter=False,
         backup=False,
@@ -197,27 +196,29 @@
             arguments['x-queue-type'] = 'classic'
             if options['lazy']:
                 #  Quorum queues cannot be defined as lazy.
                 arguments['x-queue-mode'] = 'lazy'
 
         dead_letter_queue = get_dead_letter_queue_name(queue)
 
-        # Dead letter queueimage.png
+        # Dead letter queue
         if dead_letter:
             queue_name = dead_letter_queue
 
         # Backup queue
         elif backup:
             backup_queue = get_backup_queue_name(queue, partition)
             queue_name = backup_queue
 
         # Partition queue
         else:
             self._declared_logical_queues.add(queue)
             partition_queue = get_partition_queue_name(queue, partition)
+            self._declared_queues.add(partition_queue)
+
             queue_name = partition_queue
 
             if options['dead_letters']:
                 arguments['x-dead-letter-exchange'] = self._exchange
                 arguments['x-dead-letter-routing-key'] = dead_letter_queue
 
         self._channel.queue_declare(
```

## liebre/utils.py

```diff
@@ -6,33 +6,36 @@
         content,
         ensure_ascii=False,
         separators=(',', ':'),
     )
 
 
 def deserialize_content(content):
-    if content is None:
-        return
-
     try:
         deserialized_content = json.loads(content)
+
+        # Fix double serialization
         if isinstance(content, str):
-            deserialized_content = json.loads(deserialized_content)
-    except json.JSONDecodeError:
-        deserialized_content = content
+            try:
+                deserialized_content = json.loads(deserialized_content)
+            except Exception:
+                deserialized_content = content
+
+        return deserialized_content
 
-    return deserialized_content
+    except Exception:
+        return content
 
 
 def get_suffixed_queue_name(queue, suffix):
     return f'{queue}.{suffix}'
 
 
-def get_partition_queue_name(*args, **kwargs):
-    return get_suffixed_queue_name(*args, **kwargs)
+def get_partition_queue_name(queue, partition):
+    return get_suffixed_queue_name(queue, partition)
 
 
 def get_dead_letter_queue_name(queue):
     return get_suffixed_queue_name(queue, 'dlq')
 
 
 def get_backup_queue_name(queue, partition):
```

## Comparing `liebre-2.2301.0.dist-info/LICENSE` & `liebre-2.2304.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `liebre-2.2301.0.dist-info/METADATA` & `liebre-2.2304.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liebre
-Version: 2.2301.0
+Version: 2.2304.0
 Home-page: https://github.com/councilbox/liebre-python
 Author: 
 Author-email: 
 License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

## Comparing `liebre-2.2301.0.dist-info/RECORD` & `liebre-2.2304.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-liebre/__init__.py,sha256=RXOGi1c3YRywPfPlLt9VFirxbQMs0MQbKbdFvROjQdE,222
+liebre/__init__.py,sha256=7KQ4g-VBxjes0P0wW847XsbPvEjN4W8FiRPmCea_zlI,222
 liebre/consumer.py,sha256=qlkicjuR17nKqSkWO8tl00kQvdRQqXWXKiM1DJ6qK5Y,8140
 liebre/liebre.py,sha256=FZk9hm7vBsK8G16pNugputbrrEciYqJc_XRAhTCcojI,46
 liebre/logger.py,sha256=gFdT_UHqta9GXzzGK44_sDagnInpWDLKXDJ3J4ZJkmc,69
 liebre/message.py,sha256=O086ccmRmfJhqyhdurzA4LdHu-qzr5Ps7SsuMnxlX7U,393
 liebre/producer.py,sha256=P3pM3PWePHbMKj3BPGvFgCaT_lrJS336GyHREYmyx0M,2535
-liebre/rabbit_store.py,sha256=mz964OyXXOQts5PZHVlvXWCb68dND7UGKAOH1rFg__g,7250
-liebre/utils.py,sha256=GrbQZZOocaXx2k_2LKd0Q5_FSVKfujaft0NYwV7Q8NE,1121
-liebre-2.2301.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-liebre-2.2301.0.dist-info/METADATA,sha256=30kAYj6n2kXJxtb62zVoTF1aFdi6gkQEQ2iBNZIPYDo,730
-liebre-2.2301.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-liebre-2.2301.0.dist-info/top_level.txt,sha256=cl5ALalM53myFXDcFp7jtynIzvwoKF4RqF1x1Aw4WwY,7
-liebre-2.2301.0.dist-info/RECORD,,
+liebre/rabbit_store.py,sha256=1PHFx6PlDLyZHRiCCkHGLO6fT3M3ofjXV-9ihV0Hxyk,7402
+liebre/utils.py,sha256=OP-78Gvzf4UBlnRzmkme-W779jtRdxhkx7F2Qn6FrJM,1195
+liebre-2.2304.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+liebre-2.2304.0.dist-info/METADATA,sha256=K8nK9szLSvdCRLYxVBNELEsiP7fk97sy7N8txOmRJEU,730
+liebre-2.2304.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+liebre-2.2304.0.dist-info/top_level.txt,sha256=cl5ALalM53myFXDcFp7jtynIzvwoKF4RqF1x1Aw4WwY,7
+liebre-2.2304.0.dist-info/RECORD,,
```

