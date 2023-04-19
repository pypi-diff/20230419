# Comparing `tmp/taichu-serve-2.0.6.tar.gz` & `tmp/taichu-serve-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-serve-2.0.6.tar", last modified: Wed Apr 19 02:08:03 2023, max compression
+gzip compressed data, was "taichu-serve-2.0.7.tar", last modified: Wed Apr 19 02:10:56 2023, max compression
```

## Comparing `taichu-serve-2.0.6.tar` & `taichu-serve-2.0.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:08:03.003566 taichu-serve-2.0.6/
--rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-19 02:08:03.003379 taichu-serve-2.0.6/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-19 02:08:03.003611 taichu-serve-2.0.6/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      947 2023-04-19 02:07:27.000000 taichu-serve-2.0.6/setup.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:08:02.999485 taichu-serve-2.0.6/taichu_serve/
--rw-r--r--   0 chen       (501) staff       (20)     3398 2023-04-14 02:56:12.000000 taichu-serve-2.0.6/taichu_serve/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     9214 2023-04-14 05:19:23.000000 taichu-serve-2.0.6/taichu_serve/app.py
--rw-r--r--   0 chen       (501) staff       (20)     5479 2023-04-19 02:05:09.000000 taichu-serve-2.0.6/taichu_serve/command.py
--rw-r--r--   0 chen       (501) staff       (20)      934 2023-04-18 09:03:28.000000 taichu-serve-2.0.6/taichu_serve/common.py
--rw-r--r--   0 chen       (501) staff       (20)     2110 2023-04-19 02:07:17.000000 taichu-serve-2.0.6/taichu_serve/dockerfile.py
--rw-r--r--   0 chen       (501) staff       (20)     1521 2023-04-14 04:52:00.000000 taichu-serve-2.0.6/taichu_serve/error_code.py
--rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.6/taichu_serve/grpc_predict_v2_pb2.py
--rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.6/taichu_serve/grpc_predict_v2_pb2_grpc.py
--rw-r--r--   0 chen       (501) staff       (20)     4697 2023-04-17 04:31:53.000000 taichu-serve-2.0.6/taichu_serve/grpc_server.py
--rw-r--r--   0 chen       (501) staff       (20)     2104 2023-04-14 09:24:14.000000 taichu-serve-2.0.6/taichu_serve/log.py
--rw-r--r--   0 chen       (501) staff       (20)     5444 2023-04-14 01:39:52.000000 taichu-serve-2.0.6/taichu_serve/model_server.py
--rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.6/taichu_serve/ratelimiter.py
--rw-r--r--   0 chen       (501) staff       (20)     2253 2023-04-19 01:27:54.000000 taichu-serve-2.0.6/taichu_serve/settings.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:08:03.002087 taichu-serve-2.0.6/taichu_serve/template/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.6/taichu_serve/template/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      123 2023-04-18 08:48:18.000000 taichu-serve-2.0.6/taichu_serve/template/config.ini
--rw-r--r--   0 chen       (501) staff       (20)      741 2023-04-18 03:02:30.000000 taichu-serve-2.0.6/taichu_serve/template/customize_service.py
--rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-18 03:02:30.000000 taichu-serve-2.0.6/taichu_serve/template/requirements.txt
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:08:03.003018 taichu-serve-2.0.6/taichu_serve/template/test/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.6/taichu_serve/template/test/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      690 2023-04-18 08:48:18.000000 taichu-serve-2.0.6/taichu_serve/template/test/grpc_client.py
--rw-r--r--   0 chen       (501) staff       (20)      285 2023-04-18 08:45:26.000000 taichu-serve-2.0.6/taichu_serve/template/test/http_client.py
--rw-r--r--   0 chen       (501) staff       (20)      931 2023-04-18 08:48:18.000000 taichu-serve-2.0.6/taichu_serve/template/test/stream_grpc_client.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:08:03.000439 taichu-serve-2.0.6/taichu_serve.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-19 02:08:02.000000 taichu-serve-2.0.6/taichu_serve.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      900 2023-04-19 02:08:02.000000 taichu-serve-2.0.6/taichu_serve.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-19 02:08:02.000000 taichu-serve-2.0.6/taichu_serve.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-19 02:08:02.000000 taichu-serve-2.0.6/taichu_serve.egg-info/entry_points.txt
--rw-r--r--   0 chen       (501) staff       (20)       53 2023-04-19 02:08:02.000000 taichu-serve-2.0.6/taichu_serve.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-19 02:08:02.000000 taichu-serve-2.0.6/taichu_serve.egg-info/top_level.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:10:56.731963 taichu-serve-2.0.7/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-19 02:10:56.731819 taichu-serve-2.0.7/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-19 02:10:56.732005 taichu-serve-2.0.7/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      947 2023-04-19 02:10:51.000000 taichu-serve-2.0.7/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:10:56.728961 taichu-serve-2.0.7/taichu_serve/
+-rw-r--r--   0 chen       (501) staff       (20)     3398 2023-04-14 02:56:12.000000 taichu-serve-2.0.7/taichu_serve/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     9214 2023-04-14 05:19:23.000000 taichu-serve-2.0.7/taichu_serve/app.py
+-rw-r--r--   0 chen       (501) staff       (20)     5479 2023-04-19 02:05:09.000000 taichu-serve-2.0.7/taichu_serve/command.py
+-rw-r--r--   0 chen       (501) staff       (20)      934 2023-04-18 09:03:28.000000 taichu-serve-2.0.7/taichu_serve/common.py
+-rw-r--r--   0 chen       (501) staff       (20)     2109 2023-04-19 02:10:19.000000 taichu-serve-2.0.7/taichu_serve/dockerfile.py
+-rw-r--r--   0 chen       (501) staff       (20)     1521 2023-04-14 04:52:00.000000 taichu-serve-2.0.7/taichu_serve/error_code.py
+-rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.7/taichu_serve/grpc_predict_v2_pb2.py
+-rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.7/taichu_serve/grpc_predict_v2_pb2_grpc.py
+-rw-r--r--   0 chen       (501) staff       (20)     4697 2023-04-17 04:31:53.000000 taichu-serve-2.0.7/taichu_serve/grpc_server.py
+-rw-r--r--   0 chen       (501) staff       (20)     2104 2023-04-14 09:24:14.000000 taichu-serve-2.0.7/taichu_serve/log.py
+-rw-r--r--   0 chen       (501) staff       (20)     5444 2023-04-14 01:39:52.000000 taichu-serve-2.0.7/taichu_serve/model_server.py
+-rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.7/taichu_serve/ratelimiter.py
+-rw-r--r--   0 chen       (501) staff       (20)     2253 2023-04-19 01:27:54.000000 taichu-serve-2.0.7/taichu_serve/settings.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:10:56.730576 taichu-serve-2.0.7/taichu_serve/template/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.7/taichu_serve/template/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      123 2023-04-18 08:48:18.000000 taichu-serve-2.0.7/taichu_serve/template/config.ini
+-rw-r--r--   0 chen       (501) staff       (20)      741 2023-04-18 03:02:30.000000 taichu-serve-2.0.7/taichu_serve/template/customize_service.py
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-18 03:02:30.000000 taichu-serve-2.0.7/taichu_serve/template/requirements.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:10:56.731533 taichu-serve-2.0.7/taichu_serve/template/test/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.7/taichu_serve/template/test/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      690 2023-04-18 08:48:18.000000 taichu-serve-2.0.7/taichu_serve/template/test/grpc_client.py
+-rw-r--r--   0 chen       (501) staff       (20)      285 2023-04-18 08:45:26.000000 taichu-serve-2.0.7/taichu_serve/template/test/http_client.py
+-rw-r--r--   0 chen       (501) staff       (20)      931 2023-04-18 08:48:18.000000 taichu-serve-2.0.7/taichu_serve/template/test/stream_grpc_client.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:10:56.729943 taichu-serve-2.0.7/taichu_serve.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-19 02:10:56.000000 taichu-serve-2.0.7/taichu_serve.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      900 2023-04-19 02:10:56.000000 taichu-serve-2.0.7/taichu_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-19 02:10:56.000000 taichu-serve-2.0.7/taichu_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-19 02:10:56.000000 taichu-serve-2.0.7/taichu_serve.egg-info/entry_points.txt
+-rw-r--r--   0 chen       (501) staff       (20)       53 2023-04-19 02:10:56.000000 taichu-serve-2.0.7/taichu_serve.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-19 02:10:56.000000 taichu-serve-2.0.7/taichu_serve.egg-info/top_level.txt
```

### Comparing `taichu-serve-2.0.6/setup.py` & `taichu-serve-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     name = 'taichu-serve'
 
     requirements = ['grpcio', 'grpcio-tools', 'protobuf',
                     'Flask', 'gunicorn', 'requests']
 
     setup(
         name=name,
-        version='2.0.6',
+        version='2.0.7',
         description='taichu serve is a tool for serving deep learning inference',
         # long_description='',
         author='taichu platform team',
         # author_email='noreply@noreply.com',
         python_requires=">=3.6.0",
         url='',
         keywords='Serving Deep Learning Inference AI',
```

### Comparing `taichu-serve-2.0.6/taichu_serve/__init__.py` & `taichu-serve-2.0.7/taichu_serve/__init__.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.6/taichu_serve/app.py` & `taichu-serve-2.0.7/taichu_serve/app.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.6/taichu_serve/command.py` & `taichu-serve-2.0.7/taichu_serve/command.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.6/taichu_serve/common.py` & `taichu-serve-2.0.7/taichu_serve/common.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.6/taichu_serve/dockerfile.py` & `taichu-serve-2.0.7/taichu_serve/dockerfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,17 @@
 ENTRYPOINT ["/bin/bash"]
 CMD bash /opt/launch.sh
 
 # 构建镜像命令： docker build -t taichu-serve-env .
 # 运行镜像命令： docker run -it  -v $PWD:/home taichu-serve-env bash
 """
 
-launch_sh_template = """
+launch_sh_template = """#!/bin/bash
 # 请不要修改这个文件
 # Do Not Modify This File
-#!/bin/bash
 
 default_triton_grpc_port=50000
 default_grpc_port=8080
 default_http_port=8081
 
 
 if [ -z $triton_grpc_port ];then
```

### Comparing `taichu-serve-2.0.6/taichu_serve/error_code.py` & `taichu-serve-2.0.7/taichu_serve/error_code.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.6/taichu_serve/grpc_predict_v2_pb2.py` & `taichu-serve-2.0.7/taichu_serve/grpc_predict_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.6/taichu_serve/grpc_predict_v2_pb2_grpc.py` & `taichu-serve-2.0.7/taichu_serve/grpc_predict_v2_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.6/taichu_serve/grpc_server.py` & `taichu-serve-2.0.7/taichu_serve/grpc_server.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.6/taichu_serve/log.py` & `taichu-serve-2.0.7/taichu_serve/log.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.6/taichu_serve/model_server.py` & `taichu-serve-2.0.7/taichu_serve/model_server.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.6/taichu_serve/settings.py` & `taichu-serve-2.0.7/taichu_serve/settings.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.6/taichu_serve/template/customize_service.py` & `taichu-serve-2.0.7/taichu_serve/template/customize_service.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.6/taichu_serve/template/test/grpc_client.py` & `taichu-serve-2.0.7/taichu_serve/template/test/grpc_client.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.6/taichu_serve/template/test/stream_grpc_client.py` & `taichu-serve-2.0.7/taichu_serve/template/test/stream_grpc_client.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.6/taichu_serve.egg-info/SOURCES.txt` & `taichu-serve-2.0.7/taichu_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

