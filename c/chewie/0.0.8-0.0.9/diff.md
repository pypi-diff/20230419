# Comparing `tmp/chewie-0.0.8.tar.gz` & `tmp/chewie-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chewie-0.0.8.tar", last modified: Mon Sep 17 02:55:23 2018, max compression
+gzip compressed data, was "dist/chewie-0.0.9.tar", last modified: Mon Oct  8 01:20:44 2018, max compression
```

## Comparing `chewie-0.0.8.tar` & `chewie-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-17 02:55:23.000000 chewie-0.0.8/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-17 02:55:23.000000 chewie-0.0.8/chewie/
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-09-17 02:53:55.000000 chewie-0.0.8/chewie/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1379 2018-09-17 02:53:55.000000 chewie-0.0.8/chewie/auth_8021x.py
--rw-r--r--   0 travis    (2000) travis    (2000)    13716 2018-09-17 02:53:55.000000 chewie-0.0.8/chewie/chewie.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5763 2018-09-17 02:53:55.000000 chewie-0.0.8/chewie/eap.py
--rw-r--r--   0 travis    (2000) travis    (2000)    32301 2018-09-17 02:53:55.000000 chewie-0.0.8/chewie/eap_state_machine.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1287 2018-09-17 02:53:55.000000 chewie-0.0.8/chewie/ethernet_packet.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2025 2018-09-17 02:53:55.000000 chewie-0.0.8/chewie/event.py
--rw-r--r--   0 travis    (2000) travis    (2000)      899 2018-09-17 02:53:55.000000 chewie-0.0.8/chewie/mac_address.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9130 2018-09-17 02:53:55.000000 chewie-0.0.8/chewie/message_parser.py
--rw-r--r--   0 travis    (2000) travis    (2000)    11943 2018-09-17 02:53:55.000000 chewie-0.0.8/chewie/radius.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4638 2018-09-17 02:53:55.000000 chewie-0.0.8/chewie/radius_attributes.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7898 2018-09-17 02:53:55.000000 chewie-0.0.8/chewie/radius_datatypes.py
--rw-r--r--   0 travis    (2000) travis    (2000)      357 2018-09-17 02:53:55.000000 chewie-0.0.8/chewie/utils.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-17 02:55:23.000000 chewie-0.0.8/chewie.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)      806 2018-09-17 02:55:23.000000 chewie-0.0.8/chewie.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      603 2018-09-17 02:55:23.000000 chewie-0.0.8/chewie.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-09-17 02:55:23.000000 chewie-0.0.8/chewie.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       23 2018-09-17 02:55:23.000000 chewie-0.0.8/chewie.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        7 2018-09-17 02:55:23.000000 chewie-0.0.8/chewie.egg-info/top_level.txt
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-17 02:55:23.000000 chewie-0.0.8/test/
--rw-r--r--   0 travis    (2000) travis    (2000)      789 2018-09-17 02:53:55.000000 chewie-0.0.8/test/test_auth_8021x.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2106 2018-09-17 02:53:55.000000 chewie-0.0.8/test/test_eap.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1313 2018-09-17 02:53:55.000000 chewie-0.0.8/test/test_ethernet_packet.py
--rw-r--r--   0 travis    (2000) travis    (2000)    18256 2018-09-17 02:53:55.000000 chewie-0.0.8/test/test_full_state_machine.py
--rw-r--r--   0 travis    (2000) travis    (2000)    13791 2018-09-17 02:53:55.000000 chewie-0.0.8/test/test_message_parser.py
--rw-r--r--   0 travis    (2000) travis    (2000)    33799 2018-09-17 02:53:55.000000 chewie-0.0.8/test/test_radius.py
--rw-r--r--   0 travis    (2000) travis    (2000)      642 2018-09-17 02:53:55.000000 chewie-0.0.8/README.md
--rw-r--r--   0 travis    (2000) travis    (2000)      102 2018-09-17 02:55:23.000000 chewie-0.0.8/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)      979 2018-09-17 02:53:55.000000 chewie-0.0.8/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)      806 2018-09-17 02:55:23.000000 chewie-0.0.8/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-08 01:20:44.000000 chewie-0.0.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      642 2018-10-08 01:18:44.000000 chewie-0.0.9/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      979 2018-10-08 01:18:44.000000 chewie-0.0.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-08 01:20:44.000000 chewie-0.0.9/chewie/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34578 2018-10-08 01:18:44.000000 chewie-0.0.9/chewie/eap_state_machine.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12087 2018-10-08 01:18:44.000000 chewie-0.0.9/chewie/radius.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7898 2018-10-08 01:18:44.000000 chewie-0.0.9/chewie/radius_datatypes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1379 2018-10-08 01:18:44.000000 chewie-0.0.9/chewie/auth_8021x.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-10-08 01:18:44.000000 chewie-0.0.9/chewie/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1287 2018-10-08 01:18:44.000000 chewie-0.0.9/chewie/ethernet_packet.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9130 2018-10-08 01:18:44.000000 chewie-0.0.9/chewie/message_parser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2432 2018-10-08 01:18:44.000000 chewie-0.0.9/chewie/timer_scheduler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5763 2018-10-08 01:18:44.000000 chewie-0.0.9/chewie/eap.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2392 2018-10-08 01:18:44.000000 chewie-0.0.9/chewie/event.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      357 2018-10-08 01:18:44.000000 chewie-0.0.9/chewie/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1199 2018-10-08 01:18:44.000000 chewie-0.0.9/chewie/mac_address.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4847 2018-10-08 01:18:44.000000 chewie-0.0.9/chewie/radius_attributes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14536 2018-10-08 01:18:44.000000 chewie-0.0.9/chewie/chewie.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-08 01:20:44.000000 chewie-0.0.9/chewie.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2018-10-08 01:20:43.000000 chewie-0.0.9/chewie.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       23 2018-10-08 01:20:43.000000 chewie-0.0.9/chewie.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      806 2018-10-08 01:20:43.000000 chewie-0.0.9/chewie.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-10-08 01:20:43.000000 chewie-0.0.9/chewie.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      674 2018-10-08 01:20:43.000000 chewie-0.0.9/chewie.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2018-10-08 01:20:44.000000 chewie-0.0.9/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-08 01:20:44.000000 chewie-0.0.9/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1948 2018-10-08 01:18:44.000000 chewie-0.0.9/test/test_mac_address.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22354 2018-10-08 01:18:44.000000 chewie-0.0.9/test/test_full_state_machine.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      789 2018-10-08 01:18:44.000000 chewie-0.0.9/test/test_auth_8021x.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13920 2018-10-08 01:18:44.000000 chewie-0.0.9/test/test_chewie.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1313 2018-10-08 01:18:44.000000 chewie-0.0.9/test/test_ethernet_packet.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33799 2018-10-08 01:18:44.000000 chewie-0.0.9/test/test_radius.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13791 2018-10-08 01:18:44.000000 chewie-0.0.9/test/test_message_parser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2106 2018-10-08 01:18:44.000000 chewie-0.0.9/test/test_eap.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      806 2018-10-08 01:20:44.000000 chewie-0.0.9/PKG-INFO
```

### Comparing `chewie-0.0.8/chewie/auth_8021x.py` & `chewie-0.0.9/chewie/auth_8021x.py`

 * *Files identical despite different names*

### Comparing `chewie-0.0.8/chewie/chewie.py` & `chewie-0.0.9/chewie/chewie.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 """Entry point for 802.1X speaker.
 """
 from fcntl import ioctl
-import os
-import sched
 import struct
-import time
-
+import os
+from chewie import timer_scheduler
 from eventlet import sleep, GreenPool
 from eventlet.green import socket
 from eventlet.queue import Queue
 
-
 from chewie.eap_state_machine import FullEAPStateMachine
 from chewie.radius_attributes import EAPMessage, State, CalledStationId, NASPortType
 from chewie.message_parser import MessageParser, MessagePacker
 from chewie.mac_address import MacAddress
