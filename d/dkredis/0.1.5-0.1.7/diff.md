# Comparing `tmp/dkredis-0.1.5.tar.gz` & `tmp/dkredis-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dkredis-0.1.5.tar", last modified: Wed Sep 30 13:19:33 2020, max compression
+gzip compressed data, was "dkredis-0.1.7.tar", last modified: Wed Apr 19 11:49:33 2023, max compression
```

## Comparing `dkredis-0.1.5.tar` & `dkredis-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2020-09-30 13:19:33.000000 dkredis-0.1.5/
-drwxrwxrwx   0        0        0        0 2020-09-30 13:19:33.000000 dkredis-0.1.5/dkredis/
--rw-rw-rw-   0        0        0    11419 2020-09-30 13:16:59.000000 dkredis-0.1.5/dkredis/dkredis.py
--rw-rw-rw-   0        0        0     6050 2020-09-29 14:18:14.000000 dkredis-0.1.5/dkredis/rediscache.py
--rw-rw-rw-   0        0        0       46 2020-09-30 13:17:19.000000 dkredis-0.1.5/dkredis/__init__.py
-drwxrwxrwx   0        0        0        0 2020-09-30 13:19:33.000000 dkredis-0.1.5/dkredis.egg-info/
--rw-rw-rw-   0        0        0        1 2020-09-30 13:19:32.000000 dkredis-0.1.5/dkredis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-08-21 09:01:10.000000 dkredis-0.1.5/dkredis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     1406 2020-09-30 13:19:32.000000 dkredis-0.1.5/dkredis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       13 2020-09-30 13:19:32.000000 dkredis-0.1.5/dkredis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      274 2020-09-30 13:19:32.000000 dkredis-0.1.5/dkredis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2020-09-30 13:19:32.000000 dkredis-0.1.5/dkredis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1406 2020-09-30 13:19:33.000000 dkredis-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      684 2020-05-18 05:50:14.000000 dkredis-0.1.5/README.rst
--rw-rw-rw-   0        0        0       68 2020-09-30 13:19:33.000000 dkredis-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      711 2020-09-30 13:17:19.000000 dkredis-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:49:33.409312 dkredis-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-19 11:49:33.409312 dkredis-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-19 11:49:18.000000 dkredis-0.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:49:33.409312 dkredis-0.1.7/dkredis/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 11:49:18.000000 dkredis-0.1.7/dkredis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-04-19 11:49:18.000000 dkredis-0.1.7/dkredis/dkredis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-04-19 11:49:18.000000 dkredis-0.1.7/dkredis/rediscache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:49:33.409312 dkredis-0.1.7/dkredis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-19 11:49:33.000000 dkredis-0.1.7/dkredis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-19 11:49:33.000000 dkredis-0.1.7/dkredis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:49:33.000000 dkredis-0.1.7/dkredis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:49:33.000000 dkredis-0.1.7/dkredis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 11:49:33.000000 dkredis-0.1.7/dkredis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 11:49:33.000000 dkredis-0.1.7/dkredis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-19 11:49:33.413312 dkredis-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-19 11:49:18.000000 dkredis-0.1.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dkredis-0.1.5/dkredis/dkredis.py` & `dkredis-0.1.7/dkredis/dkredis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Interface to our redis instance.
 
 Redis command reference: http://redis.io/commands
 
 Usage::
 
@@ -15,31 +14,29 @@
 Python interface peculiarities are explained here:
 https://github.com/andymccurdy/redis-py
 
 The windows version of the redis server that we use is
 from https://github.com/rgl/redis/downloads
 ----
 """
-from builtins import str as text
 import os
 import pickle
-import sys
 import time
 import redis as _redis
 from contextlib import contextmanager
 
 PICLE_PROTOCOL = 1
 
 
 class Timeout(Exception):  # pragma: nocover
     """A timout limit was exceeded.
     """
 
     def __init__(self, retry=0):
-        super(Timeout, self).__init__()
+        super().__init__()
         self.retry = retry
 
 
 # class Redis(object):
 #     def __init__(self, host='localhost', port=6379, db=0, cn=None):
 #         self.host = host
 #         self.port = port
@@ -97,15 +94,16 @@
 #     def pop_pyval(key, cn=None):
 #         """Get value and remove key.
 #         """
 #         r = cn or connect()
 #         val = get_pyval(key, cn=r)
 #         r.delete(key)
 #         # with r.pipeline() as p:
