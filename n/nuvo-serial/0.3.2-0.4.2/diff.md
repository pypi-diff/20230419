# Comparing `tmp/nuvo-serial-0.3.2.tar.gz` & `tmp/nuvo-serial-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvo-serial-0.3.2.tar", max compression
+gzip compressed data, was "nuvo-serial-0.4.2.tar", max compression
```

## Comparing `nuvo-serial-0.3.2.tar` & `nuvo-serial-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2021-04-21 16:38:53.940935 nuvo-serial-0.3.2/LICENSE
--rw-r--r--   0        0        0     5162 2021-06-22 17:27:42.737100 nuvo-serial-0.3.2/README.md
--rw-r--r--   0        0        0      856 2021-04-24 20:07:22.709573 nuvo-serial-0.3.2/nuvo_serial/__init__.py
--rw-r--r--   0        0        0     1525 2021-04-21 18:58:44.308964 nuvo-serial-0.3.2/nuvo_serial/configuration.py
--rw-r--r--   0        0        0    24534 2022-09-20 21:48:26.564579 nuvo-serial-0.3.2/nuvo_serial/connection.py
--rw-r--r--   0        0        0     1092 2022-09-19 17:25:05.361827 nuvo-serial-0.3.2/nuvo_serial/const.py
--rw-r--r--   0        0        0      474 2021-04-21 15:13:53.914957 nuvo-serial-0.3.2/nuvo_serial/exceptions.py
--rw-r--r--   0        0        0    63691 2022-09-26 17:14:32.544696 nuvo-serial-0.3.2/nuvo_serial/grand_concerto_essentia_g.py
--rw-r--r--   0        0        0    21921 2022-09-19 17:25:05.361827 nuvo-serial-0.3.2/nuvo_serial/message.py
--rw-r--r--   0        0        0      417 2022-09-19 17:25:05.361827 nuvo-serial-0.3.2/nuvo_serial/nuvo_typing.py
--rw-r--r--   0        0        0      804 2023-03-21 22:56:03.364693 nuvo-serial-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 nuvo-serial-0.3.2/setup.py
--rw-r--r--   0        0        0     5992 1970-01-01 00:00:00.000000 nuvo-serial-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2021-04-21 16:38:53.940935 nuvo-serial-0.4.2/LICENSE
+-rw-r--r--   0        0        0     5162 2021-06-22 17:27:42.737100 nuvo-serial-0.4.2/README.md
+-rw-r--r--   0        0        0      856 2021-04-24 20:07:22.709573 nuvo-serial-0.4.2/nuvo_serial/__init__.py
+-rw-r--r--   0        0        0     1525 2021-04-21 18:58:44.308964 nuvo-serial-0.4.2/nuvo_serial/configuration.py
+-rw-r--r--   0        0        0    24651 2023-04-19 17:18:14.692427 nuvo-serial-0.4.2/nuvo_serial/connection.py
+-rw-r--r--   0        0        0     1126 2023-04-19 17:18:14.692427 nuvo-serial-0.4.2/nuvo_serial/const.py
+-rw-r--r--   0        0        0      474 2021-04-21 15:13:53.914957 nuvo-serial-0.4.2/nuvo_serial/exceptions.py
+-rw-r--r--   0        0        0    64120 2023-04-19 17:18:14.692427 nuvo-serial-0.4.2/nuvo_serial/grand_concerto_essentia_g.py
+-rw-r--r--   0        0        0    21921 2022-09-19 17:25:05.361827 nuvo-serial-0.4.2/nuvo_serial/message.py
+-rw-r--r--   0        0        0      417 2022-09-19 17:25:05.361827 nuvo-serial-0.4.2/nuvo_serial/nuvo_typing.py
+-rw-r--r--   0        0        0      804 2023-04-19 17:22:32.106016 nuvo-serial-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 nuvo-serial-0.4.2/setup.py
+-rw-r--r--   0        0        0     5992 1970-01-01 00:00:00.000000 nuvo-serial-0.4.2/PKG-INFO
```

### Comparing `nuvo-serial-0.3.2/LICENSE` & `nuvo-serial-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nuvo-serial-0.3.2/README.md` & `nuvo-serial-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nuvo-serial-0.3.2/nuvo_serial/__init__.py` & `nuvo-serial-0.4.2/nuvo_serial/__init__.py`

 * *Files identical despite different names*

### Comparing `nuvo-serial-0.3.2/nuvo_serial/configuration.py` & `nuvo-serial-0.4.2/nuvo_serial/configuration.py`

 * *Files identical despite different names*

### Comparing `nuvo-serial-0.3.2/nuvo_serial/connection.py` & `nuvo-serial-0.4.2/nuvo_serial/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,14 +357,17 @@
                 _LOGGER.info("RECONNECT: connection successful")
                 self._connected = True
                 self._f_connected.set_result("connected")
 
     async def send_message_without_reply(self, message: str) -> None:
         await self._send(format_message(self._model, message))
 