-from chewie.event import EventMessageReceived, EventRadiusMessageReceived
+from chewie.event import EventMessageReceived, EventRadiusMessageReceived, EventPortStatusChange
 from chewie.utils import get_logger
 
 
 def unpack_byte_string(byte_string):
     """unpacks a byte string"""
     return "".join("%02x" % x for x in byte_string)
 
@@ -62,193 +59,207 @@
         self.state_machines = {}  # mac: sm
         self.packet_id_to_mac = {}  # radius_packet_id: mac
         self.packet_id_to_request_authenticator = {}
 
         self.eap_output_messages = Queue()
         self.radius_output_messages = Queue()
 
-        self.timer_scheduler = sched.scheduler(time.time, sleep)
+        self.timer_scheduler = timer_scheduler.TimerScheduler(self.logger)
 
         self.radius_id = -1
         self.socket = None
         self.pool = None
         self.eventlets = None
         self.radius_socket = None
         self.interface_index = None
         self.interface_address = None
 
+        self.eventlets = []
+
     def run(self):
         """setup chewie and start socket eventlet threads"""
         self.logger.info("Starting")
         self.open_socket()
         self.open_radius_socket()
         self.get_interface_info()
         self.join_multicast_group()
         self.start_threads_and_wait()
 
     def start_threads_and_wait(self):
         """Start the thread and wait until they complete (hopefully never)"""
         self.pool = GreenPool()
-        self.eventlets = []
 
         self.eventlets.append(self.pool.spawn(self.send_eap_messages))
         self.eventlets.append(self.pool.spawn(self.receive_eap_messages))
 
         self.eventlets.append(self.pool.spawn(self.send_radius_messages))
         self.eventlets.append(self.pool.spawn(self.receive_radius_messages))
 
-        self.eventlets.append(self.pool.spawn(self.timer_messages))
+        self.eventlets.append(self.pool.spawn(self.timer_scheduler.run))
 
         self.pool.waitall()
 
     def auth_success(self, src_mac, port_id):
         """authentication shim between faucet and chewie
         Args:
             src_mac (MacAddress): the mac of the successful supplicant
             port_id (MacAddress): the 'mac' identifier of what switch port the success is on"""
         if self.auth_handler:
             self.auth_handler(src_mac, port_id)
 
     def auth_failure(self, src_mac, port_id):
         """failure shim between faucet and chewie
-                Args:
-                    src_mac (MacAddress): the mac of the failed supplicant
-                    port_id (MacAddress): the 'mac' identifier of what switch port
-                     the failure is on"""
+        Args:
+            src_mac (MacAddress): the mac of the failed supplicant
+            port_id (MacAddress): the 'mac' identifier of what switch port
+             the failure is on"""
         if self.failure_handler:
             self.failure_handler(src_mac, port_id)
 
     def auth_logoff(self, src_mac, port_id):
         """logoff shim between faucet and chewie
-                Args:
-                    src_mac (MacAddress): the mac of the logoff supplicant
-                    port_id (MacAddress): the 'mac' identifier of what switch port
-                     the logoff is on"""
+        Args:
+            src_mac (MacAddress): the mac of the logoff supplicant
+            port_id (MacAddress): the 'mac' identifier of what switch port
+             the logoff is on"""
         if self.logoff_handler:
             self.logoff_handler(src_mac, port_id)
 
+    def port_down(self, port_id):
+        """
+        should be called by faucet when port has gone down.
+        Args:
+            port_id (str): id of port.
+        """
+        # all chewie needs to do is change its internal state.
+        # faucet will remove the acls by itself.
+        self.set_port_status(port_id, False)
+
+    def port_up(self, port_id):
+        """
+        should be called by faucet when port has come up
+        Args:
+            port_id (str): id of port.
+        """
+        self.set_port_status(port_id, True)
+        # TODO send preemptive identity request.
+
+    def set_port_status(self, port_id, status):
+        port_id_str = str(port_id)
+        if port_id_str not in self.state_machines:
+            self.state_machines[port_id_str] = {}
+
+        for src_mac, sm in self.state_machines[port_id_str].items():
+            event = EventPortStatusChange(status)
+            sm.event(event)
+
     def send_eap_messages(self):
         """send eap messages to supplicant forever."""
-        try:
-            while True:
+        while True:
+            try:
                 sleep(0)
                 message, src_mac, port_mac = self.eap_output_messages.get()
                 self.logger.info("Sending message %s from %s to %s" %
                                  (message, str(port_mac), str(src_mac)))
                 self.eap_send(MessagePacker.ethernet_pack(message, port_mac, src_mac))
-        except Exception as e:
-            self.logger.exception(e)
+            except Exception as e:
+                self.logger.exception(e)
 
     def eap_send(self, data):
         """send on eap socket.
             data (bytes): data to send"""
         self.socket.send(data)
 
     def receive_eap_messages(self):
         """receive eap messages from supplicant forever."""
-        try:
-            while True:
+        while True:
+            try:
                 sleep(0)
                 self.logger.info("waiting for eap.")
                 packed_message = self.eap_receive()
                 self.logger.info("Received packed_message: %s", str(packed_message))
 
                 message, dst_mac = MessageParser.ethernet_parse(packed_message)
                 self.logger.info("eap EAP(): %s", message)
                 self.logger.info("Received message: %s" % message.__dict__)
-                sm = self.get_state_machine(message.src_mac)
+                sm = self.get_state_machine(message.src_mac, dst_mac)
                 event = EventMessageReceived(message, dst_mac)
                 sm.event(event)
-        except Exception as e:
-            self.logger.exception(e)
+            except Exception as e:
+                self.logger.exception(e)
 
     def eap_receive(self):
         """receive from eap socket"""
         return self.socket.recv(4096)
 
     def send_radius_messages(self):
         """send RADIUS messages to RADIUS Server forever."""
-
-        try:
-            while True:
+        while True:
+            try:
                 sleep(0)
-                eap_message, src_mac, username, state = self.radius_output_messages.get()
+                eap_message, src_mac, username, state, port_id = self.radius_output_messages.get()
                 self.logger.info("got eap to send to radius.. mac: %s %s, username: %s",
                                  type(src_mac), src_mac, username)
                 state_dict = None
                 if state:
                     state_dict = state.__dict__
                 self.logger.info("Sending to RADIUS eap message %s with state %s",
                                  eap_message.__dict__, state_dict)
                 radius_packet_id = self.get_next_radius_packet_id()
-                self.packet_id_to_mac[radius_packet_id] = src_mac
+                self.packet_id_to_mac[radius_packet_id] = {'src_mac': src_mac, 'port_id': port_id}
                 # message is eap. needs to be wrapped into a radius packet.
                 request_authenticator = os.urandom(16)
                 self.packet_id_to_request_authenticator[radius_packet_id] = request_authenticator
                 data = MessagePacker.radius_pack(eap_message, src_mac, username,
                                                  radius_packet_id, request_authenticator, state,
                                                  self.radius_secret,
                                                  self.extra_radius_request_attributes)
                 self.radius_send(data)
                 self.logger.info("sent radius message.")
-        except Exception as e:
-            self.logger.exception(e)
+            except Exception as e:
+                self.logger.exception(e)
 
     def radius_send(self, data):
         """Sends on the radius socket
             data (bytes): what to send"""
         self.radius_socket.sendto(data, (self.radius_server_ip, self.radius_server_port))
 
     def receive_radius_messages(self):
         """receive RADIUS messages from RADIUS server forever."""
-
-        try:
-            while True:
+        while True:
+            try:
                 sleep(0)
                 self.logger.info("waiting for radius.")
                 packed_message = self.radius_receive()
                 radius = MessageParser.radius_parse(packed_message, self.radius_secret,
                                                     self.request_authenticator_callback)
                 self.logger.info("Received RADIUS message: %s", radius)
                 eap_msg = radius.attributes.find(EAPMessage.DESCRIPTION)
                 sm = self.get_state_machine_from_radius_packet_id(radius.packet_id)
                 eap_msg = eap_msg.data_type.data()
                 state = radius.attributes.find(State.DESCRIPTION)
                 self.logger.info("radius EAP: %s", eap_msg)
