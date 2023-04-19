# Comparing `tmp/gTixi-1.1.0.tar.gz` & `tmp/gTixi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gTixi-1.1.0.tar", last modified: Wed Apr 19 01:37:38 2023, max compression
+gzip compressed data, was "gTixi-1.1.1.tar", last modified: Wed Apr 19 01:59:14 2023, max compression
```

## Comparing `gTixi-1.1.0.tar` & `gTixi-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 01:37:38.064627 gTixi-1.1.0/
--rw-rw-rw-   0        0        0     1091 2022-12-02 07:39:30.000000 gTixi-1.1.0/LICENSE
--rw-rw-rw-   0        0        0    30401 2023-04-19 01:37:38.060630 gTixi-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    29967 2023-04-19 01:36:27.000000 gTixi-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 01:37:38.006652 gTixi-1.1.0/gTixi/
--rw-rw-rw-   0        0        0     5570 2023-04-10 02:42:27.000000 gTixi-1.1.0/gTixi/SSD1306.py
--rw-rw-rw-   0        0        0     1116 2023-01-04 05:19:56.000000 gTixi-1.1.0/gTixi/__init__.py
--rw-rw-rw-   0        0        0    11875 2022-12-12 09:01:56.000000 gTixi-1.1.0/gTixi/alib.py
-drwxrwxrwx   0        0        0        0 2023-04-19 01:37:38.056628 gTixi-1.1.0/gTixi/gpio4/
--rw-rw-rw-   0        0        0    22841 2022-12-12 09:01:56.000000 gTixi-1.1.0/gTixi/gpio4/__init__.py
--rw-rw-rw-   0        0        0     4478 2022-12-12 09:01:56.000000 gTixi-1.1.0/gTixi/gpio4/arduino.py
--rw-rw-rw-   0        0        0     2107 2022-12-12 09:01:56.000000 gTixi-1.1.0/gTixi/gpio4/constants.py
--rw-rw-rw-   0        0        0     8211 2023-01-09 07:29:18.000000 gTixi-1.1.0/gTixi/gpioPins.py
--rw-rw-rw-   0        0        0     7559 2023-03-01 08:39:59.000000 gTixi-1.1.0/gTixi/starMod.py
--rw-rw-rw-   0        0        0     9243 2023-04-19 01:27:41.000000 gTixi-1.1.0/gTixi/starServer.py
--rw-rw-rw-   0        0        0     6388 2023-01-05 08:57:38.000000 gTixi-1.1.0/gTixi/wLTR390.py
--rw-rw-rw-   0        0        0    15044 2023-01-09 03:55:14.000000 gTixi-1.1.0/gTixi/waDrivers.py
--rw-rw-rw-   0        0        0     4118 2023-03-01 01:49:26.000000 gTixi-1.1.0/gTixi/waFile.py
--rw-rw-rw-   0        0        0     5983 2022-12-12 09:01:56.000000 gTixi-1.1.0/gTixi/waText.py
--rw-rw-rw-   0        0        0    22878 2023-04-11 00:41:59.000000 gTixi-1.1.0/gTixi/wadapter.py
-drwxrwxrwx   0        0        0        0 2023-04-19 01:37:38.037629 gTixi-1.1.0/gTixi.egg-info/
--rw-rw-rw-   0        0        0    30401 2023-04-19 01:37:36.000000 gTixi-1.1.0/gTixi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-04-19 01:37:36.000000 gTixi-1.1.0/gTixi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 01:37:36.000000 gTixi-1.1.0/gTixi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 01:37:36.000000 gTixi-1.1.0/gTixi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 01:37:38.064627 gTixi-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-04-19 01:37:28.000000 gTixi-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:59:14.540087 gTixi-1.1.1/
+-rw-rw-rw-   0        0        0     1091 2022-12-02 07:39:30.000000 gTixi-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      123 2023-04-19 01:59:01.000000 gTixi-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    30481 2023-04-19 01:59:14.539084 gTixi-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    30047 2023-04-19 01:54:32.000000 gTixi-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 01:59:14.417084 gTixi-1.1.1/gTixi/
+-rw-rw-rw-   0        0        0   456248 2023-04-10 07:25:40.000000 gTixi-1.1.1/gTixi/Dianzhen.ttf
+-rw-rw-rw-   0        0        0     5570 2023-04-10 02:42:27.000000 gTixi-1.1.1/gTixi/SSD1306.py
+-rw-rw-rw-   0        0        0     1116 2023-01-04 05:19:56.000000 gTixi-1.1.1/gTixi/__init__.py
+-rw-rw-rw-   0        0        0    11875 2022-12-12 09:01:56.000000 gTixi-1.1.1/gTixi/alib.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:59:14.451091 gTixi-1.1.1/gTixi/gpio4/
+-rw-rw-rw-   0        0        0    22841 2022-12-12 09:01:56.000000 gTixi-1.1.1/gTixi/gpio4/__init__.py
+-rw-rw-rw-   0        0        0     4478 2022-12-12 09:01:56.000000 gTixi-1.1.1/gTixi/gpio4/arduino.py
+-rw-rw-rw-   0        0        0     2107 2022-12-12 09:01:56.000000 gTixi-1.1.1/gTixi/gpio4/constants.py
+-rw-rw-rw-   0        0        0     8211 2023-01-09 07:29:18.000000 gTixi-1.1.1/gTixi/gpioPins.py
+-rw-rw-rw-   0        0        0     7559 2023-03-01 08:39:59.000000 gTixi-1.1.1/gTixi/starMod.py
+-rw-rw-rw-   0        0        0     9243 2023-04-19 01:27:41.000000 gTixi-1.1.1/gTixi/starServer.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:59:14.535086 gTixi-1.1.1/gTixi/stardevice/
+-rw-rw-rw-   0        0        0     1150 2022-12-08 00:17:57.000000 gTixi-1.1.1/gTixi/stardevice/favicon.ico
+-rw-rw-rw-   0        0        0     3690 2023-04-19 01:15:50.000000 gTixi-1.1.1/gTixi/stardevice/index.html
+-rw-rw-rw-   0        0        0   111756 2022-12-08 00:17:57.000000 gTixi-1.1.1/gTixi/stardevice/socket.io.js
+-rw-rw-rw-   0        0        0   128872 2023-04-19 00:50:09.000000 gTixi-1.1.1/gTixi/stardevice/vue.global.js
+-rw-rw-rw-   0        0        0     6388 2023-01-05 08:57:38.000000 gTixi-1.1.1/gTixi/wLTR390.py
+-rw-rw-rw-   0        0        0    15044 2023-01-09 03:55:14.000000 gTixi-1.1.1/gTixi/waDrivers.py
+-rw-rw-rw-   0        0        0     4118 2023-03-01 01:49:26.000000 gTixi-1.1.1/gTixi/waFile.py
+-rw-rw-rw-   0        0        0     5983 2022-12-12 09:01:56.000000 gTixi-1.1.1/gTixi/waText.py
+-rw-rw-rw-   0        0        0    22878 2023-04-11 00:41:59.000000 gTixi-1.1.1/gTixi/wadapter.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:59:14.442085 gTixi-1.1.1/gTixi.egg-info/
+-rw-rw-rw-   0        0        0    30481 2023-04-19 01:59:13.000000 gTixi-1.1.1/gTixi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2023-04-19 01:59:14.000000 gTixi-1.1.1/gTixi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 01:59:13.000000 gTixi-1.1.1/gTixi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 01:59:13.000000 gTixi-1.1.1/gTixi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 01:59:14.540087 gTixi-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      698 2023-04-19 01:51:25.000000 gTixi-1.1.1/setup.py
```

### Comparing `gTixi-1.1.0/LICENSE` & `gTixi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/PKG-INFO` & `gTixi-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gTixi
-Version: 1.1.0
+Version: 1.1.1
 Summary: 高效碳基演示体系核心模块
 Home-page: https://gitee.com/lxwk1spectre/walartminstar
 Author: Spectre Lee
 Author-email: lxwk1spectre@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -610,14 +610,17 @@
 ### gpiopin(p0,p1)
 gpio调试工具，可以用于掌控版和未来板
 - p0:bool,p1:bool
     - p0针脚和p1针脚的输出，True为高电平，False为低电平
 - 返回：sf:str
     - 用于显示在显示屏上的字符串
 # 版本迭代
