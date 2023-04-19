# Comparing `tmp/taichu-serve-2.0.12.tar.gz` & `tmp/taichu-serve-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-serve-2.0.12.tar", last modified: Wed Apr 19 04:47:03 2023, max compression
+gzip compressed data, was "taichu-serve-2.0.9.tar", last modified: Wed Apr 19 02:34:49 2023, max compression
```

## Comparing `taichu-serve-2.0.12.tar` & `taichu-serve-2.0.9.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 04:47:03.799710 taichu-serve-2.0.12/
--rw-r--r--   0 chen       (501) staff       (20)     2043 2023-04-19 04:47:03.799515 taichu-serve-2.0.12/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)     1762 2023-04-19 04:38:09.000000 taichu-serve-2.0.12/README.md
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-19 04:47:03.799750 taichu-serve-2.0.12/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)     1061 2023-04-19 04:47:01.000000 taichu-serve-2.0.12/setup.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 04:47:03.797546 taichu-serve-2.0.12/taichu_serve/
--rw-r--r--   0 chen       (501) staff       (20)     3398 2023-04-14 02:56:12.000000 taichu-serve-2.0.12/taichu_serve/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     9214 2023-04-14 05:19:23.000000 taichu-serve-2.0.12/taichu_serve/app.py
--rw-r--r--   0 chen       (501) staff       (20)     5458 2023-04-19 04:46:32.000000 taichu-serve-2.0.12/taichu_serve/command.py
--rw-r--r--   0 chen       (501) staff       (20)      934 2023-04-18 09:03:28.000000 taichu-serve-2.0.12/taichu_serve/common.py
--rw-r--r--   0 chen       (501) staff       (20)     2375 2023-04-19 04:44:22.000000 taichu-serve-2.0.12/taichu_serve/dockerfile.py
--rw-r--r--   0 chen       (501) staff       (20)     1521 2023-04-14 04:52:00.000000 taichu-serve-2.0.12/taichu_serve/error_code.py
--rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.12/taichu_serve/grpc_predict_v2_pb2.py
--rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.12/taichu_serve/grpc_predict_v2_pb2_grpc.py
--rw-r--r--   0 chen       (501) staff       (20)     4697 2023-04-17 04:31:53.000000 taichu-serve-2.0.12/taichu_serve/grpc_server.py
--rw-r--r--   0 chen       (501) staff       (20)     2104 2023-04-14 09:24:14.000000 taichu-serve-2.0.12/taichu_serve/log.py
--rw-r--r--   0 chen       (501) staff       (20)     5444 2023-04-14 01:39:52.000000 taichu-serve-2.0.12/taichu_serve/model_server.py
--rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.12/taichu_serve/ratelimiter.py
--rw-r--r--   0 chen       (501) staff       (20)     2258 2023-04-19 03:58:12.000000 taichu-serve-2.0.12/taichu_serve/settings.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 04:47:03.798644 taichu-serve-2.0.12/taichu_serve/template/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.12/taichu_serve/template/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      741 2023-04-18 03:02:30.000000 taichu-serve-2.0.12/taichu_serve/template/customize_service.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 04:47:03.799276 taichu-serve-2.0.12/taichu_serve/template/test/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.12/taichu_serve/template/test/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      690 2023-04-18 08:48:18.000000 taichu-serve-2.0.12/taichu_serve/template/test/grpc_client.py
--rw-r--r--   0 chen       (501) staff       (20)      285 2023-04-18 08:45:26.000000 taichu-serve-2.0.12/taichu_serve/template/test/http_client.py
--rw-r--r--   0 chen       (501) staff       (20)      931 2023-04-18 08:48:18.000000 taichu-serve-2.0.12/taichu_serve/template/test/stream_grpc_client.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 04:47:03.798402 taichu-serve-2.0.12/taichu_serve.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)     2043 2023-04-19 04:47:03.000000 taichu-serve-2.0.12/taichu_serve.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      838 2023-04-19 04:47:03.000000 taichu-serve-2.0.12/taichu_serve.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-19 04:47:03.000000 taichu-serve-2.0.12/taichu_serve.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       59 2023-04-19 04:47:03.000000 taichu-serve-2.0.12/taichu_serve.egg-info/entry_points.txt
--rw-r--r--   0 chen       (501) staff       (20)       53 2023-04-19 04:47:03.000000 taichu-serve-2.0.12/taichu_serve.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-19 04:47:03.000000 taichu-serve-2.0.12/taichu_serve.egg-info/top_level.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.797402 taichu-serve-2.0.9/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-19 02:34:49.797253 taichu-serve-2.0.9/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-19 02:34:49.797443 taichu-serve-2.0.9/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      947 2023-04-19 02:34:18.000000 taichu-serve-2.0.9/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.793674 taichu-serve-2.0.9/taichu_serve/
+-rw-r--r--   0 chen       (501) staff       (20)     3398 2023-04-14 02:56:12.000000 taichu-serve-2.0.9/taichu_serve/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     9214 2023-04-14 05:19:23.000000 taichu-serve-2.0.9/taichu_serve/app.py
+-rw-r--r--   0 chen       (501) staff       (20)     5479 2023-04-19 02:05:09.000000 taichu-serve-2.0.9/taichu_serve/command.py
+-rw-r--r--   0 chen       (501) staff       (20)      934 2023-04-18 09:03:28.000000 taichu-serve-2.0.9/taichu_serve/common.py
+-rw-r--r--   0 chen       (501) staff       (20)     2118 2023-04-19 02:34:18.000000 taichu-serve-2.0.9/taichu_serve/dockerfile.py
+-rw-r--r--   0 chen       (501) staff       (20)     1521 2023-04-14 04:52:00.000000 taichu-serve-2.0.9/taichu_serve/error_code.py
+-rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2.py
+-rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2_grpc.py
+-rw-r--r--   0 chen       (501) staff       (20)     4697 2023-04-17 04:31:53.000000 taichu-serve-2.0.9/taichu_serve/grpc_server.py
+-rw-r--r--   0 chen       (501) staff       (20)     2104 2023-04-14 09:24:14.000000 taichu-serve-2.0.9/taichu_serve/log.py
+-rw-r--r--   0 chen       (501) staff       (20)     5444 2023-04-14 01:39:52.000000 taichu-serve-2.0.9/taichu_serve/model_server.py
+-rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.9/taichu_serve/ratelimiter.py
+-rw-r--r--   0 chen       (501) staff       (20)     2253 2023-04-19 01:27:54.000000 taichu-serve-2.0.9/taichu_serve/settings.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.795889 taichu-serve-2.0.9/taichu_serve/template/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.9/taichu_serve/template/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      123 2023-04-18 08:48:18.000000 taichu-serve-2.0.9/taichu_serve/template/config.ini
+-rw-r--r--   0 chen       (501) staff       (20)      741 2023-04-18 03:02:30.000000 taichu-serve-2.0.9/taichu_serve/template/customize_service.py
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-18 03:02:30.000000 taichu-serve-2.0.9/taichu_serve/template/requirements.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.796946 taichu-serve-2.0.9/taichu_serve/template/test/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.9/taichu_serve/template/test/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      690 2023-04-18 08:48:18.000000 taichu-serve-2.0.9/taichu_serve/template/test/grpc_client.py
+-rw-r--r--   0 chen       (501) staff       (20)      285 2023-04-18 08:45:26.000000 taichu-serve-2.0.9/taichu_serve/template/test/http_client.py
+-rw-r--r--   0 chen       (501) staff       (20)      931 2023-04-18 08:48:18.000000 taichu-serve-2.0.9/taichu_serve/template/test/stream_grpc_client.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.794937 taichu-serve-2.0.9/taichu_serve.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      900 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/entry_points.txt
+-rw-r--r--   0 chen       (501) staff       (20)       53 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/top_level.txt
```

### Comparing `taichu-serve-2.0.12/setup.py` & `taichu-serve-2.0.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,23 +8,19 @@
 
 if __name__ == '__main__':
     name = 'taichu-serve'
 
     requirements = ['grpcio', 'grpcio-tools', 'protobuf',
                     'Flask', 'gunicorn', 'requests']
 