-                event = EventRadiusMessageReceived(eap_msg, state)
+                event = EventRadiusMessageReceived(eap_msg, state, radius.attributes.to_dict())
                 sm.event(event)
-        except Exception as e:
-            self.logger.exception(e)
+            except Exception as e:
+                self.logger.exception(e)
 
     def radius_receive(self):
         """Receives from the radius socket"""
         return self.radius_socket.recv(4096)
 
     def request_authenticator_callback(self, packet_id):
         """Callback to get the RADIUS request Authenticator
         Args:
             packet_id (int):
         Returns:
             the request authenticator sent with the packet_id
             """
         return self.packet_id_to_request_authenticator[packet_id]
 
-    def timer_messages(self):
-        """Process timer based events forever."""
-        def scheduler_done():
-            self.logger.info("scheduler has processed it's last job.")
-        try:
-            while True:
-                # TODO how else could this be made to never end?
-                self.timer_scheduler.enter(999999, 99, scheduler_done)
-                self.timer_scheduler.run()
-                self.logger.info("scheduler completed")
-        except Exception as e:
-            self.logger.exception(e)
-
     def open_radius_socket(self):
         """Setup RADIUS Socket"""
         self.radius_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)  # pylint: disable=no-member
         self.logger.info("Radius Listening on %s:%d" % (self.radius_listen_ip,
                                                         self.radius_listen_port))
         self.radius_socket.bind((self.radius_listen_ip, self.radius_listen_port))
 
@@ -292,33 +303,39 @@
     def get_state_machine_from_radius_packet_id(self, packet_id):
         """Gets a FullEAPStateMachine from the RADIUS message packet_id
         Args:
             packet_id (int): id of the received RADIUS message
         Returns:
             FullEAPStateMachine
         """
-        return self.get_state_machine(self.packet_id_to_mac[packet_id])
+        return self.get_state_machine(**self.packet_id_to_mac[packet_id])
 
-    def get_state_machine(self, src_mac):
+    def get_state_machine(self, src_mac, port_id):
         """Gets or creates if it does not already exist an FullEAPStateMachine for the src_mac.
         Args:
-            src_mac (MACAddress): who's to get.
+            src_mac (MacAddress): who's to get.
+            port_id (MacAddress): ID of the port where the src_mac is.
 
         Returns:
             FullEAPStateMachine
         """
-        sm = self.state_machines.get(src_mac, None)
+        port_id_str = str(port_id)
+        src_mac_str = str(src_mac)
+        port_sms = self.state_machines.get(port_id_str, None)
+        if port_sms is None:
+            self.state_machines[port_id_str] = {}
+        sm = self.state_machines[port_id_str].get(src_mac_str, None)
         if not sm:
             sm = FullEAPStateMachine(self.eap_output_messages, self.radius_output_messages, src_mac,
                                      self.timer_scheduler, self.auth_success,
                                      self.auth_failure, self.auth_logoff, self.logger.name)
             sm.eapRestart = True
             # TODO what if port is not actually enabled, but then how did they auth?
             sm.portEnabled = True
-            self.state_machines[src_mac] = sm
+            self.state_machines[port_id_str][src_mac_str] = sm
         return sm
 
     def get_next_radius_packet_id(self):
         """Calulate the next RADIUS Packet ID
         Returns:
             int
         """