+## 1.1.1
+- 230319
+    - 加入MAINFEST.in文件，处理非py文件的打包
 ## 1.1.0
 - 230319
     - 将smp的字体文件，webUI的网页文件压缩，一起内置如gTixi中，整个包大小控制在了1M以内。
     - 禁止了httpserver和websocketsServer的自启动，现在在import gTixi时不会启动任何服务，仅在需要的时候开启。
     - 去掉了大量print的提示，使得gTixi使用起来更加纯净。
 ## 1.0.1
 - 230328
```

### Comparing `gTixi-1.1.0/README.md` & `gTixi-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -597,14 +597,17 @@
 ### gpiopin(p0,p1)
 gpio调试工具，可以用于掌控版和未来板
 - p0:bool,p1:bool
     - p0针脚和p1针脚的输出，True为高电平，False为低电平
 - 返回：sf:str
     - 用于显示在显示屏上的字符串
 # 版本迭代
+## 1.1.1
+- 230319
+    - 加入MAINFEST.in文件，处理非py文件的打包
 ## 1.1.0
 - 230319
     - 将smp的字体文件，webUI的网页文件压缩，一起内置如gTixi中，整个包大小控制在了1M以内。
     - 禁止了httpserver和websocketsServer的自启动，现在在import gTixi时不会启动任何服务，仅在需要的时候开启。
     - 去掉了大量print的提示，使得gTixi使用起来更加纯净。
 ## 1.0.1
 - 230328
