# Comparing `tmp/nb_log-8.3.tar.gz` & `tmp/nb_log-8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_log-8.3.tar", last modified: Mon Apr 17 03:21:52 2023, max compression
+gzip compressed data, was "dist\nb_log-8.4.tar", last modified: Wed Apr 19 03:37:27 2023, max compression
```

## Comparing `nb_log-8.3.tar` & `nb_log-8.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 03:21:52.000000 nb_log-8.3/
--rw-rw-rw-   0        0        0    27863 2023-04-17 03:21:52.000000 nb_log-8.3/PKG-INFO
--rw-rw-rw-   0        0        0    26926 2022-12-05 09:46:23.000000 nb_log-8.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 03:21:52.000000 nb_log-8.3/nb_log/
--rw-rw-rw-   0        0        0     2329 2022-09-17 07:28:19.000000 nb_log-8.3/nb_log/__init__.py
--rw-rw-rw-   0        0        0    50623 2023-04-17 02:59:39.000000 nb_log-8.3/nb_log/handlers.py
--rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-8.3/nb_log/handlers0000.py
--rw-rw-rw-   0        0        0      246 2023-04-17 02:59:39.000000 nb_log-8.3/nb_log/helper.py
--rw-rw-rw-   0        0        0    30405 2023-04-17 02:59:07.000000 nb_log-8.3/nb_log/log_manager.py
--rw-rw-rw-   0        0        0     7350 2023-04-17 02:59:07.000000 nb_log-8.3/nb_log/monkey_print.py
--rw-rw-rw-   0        0        0     9334 2023-04-17 03:10:36.000000 nb_log-8.3/nb_log/nb_log_config_default.py
--rw-rw-rw-   0        0        0     7710 2023-04-13 09:47:00.000000 nb_log-8.3/nb_log/set_nb_log_config.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:21:52.000000 nb_log-8.3/nb_log.egg-info/
--rw-rw-rw-   0        0        0    27863 2023-04-17 03:21:52.000000 nb_log-8.3/nb_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-04-17 03:21:52.000000 nb_log-8.3/nb_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 03:21:52.000000 nb_log-8.3/nb_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-04-17 03:21:52.000000 nb_log-8.3/nb_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 03:21:52.000000 nb_log-8.3/nb_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 03:21:52.000000 nb_log-8.3/setup.cfg
--rw-rw-rw-   0        0        0     2325 2023-04-17 03:21:43.000000 nb_log-8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 03:37:27.000000 nb_log-8.4/
+-rw-rw-rw-   0        0        0    27863 2023-04-19 03:37:27.000000 nb_log-8.4/PKG-INFO
+-rw-rw-rw-   0        0        0    26926 2022-12-05 09:46:23.000000 nb_log-8.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 03:37:27.000000 nb_log-8.4/nb_log/
+-rw-rw-rw-   0        0        0     2329 2022-09-17 07:28:19.000000 nb_log-8.4/nb_log/__init__.py
+-rw-rw-rw-   0        0        0    50524 2023-04-19 03:34:32.000000 nb_log-8.4/nb_log/handlers.py
+-rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-8.4/nb_log/handlers0000.py
+-rw-rw-rw-   0        0        0      247 2023-04-18 01:17:35.000000 nb_log-8.4/nb_log/helper.py
+-rw-rw-rw-   0        0        0    30621 2023-04-18 02:30:56.000000 nb_log-8.4/nb_log/log_manager.py
+-rw-rw-rw-   0        0        0     7782 2023-04-18 01:50:08.000000 nb_log-8.4/nb_log/monkey_print.py
+-rw-rw-rw-   0        0        0     9455 2023-04-17 07:36:14.000000 nb_log-8.4/nb_log/nb_log_config_default.py
+-rw-rw-rw-   0        0        0     7710 2023-04-13 09:47:00.000000 nb_log-8.4/nb_log/set_nb_log_config.py
+drwxrwxrwx   0        0        0        0 2023-04-19 03:37:27.000000 nb_log-8.4/nb_log.egg-info/
+-rw-rw-rw-   0        0        0    27863 2023-04-19 03:37:27.000000 nb_log-8.4/nb_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-04-19 03:37:27.000000 nb_log-8.4/nb_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 03:37:27.000000 nb_log-8.4/nb_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-04-19 03:37:27.000000 nb_log-8.4/nb_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 03:37:27.000000 nb_log-8.4/nb_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 03:37:27.000000 nb_log-8.4/setup.cfg
+-rw-rw-rw-   0        0        0     2325 2023-04-19 03:37:18.000000 nb_log-8.4/setup.py
```

### Comparing `nb_log-8.3/PKG-INFO` & `nb_log-8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_log
-Version: 8.3
+Version: 8.4
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-8.3/README.md` & `nb_log-8.4/README.md`

 * *Files identical despite different names*

### Comparing `nb_log-8.3/nb_log/__init__.py` & `nb_log-8.4/nb_log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.3/nb_log/handlers.py` & `nb_log-8.4/nb_log/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 # noinspection PyUnresolvedReferences
 from logging.handlers import WatchedFileHandler
 # noinspection PyPackageRequirements
 from nb_filelock import FileLock
 from pythonjsonlogger.jsonlogger import JsonFormatter
 from nb_log import nb_log_config_default
 from nb_log import nb_print