```

### Comparing `chewie-0.0.8/chewie/eap.py` & `chewie-0.0.9/chewie/eap.py`

 * *Files identical despite different names*

### Comparing `chewie-0.0.8/chewie/eap_state_machine.py` & `chewie-0.0.9/chewie/eap_state_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Loosely based on RFC4137 'EAP State Machines' with some interpretation"""
 import random
 
 from chewie.eap import Eap
 from chewie.event import EventMessageReceived, EventRadiusMessageReceived, EventTimerExpired, \
-    EventPortStatusChange
+    EventPortStatusChange, EventSessionTimeout
 from chewie.message_parser import SuccessMessage, FailureMessage, EapolStartMessage, \
     IdentityMessage, EapolLogoffMessage
+from chewie.radius_attributes import SessionTimeout
 from chewie.utils import get_logger, log_method
 
 
 class Policy:
     """Fleshed out enough to support passthrough mode."""
 
     @staticmethod
     def getNextMethod(eapRespData):  # pylint: disable=invalid-name
         # TODO Probably should do something else
         if isinstance(eapRespData, EapolStartMessage):
             return "IDENTITY"
-        return "NOTIFICATION"
+        return "IDENTITY"
+        # return "NOTIFICATION"
 
     @staticmethod
     def getDecision(eapRespData):  # pylint: disable=invalid-name
         # TODO if not offloading return success/failure/Continue
         if eapRespData is None or isinstance(eapRespData, EapolStartMessage):
             return Decision.CONTINUE
         return Decision.PASSTHROUGH
@@ -94,23 +96,27 @@
 
 class FullEAPStateMachine:
     """Based on RFC 4137 section 7 (EAP Full Authenticator).
     Only acts in passthrough mode (no local method support).
     """
 
     # non RFC 4137 variables/CONSTANTs
+    DEFAULT_TIMEOUT = 5  # Number of Seconds
+    DEFAULT_SESSION_TIMEOUT = 3600  # Number of Seconds
+
     currentState = None
     eap_output_messages = None
     src_mac = None
     # TODO can use dst_mac to verify where packet came rom more thoughly
     port_id_mac = None
     radius_state_attribute = None  # the last state from radius server
     sent_count = 0
+    session_timeout_job = None
 
-    DEFAULT_TIMEOUT = 5  # Number of Seconds
+    session_timeout = DEFAULT_SESSION_TIMEOUT
 
     NO_STATE = "NO_STATE"
     DISABLED = "DISABLED"
     INITIALIZE = "INITIALIZE"
     IDLE = "IDLE"
     RECEIVED = "RECEIVED"
     INTEGRITY_CHECK = "INTEGRITY_CHECK"
@@ -514,15 +520,15 @@
                 # Do nothing.
                 pass
 
             if self.currentState == FullEAPStateMachine.SUCCESS:
                 # RFC 4137 says do nothing from success(2), but we're adding a logoff state.
                 # hopefully it will work as intended.
                 # Otherwise allow transition to logoff from all states.
-                if self.eapLogoff:
+                if self.logoff:
                     self.logoff_state()
                     self.currentState = FullEAPStateMachine.LOGOFF
 
             if self.currentState == FullEAPStateMachine.TIMEOUT_FAILURE:
                 # Do nothing.
                 pass
 
@@ -671,70 +677,109 @@
                     self.logoff2_state()
                     self.currentState = FullEAPStateMachine.LOGOFF2
 
             if self.currentState == FullEAPStateMachine.TIMEOUT_FAILURE2:
                 # Do nothing.
                 pass
 
+    def lower_layer_reset(self):
+        """Sets variables that are meant to be set by the lower layer
+        RFC4137 5.1.2 (standalone authenticator to Lower Layer)"""
+        self.eapReq = False
+        self.eapNoReq = False
+        self.eapSuccess = False
+        self.eapFail = False
+        self.eapTimeout = False
+
+        self.logoff = False
+
+        self.aaaEapResp = False
+
     def event(self, event):
         """Processes an event.
         Output is via the eap/radius queue. and again will be of type ***Message.
         Args:
             event: should have message attribute which is of the ***Message types
             (e.g. SuccessMessage, IdentityMessage,...)
         """
-
-        self.logger.info("full state machine received event")
+        self.lower_layer_reset()
+        self.logger.info("full state machine received event: %s", event)
         # 'Lower Layer' shim
         if isinstance(event, EventMessageReceived):
             self.message_event_received(event)
 
         elif isinstance(event, EventTimerExpired):
             if self.timer_expired_event_received(event):
                 return
 
         elif isinstance(event, EventPortStatusChange):
             self.port_status_event_received(event)
+        elif isinstance(event, EventSessionTimeout):
+            self.session_timeout_event_received()
 
         self.handle_message_received()
         self.logger.info('end state: %s', self.currentState)
 
         if self.eapReq:
             if (hasattr(self.eapReqData, 'code') and self.eapReqData.code == Eap.REQUEST) \
                     or isinstance(self.eapReqData, (SuccessMessage, FailureMessage)):
+                self.logger.info('outputting eap, %s %s %s', self.eapReqData, self.src_mac, self.port_id_mac)
                 self.eap_output_messages.put((self.eapReqData, self.src_mac, self.port_id_mac))
                 self.sent_count += 1
                 self.set_timer()
             else:
                 self.logger.error('cant find code --- %s', self.eapReqData)
             self.eapReq = False
 
         if self.aaaEapResp and self.aaaEapRespData:
             if self.aaaEapRespData.code == Eap.RESPONSE:
+                self.logger.info('outputing radius')
                 self.radius_output_messages.put((self.aaaEapRespData, self.src_mac,
                                                  self.aaaIdentity.identity,
-                                                 self.radius_state_attribute))
+                                                 self.radius_state_attribute,
+                                                 self.port_id_mac))
                 self.sent_count += 1
                 self.set_timer()
             self.aaaEapResp = False
         elif self.aaaEapResp:
             self.logger.error("aaaEapResp is true. but data is false. This should never happen")
 
         if self.eapSuccess:
-            self.logger.info('Yay authentication successful %s %s',
-                             self.src_mac, self.aaaIdentity.identity)
-            self.auth_handler(self.src_mac, str(self.port_id_mac))
+            self.handle_success()
 
         if self.eapFail:
             self.logger.info('oh authentication not successful %s', self.src_mac)
             self.failure_handler(self.src_mac, str(self.port_id_mac))
 
         if self.eapLogoff:
-            self.logger.info('client is logging off %s', self.src_mac)
-            self.logoff_handler(self.src_mac, str(self.port_id_mac))
+            self.handle_logoff()
+
+    def handle_logoff(self):
+        """Notify the logoff callback"""
+        self.logger.info('client is logging off %s', self.src_mac)
+        self.logoff_handler(self.src_mac, str(self.port_id_mac))
+        if self.session_timeout_job:
+            self.session_timeout_job.cancel()
+
+    def handle_success(self):
+        """Notify the success callback and sets a timer event to expire this session"""
+        self.logger.info('Yay authentication successful %s %s',
+                         self.src_mac, self.aaaIdentity.identity)
+        self.auth_handler(self.src_mac, str(self.port_id_mac))
+        # new authentication so cancel the old session timeout event
+        if self.session_timeout_job:
+            self.session_timeout_job.cancel()
+
+        self.session_timeout_job = self.timer_scheduler.call_later(self.session_timeout,
+                                                                   self.event,
+                                                                   EventSessionTimeout(self))
+
+    def session_timeout_event_received(self):
+        """process session timeout event"""
+        self.logoff = True
 
     def port_status_event_received(self, event):
         """Sets variables for the port status change (link up/down) being received.
         Args:
             event (EventPortStatusChange):
         """
         self.portEnabled = event.port_status  # pylint: disable=invalid-name
@@ -765,55 +810,64 @@
         """Sets variables for the Eap message being received.
         Args:
             event (EventMessageReceived): event being processed.
         """
         self.logger.info('type: %s, message %s ', type(event.message), event.message)
         if event.port_id:
             self.port_id_mac = event.port_id
-        self.logoff = False
+
         if isinstance(event.message, EapolStartMessage):
             self.eapRestart = True
         elif isinstance(event.message, EapolLogoffMessage):
             self.logoff = True
-        if not isinstance(event, EventRadiusMessageReceived):
-            self.eapRespData = event.message  # pylint: disable=invalid-name
-            self.eapResp = True
-        else:
-            self.eapRespData = None
-            self.eapResp = False
-        self.eapReq = False
-        self.eapNoReq = False
-        self.eapSuccess = False
-        self.eapFail = False
-        self.aaaEapNoReq = False
-        self.aaaSuccess = False
-        self.aaaFail = False
-        self.aaaEapKeyAvailable = False  # pylint: disable=invalid-name
-        self.aaaEapResp = False
-        self.eapLogoff = False
+
         if isinstance(event, EventRadiusMessageReceived):
-            self.radius_state_attribute = event.state
-            self.aaaEapReq = True
-            self.aaaEapReqData = event.message  # pylint: disable=invalid-name
-            self.logger.info('sm ev.msg: %s', self.aaaEapReqData)
-            if isinstance(self.aaaEapReqData, SuccessMessage):
-                self.logger.info("aaaSuccess")
-                self.aaaSuccess = True
-            if isinstance(self.aaaEapReqData, FailureMessage):
-                self.logger.info("aaaFail")
-                self.aaaFail = True
+            self.process_radius_message(event)
         else:
-            self.aaaEapReq = False
+            self.eapRespData = event.message  # pylint: disable=invalid-name
+            self.eapResp = True
+
+    def process_radius_message(self, event):
+        """Process radius message (set and extract radius specific variables)"""
+        self.eapRespData = None
+        self.eapResp = False
+        self.logger.info('radius attributes %s', event.attributes)
+        self.radius_state_attribute = event.state
+        self.aaaEapReq = True
+        self.aaaEapReqData = event.message  # pylint: disable=invalid-name
+        self.logger.info('sm ev.msg: %s', self.aaaEapReqData)
+        if isinstance(self.aaaEapReqData, SuccessMessage):
+            self.logger.info("aaaSuccess")
+            self.aaaSuccess = True
+        if isinstance(self.aaaEapReqData, FailureMessage):
+            self.logger.info("aaaFail")
+            self.aaaFail = True
+        self.logger.info('radius event %s', event.__dict__)
+        self.set_vars_from_radius(event.attributes)
+
+    def set_vars_from_radius(self, attributes):
+        """
+        Set the statemachine variables from attributes received in the radius message.
+        If variable does not exist in the radius message, it is reset to the default
+        Args:
+            attributes (dict):  attributes to be set.
+        """
+        self.session_timeout = self.DEFAULT_SESSION_TIMEOUT
+
+        if attributes:
+            self.session_timeout = attributes.get(SessionTimeout.DESCRIPTION,
+                                                  self.DEFAULT_SESSION_TIMEOUT)
+        # TODO could also set filter-id/vlans/acls here.
 
     def set_timer(self):
         """Sets a timer to trigger a retransmit if no packet received.
         """
         # These messages should not expect a reply, so set the timer.
         if self.currentState not in [self.SUCCESS, self.SUCCESS2,
                                      self.FAILURE, self.FAILURE2,
                                      self.TIMEOUT_FAILURE, self.TIMEOUT_FAILURE2]:
             timeout = self.retransWhile
-            self.timer_scheduler.enter(timeout, 10,
-                                       self.event,
-                                       argument=[EventTimerExpired(self, self.sent_count)])
+            self.timer_scheduler.call_later(timeout,
+                                            self.event,
+                                            EventTimerExpired(self, self.sent_count))
             # TODO could cancel the scheduled events when
             # they're no longer needed (i.e. response received)
```

### Comparing `chewie-0.0.8/chewie/ethernet_packet.py` & `chewie-0.0.9/chewie/ethernet_packet.py`

 * *Files identical despite different names*

### Comparing `chewie-0.0.8/chewie/event.py` & `chewie-0.0.9/chewie/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,25 @@
         """
         # will work but please do this properly
         self.type = self.TIMER_EXPIRED
         self.state_machine = state_machine
         self.sent_count = sent_count
 
 