-#         #     val = get_pyval(key, p)  # can't get a val in the middle of a pipeline
+#         #     # can't get a val in the middle of a pipeline
+#         #     val = get_pyval(key, p)
 #         #     p.delete(key)
 #         #     p.execute()
 #         return val
 #
 #     def update(self, key, fn):
 #         """Atomic update of ``key`` with result of ``fn``.
 #
@@ -121,15 +119,16 @@
 #             while 1:
 #                 try:
 #                     p.watch(key)  # --> immediate mode
 #                     val = p.get(key)
 #                     p.multi()  # --> back to buffered mode
 #                     newval = fn(val)
 #                     p.set(key, newval)
-#                     p.execute()  # raises WatchError if anyone has changed `key`
+#                     # raises WatchError if anyone has changed `key`
+#                     p.execute()
 #                     break  # success, break out of while loop
 #                 except _redis.WatchError:  # pragma: nocover
 #                     pass  # someone else got there before us, retry.
 #         return newval
 
 
 def connect(host=None, port=6379, db=0, password=None):
@@ -160,16 +159,18 @@
 #     """setmin_cutoff(KEY, val, cutoff)
 #        ==> min(r[KEY], val) if less than cutoff
 #     """
 #     def fn(a, b):
 #         return max(cutoff, min(a, b))
 #     return update_binop(fn)
 #
-# setmin_cut = lambda cut: lambda a, b: update_binop(lambda a,b: max(cut, min(a, b)))
-# setmax_cut = lambda cut: lambda a, b: update_binop(lambda a,b: min(cut, max(a, b)))
+# setmin_cut = lambda cut: lambda a, b: update_binop(
+#                                           lambda a,b: max(cut, min(a, b)))
+# setmax_cut = lambda cut: lambda a, b: update_binop(
+#                                           lambda a,b: min(cut, max(a, b)))
 #
 # setmin0 = setmin_cut(0)
 # setmax0 = setmax_cut(0)
 #
 # def setmax_cutoff(key,
 #     """setmin_cutoff(KEY, val, cutoff)
 #        ==> max(r[KEY], val) if greater than cutoff
@@ -180,15 +181,15 @@
 # #: set to minimum of
 # setmin0 = lambda a,b: setmin_cutoff(a, b
 
 
 def update(key, fn, cn=None):
     """Usage
        ::
-       
+
             update(KEY, lambda val: val + 42)
 
     """
     r = cn or connect()
     with r.pipeline() as p:
         while 1:
             try:
@@ -209,27 +210,27 @@
 def setmax(key, val, cn=None):
     """Update key with the max of the current value and `val`::
 
           r[key] := max(r[key], val)
 
        returns the maximum value.
     """
-    if isinstance(val, text):
+    if isinstance(val, str):
         val = val.encode('u8')
     return update(key, lambda v: max(v, val), cn=cn)
 
 
 def setmin(key, val, cn=None):
     """Update key with the max of the current value and `val`::
 
           r[key] := min(r[key], val)
 
        returns the maximum value.
     """
-    if isinstance(val, text):
+    if isinstance(val, str):
         val = val.encode('u8')
     return update(key, lambda v: min(v, val), cn=cn)
 
 
 def later(n=0.0):
     """Return timestamp ``n`` seconds from now.
     """
@@ -267,15 +268,16 @@
 def pop_pyval(key, cn=None):
     """Get value and remove key.
     """
     r = cn or connect()
     val = get_pyval(key, cn=r)
     r.delete(key)
     # with r.pipeline() as p:
-    #     val = get_pyval(key, p)  # can't get a val in the middle of a pipeline
+    #     # can't get a val in the middle of a pipeline
+    #     val = get_pyval(key, p)
     #     p.delete(key)
     #     p.execute()
     return val
 
 
 def set_dict(key, dictval, secs=None, cn=None):
     """All values in `dictval` should be strings. They'll be read back
@@ -326,18 +328,18 @@
     # XXX: redis always returns bytes, and we want unicode
     return {k.decode('u8'): v.decode('u8') for k, v in result.items()}
 
 
 def convert_to_bytes(r):
     if isinstance(r, bytes):
         return r
-    if isinstance(r, text):
+    if isinstance(r, str):
         return r.encode('utf-8')
     else:
-        return text(r).encode('utf-8')
+        return str(r).encode('utf-8')
 
 
 def rate_limiting_lock(resources, seconds=30, cn=None):
     """Lock all the keys and keep them locked for ``seconds`` seconds.
        Useful e.g. to prevent sending email to the same domain more often
        than every 15 seconds.
 