-from nb_log.helper import need_filter_print
 
 very_nb_print = nb_print
 os_name = os.name
 
 
 class MongoHandler(logging.Handler):
     """
@@ -580,16 +579,14 @@
         The record is then written to the stream with a trailing newline.  If
         exception information is present, it is formatted using
         traceback.print_exception and appended to the stream.  If the stream
         has an 'encoding' attribute, it is used to determine how to do the
         output to the stream.
         """
         # noinspection PyBroadException
-        if need_filter_print(record.msg):
-            return
         try:
             # very_nb_print(record)
             # record.message = record.getMessage()
             # effective_information_msg = record.getMessage()  # 不能用msg字段，例如有的包的日志格式化还有其他字段
             # record_copy = copy.copy(record)  # copy是因为，不要因为要屏幕彩色日志而影响例如文件日志 叮叮日志等其他handler的格式。
             # record_copy.for_segmentation_color = '彩色分段标志属性而已'
             # del record_copy.msg
@@ -919,15 +916,15 @@
     def __init__(self, file_name: str, file_path: str, back_count=None):
         super().__init__()
         self.file_name = file_name
         self.file_path = file_path
         self.backupCount = back_count or nb_log_config_default.LOG_FILE_BACKUP_COUNT
         self.extMatch = re.compile(r"^\d{4}-\d{2}-\d{2}(\.\w+)?$", re.ASCII)
         self.extMatch2 = re.compile(r"^\d{2}-\d{2}-\d{2}(\.\w+)?$", re.ASCII)
-        self._last_delete_time = time.time()
+        self._last_delete_time = 0
 
         self.buffer_msgs_queue = queue.Queue()
         atexit.register(self._write_to_file)  # 如果程序属于立马就能结束的，需要在程序结束前执行这个钩子，防止不到最后一秒的日志没记录到。
         self.file_handler_list.append(self)
         if os.getpid() not in self.has_start_emit_all_file_handler_process_id_set:
             self._start_emit_all_file_handler()
             self.__class__.has_start_emit_all_file_handler_process_id_set.add(os.getpid())
@@ -962,14 +959,15 @@
                 time_str = time.strftime('%Y-%m-%d')
                 # time_str = time.strftime('%H-%M-%S')  # 方便测试用的，方便观察。
                 new_file_name = self.file_name + '.' + time_str
                 path_obj = Path(self.file_path) / Path(new_file_name)
                 path_obj.touch(exist_ok=True)
                 with path_obj.open(mode='a', encoding='utf-8') as f:
                     f.write(buffer_msgs)