+class EventSessionTimeout(Event):
+    """User's session should be terminated."""
+    def __init__(self, state_machine=None):
+        """
+        Args:
+            state_machine: state machine that triggered the event
+        """
+        self.type = self.TIMER_EXPIRED
+        self.state_machine = state_machine
+
+
 class EventMessageReceived(Event):
     """Message (EAP) Received. Radius Message event is a child"""
     def __init__(self, message, port_id):
         """
         Args:
             message:
             port_id: id of switch port where message was received.
@@ -54,22 +65,23 @@
         else:
             self.type = self.PORT_DISABLED
 
 
 class EventRadiusMessageReceived(EventMessageReceived):
     """Radius Message Received."""
 
-    def __init__(self, message, state):
+    def __init__(self, message, state, attributes=None):
         """
         Args:
             message:
             state: the RADIUS state attribute
         """
         super().__init__(message, None)
         self.state = state
+        self.attributes = attributes
 
 
 class EventShutdown(Event):
     """Shutdown has been signaled (is this even used?)"""
     def __init__(self):
         # will work but please do this properly
         self.type = self.SHUTDOWN
```

### Comparing `chewie-0.0.8/chewie/mac_address.py` & `chewie-0.0.9/chewie/mac_address.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 """MAC address helper"""
-from netils import build_byte_string
+
+import re
+
+# pylint: disable=too-few-public-methods
+
+
+_MAC_REGEX = re.compile(r'(?:[0-9a-f]{1,2}:){5}[0-9a-f]{1,2}\Z', re.IGNORECASE)
 
 
 class MacAddress:
     """Class for comparing mac addresses"""
     def __init__(self, address):
         self.address = address
 
     @classmethod
     def from_string(cls, address_string):
-        """Create a MacAddress from a string
+        """Create a MacAddress from a string.
+
         Args:
-            address_string (str):
+            address_string (str): Colon-delimited MAC address.
+
         Returns:
             MacAddress
-        """
-        address_bytes = "".join(address_string.split(":"))
-        address = build_byte_string(address_bytes)
 
+        Raises:
+            ValueError: If address_string is invalid.
+        """
+        if not _MAC_REGEX.match(address_string):
+            raise ValueError("'%s' does not appear to be a MAC address" % address_string)
+        address = bytes(int(x, 16) for x in address_string.split(':'))
         return cls(address)
 
     def __str__(self):
         address_string = ":".join("%02x" % x for x in self.address)
         return address_string
 
     def __eq__(self, other):
```

### Comparing `chewie-0.0.8/chewie/message_parser.py` & `chewie-0.0.9/chewie/message_parser.py`

 * *Files identical despite different names*

### Comparing `chewie-0.0.8/chewie/radius.py` & `chewie-0.0.9/chewie/radius.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
 
 @register_packet_type_parser
 class RadiusAccessChallenge(RadiusPacket):
     CODE = Radius.ACCESS_CHALLENGE
 
 
-class RadiusAttributesList():
+class RadiusAttributesList:
     """Container class for the Radius Attribute Value Pairs"""
 
     def __init__(self, attributes):
         self.attributes = attributes
 
     @classmethod
     def parse(cls, attributes_data):
@@ -305,7 +305,13 @@
         return total
 
     def pack(self):
         packed_attributes = bytes()
         for attr in self.attributes:
             packed_attributes += attr.pack()
         return packed_attributes
+
+    def to_dict(self):
+        ret = {}
+        for a in self.attributes:
+            ret[a.DESCRIPTION] = a.data_type.data()
+        return ret
```

### Comparing `chewie-0.0.8/chewie/radius_attributes.py` & `chewie-0.0.9/chewie/radius_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,22 @@
     """Vendor-Specific https://tools.ietf.org/html/rfc2865#section-5.26"""
     TYPE = 26
     DATA_TYPE = Vsa
     DESCRIPTION = "Vendor-Specific"
 
 
 @register_attribute_type
+class SessionTimeout(Attribute):
+    """Vendor-Specific https://tools.ietf.org/html/rfc2865#section-5.27"""
+    TYPE = 27
+    DATA_TYPE = Integer
+    DESCRIPTION = "Session-Timeout"
+
+
+@register_attribute_type
 class CalledStationId(Attribute):
     """Called-Station-Id https://tools.ietf.org/html/rfc2865#section-5.30"""
     TYPE = 30
     DATA_TYPE = Text
     DESCRIPTION = "Called-Station-Id"
```

### Comparing `chewie-0.0.8/chewie/radius_datatypes.py` & `chewie-0.0.9/chewie/radius_datatypes.py`

 * *Files identical despite different names*

### Comparing `chewie-0.0.8/chewie.egg-info/PKG-INFO` & `chewie-0.0.9/chewie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: chewie
-Version: 0.0.8
+Version: 0.0.9
 Summary: A bare-bones EAPOL/802.1x implementation
 Home-page: https://github.com/faucetsdn/chewie
 Author: Sam Russell
 Author-email: sam.h.russell@gmail.com
 License: Apache2
 Description: 
             Chewie is an EAPOL/802.1x implementation in Python.
```

### Comparing `chewie-0.0.8/chewie.egg-info/SOURCES.txt` & `chewie-0.0.9/chewie.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 chewie/ethernet_packet.py
 chewie/event.py
 chewie/mac_address.py
 chewie/message_parser.py
 chewie/radius.py
 chewie/radius_attributes.py
 chewie/radius_datatypes.py
+chewie/timer_scheduler.py
 chewie/utils.py
 chewie.egg-info/PKG-INFO
 chewie.egg-info/SOURCES.txt
 chewie.egg-info/dependency_links.txt
 chewie.egg-info/requires.txt
 chewie.egg-info/top_level.txt
 test/test_auth_8021x.py
+test/test_chewie.py
 test/test_eap.py
 test/test_ethernet_packet.py
 test/test_full_state_machine.py
+test/test_mac_address.py
 test/test_message_parser.py
 test/test_radius.py
```

### Comparing `chewie-0.0.8/test/test_auth_8021x.py` & `chewie-0.0.9/test/test_auth_8021x.py`

 * *Files identical despite different names*

### Comparing `chewie-0.0.8/test/test_eap.py` & `chewie-0.0.9/test/test_eap.py`

 * *Files identical despite different names*

### Comparing `chewie-0.0.8/test/test_ethernet_packet.py` & `chewie-0.0.9/test/test_ethernet_packet.py`

 * *Files identical despite different names*

### Comparing `chewie-0.0.8/test/test_full_state_machine.py` & `chewie-0.0.9/test/test_full_state_machine.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,203 @@
-
+"""Unittests for eap_state_machine.FullEAPStateMachine"""
 # pylint: disable=missing-docstring
 
-import sched
-import time
+import heapq
+import logging
 from queue import Queue
+import tempfile
+import time
 import unittest
 
 from netils import build_byte_string
 
+from chewie import timer_scheduler
 from chewie.eap import Eap
 from chewie.mac_address import MacAddress
 from chewie.message_parser import EapolStartMessage, IdentityMessage, Md5ChallengeMessage, \
     SuccessMessage, \
     LegacyNakMessage, TtlsMessage, FailureMessage, EapolLogoffMessage
 from chewie.eap_state_machine import FullEAPStateMachine
 from chewie.event import EventMessageReceived, EventRadiusMessageReceived, EventPortStatusChange
+from chewie.utils import get_logger
+
+
+def check_counters(_func=None, *,
+                   expected_auth_counter=0, expected_failure_counter=0, expected_logoff_counter=0):
+    """Decorator to check the handlers have been called the
+     correct number of times at the end of each test"""
+    def decorator_check_counters(func):
+        def wrapper(self):
+
+            start_auth_counter = self.auth_counter
+            start_failure_counter = self.failure_counter
+            start_logoff_counter = self.logoff_counter
+            ret = func(self)
+            self.assertEqual(self.auth_counter,
+                             start_auth_counter + expected_auth_counter)
+            self.assertEqual(self.failure_counter,
+                             start_failure_counter + expected_failure_counter)
+            self.assertEqual(self.logoff_counter,
+                             start_logoff_counter + expected_logoff_counter)
+            return ret
+
+        return wrapper
+    if _func is None:
+        return decorator_check_counters
+    else:
+        return decorator_check_counters(_func)
 
 
 class FullStateMachineStartTestCase(unittest.TestCase):
     # TODO tests could be more thorough, and test that
     # the correct packet (type/content) has been put in its respective queue.
     # Would also be nice to check that the states are correctly transitioned through,
     # and not just the final resting spot. Not sure how to do that - maybe parse the log??
 
     def setUp(self):