-    long_description = ''
-    with open('README.md', 'r') as f:
-        long_description = f.read()
-
     setup(
         name=name,
-        version='2.0.12',
+        version='2.0.9',
         description='taichu serve is a tool for serving deep learning inference',
-        long_description=long_description,
+        # long_description='',
         author='taichu platform team',
         # author_email='noreply@noreply.com',
         python_requires=">=3.6.0",
         url='',
         keywords='Serving Deep Learning Inference AI',
         packages=pkgs,
         install_requires=requirements,
```

### Comparing `taichu-serve-2.0.12/taichu_serve/__init__.py` & `taichu-serve-2.0.9/taichu_serve/__init__.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.12/taichu_serve/app.py` & `taichu-serve-2.0.9/taichu_serve/app.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.12/taichu_serve/command.py` & `taichu-serve-2.0.9/taichu_serve/command.py`

 * *Files 20% similar despite different names*

```diff
@@ -53,19 +53,16 @@
 
     with open(os.path.join(name, "dependencies.txt"), "w") as f:
         f.write("# 请在这里添加apt-get安装的依赖，每行一个依赖，如：curl")
     print("create file: ", os.path.join(name, "dependencies.txt"))
     print("init project done!")
 
 
-def build_env(name, base_image):
-    # 检查镜像名称是否合法
-    if name is None or name == "":
-        name = "taichu-serve-env"
-
+def build_env(base_image):
+    # 1. 创建dockerfile
     if base_image is None or base_image == "":
         base_image = "swr.cn-central-221.ovaijisuan.com/wair/taichu-serve:latest"
     if os.path.exists("Dockerfile"):
         print("Dockerfile已存在，请删除后重试！")
         return
 
     if os.path.exists("launch.sh"):
@@ -101,36 +98,35 @@
     print("create file: ", "launch.sh")
     with open("Dockerfile", "w") as f:
         f.write(dockerfile_content)
     print("create file: ", "Dockerfile")
 
     print("build docker image...")
     tag = uuid.uuid4().hex[:8]
-    image_name = f"{name}:{tag}"
-    cmd = f"docker build -t {image_name} ."
-    print(f"[CMD] {cmd} ")
+    print("[CMD] docker build -t taichu-serve-env:{tag} .".format(tag=tag))
+    cmd = "docker build -t taichu-serve-env:{tag} .".format(tag=tag)
     os.system(cmd)
     print("build docker image done!")
 
     print("进入镜像调试命令：")
-    print(f"[CMD] docker run -it -p 8080:8080 -p 8081:8081 -v $PWD:/home {image_name} bash")
-    print("调试完成后，可以使用以下命令将镜像推送到仓库：")
+    print("[CMD] docker run -it -p 8080:8080 -p 8081:8081 -v $PWD:/home taichu-serve-env:{tag} bash".format(tag=tag))
 
-    print("[CMD] docker tag {image_name} swr.cn-central-221.ovaijisuan.com/wair/{image_name}".format(
-        image_name=image_name))
+    print("调试完成后，可以使用以下命令将镜像推送到仓库：")
+    image_name = "taichu-serve-env:{tag}".format(tag=tag)
+    print("[CMD] docker tag {image_name} swr.cn-central-221.ovaijisuan.com/wair/{image_name}".format(image_name=image_name))
     print("[CMD] docker push swr.cn-central-221.ovaijisuan.com/wair/{image_name}".format(image_name=image_name))
 
 
 def cli():
     args = parse_args()
     if args.action == "init":
         init_project()
         return
-    if args.action == "build":
-        build_env(args.name, args.from_image)
+    if args.action == "build_env":
+        build_env(args.base_image)
         return
 
     init_model_service_instance()
     server = grpc.server(futures.ThreadPoolExecutor(max_workers=args.max_concurrent_requests),
                          maximum_concurrent_rpcs=args.max_concurrent_requests + 5,
                          interceptors=[GrpcServerInterceptor()])
```

### Comparing `taichu-serve-2.0.12/taichu_serve/common.py` & `taichu-serve-2.0.9/taichu_serve/common.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.12/taichu_serve/dockerfile.py` & `taichu-serve-2.0.9/taichu_serve/dockerfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,32 +6,29 @@
 
 USER root
 
 WORKDIR /opt
 COPY ./launch.sh /opt/launch.sh
 COPY ./requirements.txt /opt/requirements.txt
 
-RUN chmod -R 777 /opt/launch.sh && chmod -R 777 /opt/requirements.txt
+RUN chmod -R 777 /opt
 RUN chmod -R 777 /home
 
 # 安装apt依赖
 {apt_install}
 
 RUN pip3 install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple
 
 WORKDIR /home
 
 ENTRYPOINT ["/bin/bash", "-c"]
 CMD ["/opt/launch.sh"]
 
 # 构建镜像命令： docker build -t taichu-serve-env .
 # 运行镜像命令： docker run -it  -v $PWD:/home taichu-serve-env bash
-# 推送镜像命令： 
-#               docker tag taichu-serve-env swr.cn-central-221.ovaijisuan.com/wair/taichu-serve-env
-#               docker push swr.cn-central-221.ovaijisuan.com/wair/taichu-serve-env
 """
 
 launch_sh_template = """#!/bin/bash
 # 请不要修改这个文件
 # Do Not Modify This File
 
 default_triton_grpc_port=50000
```

### Comparing `taichu-serve-2.0.12/taichu_serve/error_code.py` & `taichu-serve-2.0.9/taichu_serve/error_code.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.12/taichu_serve/grpc_predict_v2_pb2.py` & `taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.12/taichu_serve/grpc_predict_v2_pb2_grpc.py` & `taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.12/taichu_serve/grpc_server.py` & `taichu-serve-2.0.9/taichu_serve/grpc_server.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.12/taichu_serve/log.py` & `taichu-serve-2.0.9/taichu_serve/log.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.12/taichu_serve/model_server.py` & `taichu-serve-2.0.9/taichu_serve/model_server.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.12/taichu_serve/settings.py` & `taichu-serve-2.0.9/taichu_serve/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 DEFAULT_TF_SERVER_PORT = 8500
 
 logger = logging.getLogger(__name__)
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Taichu Model Server')
-    parser.add_argument('action', action="store", choices=['init', 'run', 'build'])
+    parser.add_argument('action', action="store", choices=['init', 'run', 'build_env'])
 
-    parser.add_argument('--from_image', action="store",
+    parser.add_argument('--base_image', action="store",
                         default='swr.cn-central-221.ovaijisuan.com/wair/taichu-serve:latest', type=str)
-    parser.add_argument('--name', action="store", default='taichu-serve-env', type=str)
+    # parser.add_argument('name', action="store", default='default', type=str)
 
     parser.add_argument('--grpc_port', action="store", default=8080, type=int)
     parser.add_argument('--http_port', action="store", default=8081, type=int)
     parser.add_argument('--grpc_only', action="store", default=False, type=bool)
     parser.add_argument('--model_path', action="store", default='./', type=str)
     parser.add_argument('--service_file', action="store", default='customize_service.py', type=str)
     parser.add_argument('--max_concurrent_requests', action="store", default=1, type=int)
```

### Comparing `taichu-serve-2.0.12/taichu_serve/template/customize_service.py` & `taichu-serve-2.0.9/taichu_serve/template/customize_service.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.12/taichu_serve/template/test/grpc_client.py` & `taichu-serve-2.0.9/taichu_serve/template/test/grpc_client.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.12/taichu_serve/template/test/stream_grpc_client.py` & `taichu-serve-2.0.9/taichu_serve/template/test/stream_grpc_client.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.12/taichu_serve.egg-info/SOURCES.txt` & `taichu-serve-2.0.9/taichu_serve.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-README.md
 setup.py
 taichu_serve/__init__.py
 taichu_serve/app.py
 taichu_serve/command.py
 taichu_serve/common.py
 taichu_serve/dockerfile.py
 taichu_serve/error_code.py
@@ -16,12 +15,14 @@
 taichu_serve.egg-info/PKG-INFO
 taichu_serve.egg-info/SOURCES.txt
 taichu_serve.egg-info/dependency_links.txt
 taichu_serve.egg-info/entry_points.txt
 taichu_serve.egg-info/requires.txt
 taichu_serve.egg-info/top_level.txt
 taichu_serve/template/__init__.py
+taichu_serve/template/config.ini
 taichu_serve/template/customize_service.py
+taichu_serve/template/requirements.txt
 taichu_serve/template/test/__init__.py
 taichu_serve/template/test/grpc_client.py
 taichu_serve/template/test/http_client.py
 taichu_serve/template/test/stream_grpc_client.py
```

