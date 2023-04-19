# Comparing `tmp/perm_broker-0.1.5.tar.gz` & `tmp/perm_broker-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perm_broker-0.1.5.tar", last modified: Sun May 22 15:16:45 2022, max compression
+gzip compressed data, was "perm_broker-0.1.6.tar", max compression
```

## Comparing `perm_broker-0.1.5.tar` & `perm_broker-0.1.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rwxr-xr-x   0        0        0        1 2021-04-08 04:00:01.972568 perm_broker-0.1.5/perm_broker/__init__.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.125079 perm_broker-0.1.5/perm_broker/auth/__init__.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.148080 perm_broker-0.1.5/perm_broker/auth/ops/__init__.py
--rwxr-xr-x   0        0        0     1648 2021-06-15 05:21:45.437718 perm_broker-0.1.5/perm_broker/auth/ops/common.py
--rwxr-xr-x   0        0        0     5365 2021-04-20 11:15:17.634688 perm_broker-0.1.5/perm_broker/auth/ops/dingtalk_auth.py
--rwxr-xr-x   0        0        0    10596 2021-04-19 01:53:59.140475 perm_broker-0.1.5/perm_broker/auth/ops/pass_auth.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.819243 perm_broker-0.1.5/perm_broker/auth/views/__init__.py
--rwxr-xr-x   0        0        0     7560 2021-04-20 05:50:24.352093 perm_broker-0.1.5/perm_broker/auth/views/api.py
--rwxr-xr-x   0        0        0     1001 2021-04-20 05:49:51.948199 perm_broker-0.1.5/perm_broker/auth/views/debug_api.py
--rwxr-xr-x   0        0        0     3315 2021-04-19 01:54:39.483884 perm_broker-0.1.5/perm_broker/auth/views/web.py
--rwxr-xr-x   0        0        0     1733 2021-04-19 16:17:35.240289 perm_broker-0.1.5/perm_broker/backend/__init__.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:23:48.481050 perm_broker-0.1.5/perm_broker/backend/mongodb/__init__.py
--rwxr-xr-x   0        0        0     1010 2021-04-18 08:50:15.164123 perm_broker-0.1.5/perm_broker/backend/mongodb/helper.py
--rwxr-xr-x   0        0        0     7403 2021-04-12 04:01:02.799251 perm_broker-0.1.5/perm_broker/backend/mongodb/models.py
--rwxr-xr-x   0        0        0     1992 2021-04-08 02:36:18.373066 perm_broker-0.1.5/perm_broker/backend/mongodb/util.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:24:06.111322 perm_broker-0.1.5/perm_broker/backend/mssql/__init__.py
--rwxr-xr-x   0        0        0     1796 2021-04-19 16:08:52.183937 perm_broker-0.1.5/perm_broker/backend/mssql/helper.py
--rwxr-xr-x   0        0        0     6835 2022-05-22 15:12:18.126089 perm_broker-0.1.5/perm_broker/backend/mssql/models.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:23:56.462111 perm_broker-0.1.5/perm_broker/backend/mysql/__init__.py
--rwxr-xr-x   0        0        0     1797 2021-06-22 09:36:15.795297 perm_broker-0.1.5/perm_broker/backend/mysql/helper.py
--rwxr-xr-x   0        0        0     6490 2022-05-22 15:12:34.594047 perm_broker-0.1.5/perm_broker/backend/mysql/models.py
--rwxr-xr-x   0        0        0      371 2021-04-19 01:51:20.828270 perm_broker-0.1.5/perm_broker/common/__init__.py
--rwxr-xr-x   0        0        0      790 2021-04-19 02:28:48.208051 perm_broker-0.1.5/perm_broker/common/conf.py
--rwxr-xr-x   0        0        0      336 2021-04-07 04:10:42.861241 perm_broker-0.1.5/perm_broker/common/event.py
--rwxr-xr-x   0        0        0      218 2021-04-19 01:51:00.944279 perm_broker-0.1.5/perm_broker/common/exceptions.py
--rwxr-xr-x   0        0        0       43 2021-04-09 02:02:20.633462 perm_broker-0.1.5/perm_broker/context.py
--rwxr-xr-x   0        0        0      160 2021-04-14 08:50:04.214774 perm_broker-0.1.5/perm_broker/default.py
--rwxr-xr-x   0        0        0     1092 2021-06-12 08:24:51.888915 perm_broker-0.1.5/perm_broker/entry.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.919749 perm_broker-0.1.5/perm_broker/perm/__init__.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.946188 perm_broker-0.1.5/perm_broker/perm/ops/__init__.py
--rwxr-xr-x   0        0        0     1018 2021-04-07 04:10:42.949189 perm_broker-0.1.5/perm_broker/perm/ops/decr.py
--rwxr-xr-x   0        0        0     5027 2021-04-07 04:10:42.952188 perm_broker-0.1.5/perm_broker/perm/ops/perm_base.py
--rwxr-xr-x   0        0        0    16979 2021-04-18 13:55:34.378769 perm_broker-0.1.5/perm_broker/perm/ops/position.py
--rwxr-xr-x   0        0        0    10306 2021-06-15 07:27:43.387076 perm_broker-0.1.5/perm_broker/perm/ops/user_perm.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.030188 perm_broker-0.1.5/perm_broker/perm/views/__init__.py
--rwxr-xr-x   0        0        0    27107 2021-06-13 12:34:27.584245 perm_broker-0.1.5/perm_broker/perm/views/api.py
--rwxr-xr-x   0        0        0     1840 2021-04-07 04:10:43.626829 perm_broker-0.1.5/perm_broker/templates/dingtalk_login.html
--rwxr-xr-x   0        0        0     1564 2021-04-07 04:10:43.628831 perm_broker-0.1.5/perm_broker/templates/dingtalk_login_mobile.html
--rwxr-xr-x   0        0        0      107 2021-04-07 04:10:43.630829 perm_broker-0.1.5/perm_broker/templates/dingtalk_success.html
--rwxr-xr-x   0        0        0      248 2021-04-07 04:10:43.640829 perm_broker-0.1.5/perm_broker/templates/password_login.html
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.670828 perm_broker-0.1.5/perm_broker/user/__init__.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.707829 perm_broker-0.1.5/perm_broker/user/ops/__init__.py
--rwxr-xr-x   0        0        0     5725 2021-07-03 02:05:06.716092 perm_broker-0.1.5/perm_broker/user/ops/user_base.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.730833 perm_broker-0.1.5/perm_broker/user/views/__init__.py
--rwxr-xr-x   0        0        0     6391 2021-04-19 01:30:12.640053 perm_broker-0.1.5/perm_broker/user/views/api.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.743830 perm_broker-0.1.5/perm_broker/util/__init__.py
--rwxr-xr-x   0        0        0     2660 2021-06-23 00:32:57.086878 perm_broker-0.1.5/perm_broker/util/api_base.py
--rwxr-xr-x   0        0        0      198 2021-04-18 15:48:09.799058 perm_broker-0.1.5/perm_broker/util/cache_util.py
--rwxr-xr-x   0        0        0      355 2021-04-07 04:10:43.749659 perm_broker-0.1.5/perm_broker/util/chinese.py
--rwxr-xr-x   0        0        0     1992 2021-04-07 04:10:43.751819 perm_broker-0.1.5/perm_broker/util/db.py
--rwxr-xr-x   0        0        0      278 2022-05-22 15:15:40.748151 perm_broker-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 perm_broker-0.1.5/setup.py
--rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 perm_broker-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0        1 2021-04-08 04:00:01.000000 perm_broker-0.1.6/perm_broker/__init__.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/auth/__init__.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/auth/ops/__init__.py
+-rwxr-xr-x   0        0        0     1648 2021-06-15 05:21:45.000000 perm_broker-0.1.6/perm_broker/auth/ops/common.py
+-rwxr-xr-x   0        0        0     5365 2021-04-20 11:15:17.000000 perm_broker-0.1.6/perm_broker/auth/ops/dingtalk_auth.py
+-rwxr-xr-x   0        0        0    10596 2021-04-19 01:53:59.000000 perm_broker-0.1.6/perm_broker/auth/ops/pass_auth.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/auth/views/__init__.py
+-rwxr-xr-x   0        0        0     7560 2021-04-20 05:50:24.000000 perm_broker-0.1.6/perm_broker/auth/views/api.py
+-rwxr-xr-x   0        0        0     1040 2023-03-23 09:17:00.769764 perm_broker-0.1.6/perm_broker/auth/views/debug_api.py
+-rwxr-xr-x   0        0        0     3315 2021-04-19 01:54:39.000000 perm_broker-0.1.6/perm_broker/auth/views/web.py
+-rwxr-xr-x   0        0        0     1733 2021-04-19 16:17:35.000000 perm_broker-0.1.6/perm_broker/backend/__init__.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:23:48.000000 perm_broker-0.1.6/perm_broker/backend/mongodb/__init__.py
+-rwxr-xr-x   0        0        0     1010 2021-04-18 08:50:15.000000 perm_broker-0.1.6/perm_broker/backend/mongodb/helper.py
+-rwxr-xr-x   0        0        0     7403 2021-04-09 02:02:58.000000 perm_broker-0.1.6/perm_broker/backend/mongodb/models.py
+-rwxr-xr-x   0        0        0     1992 2021-04-08 02:36:18.000000 perm_broker-0.1.6/perm_broker/backend/mongodb/util.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:24:06.000000 perm_broker-0.1.6/perm_broker/backend/mssql/__init__.py
+-rwxr-xr-x   0        0        0     1796 2021-04-19 16:08:52.000000 perm_broker-0.1.6/perm_broker/backend/mssql/helper.py
+-rwxr-xr-x   0        0        0     6835 2022-05-22 15:11:35.000000 perm_broker-0.1.6/perm_broker/backend/mssql/models.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:23:56.000000 perm_broker-0.1.6/perm_broker/backend/mysql/__init__.py
+-rwxr-xr-x   0        0        0     1797 2021-06-22 09:36:15.000000 perm_broker-0.1.6/perm_broker/backend/mysql/helper.py
+-rwxr-xr-x   0        0        0     6490 2022-05-22 15:12:34.000000 perm_broker-0.1.6/perm_broker/backend/mysql/models.py
+-rwxr-xr-x   0        0        0      371 2021-04-19 01:51:20.000000 perm_broker-0.1.6/perm_broker/common/__init__.py
+-rwxr-xr-x   0        0        0      790 2021-04-19 02:28:48.000000 perm_broker-0.1.6/perm_broker/common/conf.py
+-rwxr-xr-x   0        0        0      336 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/common/event.py
+-rwxr-xr-x   0        0        0      218 2021-04-19 01:51:00.000000 perm_broker-0.1.6/perm_broker/common/exceptions.py
+-rwxr-xr-x   0        0        0       43 2021-04-09 02:02:20.000000 perm_broker-0.1.6/perm_broker/context.py
+-rwxr-xr-x   0        0        0      160 2021-04-14 08:50:04.000000 perm_broker-0.1.6/perm_broker/default.py
+-rwxr-xr-x   0        0        0     1092 2021-06-12 08:24:51.000000 perm_broker-0.1.6/perm_broker/entry.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/perm/__init__.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/perm/ops/__init__.py
+-rwxr-xr-x   0        0        0     1018 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/perm/ops/decr.py
+-rwxr-xr-x   0        0        0     5027 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/perm/ops/perm_base.py
+-rwxr-xr-x   0        0        0    16979 2021-04-18 13:55:34.000000 perm_broker-0.1.6/perm_broker/perm/ops/position.py
+-rwxr-xr-x   0        0        0    10306 2021-06-15 07:27:43.000000 perm_broker-0.1.6/perm_broker/perm/ops/user_perm.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/perm/views/__init__.py
+-rwxr-xr-x   0        0        0    27092 2023-04-19 01:34:21.916639 perm_broker-0.1.6/perm_broker/perm/views/api.py
+-rwxr-xr-x   0        0        0     1840 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/templates/dingtalk_login.html
+-rwxr-xr-x   0        0        0     1564 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/templates/dingtalk_login_mobile.html
+-rwxr-xr-x   0        0        0      107 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/templates/dingtalk_success.html
+-rwxr-xr-x   0        0        0      248 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/templates/password_login.html
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/user/__init__.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/user/ops/__init__.py
+-rwxr-xr-x   0        0        0     5725 2021-07-03 02:05:06.000000 perm_broker-0.1.6/perm_broker/user/ops/user_base.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/user/views/__init__.py
+-rwxr-xr-x   0        0        0     6391 2021-04-19 01:30:12.000000 perm_broker-0.1.6/perm_broker/user/views/api.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/util/__init__.py
+-rwxr-xr-x   0        0        0     2660 2021-06-23 00:32:57.000000 perm_broker-0.1.6/perm_broker/util/api_base.py
+-rwxr-xr-x   0        0        0      198 2021-04-18 15:48:09.000000 perm_broker-0.1.6/perm_broker/util/cache_util.py
+-rwxr-xr-x   0        0        0      355 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/util/chinese.py
+-rwxr-xr-x   0        0        0     1992 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/util/db.py
+-rwxr-xr-x   0        0        0      278 2023-04-19 01:39:57.575440 perm_broker-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 perm_broker-0.1.6/setup.py
+-rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 perm_broker-0.1.6/PKG-INFO
```

### Comparing `perm_broker-0.1.5/perm_broker/auth/ops/common.py` & `perm_broker-0.1.6/perm_broker/auth/ops/common.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/auth/ops/dingtalk_auth.py` & `perm_broker-0.1.6/perm_broker/auth/ops/dingtalk_auth.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/auth/ops/pass_auth.py` & `perm_broker-0.1.6/perm_broker/auth/ops/pass_auth.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/auth/views/api.py` & `perm_broker-0.1.6/perm_broker/auth/views/api.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/auth/views/debug_api.py` & `perm_broker-0.1.6/perm_broker/auth/views/debug_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 @pb_root.route('/auth/api/debug/login', methods=['GET'])
 def debug_login():
     if common.is_logined(flask.request, flask.session):
         return api_base.send_json_result("USER_LOGIN")
     user = None
     for k, v in flask.request.args.items():
