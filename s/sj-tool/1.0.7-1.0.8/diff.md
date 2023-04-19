# Comparing `tmp/sj_tool-1.0.7-py3-none-any.whl.zip` & `tmp/sj_tool-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 12950 bytes, number of entries: 29
+Zip file size: 13138 bytes, number of entries: 29
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 09:37 sj_tool/__init__.py
 -rw-rw-rw-  2.0 fat      226 b- defN 23-Apr-10 10:09 sj_tool/decorator.py
 -rw-rw-rw-  2.0 fat      476 b- defN 23-Apr-01 13:00 sj_tool/email.py
 -rw-rw-rw-  2.0 fat      476 b- defN 23-Apr-01 13:00 sj_tool/email_sender.py
 -rw-rw-rw-  2.0 fat      155 b- defN 23-Mar-14 09:42 sj_tool/file.py
 -rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-04 05:43 sj_tool/json.py
 -rw-rw-rw-  2.0 fat      335 b- defN 23-Apr-14 09:33 sj_tool/parallel.py
@@ -18,14 +18,14 @@
 -rw-rw-rw-  2.0 fat      897 b- defN 23-Apr-10 09:07 sj_tool/fjsp/entity/fjsp_pool.py
 -rw-rw-rw-  2.0 fat      897 b- defN 23-Apr-10 09:07 sj_tool/fjsp/entity/global_pool.py
 -rw-rw-rw-  2.0 fat      736 b- defN 23-Apr-15 11:54 sj_tool/fjsp/entity/job.py
 -rw-rw-rw-  2.0 fat      411 b- defN 23-Apr-09 05:22 sj_tool/fjsp/entity/machine.py
 -rw-rw-rw-  2.0 fat      829 b- defN 23-Apr-15 11:54 sj_tool/fjsp/entity/operation.py
 -rw-rw-rw-  2.0 fat      113 b- defN 23-Apr-09 09:02 sj_tool/fjsp/entity/product.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-30 02:45 sj_tool/logger/__init__.py
--rw-rw-rw-  2.0 fat     1866 b- defN 23-Apr-08 12:57 sj_tool/logger/text_logger.py
--rw-rw-rw-  2.0 fat     2718 b- defN 23-Apr-09 03:19 sj_tool/logger/visual_logger.py
--rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-15 11:54 sj_tool-1.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-15 11:54 sj_tool-1.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-15 11:54 sj_tool-1.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2289 b- defN 23-Apr-15 11:54 sj_tool-1.0.7.dist-info/RECORD
-29 files, 24199 bytes uncompressed, 9274 bytes compressed:  61.7%
+-rw-rw-rw-  2.0 fat     2256 b- defN 23-Apr-19 09:16 sj_tool/logger/text_logger.py
+-rw-rw-rw-  2.0 fat     2753 b- defN 23-Apr-19 09:41 sj_tool/logger/visual_logger.py
+-rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-19 09:41 sj_tool-1.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 09:41 sj_tool-1.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-19 09:41 sj_tool-1.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2289 b- defN 23-Apr-19 09:41 sj_tool-1.0.8.dist-info/RECORD
+29 files, 24624 bytes uncompressed, 9462 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -69,20 +69,20 @@
 
 Filename: sj_tool/logger/text_logger.py
 Comment: 
 
 Filename: sj_tool/logger/visual_logger.py
 Comment: 
 
-Filename: sj_tool-1.0.7.dist-info/METADATA
+Filename: sj_tool-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: sj_tool-1.0.7.dist-info/WHEEL
+Filename: sj_tool-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: sj_tool-1.0.7.dist-info/top_level.txt
+Filename: sj_tool-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: sj_tool-1.0.7.dist-info/RECORD
+Filename: sj_tool-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sj_tool/logger/text_logger.py

