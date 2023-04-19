# Comparing `tmp/gTixi-1.0.0.tar.gz` & `tmp/gTixi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gTixi-1.0.0.tar", last modified: Fri Mar 10 07:14:42 2023, max compression
+gzip compressed data, was "gTixi-1.1.0.tar", last modified: Wed Apr 19 01:37:38 2023, max compression
```

## Comparing `gTixi-1.0.0.tar` & `gTixi-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 07:14:42.747099 gTixi-1.0.0/
--rw-rw-rw-   0        0        0     1091 2022-12-02 07:39:30.000000 gTixi-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    29745 2023-03-10 07:14:42.745084 gTixi-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    29311 2023-03-08 00:36:53.000000 gTixi-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-10 07:14:42.711112 gTixi-1.0.0/gTixi/
--rw-rw-rw-   0        0        0     1116 2023-01-04 05:19:56.000000 gTixi-1.0.0/gTixi/__init__.py
--rw-rw-rw-   0        0        0    11875 2022-12-12 09:01:56.000000 gTixi-1.0.0/gTixi/alib.py
-drwxrwxrwx   0        0        0        0 2023-03-10 07:14:42.742085 gTixi-1.0.0/gTixi/gpio4/
--rw-rw-rw-   0        0        0    22841 2022-12-12 09:01:56.000000 gTixi-1.0.0/gTixi/gpio4/__init__.py
--rw-rw-rw-   0        0        0     4478 2022-12-12 09:01:56.000000 gTixi-1.0.0/gTixi/gpio4/arduino.py
--rw-rw-rw-   0        0        0     2107 2022-12-12 09:01:56.000000 gTixi-1.0.0/gTixi/gpio4/constants.py
--rw-rw-rw-   0        0        0     8211 2023-01-09 07:29:18.000000 gTixi-1.0.0/gTixi/gpioPins.py
--rw-rw-rw-   0        0        0     7559 2023-01-09 01:44:01.000000 gTixi-1.0.0/gTixi/starMod.py
--rw-rw-rw-   0        0        0     8756 2023-01-11 01:38:14.000000 gTixi-1.0.0/gTixi/starServer.py
--rw-rw-rw-   0        0        0     6388 2023-01-05 08:57:38.000000 gTixi-1.0.0/gTixi/wLTR390.py
--rw-rw-rw-   0        0        0    15044 2023-01-09 03:55:14.000000 gTixi-1.0.0/gTixi/waDrivers.py
--rw-rw-rw-   0        0        0     4118 2022-12-12 09:01:56.000000 gTixi-1.0.0/gTixi/waFile.py
--rw-rw-rw-   0        0        0     5983 2022-12-12 09:01:56.000000 gTixi-1.0.0/gTixi/waText.py
--rw-rw-rw-   0        0        0    22796 2023-01-11 00:43:12.000000 gTixi-1.0.0/gTixi/wadapter.py
-drwxrwxrwx   0        0        0        0 2023-03-10 07:14:42.732086 gTixi-1.0.0/gTixi.egg-info/
--rw-rw-rw-   0        0        0    29745 2023-03-10 07:14:42.000000 gTixi-1.0.0/gTixi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-03-10 07:14:42.000000 gTixi-1.0.0/gTixi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 07:14:42.000000 gTixi-1.0.0/gTixi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-03-10 07:14:42.000000 gTixi-1.0.0/gTixi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-10 07:14:42.747099 gTixi-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-03-10 07:05:12.000000 gTixi-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:37:38.064627 gTixi-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2022-12-02 07:39:30.000000 gTixi-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0    30401 2023-04-19 01:37:38.060630 gTixi-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    29967 2023-04-19 01:36:27.000000 gTixi-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 01:37:38.006652 gTixi-1.1.0/gTixi/
+-rw-rw-rw-   0        0        0     5570 2023-04-10 02:42:27.000000 gTixi-1.1.0/gTixi/SSD1306.py
+-rw-rw-rw-   0        0        0     1116 2023-01-04 05:19:56.000000 gTixi-1.1.0/gTixi/__init__.py
+-rw-rw-rw-   0        0        0    11875 2022-12-12 09:01:56.000000 gTixi-1.1.0/gTixi/alib.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:37:38.056628 gTixi-1.1.0/gTixi/gpio4/
+-rw-rw-rw-   0        0        0    22841 2022-12-12 09:01:56.000000 gTixi-1.1.0/gTixi/gpio4/__init__.py
+-rw-rw-rw-   0        0        0     4478 2022-12-12 09:01:56.000000 gTixi-1.1.0/gTixi/gpio4/arduino.py
+-rw-rw-rw-   0        0        0     2107 2022-12-12 09:01:56.000000 gTixi-1.1.0/gTixi/gpio4/constants.py
+-rw-rw-rw-   0        0        0     8211 2023-01-09 07:29:18.000000 gTixi-1.1.0/gTixi/gpioPins.py
+-rw-rw-rw-   0        0        0     7559 2023-03-01 08:39:59.000000 gTixi-1.1.0/gTixi/starMod.py
+-rw-rw-rw-   0        0        0     9243 2023-04-19 01:27:41.000000 gTixi-1.1.0/gTixi/starServer.py
+-rw-rw-rw-   0        0        0     6388 2023-01-05 08:57:38.000000 gTixi-1.1.0/gTixi/wLTR390.py
+-rw-rw-rw-   0        0        0    15044 2023-01-09 03:55:14.000000 gTixi-1.1.0/gTixi/waDrivers.py
+-rw-rw-rw-   0        0        0     4118 2023-03-01 01:49:26.000000 gTixi-1.1.0/gTixi/waFile.py
+-rw-rw-rw-   0        0        0     5983 2022-12-12 09:01:56.000000 gTixi-1.1.0/gTixi/waText.py
+-rw-rw-rw-   0        0        0    22878 2023-04-11 00:41:59.000000 gTixi-1.1.0/gTixi/wadapter.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:37:38.037629 gTixi-1.1.0/gTixi.egg-info/
+-rw-rw-rw-   0        0        0    30401 2023-04-19 01:37:36.000000 gTixi-1.1.0/gTixi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-04-19 01:37:36.000000 gTixi-1.1.0/gTixi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 01:37:36.000000 gTixi-1.1.0/gTixi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 01:37:36.000000 gTixi-1.1.0/gTixi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 01:37:38.064627 gTixi-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      666 2023-04-19 01:37:28.000000 gTixi-1.1.0/setup.py
```

### Comparing `gTixi-1.0.0/LICENSE` & `gTixi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gTixi-1.0.0/PKG-INFO` & `gTixi-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gTixi
-Version: 1.0.0
+Version: 1.1.0
 Summary: 高效碳基演示体系核心模块
 Home-page: https://gitee.com/lxwk1spectre/walartminstar
 Author: Spectre Lee
 Author-email: lxwk1spectre@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -488,14 +488,16 @@
 #### starMessager.wsStat
 #### starMessager.wsMsg
 - str
 - 与异步模块交互的几个状态变量，当stat不再是waiting时，相关的异步模块就会执行对应的指令。
 #### starMessager.shipei
 - wad.shipei
 - 值为wad.wa，适配器根据设备返回的类，具体用法见[适配器wa](#wa)。
+#### starMessager.starServer()
+- 现在修改为import gTixi之后，不会自动启动按键监控的进程，需要手动打开以节省资源
 #### starMessager.workModule
 - baseMod
 - 当前正在工作的模块，gTixi控制系统通过修改workModule的值来实现不同模块之间的切换。
 ### httpServer
 ### wsServer
 - threading.Thread
 - 分别为网站服务器（bottle架构）和websockets通讯服务器的线程实例。根据需要，要执行如下代码即可。
@@ -608,14 +610,22 @@
 ### gpiopin(p0,p1)
 gpio调试工具，可以用于掌控版和未来板
 - p0:bool,p1:bool
     - p0针脚和p1针脚的输出，True为高电平，False为低电平
 - 返回：sf:str
     - 用于显示在显示屏上的字符串
 # 版本迭代
+## 1.1.0
+- 230319
+    - 将smp的字体文件，webUI的网页文件压缩，一起内置如gTixi中，整个包大小控制在了1M以内。
+    - 禁止了httpserver和websocketsServer的自启动，现在在import gTixi时不会启动任何服务，仅在需要的时候开启。
+    - 去掉了大量print的提示，使得gTixi使用起来更加纯净。
+## 1.0.1
+- 230328
+    - 禁止了zkb，wlb的按键响应服务的自动加载，需要运行starMessager.startServer()才会自动运行。
 ## 1.0.0
 - 230307
     - 经过了与maop的开发联动，进一步验证了gTixi的稳定性
     - 完整界面的git里，加入了介绍部署方案的SOP文档。
     - 本次版本没有代码上的修改
 ## 0.1.2
 - 230111
```

### Comparing `gTixi-1.0.0/README.md` & `gTixi-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -475,14 +475,16 @@
 #### starMessager.wsStat
 #### starMessager.wsMsg
 - str
 - 与异步模块交互的几个状态变量，当stat不再是waiting时，相关的异步模块就会执行对应的指令。
 #### starMessager.shipei
 - wad.shipei
 - 值为wad.wa，适配器根据设备返回的类，具体用法见[适配器wa](#wa)。
+#### starMessager.starServer()
+- 现在修改为import gTixi之后，不会自动启动按键监控的进程，需要手动打开以节省资源
 #### starMessager.workModule
 - baseMod
 - 当前正在工作的模块，gTixi控制系统通过修改workModule的值来实现不同模块之间的切换。
 ### httpServer
 ### wsServer
 - threading.Thread
 - 分别为网站服务器（bottle架构）和websockets通讯服务器的线程实例。根据需要，要执行如下代码即可。
@@ -595,14 +597,22 @@
 ### gpiopin(p0,p1)
 gpio调试工具，可以用于掌控版和未来板
 - p0:bool,p1:bool
     - p0针脚和p1针脚的输出，True为高电平，False为低电平
 - 返回：sf:str
     - 用于显示在显示屏上的字符串
 # 版本迭代
+## 1.1.0
+- 230319
+    - 将smp的字体文件，webUI的网页文件压缩，一起内置如gTixi中，整个包大小控制在了1M以内。
+    - 禁止了httpserver和websocketsServer的自启动，现在在import gTixi时不会启动任何服务，仅在需要的时候开启。
+    - 去掉了大量print的提示，使得gTixi使用起来更加纯净。
+## 1.0.1
+- 230328
+    - 禁止了zkb，wlb的按键响应服务的自动加载，需要运行starMessager.startServer()才会自动运行。
 ## 1.0.0
 - 230307
     - 经过了与maop的开发联动，进一步验证了gTixi的稳定性
     - 完整界面的git里，加入了介绍部署方案的SOP文档。
     - 本次版本没有代码上的修改
 ## 0.1.2
 - 230111
```

### Comparing `gTixi-1.0.0/gTixi/__init__.py` & `gTixi-1.1.0/gTixi/__init__.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.0.0/gTixi/alib.py` & `gTixi-1.1.0/gTixi/alib.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.0.0/gTixi/gpio4/__init__.py` & `gTixi-1.1.0/gTixi/gpio4/__init__.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.0.0/gTixi/gpio4/arduino.py` & `gTixi-1.1.0/gTixi/gpio4/arduino.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.0.0/gTixi/gpio4/constants.py` & `gTixi-1.1.0/gTixi/gpio4/constants.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.0.0/gTixi/gpioPins.py` & `gTixi-1.1.0/gTixi/gpioPins.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.0.0/gTixi/starMod.py` & `gTixi-1.1.0/gTixi/starMod.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.0.0/gTixi/starServer.py` & `gTixi-1.1.0/gTixi/starServer.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,29 @@
         except:
             from wadapter import wa
         self.workModule = None
         self.wsStat = "waiting"
         self.wsMsg = ""
         self.closedWs = []
         self.shipei = wa
+        self.allServers = []
     def output(self,str):
         if sm.shipei.name == 'win':
             print("{}\n{}\n{}".format("-"*20,str,"-"*20))
         self.wsStat = "screen"
         self.shipei.DrawStdLines(str)
         self.wsMsg = str
+    def startServers(self):
+        for func in self.allServers:
+            func()
+        
 sm = starMessager()
 
+
+
 #基于线程的输入输出控制
 if sm.shipei.name == 'zkb':
     from mpython import *
     def inputP(_):
         sm.workModule.InputKey("P")
     def inputY(_):
         sm.workModule.InputKey("Y")
@@ -41,43 +48,47 @@
         sm.workModule.InputKey("O")
     def inputN(_):
         sm.workModule.InputKey("N")
     def inputA(_):
         sm.workModule.InputKey("A")
     def inputB(_):
         sm.workModule.InputKey("B")
-    touchpad_p.event_pressed = inputP
-    touchpad_y.event_pressed = inputY
-    touchpad_t.event_pressed = inputT
-    touchpad_h.event_pressed = inputH
-    touchpad_o.event_pressed = inputO
-    touchpad_n.event_pressed = inputN
-    button_a.event_pressed = inputA
-    button_b.event_pressed = inputB
+    def zkbControl():
+        touchpad_p.event_pressed = inputP
+        touchpad_y.event_pressed = inputY
+        touchpad_t.event_pressed = inputT
+        touchpad_h.event_pressed = inputH
+        touchpad_o.event_pressed = inputO
+        touchpad_n.event_pressed = inputN
+        button_a.event_pressed = inputA
+        button_b.event_pressed = inputB
+    sm.allServers.append(zkbControl)
 
 if sm.shipei.name == 'wlb':
     def wlbKey(_):
         from future import sensor
         while True:
             sm.shipei.Sleep(0.2)
             if sensor.btnValue("a"):
                 sm.workModule.InputKey("A")
             elif sensor.btnValue("b"):
                 sm.workModule.InputKey("B")
-
-    import _thread as th
-    th.start_new_thread(wlbKey,(None,))
+    def wlbControl():
+        import _thread as th
+        th.start_new_thread(wlbKey,(None,))
+    sm.allServers.append(wlbControl)
 
 ########## ws服务器实体  ################
 class webConfig():
     def __init__(self):
         self.wsPort = '8525'
         self.httpPort = '8081'
-        self.webPath = './stardevice'
-        self.bdzPath = '/sdcard/qpython/projects3/WalArtMinS/stardevice/'
+        import os
+        self.webPath = os.path.join(os.path.dirname(__file__),'stardevice')
+        self.bdzPath = '/sdcard/qpython/projects3/WalArtMinS/gTixi/stardevice'
 webConf = webConfig()
 
 if not sm.shipei.name in ['zkb','wlb']:
     import asyncio
     import websockets
     import json
 
@@ -148,26 +159,31 @@
         await websocket.send(d2j({"type":"screen","msg":SvgScreen(ScreenSize).DrawStdLines("欢迎来到星尘演示机\n")}))
         await asyncio.sleep(1)
         sm.workModule.show()
         await asyncio.gather(webIn(websocket),webOut(websocket),sendKey(websocket))
         alllink.remove(websocket)
         sm.closedWs.remove(id(websocket))
         
-    loop = asyncio.new_event_loop()
-    print('Star Socket Server Start!')
-    print('---------------------------')
-    asyncio.set_event_loop(loop)
-    try:
-        loop.run_until_complete(websockets.serve(echo, '0.0.0.0', webConf.wsPort))
-    except:
-        print("Port {} is binded to wsServer!".format(webConf.wsPort))
+
+    loop = None
     def wsStart():
+        try:
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
+            loop.run_until_complete(websockets.serve(echo, '0.0.0.0', webConf.wsPort))
+            print('Star Socket Server Start!')
+            print('---------------------------')
+        except Exception as e:
+            print("Port {} has been binded to wsServer!".format(webConf.wsPort))
+            print(e)
+
         loop.run_forever()
     def wsStop():
-        loop.stop()
+        if loop:
+            loop.stop()
 
     import threading
     wsServer = threading.Thread(target=wsStart)
     class wsCtrl():
         def __init__(self):
             self.loop = loop
             self.t1 = threading.Thread(target=wsStart)
```

### Comparing `gTixi-1.0.0/gTixi/wLTR390.py` & `gTixi-1.1.0/gTixi/wLTR390.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.0.0/gTixi/waDrivers.py` & `gTixi-1.1.0/gTixi/waDrivers.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.0.0/gTixi/waFile.py` & `gTixi-1.1.0/gTixi/waFile.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.0.0/gTixi/waText.py` & `gTixi-1.1.0/gTixi/waText.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.0.0/gTixi/wadapter.py` & `gTixi-1.1.0/gTixi/wadapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,15 +372,15 @@
         self.tag.extend(['web','smbus','gpiorpi','pinmap'])
         self.aenv=aenv
         self.cSoftKey=''
         import math
         import time
 
         import spidev as SPI
-        import SSD1306
+        from . import SSD1306
 
         import smbus
         self.oi2c=smbus.SMBus(1)
         i2c=self.oi2c
         class AI2C():
             def __init__(self,write_byte_data,read_byte_data,read_i2c_block_data):
                 self.write_byte_data = write_byte_data
@@ -390,15 +390,15 @@
         self.hasSsd=None
         self.oSvg=None
         self.InitDisplay()
 
     def InitDisplay(self):
         try:
             import spidev as SPI
-            import SSD1306
+            from . import SSD1306
             from PIL import Image
             from PIL import ImageFont
             from PIL import ImageDraw
 
             # Raspberry Pi pin configuration:
             RST = 19
             DC = 16
@@ -426,20 +426,21 @@
             self.image = Image.new('1', (width, height))
 
             # Get drawing object to draw on image.
             self.draw = ImageDraw.Draw(self.image)
             self.disp=disp
             # Draw a black filled box to clear the image.
             #draw.rectangle((0,0,width,height), outline=0, fill=0)
-
-            fontpath='simsun.ttf'
+            import os
+            fontpath= os.path.join(os.path.dirname(__file__),"Dianzhen.ttf")
+            
             self.font=ImageFont.truetype(fontpath,15)
             self.hasSsd=True
         except Exception as e:
-            print('SSD初始化出错:',e)
+            print('SSD1306初始化出错:',e)
             self.hasSsd=False
         self.oSvg=SvgScreen()
 
     def CheckKey(self):
         import RPi.GPIO as GPIO
         import smbus
         import time
@@ -637,43 +638,44 @@
         ip = s.getsockname()[0]
         s.close()
     except:
         ip='no network'
     aWaEnv['sIp']=ip
     return ip
 def Wa(aenv=aWaEnv):
-    if aenv == 'debug':
+    #if aenv == 'debug':
+    if "SMP" in aenv['sVersion']:
         return SpSmp(aenv)
     elif 'mpython' in aenv['sMachine']:
         return SpZkb(aenv)
     elif 'Future' in aenv['sMachine']:
         return SpWlb(aenv)
     elif 'v7l' in aenv['sMachine']:
         if 'localhost' in aenv['sNodename']:
             return SpBdz(aenv)
         else:
             return SpSmp(aenv)
     else:
-        #print(aenv.sMachine)
+        
         return SpWin(aenv)
 SIp()
 Hello()
 wa=Wa()
-print(wa.name)
+
 ##################################################
 DEBUG=False
 aI2c='''[#comment|此体系中器件有统一i2c地址]
 [0x20|PCF8574IO扩展（Pioneer600）]
 [0x26|GTmcp的mcp23017]
 [0x39|APDS9960光线颜色传感器]
 [0x42|UPS HAT]
 [0x48|PCF8591ADDA（Pioneer600）]
 [0x53|LTR390紫外光光感]
 [0x5a|MLX90614红外传感]
 [0x68|DS3231时钟模块（Pioneer600）]
 [0x76|BMP280温度压力传感（Pioneer600）]
 [0x77|BME280温湿度压力传感器]'''
 strWaEnv = str(aWaEnv).replace("{","[").replace("}","]").replace(": ","|").replace("'","").replace(", ","][")
-print(strWaEnv)
+
 
 if __name__ == "__main__":
     pass
```

### Comparing `gTixi-1.0.0/gTixi.egg-info/PKG-INFO` & `gTixi-1.1.0/gTixi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gTixi
-Version: 1.0.0
+Version: 1.1.0
 Summary: 高效碳基演示体系核心模块
 Home-page: https://gitee.com/lxwk1spectre/walartminstar
 Author: Spectre Lee
 Author-email: lxwk1spectre@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -488,14 +488,16 @@
 #### starMessager.wsStat
 #### starMessager.wsMsg
 - str
 - 与异步模块交互的几个状态变量，当stat不再是waiting时，相关的异步模块就会执行对应的指令。
 #### starMessager.shipei
 - wad.shipei
 - 值为wad.wa，适配器根据设备返回的类，具体用法见[适配器wa](#wa)。
+#### starMessager.starServer()
+- 现在修改为import gTixi之后，不会自动启动按键监控的进程，需要手动打开以节省资源
 #### starMessager.workModule
 - baseMod
 - 当前正在工作的模块，gTixi控制系统通过修改workModule的值来实现不同模块之间的切换。
 ### httpServer
 ### wsServer
 - threading.Thread
 - 分别为网站服务器（bottle架构）和websockets通讯服务器的线程实例。根据需要，要执行如下代码即可。
@@ -608,14 +610,22 @@
 ### gpiopin(p0,p1)
 gpio调试工具，可以用于掌控版和未来板
 - p0:bool,p1:bool
     - p0针脚和p1针脚的输出，True为高电平，False为低电平
 - 返回：sf:str
     - 用于显示在显示屏上的字符串
 # 版本迭代
+## 1.1.0
+- 230319
+    - 将smp的字体文件，webUI的网页文件压缩，一起内置如gTixi中，整个包大小控制在了1M以内。
+    - 禁止了httpserver和websocketsServer的自启动，现在在import gTixi时不会启动任何服务，仅在需要的时候开启。
+    - 去掉了大量print的提示，使得gTixi使用起来更加纯净。
+## 1.0.1
+- 230328
+    - 禁止了zkb，wlb的按键响应服务的自动加载，需要运行starMessager.startServer()才会自动运行。
 ## 1.0.0
 - 230307
     - 经过了与maop的开发联动，进一步验证了gTixi的稳定性
     - 完整界面的git里，加入了介绍部署方案的SOP文档。
     - 本次版本没有代码上的修改
 ## 0.1.2
 - 230111
```

### Comparing `gTixi-1.0.0/setup.py` & `gTixi-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gTixi",
-    version="1.0.0",
+    version="1.1.0",
     author="Spectre Lee",
     author_email="lxwk1spectre@foxmail.com",
     description="高效碳基演示体系核心模块",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/lxwk1spectre/walartminstar",
     packages=setuptools.find_packages(),
```