+        logger = logging.getLogger()
+        logger.level = logging.DEBUG
+        self.log_file = tempfile.NamedTemporaryFile()
+        logger.addHandler(logging.FileHandler(self.log_file.name))
+
         self.eap_output_queue = Queue()
         self.radius_output_queue = Queue()
-        self.timer_scheduler = sched.scheduler(time.time, time.sleep)
+        self.timer_scheduler = timer_scheduler.TimerScheduler(get_logger('chewie'))
         self.src_mac = MacAddress.from_string("00:12:34:56:78:90")
         self.sm = FullEAPStateMachine(self.eap_output_queue, self.radius_output_queue, self.src_mac,
                                       self.timer_scheduler,
-                                      self.auth_handler, self.failure_handler, self.logoff_handler, 'Chewie')
+                                      self.auth_handler, self.failure_handler, self.logoff_handler,
+                                      'Chewie')
         self.MAX_RETRANSMITS = 3
         self.sm.MAX_RETRANS = self.MAX_RETRANSMITS
         self.sm.DEFAULT_TIMEOUT = 0.1
         self.sm.portEnabled = True
         self.sm.eapRestart = True
 
-    def auth_handler(self, client_mac, port_id_mac):
+        self.auth_counter = 0
+        self.failure_counter = 0
+        self.logoff_counter = 0
+
+    def tearDown(self):
+        with open(self.log_file.name) as log:
+            self.assertNotIn('aaaEapResp is true. but data is false. This should never happen',
+                             log.read())
+
+    def run_scheduler(self):
+        """use this to run the scheduler without the whole threading/eventlet thing
+         (this returns when empty)"""
+        while True:
+            if len(self.timer_scheduler.timer_heap):
+                if self.timer_scheduler.timer_heap[0][0] < time.time():
+                    _, job = heapq.heappop(self.timer_scheduler.timer_heap)
+                    if not job.cancelled():
+                        job.func(*job.args)
+                else:
+                    time.sleep(1)
+            else:
+                time.sleep(1)
+                return
+
+    def auth_handler(self, client_mac, port_id_mac):  # pylint: disable=unused-argument
+        self.auth_counter += 1
         print('Successful auth from MAC %s' % str(client_mac))
 
-    def failure_handler(self, client_mac, port_id_mac):
+    def failure_handler(self, client_mac, port_id_mac):  # pylint: disable=unused-argument
+        self.failure_counter += 1
         print('failure from MAC %s' % str(client_mac))
 
-    def logoff_handler(self, client_mac, port_id_mac):
+    def logoff_handler(self, client_mac, port_id_mac):  # pylint: disable=unused-argument
+        self.logoff_counter += 1
         print('logoff from MAC %s' % str(client_mac))
 
+    @check_counters
     def test_eap_start(self):
         # input EAPStart packet.
         # output EAPIdentityRequest on eap_output_q
         message = EapolStartMessage(self.src_mac)
         self.sm.event(EventMessageReceived(message, None))
         self.assertEqual(self.sm.currentState, self.sm.IDLE)
 
         self.assertEqual(self.eap_output_queue.qsize(), 1)
         output = self.eap_output_queue.get_nowait()[0]
         self.assertIsInstance(output, IdentityMessage)
         self.assertEqual(self.radius_output_queue.qsize(), 0)
+
         return output  # Used by test_identity_response
 
+    @check_counters
     def test_eap_restart(self):
         self.test_eap_start()
         message = EapolStartMessage(self.src_mac)
         self.sm.event(EventMessageReceived(message, None))
         self.assertEqual(self.sm.currentState, self.sm.IDLE)
 
         self.assertEqual(self.eap_output_queue.qsize(), 1)
         output = self.eap_output_queue.get_nowait()[0]
         self.assertIsInstance(output, IdentityMessage)
         self.assertEqual(self.radius_output_queue.qsize(), 0)
 
+    @check_counters
     def test_timeout_failure_from_max_retransmits(self):
         """Go to timeout failure from exceeding max retransmits (also tests retransmitting)"""
         output0 = self.test_eap_start()
 
         old_radius_count = self.radius_output_queue.qsize()
-        self.timer_scheduler.run()
+        self.run_scheduler()
 
         output1 = self.eap_output_queue.get_nowait()[0]
         output2 = self.eap_output_queue.get_nowait()[0]
         self.assertIsInstance(output0, IdentityMessage)
         self.assertIsInstance(output1, IdentityMessage)
         self.assertEqual(output0, output1)
         self.assertEqual(output0, output2)
         self.assertEqual(self.radius_output_queue.qsize(), 0)
 
         self.assertEqual(self.sm.currentState, self.sm.TIMEOUT_FAILURE)
         self.assertEqual(self.eap_output_queue.qsize(), 0)
         self.assertEqual(old_radius_count, self.radius_output_queue.qsize())
 
+    @check_counters
     def test_timeout_failure2_from_aaa_timeout(self):
         """no response from AAA server equals timeout_failure2"""
         self.test_md5_challenge_response()
         old_eap_count = self.eap_output_queue.qsize()
         old_radius_count = self.radius_output_queue.qsize()
 
-        self.timer_scheduler.run()
+        self.run_scheduler()
 
         self.assertEqual(self.sm.currentState, self.sm.TIMEOUT_FAILURE2)
         self.assertEqual(old_eap_count, self.eap_output_queue.qsize())
         self.assertEqual(old_radius_count, self.radius_output_queue.qsize())
 
+    @check_counters
     def test_timeout_failure2_from_max_retransmits(self):
         """If client does not respond when in passthrough mode,
          send again and again until max retransmit counter is reached."""
         self.test_md5_challenge_request()
         self.assertEqual(self.eap_output_queue.qsize(), 0)
         old_radius_count = self.radius_output_queue.qsize()
 
-        self.timer_scheduler.run()
+        self.run_scheduler()
 
         self.assertEqual(self.sm.currentState, self.sm.TIMEOUT_FAILURE2)
         self.assertEqual(self.MAX_RETRANSMITS, self.eap_output_queue.qsize())
         self.assertEqual(old_radius_count, self.radius_output_queue.qsize())
 
+    @check_counters(expected_auth_counter=1)
     def test_disabled_state(self):
         """move to disabled and then from disabled"""
+        self.test_success2()
         # move to disabled. e.g. link down.
-        self.test_eap_start()
         self.sm.event(EventPortStatusChange(False))
         self.assertEqual(self.sm.currentState, self.sm.DISABLED)
 
         self.assertEqual(self.eap_output_queue.qsize(), 0)
         self.assertEqual(self.radius_output_queue.qsize(), 0)
-
+        self.assertEqual(self.auth_counter, 1)
         # don't transition to initialize (still not enabled)
         message = EapolStartMessage(self.src_mac)
         self.sm.event(EventMessageReceived(message, None))
         self.assertEqual(self.sm.currentState, self.sm.DISABLED)
         self.assertEqual(self.eap_output_queue.qsize(), 0)
         self.assertEqual(self.radius_output_queue.qsize(), 0)
 
@@ -135,119 +205,150 @@
         self.sm.event(EventPortStatusChange(True))
 
         self.assertEqual(self.sm.currentState, self.sm.IDLE)
 
         self.assertEqual(self.eap_output_queue.qsize(), 1)
         self.assertEqual(self.radius_output_queue.qsize(), 0)
 
+    @check_counters
     def test_identity_response(self):
         _id = self.test_eap_start().message_id
         # input EapIdentityResponse
         # output EapIdentityResponse on radius_output_q
         message = IdentityMessage(self.src_mac, _id, Eap.RESPONSE, "host1user")
         self.sm.event(EventMessageReceived(message, None))
         self.assertEqual(self.sm.currentState, self.sm.AAA_IDLE)
 
         self.assertEqual(self.eap_output_queue.qsize(), 0)
         self.assertEqual(self.radius_output_queue.qsize(), 1)
         self.assertIsInstance(self.radius_output_queue.get_nowait()[0], IdentityMessage)
 