+        if not k:
+            continue
         user = user_base.query_by_info(k, v).first()
         if user:
             break
     if user:
         common.login(user, flask.request, flask.session)
         common.record_login(str(user.id), 'debug', **flask.request.headers)
         return api_base.send_json_result("SUCC")
```

### Comparing `perm_broker-0.1.5/perm_broker/auth/views/web.py` & `perm_broker-0.1.6/perm_broker/auth/views/web.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/backend/__init__.py` & `perm_broker-0.1.6/perm_broker/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/backend/mongodb/helper.py` & `perm_broker-0.1.6/perm_broker/backend/mongodb/helper.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/backend/mongodb/models.py` & `perm_broker-0.1.6/perm_broker/backend/mongodb/models.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/backend/mongodb/util.py` & `perm_broker-0.1.6/perm_broker/backend/mongodb/util.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/backend/mssql/helper.py` & `perm_broker-0.1.6/perm_broker/backend/mssql/helper.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/backend/mssql/models.py` & `perm_broker-0.1.6/perm_broker/backend/mssql/models.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/backend/mysql/helper.py` & `perm_broker-0.1.6/perm_broker/backend/mysql/helper.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/backend/mysql/models.py` & `perm_broker-0.1.6/perm_broker/backend/mysql/models.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/common/conf.py` & `perm_broker-0.1.6/perm_broker/common/conf.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/entry.py` & `perm_broker-0.1.6/perm_broker/entry.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/perm/ops/decr.py` & `perm_broker-0.1.6/perm_broker/perm/ops/decr.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/perm/ops/perm_base.py` & `perm_broker-0.1.6/perm_broker/perm/ops/perm_base.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/perm/ops/position.py` & `perm_broker-0.1.6/perm_broker/perm/ops/position.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/perm/ops/user_perm.py` & `perm_broker-0.1.6/perm_broker/perm/ops/user_perm.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/perm/views/api.py` & `perm_broker-0.1.6/perm_broker/perm/views/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,15 +419,15 @@
 
 @pb_root.route('/perm/api/role/user/update', methods=['PUT'])
 @perm_required("pauli:perm:user:update")
 def api_update_user_role():
     data = flask.request.get_json(force=True, silent=True) or {}
     user_id = data.get('user_id')
     role_ids = data.get('role_ids') or []
