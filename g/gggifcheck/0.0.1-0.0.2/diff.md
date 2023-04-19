# Comparing `tmp/gggifcheck-0.0.1.tar.gz` & `tmp/gggifcheck-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gggifcheck-0.0.1.tar", last modified: Thu Apr 13 04:57:36 2023, max compression
+gzip compressed data, was "gggifcheck-0.0.2.tar", last modified: Wed Apr 19 07:37:07 2023, max compression
```

## Comparing `gggifcheck-0.0.1.tar` & `gggifcheck-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 04:57:36.938900 gggifcheck-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggifcheck-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3712 2023-04-13 04:57:36.938900 gggifcheck-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3002 2023-04-13 04:46:30.000000 gggifcheck-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 04:57:36.933913 gggifcheck-0.0.1/gggifcheck/
--rw-rw-rw-   0        0        0       86 2023-04-13 04:29:58.000000 gggifcheck-0.0.1/gggifcheck/__init__.py
--rw-rw-rw-   0        0        0    11428 2023-04-13 03:21:26.000000 gggifcheck-0.0.1/gggifcheck/fields.py
--rw-rw-rw-   0        0        0     6473 2023-04-13 03:04:31.000000 gggifcheck-0.0.1/gggifcheck/items.py
--rw-rw-rw-   0        0        0     1253 2023-04-13 04:43:25.000000 gggifcheck-0.0.1/gggifcheck/scrapy_ifcheck.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:57:36.937903 gggifcheck-0.0.1/gggifcheck.egg-info/
--rw-rw-rw-   0        0        0     3712 2023-04-13 04:57:36.000000 gggifcheck-0.0.1/gggifcheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-04-13 04:57:36.000000 gggifcheck-0.0.1/gggifcheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 04:57:36.000000 gggifcheck-0.0.1/gggifcheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-13 04:57:36.000000 gggifcheck-0.0.1/gggifcheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      770 2023-04-13 04:57:36.943430 gggifcheck-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      164 2023-04-13 03:43:33.000000 gggifcheck-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:07.334746 gggifcheck-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggifcheck-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4783 2023-04-19 07:37:07.335745 gggifcheck-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4073 2023-04-19 07:32:34.000000 gggifcheck-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:07.330924 gggifcheck-0.0.2/gggifcheck/
+-rw-rw-rw-   0        0        0       86 2023-04-13 04:29:58.000000 gggifcheck-0.0.2/gggifcheck/__init__.py
+-rw-rw-rw-   0        0        0    11500 2023-04-18 09:27:13.000000 gggifcheck-0.0.2/gggifcheck/fields.py
+-rw-rw-rw-   0        0        0     6948 2023-04-19 07:19:30.000000 gggifcheck-0.0.2/gggifcheck/items.py
+-rw-rw-rw-   0        0        0     2838 2023-04-19 07:32:34.000000 gggifcheck-0.0.2/gggifcheck/scrapy_ifcheck.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:07.334746 gggifcheck-0.0.2/gggifcheck.egg-info/
+-rw-rw-rw-   0        0        0     4783 2023-04-19 07:37:07.000000 gggifcheck-0.0.2/gggifcheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-04-19 07:37:07.000000 gggifcheck-0.0.2/gggifcheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 07:37:07.000000 gggifcheck-0.0.2/gggifcheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-19 07:37:07.000000 gggifcheck-0.0.2/gggifcheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      770 2023-04-19 07:37:07.340675 gggifcheck-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      164 2023-04-13 03:43:33.000000 gggifcheck-0.0.2/setup.py
```

### Comparing `gggifcheck-0.0.1/LICENSE` & `gggifcheck-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gggifcheck-0.0.1/README.md` & `gggifcheck-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: gggifcheck
+Version: 0.0.2
+Summary: 通用、便捷、准确的字符串时间解析工具
+Home-page: https://github.com/kusen-alpha/gggifcheck
+Author: kusen
+Author-email: hu1194542196@qq.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggifcheck/issues
+Project-URL: Documentation, https://github.com/kusen-alpha/gggifcheck/blob/master/README.md
+Project-URL: Source Code, https://github.com/kusen-alpha/gggifcheck
+Platform: any
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # gggifcheck
 
 通用条目字段检查(General General General Item Field Check)
 ，是基于Python编写通用检查工具，适应于各种场景的使用，只需要略微进行适配。
 
 ## 使用方法
 
@@ -53,44 +71,70 @@
 import scrapy
 from gggifcheck import fields
 from gggifcheck.items import CheckItem
 
 
 class ScrapyCheckItem(scrapy.Item, CheckItem):
 
