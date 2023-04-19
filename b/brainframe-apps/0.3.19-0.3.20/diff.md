# Comparing `tmp/brainframe_apps-0.3.19.tar.gz` & `tmp/brainframe_apps-0.3.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainframe_apps-0.3.19.tar", max compression
+gzip compressed data, was "brainframe_apps-0.3.20.tar", max compression
```

## Comparing `brainframe_apps-0.3.19.tar` & `brainframe_apps-0.3.20.tar`

### file list

```diff
@@ -1,26 +1,29 @@
--rw-r--r--   0        0        0      599 2023-04-09 00:36:44.237108 brainframe_apps-0.3.19/brainframe_apps/__init__.py
--rw-r--r--   0        0        0     4847 2023-04-10 05:04:21.218631 brainframe_apps-0.3.19/brainframe_apps/add_stream.py
--rw-r--r--   0        0        0      665 2022-12-19 23:19:56.515826 brainframe_apps-0.3.19/brainframe_apps/bf_log_print.py
--rw-r--r--   0        0        0    14973 2023-04-09 00:36:55.997030 brainframe_apps-0.3.19/brainframe_apps/capsule_control.py
--rw-r--r--   0        0        0     1115 2023-04-09 03:58:17.840070 brainframe_apps-0.3.19/brainframe_apps/cli.py
--rw-r--r--   0        0        0      571 2023-04-08 04:43:59.581232 brainframe_apps-0.3.19/brainframe_apps/command_utils.py
--rw-r--r--   0        0        0     2582 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/delete_stream.py
--rw-r--r--   0        0        0     4691 2022-12-19 23:19:56.515826 brainframe_apps-0.3.19/brainframe_apps/fps_report.py
--rw-r--r--   0        0        0     6343 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/get_configuration.py
--rw-r--r--   0        0        0     8070 2023-04-09 00:36:44.237108 brainframe_apps-0.3.19/brainframe_apps/get_zone_statuses.py
--rw-r--r--   0        0        0     4733 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/identity_control.py
--rw-r--r--   0        0        0     2434 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/license_control.py
--rw-r--r--   0        0        0     6284 2023-04-09 00:36:44.213108 brainframe_apps-0.3.19/brainframe_apps/list_stream.py
--rw-r--r--   0        0        0     2903 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/logger_factory.py
--rw-r--r--   0        0        0      734 2023-04-09 00:33:40.814733 brainframe_apps-0.3.19/brainframe_apps/print_utils.py
--rw-r--r--   0        0        0     4455 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/process_image.py
--rw-r--r--   0        0        0     9613 2023-04-10 05:04:21.218631 brainframe_apps-0.3.19/brainframe_apps/set_configuration.py
--rw-r--r--   0        0        0     3909 2023-04-10 05:04:21.218631 brainframe_apps-0.3.19/brainframe_apps/start_analyzing.py
--rw-r--r--   0        0        0     2153 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/stop_analyzing.py
--rw-r--r--   0        0        0     1046 2022-12-19 23:19:56.519826 brainframe_apps-0.3.19/brainframe_apps/time_utils.py
--rw-r--r--   0        0        0      862 2023-04-09 04:06:05.729507 brainframe_apps-0.3.19/brainframe_apps/translations/portal.en.yml
--rw-r--r--   0        0        0     3064 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/urls.py
--rw-r--r--   0        0        0     1037 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/wait_for_ready.py
--rw-r--r--   0        0        0      783 2023-04-10 23:39:20.670023 brainframe_apps-0.3.19/pyproject.toml
--rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 brainframe_apps-0.3.19/setup.py
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 brainframe_apps-0.3.19/PKG-INFO
+-rw-r--r--   0        0        0      638 2023-04-18 23:48:33.122778 brainframe_apps-0.3.20/brainframe_apps/__init__.py
+-rw-r--r--   0        0        0     4811 2023-04-17 00:40:49.913946 brainframe_apps-0.3.20/brainframe_apps/add_stream.py
+-rw-r--r--   0        0        0     1456 2023-04-19 18:29:12.650825 brainframe_apps-0.3.20/brainframe_apps/auth_dilili_tokens.py
+-rw-r--r--   0        0        0      665 2022-12-19 23:19:56.515826 brainframe_apps-0.3.20/brainframe_apps/bf_log_print.py
+-rw-r--r--   0        0        0    14973 2023-04-09 00:36:55.997030 brainframe_apps-0.3.20/brainframe_apps/capsule_control.py
+-rw-r--r--   0        0        0     1115 2023-04-09 03:58:17.840070 brainframe_apps-0.3.20/brainframe_apps/cli.py
+-rw-r--r--   0        0        0     5466 2023-04-19 18:29:12.682825 brainframe_apps-0.3.20/brainframe_apps/cognito_tokens.py
+-rw-r--r--   0        0        0      571 2023-04-08 04:43:59.581232 brainframe_apps-0.3.20/brainframe_apps/command_utils.py
+-rw-r--r--   0        0        0     2587 2023-04-18 21:54:38.559023 brainframe_apps-0.3.20/brainframe_apps/delete_stream.py
+-rw-r--r--   0        0        0     4691 2022-12-19 23:19:56.515826 brainframe_apps-0.3.20/brainframe_apps/fps_report.py
+-rw-r--r--   0        0        0     6343 2023-04-09 00:36:34.917171 brainframe_apps-0.3.20/brainframe_apps/get_configuration.py
+-rw-r--r--   0        0        0     8070 2023-04-09 00:36:44.237108 brainframe_apps-0.3.20/brainframe_apps/get_zone_statuses.py
+-rw-r--r--   0        0        0     4733 2023-04-09 00:36:34.917171 brainframe_apps-0.3.20/brainframe_apps/identity_control.py
+-rw-r--r--   0        0        0     2288 2023-04-17 00:40:49.913946 brainframe_apps-0.3.20/brainframe_apps/license_control.py
+-rw-r--r--   0        0        0     6284 2023-04-09 00:36:44.213108 brainframe_apps-0.3.20/brainframe_apps/list_stream.py
+-rw-r--r--   0        0        0     2903 2023-04-09 00:36:34.917171 brainframe_apps-0.3.20/brainframe_apps/logger_factory.py
+-rw-r--r--   0        0        0      734 2023-04-09 00:33:40.814733 brainframe_apps-0.3.20/brainframe_apps/print_utils.py
+-rw-r--r--   0        0        0     4455 2023-04-09 00:36:34.917171 brainframe_apps-0.3.20/brainframe_apps/process_image.py
+-rw-r--r--   0        0        0     9556 2023-04-17 00:40:49.913946 brainframe_apps-0.3.20/brainframe_apps/set_configuration.py
+-rw-r--r--   0        0        0     3848 2023-04-18 21:54:38.559023 brainframe_apps-0.3.20/brainframe_apps/start_analyzing.py
+-rw-r--r--   0        0        0     2086 2023-04-17 00:40:49.917946 brainframe_apps-0.3.20/brainframe_apps/stop_analyzing.py
+-rw-r--r--   0        0        0     1046 2022-12-19 23:19:56.519826 brainframe_apps-0.3.20/brainframe_apps/time_utils.py
+-rw-r--r--   0        0        0      881 2023-04-17 00:54:01.278847 brainframe_apps-0.3.20/brainframe_apps/translations/portal.en.yml
+-rw-r--r--   0        0        0     3064 2023-04-09 00:36:34.917171 brainframe_apps-0.3.20/brainframe_apps/urls.py
+-rw-r--r--   0        0        0     4032 2023-04-19 18:29:12.682825 brainframe_apps-0.3.20/brainframe_apps/user_control.py
+-rw-r--r--   0        0        0     1037 2023-04-09 00:36:34.917171 brainframe_apps-0.3.20/brainframe_apps/wait_for_ready.py
+-rw-r--r--   0        0        0      783 2023-04-17 17:09:56.087001 brainframe_apps-0.3.20/pyproject.toml
+-rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 brainframe_apps-0.3.20/setup.py
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 brainframe_apps-0.3.20/PKG-INFO
```

### Comparing `brainframe_apps-0.3.19/brainframe_apps/__init__.py` & `brainframe_apps-0.3.20/brainframe_apps/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,8 +6,9 @@
 from .get_configuration import save_settings_main
 from .start_analyzing import start_analyzing_main
 from .stop_analyzing import stop_analyzing_main
 from .capsule_control import capsule_control_main
 from .process_image import process_image_main
 from .get_zone_statuses import get_zone_statuses_main
 from .license_control import license_control
