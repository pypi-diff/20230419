# Comparing `tmp/discord_data-0.1.2.tar.gz` & `tmp/discord_data-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_data-0.1.2.tar", last modified: Mon Apr  3 22:26:47 2023, max compression
+gzip compressed data, was "discord_data-0.2.0.tar", last modified: Wed Apr 19 02:18:49 2023, max compression
```

## Comparing `discord_data-0.1.2.tar` & `discord_data-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2023-04-03 22:26:47.728932 discord_data-0.1.2/
--rw-r--r--   0 sean      (1000) sean      (1000)    11358 2020-10-27 01:14:31.000000 discord_data-0.1.2/LICENSE
--rw-r--r--   0 sean      (1000) sean      (1000)       47 2020-10-27 01:14:31.000000 discord_data-0.1.2/MANIFEST.in
--rw-r--r--   0 sean      (1000) sean      (1000)     4158 2023-04-03 22:26:47.728932 discord_data-0.1.2/PKG-INFO
--rw-r--r--   0 sean      (1000) sean      (1000)     3415 2022-05-26 03:28:21.000000 discord_data-0.1.2/README.md
-drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2023-04-03 22:26:47.728932 discord_data-0.1.2/discord_data/
--rw-r--r--   0 sean      (1000) sean      (1000)      177 2021-03-24 06:41:39.000000 discord_data-0.1.2/discord_data/__init__.py
--rw-r--r--   0 sean      (1000) sean      (1000)     1459 2023-02-10 09:47:05.000000 discord_data-0.1.2/discord_data/__main__.py
--rw-r--r--   0 sean      (1000) sean      (1000)      216 2021-06-17 22:59:42.000000 discord_data-0.1.2/discord_data/common.py
--rw-r--r--   0 sean      (1000) sean      (1000)     2668 2021-06-17 22:59:42.000000 discord_data-0.1.2/discord_data/merge.py
--rw-r--r--   0 sean      (1000) sean      (1000)     2381 2022-05-26 09:05:53.000000 discord_data-0.1.2/discord_data/model.py
--rw-r--r--   0 sean      (1000) sean      (1000)     5516 2023-04-03 22:23:40.000000 discord_data-0.1.2/discord_data/parse.py
--rw-r--r--   0 sean      (1000) sean      (1000)        0 2021-03-15 08:07:44.000000 discord_data-0.1.2/discord_data/py.typed
-drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2023-04-03 22:26:47.728932 discord_data-0.1.2/discord_data.egg-info/
--rw-r--r--   0 sean      (1000) sean      (1000)     4158 2023-04-03 22:26:47.000000 discord_data-0.1.2/discord_data.egg-info/PKG-INFO
--rw-r--r--   0 sean      (1000) sean      (1000)      427 2023-04-03 22:26:47.000000 discord_data-0.1.2/discord_data.egg-info/SOURCES.txt
--rw-r--r--   0 sean      (1000) sean      (1000)        1 2023-04-03 22:26:47.000000 discord_data-0.1.2/discord_data.egg-info/dependency_links.txt
--rw-r--r--   0 sean      (1000) sean      (1000)       60 2023-04-03 22:26:47.000000 discord_data-0.1.2/discord_data.egg-info/entry_points.txt
--rw-r--r--   0 sean      (1000) sean      (1000)       24 2023-04-03 22:26:47.000000 discord_data-0.1.2/discord_data.egg-info/requires.txt
--rw-r--r--   0 sean      (1000) sean      (1000)       13 2023-04-03 22:26:47.000000 discord_data-0.1.2/discord_data.egg-info/top_level.txt
--rw-r--r--   0 sean      (1000) sean      (1000)      461 2023-04-03 22:26:47.732265 discord_data-0.1.2/setup.cfg
--rw-r--r--   0 sean      (1000) sean      (1000)     1486 2023-04-03 22:24:23.000000 discord_data-0.1.2/setup.py
+drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2023-04-19 02:18:49.877987 discord_data-0.2.0/
+-rw-r--r--   0 sean      (1000) sean      (1000)    11358 2020-10-27 01:14:31.000000 discord_data-0.2.0/LICENSE
+-rw-r--r--   0 sean      (1000) sean      (1000)       47 2020-10-27 01:14:31.000000 discord_data-0.2.0/MANIFEST.in
+-rw-r--r--   0 sean      (1000) sean      (1000)     4528 2023-04-19 02:18:49.877987 discord_data-0.2.0/PKG-INFO
+-rw-r--r--   0 sean      (1000) sean      (1000)     3785 2023-04-17 19:06:53.000000 discord_data-0.2.0/README.md
+drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2023-04-19 02:18:49.877987 discord_data-0.2.0/discord_data/
+-rw-r--r--   0 sean      (1000) sean      (1000)      177 2021-03-24 06:41:39.000000 discord_data-0.2.0/discord_data/__init__.py
+-rw-r--r--   0 sean      (1000) sean      (1000)     1459 2023-02-10 09:47:05.000000 discord_data-0.2.0/discord_data/__main__.py
+-rw-r--r--   0 sean      (1000) sean      (1000)      216 2021-06-17 22:59:42.000000 discord_data-0.2.0/discord_data/common.py
+-rw-r--r--   0 sean      (1000) sean      (1000)      132 2023-04-17 18:52:31.000000 discord_data-0.2.0/discord_data/error.py
+-rw-r--r--   0 sean      (1000) sean      (1000)     2860 2023-04-17 18:58:47.000000 discord_data-0.2.0/discord_data/merge.py
+-rw-r--r--   0 sean      (1000) sean      (1000)     2381 2022-05-26 09:05:53.000000 discord_data-0.2.0/discord_data/model.py
+-rw-r--r--   0 sean      (1000) sean      (1000)     6160 2023-04-17 18:56:48.000000 discord_data-0.2.0/discord_data/parse.py
+-rw-r--r--   0 sean      (1000) sean      (1000)        0 2021-03-15 08:07:44.000000 discord_data-0.2.0/discord_data/py.typed
+drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2023-04-19 02:18:49.877987 discord_data-0.2.0/discord_data.egg-info/
+-rw-r--r--   0 sean      (1000) sean      (1000)     4528 2023-04-19 02:18:49.000000 discord_data-0.2.0/discord_data.egg-info/PKG-INFO
+-rw-r--r--   0 sean      (1000) sean      (1000)      449 2023-04-19 02:18:49.000000 discord_data-0.2.0/discord_data.egg-info/SOURCES.txt
+-rw-r--r--   0 sean      (1000) sean      (1000)        1 2023-04-19 02:18:49.000000 discord_data-0.2.0/discord_data.egg-info/dependency_links.txt
+-rw-r--r--   0 sean      (1000) sean      (1000)       60 2023-04-19 02:18:49.000000 discord_data-0.2.0/discord_data.egg-info/entry_points.txt
+-rw-r--r--   0 sean      (1000) sean      (1000)       24 2023-04-19 02:18:49.000000 discord_data-0.2.0/discord_data.egg-info/requires.txt
+-rw-r--r--   0 sean      (1000) sean      (1000)       13 2023-04-19 02:18:49.000000 discord_data-0.2.0/discord_data.egg-info/top_level.txt
+-rw-r--r--   0 sean      (1000) sean      (1000)      461 2023-04-19 02:18:49.877987 discord_data-0.2.0/setup.cfg
+-rw-r--r--   0 sean      (1000) sean      (1000)     1486 2023-04-17 19:04:20.000000 discord_data-0.2.0/setup.py
```

### Comparing `discord_data-0.1.2/LICENSE` & `discord_data-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord_data-0.1.2/PKG-INFO` & `discord_data-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord_data
-Version: 0.1.2
+Version: 0.2.0
 Summary: Library to parse the Discord GDPR export
 Home-page: https://github.com/seanbreckenridge/discord_data
 Author: Sean Breckenridge
 Author-email: seanbrecke@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Keywords: discord data
 Classifier: License :: OSI Approved :: Apache Software License