```

### Comparing `gTixi-1.1.0/gTixi/SSD1306.py` & `gTixi-1.1.1/gTixi/SSD1306.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/gTixi/__init__.py` & `gTixi-1.1.1/gTixi/__init__.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/gTixi/alib.py` & `gTixi-1.1.1/gTixi/alib.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/gTixi/gpio4/__init__.py` & `gTixi-1.1.1/gTixi/gpio4/__init__.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/gTixi/gpio4/arduino.py` & `gTixi-1.1.1/gTixi/gpio4/arduino.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/gTixi/gpio4/constants.py` & `gTixi-1.1.1/gTixi/gpio4/constants.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/gTixi/gpioPins.py` & `gTixi-1.1.1/gTixi/gpioPins.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/gTixi/starMod.py` & `gTixi-1.1.1/gTixi/starMod.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/gTixi/starServer.py` & `gTixi-1.1.1/gTixi/starServer.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/gTixi/wLTR390.py` & `gTixi-1.1.1/gTixi/wLTR390.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/gTixi/waDrivers.py` & `gTixi-1.1.1/gTixi/waDrivers.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/gTixi/waFile.py` & `gTixi-1.1.1/gTixi/waFile.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/gTixi/waText.py` & `gTixi-1.1.1/gTixi/waText.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/gTixi/wadapter.py` & `gTixi-1.1.1/gTixi/wadapter.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.0/gTixi.egg-info/PKG-INFO` & `gTixi-1.1.1/gTixi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gTixi
-Version: 1.1.0
+Version: 1.1.1
 Summary: 高效碳基演示体系核心模块
 Home-page: https://gitee.com/lxwk1spectre/walartminstar
 Author: Spectre Lee
 Author-email: lxwk1spectre@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -610,14 +610,17 @@
 ### gpiopin(p0,p1)
 gpio调试工具，可以用于掌控版和未来板
 - p0:bool,p1:bool
     - p0针脚和p1针脚的输出，True为高电平，False为低电平
 - 返回：sf:str
     - 用于显示在显示屏上的字符串
 # 版本迭代
+## 1.1.1
+- 230319
+    - 加入MAINFEST.in文件，处理非py文件的打包
 ## 1.1.0
 - 230319
     - 将smp的字体文件，webUI的网页文件压缩，一起内置如gTixi中，整个包大小控制在了1M以内。
     - 禁止了httpserver和websocketsServer的自启动，现在在import gTixi时不会启动任何服务，仅在需要的时候开启。
     - 去掉了大量print的提示，使得gTixi使用起来更加纯净。
 ## 1.0.1
 - 230328
```

### Comparing `gTixi-1.1.0/setup.py` & `gTixi-1.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gTixi",
-    version="1.1.0",
+    version="1.1.1",
     author="Spectre Lee",
     author_email="lxwk1spectre@foxmail.com",
     description="高效碳基演示体系核心模块",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    include_package_data=True,
     url="https://gitee.com/lxwk1spectre/walartminstar",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