-    if not (user_id and role_ids):
+    if not user_id:
         return api_base.send_json_result("FORBIDDEN")
     succ, obj = user_perm.update_user_roles(user_id, role_ids)
     if succ:
         roles = user_perm.get_user_roles(user_id)
         roles_list = list(map(lambda x: {'id': str(x.id), 'name': x.name}, roles))
         return api_base.send_json_result("SUCC",
                                    result={'roles': roles_list})
```

### Comparing `perm_broker-0.1.5/perm_broker/templates/dingtalk_login.html` & `perm_broker-0.1.6/perm_broker/templates/dingtalk_login.html`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/templates/dingtalk_login_mobile.html` & `perm_broker-0.1.6/perm_broker/templates/dingtalk_login_mobile.html`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/user/ops/user_base.py` & `perm_broker-0.1.6/perm_broker/user/ops/user_base.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/user/views/api.py` & `perm_broker-0.1.6/perm_broker/user/views/api.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/util/api_base.py` & `perm_broker-0.1.6/perm_broker/util/api_base.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/perm_broker/util/db.py` & `perm_broker-0.1.6/perm_broker/util/db.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.5/setup.py` & `perm_broker-0.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from distutils.core import setup
+from setuptools import setup
 
 packages = \
 ['perm_broker',
  'perm_broker.auth',
  'perm_broker.auth.ops',
  'perm_broker.auth.views',
  'perm_broker.backend',
@@ -20,20 +20,22 @@
  'perm_broker.util']
 
 package_data = \
 {'': ['*'], 'perm_broker': ['templates/*']}
 
 setup_kwargs = {
     'name': 'perm-broker',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': '',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Gongziting Tech Ltd.',
-    'author_email': None,
-    'url': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