@@ -93,8 +93,19 @@
 ```python
 # locates the corresponding `messages` directories in the folder structure
 list(merge_messages(export_dir="./discord"))`
 # supply a list of the message directories yourself
 list(merge_messages(paths=["./discord/march_2021/messages", "./discord/october_2020/messages"]))
 ```
 
+If the format for the discord export changes, the parse/merge functions will still work, they just might yield errors as part of their output. To ignore those, you can do:
+
+```python
+for msg in merge_messages(export_dir="./discord"):
+    if isinstance(msg, Exception):
+        logger.warning(msg)
+        continue
+    # do something with msg
+    print(msg.content)
+```
+
 Created to be used as part of [`HPI`](https://github.com/seanbreckenridge/HPI)
```

### Comparing `discord_data-0.1.2/README.md` & `discord_data-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -73,8 +73,19 @@
 ```python
 # locates the corresponding `messages` directories in the folder structure
 list(merge_messages(export_dir="./discord"))`
 # supply a list of the message directories yourself
 list(merge_messages(paths=["./discord/march_2021/messages", "./discord/october_2020/messages"]))
 ```
 
+If the format for the discord export changes, the parse/merge functions will still work, they just might yield errors as part of their output. To ignore those, you can do:
+
+```python
+for msg in merge_messages(export_dir="./discord"):
+    if isinstance(msg, Exception):
+        logger.warning(msg)
+        continue
+    # do something with msg
+    print(msg.content)
+```
+
 Created to be used as part of [`HPI`](https://github.com/seanbreckenridge/HPI)
```

