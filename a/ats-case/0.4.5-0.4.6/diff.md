# Comparing `tmp/ats_case-0.4.5.tar.gz` & `tmp/ats_case-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.4.5.tar", last modified: Tue Apr 18 06:40:23 2023, max compression
+gzip compressed data, was "ats_case-0.4.6.tar", last modified: Wed Apr 19 08:19:03 2023, max compression
```

## Comparing `ats_case-0.4.5.tar` & `ats_case-0.4.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 06:40:23.976412 ats_case-0.4.5/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.4.5/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-18 06:40:23.973419 ats_case-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 06:40:23.577253 ats_case-0.4.5/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.4.5/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:40:23.793589 ats_case-0.4.5/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.4.5/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    16904 2023-04-18 06:39:42.000000 ats_case-0.4.5/ats_case/case/command.py
--rw-rw-rw-   0        0        0    10337 2023-04-18 06:38:27.000000 ats_case-0.4.5/ats_case/case/context.py
--rw-rw-rw-   0        0        0     5317 2023-04-15 05:22:12.000000 ats_case-0.4.5/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5437 2023-04-12 01:16:48.000000 ats_case-0.4.5/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:40:23.862718 ats_case-0.4.5/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.4.5/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      381 2023-04-10 07:20:19.000000 ats_case-0.4.5/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      646 2023-04-15 05:21:08.000000 ats_case-0.4.5/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:40:23.921559 ats_case-0.4.5/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.5/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.4.5/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2586 2023-04-12 01:16:48.000000 ats_case-0.4.5/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:40:23.963447 ats_case-0.4.5/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.5/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2089 2023-04-12 01:03:34.000000 ats_case-0.4.5/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-18 06:40:23.668719 ats_case-0.4.5/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-18 06:40:23.000000 ats_case-0.4.5/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-18 06:40:23.000000 ats_case-0.4.5/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 06:40:23.000000 ats_case-0.4.5/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-18 06:40:23.000000 ats_case-0.4.5/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 06:40:23.000000 ats_case-0.4.5/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 06:40:23.976412 ats_case-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-18 06:39:42.000000 ats_case-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:19:03.100308 ats_case-0.4.6/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-19 08:19:03.098312 ats_case-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 08:19:02.618795 ats_case-0.4.6/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.4.6/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:19:02.885468 ats_case-0.4.6/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.4.6/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    16757 2023-04-19 08:16:19.000000 ats_case-0.4.6/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    10234 2023-04-19 08:13:19.000000 ats_case-0.4.6/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     5317 2023-04-15 05:22:12.000000 ats_case-0.4.6/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5441 2023-04-19 06:25:18.000000 ats_case-0.4.6/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:19:02.958275 ats_case-0.4.6/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.4.6/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      381 2023-04-10 07:20:19.000000 ats_case-0.4.6/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      646 2023-04-15 05:21:08.000000 ats_case-0.4.6/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:19:03.039705 ats_case-0.4.6/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.6/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.4.6/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     3083 2023-04-19 08:18:35.000000 ats_case-0.4.6/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:19:03.089337 ats_case-0.4.6/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.6/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2089 2023-04-12 01:03:34.000000 ats_case-0.4.6/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-19 08:19:02.749829 ats_case-0.4.6/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-19 08:19:01.000000 ats_case-0.4.6/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-19 08:19:02.000000 ats_case-0.4.6/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 08:19:01.000000 ats_case-0.4.6/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-19 08:19:01.000000 ats_case-0.4.6/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 08:19:01.000000 ats_case-0.4.6/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 08:19:03.100308 ats_case-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-19 08:18:43.000000 ats_case-0.4.6/setup.py
```

### Comparing `ats_case-0.4.5/PKG-INFO` & `ats_case-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.4.5
+Version: 0.4.6
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.4.5/README.md` & `ats_case-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.5/ats_case/case/command.py` & `ats_case-0.4.6/ats_case/case/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,24 +77,14 @@
     if disabled == 1:
         if clazz == OperationClazz.BENCH:
             return True
 
     return False
 
 
-def cache(context: Context, data):
-    """
-    缓存
-    :param context:
-    :param data:
-    :return:
-    """
-    pass
-
-
 """
     内部方法
 """
 
 
 def _replace(context: Context, data: dict):
     sd = str(data)
