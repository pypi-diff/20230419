# Comparing `tmp/xj_recycle-1.0.3.tar.gz` & `tmp/xj_recycle-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xj_recycle-1.0.3.tar", last modified: Tue Sep 27 15:27:56 2022, max compression
+gzip compressed data, was "dist\xj_recycle-1.0.4.tar", last modified: Wed Apr 19 05:27:44 2023, max compression
```

## Comparing `xj_recycle-1.0.3.tar` & `xj_recycle-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-09-27 15:27:56.865494 xj_recycle-1.0.3/
--rw-rw-rw-   0        0        0     1969 2022-09-27 15:27:56.865494 xj_recycle-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2022-05-06 14:37:00.000000 xj_recycle-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2022-09-27 15:27:56.866491 xj_recycle-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      893 2022-09-27 15:27:43.000000 xj_recycle-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-27 15:27:56.852529 xj_recycle-1.0.3/xj_recycle/
--rw-rw-rw-   0        0        0        0 2022-07-29 14:35:59.000000 xj_recycle-1.0.3/xj_recycle/__init__.py
--rw-rw-rw-   0        0        0      595 2022-07-29 14:35:59.000000 xj_recycle-1.0.3/xj_recycle/admin.py
-drwxrwxrwx   0        0        0        0 2022-09-27 15:27:56.861504 xj_recycle-1.0.3/xj_recycle/apis/
--rw-rw-rw-   0        0        0        0 2022-07-29 14:35:59.000000 xj_recycle-1.0.3/xj_recycle/apis/__init__.py
--rw-rw-rw-   0        0        0      635 2022-07-29 14:35:59.000000 xj_recycle-1.0.3/xj_recycle/apis/recycle_bin_add.py
--rw-rw-rw-   0        0        0     2405 2022-07-29 14:35:59.000000 xj_recycle-1.0.3/xj_recycle/apis/recycle_bin_list.py
--rw-rw-rw-   0        0        0     1211 2022-07-29 14:35:59.000000 xj_recycle-1.0.3/xj_recycle/apis/recycle_bin_restore.py
--rw-rw-rw-   0        0        0      238 2022-09-05 15:41:35.000000 xj_recycle-1.0.3/xj_recycle/apps.py
--rw-rw-rw-   0        0        0     1893 2022-07-29 14:35:59.000000 xj_recycle-1.0.3/xj_recycle/models.py
-drwxrwxrwx   0        0        0        0 2022-09-27 15:27:56.864496 xj_recycle-1.0.3/xj_recycle/services/
--rw-rw-rw-   0        0        0        0 2022-07-29 14:35:59.000000 xj_recycle-1.0.3/xj_recycle/services/__init__.py
--rw-rw-rw-   0        0        0     6967 2022-07-29 14:35:59.000000 xj_recycle-1.0.3/xj_recycle/services/recycle_service.py
--rw-rw-rw-   0        0        0     2814 2022-07-29 14:35:59.000000 xj_recycle-1.0.3/xj_recycle/tool.py
--rw-rw-rw-   0        0        0      559 2022-07-29 14:35:59.000000 xj_recycle-1.0.3/xj_recycle/urls.py
-drwxrwxrwx   0        0        0        0 2022-09-27 15:27:56.857515 xj_recycle-1.0.3/xj_recycle.egg-info/
--rw-rw-rw-   0        0        0     1969 2022-09-27 15:27:56.000000 xj_recycle-1.0.3/xj_recycle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2022-09-27 15:27:56.000000 xj_recycle-1.0.3/xj_recycle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-27 15:27:56.000000 xj_recycle-1.0.3/xj_recycle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-09-27 15:27:56.000000 xj_recycle-1.0.3/xj_recycle.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 05:27:44.000000 xj_recycle-1.0.4/
+-rw-rw-rw-   0        0        0     1969 2023-04-19 05:27:44.000000 xj_recycle-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2022-08-08 01:33:13.000000 xj_recycle-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 05:27:44.000000 xj_recycle-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-04-19 05:27:27.000000 xj_recycle-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 05:27:44.000000 xj_recycle-1.0.4/xj_recycle/
+-rw-rw-rw-   0        0        0        0 2022-08-08 01:33:13.000000 xj_recycle-1.0.4/xj_recycle/__init__.py
+-rw-rw-rw-   0        0        0      595 2022-08-08 01:33:13.000000 xj_recycle-1.0.4/xj_recycle/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-19 05:27:44.000000 xj_recycle-1.0.4/xj_recycle/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-08 01:33:13.000000 xj_recycle-1.0.4/xj_recycle/apis/__init__.py
+-rw-rw-rw-   0        0        0      635 2022-08-08 01:33:13.000000 xj_recycle-1.0.4/xj_recycle/apis/recycle_bin_add.py
+-rw-rw-rw-   0        0        0     2405 2022-08-08 01:33:13.000000 xj_recycle-1.0.4/xj_recycle/apis/recycle_bin_list.py
+-rw-rw-rw-   0        0        0     1211 2022-08-08 01:33:13.000000 xj_recycle-1.0.4/xj_recycle/apis/recycle_bin_restore.py
+-rw-rw-rw-   0        0        0      219 2022-08-08 01:33:13.000000 xj_recycle-1.0.4/xj_recycle/apps.py
+-rw-rw-rw-   0        0        0     1878 2023-04-18 14:44:55.000000 xj_recycle-1.0.4/xj_recycle/models.py
+drwxrwxrwx   0        0        0        0 2023-04-19 05:27:44.000000 xj_recycle-1.0.4/xj_recycle/services/
+-rw-rw-rw-   0        0        0        0 2022-08-08 01:33:13.000000 xj_recycle-1.0.4/xj_recycle/services/__init__.py
+-rw-rw-rw-   0        0        0     6967 2022-08-08 01:33:13.000000 xj_recycle-1.0.4/xj_recycle/services/recycle_service.py
+-rw-rw-rw-   0        0        0     2814 2022-08-08 01:33:13.000000 xj_recycle-1.0.4/xj_recycle/tool.py
+-rw-rw-rw-   0        0        0      559 2022-08-08 01:33:13.000000 xj_recycle-1.0.4/xj_recycle/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-19 05:27:44.000000 xj_recycle-1.0.4/xj_recycle.egg-info/
+-rw-rw-rw-   0        0        0     1969 2023-04-19 05:27:44.000000 xj_recycle-1.0.4/xj_recycle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1969 2023-04-19 05:25:18.000000 xj_recycle-1.0.4/xj_recycle.egg-info/PKG-INFO~12c86d998be384ef2e8ad65713880f88b1070905
+-rw-rw-rw-   0        0        0      554 2023-04-19 05:27:44.000000 xj_recycle-1.0.4/xj_recycle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 05:27:44.000000 xj_recycle-1.0.4/xj_recycle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-19 05:27:44.000000 xj_recycle-1.0.4/xj_recycle.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `xj_recycle-1.0.3/PKG-INFO` & `xj_recycle-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_recycle
-Version: 1.0.3
+Version: 1.0.4
 Summary: 回收模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sieyoo@163.com
 Maintainer: 孙楷炎
 Maintainer-email: sky4834@163.com
 License: apache 3.0
```