+from .user_control import user_control
 from .identity_control import identity_control_main
```

### Comparing `brainframe_apps-0.3.19/brainframe_apps/add_stream.py` & `brainframe_apps-0.3.20/brainframe_apps/add_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from brainframe_apps.list_stream import list_stream_parse_args
 from brainframe_apps.logger_factory import log
 from brainframe_apps.urls import UrlList
 
 from brainframe_apps.command_utils import command, subcommand_parse_args, by_name
 
 
-def add_stream(api, local_video_file, stream_url, no_print=True):
+def add_stream(api, local_video_file, stream_url):
     if local_video_file:
         video_bytes = Path(local_video_file).read_bytes()
         storage_id = api.new_storage(data=video_bytes, mime_type="video/mp4")
 
         stream_configuration_dict = bf_codecs.StreamConfiguration(
             name=local_video_file,
             premises_id=None,
@@ -94,24 +94,24 @@
         f"{os.path.basename(sys.argv[0])} Waiting for BrainFrame server at '{server_url}'"
     )
     api = BrainFrameAPI(server_url)
     api.wait_for_server_initialization()
 
     if args.stream_url is not None:
         stream_url = args.stream_url
-        stream_configuration = add_stream(api, args.video_file, stream_url, False)
+        stream_configuration = add_stream(api, args.video_file, stream_url)
     elif args.video_file is not None:
-        stream_configuration = add_stream(api, args.video_file, None, False)
+        stream_configuration = add_stream(api, args.video_file, None)
     elif args.stream_url_list is not None:
         stream_url_list = UrlList(args.stream_url_list)
         if stream_url_list:
             stream_configuration = None
             for stream_url in stream_url_list:
                 stream_configuration = add_stream(
-                    api, args.video_file, stream_url, False
+                    api, args.video_file, stream_url
                 )
         else:
             log.debug(f"Read {args.stream_url_list} failed")
     else:
         log.debug("No video source input")
```

### Comparing `brainframe_apps-0.3.19/brainframe_apps/bf_log_print.py` & `brainframe_apps-0.3.20/brainframe_apps/bf_log_print.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/brainframe_apps/capsule_control.py` & `brainframe_apps-0.3.20/brainframe_apps/capsule_control.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/brainframe_apps/cli.py` & `brainframe_apps-0.3.20/brainframe_apps/cli.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/brainframe_apps/command_utils.py` & `brainframe_apps-0.3.20/brainframe_apps/command_utils.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/brainframe_apps/delete_stream.py` & `brainframe_apps-0.3.20/brainframe_apps/delete_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     stream = None
 
     try:
         for stream in streams:
 
             if stream_persistent_id is not None:
                 # only delete the matching streams
-                if get_stream_persistent_id(stream) == stream_persistent_id:
+                if str(get_stream_persistent_id(stream)) == stream_persistent_id:
                     api.delete_stream_configuration(stream.id, 5)
                     stream_id = stream.id
                     log.debug(
                         f"    {stream.id}: {stream.name} {stream_persistent_id} deleted"
                     )
             else:
                 # delete all streams