+    @check_counters
     def test_md5_challenge_request(self):
         self.test_identity_response()
 
         eap_message = Md5ChallengeMessage(self.src_mac, 2, Eap.REQUEST,
                                           build_byte_string("74d3db089b727d9cc5774599e4a32a29"),
                                           b"host1user")
         self.sm.event(EventRadiusMessageReceived(eap_message, None))
         self.assertEqual(self.sm.currentState, self.sm.IDLE2)
 
         self.assertEqual(self.eap_output_queue.qsize(), 1)
-        self.assertIsInstance(self.eap_output_queue.get_nowait()[0], Md5ChallengeMessage)
+        output = self.eap_output_queue.get_nowait()[0]
+        self.assertIsInstance(output, Md5ChallengeMessage)
 
         self.assertEqual(self.radius_output_queue.qsize(), 0)
+        return output
 
+    @check_counters
     def test_md5_challenge_response(self):
         self.test_md5_challenge_request()
 
         message = Md5ChallengeMessage(self.src_mac, 2, Eap.RESPONSE,
                                       build_byte_string("3a535f0ee8c6b34fe714aa7dad9a0e15"),
                                       b"host1user")
         self.sm.event(EventMessageReceived(message, None))
         self.assertEqual(self.sm.currentState, self.sm.AAA_IDLE)
         self.assertEqual(self.eap_output_queue.qsize(), 0)
         self.assertEqual(self.radius_output_queue.qsize(), 1)
         self.assertIsInstance(self.radius_output_queue.get_nowait()[0], Md5ChallengeMessage)
 
+    @check_counters(expected_auth_counter=1)
     def test_success2(self):
         self.test_md5_challenge_response()
 
         message = SuccessMessage(self.src_mac, 3)
         self.sm.event(EventRadiusMessageReceived(message, None))
 
         self.assertEqual(self.sm.currentState, self.sm.SUCCESS2)
         self.assertEqual(self.eap_output_queue.qsize(), 1)
         self.assertIsInstance(self.eap_output_queue.get_nowait()[0], SuccessMessage)
         self.assertEqual(self.radius_output_queue.qsize(), 0)
 
+    @check_counters(expected_auth_counter=2)
+    def test_two_success2(self):
+        self.test_success2()
+
+        expiry_job = self.sm.session_timeout_job
+        self.assertFalse(expiry_job.cancelled())
+
+        self.test_success2()
+        self.assertTrue(expiry_job.cancelled())
+
+        expiry_job = self.sm.session_timeout_job
+        self.assertFalse(expiry_job.cancelled())
+
+    @check_counters(expected_auth_counter=2, expected_logoff_counter=1)
     def test_logoff2(self):
         """Test logoff from success2 state."""
         self.test_success2()
 
+        # test the second logon expires the firsts session timeout event.
+        expiry_job = self.sm.session_timeout_job
+        self.assertFalse(expiry_job.cancelled())
+
         message = EapolLogoffMessage(self.src_mac)
         self.sm.event(EventRadiusMessageReceived(message, None))
 
+        self.assertTrue(expiry_job.cancelled())
+
         self.assertEqual(self.sm.currentState, self.sm.LOGOFF2)
         self.assertEqual(self.eap_output_queue.qsize(), 0)
         self.assertEqual(self.radius_output_queue.qsize(), 0)
 
         self.test_success2()
 
+    @check_counters
     def test_logoff_from_idle2(self):
         """Test logoff from middle of authentication. should be ignored"""
         self.test_md5_challenge_request()
 
         message = EapolLogoffMessage(self.src_mac)
         self.sm.event(EventRadiusMessageReceived(message, None))
 
         # should be in same state as when test_md5_challenge_request returned.
         self.assertEqual(self.sm.currentState, self.sm.IDLE2)
         self.assertEqual(self.eap_output_queue.qsize(), 0)
         self.assertEqual(self.radius_output_queue.qsize(), 0)
 
+    @check_counters(expected_failure_counter=1)
     def test_failure2(self):
         self.test_md5_challenge_response()
         message = FailureMessage(self.src_mac, 3)
         self.sm.event(EventRadiusMessageReceived(message, None))
 
         self.assertEqual(self.sm.currentState, self.sm.FAILURE2)
         self.assertEqual(self.eap_output_queue.qsize(), 1)
         self.assertIsInstance(self.eap_output_queue.get_nowait()[0], FailureMessage)
         self.assertEqual(self.radius_output_queue.qsize(), 0)
 
+    @check_counters
     def test_discard2(self):
-        self.test_md5_challenge_request()
+        request = self.test_md5_challenge_request()
 