### Comparing `discord_data-0.1.2/discord_data/__main__.py` & `discord_data-0.2.0/discord_data/__main__.py`

 * *Files identical despite different names*

### Comparing `discord_data-0.1.2/discord_data/merge.py` & `discord_data-0.2.0/discord_data/merge.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import warnings
 import logging
 from pathlib import Path
 from typing import Set, Optional, Iterator, List, Sequence
 
 from .model import Json, Message, Activity
+from .error import Res
 from .common import PathIsh, expand_path
 from .parse import (
     parse_messages,
     parse_raw_activity,
     _parse_activity_blob,
 )
 
@@ -59,27 +60,31 @@
 
 
 def merge_activity(
     *,
     export_dir: Optional[PathIsh] = None,
     paths: Optional[Sequence[PathIsh]] = None,
     logger: Optional[logging.Logger] = None,
-) -> Iterator[Activity]:
-    yield from map(
-        _parse_activity_blob,
-        merge_raw_activity(export_dir=export_dir, paths=paths, logger=logger),
-    )
+) -> Iterator[Res[Activity]]:
+    for rawact in merge_raw_activity(export_dir=export_dir, paths=paths, logger=logger):
+        try:
+            yield _parse_activity_blob(rawact)
+        except Exception as e:
+            yield e
 
 
 def merge_messages(
     *,
     export_dir: Optional[PathIsh] = None,
     paths: Optional[Sequence[PathIsh]] = None,
-) -> Iterator[Message]:
+) -> Iterator[Res[Message]]:
     emitted: Set[int] = set()
     for p in _list_exports("messages", export_dir, paths):
         for msg in parse_messages(p):
+            if isinstance(msg, Exception):
+                yield msg
+                continue
             key: int = msg.message_id
             if key in emitted:
                 continue
             yield msg
             emitted.add(msg.message_id)
```

### Comparing `discord_data-0.1.2/discord_data/model.py` & `discord_data-0.2.0/discord_data/model.py`

 * *Files identical despite different names*

### Comparing `discord_data-0.1.2/discord_data/parse.py` & `discord_data-0.2.0/discord_data/parse.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Iterator, Optional, Dict, List, Any, Union
 
 
 from .model import Message, Channel, Json, Activity, RegionInfo, Fingerprint, Server
 from .common import expand_path, PathIsh
+from .error import Res
 
 
-def get_self_user_id(export_root_dir: PathIsh) -> str:
+def _get_self_user_id(export_root_dir: PathIsh) -> str:
     user_info_f: Path = expand_path(export_root_dir) / "account" / "user.json"
     assert user_info_f.exists()
     user_json = json.loads(user_info_f.read_text())
     return str(user_json["id"])
 
 
 # timezone aware
@@ -38,65 +39,81 @@
         naive = datetime.fromisoformat(d)
         return naive.replace(tzinfo=timezone.utc)
     except ValueError as v:
         print(f"Could not parse datetime with any of the known formats: {ds}")
         raise v
 
 
-def parse_messages(messages_dir: PathIsh) -> Iterator[Message]:
+def parse_messages(messages_dir: PathIsh) -> Iterator[Res[Message]]:
     pmsg_dir: Path = expand_path(messages_dir)
     # get user id
-    # my_user: str = _get_self_user_id(pmsg_dir.parent)
 
     # parse index
     index_f = pmsg_dir / "index.json"
-    assert index_f.exists(), f"Message index 'index.json' doesnt exist at {index_f}"
+    if not index_f.exists():
+        yield RuntimeError(f"Message index 'index.json' doesnt exist at {index_f}")
+        return
     index: Dict[str, Optional[str]] = json.loads(index_f.read_text())
 
     # get individual message directories
     msg_dirs: List[Path] = list(
         filter(lambda d: d.is_dir() and not d.name.startswith("."), pmsg_dir.iterdir())
     )
     for msg_chan in msg_dirs:
         # chanel.json has some metadata about the channel/server
         channel_info_f: Path = msg_chan / "channel.json"
+        if not channel_info_f.exists():
+            yield RuntimeError(
+                f"Channel info 'channel.json' doesnt exist at {channel_info_f}"
+            )
+            continue
         channel_json: Dict[str, Any] = json.loads(channel_info_f.read_text())
 
         # optionally, find server information
         server_info: Optional[Server] = None
 
         # if the channel.json included guild (server) info