+    async def send_raw_bytes_message_without_reply(self, message: bytes) -> None:
+        await self._send(message)
+
     @overload
     async def send_message(
         self,
         msg: str,
         message_types: Tuple[
             Literal["ZoneButton"], Literal["ZoneStatus"], Literal["OKResponse"]
         ],
```

### Comparing `nuvo-serial-0.3.2/nuvo_serial/const.py` & `nuvo-serial-0.4.2/nuvo_serial/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,7 +32,9 @@
 RESPONSE_STRING_OK = "#OK"
 RESPONSE_STRING_ERROR = "#?"
 
 EMIT_LEVEL_ALL = "emit_all"
 EMIT_LEVEL_EXTERNAL = "emit_external"
 EMIT_LEVEL_INTERNAL = "emit_internal"
 EMIT_LEVEL_NONE = "emit_none"
+
+WAKEUP_PAUSE_SECS: Final = 0.005
```

### Comparing `nuvo-serial-0.3.2/nuvo_serial/grand_concerto_essentia_g.py` & `nuvo-serial-0.4.2/nuvo_serial/grand_concerto_essentia_g.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from nuvo_serial.const import (
     EMIT_LEVEL_ALL,
     EMIT_LEVEL_EXTERNAL,
     EMIT_LEVEL_INTERNAL,
     EMIT_LEVEL_NONE,
     ERROR_RESPONSE,
+    MODEL_ESSENTIA_G,
     ZONE_ALL_OFF,
     ZONE_STATUS,
     ZONE_EQ_STATUS,
     ZONE_CONFIGURATION,
     ZONE_VOLUME_CONFIGURATION,
     SOURCE_CONFIGURATION,
     ZONE_BUTTON,
@@ -37,14 +38,15 @@
     ZONE_BUTTON_PREV,
     ZONE_BUTTON_NEXT,
     SYSTEM_MUTE,
     SYSTEM_PAGING,
     SYSTEM_PARTY,
     SYSTEM_VERSION,
     OK_RESPONSE,
+    WAKEUP_PAUSE_SECS
 )
 from nuvo_serial.exceptions import ModelMismatchError
 from nuvo_serial.message import (
     DndMask,
     ErrorResponse,
     OKResponse,
     Mute,
@@ -683,22 +685,24 @@
         self,
         port_url: str,
         model: str,
         timeout: Optional[float] = None,
         disconnect_time: Optional[float] = None,
         do_model_check: Optional[bool] = True,
         track_state: Optional[bool] = True,
+        wakeup_essentia: Optional[bool] = True,
     ):
         self._retry_request = None
         self._port_url = port_url
         self._model = model
         self._timeout = timeout
         self._disconnect_time = disconnect_time
         self._do_model_check = do_model_check
         self._track_state = track_state
+        self._wakeup_essentia = wakeup_essentia
         _set_model_globals(self._model)
         self._bus = MsgBus()
         self._physical_zones: int = config[self._model]["zones"]["physical"]
 
     async def connect(self) -> None:
         if self._track_state:
             self._state_tracker = StateTrack(self, self._model)
@@ -758,14 +762,16 @@
         return await self._connection.send_message(
             _format_zone_status_request(zone), ZONE_STATUS, emit_level
         )
 
     @locked
     @icontract.require(lambda zone: zone in ZONE_RANGE)
     async def set_power(self, zone: int, power: bool) -> ZoneStatus:
+        if self._model == MODEL_ESSENTIA_G and self._wakeup_essentia and power:
+            await self.wakeup_essentia()
         return await self._connection.send_message(
             _format_set_power(zone, power), ZONE_STATUS
         )
 
     @locked
     @icontract.require(lambda zone: zone in ZONE_RANGE)
     async def set_mute(self, zone: int, mute: bool) -> ZoneStatus | Mute:
@@ -1169,14 +1175,18 @@
     @locked
     async def mute_all_zones(self, mute: bool) -> Mute:
         return await self._connection.send_message(
             _format_mute_all_zones(mute), SYSTEM_MUTE
 
         )
 
+    async def wakeup_essentia(self) -> None:
+        await self._connection.send_raw_bytes_message_without_reply(b"\r")
+        await asyncio.sleep(WAKEUP_PAUSE_SECS)
+
 
 class NuvoSync:
     def __init__(self, port_url: str, model: str, retries: Optional[int] = None):
         _set_model_globals(model)
         _LOGGER.info('Attempting connection - "%s"', port_url)
         self._retry_request = SyncRequest(port_url, model, retries)
```

### Comparing `nuvo-serial-0.3.2/nuvo_serial/message.py` & `nuvo-serial-0.4.2/nuvo_serial/message.py`

 * *Files identical despite different names*

### Comparing `nuvo-serial-0.3.2/pyproject.toml` & `nuvo-serial-0.4.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nuvo-serial"
-version = "0.3.2"
+version = "0.4.2"
 description = "Python API implementing the Nuvo Grand Concerto/Essentia G multi-zone audio amplifier serial control protocol"
 authors = ["sprocket-9 <sprocketnumber9@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/sprocket-9/nuvo-serial"
 repository = "https://github.com/sprocket-9/nuvo-serial"
```

### Comparing `nuvo-serial-0.3.2/setup.py` & `nuvo-serial-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['icontract>=2.4',
  'pyserial-asyncio>=0.5',
  'pyserial>=3.5',
  'typeguard>=2.10,<3.0']
 
 setup_kwargs = {
     'name': 'nuvo-serial',
-    'version': '0.3.2',
+    'version': '0.4.2',
     'description': 'Python API implementing the Nuvo Grand Concerto/Essentia G multi-zone audio amplifier serial control protocol',
     'long_description': '# nuvo-serial\nPython API implementing the Nuvo Grand Concerto/Essentia G multi-zone audio amplifier serial control protocol.\n\n\n## Notes\nA [Nuvo Integration](https://github.com/sprocket-9/hacs-nuvo-serial) built using this library, is available to control a Nuvo through a [Home Assistant](https://www.home-assistant.io/) frontend.\n\n## Usage\n\nSupported models: "Grand_Concerto" and "Essentia_G"\n\nasync and sync version of most commands.\n\nCommands return instances of a python dataclass which represents the Nuvo response message type:\n\n```\n* ZoneStatus\n* ZoneConfiguration\n* ZoneVolumeConfiguration\n* ZoneEQStatus\n* ZoneButton\n* ZoneAllOff\n* SourceConfiguration\n* Version\n```\n## Connection\nDirect serial cable or remote network connection using hardware serial-to-network adapter or software such as [ser2net](https://linux.die.net/man/8/ser2net) will\nwork, all that is needed is a change of the port_url argument:\n\nE.g:\n\nLocal: ```/dev/ttyUSB1```\n\nRemote: ```socket://host:port```\n\nA possible ser2net configuration connecting TCP port 10003 to the nuvo device on /dev/ttyUSB1:\n\n```10003:raw:0:/dev/ttyUSB1:57600 8DATABITS NONE 1STOPBIT```\n\n ```port_url="socket://192.168.5.1:10003"```\n\n## Synchronous Interface\n\nNot all the available setter methods are\nshown, but there are methods to configure most fields in each of the data classes.\n\n```python\nfrom nuvo_serial import get_nuvo\n\nnuvo = get_nuvo(port_url=\'/dev/ttyUSB0\', model=\'Grand_Concerto\')\n\nprint(nuvo.get_version()\n# Version(model=\'Grand_Concerto\', product_number=\'NV-I8G\', firmware_version=\'FWv2.66\', hardware_version=\'HWv0\')\n\nprint(nuvo.zone_status(1))\n# ZoneStatus(zone=1, power=True, source=1, volume=20, mute=False, dnd=False, lock=False)\n\nprint(nuvo.zone_configuration(1))\n# ZoneConfiguration(zone=1, enabled=True, name=\'Music Room\', slave_to=0, group=0, sources=[\'SOURCE1\'], exclusive_source=False, ir_enabled=1, dnd=[], locked=False, slave_eq=0)\n\nprint(nuvo.zone_volume_configuration(1))\n# ZoneVolumeConfiguration(zone=1, max_vol=33, ini_vol=20, page_vol=40, party_vol=50, vol_rst=False)\n\nprint(nuvo.zone_eq_status(1))\n# ZoneEQStatus(zone=1, bass=-2, treble=0, loudcmp=True, balance_position=\'C\', balance_value=0)\n\nprint(nuvo.source_configuration(2))\n# SourceConfiguration(source=2, enabled=True, name=\'Sonos\', gain=4, nuvonet_source=False, short_name=\'SON\')\n\n# Turn off zone #1\nprint(nuvo.set_power(1, False))\n# ZoneStatus(zone=1, power=False, source=None, volume=None, mute=None, dnd=None, lock=None)\n\n# Mute zone #1\nnuvo.set_mute(1, True)\n# ZoneStatus(zone=1, power=True, source=1, volume=None, mute=True, dnd=False, lock=False)\n\n# Change Zone name\nprint(nuvo.zone_set_name(1, "Kitchen"))\n# ZoneConfiguration(zone=1, enabled=True, name=\'Kitchen\', slave_to=0, group=0, sources=[\'SOURCE1\'], exclusive_source=False, ir_enabled=1, dnd=[], locked=False, slave_eq=0)\n\n# Change Zone\'s permitted sources\nprint(nuvo.zone_set_source_mask(1, [\'SOURCE3\', \'SOURCE4\']))\nZoneConfiguration(zone=1, enabled=True, name=\'Kitchen\', slave_to=0, group=0, sources=[\'SOURCE3\', \'SOURCE4\'], exclusive_source=False, ir_enabled=1, dnd=[], locked=False, slave_eq=0)\n\n# Change Zone max volume\nprint(nuvo.zone_volume_max(1, 20))\n# ZoneVolumeConfiguration(zone=1, max_vol=20, ini_vol=20, page_vol=40, party_vol=50, vol_rst=False)\n\n# Change Zone Bass\nprint(nuvo.set_bass(1, 6))\n# ZoneEQStatus(zone=1, bass=6, treble=0, loudcmp=True, balance_position=\'C\', balance_value=0)\n\n# Set volume for zone #1\nnuvo.set_volume(1, 15)\n\n# Set source 2 for zone #1 \nnuvo.set_source(1, 2)\n\n# Set balance for zone #1\nnuvo.set_balance(1, L, 8)\n# ZoneEQStatus(zone=1, bass=-2, treble=0, loudcmp=True, balance_position=\'L\', balance_value=8)\n\n```\n\n## Asynchronous Interface\n\nAll the method names and syntax are as above in the sync interface, but now all the methods are coroutines and must\nbe awaited.\n\nAn added feature with the async interface is it will constantly monitor the\nserial line and attempt to classify any messages emitted by the Nuvo.\nA subscriber to these messages in the form of a coroutine callback can optionally be added\nfor any of the Nuvo message data classes.  This allows receiving messages sent\nby the Nuvo in response to commands initiated from Zone keypads.\n\n```python\n\nimport asyncio\nfrom nuvo_serial import get_nuvo_async\n\nasync def message_receiver(message: dict):\n    print(message)\n    # e.g. {\'event_name\': \'ZoneStatus\', \'event\': ZoneStatus(zone=1, power=True, source=1, volume=None, mute=True, dnd=False, lock=False)}\n    # e.g. {\'event_name\': \'ZoneButton\', \'event\': ZoneButton(zone=1, source=1, button=\'PLAYPAUSE\')}\n\nasync def main():\n\n    nuvo = await get_nuvo_async(\'/dev/ttyUSB0\', \'Grand_Concerto\')\n\n    print(await nuvo.zone_status(1))\n    # ZoneStatus(zone=1, power=True, source=1, volume=20, mute=False, dnd=False, lock=False)\n   \n    """message_receiver coro will be called everytime a ZoneStatus message is received\n    from the Nuvo."""\n   nuvo.add_subscriber(message_receiver, "ZoneStatus")\n\n   nuvo.add_subscriber(message_receiver, "ZoneButton")\n   ...\n   nuvo.remove_subscriber(message_receiver, "ZoneStatus")\n   nuvo.disconnect()\n\n\nloop = asyncio.get_event_loop()\nloop.run_until_complete(main())\n\n```\n',
     'author': 'sprocket-9',
     'author_email': 'sprocketnumber9@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/sprocket-9/nuvo-serial',
```

### Comparing `nuvo-serial-0.3.2/PKG-INFO` & `nuvo-serial-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuvo-serial
-Version: 0.3.2
+Version: 0.4.2
 Summary: Python API implementing the Nuvo Grand Concerto/Essentia G multi-zone audio amplifier serial control protocol
 Home-page: https://github.com/sprocket-9/nuvo-serial
 License: MIT
 Author: sprocket-9
 Author-email: sprocketnumber9@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

