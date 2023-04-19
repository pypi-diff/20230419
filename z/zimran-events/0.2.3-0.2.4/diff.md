# Comparing `tmp/zimran-events-0.2.3.tar.gz` & `tmp/zimran-events-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-events-0.2.3.tar", last modified: Fri Apr 14 10:04:05 2023, max compression
+gzip compressed data, was "zimran-events-0.2.4.tar", last modified: Wed Apr 19 10:57:51 2023, max compression
```

## Comparing `zimran-events-0.2.3.tar` & `zimran-events-0.2.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:04:05.757557 zimran-events-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:04:05.745556 zimran-events-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:04:05.757557 zimran-events-0.2.3/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:04:05.757557 zimran-events-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 10:03:56.000000 zimran-events-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-14 10:04:05.757557 zimran-events-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-14 10:03:56.000000 zimran-events-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-14 10:03:56.000000 zimran-events-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 10:03:56.000000 zimran-events-0.2.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 10:04:05.757557 zimran-events-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:04:05.745556 zimran-events-0.2.3/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:04:05.757557 zimran-events-0.2.3/zimran/events/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:04:05.757557 zimran-events-0.2.3/zimran_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-14 10:04:05.000000 zimran-events-0.2.3/zimran_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-14 10:04:05.000000 zimran-events-0.2.3/zimran_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:04:05.000000 zimran-events-0.2.3/zimran_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-14 10:04:05.000000 zimran-events-0.2.3/zimran_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 10:04:05.000000 zimran-events-0.2.3/zimran_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:57:51.066606 zimran-events-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:57:51.062606 zimran-events-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:57:51.066606 zimran-events-0.2.4/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:57:51.066606 zimran-events-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-19 10:57:43.000000 zimran-events-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-19 10:57:51.066606 zimran-events-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-19 10:57:43.000000 zimran-events-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-19 10:57:43.000000 zimran-events-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-19 10:57:43.000000 zimran-events-0.2.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 10:57:51.066606 zimran-events-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:57:51.062606 zimran-events-0.2.4/zimran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:57:51.066606 zimran-events-0.2.4/zimran/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:57:51.066606 zimran-events-0.2.4/zimran_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-19 10:57:51.000000 zimran-events-0.2.4/zimran_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 10:57:51.000000 zimran-events-0.2.4/zimran_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:57:51.000000 zimran-events-0.2.4/zimran_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-19 10:57:51.000000 zimran-events-0.2.4/zimran_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 10:57:51.000000 zimran-events-0.2.4/zimran_events.egg-info/top_level.txt
```

### Comparing `zimran-events-0.2.3/.github/scripts/release.py` & `zimran-events-0.2.4/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.3/.gitignore` & `zimran-events-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.3/.pre-commit-config.yaml` & `zimran-events-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.3/LICENSE` & `zimran-events-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.3/PKG-INFO` & `zimran-events-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.2.3
+Version: 0.2.4
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.2.3/README.md` & `zimran-events-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.3/pyproject.toml` & `zimran-events-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zimran-events"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Talgat Abdraimov", email="abdraimov.talga@gmail.com" },
 ]
 description = "The zimran-events provides amqp interface"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
```

### Comparing `zimran-events-0.2.3/zimran/events/connection.py` & `zimran-events-0.2.4/zimran/events/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,17 @@
         if self._connection is not None and self._connection.is_open:
             self._connection.close()
 
         logger.info('AMQP Connection disconnected')
 
 
 class AsyncConnection:
-    def __init__(self, *, broker_url: str, loop=None, channel_number: int = 1):
+    def __init__(self, *, broker_url: str, loop: asyncio.AbstractEventLoop, channel_number: int = 1):
         self._url = broker_url
-        self._loop = loop or asyncio.get_event_loop()
+        self._loop = loop
 
         self._connection = None
         self._channel = None
         self._channel_number = channel_number
 
     async def __aenter__(self):
         await self.connect()
