# Comparing `tmp/flask_redis_ex-0.0.1-py3-none-any.whl.zip` & `tmp/flask_redis_ex-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1543 bytes, number of entries: 5
--rw-rw-r--  2.0 unx      429 b- defN 23-Apr-19 14:20 flask_redis_ex/__init__.py
--rw-rw-r--  2.0 unx      286 b- defN 23-Apr-19 14:42 flask_redis_ex-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 14:42 flask_redis_ex-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-19 14:42 flask_redis_ex-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      407 b- defN 23-Apr-19 14:42 flask_redis_ex-0.0.1.dist-info/RECORD
-5 files, 1229 bytes uncompressed, 777 bytes compressed:  36.8%
+Zip file size: 1698 bytes, number of entries: 5
+-rw-rw-r--  2.0 unx      434 b- defN 23-Apr-19 15:00 flask_redis_ex/__init__.py
+-rw-rw-r--  2.0 unx      570 b- defN 23-Apr-19 15:10 flask_redis_ex-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 15:10 flask_redis_ex-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-19 15:10 flask_redis_ex-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      407 b- defN 23-Apr-19 15:10 flask_redis_ex-0.0.2.dist-info/RECORD
+5 files, 1518 bytes uncompressed, 932 bytes compressed:  38.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: flask_redis_ex/__init__.py
 Comment: 
 
-Filename: flask_redis_ex-0.0.1.dist-info/METADATA
+Filename: flask_redis_ex-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: flask_redis_ex-0.0.1.dist-info/WHEEL
+Filename: flask_redis_ex-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: flask_redis_ex-0.0.1.dist-info/top_level.txt
+Filename: flask_redis_ex-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: flask_redis_ex-0.0.1.dist-info/RECORD
+Filename: flask_redis_ex-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flask_redis_ex/__init__.py

```diff
@@ -1,13 +1,13 @@
 from flask import current_app
 from werkzeug.local import LocalProxy
 
 import redis
 
 def _get_client():
-    if not hasattr(current_app, 'redisClient') or current_app.redisClient is None:
+    if not hasattr(current_app, 'redis_client') or current_app.redis_client is None:
         config = current_app.config
         redis_url = config.get("REDIS_URL")
-        current_app.redisClient = redis.from_url(redis_url)
-    return getattr(current_app, 'redisClient', None)
+        current_app.redis_client = redis.from_url(redis_url)
+    return getattr(current_app, 'redis_client', None)
 
-redisClient: redis.Redis = LocalProxy(_get_client)
+redis_client: redis.Redis = LocalProxy(_get_client)
```