+    def __init__(self, *args, **kwargs):
+        self._values = {}
+        self.check_fields = {}
+        if args or kwargs:
+            for k, v in dict(*args, **kwargs).items():
+                self[k] = v
+
     def __getitem__(self, key):
         if key in self.fields and key not in self._values:
             value = None
             for field1, field2 in self.relate_process_default:
                 value = self[field2]
                 break
             self[key] = value
         return self._values[key]
 
     def __setitem__(self, key, value):
         if key in self.fields:
-            field = self.fields[key]['check_field']
-            field.input(key, value)
-            self._values[key] = field.value
+            field = self.fields[key]
+            build_check_field = field.get('build_check_field')
+            if build_check_field:
+                check_field = build_check_field.build(key=key, value=value)
+                self.check_fields[key] = check_field
+                self._values[key] = check_field.value
+            else:
+                self._values[key] = value
         else:
             raise KeyError(
                 f"{self.__class__.__name__} does not support field: {key}")
 
     def __setattr__(self, name, value):
-        if name.startswith('_'):
+        if name.startswith('_') or name in ['check_fields']:
             self.__dict__[name] = value
         else:
             raise AttributeError(
                 f"Use item[{name!r}] = {value!r} to set field value")
 
     def keys(self):
         self._process_and_check()
         _ = [self[field] for field in self.fields]  # 进行所有字段检查
         return self._values.keys()
 
+    def get_base_value(self, key):
+        if key in self.check_fields:
+            return self.check_fields[key].base_value
+        elif key in self.fields:
+            field = self.fields[key]
+            build_check_field = field.get('build_check_field')
+            if build_check_field:
+                return build_check_field.build_default(
+                    key=key, value=None).base_value
+            return self.fields[key] or None
+        else:
+            raise KeyError(
+                f"{self.__class__.__name__} does not support field: {key}")
+
 
 # 示例
 class PostItem(ScrapyCheckItem):
     id = scrapy.Field(
         check_field=fields.MD5CheckField(
             nullable=False))
     channel = scrapy.Field(
@@ -104,8 +148,8 @@
 print(dict(item))
 ```
 
 ## 关于作者
 
 1. 邮箱：1194542196@qq.com
 2. 微信：hu1194542196
-3. 目前还需要很多需要改进的地方，可以私信作者，你们的提供越多，本库才能更完善。
+3. 目前还需要很多需要改进的地方，可以私信作者，你们的提供越多，本库才能更完善。
```

### Comparing `gggifcheck-0.0.1/gggifcheck/fields.py` & `gggifcheck-0.0.2/gggifcheck/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,18 @@
     def format(self, value):
         return value
 
     @property
     def value(self):
         return self.output()
 
+    @property
+    def base_value(self):
+        return self._value
+
     def check(self):
         errors = self._check()
         for error in errors:
             raise Exception(error)
 
     def _check(self):
         return [
```

### Comparing `gggifcheck-0.0.1/gggifcheck/items.py` & `gggifcheck-0.0.2/gggifcheck/items.py`

 * *Files 12% similar despite different names*

```diff
@@ -165,7 +165,22 @@
         else:
             raise AttributeError(
                 f"Use item[{name!r}] = {value!r} to set field value")
 
     def keys(self):  # to dict时优先调用，不会调用__iter__和__len__，但必须实现
         self._process_and_check()
         return self.fields.keys()
+
+
+class BuildCheckField(object):
+    def __init__(self, check_field_class, **kwargs):
+        self.check_field_class = check_field_class
+        self.kwargs = kwargs
+
+    def build(self, key, value):
+        check_field = self.check_field_class(**self.kwargs)
+        check_field.input(key, value)
+        return check_field
+
+    def build_default(self, key, value=None):
+        return self.check_field_class(
+            key=key, value=value, **self.kwargs)
```

### Comparing `gggifcheck-0.0.1/setup.cfg` & `gggifcheck-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6767 6966 6368 6563 6b0d 0a76   = gggifcheck..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e31 0d0a  ersion = 0.0.1..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e32 0d0a  ersion = 0.0.2..
 00000030: 6175 7468 6f72 203d 206b 7573 656e 0d0a  author = kusen..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2068  author_email = h
 00000050: 7531 3139 3435 3432 3139 3640 7171 2e63  u1194542196@qq.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 cda8 d3c3 a1a2 b1e3 bddd a1a2 d7bc  = ..............
 00000080: c8b7 b5c4 d7d6 b7fb b4ae cab1 bce4 bde2  ................
 00000090: cef6 b9a4 bedf 0d0a 6c6f 6e67 5f64 6573  ........long_des
```

