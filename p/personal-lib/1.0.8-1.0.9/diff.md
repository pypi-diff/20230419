# Comparing `tmp/personal_lib-1.0.8.tar.gz` & `tmp/personal_lib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal_lib-1.0.8.tar", last modified: Fri Sep 16 03:01:08 2022, max compression
+gzip compressed data, was "personal_lib-1.0.9.tar", last modified: Fri Oct 28 07:20:37 2022, max compression
```

## Comparing `personal_lib-1.0.8.tar` & `personal_lib-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-09-16 03:01:08.945464 personal_lib-1.0.8/
--rw-rw-rw-   0        0        0      193 2022-09-16 03:01:08.944463 personal_lib-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-09-16 03:01:08.859492 personal_lib-1.0.8/personal_lib/
--rw-rw-rw-   0        0        0      150 2022-05-17 07:27:13.000000 personal_lib-1.0.8/personal_lib/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-16 03:01:08.941465 personal_lib-1.0.8/personal_lib/utils/
--rw-rw-rw-   0        0        0        0 2022-01-12 01:55:29.000000 personal_lib-1.0.8/personal_lib/utils/__init__.py
--rw-rw-rw-   0        0        0     3926 2022-09-15 08:43:10.000000 personal_lib-1.0.8/personal_lib/utils/common_utils.py
--rw-rw-rw-   0        0        0      868 2022-05-19 08:32:23.000000 personal_lib-1.0.8/personal_lib/utils/db_utils.py
--rw-rw-rw-   0        0        0      604 2022-01-12 03:06:46.000000 personal_lib-1.0.8/personal_lib/utils/mail_utils.py
--rw-rw-rw-   0        0        0    12722 2022-09-16 02:58:52.000000 personal_lib-1.0.8/personal_lib/utils/ssh_utils.py
--rw-rw-rw-   0        0        0     1487 2022-09-16 02:58:18.000000 personal_lib-1.0.8/personal_lib/utils/test.py
--rw-rw-rw-   0        0        0    85728 2022-05-19 08:31:25.000000 personal_lib-1.0.8/personal_lib/utils/trade_dates.txt
--rw-rw-rw-   0        0        0      341 2022-05-17 07:26:59.000000 personal_lib-1.0.8/personal_lib/utils/wx_utils.py
-drwxrwxrwx   0        0        0        0 2022-09-16 03:01:08.881483 personal_lib-1.0.8/personal_lib.egg-info/
--rw-rw-rw-   0        0        0      193 2022-09-16 03:01:08.000000 personal_lib-1.0.8/personal_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2022-09-16 03:01:08.000000 personal_lib-1.0.8/personal_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-16 03:01:08.000000 personal_lib-1.0.8/personal_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2022-09-16 03:01:08.000000 personal_lib-1.0.8/personal_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2022-09-16 03:01:08.000000 personal_lib-1.0.8/personal_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-16 03:01:08.945464 personal_lib-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      408 2022-09-16 02:59:17.000000 personal_lib-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-28 07:20:37.711428 personal_lib-1.0.9/
+-rw-rw-rw-   0        0        0      193 2022-10-28 07:20:37.711428 personal_lib-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-10-28 07:20:37.688436 personal_lib-1.0.9/personal_lib/
+-rw-rw-rw-   0        0        0      150 2022-05-17 07:27:13.000000 personal_lib-1.0.9/personal_lib/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-28 07:20:37.708428 personal_lib-1.0.9/personal_lib/utils/
+-rw-rw-rw-   0        0        0        0 2022-01-12 01:55:29.000000 personal_lib-1.0.9/personal_lib/utils/__init__.py
+-rw-rw-rw-   0        0        0     5764 2022-09-22 07:24:19.000000 personal_lib-1.0.9/personal_lib/utils/common_utils.py
+-rw-rw-rw-   0        0        0     1101 2022-10-28 07:15:24.000000 personal_lib-1.0.9/personal_lib/utils/db_utils.py
+-rw-rw-rw-   0        0        0      604 2022-01-12 03:06:46.000000 personal_lib-1.0.9/personal_lib/utils/mail_utils.py
+-rw-rw-rw-   0        0        0    12722 2022-09-16 02:58:52.000000 personal_lib-1.0.9/personal_lib/utils/ssh_utils.py
+-rw-rw-rw-   0        0        0    85728 2022-05-19 08:31:25.000000 personal_lib-1.0.9/personal_lib/utils/trade_dates.txt
+-rw-rw-rw-   0        0        0      341 2022-05-17 07:26:59.000000 personal_lib-1.0.9/personal_lib/utils/wx_utils.py
+drwxrwxrwx   0        0        0        0 2022-10-28 07:20:37.695453 personal_lib-1.0.9/personal_lib.egg-info/
+-rw-rw-rw-   0        0        0      193 2022-10-28 07:20:37.000000 personal_lib-1.0.9/personal_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      668 2022-10-28 07:20:37.000000 personal_lib-1.0.9/personal_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-28 07:20:37.000000 personal_lib-1.0.9/personal_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2022-10-28 07:20:37.000000 personal_lib-1.0.9/personal_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2022-10-28 07:20:37.000000 personal_lib-1.0.9/personal_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-10-28 07:20:37.711428 personal_lib-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      408 2022-10-28 07:17:21.000000 personal_lib-1.0.9/setup.py
```

### Comparing `personal_lib-1.0.8/personal_lib/utils/common_utils.py` & `personal_lib-1.0.9/personal_lib/utils/common_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import os
 import numpy as np
 import stat, errno, shutil
 import random
 import string
 from datetime import datetime
 import time