@@ -346,15 +348,15 @@
             function (below).
 
     """
     if not resources:
         return True
 
     resources = [convert_to_bytes(r) for r in resources]
-    keys = dict((b'rl-lock.' + r, later(seconds)) for r in resources)
+    keys = {b'rl-lock.' + r: later(seconds) for r in resources}
 
     r = cn or connect()
 
     if r.msetnx(keys):
         with r.pipeline() as pipe:
             for key in keys:
                 pipe.expire(key, seconds)
```

### Comparing `dkredis-0.1.5/dkredis/rediscache.py` & `dkredis-0.1.7/dkredis/rediscache.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# -*- coding: utf-8 -*-
-"""Object cache implementation using redis as a backend.
 """
-from __future__ import print_function, absolute_import
+Object cache implementation using redis as a backend.
+"""
 import pickle
 import hashlib
-import zlib
-import base64
 from . import dkredis
+import logging
 
+log = logging.getLogger(__name__)
 
-PICLE_PROTOCOL = 0
-REDIS_CACHE_DEBUG = True
+PICLE_PROTOCOL = 1
+REDIS_CACHE_DEBUG = False
 
 if REDIS_CACHE_DEBUG:
     def writeln(*args, **kw):
         return print(*args, **kw)
 else:
     def writeln(*args, **kw):
         return None
 
 
 def _cache_serialize(val):
     """Serialize a python value to go into the cache.
     """
-    return base64.b64encode(zlib.compress(pickle.dumps(val,protocol=PICLE_PROTOCOL)))
+    return pickle.dumps(val, protocol=PICLE_PROTOCOL)
 
 
 def _cache_unserialize(val):
     """Unserialize a python value from the cache.
     """