@@ -210,42 +200,42 @@
                                                                                       self._element))
         if type(self._parameter) is dict:
             self._parameter = _replace(context, self._parameter)
 
         parse = pro.encode(func.to_dict(protocol=self._protocol.name, comm_addr=self._comm_addr,
                                         operation=self._operation, element=self._element, parameter=self._parameter,
                                         addition=self._addition, security=self._security,
-                                        session_key=context.session.basename))
+                                        session_key=context.session.test_sn))
         logger.info('~ @PRO-ENCODE<- protocol:{} frame:{}'.format(self._protocol, parse.get('frame')))
 
         self._frame = parse.get('frame')
         return self._frame
 
     def decode(self, context: Context, index=0):
         # 异常判断 - 客户端返回结果
         if self._frame is None or len(self._frame) <= 0:
             raise ClientReturnError(self._frame)
 
         logger.info('~ @PRO-DECODE-> protocol:{} frame:{}'.format(self._protocol, self._frame))
         data = pro.decode(
-            func.to_dict(protocol=self._protocol.name, frame=self._frame, session_key=context.session.basename))
+            func.to_dict(protocol=self._protocol.name, frame=self._frame, session_key=context.test_sn))
         logger.info('~ @PRO-DECODE<- protocol:{} parse:{}'.format(self._protocol, data))
 
         # 异常判断 - 协议服务返回结果
         if data.get('error') == 1:
             raise MeterOperationError(data.get('result'))
 
         # 分帧处理开始
         next_frame = data.get('next_frame', None)
         if next_frame is not None:
             result = send(context,
                           todo={
                               'meter:comm': {'channel': {'type': 'RS485', 'baudrate': 9600}, 'frame': next_frame}})
             self._frame = result.get('result')
-            self.decode(context, index+1)
+            self.decode(context, index + 1)
         else:
             context.runtime.final_result = data.get('result')
         # 分帧处理结束
 
         if index == 0:
             self._parse = context.runtime.final_result
             self._flush(context)
@@ -311,15 +301,15 @@
         return self
 
     def handle(self, context: Context):
         try:
             if self._parameter is None:
                 self._parameter = {}
             self._parameter = context.runtime.steps[context.runtime.step - 1]['result']
-            self._parameter['basename'] = context.session.basename
+            self._parameter['session_key'] = context.test_sn
         except:
             pass
 
         logger.info(
             '~ @EM-> protocol:{} operation:{} parameter:{}'.format(self._protocol, self._operation, self._parameter))
         self._result = em.handle(self._protocol.name, self._operation, self._parameter)
         logger.info('~ @EM<- protocol:{} operation:{} result:{}'.format(self._protocol, self._operation, self._result))
```

### Comparing `ats_case-0.4.5/ats_case/case/context.py` & `ats_case-0.4.6/ats_case/case/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
         self._tester = self.Tester(tl.get('tester'))
         self._case = self.Case(tl.get('usercase'))
         self._meter = self.Meter(tl.get('meter'))
         self._bench = self.Bench(tl.get('bench'))
         self._runtime = self.Runtime()
         self._session = self.Session(self)
+        # Debug模式 - 测试开发人员本机调试数据比对服务使用
         self._acd_url = tl.get('acd_url')
 
     #     self._bench = self.Bench(tl.get('bench'))
     #     self._case = self.Case(tl.get('cases').get(self.case_id))
     #     self._meter = tl.get('meter')
     #     self._runtime = self.Runtime()
     #
@@ -354,19 +355,15 @@
 
         @final_result.setter
         def final_result(self, value):
             self._final_result = value
 
     class Session(object):
         def __init__(self, parent):
-            self._basename = '{}:{}:{}'.format(parent.test_sn
-                                               , parent.case.id, parent.meter.pos)
+            self._parent = parent
 
         def get(self, name: str, key: str):
-            return mm.Dict.get('{}:{}'.format(self._basename, name), key)
+            return mm.Dict.get('{}:{}'.format(self._parent.test_sn, name), key)
 
         def set(self, name: str, key: str, data):
-            return mm.Dict.put('{}:{}'.format(self._basename, name), key, data)
+            return mm.Dict.put('{}:{}'.format(self._parent.test_sn, name), key, data)
 
-        @property
-        def basename(self):
-            return self._basename
```

### Comparing `ats_case-0.4.5/ats_case/case/executor.py` & `ats_case-0.4.6/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.5/ats_case/case/translator.py` & `ats_case-0.4.6/ats_case/case/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,7 +187,9 @@
 
         if param is not None:
             code += ".parameter({})".format(param)
 
         code += ".exec(context)"
 
         return code
+
+
```

### Comparing `ats_case-0.4.5/ats_case/common/error.py` & `ats_case-0.4.6/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.5/ats_case/manage/core.py` & `ats_case-0.4.6/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.5/ats_case/template/testcase_v1.tmp` & `ats_case-0.4.6/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.5/ats_case.egg-info/PKG-INFO` & `ats_case-0.4.6/ats_case.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.4.5
+Version: 0.4.6
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.4.5/ats_case.egg-info/SOURCES.txt` & `ats_case-0.4.6/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.5/setup.py` & `ats_case-0.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.4.5",
+    version="0.4.6",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