+                    f.flush()
                 if time.time() - self._last_delete_time > 60:
                     self._find_and_delete_files()
                     self._last_delete_time = time.time()
 
     def _find_and_delete_files(self):
         """
         这一段命名不规范是复制原来的官方旧代码。
@@ -1039,15 +1037,15 @@
         :param record:
         :return:
         """
         # noinspection PyBroadException
         try:
             msg = self.format(record)
             self.fp.write(msg + '\n')
-            # self.fp.flush() # 需要flush才能及时写入。重写close可以写入程序结束前的缓冲。
+            self.fp.flush() # 需要flush才能及时写入。重写close可以写入程序结束前的缓冲。
         except Exception as e:
             print(e)
             self.handleError(record)
         if time.time() - self._last_delete_time > 60:
             self._get_fp()
             self._find_and_delete_files()
             self._last_delete_time = time.time()
@@ -1096,15 +1094,15 @@
     def __init__(self, file_name: str, file_path: str, back_count=None):
         super().__init__()
         self.file_name = file_name
         self.file_path = file_path
         self.backupCount = back_count or nb_log_config_default.LOG_FILE_BACKUP_COUNT
         self.extMatch = re.compile(r"^\d{4}-\d{2}-\d{2}(\.\w+)?$", re.ASCII)
         self.extMatch2 = re.compile(r"^\d{2}-\d{2}-\d{2}(\.\w+)?$", re.ASCII)
-        self._last_delete_time = time.time()
+        self._last_delete_time = 0
 
         time_str = time.strftime('%H-%M-%S')  # 方便测试用的，方便观察。
         new_file_name = self.file_name + '.' + time_str
         path_obj = Path(self.file_path) / Path(new_file_name)
         path_obj.touch(exist_ok=True)
         self.fp = open(path_obj, 'a', encoding='utf-8')
         self.time_str = time_str
@@ -1130,19 +1128,19 @@
         emit已经在logger的handle方法中加了锁，所以这里的重置上次写入时间和清除buffer_msgs不需要加锁了。
         :param record:
         :return:
         """
         # noinspection PyBroadException
         try:
             msg = self.format(record)
-            self.fp.write(msg + '\n')
             if time.time() - self._last_delete_time > 0.5:
                 self._get_fp()
                 self._find_and_delete_files()
                 self._last_delete_time = time.time()
+            self.fp.write(msg + '\n')
         except Exception as e:
             print(e)
             self.handleError(record)
 
     def _find_and_delete_files(self):
         """
         这一段命名不规范是复制原来的官方旧代码。
```

### Comparing `nb_log-8.3/nb_log/handlers0000.py` & `nb_log-8.4/nb_log/handlers0000.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.3/nb_log/log_manager.py` & `nb_log-8.4/nb_log/log_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,22 @@
     credentials: tuple = nb_log_config_default.EMAIL_CREDENTIALS
     secure = None
     timeout = 5.0
     is_use_ssl = True
     mail_time_interval = 60
 
 
+LOG_LEVEL_LIST = [logging.DEBUG, logging.INFO, logging.WARNING, logging.ERROR, logging.CRITICAL]  # 就是 10 20 30 40 50
+
+
+def check_log_level(log_level: int):
+    if log_level not in LOG_LEVEL_LIST:
+        raise ValueError(f'你设置的日志级别不正确,你设置的级别是 {log_level} ，日志级别必须是 {LOG_LEVEL_LIST} 其中之一')
+
+
 # noinspection PyMissingOrEmptyDocstring,PyPep8
 class LogManager(object):
     """
     一个日志管理类，用于创建logger和添加handler，支持将日志打印到控制台打印和写入日志文件和mongodb和邮件。
     """
     logger_name_list = []
     logger_list = []
@@ -217,16 +225,15 @@
     def preset_log_level(self, log_level_int=20):
         """
         提前设置锁定日志级别，当之后再设置该命名空间日志的级别的时候，按照提前预设的级别，无视之后设定的级别。
         主要是针对动态初始化的日志，在生成日志之后再去设置日志级别不方便。
         :param log_level_int:logging.DEBUG LOGGING.INFO 等
         :return:
         """