```

### Comparing `zimran-events-0.2.3/zimran/events/consumer.py` & `zimran-events-0.2.4/zimran/events/consumer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 
 import aio_pika
 from aioretry import retry
+from pika.channel import Channel
 
 
 try:
     from loguru import logger
 except ImportError:
     import logging
 
@@ -54,66 +55,68 @@
         self._service_name = service_name.replace('-', '_').lower()
         self._prefetch_count = prefetch_count
 
         self._event_handlers = {}
 
     def run(self):
         try:
-            self.channel.basic_qos(prefetch_count=self._prefetch_count)
+            channel = self.channel
+            channel.basic_qos(prefetch_count=self._prefetch_count)
 
-            self._declare_unroutable_exchange()
+            self._declare_unroutable_exchange(channel)
 
             consumer_amount = 0
             for event_name, data in self._event_handlers.items():
                 queue_name = cleanup_and_normalize_queue_name(f'{self._service_name}.{event_name}')
-                self.channel.queue_declare(
+                channel.queue_declare(
                     queue_name,
                     durable=True,
                     arguments={
                         'x-dead-letter-exchange': DEAD_LETTER_EXCHANGE_NAME,
                     },
                 )
 
                 if exchange := data['exchange']:
-                    self.channel.exchange_declare(
+                    channel.exchange_declare(
                         exchange=exchange.name,
                         exchange_type=exchange.type,
                         **exchange.as_dict(exclude=['name', 'type', 'timeout']),
                     )
-                    self.channel.queue_bind(queue=queue_name, exchange=exchange.name, routing_key=event_name)
+                    channel.queue_bind(queue=queue_name, exchange=exchange.name, routing_key=event_name)
 
-                self.channel.basic_consume(queue_name, data['handler'])
+                channel.basic_consume(queue_name, data['handler'])
                 logger.info(f'Registering consumer | queue: {queue_name} | routing_key: {event_name}')
                 consumer_amount += 1
 
             logger.info(f'Registered {consumer_amount} consumers')
-            self.channel.start_consuming()
+            channel.start_consuming()
         except Exception as exc:
             logger.error(f'Exception occured | error: {exc} | type: {type(exc)}')
         finally:
             self.disconnect()
 
-    def _declare_unroutable_exchange(self):
-        self.channel.exchange_declare(exchange=UNROUTABLE_EXCHANGE_NAME, exchange_type='fanout', durable=True)
-        self.channel.queue_declare(queue=UNROUTABLE_QUEUE_NAME, durable=True)
-        self.channel.queue_bind(queue=UNROUTABLE_QUEUE_NAME, exchange=UNROUTABLE_EXCHANGE_NAME, routing_key='')
+    def _declare_unroutable_exchange(self, channel: Channel):
+        channel.exchange_declare(exchange=UNROUTABLE_EXCHANGE_NAME, exchange_type='fanout', durable=True)
+        channel.queue_declare(queue=UNROUTABLE_QUEUE_NAME, durable=True)
+        channel.queue_bind(queue=UNROUTABLE_QUEUE_NAME, exchange=UNROUTABLE_EXCHANGE_NAME, routing_key='')
 
         logger.info('Declared unroutable events exchange')
 
 
 class AsyncConsumer(AsyncConnection, ConsumerMixin):
     def __init__(
         self,
         *,
         service_name: str,
         broker_url: str,
         channel_number: int = 1,
         prefetch_count: int = 10,
         loop=None,
     ):
+        loop = loop or asyncio.get_event_loop()
         super().__init__(broker_url=broker_url, loop=loop, channel_number=channel_number)
 
         self._service_name = service_name.replace('-', '_').lower()
         self._prefetch_count = prefetch_count
 
         self._event_handlers = {}
```

### Comparing `zimran-events-0.2.3/zimran/events/producer.py` & `zimran-events-0.2.4/zimran/events/producer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import json
 
 import aio_pika
 import pika
 from aioretry import retry
 
 
@@ -11,96 +12,100 @@
     import logging
 
     logger = logging.getLogger(__name__)
 
 
 from .connection import AsyncConnection, Connection
 from .constants import UNROUTABLE_EXCHANGE_NAME, UNROUTABLE_QUEUE_NAME
-from .schemas import ContextScheme
-from .utils import retry_policy, validate_context, validate_exchange
+from .schemas import ChannelPropertiesScheme, ExchangeScheme
+from .utils import retry_policy, validate_channel_properties, validate_exchange
 
 
 class Producer(Connection):
     def __init__(self, *, broker_url: str, channel_number: int = 1):
         super().__init__(broker_url=broker_url, channel_number=channel_number)
 
-    def publish(self, routing_key: str, *, payload: dict, context: ContextScheme | None = None):
-        if context is None:
-            context = ContextScheme()
+    def publish(
+        self,
+        routing_key: str,
+        *,
+        payload: dict,
+        exchange: ExchangeScheme | None = None,
+        properties: ChannelPropertiesScheme | None = None,
+    ):
+        if properties is None:
+            properties = ChannelPropertiesScheme()
         else:
-            validate_context(context)
+            validate_channel_properties(properties)
 
-        properties = pika.BasicProperties(
-            content_type='application/json',
-            delivery_mode=pika.DeliveryMode.Persistent,
-            correlation_id=context.correlation_id,
-            headers=context.headers,
-        )
+        basic_properties = pika.BasicProperties(**properties.as_dict(exclude_none=True))
         body = json.dumps(payload, default=str)
-        if context.exchange is None:
-            self.channel.basic_publish(exchange='', routing_key=routing_key, body=body, properties=properties)
+        if exchange is None:
+            self.channel.basic_publish(exchange='', routing_key=routing_key, body=body, properties=basic_properties)
             logger.info(f'Message published to basic exchange | routing_key: {routing_key}')
             return
 
         self._declare_unroutable_queue()
 
-        validate_exchange(context.exchange)
+        validate_exchange(exchange)
         self.channel.exchange_declare(
-            exchange=context.exchange.name,
-            exchange_type=context.exchange.type,
-            **context.exchange.as_dict(exclude=['name', 'type', 'timeout'], exclude_none=True),
+            exchange=exchange.name,
+            exchange_type=exchange.type,
+            **exchange.as_dict(exclude=['name', 'type', 'timeout'], exclude_none=True),
         )
 
         self.channel.basic_publish(
-            exchange=context.exchange.name,
+            exchange=exchange.name,
             routing_key=routing_key,
             body=body,
-            properties=properties,
+            properties=basic_properties,
         )
-        logger.info(f'Message published to {context.exchange.name} exchange | routing_key: {routing_key}')
+        logger.info(f'Message published to {exchange.name} exchange | routing_key: {routing_key}')
 
     def _declare_unroutable_queue(self):
         self.channel.exchange_declare(exchange=UNROUTABLE_EXCHANGE_NAME, exchange_type='fanout', durable=True)
         self.channel.queue_declare(queue=UNROUTABLE_QUEUE_NAME, durable=True)
         self.channel.queue_bind(queue=UNROUTABLE_QUEUE_NAME, exchange=UNROUTABLE_EXCHANGE_NAME, routing_key='')
 
 
 class AsyncProducer(AsyncConnection):
-    def __init__(self, *, broker_url: str, channel_number: int = 1):
-        super().__init__(broker_url=broker_url, channel_number=channel_number)
+    def __init__(self, *, broker_url: str, channel_number: int = 1, loop: asyncio.AbstractEventLoop | None = None):
+        loop = loop or asyncio.get_event_loop()
+        super().__init__(broker_url=broker_url, channel_number=channel_number, loop=loop)
 
     @retry(retry_policy)
-    async def publish(self, routing_key: str, *, payload: dict, context: ContextScheme | None = None):
-        if context is None:
-            context = ContextScheme()
+    async def publish(
+        self,
+        routing_key: str,
+        *,
+        payload: dict,
+        exchange: ExchangeScheme | None = None,
+        properties: ChannelPropertiesScheme | None = None,
+    ):
+        if properties is None:
+            properties = ChannelPropertiesScheme()
         else:
-            validate_context(context)
+            validate_channel_properties(properties)
 
-        message = self._get_message(context=context, payload=payload)
+        message = self._get_message(properties=properties, payload=payload)
 
         channel = await self.channel
-        if context.exchange is None:
+        if exchange is None:
             await channel.default_exchange.publish(message=message, routing_key=routing_key)
             logger.info(f'Message published to basic exchange | routing_key: {routing_key}')
             return
 
-        validate_exchange(context.exchange)
+        validate_exchange(exchange)
         await self._declare_unroutable_queue(channel)
 
-        exchange = await channel.declare_exchange(**context.exchange.as_dict(exclude_none=True))
-        await exchange.publish(message=message, routing_key=routing_key)
-        logger.info(f'Message published to {context.exchange.name} exchange | routing_key: {routing_key}')
+        declared_exchange = await channel.declare_exchange(**exchange.as_dict(exclude_none=True))
+        await declared_exchange.publish(message=message, routing_key=routing_key)
+        logger.info(f'Message published to {exchange.name} exchange | routing_key: {routing_key}')
 
     @staticmethod
-    def _get_message(context: ContextScheme, payload: dict):
-        return aio_pika.Message(
-            body=json.dumps(payload, default=str).encode(),
-            headers=context.headers,
-            content_type='application/json',
-            correlation_id=context.correlation_id,
-            delivery_mode=aio_pika.DeliveryMode.PERSISTENT,
-        )
+    def _get_message(properties: ChannelPropertiesScheme, payload: dict):
+        return aio_pika.Message(body=json.dumps(payload, default=str).encode(), **properties.as_dict(exclude_none=True))
 
     async def _declare_unroutable_queue(self, channel: aio_pika.abc.AbstractRobustChannel):
         exchange = await channel.declare_exchange(name=UNROUTABLE_EXCHANGE_NAME, type='fanout', durable=True)
         queue = await channel.declare_queue(name=UNROUTABLE_QUEUE_NAME, durable=True)
         await queue.bind(exchange=exchange, routing_key='')
```

### Comparing `zimran-events-0.2.3/zimran/events/utils.py` & `zimran-events-0.2.4/zimran/events/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 try:
     from loguru import logger
 except ImportError:
     import logging
 
     logger = logging.getLogger(__name__)
 
-from .exceptions import ContextTypeError, ExchangeTypeError
-from .schemas import ContextScheme, ExchangeScheme
+from .exceptions import ChannelPropertiesTypeError, ExchangeTypeError
+from .schemas import ChannelPropertiesScheme, ExchangeScheme
 
 
 def validate_exchange(exchange: ExchangeScheme):
     if not isinstance(exchange, ExchangeScheme):
         raise ExchangeTypeError('ExchangeTypeError: <exchange> must be instance of <ExchangeScheme>')
 
 
-def validate_context(context: ContextScheme):
-    if not isinstance(context, ContextScheme):
-        raise ContextTypeError('ContextTypeError: <context> must be instance of <ContextScheme>')
+def validate_channel_properties(properties: ChannelPropertiesScheme):
+    if not isinstance(properties, ChannelPropertiesScheme):
+        raise ChannelPropertiesTypeError(
+            'ChannelPropertiesTypeError: <properties> must be instance of <ChannelPropertiesScheme>',
+        )
 
 
 def cleanup_and_normalize_queue_name(queue_name: str):
     if '*' in queue_name:
         queue_name = queue_name.replace('*', '')
 
     if '#' in queue_name:
```

### Comparing `zimran-events-0.2.3/zimran_events.egg-info/PKG-INFO` & `zimran-events-0.2.4/zimran_events.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.2.3
+Version: 0.2.4
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.2.3/zimran_events.egg-info/SOURCES.txt` & `zimran-events-0.2.4/zimran_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