### Comparing `xj_recycle-1.0.3/README.md` & `xj_recycle-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `xj_recycle-1.0.3/setup.py` & `xj_recycle-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_recycle',  # 模块名称
-    version='1.0.3',  # 模块版本
+    version='1.0.4',  # 模块版本
     description='回收模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     author='赵向明',  # 作者
     author_email='sieyoo@163.com',  # 作者邮箱
     maintainer="孙楷炎",  # 维护者
     maintainer_email="sky4834@163.com",  # 维护者的邮箱地址
```

### Comparing `xj_recycle-1.0.3/xj_recycle/admin.py` & `xj_recycle-1.0.4/xj_recycle/admin.py`

 * *Files identical despite different names*

### Comparing `xj_recycle-1.0.3/xj_recycle/apis/recycle_bin_add.py` & `xj_recycle-1.0.4/xj_recycle/apis/recycle_bin_add.py`

 * *Files identical despite different names*

### Comparing `xj_recycle-1.0.3/xj_recycle/apis/recycle_bin_list.py` & `xj_recycle-1.0.4/xj_recycle/apis/recycle_bin_list.py`

 * *Files identical despite different names*

### Comparing `xj_recycle-1.0.3/xj_recycle/apis/recycle_bin_restore.py` & `xj_recycle-1.0.4/xj_recycle/apis/recycle_bin_restore.py`

 * *Files identical despite different names*

### Comparing `xj_recycle-1.0.3/xj_recycle/models.py` & `xj_recycle-1.0.4/xj_recycle/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class RecycleBin(models.Model):
     # 回收站模块（删除还原功能）
     id = models.AutoField(primary_key=True, auto_created=True)
     user_id = models.BigIntegerField('用户ID', blank=True, null=True, )
     user_name = models.CharField('用户名', max_length=255, blank=True, null=True)
-    title = models.CharField('回收标题', max_length=255, blank=True, null=True, db_index=True)  # 数据标题。用于搜索
+    title = models.CharField('回收标题', max_length=255, blank=True, null=True)  # 数据标题。用于搜索
     summary = models.CharField('回收摘要', max_length=255, blank=True, null=True,
                                db_index=True)  # 摘要。用于模糊搜索。开发者自定义内容，如：张三删除站码1003，站名陈家沟，位于河南省开封市的测站
     from_table = models.CharField('回收来源表', max_length=128)
     primary_key = models.CharField('回收主键', max_length=128)  # 目标表的主键
     target_id = models.BigIntegerField('主键值', blank=False)
     target_data = models.TextField('备份数据', blank=False)  # 目标数据。删除时的回收数据区，json<object>结构
     keys_map = models.TextField('key关联', blank=True,
```

### Comparing `xj_recycle-1.0.3/xj_recycle/services/recycle_service.py` & `xj_recycle-1.0.4/xj_recycle/services/recycle_service.py`

 * *Files identical despite different names*

### Comparing `xj_recycle-1.0.3/xj_recycle/tool.py` & `xj_recycle-1.0.4/xj_recycle/tool.py`

 * *Files identical despite different names*

### Comparing `xj_recycle-1.0.3/xj_recycle/urls.py` & `xj_recycle-1.0.4/xj_recycle/urls.py`

 * *Files identical despite different names*

### Comparing `xj_recycle-1.0.3/xj_recycle.egg-info/PKG-INFO` & `xj_recycle-1.0.4/xj_recycle.egg-info/PKG-INFO~12c86d998be384ef2e8ad65713880f88b1070905`

 * *Files identical despite different names*