-        if log_level_int not in [logging.DEBUG, logging.INFO, logging.WARNING, logging.ERROR, logging.CRITICAL]:
-            raise ValueError('你设置的日志级别不正确')
+        check_log_level(log_level_int)
         self.preset_name__level_map[self._logger_name] = log_level_int
 
     # 加*是为了强制在调用此方法时候使用关键字传参，如果以位置传参强制报错，因为此方法后面的参数中间可能以后随时会增加更多参数，造成之前的使用位置传参的代码参数意义不匹配。
     # noinspection PyAttributeOutsideInit
     def get_logger_and_add_handlers(self, log_level_int: int = None, *, is_add_stream_handler=True,
                                     do_not_use_color_handler=None, log_path=None,
                                     log_filename=None, log_file_size: int = None,
@@ -277,15 +284,16 @@
             log_file_size = nb_log_config_default.LOG_FILE_SIZE
         if log_path is None:
             # print(nb_log_config_default.LOG_PATH)
             log_path = nb_log_config_default.LOG_PATH or '/pythonlogs'
         if formatter_template is None:
             formatter_template = nb_log_config_default.FORMATTER_KIND
 
-        self._logger_level = log_level_int * 10 if log_level_int < 10 else log_level_int
+        check_log_level(log_level_int)
+        self._logger_level = log_level_int
         # if self._logger_name in self.preset_name__level_map:
         #     # print(self.preset_name__level_map)
         #     self._logger_level = (self.preset_name__level_map[self._logger_name])
         # else:
         #     self._logger_level = self._logger_level
         self._is_add_stream_handler = is_add_stream_handler
         self._do_not_use_color_handler = do_not_use_color_handler
```

### Comparing `nb_log-8.3/nb_log/monkey_print.py` & `nb_log-8.4/nb_log/monkey_print.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,40 @@
 
 """
 import multiprocessing
 import sys
 import time
 import traceback
 from nb_log import nb_log_config_default
-from nb_log.helper import need_filter_print
+from nb_log.helper import _need_filter_print
 
 print_raw = print
+sys_stdout_write_raw = sys.stdout.write
+sys_stderr_write_raw = sys.stderr.write
 
 WORD_COLOR = 37
 
 
+def _sys_stdout_write_monkey(msg: str):
+    if _need_filter_print(msg):
+        return
+    else:
+        sys_stdout_write_raw(msg)
+
+def _sys_stderr_write_monkey(msg: str):
+    if _need_filter_print(msg):
+        return
+    else:
+        sys_stderr_write_raw(msg)
+
+
+sys.stdout.write = _sys_stdout_write_monkey  # 对 sys.stdout.write 打了猴子补丁。使得可以过滤包含指定字符串的消息。
+sys.stderr.write = _sys_stderr_write_monkey
+
+
 def stdout_write(msg: str):
     sys.stdout.write(msg)
     sys.stdout.flush()
 
 
 def stderr_write(msg: str):
     sys.stderr.write(msg)
@@ -31,17 +50,14 @@
 def nb_print(*args, sep=' ', end='\n', file=None, flush=True):
     """
     超流弊的print补丁
     :param x:
     :return:
     """
 
-    if need_filter_print(sep.join(args)):
-        return
-
     args = (str(arg) for arg in args)  # REMIND 防止是数字不能被join
     if file == sys.stderr:
         stderr_write(sep.join(args))  # 如 threading 模块第926行，打印线程错误，希望保持原始的红色错误方式，不希望转成蓝色。
     elif file in [sys.stdout, None]:
         # 获取被调用函数在被调用时所处代码行数
         line = sys._getframe().f_back.f_lineno
         # 获取被调用函数所在模块文件名
@@ -146,16 +162,14 @@
 def is_main_process():
     return multiprocessing.process.current_process().name == 'MainProcess'
 
 
 # noinspection DuplicatedCode
 def only_print_on_main_process(*args, sep=' ', end='\n', file=None, flush=True):
     # 获取被调用函数在被调用时所处代码行数
-    if need_filter_print(sep.join(args)):
-        return
     if is_main_process():
         args = (str(arg) for arg in args)  # REMIND 防止是数字不能被join
         if file == sys.stderr:
             stderr_write(sep.join(args))  # 如 threading 模块第926行，打印线程错误，希望保持原始的红色错误方式，不希望转成蓝色。
         elif file in [sys.stdout, None]:
             # 获取被调用函数在被调用时所处代码行数
             line = sys._getframe().f_back.f_lineno
```

### Comparing `nb_log-8.3/nb_log/nb_log_config_default.py` & `nb_log-8.4/nb_log/nb_log_config_default.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,16 @@
    这个是采用了文件锁，多进程安全切割，文件锁在linux上使用fcntl性能还行，win上使用win32con性能非常惨。按大小切割建议不要选第5个个filehandler而是选择第1个。
 """
 
 LOG_LEVEL_FILTER = logging.DEBUG  # 默认日志级别，低于此级别的日志不记录了。例如设置为INFO，那么logger.debug的不会记录，只会记录logger.info以上级别的。
 # 强烈不建议调高这里的级别为INFO，日志是有命名空间的，单独提高打印啰嗦的日志命名空间的日志级别就可以了，不要全局提高日志级别。
 # https://nb-log-doc.readthedocs.io/zh_CN/latest/articles/c9.html#id2  文档9.5里面讲了几百次 python logging的命名空间的作用了，有些人到现在还不知道日志的name作用。
 
-# 屏蔽的字符串显示，用 if in {打印信息} 来判断实现的,如果打印的消息中包括 FILTER_WORDS_PRINT 数组中的任何一个字符串，那么消息就不执行打印。这个配置对 print 和 logger的控制台输出都生效。这个可以过滤某些啰嗦的print信息，也可以过滤同级别日志中的某些烦人的日志。
+# 屏蔽的字符串显示，用 if in {打印信息} 来判断实现的,如果打印的消息中包括 FILTER_WORDS_PRINT 数组中的任何一个字符串，那么消息就不执行打印。
+# 这个配置对 print 和 logger的控制台输出都生效。这个可以过滤某些啰嗦的print信息，也可以过滤同级别日志中的某些烦人的日志。可以用来过滤三方包中某些控制台打印。数组不要配置过多，否则有一丝丝影响性能会。
 FILTER_WORDS_PRINT = []  # 例如， 你希望消息中包括阿弥陀佛 或者 包括善哉善哉 就不打印，那么可以把  FILTER_WORDS_PRINT = ['阿弥陀佛','善哉善哉']
 
 RUN_ENV = 'test'
 
 FORMATTER_DICT = {
     1: logging.Formatter(
         '日志时间【%(asctime)s】 - 日志名称【%(name)s】 - 文件【%(filename)s】 - 第【%(lineno)d】行 - 日志等级【%(levelname)s】 - 日志信息【%(message)s】',
```

### Comparing `nb_log-8.3/nb_log/set_nb_log_config.py` & `nb_log-8.4/nb_log/set_nb_log_config.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.3/nb_log.egg-info/PKG-INFO` & `nb_log-8.4/nb_log.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-log
-Version: 8.3
+Version: 8.4
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-8.3/setup.py` & `nb_log-8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ]
 
 if os.name == 'nt':
     install_requires.append('pywin32')
 
 setup(
     name='nb_log',  #
-    version="8.3",
+    version="8.4",
     description=(
         'very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on '
     ),
     keywords=["logging", "logger", "multiprocess file handler", "color handler"],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
@@ -61,14 +61,14 @@
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
 
 python setup.py sdist & twine upload dist/nb_log-6.0.tar.gz
-python setup.py sdist & python -m  twine upload dist/nb_log-8.3.tar.gz
+python setup.py sdist & python -m  twine upload dist/nb_log-8.4.tar.gz
 
 twine upload dist/*
 
 
 python -m pip install nb_log --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```

