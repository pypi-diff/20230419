# Comparing `tmp/pyShelly-1.0.2.tar.gz` & `tmp/pyShelly-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyShelly-1.0.2.tar", last modified: Mon May  9 17:50:04 2022, max compression
+gzip compressed data, was "pyShelly-1.0.3.tar", last modified: Wed Apr 19 08:28:17 2023, max compression
```

## Comparing `pyShelly-1.0.2.tar` & `pyShelly-1.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 17:50:04.481827 pyShelly-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-05-09 17:49:50.000000 pyShelly-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-09 17:49:50.000000 pyShelly-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-05-09 17:50:04.481827 pyShelly-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-05-09 17:49:50.000000 pyShelly-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 17:50:04.481827 pyShelly-1.0.2/pyShelly/
--rwxr-xr-x   0 runner    (1001) docker     (121)    14677 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10922 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    29141 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/block.py
--rw-r--r--   0 runner    (1001) docker     (121)     6649 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     7123 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/coap.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     8954 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     4073 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     4016 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/device.py
--rw-r--r--   0 runner    (1001) docker     (121)     3710 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/dimmer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/firmware.py
--rw-r--r--   0 runner    (1001) docker     (121)    16723 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/light.py
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/loop.py
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/mdns.py
--rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7269 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/mqtt_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     7189 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/powermeter.py
--rw-r--r--   0 runner    (1001) docker     (121)     6787 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/relay.py
--rw-r--r--   0 runner    (1001) docker     (121)     3817 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/roller.py
--rw-r--r--   0 runner    (1001) docker     (121)     5105 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/sensor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4002 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/switch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/trv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3309 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3350 2022-05-09 17:49:50.000000 pyShelly-1.0.2/pyShelly/ws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 17:50:04.481827 pyShelly-1.0.2/pyShelly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-05-09 17:50:04.000000 pyShelly-1.0.2/pyShelly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-05-09 17:50:04.000000 pyShelly-1.0.2/pyShelly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-09 17:50:04.000000 pyShelly-1.0.2/pyShelly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-05-09 17:50:04.000000 pyShelly-1.0.2/pyShelly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-09 17:50:04.000000 pyShelly-1.0.2/pyShelly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-09 17:50:04.481827 pyShelly-1.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1527 2022-05-09 17:49:50.000000 pyShelly-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:28:17.306119 pyShelly-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-19 08:28:04.000000 pyShelly-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 08:28:04.000000 pyShelly-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-19 08:28:17.306119 pyShelly-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-19 08:28:04.000000 pyShelly-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:28:17.306119 pyShelly-1.0.3/pyShelly/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14677 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29437 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/coap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/mqtt_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/powermeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/roller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/trv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-19 08:28:04.000000 pyShelly-1.0.3/pyShelly/ws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:28:17.306119 pyShelly-1.0.3/pyShelly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-19 08:28:17.000000 pyShelly-1.0.3/pyShelly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-19 08:28:17.000000 pyShelly-1.0.3/pyShelly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:28:17.000000 pyShelly-1.0.3/pyShelly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-19 08:28:17.000000 pyShelly-1.0.3/pyShelly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 08:28:17.000000 pyShelly-1.0.3/pyShelly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:28:17.306119 pyShelly-1.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-04-19 08:28:04.000000 pyShelly-1.0.3/setup.py
```

### Comparing `pyShelly-1.0.2/LICENSE` & `pyShelly-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/PKG-INFO` & `pyShelly-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyShelly
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for Shelly smart home devices
 Home-page: https://github.com/StyraHem/pyShelly
 Author: StyraHem / Tarra AB
 Author-email: info@styrahem.se
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -117,9 +116,7 @@
 Please give us feedback on info@styrahem.se or Facebook groups: [Shelly grupp (Swedish)](https://www.facebook.com/groups/ShellySweden) or [Shelly support group (English)](https://www.facebook.com/groups/ShellyIoTCommunitySupport/)
 
 ## Founder
 
 This plugin is created by the StyraHem.se, the Swedish distributor of Shelly. In Sweden you can buy Shellies from [StyraHem.se](https://www.styrahem.se/c/126/shelly) or any of the retailers like NetOnNet, Kjell&Company etc.
 
 [![buy me a coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/styrahem)
-
-
```

### Comparing `pyShelly-1.0.2/README.md` & `pyShelly-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/__init__.py` & `pyShelly-1.0.3/pyShelly/__init__.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/base.py` & `pyShelly-1.0.3/pyShelly/base.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/block.py` & `pyShelly-1.0.3/pyShelly/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,16 @@
             status = json.loads(payload['data'])
             self._update_status_info(status, SRC_MQTT_STATUS)
         elif topic == "announce":
             pass
         else:
             if self.rpc:
                 data = json.loads(payload['data'])
-                data = data['params'] if 'params' in data else data['result']
+                data = data['params'] if 'params' in data else data
+                data = data['result'] if 'result' in data else data
                 self.update_rpc(data, SRC_MQTT)
             else:
                 self._update_info_values_mqtt(payload, BLOCK_INFO_VALUES)
                 for dev in self.devices:
                     dev._update_info_values_mqtt(payload)
                     if hasattr(dev, 'update_mqtt'):
                         dev.update_mqtt(payload)
@@ -431,15 +432,20 @@
         #Shelly Plus 1PM
         elif self.type == 'ShellyPlus2PM':
             self.rpc = True
             for channel in range(2):
                 self._add_device(Relay(self, channel + 1))
                 self._add_device(PowerMeter(self, channel + 1, gen=2))
                 self._add_device(Switch(self, channel + 1))
-        #Shelly 2
+        #Shelly plus Plug S
+        elif self.type == 'ShellyPlusPlugS':
+            self.rpc = True
+            self._add_device(Relay(self, 1))
+            self._add_device(PowerMeter(self, 1, gen=2))
+            #self._add_device(Switch(self, 1))
         elif self.type == 'SHSW-21':           
             self._add_device(Switch(self, 1))
             self._add_device(Switch(self, 2))
             self._add_device(PowerMeter(self, 0))
             self._need_setup_delayed_devices = True
         #Shelly 2.5
         elif self.type == 'SHSW-25':
```

### Comparing `pyShelly-1.0.2/pyShelly/cloud.py` & `pyShelly-1.0.3/pyShelly/cloud.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/coap.py` & `pyShelly-1.0.3/pyShelly/coap.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/compat.py` & `pyShelly-1.0.3/pyShelly/compat.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/const.py` & `pyShelly-1.0.3/pyShelly/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import logging
 
 LOGGER = logging.getLogger('pyShelly')
 
 NAME = "pyShelly"
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 
 COAP_IP = "224.0.1.187"
 COAP_PORT = 5683
 
 MDNS_IP = "224.0.0.251"
 MDNS_PORT = 5353
 
@@ -172,14 +172,15 @@
     'SHUNI-1': {'name': "Shelly UNI", 'mqtt':'shellyuni'},
     'SHSW-L': {'name': "Shelly 1L", 'mqtt':'shelly1l'},
     'SHMOS-01': {'name': "Shelly Motion", 'mqtt':'shellymotionsensor'},
     'ShellyPlus1': {'name':"Shelly Plus 1", 'mqtt':'shellyplus1'},
     'ShellyPlus1PM': {'name':"Shelly Plus 1PM", 'mqtt':'shellyplus1pm'},    
     'ShellyPlus2': {'name':"Shelly Plus 2", 'mqtt':'shellyplus2'},
     'ShellyPlus2PM': {'name':"Shelly Plus 2PM", 'mqtt':'shellyplus2pm'},
+    'ShellyPlusPlugS': {'name':"Shelly Plus Plug S", 'mqtt':'shellyplusplugs'},
     'ShellyPro1': {'name':"Shelly Pro 1", 'mqtt':'shellypro1'},
     'ShellyPro1PM': {'name':"Shelly Pro 1PM", 'mqtt':'shellypro1pm'},
     'ShellyPro2': {'name':"Shelly Pro 2", 'mqtt':'shellypro2'},
     'ShellyPro2PM': {'name':"Shelly Pro 2PM", 'mqtt':'shellypro2pm'},
     'ShellyPro4PM': {'name':"Shelly Pro 4PM", 'mqtt':'shellypro4pm'},
     'ShellyPlusI4': {'name':"Shelly Plus i4", 'mqtt':'shellyplusi4'},
     'SHTRV-01': {'name':"Shelly TRV", 'mqtt':'shellytrv'},
```

### Comparing `pyShelly-1.0.2/pyShelly/debug.py` & `pyShelly-1.0.3/pyShelly/debug.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/device.py` & `pyShelly-1.0.3/pyShelly/device.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/dimmer.py` & `pyShelly-1.0.3/pyShelly/dimmer.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/firmware.py` & `pyShelly-1.0.3/pyShelly/firmware.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/light.py` & `pyShelly-1.0.3/pyShelly/light.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/loop.py` & `pyShelly-1.0.3/pyShelly/loop.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/mdns.py` & `pyShelly-1.0.3/pyShelly/mdns.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/mqtt.py` & `pyShelly-1.0.3/pyShelly/mqtt.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,15 +41,28 @@
                     'name': name,
                     'topic': cmd,
                     'data': data,
                     'src':  self.src
                 }                
                 self._root.update_block(device_id, \
                     device_type, None, 'MQTT', payload, mqtt=name)
-                
+            elif topic.startswith("shelly") and "/status/" in topic:                
+                name, cmd, start = topic.rsplit('/', 2)
+                _type, device_id = name.rsplit('-', 1)
+                device_type = self._mqtt_types.get(_type)
+                data = "{\"" + start + "\":" + data + "}"
+                payload = {
+                    'type': 'mqtt',
+                    'name': name,
+                    'topic': cmd,
+                    'data': data,
+                    'src':  self.src
+                }                
+                self._root.update_block(device_id, \
+                    device_type, None, 'MQTT', payload, mqtt=name)               
             elif topic.startswith("shellies/shelly"):
                 _, name, cmd = topic.split('/', 2)
                 if name == 'announce':
                     return
                 if cmd == 'command':
                     return; 
                 _type, device_id = name.rsplit('-', 1)
```

### Comparing `pyShelly-1.0.2/pyShelly/mqtt_client.py` & `pyShelly-1.0.3/pyShelly/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/mqtt_server.py` & `pyShelly-1.0.3/pyShelly/mqtt_server.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/powermeter.py` & `pyShelly-1.0.3/pyShelly/powermeter.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/relay.py` & `pyShelly-1.0.3/pyShelly/relay.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/roller.py` & `pyShelly-1.0.3/pyShelly/roller.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/sensor.py` & `pyShelly-1.0.3/pyShelly/sensor.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/switch.py` & `pyShelly-1.0.3/pyShelly/switch.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/trv.py` & `pyShelly-1.0.3/pyShelly/trv.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/utils.py` & `pyShelly-1.0.3/pyShelly/utils.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly/ws_client.py` & `pyShelly-1.0.3/pyShelly/ws_client.py`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/pyShelly.egg-info/PKG-INFO` & `pyShelly-1.0.3/pyShelly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyShelly
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for Shelly smart home devices
 Home-page: https://github.com/StyraHem/pyShelly
 Author: StyraHem / Tarra AB
 Author-email: info@styrahem.se
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -117,9 +116,7 @@
 Please give us feedback on info@styrahem.se or Facebook groups: [Shelly grupp (Swedish)](https://www.facebook.com/groups/ShellySweden) or [Shelly support group (English)](https://www.facebook.com/groups/ShellyIoTCommunitySupport/)
 
 ## Founder
 
 This plugin is created by the StyraHem.se, the Swedish distributor of Shelly. In Sweden you can buy Shellies from [StyraHem.se](https://www.styrahem.se/c/126/shelly) or any of the retailers like NetOnNet, Kjell&Company etc.
 
 [![buy me a coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/styrahem)
-
-
```

### Comparing `pyShelly-1.0.2/pyShelly.egg-info/SOURCES.txt` & `pyShelly-1.0.3/pyShelly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyShelly-1.0.2/setup.py` & `pyShelly-1.0.3/setup.py`

 * *Files identical despite different names*