```

### Comparing `brainframe_apps-0.3.19/brainframe_apps/fps_report.py` & `brainframe_apps-0.3.20/brainframe_apps/fps_report.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/brainframe_apps/get_configuration.py` & `brainframe_apps-0.3.20/brainframe_apps/get_configuration.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/brainframe_apps/get_zone_statuses.py` & `brainframe_apps-0.3.20/brainframe_apps/get_zone_statuses.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/brainframe_apps/identity_control.py` & `brainframe_apps-0.3.20/brainframe_apps/identity_control.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/brainframe_apps/license_control.py` & `brainframe_apps-0.3.20/brainframe_apps/license_control.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,45 +5,39 @@
 
 from brainframe.api import BrainFrameAPI, bf_errors
 from brainframe_apps.logger_factory import log
 
 from brainframe_apps.command_utils import command, subcommand_parse_args, by_name
 
 
-def set_license(api, license_file, no_print=True):
+def set_license(api, license_file):
     with open(license_file, "r") as fp:
         license_key = fp.readlines()
 
     try:
         license_info = api.set_license_key(str(license_key))
         is_it_valid = license_info.state
         terms = license_info.terms
         message_str = f"License is {is_it_valid}\n {terms}"
     except Exception as e:
         message_str = f"Uploading license failed {e}: {license_key}"
 
-    if no_print:
-        log.debug(message_str)
-    else:
-        print(message_str)
+    log.debug(message_str)
 
 
-def get_license(api, no_print=True):
+def get_license(api):
     try:
         license_info = api.get_license_info()
         is_it_valid = license_info.state
         terms = license_info.terms
         message_str = f"License is {is_it_valid}\n {terms}"
     except Exception as e:
         message_str = f"Get license failed {e}"
 