+from nt import DirEntry
+
 
 def code_process(codes, add_market=False):
     '''
     处理股票代码
     :param codes:
     :param add_market:
     :return:
@@ -123,9 +125,73 @@
             if current_datetime > update_time > pre_time_point:
                 print(f'当前时间大于文件更新时间大于预测时间节点，开始预测')
                 break
         time.sleep(1)
         current_datetime = datetime.now()
 
 
+def find_path(file, dir):
+    try:
+        fs = os.scandir(dir)
+        for s in fs:
+            # path = os.path.join(dir, s)
+            if s.is_dir():
+                result = find_path(file, s.path)
+                if result is None:
+                    continue
+                else:
+                    return result
+            else:
+                if s.name == file:
+                    return s.path
+        return None
+    except:
+        print(dir + "  目录无访问权限")
+
+
+def pytree(dir, level=0):
+    def create_dir_content(dir_name, level, is_last):
+        if level == 0:
+            return dir_name
+        elif level == 1:
+            if not is_last:
+                return f'├── {dir_name}'
+            else:
+                return f'└── {dir_name}'
+        else:
+            pass
+
+    base_name = os.path.basename(dir)
+    if level == 0:
+        print(base_name)
+    else:
+        print('├' + ' ' * 3 * (level - 1) + '──' + base_name)
+    try:
+        fs = os.scandir(dir)
+        for s in fs:
+            if s.is_dir():
+                pytree(s.path, level + 1)
+            # else:
+            #     print('├' * level + '──' + s.name)
+        return None
+    except:
+        pass
+
+def tree(path, depth=0):
+    if depth == 0:
+        print(path)
+    items = os.listdir(path)
+    for i in range(len(items)):
+        item = items[i]
+        # 输出文件夹中的文件和子文件夹名
+        if i != len(items)-1:
+            print('│    ' * depth, end='')
+            print('├──', item)
+        else:
+            print('     ' * depth, end='')
+            print('└──', item)
+        item = os.path.join(path, item)
+        if os.path.isdir(item):
+            tree(item, depth+1)
+
 if __name__ == '__main__':
-    rm_dir('D:/D2B')
+    tree('D:/test')
```

### Comparing `personal_lib-1.0.8/personal_lib/utils/db_utils.py` & `personal_lib-1.0.9/personal_lib/utils/db_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 import pandas as pd
 import pymysql
 from pymysql.cursors import DictCursor
 
-connection_dict = {}
-current_conn = None
+conn_pool = {}
 
 
-def connect(host, port, user, passwd, db, conn_name=None):
-    global current_conn
-    conn = pymysql.connect(user=user, passwd=passwd, host=host, port=port, db=db)
-    if conn_name is not None:
-        connection_dict[conn_name] = conn
-    current_conn = conn
-    return conn
-
-
-def close(conn):
-    conn.close()
-
-
-def query_data(sql, conn_name=None):
-    conn = None
-    if conn_name is not None:
-        conn = connection_dict[conn_name]
-    elif current_conn is not None:
-        conn = current_conn
-    if conn is None:
-        raise Exception('database was not connected')
-    cursor = conn.cursor(DictCursor)
-    cursor.execute(sql)
-    results = cursor.fetchall()
-    df = pd.DataFrame(results)
-    return df
+def add_connect(host, port, user, passwd, db, name):
+    global conn_pool
+    db = DBConn(host, port, user, passwd, db, name)
+    conn_pool[db.name] = db
+
+
+def get_conn(name):
+    global conn_pool
+    current_conn = conn_pool[name]
+    return current_conn
+
+
+class DBConn():
+    def __init__(self, host, port, user, passwd, db, name):
+        self.name = name
+        self.conn = pymysql.connect(user=user, passwd=passwd, host=host, port=port, db=db)
+        self.cur = self.conn.cursor(DictCursor)
+
+    def close(self):
+        if self.conn is not None:
+            self.conn.close()
+
+    def query_data(self, sql, args=None):
+        self.cur.execute(sql, args)
+        results = self.cur.fetchall()
+        df = pd.DataFrame(results)
+        return df
+
+    def exec_sql(self, sql, args=None):
+        self.cur.execute(sql, args)
+        self.conn.commit()
+
+    def exec_many(self, sql, args=None):
+        self.cur.executemany(sql, args)
+        self.conn.commit()
```

### Comparing `personal_lib-1.0.8/personal_lib/utils/mail_utils.py` & `personal_lib-1.0.9/personal_lib/utils/mail_utils.py`

 * *Files identical despite different names*

### Comparing `personal_lib-1.0.8/personal_lib/utils/ssh_utils.py` & `personal_lib-1.0.9/personal_lib/utils/ssh_utils.py`

 * *Files identical despite different names*

### Comparing `personal_lib-1.0.8/personal_lib/utils/trade_dates.txt` & `personal_lib-1.0.9/personal_lib/utils/trade_dates.txt`

 * *Files identical despite different names*

### Comparing `personal_lib-1.0.8/personal_lib.egg-info/SOURCES.txt` & `personal_lib-1.0.9/personal_lib.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 personal_lib.egg-info/requires.txt
 personal_lib.egg-info/top_level.txt
 personal_lib/utils/__init__.py
 personal_lib/utils/common_utils.py
 personal_lib/utils/db_utils.py
 personal_lib/utils/mail_utils.py
 personal_lib/utils/ssh_utils.py
-personal_lib/utils/test.py
 personal_lib/utils/trade_dates.txt
 personal_lib/utils/wx_utils.py
 personal_lib/utils/__init__.py
 personal_lib/utils/common_utils.py
 personal_lib/utils/db_utils.py
 personal_lib/utils/mail_utils.py
 personal_lib/utils/ssh_utils.py
```