-        if "guild" in channel_json:
+        if (
+            "guild" in channel_json
+            and "id" in channel_json["guild"]
+            and "name" in channel_json["guild"]
+        ):
             server_info = Server(
                 server_id=int(channel_json["guild"]["id"]),
                 name=channel_json["guild"]["name"],
             )
 
         channel_name: Optional[str] = index.get(channel_json["id"])
 
+        if "id" not in channel_json:
+            yield RuntimeError(f"Channel id not found in {channel_info_f}")
+            continue
         channel_obj: Channel = Channel(
             channel_id=int(channel_json["id"]),
             name=channel_name,
             server=server_info,
         )
 
         # read CSV file to get messages
         with (msg_chan / "messages.csv").open("r", encoding="utf-8", newline="") as f:
             csv_reader = csv.reader(
                 f, delimiter=",", quotechar='"', quoting=csv.QUOTE_MINIMAL
             )
             next(csv_reader)  # ignore header row
             for row in csv_reader:
-                yield Message(
-                    message_id=int(row[0]),
-                    timestamp=_parse_message_datetime(row[1]),
-                    channel=channel_obj,
-                    content=row[2],
-                    attachments=row[3],
-                )
+                try:
+                    yield Message(
+                        message_id=int(row[0]),
+                        timestamp=_parse_message_datetime(row[1]),
+                        channel=channel_obj,
+                        content=row[2],
+                        attachments=row[3],
+                    )
+                except Exception as e:
+                    yield e
 
 
 def _parse_activity_blob(blob: Json) -> Activity:
     reginfo = None
     try:
         reginfo = RegionInfo(
             city=blob["city"],
@@ -126,25 +143,28 @@
         timestamp=_parse_activity_datetime(blob["timestamp"]),
         json_data_str=json.dumps(json_clean) if json_clean else None,
     )
 
 
 def parse_activity(
     events_dir: PathIsh, logger: Optional[logging.Logger] = None
-) -> Iterator[Activity]:
+) -> Iterator[Res[Activity]]:
     """
     Return useful fields from the JSON blobs
     """
     for x in parse_raw_activity(events_dir, logger):
-        if x.get('predicted_gender') is not None or x.get('predicted_age') is not None:
+        if x.get("predicted_gender") is not None or x.get("predicted_age") is not None:
             # newer (2023ish) export have a few (2-3) of these events
             # they don't have any useful info apart from some probabilites of user's gender/age
             # don't have any event_id or event_type either so we can't really parse them
             continue
-        yield _parse_activity_blob(x)
+        try:
+            yield _parse_activity_blob(x)
+        except Exception as e:
+            yield e
 
 
 def parse_raw_activity(
     events_dir: PathIsh, logger: Optional[logging.Logger] = None
 ) -> Iterator[Json]:
     """
     Return all the objects from the activity directory, as
```

### Comparing `discord_data-0.1.2/discord_data.egg-info/PKG-INFO` & `discord_data-0.2.0/discord_data.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-data
-Version: 0.1.2
+Version: 0.2.0
 Summary: Library to parse the Discord GDPR export
 Home-page: https://github.com/seanbreckenridge/discord_data
 Author: Sean Breckenridge
 Author-email: seanbrecke@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Keywords: discord data
 Classifier: License :: OSI Approved :: Apache Software License
@@ -93,8 +93,19 @@
 ```python
 # locates the corresponding `messages` directories in the folder structure
 list(merge_messages(export_dir="./discord"))`
 # supply a list of the message directories yourself
 list(merge_messages(paths=["./discord/march_2021/messages", "./discord/october_2020/messages"]))
 ```
 
+If the format for the discord export changes, the parse/merge functions will still work, they just might yield errors as part of their output. To ignore those, you can do:
+
+```python
+for msg in merge_messages(export_dir="./discord"):
+    if isinstance(msg, Exception):
+        logger.warning(msg)
+        continue
+    # do something with msg
+    print(msg.content)
+```
+
 Created to be used as part of [`HPI`](https://github.com/seanbreckenridge/HPI)
```

### Comparing `discord_data-0.1.2/setup.py` & `discord_data-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 reqs = Path("requirements.txt").read_text().strip().splitlines()
 pkg = "discord_data"
 
 
 def main() -> None:
     setup(
         name=pkg,
-        version="0.1.2",
+        version="0.2.0",
         url="https://github.com/seanbreckenridge/discord_data",
         author="Sean Breckenridge",
         author_email="seanbrecke@gmail.com",
         description=("""Library to parse the Discord GDPR export"""),
         long_description=long_description,
         long_description_content_type="text/markdown",
         license="http://www.apache.org/licenses/LICENSE-2.0",
```