-    return pickle.loads(zlib.decompress(base64.b64decode(val)))
+    # return pickle.loads(zlib.decompress(base64.b64decode(val)))
+    return pickle.loads(val)
 
 
-class cache(object):
+class cache:
     """Usage::
 
          from dkredis.rediscache import cache
 
          try:
              v = cache.get(key)
          except cache.DoesNotExist:
@@ -53,93 +53,104 @@
     class DoesNotExist(Exception):
         "Value not in cache (possibly due to expiration)."
 
     @staticmethod
     def rediskey(key):
         "The redis key is obj-cache. + the md5 hexdigest of its serialization."
         k = _cache_serialize(key)
-        return "obj-cache." + hashlib.md5(k).hexdigest()
+        return "obj-cache:" + hashlib.md5(k).hexdigest()
 
     @classmethod
     def ping(cls):
         r = dkredis.connect()
         r.ping()
 
     @classmethod
     def remove(cls, key):
-        "Remove key from cache."
-        writeln("CACHE:REMOVE:", key)
+        """Remove key from cache.
+        """
+        log.debug("CACHE:REMOVE: %r", key)
         r = dkredis.connect()
         r.delete(cls.rediskey(key))
 
     @classmethod
     def put(cls, key, value, duration=None):
-        "Put ``value`` in cache, under ``key``, for ``duration`` seconds."
-        writeln("CACHE:PUT[%r] = [[%r]] @%r" % (key, value, duration))
+        """Put ``value`` in cache, under ``key``, for ``duration`` seconds.
+        """
+        # writeln("CACHE:PUT[%r] = [[%r]] @%r" % (key, value, duration))
+        log.debug("CACHE:PUT[%r] = [[%r]] @%r", key, value, duration)
         if duration is None:
             _duration = 30 * 60  # 30 minutes
         elif hasattr(duration, 'to_int'):
             # ttcal.Duration
             _duration = duration.to_int()   # pragma: nocover
         elif hasattr(duration, 'days') and hasattr(duration, 'seconds'):
             # datetime.timedelta
             _duration = duration.days * 24 * 60 * 60 + duration.seconds
         else:
             _duration = int(duration)  # try int conversion, throws ValueError
         assert _duration >= 1  # smallest cache duration is +1 second
 
-        cls.remove(key)
+        # no need to remove an existing key...
+        # cls.remove(key)
 
         k = cls.rediskey(key)
         v = _cache_serialize(value)
 
         r = dkredis.connect()
-        writeln("....cache:put:setex(%r, %r, %r) for %r" % (k, _duration, v, key))
-        r.setex(k, _duration, v)
+        # writeln("....cache:put:setex(%r, %r, %r) for %r" % (
+        #     k, _duration, v, key
+        # ))
+        log.debug("....cache:put:setex(%r, %r, %r) for %r", k, _duration, v, key)
+        r.set(k, v, ex=_duration)
 
     @classmethod
     def _raw_get(cls, key):
         r = dkredis.connect()
-        return r.get(cls.rediskey(key))
-    
+        rkey = cls.rediskey(key)
+        log.debug("KEY: %s, TTL: %r", key, r.ttl(rkey))
+        return r.get(rkey)
+
     @classmethod
     def get(cls, key):
         "Fetch value for ``key`` from redis."
         val = cls._raw_get(key)
         if val is not None:
             res = _cache_unserialize(val)
-            import json
-            writeln("CACHE:GET(%r) => %s" % (key, json.dumps(res, indent=4)))
+            # import json
+            # writeln("CACHE:GET(%r) => %s" % (key, json.dumps(res, indent=4)))
             # writeln("CACHE:GET(%r) => %r" % (key, res))
+            log.debug("CACHE:GET(%r) => %r", key, res)
             return res
-        writeln("CACHE:GET(%r) => NOT-FOUND" % key)
+        # writeln("CACHE:GET(%r) => NOT-FOUND" % key)
+        log.debug("CACHE:GET(%r) => NOT-FOUND", key)
         raise cls.DoesNotExist(
             "Value not in cache (possibly due to expiration).")
 
     @classmethod
     def get_value(cls, key, default=None):
         try:
             return cls.get(key)
         except cls.DoesNotExist:
             return default
 
 
-class djangocache(object):
+class djangocache:
     "Django facade to the rediscache."
-    
+
     @classmethod
     def get(cls, key, default=None):
         return cache.get_value(key, default)
 
     @classmethod
     def set(cls, key, value, duration):
         cache.put(key, value, duration)
 
 
-class Cached(object):
+class Cached:
     """Mixin class to invalidate cache keys on model.save().
 
        Usage::
 
            class MyModel(Cached, models.Model):   # models.Model must be last
                @property
                def cache_keys(self):
@@ -150,15 +161,15 @@
        called).
     """
     cache_keys = []
 
     def save(self, *args, **kwargs):
         for ckey in self.cache_keys:
             cache.remove(ckey)
-        super(Cached, self).save(*args, **kwargs)
+        super().save(*args, **kwargs)
 
     def get_cache_values(self):
         """Get all cached values for this object.
 
            .. Note:: returns None both for keys that are None and
                      non-existant keys!
         """
@@ -188,19 +199,20 @@
     def _cached(func):
         def do_cache(*args, **kws):
             if isinstance(cache_key, str):
                 key = cache_key % locals()
             elif callable(cache_key):
                 key = cache_key(*args, **kws)
             else:
-                key = hashlib.sha1(
-                    (str(func.__module__)
+                key = hashlib.sha1((
+                    str(func.__module__)
                     + str(func.__name__)
                     + str(args)
-                    + str(kws)).encode('ascii')
+                    + str(kws)
+                    ).encode('ascii')
                 ).hexdigest()
             # key = "FNCACHED-" + key
             try:
                 return cache.get(key)
             except cache.DoesNotExist:
                 data = func(*args, **kws)
                 cache.put(key, data, timeout)
```

### Comparing `dkredis-0.1.5/README.rst` & `dkredis-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `dkredis-0.1.5/setup.py` & `dkredis-0.1.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """dkredis - Python interface to Redis
 """
 
 classifiers = """\
-Development Status :: 3 - Alpha
+Development Status :: 5 - Production/Stable
 Intended Audience :: Developers
 Programming Language :: Python
-Programming Language :: Python :: 2
-Programming Language :: Python :: 2.7
 Programming Language :: Python :: 3
 Topic :: Software Development :: Libraries
 """
 
 import setuptools
 
-version = '0.1.5'
+version = '0.1.7'
 
 setuptools.setup(
     name='dkredis',
     version=version,
     install_requires=[
         'redis==3.5.3',
     ],
```