-        message = Md5ChallengeMessage(self.src_mac, 222, Eap.RESPONSE,
+        message = Md5ChallengeMessage(self.src_mac, request.message_id + 10, Eap.RESPONSE,
                                       build_byte_string("3a535f0ee8c6b34fe714aa7dad9a0e15"),
                                       b"host1user")
         self.sm.event(EventMessageReceived(message, None))
         self.assertEqual(self.sm.currentState, self.sm.IDLE2)
         self.assertEqual(self.eap_output_queue.qsize(), 0)
         self.assertEqual(self.radius_output_queue.qsize(), 0)
 
+    @check_counters
     def test_discard(self):
-        self.test_eap_start()
-
-        message = IdentityMessage(self.src_mac, 40, Eap.RESPONSE, "host1user")
+        message = self.test_eap_start()
+        # Make a message that will be discarded (id here is not sequential)
+        message = IdentityMessage(self.src_mac, message.message_id + 10, Eap.RESPONSE, "host1user")
         self.sm.event(EventMessageReceived(message, None))
         self.assertEqual(self.sm.currentState, self.sm.IDLE)
 
         self.assertEqual(self.eap_output_queue.qsize(), 0)
         self.assertEqual(self.radius_output_queue.qsize(), 0)
 
+    @check_counters
     def test_ttls_request(self):
         self.test_md5_challenge_request()
         self.assertEqual(self.eap_output_queue.qsize(), 0)
         self.assertEqual(self.radius_output_queue.qsize(), 0)
 
         message = LegacyNakMessage(self.src_mac, 2, Eap.RESPONSE, 21)
         self.sm.event(EventMessageReceived(message, None))
@@ -270,7 +371,16 @@
 
         message = TtlsMessage(self.src_mac, 4, Eap.REQUEST, 0x00, build_byte_string(
             '160303003e0200003a03036bf75d277e59b04228197af91c1c32c78beb8a708193ab3ac23a9aed30f5390c00c030000012ff01000100000b000403000102000f00010116030308d30b0008cf0008cc0003de308203da308202c2a003020102020101300d06092a864886f70d01010b0500308193310b3009060355040613024652310f300d06035504080c065261646975733112301006035504070c09536f6d65776865726531153013060355040a0c0c4578616d706c6520496e632e3120301e06092a864886f70d010901161161646d696e406578616d706c652e6f72673126302406035504030c1d4578616d706c6520436572746966696361746520417574686f72697479301e170d3138303630353033353134345a170d3138303830343033353134345a307c310b3009060355040613024652310f300d06035504080c0652616469757331153013060355040a0c0c4578616d706c6520496e632e3123302106035504030c1a4578616d706c65205365727665722043657274696669636174653120301e06092a864886f70d010901161161646d696e406578616d706c652e6f726730820122300d06092a864886f70d01010105000382010f003082010a0282010100cf5456d7e6142383101cf79275f6396e2c9b3f7cb2878d35e5ecc6f47ee11ef20bc8a8b3217a89351c55856e5cd5eed2d10037c9bcce89fbdf927e4cc4f069863acbac4accee7e80f2105ad80d837fa50a931c5b41d03c993f5e338cfd8e69e23818360053501c34c08132ec3d6e14df89ff29c5cec5c7a87d48c4afdcf9d3f8290050be5b903ba6a2a5ce2eb79c922cae70869618c75923059f9a8d62144e8ecdaf0a9f02886afa0e73e3d68037ea9fdca2bdd0f0785e05f5ac88031010c105575dbb09eb4f307547622120ee384ab454376de8e14e0afea02f1211801b6c932324ef6dba7abf3f48f8e3e84716c40b59041ec936cb273d684b22aa1c9d24e10203010001a34f304d30130603551d25040c300a06082b0601050507030130360603551d1f042f302d302ba029a0278625687474703a2f2f7777772e6578616d706c652e636f6d2f6578616d706c655f63612e63726c300d06092a864886f70d01010b0500038201010054fdcdabdc3a153dc167d6b210d1b324ecfac0e3b8d385704463a7f8ebf46e2e6952f249f4436ec66760868860e5ed50b519ec14628179472c312f507bc9349971d21f8f2b7d6b329b02fab448bd90fd4ce4dfbc78f23a8c4eed74d5589f4c3bd11b552535b8ab8a1a6ab9d1dfda21f247a93354702c12fdde1113cb8dd0e46e2a3a94547c9871df2a88943751d8276dc43f7f6aed921f43f6a33f9beba804c3d2b5781d754abe36ba58461798be8585b8b24b5c4a26d1e0905eb5bbae6e139b06728406bfe31baa27852252c7b4711c35ec9a41945488ef8c79a8a201351189e65baed66300528b45dfbcad233cd045336d5b35331ee76360b58583884eb0aa0004e8308204e4308203cca003020102020900de5bbe2e4d41d7fd300d06092a864886f70d01010b0500308193310b3009060355040613024652310f300d06035504080c065261646975733112301006035504070c09536f6d65776865726531153013060355040a0c0c4578616d706c6520496e632e3120301e06092a864886f70d010901161161646d696e406578616d706c652e6f72673126302406035504030c1d4578616d706c6520436572746966696361746520417574686f72697479301e170d3138303630353033353134345a170d3138303830343033353134345a308193310b3009060355040613024652310f300d06035504080c065261646975733112301006035504070c09536f6d65776865726531153013060355040a0c0c4578616d706c6520496e632e3120301e06092a864886f70d010901161161646d696e406578616d706c652e6f72673126302406035504030c1d4578616d706c6520436572746966696361746520417574686f7269747930820122300d06092a864886f70d01010105000382010f003082010a02820101009b2190c32456e96ad8d08c6577839dcaf819f98a104bad079330714b7c12c765861c9a2e74eb0aec87a64eb58caa781f543eb2971db6b9e3b662952213aaf806fbb38c7a7fa46135c14a2e0e0a158162c2414e3c3f835bf4b80007c03df51746a04715dada1fb9fb155d479da9c34e40f192c65f64b16d4c742e66cbdc748ce0763cd45b7a88ff7d99d66449676a07116651394107c2ab5d654ad9a0315b78a2342a26790629fbe1e19a734e5e2eab933f3cef3e81c4413443988c8ccd9bc35b7ba3c6ec5571f4089ab07e401b2f21131316d4f8333782acc76d661f8440287c8e0a122200d9067b6b5d2af4cd5ab23f69cd689652c813fdd04f4f83544b4d450203010001a382013730820133301d0603551d0e0416041473fd7fcd4adc85cbfd85734c722335e7472b8df03081c80603551d230481c03081bd801473fd7fcd4adc85cbfd85734c722335e7472b8df0a18199a48196308193310b3009060355040613024652310f300d06035504080c065261646975733112301006035504070c09536f6d65776865726531153013060355040a0c0c4578616d706c6520496e632e3120301e06092a864886f70d010901161161646d696e406578616d706c652e6f72673126302406035504030c1d4578616d706c6520436572746966696361746520417574686f72697479820900de5bbe2e4d41d7fd300f0603551d130101ff040530030101ff30360603551d1f042f302d302ba029a0278625687474703a2f2f7777772e6578616d706c652e6f72672f6578616d706c655f63612e63726c300d06092a864886f70d01010b05000382010100139e9c2b1e9bf30c6567759ffb57af9f031a59b6a8adb1702a55de2e51f2286715ef1399ebdc593d38db3ad4794c3e78037d3de5612cba33cefc5b830c3a2118bfc0572d201c07105b7c0ef5bb64225d959afef6a4527a88d1e5fd552fd16775a5c90802d11ad793da157441f7a181f85a2908ebcb87a86960c6d3ae631019bc73f850bc5be494a97084ccaea1cc13c44a4fdf0ef123c067b688e47a4d223c15fd56798051ff4912c721f15c96061ef683b1ade02b5449b06184f59d4218f2287d35cfa0a3a4f65e40c8750d0c70dc00d65a8981e0a2cf6961b1355c10d399ce583a426e211b0feef37da67a57bbbc81d912d5379668cfdc3666bacf5e9d9c7d160303014d0c0001490300174104b275c284c5c067b9c3104305ba6704b4b0e083f0e285d9b205a8d7307e503907478f314679d084a0f1ccbc3ceaa6b6d56c588654d223fd16514bba463c5f8d7006010100bca760ef9aab5f1cf9239bab7d0bbf585e12f9c6440b9dd36affc87ff8f334b0dbea94686edbcff9143bd40a5136b065d5599742665fa27d5ec5e86898b7c8cc2c375d190646c644df7911f41a12a7219f667527cfc4ba99b684fb763a01f4dc361a891906e3ade0c6e787c096f868726a5aafafb76ce71ce896b50015c9db89e9c3d13c90e90b5d82a1327941404298c1e358cbc7bbbf8e4fe2e1ecafbcbddfbe0b1a7d3f0769306f16f3ed4972b14b8af0f51761053754ec73a1a41b294fe0d00a9281e3d9c0175651d2bbaf28df32a25bfbae85983a3935891f0a955b636b3540cde3aba4ec20d62988a81a608b450e87b3eefcb66f50cf3104a4b367122d16030300040e000000'))
         self.sm.event(EventRadiusMessageReceived(message, None))
         self.assertEqual(self.sm.currentState, self.sm.IDLE2)
         self.assertEqual(self.eap_output_queue.qsize(), 2)
         self.assertEqual(self.radius_output_queue.qsize(), 2)
+
+    @check_counters(expected_auth_counter=1, expected_logoff_counter=1)
+    def test_deauth_timer(self):
+        self.sm.DEFAULT_SESSION_TIMEOUT = 2
+        self.test_success2()
+
+        self.run_scheduler()
+
+        self.assertEqual(self.sm.currentState, self.sm.LOGOFF2)
```

### Comparing `chewie-0.0.8/test/test_message_parser.py` & `chewie-0.0.9/test/test_message_parser.py`

 * *Files identical despite different names*

### Comparing `chewie-0.0.8/test/test_radius.py` & `chewie-0.0.9/test/test_radius.py`

 * *Files identical despite different names*

### Comparing `chewie-0.0.8/README.md` & `chewie-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `chewie-0.0.8/setup.py` & `chewie-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     More information at https://github.com/faucetsdn/chewie
 """
 
 setup(
     name='chewie',
     description='A bare-bones EAPOL/802.1x implementation',
     long_description=long_description,
-    version='0.0.8',
+    version='0.0.9',
     url='https://github.com/faucetsdn/chewie',
     author='Sam Russell',
     author_email='sam.h.russell@gmail.com',
     license='Apache2',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: System Administrators',
```

### Comparing `chewie-0.0.8/PKG-INFO` & `chewie-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: chewie
-Version: 0.0.8
+Version: 0.0.9
 Summary: A bare-bones EAPOL/802.1x implementation
 Home-page: https://github.com/faucetsdn/chewie
 Author: Sam Russell
 Author-email: sam.h.russell@gmail.com
 License: Apache2
 Description: 
             Chewie is an EAPOL/802.1x implementation in Python.
```