-    if no_print:
-        log.debug(message_str)
-    else:
-        print(message_str)
+    log.debug(message_str)
 
 
 def _license_control_parse_args(parser):
     parser.add_argument(
         "--server-url",
         default="http://localhost",
         help="The BrainFrame server " "URL, Default: %(default)s",
```

### Comparing `brainframe_apps-0.3.19/brainframe_apps/list_stream.py` & `brainframe_apps-0.3.20/brainframe_apps/list_stream.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/brainframe_apps/logger_factory.py` & `brainframe_apps-0.3.20/brainframe_apps/logger_factory.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/brainframe_apps/print_utils.py` & `brainframe_apps-0.3.20/brainframe_apps/print_utils.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/brainframe_apps/process_image.py` & `brainframe_apps-0.3.20/brainframe_apps/process_image.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/brainframe_apps/set_configuration.py` & `brainframe_apps-0.3.20/brainframe_apps/set_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,25 +13,23 @@
 from brainframe_apps.list_stream import get_stream_id
 from brainframe_apps.urls import UrlList, get_ip
 from brainframe_apps.wait_for_ready import wait_for_capsule
 from brainframe_apps.logger_factory import log
 
 from brainframe_apps.command_utils import command, subcommand_parse_args, by_name
 
-def set_conf_global(local_video_file, stream_url, setting_file, api, no_print=True):
+def set_conf_global(local_video_file, stream_url, setting_file, api):
     # Load settings from config file
     with open(setting_file) as file:
         server_setting = json.load(file)
 
     load_global_capsule_options(server_setting, api)
 
 
-def set_conf_stream(
-    local_video_file, stream_persistent_id, setting_file, api, no_print=True
-):
+def set_conf_stream(local_video_file, stream_persistent_id, setting_file, api):
     # Load settings from config file
     with open(setting_file) as file:
         server_setting = json.load(file)
 
     if "localhost" in stream_persistent_id:
         stream_persistent_id_for_server = stream_persistent_id.replace(
             "localhost", get_ip()
@@ -234,32 +232,32 @@
 
     try:
         api.wait_for_server_initialization(timeout=15)
     except (TimeoutError, bf_errors.ServerNotReadyError):
         log.error(f"BrainFrame server connection timeout")
         return
 
-    set_conf_global(None, None, args.setting_file, api, False)
+    set_conf_global(None, None, args.setting_file, api)
 
     if args.stream_url is not None:
         stream_url = args.stream_url.replace("localhost", str(get_ip()))
 
         stream_id = set_conf_stream(
-            args.video_file, stream_url, args.setting_file, api, False
+            args.video_file, stream_url, args.setting_file, api
         )
         if stream_id is not None:
             log.debug(f"Loading for {stream_url} has succeeded.")
         else:
             log.error(f"Loading for {stream_url} has failed.")
     else:
         stream_url_list = UrlList(args.stream_url_list)
         if stream_url_list:
             for stream_url in stream_url_list:
                 stream_id = set_conf_stream(
-                    args.video_file, stream_url, args.setting_file, api, False
+                    args.video_file, stream_url, args.setting_file, api
                 )
                 if stream_id is not None:
                     log.debug(f"Loading for {stream_url} has succeeded.")
                 else:
                     log.error(f"Loading for {stream_url} has failed.")
     
         else:
```

### Comparing `brainframe_apps-0.3.19/brainframe_apps/start_analyzing.py` & `brainframe_apps-0.3.20/brainframe_apps/start_analyzing.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 
 from brainframe_apps.list_stream import get_stream_persistent_id
 from brainframe_apps.logger_factory import log
 from brainframe_apps.urls import UrlList, get_ip
 from brainframe_apps.command_utils import command, subcommand_parse_args, by_name
 
 
-def start_analyzing(api, stream_url, no_print=True):
+def start_analyzing(api, stream_url):
     stream_id = analyzing_on_off_persistent_id(api, stream_url, True, False)
 
-    if not no_print:
-        if stream_id is not None:
-            log.debug(
-                f"{os.path.basename(__file__)}: {stream_url} succeeded: {stream_id}"
-            )
-        else:
-            log.error(f"{os.path.basename(__file__)}: {stream_url} failed")
+    if stream_id is not None:
+        log.debug(
+            f"{os.path.basename(__file__)}: {stream_url} succeeded: {stream_id}"
+        )
+    else:
+        log.error(f"{os.path.basename(__file__)}: {stream_url} failed")
 
     return stream_id
 
 
 def analyzing_on_off_persistent_id(
     api, stream_persistent_id, analyzing_on, keyframe_only
 ):
@@ -35,15 +34,15 @@
 
     stream_id = None
     try:
         streams = api.get_stream_configurations()
 
         for stream in streams:
             server_stream_persistent_id = get_stream_persistent_id(stream)
-            if stream_persistent_id == server_stream_persistent_id:
+            if stream_persistent_id == str(server_stream_persistent_id):
                 _analyzing_on_off(api, stream.id, analyzing_on, keyframe_only)
                 stream_id = stream.id
                 break
 
     except (bf_errors.ServerNotReadyError, json.decoder.JSONDecodeError) as e:
         log.error(f"{e}")
 
@@ -113,15 +112,15 @@
     except (TimeoutError, bf_errors.ServerNotReadyError):
         log.error(f"BrainFrame server connection timeout")
         return
 
     if args.stream_url is not None:
         stream_url = args.stream_url.replace("localhost", str(get_ip()))
 
-        stream_id = start_analyzing(api, stream_url, True)
+        stream_id = start_analyzing(api, stream_url)
 
     else:
         stop_analyzing_all(api)
 
 
 if __name__ == "__main__":
     by_name["start_analyzing"]()
```

### Comparing `brainframe_apps-0.3.19/brainframe_apps/stop_analyzing.py` & `brainframe_apps-0.3.20/brainframe_apps/stop_analyzing.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,23 @@
     analyzing_on_off_all,
     analyzing_on_off_persistent_id,
     start_analyzing_parse_args,
 )
 from brainframe_apps.urls import UrlList, get_ip
 from brainframe_apps.command_utils import command, subcommand_parse_args, by_name
 
-def stop_analyzing(api, stream_url, no_print=True):
+def stop_analyzing(api, stream_url):
     stream_id = analyzing_on_off_persistent_id(api, stream_url, False, False)
 
-    if not no_print:
-        if stream_id is not None:
-            log.debug(
-                f"{os.path.basename(__file__)}: {stream_url} succeeded: {stream_id}"
-            )
-        else:
-            log.error(f"{os.path.basename(__file__)}: {stream_url} failed")
+    if stream_id is not None:
+        log.debug(
+            f"{os.path.basename(__file__)}: {stream_url} succeeded: {stream_id}"
+        )
+    else:
+        log.error(f"{os.path.basename(__file__)}: {stream_url} failed")
 
     return stream_id
 
 
 def stop_analyzing_all(api):
     analyzing_on_off_all(api, False)
 
@@ -49,15 +48,15 @@
     except (TimeoutError, bf_errors.ServerNotReadyError):
         log.error(f"BrainFrame server connection timeout")
         return
 
     if args.stream_url is not None:
         stream_url = args.stream_url.replace("localhost", str(get_ip()))
 
-        stream_id = stop_analyzing(api, stream_url, False)
+        stream_id = stop_analyzing(api, stream_url)
 
         if stream_id is not None:
             log.debug(f"{stream_id} {stream_url}: analyzing has stopped")
         else:
             log.error(f"{stream_id} {stream_url}: stop analyzing has failed")
     else:
         stream_id = stop_analyzing_all(api)
```

### Comparing `brainframe_apps-0.3.19/brainframe_apps/time_utils.py` & `brainframe_apps-0.3.20/brainframe_apps/time_utils.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/brainframe_apps/translations/portal.en.yml` & `brainframe_apps-0.3.20/brainframe_apps/translations/portal.en.yml`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
       start_analyzing
       stop_analyzing
       get_zone_statuses
       process_image
       capsule_control
       identity_control
       license_control
+      user_control
 
     Examples:
       brainframe_apps add_stream --server-url SERVER_URL --stream-url STREAM_URL
       brainframe_apps add_stream --help
       brainframe_apps start_analyzing
  
   command-help: "The brainframe-apps command to run"
```

### Comparing `brainframe_apps-0.3.19/brainframe_apps/urls.py` & `brainframe_apps-0.3.20/brainframe_apps/urls.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/brainframe_apps/wait_for_ready.py` & `brainframe_apps-0.3.20/brainframe_apps/wait_for_ready.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.19/pyproject.toml` & `brainframe_apps-0.3.20/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainframe-apps"
-version = "0.3.19"
+version = "0.3.20"
 description = "BrainFrame Apps use BrainFrame REST API to interact with the BrainFrame OS"
 authors = ["Stephen Li <stephen@dilililabs.com>"]
 license = "BSD License"
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `brainframe_apps-0.3.19/setup.py` & `brainframe_apps-0.3.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['brainframe-api>=0.29.1,<0.30.0']
 
 entry_points = \
 {'console_scripts': ['brainframe-apps = brainframe_apps.cli:cli_main']}
 
 setup_kwargs = {
     'name': 'brainframe-apps',
-    'version': '0.3.19',
+    'version': '0.3.20',
     'description': 'BrainFrame Apps use BrainFrame REST API to interact with the BrainFrame OS',
     'long_description': 'None',
     'author': 'Stephen Li',
     'author_email': 'stephen@dilililabs.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `brainframe_apps-0.3.19/PKG-INFO` & `brainframe_apps-0.3.20/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainframe-apps
-Version: 0.3.19
+Version: 0.3.20
 Summary: BrainFrame Apps use BrainFrame REST API to interact with the BrainFrame OS
 License: BSD License
 Author: Stephen Li
 Author-email: stephen@dilililabs.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
```