```diff
@@ -3,14 +3,15 @@
 """
 
 import os
 import sys
 
 import loguru
 from loguru import logger
+from datetime import datetime
 
 
 class LogLevel:
     """
     TRACE：最低级别的日志，通常用于调试和追踪代码的执行过程。
 
     DEBUG：用于详细输出程序执行过程中的变量、状态和异常信息等，通常用于调试和问题定位。
@@ -31,24 +32,32 @@
     INFO = "INFO"
     SUCCESS = "SUCCESS"
     WARNING = "WARNING"
     ERROR = "ERROR"
     CRITICAL = "CRITICAL"
 
 
-def init(level: str, filepath=None, max_filesize=None, replace=False) -> loguru.logger:
+def init(level: str, save_log=True, logdir=None, comment="", filename="text.log", max_filesize=None) -> loguru.logger:
     """
     初始化日志框架
     :param level: 最低的日志level，如LogLevel.INFO
-    :param filepath: 日志文件路径
+    :param save_log: 是否保存log到文件
+    :param logdir: 保存log到文件
+    :param comment: log文件夹名后缀(仅在logdir为None时有效)
+    :param filename: 日志文件名
     :param max_filesize: 最大文件大小
     :param replace: 是否替换已有文件（如果文件存在）
     :return:
     """
     logger.remove()
     logger.add(sys.stdout, level=level)
-    if filepath is not None:
-        if replace:
-            os.remove(filepath)
-        logger.add(filepath, rotation=max_filesize, compression="zip", level=level)
+
+    if not logdir:
+        current_time = datetime.now().strftime("%b%d_%H-%M-%S")
+        if "" != comment:
+            comment = "." + comment
+        logdir = os.path.join("runs", current_time + comment)
+
+    if save_log:
+        logger.add(os.path.join(logdir, filename), rotation=max_filesize, compression="zip", level=level)
 
     return logger
```

## sj_tool/logger/visual_logger.py

```diff
@@ -5,16 +5,16 @@
 
 from typing import List, Union
 from visualdl import LogWriter
 from tensorboardX import SummaryWriter
 
 
 class VisualLogger(object):
-    def __init__(self, logdir, use_visualdl=True, text_logger: loguru.Logger = None):
-        self.writer = LogWriter(logdir) if use_visualdl else SummaryWriter(logdir)
+    def __init__(self, logdir=None, comment="", use_visualdl=True, text_logger: loguru.logger = None):
+        self.writer = LogWriter(logdir, comment) if use_visualdl else SummaryWriter(logdir, comment)
         self.text_logger = text_logger
 
     def add_scalar(self, tag: str, value: Union[str, int, float], step: int):
         self.writer.add_scalar(tag, value, step)
 
     def add_image(self, tag: str, img: np.ndarray, step: int):
         self.writer.add_image(tag=tag, img=img, step=step)
```

## Comparing `sj_tool-1.0.7.dist-info/RECORD` & `sj_tool-1.0.8.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -17,13 +17,13 @@
 sj_tool/fjsp/entity/fjsp_pool.py,sha256=9-pE3_NIZqVWDM0TrGosycMfzaE1iQov8mSZ3-LZEPo,897
 sj_tool/fjsp/entity/global_pool.py,sha256=9-pE3_NIZqVWDM0TrGosycMfzaE1iQov8mSZ3-LZEPo,897
 sj_tool/fjsp/entity/job.py,sha256=r4DGShXcv-K6rnKn5602-X2t6bs3yE1nfcAd3qIMe28,736
 sj_tool/fjsp/entity/machine.py,sha256=zBjVt5VYEuJlqA4yHzzEw9wlbVSAaJHlgj0lweSNaSw,411
 sj_tool/fjsp/entity/operation.py,sha256=nJaMbjFyTJTGkjBg4yokXgwqldMkdbqs7psG-9d6nmo,829
 sj_tool/fjsp/entity/product.py,sha256=IzErQu-Hm0d8rSdWA3Z-HYaYBDmNUbyOMBumYc1dwuU,113
 sj_tool/logger/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sj_tool/logger/text_logger.py,sha256=hNPAxGVOsL46q-9cd-o-S7WV3CL52vlhD7HWKRAeh2Y,1866
-sj_tool/logger/visual_logger.py,sha256=AfKNWJpTb-Odm4gWUyVRXIykiXyvfrdAjukwugCD6os,2718
-sj_tool-1.0.7.dist-info/METADATA,sha256=D_uAxcooGUPy6Ua36yf8LijfaXymEosDbq0Pnp9tFsw,492
-sj_tool-1.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sj_tool-1.0.7.dist-info/top_level.txt,sha256=U2pHVPt1Cmde1D9tGeZIoA5KUuo-Urt6Etd-qD5A_cA,8
-sj_tool-1.0.7.dist-info/RECORD,,
+sj_tool/logger/text_logger.py,sha256=P_V4ABz7_PZ09PoaZzWuVk5bcrvlMuYwfEIQ026rdvA,2256
+sj_tool/logger/visual_logger.py,sha256=-OLn2lG2DUZiuSeTklO7h4sXHBeT6pXkN_tjfBeJBGE,2753
+sj_tool-1.0.8.dist-info/METADATA,sha256=M7ZCcAEY10e3dLOkU9_I13oopuJ6vVSsFG_VPvAqLgY,492
+sj_tool-1.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+sj_tool-1.0.8.dist-info/top_level.txt,sha256=U2pHVPt1Cmde1D9tGeZIoA5KUuo-Urt6Etd-qD5A_cA,8
+sj_tool-1.0.8.dist-info/RECORD,,
```

