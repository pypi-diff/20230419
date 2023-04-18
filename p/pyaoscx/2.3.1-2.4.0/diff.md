# Comparing `tmp/pyaoscx-2.3.1.tar.gz` & `tmp/pyaoscx-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaoscx-2.3.1.tar", last modified: Mon Oct 24 22:36:10 2022, max compression
+gzip compressed data, was "/ws/chiapuzi/tme/pyaoscx/dist/.tmp-eyqizy5b/pyaoscx-2.4.0.tar", last modified: Tue Apr 18 21:01:16 2023, max compression
```

## Comparing `pyaoscx-2.3.1.tar` & `pyaoscx-2.4.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2022-10-24 22:36:10.879690 pyaoscx-2.3.1/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     4495 2022-10-24 22:36:10.879690 pyaoscx-2.3.1/PKG-INFO
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     3892 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/README.md
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2022-10-24 22:36:10.875690 pyaoscx-2.3.1/pyaoscx/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    18368 2022-10-24 22:31:14.000000 pyaoscx-2.3.1/pyaoscx/acl.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    20314 2022-10-24 22:31:14.000000 pyaoscx-2.3.1/pyaoscx/acl_entry.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    14746 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/aggregate_address.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     6611 2022-08-01 18:02:33.000000 pyaoscx-2.3.1/pyaoscx/api.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    14684 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/bgp_neighbor.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    15436 2022-08-01 18:02:33.000000 pyaoscx-2.3.1/pyaoscx/bgp_router.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    16265 2022-10-24 22:31:14.000000 pyaoscx-2.3.1/pyaoscx/configuration.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    17602 2022-10-24 22:31:14.000000 pyaoscx-2.3.1/pyaoscx/device.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    13677 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/dhcp_relay.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    11085 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/dns.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2022-10-24 22:36:10.875690 pyaoscx-2.3.1/pyaoscx/exceptions/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/exceptions/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1087 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/exceptions/generic_op_error.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      801 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/exceptions/login_error.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      320 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/exceptions/parameter_error.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      450 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/exceptions/pyaoscx_error.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      879 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/exceptions/response_error.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      321 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/exceptions/unsupported_capability_error.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      871 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/exceptions/verification_error.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1002 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/firmware.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    82298 2022-08-01 18:02:33.000000 pyaoscx-2.3.1/pyaoscx/interface.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    12938 2022-08-01 18:02:33.000000 pyaoscx-2.3.1/pyaoscx/ipv6.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    12202 2022-08-01 18:02:33.000000 pyaoscx-2.3.1/pyaoscx/mac.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    11203 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/ospf_area.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    10216 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/ospf_interface.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    12445 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/ospf_router.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     8448 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/ospf_virtual_link.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      321 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/ospfv3_router.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     8435 2022-08-01 18:02:33.000000 pyaoscx-2.3.1/pyaoscx/poe_interface.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    57107 2022-08-01 18:02:33.000000 pyaoscx-2.3.1/pyaoscx/pyaoscx_factory.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    12390 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/pyaoscx_module.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     9771 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/qos.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     9169 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/qos_cos.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    11970 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/qos_dscp.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     9405 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/queue.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     7482 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/queue_profile.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     7684 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/queue_profile_entry.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2022-10-24 22:36:10.875690 pyaoscx-2.3.1/pyaoscx/rest/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/rest/__init__.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2022-10-24 22:36:10.875690 pyaoscx-2.3.1/pyaoscx/rest/v1/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/rest/v1/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     2703 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/rest/v1/api.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    32985 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/rest/v1/interface.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2022-10-24 22:36:10.875690 pyaoscx-2.3.1/pyaoscx/rest/v10_04/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/rest/v10_04/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1321 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/rest/v10_04/api.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      286 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/rest/v10_04/interface.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2022-10-24 22:36:10.875690 pyaoscx-2.3.1/pyaoscx/rest/v10_08/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/rest/v10_08/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1322 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/rest/v10_08/api.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      286 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/rest/v10_08/interface.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2022-10-24 22:36:10.879690 pyaoscx-2.3.1/pyaoscx/rest/v10_09/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-10-24 22:31:14.000000 pyaoscx-2.3.1/pyaoscx/rest/v10_09/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1369 2022-10-24 22:31:14.000000 pyaoscx-2.3.1/pyaoscx/rest/v10_09/api.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      281 2022-10-24 22:31:14.000000 pyaoscx-2.3.1/pyaoscx/rest/v10_09/interface.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    12385 2022-10-24 22:31:14.000000 pyaoscx-2.3.1/pyaoscx/session.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     7207 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/static_mac.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    15714 2022-08-01 18:02:33.000000 pyaoscx-2.3.1/pyaoscx/static_nexthop.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    16473 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/static_route.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     8305 2022-08-01 18:02:33.000000 pyaoscx-2.3.1/pyaoscx/tunnel_endpoint.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2022-10-24 22:36:10.879690 pyaoscx-2.3.1/pyaoscx/utils/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/utils/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     3693 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/utils/list_attributes.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     7306 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/utils/util.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    18684 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/vlan.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     9710 2022-08-01 18:02:33.000000 pyaoscx-2.3.1/pyaoscx/vni.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    25349 2022-08-01 18:02:33.000000 pyaoscx-2.3.1/pyaoscx/vrf.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    13225 2022-08-01 18:02:33.000000 pyaoscx-2.3.1/pyaoscx/vrf_address_family.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     8265 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/pyaoscx/vsx.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2022-10-24 22:36:10.875690 pyaoscx-2.3.1/pyaoscx.egg-info/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     4495 2022-10-24 22:36:10.000000 pyaoscx-2.3.1/pyaoscx.egg-info/PKG-INFO
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1851 2022-10-24 22:36:10.000000 pyaoscx-2.3.1/pyaoscx.egg-info/SOURCES.txt
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        1 2022-10-24 22:36:10.000000 pyaoscx-2.3.1/pyaoscx.egg-info/dependency_links.txt
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        1 2022-08-01 21:22:25.000000 pyaoscx-2.3.1/pyaoscx.egg-info/not-zip-safe
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)       24 2022-10-24 22:36:10.000000 pyaoscx-2.3.1/pyaoscx.egg-info/requires.txt
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)       18 2022-10-24 22:36:10.000000 pyaoscx-2.3.1/pyaoscx.egg-info/top_level.txt
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)       38 2022-10-24 22:36:10.879690 pyaoscx-2.3.1/setup.cfg
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1082 2022-10-24 22:31:14.000000 pyaoscx-2.3.1/setup.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2022-10-24 22:36:10.879690 pyaoscx-2.3.1/workflows/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/workflows/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     3929 2022-03-04 22:37:13.000000 pyaoscx-2.3.1/workflows/workflow.py
+drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     4495 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/PKG-INFO
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     3892 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/README.md
+drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/__init__.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    18333 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/acl.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    21841 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/acl_entry.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    14710 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/aggregate_address.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     6590 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/api.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    14625 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/bgp_neighbor.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    15388 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/bgp_router.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    16209 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/configuration.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    18864 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/device.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    13836 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/dhcp_relay.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    10951 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/dns.py
+drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/exceptions/
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/__init__.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1087 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/generic_op_error.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)      801 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/login_error.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)      320 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/parameter_error.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)      450 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/pyaoscx_error.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)      879 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/response_error.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)      321 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/unsupported_capability_error.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)      871 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/verification_error.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1005 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/firmware.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    83726 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/interface.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    12912 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/ipv6.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    13019 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/mac.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    11167 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/ospf_area.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    10174 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/ospf_interface.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    13376 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/ospf_router.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     8406 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/ospf_virtual_link.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)      321 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/ospfv3_router.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     8680 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/poe_interface.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    56938 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/pyaoscx_factory.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    12301 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/pyaoscx_module.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     9780 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/qos.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     9149 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/qos_cos.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    11962 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/qos_dscp.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     9377 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/queue.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     7452 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/queue_profile.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     7662 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/queue_profile_entry.py
+drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/rest/
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/__init__.py
+drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/rest/v1/
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v1/__init__.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     2703 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v1/api.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    32985 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v1/interface.py
+drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_04/
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_04/__init__.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1321 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_04/api.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)      286 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_04/interface.py
+drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_08/
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_08/__init__.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1322 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_08/api.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)      286 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_08/interface.py
+drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_09/
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-10-24 22:31:14.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_09/__init__.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1369 2022-10-24 22:31:14.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_09/api.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)      281 2022-10-24 22:31:14.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_09/interface.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    12436 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/session.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    11182 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/static_mac.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    15678 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/static_nexthop.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    16433 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/static_route.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     8288 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/tunnel_endpoint.py
+drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/utils/
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/utils/__init__.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     3693 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/utils/list_attributes.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    11109 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/utils/util.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    18698 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/vlan.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     9887 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/vni.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    25272 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/vrf.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)    13186 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/vrf_address_family.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     8257 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/vsx.py
+drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx.egg-info/
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     4495 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx.egg-info/PKG-INFO
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1851 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx.egg-info/SOURCES.txt
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)        1 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx.egg-info/dependency_links.txt
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)        1 2022-08-01 21:22:25.000000 pyaoscx-2.4.0/pyaoscx.egg-info/not-zip-safe
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)       48 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx.egg-info/requires.txt
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)       18 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx.egg-info/top_level.txt
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)       38 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/setup.cfg
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1159 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/setup.py
+drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/workflows/
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/workflows/__init__.py
+-rw-r--r--   0 chiapuzi (60029124) warp      (2000)     3929 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/workflows/workflow.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyaoscx-2.3.1/PKG-INFO` & `pyaoscx-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaoscx
-Version: 2.3.1
+Version: 2.4.0
 Summary: AOS-CX Python Modules
 Home-page: https://github.com/aruba/pyaoscx
 Author: Aruba Automation
 Author-email: aruba-automation@hpe.com
 License: Apache 2.0
 Keywords: networking aruba aos-cx switch rest api python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyaoscx-2.3.1/README.md` & `pyaoscx-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.3.1/pyaoscx/acl.py` & `pyaoscx-2.4.0/pyaoscx/acl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 import re
 
 from random import randint
@@ -50,14 +50,15 @@
         self._update_version()
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for an ACL table entry and fill
             the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if there is not an exception raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -131,14 +132,15 @@
         return True
 
     @classmethod
     def get_all(cls, session):
         """
         Perform a GET call to retrieve all system ACLs, and create a dictionary
             containing them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :return: Dictionary containing ACLs IDs as keys and a Acl objects as
             values.
         """
         logging.info("Retrieving all %s data from switch", cls.__name__)
@@ -167,14 +169,15 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update an existing ACL table
             entry. Checks whether the ACL exists in the switch. Calls
             self.update() if ACL being updated. Calls self.create() if a new
             ACL is being created.
+
         :return modified: Boolean, True if object was created or modified.
         """
         modified = False
         if self.materialized:
             modified = self.update()
         else:
             modified = self.create()
@@ -182,14 +185,15 @@
         self.__modified = modified
         return modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing ACL table entry.
+
         :return modified: True if Object was modified and a PUT request
             was made.
         """
         # Variable returned
         modified = False
 
         acl_data = utils.get_attrs(self, self.config_attrs)
@@ -231,14 +235,15 @@
         return modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new ACL table entry. Only returns if no
             exception is raised.
+
         :return modified: Boolean, True if entry was created.
         """
         acl_data = utils.get_attrs(self, self.config_attrs)
         acl_data["name"] = self.name
         acl_data["list_type"] = self.list_type
 
         post_data = json.dumps(acl_data)
@@ -288,14 +293,15 @@
         # Delete object attributes
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, response_data):
         """
         Create a Acl object given a response_data.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device
         :param response_data: The response must be a dictionary of the form:
             { "{name},{list_type}": URL }, with URL being of the form:
             "/rest/v10.04/system/acls/{name},{list_type}"
         :return: Acl object.
@@ -306,14 +312,15 @@
 
         return ACL(session, name, list_type)
 
     @classmethod
     def from_uri(cls, session, uri):
         """
         Create a Acl object given a URI.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param uri: a String with a URI
         :return indices, acl: tuple containing both the indices and Acl object.
         """
         # Obtain ID from URI
@@ -332,14 +339,15 @@
     def __str__(self):
         return "ACL name:{0}, list_type:{1}".format(self.name, self.list_type)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific ACL URI.
+
         return: Object's URI.
         """
         if self._uri is None:
             self._uri = "{0}{1}/{2}{3}{4}".format(
                 self.session.resource_prefix,
                 ACL.base_uri,
                 self.name,
@@ -350,14 +358,15 @@
         return self._uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
+
         return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     @property
     def modified(self):
         """
@@ -365,14 +374,15 @@
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     def _update_version(self):
         """
         Whenever the ACL (or any of its entries) change,the version should be
@@ -416,39 +426,40 @@
         src_mac=None,
         dst_mac=None,
         ethertype=None,
     ):
         """
         Create an AclEntry object, ACL Entry already exists, value passed
             won't update the entry.
+
         :param sequence_num: Integer number of the sequence
         :param action: Action should be either "permit" or "deny"
         :param count: Optional boolean flag that when true, will make entry
             increment hit count for matched packets
         :param protocol: Optional integer IP protocol number
         :param src_ip: Optional source IP address. Both IPv4 and IPv6 are
             supported.
             Example:
-                10.10.12.11/255.255.255.255
-                2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
+            10.10.12.11/255.255.255.255
+            2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
         :param dst_ip: Optional destination IP address. Both IPv4 and IPv6
             are supported.
             Example:
-                10.10.12.11/255.255.255.255
-                2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
+            10.10.12.11/255.255.255.255
+            2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
         :param dst_l4_port_min: Optional minimum L4 port number in range; used
             in conjunction with dst_l4_port_max.
         :param dst_l4_port_max: Optional maximum L4 port number in range; used
             in conjunction with dst_l4_port_min.
         :param src_mac: Optional source MAC address
             Example:
-                '01:02:03:04:05:06'
+            '01:02:03:04:05:06'
         :param dst_mac: Optional destination MAC address
             Example:
-                '01:02:03:04:05:06'
+            '01:02:03:04:05:06'
         :param ethertype: Optional integer EtherType number
         :return acl_entry: A AclEntry object
         """
         # Create ACL Entry
         acl_entry_obj = self.session.api.get_module(
             self.session,
             "AclEntry",
@@ -486,38 +497,39 @@
         dst_l4_port_max=None,
         src_mac=None,
         dst_mac=None,
         ethertype=None,
     ):
         """
         Modify an existing ACL Entry.
+
         :param sequence_num: Integer number of the sequence.
         :param action: Action should be either "permit" or "deny".
         :param count: Optional boolean flag that when true, will make entry
             increment hit count for matched packets.
         :param src_ip: Optional source IP address. Both IPv4 and IPv6
             are supported.
             Example:
-                10.10.12.11/255.255.255.255
-                2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
+            10.10.12.11/255.255.255.255
+            2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
         :param dst_ip: Optional destination IP address. Both IPv4 and IPv6
             are supported.
             Example:
-                10.10.12.11/255.255.255.255
-                2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
+            10.10.12.11/255.255.255.255
+            2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
         :param dst_l4_port_min: Optional minimum L4 port number in range; used
             in conjunction with dst_l4_port_max.
         :param dst_l4_port_max: Optional maximum L4 port number in range; used
             in conjunction with dst_l4_port_min.
         :param src_mac: Optional source MAC address
             Example:
-                '01:02:03:04:05:06'
+            '01:02:03:04:05:06'
         :param dst_mac: Optional destination MAC address
             Example:
-                '01:02:03:04:05:06'
+            '01:02:03:04:05:06'
         :param ethertype: Optional integer EtherType number.
         :return acl_entry: A AclEntry object.
         """
         # Create ACL Entry
         acl_entry_obj = self.session.api.get_module(
             self.session, "AclEntry", sequence_num, parent_acl=self
         )
@@ -538,14 +550,15 @@
         )
 
         return acl_entry_obj
 
     def delete_all_acl_entries(self):
         """
         Delete all ACL Entries within an ACL.
+
         :return: True if object was changed
         """
         # Verify ACL has the latest data
         self.get()
 
         # Delete all entries
         self.cfg_aces = []
```

### Comparing `pyaoscx-2.3.1/pyaoscx/acl_entry.py` & `pyaoscx-2.4.0/pyaoscx/acl_entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 import re
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
 from pyaoscx.exceptions.response_error import ResponseError
+from pyaoscx.exceptions.verification_error import VerificationError
 
 from pyaoscx.utils import util as utils
 
 from pyaoscx.pyaoscx_module import PyaoscxModule
 
 
 class AclEntry(PyaoscxModule):
@@ -97,22 +98,27 @@
         # List used to determine attributes related to the acl_entry
         # configuration
         self.config_attrs = []
         self.materialized = False
         # Attribute dictionary used to manage the original data
         # obtained from the GET
         self.__original_attributes = {}
+        if "src_ip" in kwargs:
+            self.src_ip = kwargs.pop("src_ip")
+        if "dst_ip" in kwargs:
+            self.dst_ip = kwargs.pop("dst_ip")
         # Set arguments needed for correct creation
         utils.set_creation_attrs(self, **kwargs)
         # Attribute used to know if object was changed recently
         self.__modified = False
 
     def __set_acl(self, parent_acl):
         """
         Set parent Acl object as an attribute for the AclEntry object.
+
         :param parent_acl: a Acl object.
         """
         # Set parent acl
         self.__parent_acl = parent_acl
 
         # Set URI
         self.base_uri = "{0}/{1}{2}{3}/cfg_aces".format(
@@ -132,14 +138,15 @@
                 self.__parent_acl.cfg_aces.append(self)
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for an ACL Entry table entry and
             fill the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if no exception is raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -193,14 +200,15 @@
         return True
 
     @classmethod
     def get_all(cls, session, parent_acl):
         """
         Perform a GET call to retrieve all system ACL Entries inside an ACL,
             and create a dictionary containing them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_acl: parent Acl object where ACL Entry is stored.
         :return acl_entry_dict: Dictionary containing ACL Entry IDs as keys
             and an ACL Entry objects as values.
         """
@@ -241,14 +249,15 @@
     def apply(self):
         """
         Main method used to either create a new ACL Entry or update an existing
             one. It is possible that in case the are differences between the
             ACE on the switch and the local representation on immutable
             attributes a replace (delete+create) will take place. Note that
             unspecified parameters will be kept intact.
+
         :return modified: Boolean, True if object was created or modified.
         """
         if not self.__parent_acl.materialized:
             self.__parent_acl.apply()
 
         modified = False
 
@@ -287,14 +296,15 @@
 
         return modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing ACL Entry.
+
         :return modified: True if Object was modified and a PUT request
             was made.
         """
         # Variable returned
         modified = False
 
         acl_entry_data = utils.get_attrs(self, self.config_attrs)
@@ -332,29 +342,33 @@
             # Set new original attributes
             self.__original_attributes = acl_entry_data
 
             # Object was modified
             modified = True
 
         if modified:
-            self.__parent_acl._update_version()
             self.__parent_acl.apply()
 
         self.__modified = modified
         return modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new ACL Entry. Only returns if no
             exception is raised.
+
         :return modified: Boolean, True if entry was created
         """
         acl_entry_data = utils.get_attrs(self, self.config_attrs)
         acl_entry_data["sequence_number"] = self.sequence_number
+        if self.src_ip:
+            acl_entry_data["src_ip"] = self.src_ip
+        if self.dst_ip:
+            acl_entry_data["dst_ip"] = self.dst_ip
 
         # Try to get protocol number
         try:
             if isinstance(self.protocol, str):
                 if self.protocol == "any" or self.protocol == "":
                     acl_entry_data.pop("protocol")
                 else:
@@ -378,15 +392,14 @@
             raise GenericOperationError(response.text, response.status_code)
 
         logging.info("SUCCESS: Adding %s", self)
 
         # Get all object's data
         self.get()
 
-        self.__parent_acl._update_version()
         self.__parent_acl.apply()
 
         # Object was created, means modified
         self.__modified = True
         return True
 
     @PyaoscxModule.connected
@@ -407,45 +420,46 @@
 
         logging.info("SUCCESS: Deleting %s", self)
 
         # Delete back reference from ACL
         for acl_entry in self.__parent_acl.cfg_aces:
             if acl_entry.sequence_number == self.sequence_number:
                 self.__parent_acl.cfg_aces.remove(acl_entry)
-        self.__parent_acl._update_version()
         self.__parent_acl.apply()
 
         # Delete object attributes
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, parent_acl, response_data):
         """
         Create a AclEntry object given a response_data related to the ACL Entry
             sequence_number object.
+
         :param cls: Class calling the method.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_acl: parent Acl object where ACL Entry is stored.
         :param response_data: The response must be a dictionary of the form:
             {
-                <seq_number>: "/rest/v10.04/system/acls/cfg_aces/<seq_number>"
+            <seq_number>: "/rest/v10.04/system/acls/cfg_aces/<seq_number>"
             }
         :return: AclEntry object.
         """
         acl_entry_arr = session.api.get_keys(
             response_data, AclEntry.resource_uri_name
         )
         sequence_number = acl_entry_arr[0]
         return AclEntry(session, sequence_number, parent_acl)
 
     @classmethod
     def from_uri(cls, session, parent_acl, uri):
         """
         Create a AclEntry object given a URI.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_acl: parent Acl object where ACL Entry is stored.
         :param uri: a String with a URI.
         :return index, acl_entry_obj: tuple containing both the AclEntry
             object and the acl_entry's sequence_number.
         """
@@ -461,14 +475,15 @@
     def __str__(self):
         return "ACL Entry ID {0}".format(self.sequence_number)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific ACL Entry URI.
+
         return: AclEntry object's URI.
         """
         if self._uri is None:
             self._uri = "{0}{1}/{2}".format(
                 self.session.resource_prefix,
                 self.base_uri,
                 self.sequence_number,
@@ -477,14 +492,15 @@
         return self._uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
+
         return: AclEntry object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     @property
     def modified(self):
         return self.__modified
@@ -515,14 +531,15 @@
 
         return modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     ####################################################################
     # IMPERATIVE FUNCTIONS
     ####################################################################
@@ -538,25 +555,26 @@
         src_mac=None,
         dst_mac=None,
         ethertype=None,
     ):
         """
         Create an AclEntry object, ACL Entry already exists, value passed won't
             update the entry.
+
         :param action: Action should be either "permit" or "deny".
         :param count: Optional boolean flag that when true, will make entry
             increment hit count for matched packets.
         :param src_ip: Optional source IP address. Both IPv4 and IPv6 are
             supported. Example:
-                10.10.12.11/255.255.255.255
-                2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
+            10.10.12.11/255.255.255.255
+            2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
         :param dst_ip: Optional destination IP address. Both IPv4 and IPv6 are
             supported. Example:
-                10.10.12.11/255.255.255.255
-                2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
+            10.10.12.11/255.255.255.255
+            2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
         :param dst_l4_port_min: Optional minimum L4 port number in range; used
             in conjunction with dst_l4_port_max.
         :param dst_l4_port_max: Optional maximum L4 port number in range; used
             in conjunction with dst_l4_port_min.
         :param src_mac: Optional source MAC address. Example:
             '01:02:03:04:05:06'
         :param dst_mac: Optional destination MAC address. Example:
@@ -589,7 +607,51 @@
             self.dst_mac = dst_mac
 
         if ethertype is not None:
             self.ethertype = ethertype
 
         # Apply changes
         return self.apply()
+
+    @property
+    def src_ip(self):
+        """
+        Getter method for source ip attribute.
+
+        :return: String value for src_ip.
+        """
+        return self._src_ip if hasattr(self, "_src_ip") else None
+
+    @src_ip.setter
+    def src_ip(self, new_src_ip):
+        """
+        Setter method for the src_ip attribute.
+        """
+        version = utils.get_ip_version(new_src_ip)
+        if version != self.__parent_acl.list_type:
+            raise VerificationError(
+                "Version does not match the IP"
+                "version type in {}".format(self.__parent_acl.name)
+            )
+        self._src_ip = new_src_ip
+
+    @property
+    def dst_ip(self):
+        """
+        Getter method for destination ip attribute.
+
+        :return: String value for dst_ip.
+        """
+        return self._dst_ip if hasattr(self, "_dst_ip") else None
+
+    @dst_ip.setter
+    def dst_ip(self, new_dst_ip):
+        """
+        Setter method for the dst_ip attribute.
+        """
+        version = utils.get_ip_version(new_dst_ip)
+        if version != self.__parent_acl.list_type:
+            raise VerificationError(
+                "Version does not match the IP"
+                "version type in {}".format(self.__parent_acl.name)
+            )
+        self._dst_ip = new_dst_ip
```

### Comparing `pyaoscx-2.3.1/pyaoscx/aggregate_address.py` & `pyaoscx-2.4.0/pyaoscx/aggregate_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 import re
 
 from urllib.parse import quote_plus, unquote_plus
@@ -50,14 +50,15 @@
         utils.set_creation_attrs(self, **kwargs)
         # Attribute used to know if object was changed recently
         self.__modified = False
 
     def __set_name(self, ip_prefix):
         """
         Set name attribute in the proper form for references.
+
         :param ip_prefix: Object's IP.
         """
         # Add attributes to class
         self._is_lag = False
         self.ip_prefix = None
         self.reference_ip_prefix = None
         if r"%2F" in ip_prefix:
@@ -92,14 +93,15 @@
                 self.__parent_bgp_router.aggregate_addresses.append(self)
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a Aggregate Address table entry
             and fill the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if there is not an exception raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -159,14 +161,15 @@
         return True
 
     @classmethod
     def get_all(cls, session, parent_bgp_router):
         """
         Perform a GET call to retrieve all system Aggregate Addresses inside a
             BGP Router, and create a dictionary containing them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_bgp_router: parent bgp_router object where Aggregate
             Address is stored.
         :return: Dictionary containing Aggregate Addresses IDs as keys and a
             AggregateAddress objects as values.
@@ -203,15 +206,16 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method to either create or update an existing Aggregate Address.
             Checks whether the Aggregate Addresses exists in the switch. Calls
             self.update() if Aggregate Address is being updated. Calls
             self.create() if a new Aggregate Address is being created.
-        :return modified: Boolean, True if object was created or modified.
+
+        :return: Boolean, True if object was created or modified.
         """
         if not self.__parent_bgp_router.materialized:
             self.__parent_bgp_router.apply()
 
         modified = False
         if self.materialized:
             modified = self.update()
@@ -221,15 +225,16 @@
         self.__modified = modified
         return modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing Aggregate Address.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         # Variable returned
         modified = False
 
         agg_address_data = utils.get_attrs(self, self.config_attrs)
 
@@ -267,15 +272,16 @@
         return modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new Aggregate Address table entry. Only
             returns if no exception is raised.
-        :return modified: True if entry was created.
+
+        :return: True if entry was created.
         """
         ag_address_data = utils.get_attrs(self, self.config_attrs)
         ag_address_data["address-family"] = self.address_family
         ag_address_data["ip_prefix"] = self.ip_prefix
 
         post_data = json.dumps(ag_address_data)
 
@@ -332,14 +338,15 @@
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, parent_bgp_router, response_data):
         """
         Create a AggregateAddress object given a response_data related to the
             Aggregate Address ID object.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_bgp_router: parent BGP Router class where Aggregate
             Address is stored.
         :param response_data: The response must be a dictionary of the form:
             {id: URL}, with the URL being of the form:
@@ -358,20 +365,21 @@
             session, address_family, ip_prefix, parent_bgp_router
         )
 
     @classmethod
     def from_uri(cls, session, parent_bgp_router, uri):
         """
         Create a AggregateAddress object.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_bgp_router: parent BGP Router class where Aggregate
             Address is stored.
         :param uri: a String with a URI.
-        :return indices, aggr_address: tuple containing both the Aggregate
+        :return: tuple containing both the Aggregate
             Address object and the Aggregate Address' ID.
         """
         # Obtain ID from URI
         index_pattern = re.compile(
             r"(.*)aggregate_addresses/(?P<index1>.+)[,./-](?P<index2>.+)"
         )
         index1 = index_pattern.match(uri).group("index1")
@@ -388,15 +396,16 @@
     def __str__(self):
         return "Aggregate Address ID {0}".format(self.address_family)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific Aggregate Address URI.
-        return: Object's URI.
+
+        :return: Object's URI.
         """
         if self._uri is None:
             self._uri = "{0}{1}/{2}{3}{4}".format(
                 self.session.resource_prefix,
                 self.base_uri,
                 self.address_family,
                 self.session.api.compound_index_separator,
@@ -406,25 +415,27 @@
         return self._uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
-        return: Object format depending on the API Version.
+
+        :return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     @property
     def modified(self):
         """
         Return boolean with whether this object has been modified.
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
```

### Comparing `pyaoscx-2.3.1/pyaoscx/api.py` & `pyaoscx-2.4.0/pyaoscx/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     def __str__(self):
         return self.version
 
     @classmethod
     def create(cls, target_version):
         """
         Translate the version string name to a valid python symbol.
+
         :param cls: API Class object.
         :param target_version: String with the API Version.
         :return api: API object.
         """
         version_name = "v" + target_version.replace(".", "_")
 
         try:
@@ -45,27 +46,29 @@
             internal attributes, like version as minimum.
         """
         pass
 
     def valid_depth(self, depth):
         """
         Verifies if given depth is valid for the current API version.
+
         :param depth: Integer
         :return valid: Boolean True if depth is valid.
         """
         return depth in self.valid_depths
 
     def get_index(self, obj):
         """
         Method used to obtain the correct format of the objects information
             which depends on the Current API version.
+
         :param obj: PyaoscxModule object.
         :return info: Dictionary in the form of:
             "keepalive_vrf": {
-                "keepalive_name": "Resource uri",
+            "keepalive_name": "Resource uri",
             }.
         """
         key_str = ""
         length = len(obj.indices)
         attributes = []
         for i in range(length):
             attr_name = obj.indices[i]
@@ -79,53 +82,56 @@
         return info
 
     def get_keys(self, response_data, module_name=None):
         """
         Given a response_data obtain the indices of said dictionary and return
             them. Get keys should be used for only one element in the
             dictionary.
+
         :param response_data: a dictionary object in the form of:
             {
-                "idx_1,idx_2": "/rest/v10.0X/system/<module>/<idx_1>,<idx_2>",
+            "idx_1,idx_2": "/rest/v10.0X/system/<module>/<idx_1>,<idx_2>",
             }
         :return indices: List of indices.
         """
         indices = None
         for k, v in response_data.items():
             indices = k
 
         indices = indices.split(",")
         return indices
 
     def get_uri_from_data(self, data):
         """
         Given a response data, create a list of URI items. In this Version the
             data is a dict.
+
         :param data: Dictionary containing URI data in the form of:
             {
-                '<name>': '/rest/v10.0X/system/<module>/<name>',
-                '<name>': '/rest/v10.0X/system/<module>/<name>',
-                '<name>': '/rest/v10.0X/system/<module>/<name>'
+            '<name>': '/rest/v10.0X/system/<module>/<name>',
+            '<name>': '/rest/v10.0X/system/<module>/<name>',
+            '<name>': '/rest/v10.0X/system/<module>/<name>'
             }.
         :return uri_list: a list containing the input dictionary's values.
             Example:
             [
-                '/rest/v10.0X/system/<module>/<name>',
-                '/rest/v10.0X/system/<module>/<name>'
+            '/rest/v10.0X/system/<module>/<name>',
+            '/rest/v10.0X/system/<module>/<name>'
             ].
         """
         uri_list = []
         for k, v in data.items():
             uri_list.append(v)
 
         return uri_list
 
     def get_module_class(self, session, name):
         """
         Get a module's class given a session, and the module's name.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param name: Name of the module's class to be imported.
         """
         module_names = {
             "Interface": "rest.v{0}.interface".format(
                 self.version.replace(".", "_")
@@ -165,14 +171,15 @@
                 "Wrong module name. {0} doesn't exist".format(name)
             )
         return getattr(import_module("pyaoscx." + module_names[name]), name)
 
     def get_module(self, session, module, index_id=None, **kwargs):
         """
         Create a module object given a response data and the module's type.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device
         :param module: Name representing the module which is about to be
             created
         :param index_id: The module index_id or ID
         :return object: Return object same as module
         """
```

### Comparing `pyaoscx-2.3.1/pyaoscx/bgp_neighbor.py` & `pyaoscx-2.4.0/pyaoscx/bgp_neighbor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 import re
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
@@ -47,15 +47,16 @@
         utils.set_creation_attrs(self, **kwargs)
         # Attribute used to know if object was changed recently
         self.__modified = False
 
     def __set_bgp_router(self, parent_bgp_router):
         """
         Set parent BgpRouter object as an attribute for the BGP class
-        :param parent_bgp_router a BgpRouter object
+
+        :param parent_bgp_router: a BgpRouter object
         """
 
         # Set parent BGP Router
         self.__parent_bgp_router = parent_bgp_router
 
         # Set URI
         self.base_uri = "{0}/{1}/bgp_neighbors".format(
@@ -149,14 +150,15 @@
         return True
 
     @classmethod
     def get_all(cls, session, parent_bgp_router):
         """
         Perform a GET call to retrieve all system BGP Neighbors inside a BGP
         Router, and create a dictionary containing them
+
         :param cls: Object's class
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device
         :param parent_bgp_router: parent BgpRouter object where BGP Neighbor
             is stored
         :return: Dictionary containing BGP Neighbors IDs as keys and a BGP
             Neighbors objects as values
@@ -195,15 +197,16 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update an existing BGP Neighbor.
             Checks whether the BGP Neighbor exists in the switch. Calls
             self.update() if BGP Neighbor is being updated. Calls self.create()
             if a new BGP Neighbor is being created.
-        :return modified: Boolean, True if object was created or modified.
+
+        :return: Boolean, True if object was created or modified.
         """
         if not self.__parent_bgp_router.materialized:
             self.__parent_bgp_router.apply()
 
         modified = False
         if self.materialized:
             modified = self.update()
@@ -213,15 +216,16 @@
         self.__modified = modified
         return modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing BGP Neighbor.
-        :return modified: True if Object was modified and a PUT request
+
+        :return: True if Object was modified and a PUT request
             was made.
         """
         # Variable returned
         modified = False
 
         bgp_neighbor_data = utils.get_attrs(self, self.config_attrs)
 
@@ -261,16 +265,15 @@
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new BGP Neighbor table entry
         Only returns if an exception is not raise
 
-        :return modified: Boolean, True if entry was created
-
+        :return: Boolean, True if entry was created
         """
         bgp_neighbor_data = utils.get_attrs(self, self.config_attrs)
         bgp_neighbor_data[
             "ip_or_ifname_or_group_name"
         ] = self.ip_or_ifname_or_group_name
 
         if hasattr(self, "local_interface"):
@@ -307,16 +310,15 @@
 
         # Object was modified, as it was created inside Device
         return True
 
     @PyaoscxModule.connected
     def delete(self):
         """
-        Perform DELETE call to delete  BGP Neighbor table entry.
-
+        Perform DELETE call to delete BGP Neighbor table entry.
         """
 
         uri = "{0}/{1}".format(self.base_uri, self.ip_or_ifname_or_group_name)
 
         try:
             response = self.session.request("DELETE", uri)
 
@@ -340,47 +342,48 @@
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, parent_bgp_router, response_data):
         """
         Create a  BgpNeighbor object given a response_data related to the
         BGP Router ID object
+
         :param cls: Object's class
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device
         :param parent_bgp_router: parent BgpRouter object where BGP
             Neighbor is stored
         :param response_data: The response can be either a
             dictionary: {
-                    id: "/rest/v10.04/system/vrfs/<vrf_name>/bgp_routers/asn
-                        /bgp_neighbors/id"
-                }
+            id: "/rest/v10.04/system/vrfs/<vrf_name>/bgp_routers/asn
+            /bgp_neighbors/id"
+            }
             or a
             string: "/rest/v10.04/system/vrfs/<vrf_name>/bgp_routers/asn/
-                bgp_neighbors/id"
+            bgp_neighbors/id"
         :return: BgpNeighbor object
         """
         bgp_arr = session.api.get_keys(
             response_data, BgpNeighbor.resource_uri_name
         )
         bgp_neighbor_id = bgp_arr[0]
         return BgpNeighbor(session, bgp_neighbor_id, parent_bgp_router)
 
     @classmethod
     def from_uri(cls, session, parent_bgp_router, uri):
         """
         Create a BgpNeighbor object given a URI
+
         :param cls: Object's class
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device
         :param parent_bgp_router: parent BgpRouter object where BGP Neighbor
             is stored
         :param uri: a String with a URI
-
-        :return index, bgp_obj: tuple containing both the BGP object and the
+        :return: tuple containing both the BGP object and the
             BGP's ID
         """
         # Obtain ID from URI
         index_pattern = re.compile(r"(.*)bgp_neighbors/(?P<index>.+)")
         index = index_pattern.match(uri).group("index")
 
         # Create BGP object
@@ -391,14 +394,15 @@
     def __str__(self):
         return "Bgp Neighbor ID {0}".format(self.ip_or_ifname_or_group_name)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific BGP Neighbor URI
+
         return: Object's URI
         """
         if self._uri is None:
             self._uri = "{0}{1}/{2}".format(
                 self.session.resource_prefix,
                 self.base_uri,
                 self.ip_or_ifname_or_group_name,
@@ -406,26 +410,28 @@
 
         return self._uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
-        other objects
-        return: Object format depending on the API Version
+            other objects
+
+        :return: Object format depending on the API Version
         """
         return self.session.api.get_index(self)
 
     @property
     def modified(self):
         """
         Return boolean with whether this object has been modified
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
```

### Comparing `pyaoscx-2.3.1/pyaoscx/bgp_router.py` & `pyaoscx-2.4.0/pyaoscx/bgp_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
 from pyaoscx.exceptions.response_error import ResponseError
@@ -66,14 +66,15 @@
         return self.__asn
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a BGP Router table entry and
             fill the object with the incoming attributes
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if there is not an exception raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -126,14 +127,15 @@
         return True
 
     @classmethod
     def get_all(cls, session, parent_vrf):
         """
         Perform a GET call to retrieve all system BGP Routers inside a VRF, and
             create a dictionary containing them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_vrf: Vrf object where BGP Router is stored.
         :return: Dictionary containing BGP Router IDs as keys and a BGP Router
             objects as values.
         """
@@ -166,39 +168,42 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update an existing BGP Router.
             Checks whether the BGP Router exists in the switch. Calls
             self.update() if BGP Router is being updated. Calls self.create()
             if a new BGP Router is being created.
-        :return modified: Boolean, True if object was created or modified.
+
+        :return: Boolean, True if object was created or modified.
         """
         if not self.__parent_vrf.materialized:
             self.__parent_vrf.apply()
         if self.materialized:
             return self.update()
         return self.create()
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing BGP Router.
-        :return modified: True if Object was modified and a PUT request
+
+        :return: True if Object was modified and a PUT request
             was made.
         """
         bgp_router_data = utils.get_attrs(self, self.config_attrs)
         self.__modified = self._put_data(bgp_router_data)
         return self.__modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new BGP Router table entry. Only
             returns if no exception is raised.
-        :return modified: Boolean, True if entry was created.
+
+        :return: Boolean, True if entry was created.
         """
         bgp_data = utils.get_attrs(self, self.config_attrs)
         bgp_data["asn"] = self.asn
 
         self.__modified = self._post_data(bgp_data)
         return self.__modified
 
@@ -212,40 +217,42 @@
         # Delete object attributes
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, parent_vrf, response_data):
         """
         Create a BgpRouter object given a response_data related to it.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_vrf: Vrf object where BGP Router is stored.
         :param response_data: The response must be a dictionary of the form:
             {
-                <asn>: "/rest/v10.04/system/vrfs/<name>/bgp_routers/<asn>"
+            <asn>: "/rest/v10.04/system/vrfs/<name>/bgp_routers/<asn>"
             }
         :return: BgpRouter object.
         """
         bgp_arr = session.api.get_keys(
             response_data, BgpRouter.resource_uri_name
         )
         asn = bgp_arr[0]
         return BgpRouter(session, asn, parent_vrf)
 
     @classmethod
     def from_uri(cls, session, parent_vrf, uri):
         """
         Create a BgpRouter object given a URI.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_vrf: Vrf object where BGP Router is stored.
         :param uri: a String with a URI.
-        :return index, bgp_obj: tuple containing both the BgpRouter object
+        :return: tuple containing both the BgpRouter object
             and the BGP's asn.
         """
         # Obtain ID from URI
         # system/vrfs/<name>/bgp_routers/<asn>
         asn = uri.split("/")[-1]
 
         # Create BGP object
@@ -256,51 +263,55 @@
     def __str__(self):
         return "BGP Router ID {0}".format(self.asn)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific BGP Router URI.
-        return: Object's URI.
+
+        :return: Object's URI.
         """
         return self.path
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
-        return: Object format depending on the API Version.
+
+        :return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     @property
     def modified(self):
         """
         Return boolean with whether this object has been modified.
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     ####################################################################
     # IMPERATIVE FUNCTIONS
     ####################################################################
 
     def update_bgp_neighbors(self, new_neighbor):
         """
         Update references to BGP Neighbors. If a Neighbor with the same IP,
             Interface or group name is found, update the reference to the new
             neighbor, otherwise, add reference to the new neighbor.
+
         :param new_neighbor: Neighbor to add reference to.
         """
         for neighbor in self.neighbors:
             if (
                 neighbor.ip_or_ifname_or_group_name
                 == new_neighbor.ip_or_ifname_or_group_name
             ):
@@ -308,14 +319,15 @@
                 return
         self.new_neighbor.append(new_neighbor)
 
     def remove_bgp_neighbor(self, neighbor):
         """
         Update references to BGP Neighbors. If a Neighbor with the same IP,
             Interface or group name is found, delete the reference to it.
+
         :param new_neighbor: Neighbor to add reference to.
         """
         for i in self.neighbors:
             if (
                 i.ip_or_ifname_or_group_name
                 == neighbor.ip_or_ifname_or_group_name
             ):
@@ -333,14 +345,15 @@
         remote_as=None,
         update_source=None,
     ):
         """
         Perform a POST call to create BGP Neighbors to the associated current
             BGP Router. With l2vpn_evpn being True, this will also apply EVPN
             settings to the BGP neighbor configurations.
+
         :param family_type: Alphanumeric to specify what type of neighbor
             settings to configure. The options are 'ipv4-unicast',
             'ipv6-unicast' and 'l2vpn-evpn'.
         :param ip_or_ifname_or_group_name: IPv4 address or name of group of
             the neighbors that functions as the BGP Router link. Example IPv4:
             10.10.12.11/255.255.255.255
         :param activate: Boolean value to activate neighbor in the address
@@ -349,15 +362,15 @@
             soft reconfiguration.
         :param route_reflector_client: Boolean value to determine whether this
             neighbor has route reflector enabled.
         :param send_community: Boolean value to determine whether this neighbor
             has send-community enabled.
         :param remote_as: Integer peer ASN.
         :param update_source: Source address for the neighbor session.
-        :return bgp_neighbor_obj: BgpRouter object.
+        :return: BgpRouter object.
         """
         if (
             activate is not None
             or inbound_soft_reconfiguration is not None
             or route_reflector_client is not None
             or send_community is not None
         ):
```

### Comparing `pyaoscx-2.3.1/pyaoscx/configuration.py` & `pyaoscx-2.4.0/pyaoscx/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from pyaoscx.utils import util as utils
 
 from pyaoscx.pyaoscx_module import PyaoscxModule
 
 
 class Configuration:
     """
-    Represents a Device's Configuration and all of its attributes.
-    Keeping all configuration information.
+    Represents a Device's Configuration and all of its attributes
+        keeping all configuration information.
     """
 
     base_uri = "system"
 
     def __init__(self, session):
         self.session = session
         # Used to set attributes
@@ -82,28 +82,30 @@
 
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to update System Attributes. Checks whether the System
             is materialized. Calls self.update() if the configuration is being
             updated.
-        :return modified: Boolean, True if object was modified.
+
+        :return: Boolean, True if object was modified.
         """
         modified = False
         if self.materialized:
             modified = self.update()
         else:
             raise VerificationError("Device", "Not materialized")
         return modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to a Device Configuration.
-        :return modified: Boolean, True if object was modified.
+
+        :return: Boolean, True if object was modified.
         """
         system_data = utils.get_attrs(self, self.config_attrs)
 
         # Compare dictionaries
         if system_data == self.__original_attributes:
             # Object was not modified
             modified = False
@@ -139,14 +141,15 @@
     ####################################################################
     # IMPERATIVE FUNCTIONS
     ####################################################################
 
     def get_full_config(self, config_name="running-config"):
         """
         Perform a GET request to obtain the device's full config.
+
         :param config_name: String with the local-config name wanted.
             Defaults to 'running-config'.
         :return config_data: Data containing the full configuration.
         """
         uri = "fullconfigs/{0}".format(config_name)
         try:
             response = self.session.request("GET", uri)
@@ -163,21 +166,22 @@
         return config_data
 
     def tftp_switch_config_from_remote_location(
         self, config_file_location, config_name, vrf
     ):
         """
         TFTP switch config from TFTP server.
+
         :param config_file_location: TFTP server address and path for
             uploading configuration.
         :param config_name: Config file or checkpoint to be uploaded to.
             When using TFTP only running-config or startup-config can be used.
         :param vrf: VRF to be used to contact TFTP server, required if
             remote_output_file_tftp_path is provided.
-        :return success: Return True if response is successful or False if
+        :return: Return True if response is successful or False if
             it was not.
         """
         success = False
         uri = "fullconfigs/{0}?from={1}&vrf={2}".format(
             config_name, config_file_location, vrf
         )
 
@@ -195,14 +199,15 @@
         return success
 
     def copy_switch_config_to_remote_location(
         self, config_name, config_type, destination, vrf
     ):
         """
         Copy TFTP switch config to TFTP server using a PUT request.
+
         :param config_name:  String with the config file or checkpoint to be
             downloaded. When using TFTP only 'running-config' or
             'startup-config' can be used.
         :param config_type: Configuration type to be downloaded, JSON or CLI
             version of the config. 'json' or 'cli'.
         :param destination: TFTP server address and path for copying
             configuration, must be reachable through provided vrf.
@@ -231,26 +236,27 @@
         vrf=None,
         config_type="json",
         remote_file_tftp_path=None,
     ):
         """
         Obtains the switch's full config in json format and saves it to
             a local file or a remote location over TFTP.
+
         :param config_name:  String with the config file or checkpoint to be
             downloaded. When using TFTP only 'running-config' or
             'startup-config' can be used.
         :param output_file: String with the File name and path for locally
             downloading configuration, only JSON version of configuration will
             be downloaded.
         :param vrf: VRF to be used to contact TFTP server.
         :param config_type: Configuration type to be downloaded, JSON or CLI
             version of the config. 'json' or 'cli'. Defaults to 'json'.
         :param remote_file_tftp_path: TFTP server address and path for
             copying off configuration, must be reachable through provided vrf.
-        :return bool: True if success.
+        :return: True if success.
         """
         success = False
 
         if remote_file_tftp_path is not None:
             tftp_path = remote_file_tftp_path
             if vrf is None:
                 raise VerificationError(
@@ -281,19 +287,20 @@
         # Return result
         return success
 
     def create_checkpoint(self, source_config, destination_config):
         """
         Perform a PUT request to create a new checkpoint or copy an existing
               checkpoint to AOS-CX switch config.
+
         :param source_config: Name of the source configuration from which
             checkpoint needs to be created or copied.
         :param destination_config: Name of the destination configuration or
             name of checkpoint.
-        :return bool: True if success.
+        :return: True if success.
         """
         success = False
 
         source_url = "{0}fullconfigs/{1}".format(
             self.session.resource_prefix, source_config
         )
         uri = "fullconfigs/{0}?from={1}".format(
@@ -313,19 +320,20 @@
 
         # Return result
         return success
 
     def setup_mgmt_nameservers_dns(self, primary=None, secondary=None):
         """
         Setup primary and secondary name servers on a mgmt interface.
+
         :param primary: Primary nameservers on mgmt interface, a IPv4 address.
             Example: "10.10.2.10".
         :param secondary: Secondary nameservers on mgmt interface,
             a IP address. Example: "10.10.2.10".
-        :return modified: Return True if coinfig was modified.
+        :return: Return True if coinfig was modified.
         """
         if "mode" in self.mgmt_intf:
             mgmt_if_mode = self.mgmt_intf["mode"]
         else:
             mgmt_if_mode = "dhcp"
 
         if mgmt_if_mode != "static":
@@ -339,15 +347,16 @@
             self.mgmt_intf["dns_server_2"] = secondary
 
         return self.apply()
 
     def delete_mgmt_nameservers_dns(self):
         """
         Delete primary and secondary name servers on a mgmt interface.
-        :return modified: Return True if coinfig was modified.
+
+        :return: Return True if coinfig was modified.
         """
         if "dns_server_1" in self.mgmt_intf:
             self.mgmt_intf.pop("dns_server_1")
 
         if "dns_server_2" in self.mgmt_intf:
             self.mgmt_intf.pop("dns_server_2")
 
@@ -359,29 +368,30 @@
         config_file=None,
         config_json=None,
         vrf=None,
         remote_file_tftp_path=None,
     ):
         """
         Uploads configuration from a configuration file.
+
         :param config_name:  String with the Config file or checkpoint to be
             uploaded to. When using TFTP only 'running-config' or
             'startup-config' can be used. Defaults to None.
         :param config_file: File name for locally downloading configuration,
             only JSON version of configuration will be downloaded. Defaults to
             None.
         :param config_json: String with the JSON file name and path for locally
             uploading configuration, only JSON version of configuration can be
             uploaded. Defaults to None.
         :param vrf: String for VRF to be used to contact TFTP server, required
             if remote_output_file_tftp_path is provided. Defaults to None.
         :param remote_file_tftp_path: String for TFTP server address and path
             for copying off configuration, must be reachable through provided
             vrf. Defaults to None.
-        :return success: Return boolean True if response is successful.
+        :return: Return boolean True if response is successful.
         """
         success = False
 
         if remote_file_tftp_path is not None:
             if vrf is None:
                 raise VerificationError(
                     "Upload Config",
@@ -411,24 +421,25 @@
         return success
 
     def upload_switch_config_from_local(
         self, config_json=None, config_file=None, config_name=None
     ):
         """
         Uploads configuration from a configuration file.
+
         :param config_name:  String with the Config file or checkpoint
             to be uploaded to. When using TFTP only 'running-config' or
             'startup-config' can be used. Defaults to None.
         :param config_file: String with the File name and path for
             locally downloading configuration, only JSON version of
             configuration will be downloaded. Defaults to None.
         :param config_json: String with the JSON file name and path for
             locally uploading configuration, only JSON version of
             configuration can be uploaded. Defaults to None.
-        :return success: Return boolean True if response is successful.
+        :return: Return boolean True if response is successful.
         """
         success = False
 
         if config_json:
             with open(config_json) as json_file:
                 config_json = json.load(json_file)
```

### Comparing `pyaoscx-2.3.1/pyaoscx/device.py` & `pyaoscx-2.4.0/pyaoscx/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 from copy import deepcopy
 
 import logging
 import json
 from urllib.parse import quote_plus
@@ -190,52 +190,79 @@
         # Create class attributes using util.create_attrs
         utils.create_attrs(self, data_subsystems)
 
     @PyaoscxModule.connected
     def get_firmware_version(self):
         """
         Perform a GET call to retrieve device firmware version.
-        :return: firmware_version: The firmware version.
+
+        :return: The firmware version.
         """
         data = self.get_firmware_info()
         self.firmware_version = data["current_version"]
         # Return Version
         return self.firmware_version
 
     @PyaoscxModule.connected
     def get_firmware_info(self):
         """
         Perform a GET call to retrieve device firmware information.
-        :return: firmware_info: The versions of current, primary and
+
+        :return: The versions of current, primary and
             secondary images.
         """
         try:
             response = self.session.request("GET", "firmware")
 
         except Exception as e:
             raise ResponseError("GET", e)
 
         if not utils._response_ok(response, "GET"):
             raise GenericOperationError(response.text, response.status_code)
 
         firmware_info = json.loads(response.text)
         return firmware_info
 
+    @PyaoscxModule.connected
+    def get_firmware_status(self):
+        """
+        Perform a GET call to retrieve device firmware status.
+
+        :return: firmware_status: The date, reason and status of the firmware
+            upload.
+        """
+        uri = "firmware/status"
+
+        try:
+            # Try to perform a GET call and retrieve the data
+            response = self.session.request("GET", uri)
+
+        except Exception as e:
+            raise ResponseError("GET", e)
+
+        if not utils._response_ok(response, "GET"):
+            raise GenericOperationError(response.text, response.status_code)
+
+        firmware_status = json.loads(response.text)
+        return firmware_status
+
     @PyaoscxModule.materialized
     def apply(self):
         """
         Main method to update an existing Device object.
+
         :return modified: Boolean, True if object was created or modified.
         """
         return self.update()
 
     @PyaoscxModule.materialized
     def update(self):
         """
         Perform a PUT call to apply changes to a Device object.
+
         :return modified: Boolean, True if object was created or modified.
         """
         if not self.modified:
             return False
 
         device_data = utils.get_attrs(self, self.config_attrs)
         put_data = json.dumps(device_data)
@@ -256,17 +283,18 @@
     ####################################################################
     # IMPERATIVE FUNCTIONS
     ####################################################################
 
     def update_banner(self, banner_info, banner_type="banner"):
         """
         Perform a PUT request to modify a Device's Banner.
+
         :param banner_info: String to be configured as the banner.
-        :param banner_type: Type of banner being configured on the switch.
-            Either banner or banner_exec.
+        :param banner_type: Type of banner being configured on the switch
+            either banner or banner_exec.
         :return modified: Returns True if Banner was modified.
         """
         modified = False
 
         logging.info("Setting Banner")
         depth = self.session.api.default_depth
 
@@ -320,16 +348,17 @@
             modified = True
 
         return modified
 
     def delete_banner(self, banner_type="banner"):
         """
         Perform a DELETE request to delete a device's Banner.
-        :param banner_type: Type of banner being removed on the switch.
-            Either banner or banner_exec.
+
+        :param banner_type: Type of banner being removed on the switch
+            either banner or banner_exec.
         :return modified: Returns True if Banner was modified.
         """
         logging.info("Removing Banner")
         depth = self.session.api.default_depth
 
         # Second GET request to obtain just the variables that are writable
         selector = self.session.api.default_selector
@@ -376,14 +405,15 @@
 
         return modified
 
     def boot_firmware(self, partition_name="primary"):
         """
         Perform a POST request to Boot the AOS-CX switch with image present
             to the specified partition.
+
         :param partition_name: Name of the partition for device to boot to.
         :return bool: True if success.
         """
         # Lower case for partition name
         partition_name = partition_name.lower()
         if partition_name not in ["primary", "secondary"]:
             raise VerificationError("Boot Firmware", "Bad partition name")
@@ -403,14 +433,15 @@
         return success
 
     def upload_firmware_http(
         self, remote_firmware_file_path, vrf, partition_name="primary"
     ):
         """
         Perform a PUT request to upload a firmware image given a http_request.
+
         :param remote_firmware_file_path: "HTTP server address and path for
             uploading firmware image, must be reachable through provided vrf
             ex: http://192.168.1.2:8000/TL_10_04_0030A.swi".
         :param vrf: VRF to be used to contact HTTP server, required if
             remote_firmware_file_path is provided.
         :param partition_name: Name of the partition for the image to be
             uploaded to.
@@ -450,57 +481,77 @@
         # PUT for a HTTP Request
         try:
             response = self.session.request("PUT", uri)
 
         except Exception as e:
             raise ResponseError("PUT", e)
 
-        if not utils._response_ok(response, "PUT"):
+        if (
+            not utils._response_ok(response, "PUT")
+            and response.status_code != 400
+        ):
+            # In this case, status code 400 is a valid state
+            # PUT often returns "400: Firmware upgrade in progress"
             raise GenericOperationError(response.text, response.status_code)
 
         # True if successful
         return True
 
     def upload_firmware_local(
-        self, partition_name="primary", firmware_file_path=None
+        self,
+        partition_name="primary",
+        firmware_file_path=None,
+        try_pycurl=False,
     ):
         """
         Perform a POST request to upload a firmware image from a local file.
+
         :param partition_name: Name of the partition for the image to be
             uploaded to.
         :param firmware_file_path: File name and path for local file uploading
             firmware image.
+        :param try_pycurl: If True the function will try to use pycurl instead
+            of requests.
         :return success: True if success.
         """
         uri = "firmware?image={0}".format(partition_name)
 
-        success = utils.file_upload(self.session, firmware_file_path, uri)
+        success = utils.file_upload(
+            self.session,
+            firmware_file_path,
+            self.session._build_uri(uri),
+            try_pycurl,
+        )
         # If no errors detected
         return success
 
     def upload_firmware(
         self,
         partition_name=None,
         firmware_file_path=None,
         remote_firmware_file_path=None,
         vrf=None,
+        try_pycurl=False,
     ):
         """
         Upload a firmware image from a local file OR from a remote location.
+
         :param partition_name: Name of the partition for the image to be
             uploaded to.
         :param firmware_file_path: File name and path for local file uploading
             firmware image.
             IMPORTANT: For this to be used, the remote_firmware_file_path
             parameter must be None.
         :param remote_firmware_file_path: HTTP server address and path for
             uploading firmware image, must be reachable through provided vrf
             ex: 'http://192.168.1.2:8000/TL_10_04_0030A.swi'.
         :param vrf: VRF to be used to contact HTTP server, required if
             remote_firmware_file_path is provided.
+        :param try_pycurl: If True the function will try to use pycurl instead
+            of requests.
         :return bool: True if success.
         """
         result = None
         if partition_name is None:
             partition_name = "primary"
 
         # Use HTTP Server
@@ -508,30 +559,32 @@
             result = self.upload_firmware_http(
                 remote_firmware_file_path, vrf, partition_name
             )
 
         # Locally
         else:
             result = self.upload_firmware_local(
-                partition_name, firmware_file_path
+                partition_name, firmware_file_path, try_pycurl
             )
 
         # If no errors detected
         return result
 
     def vsx_capable(self):
         """
         Return whether this device supports the VSX functionality.
+
         :return: True if device supports VSX.
         """
         return hasattr(self, "capabilities") and "vsx" in self.capabilities
 
     def is_capable(self, capability):
         """
         Check if the current Device has the given capability.
+
         :param capability: String name of a Device capability.
         :return: True if Device is capable.
         """
         if not self.materialized:
             self.get()
 
         return capability in self.capabilities
```

### Comparing `pyaoscx-2.3.1/pyaoscx/dhcp_relay.py` & `pyaoscx-2.4.0/pyaoscx/dhcp_relay.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 import re
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
@@ -42,14 +42,15 @@
         self.__modified = False
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a DHCP Relay table entry and
             fill the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if there is not an exception raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -115,14 +116,15 @@
         return True
 
     @classmethod
     def get_all(cls, session):
         """
         Perform a GET call to retrieve all system DHCP Relays, and create a
             dictionary containing them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :return: Dictionary containing DHCP Relays IDs as keys and a DHCP Relay
             objects as values.
         """
         logging.info("Retrieving all %s data from switch", cls.__name__)
@@ -151,30 +153,32 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update an existing DHCP Relay.
             Checks whether the DHCP Relay exists in the switch. Calls
             self.update() if DHCP Relay is being updated. Calls self.create()
             if a new DHCP Relay is being created.
-        :return modified: Boolean, True if object was created or modified.
+
+        :return: Boolean, True if object was created or modified.
         """
         modified = False
         if self.materialized:
             modified = self.update()
         else:
             modified = self.create()
         # Set internal attribute
         self.__modified = modified
         return modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing DHCP Relay.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         # Variable returned
         modified = False
 
         dhcp_relay_data = utils.get_attrs(self, self.config_attrs)
 
@@ -214,15 +218,16 @@
         return modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new DHCP Relay. Only returns if no
             exception is raised.
-        :return modified: Boolean, True if entry was created.
+
+        :return: Boolean, True if entry was created.
         """
         dhcp_relay_data = utils.get_attrs(self, self.config_attrs)
         dhcp_relay_data["vrf"] = self.vrf.get_info_format()
         dhcp_relay_data["port"] = self.port.get_info_format()
 
         post_data = json.dumps(dhcp_relay_data)
 
@@ -271,22 +276,23 @@
         # Delete object attributes
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, response_data):
         """
         Create a DhcpRelay object given a response_data.
+
         :param cls: Class calling the method.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param response_data: The response must be a dictionary of the form:
             {
-                {vrf},{port}: "/rest/v10.04/system/dhcp_relays/{vrf},{port}"
+            {vrf},{port}: "/rest/v10.04/system/dhcp_relays/{vrf},{port}"
             }
-        return: DhcpRelay object.
+        :return: DhcpRelay object.
         """
         dhcp_relay_arr = session.api.get_keys(
             response_data, DhcpRelay.resource_uri_name
         )
         port_name = dhcp_relay_arr[1]
         vrf_name = dhcp_relay_arr[0]
         # Create Modules
@@ -295,19 +301,20 @@
 
         return DhcpRelay(session, vrf_obj, port_obj)
 
     @classmethod
     def from_uri(cls, session, uri):
         """
         Create a DHCP Relay object given a URI.
+
         :param cls: Class calling the method.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param uri: a String with a URI.
-        :return indices, dhcp_relay: tuple containing both the indices and
+        :return: tuple containing both the indices and
             DhcpRelay object.
         """
         # Obtain ID from URI
         index_pattern = re.compile(
             r"(.*)dhcp_relays/(?P<index1>.+)/(?P<index2>.+)"
         )
         vrf = index_pattern.match(uri).group("index1")
@@ -325,15 +332,16 @@
     def __str__(self):
         return "DhcpRelay vrf:{0}, port:{1}".format(self.vrf, self.port.name)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific DhcpRelay URI.
-        return: Object's URI.
+
+        :return: Object's URI.
         """
         if self._uri is None:
             self._uri = "{0}{1}/{2}{3}{4}".format(
                 self.session.resource_prefix,
                 DhcpRelay.base_uri,
                 self.vrf.name,
                 self.session.api.compound_index_separator,
@@ -343,63 +351,70 @@
         return self._uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
-        return: Object format depending on the API Version.
+
+        :return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     @property
     def modified(self):
         """
         Return boolean with whether this object has been modified
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     ####################################################################
     # IMPERATIVE FUNCTIONS
     ####################################################################
 
     def add_ipv4_addresses(self, ipv4_list):
         """
         Perform a PUT calls to modify an existing DhcpRelay. Adding a list of
             IPv4 addresses into IPv4_ucast_server
+
         :param ipv4_list: List of IPv4 addresses. Example: ['1.1.1.1',
             '2.2.2.2']
         :return: True if object was changed.
         """
         # Set IPv4
         if ipv4_list is not None and ipv4_list != []:
-            for i in range(len(ipv4_list)):
-                if ipv4_list[i] not in self.ipv4_ucast_server:
-                    self.ipv4_ucast_server.append(ipv4_list[i])
-
+            for ipv4 in ipv4_list:
+                if ipv4 not in self.ipv4_ucast_server:
+                    self.ipv4_ucast_server.append(ipv4)
+            if "ipv4_ucast_server" not in self.config_attrs:
+                self.config_attrs.append("ipv4_ucast_server")
         # Apply changes inside switch
         return self.apply()
 
     def add_ipv6_addresses(self, ipv6_list):
         """
         Perform a PUT calls to modify an existing DhcpRelay. Adding a list of
             IPv6 addresses into IPv6_ucast_server.
+
         :param ipv6_list: List of IPv6 addresses. Example:
             ['2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff']
         :return: True if object was changed.
         """
         # Set IPv6
         if ipv6_list is not None and ipv6_list != []:
-            for i in range(len(ipv6_list)):
-                if ipv6_list[i] not in self.ipv6_ucast_server:
-                    self.ipv6_ucast_server.append(ipv6_list[i])
+            for ipv6 in ipv6_list:
+                if ipv6 not in self.ipv6_ucast_server:
+                    self.ipv6_ucast_server.append(ipv6)
+            if "ipv6_ucast_server" not in self.config_attrs:
+                self.config_attrs.append("ipv6_ucast_server")
 
         # Apply changes inside switch
         return self.apply()
```

### Comparing `pyaoscx-2.3.1/pyaoscx/dns.py` & `pyaoscx-2.4.0/pyaoscx/dns.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         self.__internal_vrf.get()
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a DNS inside the VRF table
             entry and fill the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if there is not an exception raised.
         """
         # Get VRF
@@ -113,29 +114,31 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create a new DNS or update an existing DNS,
             configuring it inside the Vrf object. Checks whether the DNS exists
             in the switch. Calls self.update() if DNS configuration is being
             updated.
-        :return modified: Boolean, True if object was created or modified.
+
+        :return: Boolean, True if object was created or modified.
         """
         modified = False
         # Apply changes
         modified = self.update()
 
         # Set internal attribute
         self.__modified = modified
         return modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing DNS.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         # Variable returned
         modified = False
 
         # Obtain variables
         self.__internal_vrf.dns_domain_name = self.dns_domain_name
@@ -212,41 +215,44 @@
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     ####################################################################
     # IMPERATIVE FUNCTIONS
     ####################################################################
 
     def setup_mgmt_nameservers(self, primary=None, secondary=None):
         """
         Setup primary and secondary name servers on a mgmt interface.
+
         :param primary: Primary nameservers on mgmt interface, a IPv4 address.
             Example: '10.10.2.10'.
         :param secondary: Secondary nameservers on mgmt interface,
             a IP address. Example: '10.10.2.10'.
-        :return modified: Return True if coinfig was modified.
+        :return: Return True if coinfig was modified.
         """
         # Create configuration Object
         config = Configuration()
 
         # Return if configuration was modified
         return config.setup_mgmt_nameservers_dns(primary, secondary)
 
     def delete_mgmt_nameservers(self):
         """
         Delete primary and secondary name servers on a mgmt interface.
-        :return modified: Return True if coinfig was modified.
+
+        :return: Return True if coinfig was modified.
         """
         # Create configuration Object
         config = Configuration()
 
         return config.delete_mgmt_nameservers_dns()
 
     def setup_dns(
@@ -255,41 +261,42 @@
         domain_list=None,
         domain_servers=None,
         host_v4_address_mapping=None,
         host_v6_address_mapping=None,
     ):
         """
         Setup DNS client configuration within a Vrf object.
+
         :param domain_name: Domain name used for name resolution by the DNS
             client, if 'dns_domain_list' is not configured.
         :param domain_list: dict of DNS Domain list names to be used for
             address resolution, keyed by the resolution priority order.
             Example:
-                {
-                    0: "hpe.com"
-                    1: "arubanetworks.com"
-                }
+            {
+            0: "hpe.com"
+            1: "arubanetworks.com"
+            }
         :param domain_servers: dict of DNS Name servers to be used for address
             resolution, keyed by the resolution priority order. Example:
-                {
-                    0: "4.4.4.10"
-                    1: "4.4.4.12"
-                }
+            {
+            0: "4.4.4.10"
+            1: "4.4.4.12"
+            }
         :param host_v4_address_mapping: dict of static host address
             configurations and the IPv4 address associated with them. Example:
-                {
-                    "host1": "5.5.44.5"
-                    "host2": "2.2.44.2"
-                }
+            {
+            "host1": "5.5.44.5"
+            "host2": "2.2.44.2"
+            }
         :param host_v6_address_mapping: dict of static host address
             configurations and the IPv6 address associated with them. Example:
-                {
-                    "host1": "2001:0db8:85a3:0000:0000:8a2e:0370:7334"
-                }
-        :return modified: Returns True if modified.
+            {
+            "host1": "2001:0db8:85a3:0000:0000:8a2e:0370:7334"
+            }
+        :return: Returns True if modified.
         """
         # Update Values
 
         if domain_name is not None:
             self.dns_domain_name = domain_name
 
         if domain_list is not None:
@@ -312,20 +319,21 @@
         domain_list=None,
         domain_servers=None,
         host_v4_address_mapping=None,
         host_v6_address_mapping=None,
     ):
         """
         Delete DNS client configuration within a Vrf object.
+
         :param domain_name: If value is not None, it is deleted.
         :param domain_list: If value is not None, it is deleted.
         :param domain_servers: If value is not None, it is deleted.
         :param host_v4_address_mapping: If value is not None, it is deleted.
         :param host_v6_address_mapping: If value is not None, it is deleted.
-        :return modified: Returns True if modified.
+        :return: Returns True if modified.
         """
         # Update Values
 
         if domain_name is not None:
             self.dns_domain_name = None
 
         if domain_list is not None:
```

### Comparing `pyaoscx-2.3.1/pyaoscx/exceptions/generic_op_error.py` & `pyaoscx-2.4.0/pyaoscx/exceptions/generic_op_error.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.3.1/pyaoscx/exceptions/login_error.py` & `pyaoscx-2.4.0/pyaoscx/exceptions/login_error.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.3.1/pyaoscx/exceptions/response_error.py` & `pyaoscx-2.4.0/pyaoscx/exceptions/response_error.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.3.1/pyaoscx/exceptions/verification_error.py` & `pyaoscx-2.4.0/pyaoscx/exceptions/verification_error.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.3.1/pyaoscx/firmware.py` & `pyaoscx-2.4.0/pyaoscx/firmware.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 from pyaoscx.utils import util as utils
 
 
 def get_firmware_version(**kwargs):
     """
     Perform GET calls to retrieve the current firmware version.
+
     :param kwargs:
-        keyword s: requests.session object with loaded cookie jar
-        keyword url: URL in main() function.
+        keyword "s" requests.session object with loaded cookie jar
+        keyword "url" URL in main() function.
     :return: Firmware version string if found, otherwise None.
     """
     target_url = kwargs["url"] + "firmware"
 
     response = kwargs["s"].get(
         target_url, verify=False, proxies=kwargs["s"].proxies
     )
```

### Comparing `pyaoscx-2.3.1/pyaoscx/interface.py` & `pyaoscx-2.4.0/pyaoscx/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Apache License 2.0
 
 import json
 import logging
 import re
 
 from copy import deepcopy
+from random import randint
 from urllib.parse import quote_plus, unquote_plus
 from warnings import warn
 
 from netaddr import mac_eui48
 from netaddr import EUI as MacAddress
 from netaddr.core import AddrFormatError
 
@@ -80,14 +81,15 @@
         return self.__modified
 
     def __set_name(self, name):
         """
         Set name attribute in the proper form for Interface object. Also sets
             the "percents name"-the name with any special characters replaced
             with percent-encodings.
+
         :param name: Interface name.
         """
         # Add attributes to class
         self.name = None
         self.percents_name = None
 
         if r"%2F" in name or r"%2C" in name or r"%3A" in name:
@@ -124,14 +126,15 @@
         else:
             self.__is_special_type = False
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a Interface table entry.
+
         :param depth: Integer deciding how many levels into the API JSON
             that references will be returned.
         :param selector: Alphanumeric option to select specific
             information to return.
         :return: Returns True if no exception is raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -323,14 +326,15 @@
         return True
 
     @classmethod
     def get_all(cls, session):
         """
         Perform a GET call to retrieve all system Interfaces and create.
         a dictionary containing each Interface as a Interface Object.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :return: Dictionary containing Interface's name as key and a Interface
             objects as values.
         """
         logging.info("Retrieving all %s data from switch", cls.__name__)
@@ -358,14 +362,15 @@
         return interfaces_dict
 
     @classmethod
     def from_response(cls, session, response_data):
         """
         Create an Interface object given a response_data related to the
             Interface object.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param response_data: The response must be a dictionary of the form:
             { "<interface_name>": URL }, with URL:
             "/rest/v10.04/system/interfaces/<interface_name>"
         :return: Interface object.
@@ -376,14 +381,15 @@
         interface_name = interfaces_id_arr[0]
         return session.api.get_module(session, "Interface", interface_name)
 
     @classmethod
     def from_uri(cls, session, uri):
         """
         Create an Interface object given a interface URI.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param uri: a String with a URI.
         :return name, interface_obj: tuple containing both the Interface's name
             and an Interface object.
         """
@@ -398,14 +404,15 @@
 
         return name, interface_obj
 
     @classmethod
     def get_facts(cls, session):
         """
         Perform a GET call to retrieve all Interfaces and their data.
+
         :param cls: Class reference.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :return facts: Dictionary containing Interface IDs as keys and
             Interface objects as values.
         """
         logging.info("Retrieving the switch interfaces facts")
@@ -432,14 +439,15 @@
         return facts
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create an Interface Object. Only returns if no
             exception is raised.
+
         :return True if entry was created inside Device.
         """
         interface_data = utils.get_attrs(self, self.config_attrs)
 
         interface_data["name"] = self.name
         # Set Type
         if self.type is not None:
@@ -468,14 +476,15 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to update or create a Interface or Port table entry.
             Checks whether the Interface exists in the switch. Calls
             self.update() if Interface is being updated. Calls self.create() if
             a Interface table entry is being created.
+
         :return modified: Boolean, True if object was created or modified.
         """
         modified = False
         if self.materialized:
             modified = self.update()
         else:
             modified = self.create()
@@ -516,14 +525,15 @@
         utils.delete_attrs(self, self.config_attrs)
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing Interface or Port
             table entry.
+
         :return modified: True if Object was modified and a PUT request was
             made.
         """
         # Variable returned
         modified = False
 
         # Get interface PUT data depending on the configuration attributes
@@ -678,14 +688,15 @@
             modified = True
         return modified
 
     @PyaoscxModule.connected
     def __add_member_to_lag(self, lag):
         """
         Perform PUT calls to configure a Port as a LAG member, and enable it.
+
         :param lag: pyaoscx.Interface object, to which the current port is
             being assigned to.
         """
         if not lag.materialized:
             raise VerificationError(
                 "LAG {0}".format(lag.name),
                 "Object is not materialized - Perform get()",
@@ -709,14 +720,15 @@
         self.update()
 
     @PyaoscxModule.connected
     def __delete_lag(self, lag):
         """
         Perform PUT calls to update Interface, deleting the LAG reference
             inside of the Port that was assigned to that LAG.
+
         :param lag: pyaoscx.Interface object.
         """
         if not lag.materialized:
             raise VerificationError(
                 "LAG {0}".format(lag.name),
                 "Object is not materialized - Perform get()",
             )
@@ -731,14 +743,15 @@
         # Make a PUT call and update values
         self.update()
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific Interface URI.
+
         return: Object's URI.
         """
         if self._uri is None:
             self._uri = "{0}{1}/{2}".format(
                 self.session.resource_prefix,
                 Interface.base_uri,
                 self.percents_name,
@@ -747,28 +760,31 @@
         return self._uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
+
         return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     def __str__(self):
         """
         String containing the Interface name.
+
         :return: This class' string representation.
         """
         return "Interface Object, name: '{0}'".format(self.name)
 
     def __set_to_default(self):
         """
         Perform a PUT call to set Interface to default settings.
+
         :return: True if object was changed.
         """
         # Check for IPv6 addresses and delete them
         for address in self.ip6_addresses:
             address.delete()
         # Clean Attribute
         self.ip6_addresses = []
@@ -813,27 +829,29 @@
         self.get()
         return True
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     ####################################################################
     # IMPERATIVE FUNCTIONS
     ####################################################################
 
     @PyaoscxModule.materialized
     def configure_mclag_options(self, mc_lag=None, lacp_fallback=None):
         """
         Configure an Interface object, set its LAG attributes. Requires a
             call to apply() afterwards.
+
         :param mc_lag: Boolean to set the LAG as a multi-chassis LAG.
         :param lacp_fallback: Boolean to set the LAG's LACP fallback mode.
         """
         if not self.__is_special_type:
             logging.warning(
                 "Interface is not a LAG Interface, cannot set MCLAG options"
             )
@@ -857,14 +875,15 @@
         vlan_mode="native-untagged",
         trunk_allowed_all=False,
         native_vlan_tag=True,
     ):
         """
         Configure an Interface object, set the attributes to a L2 LAG and
             apply() changes inside Switch.
+
         :param phys_ports: List of physical ports to aggregate (e.g. ["1/1/1",
             "1/1/2", "1/1/3"]) or list of Interface Objects.
         :param ipv4: Optional list of IPv4 address to assign to the interface.
             If more than one is specified, all addresses except for the first
             are added as secondary_ip4. Defaults to nothing if not specified.
             Example: ['1.1.1.1', '2.2.2.2']
         :param vlan_ids_list: Optional list of integer VLAN IDs or VLAN objects
@@ -970,14 +989,15 @@
         fallback_enabled=None,
         mc_lag=None,
     ):
         """
         Configure an Interface object, if not materialized, materialize it and
             then set the attributes to a L3 LAG and apply() changes inside
             Switch.
+
         :param phys_ports: List of physical ports to aggregate (e.g. ["1/1/1",
             "1/1/2", "1/1/3"]) or list of Interface Objects.
         :param ipv4: Optional list of IPv4 address to assign
             to the interface. If more than one is specified, all addresses
             except for the first are added as secondary_ip4. Defaults to
             nothing if not specified. Example: ['1.1.1.1', '2.2.2.2']
         :param ipv6: String list of IPv6 addresses to assign to the interface.
@@ -1078,14 +1098,15 @@
         vrf=None,
         description=None,
         int_type="vlan",
         user_config="up",
     ):
         """
         Configure a Interface table entry for a VLAN.
+
         :param vlan: Numeric ID of VLAN
             A Vlan object is also accepted
         :param ipv4: Optional list of IPv4 address to assign to the interface.
             If more than one is specified, all addresses except for the first
             are added as secondary_ip4. Defaults to nothing if not specified.
             Example: ['1.1.1.1'].
         :param ipv6: String list of IPv6 addresses to assign to the interface.
@@ -1185,14 +1206,15 @@
         return self.apply() or ipv6_configured
 
     @PyaoscxModule.materialized
     def add_ipv4_address(self, ip_address):
         """
         Configure a Interface object to add a new IPv4 address to it and
             calls apply(), applying changes inside Switch.
+
         :param ip_address: IPv4 address to assign to the interface.
             Example: "1.1.1.1"
         :return: True if object was changed.
         """
         # Set incoming IPv4 address
         self.ip4_address = ip_address
 
@@ -1200,14 +1222,15 @@
         return self.apply()
 
     @PyaoscxModule.materialized
     def add_ipv6_address(self, ip_address, address_type="global-unicast"):
         """
         Configure a Interface object to append a IPv6 address to its
             ip6_addresses list and apply changes.
+
         :param ip_address: IPv6 address to assign to the interface.
             A Ipv6 object is also accepted. Example:
             '2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff'
         :param address_type: Type of Address. Defaults to global-unicast.
         :return: Ipv6 object.
         """
         # Verify if incoming address is a string
@@ -1237,14 +1260,15 @@
         self.apply()
 
         return ipv6
 
     def delete_ipv6_address(self, ip_address):
         """
         Given a IPv6 address, delete that address from the current Interface.
+
         :param ip_address: IPv6 address to assign to the interface. A Ipv6
             object is also accepted. Example:
             '2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff'.
         """
         if not self.materialized:
             raise VerificationError(
                 "Interface {0}".format(self.name), "Object not materialized"
@@ -1263,14 +1287,15 @@
 
     def configure_loopback(self, vrf, ipv4=None, description=None):
         """
         Configure an Interface object to create a Loopback Interface for a
             logical L3 Interface. If the Loopback Interface already exists and
             an IPv4 address is given, this function will update the IPv4
             address.
+
         :param vrf: VRF to attach the Loopback to. Defaults to "default"
             if not specified.
         :param ipv4: IPv4 address to assign to the interface. Defaults to
             nothing if not specified. Example: '1.1.1.1'
         :param description: Optional description for the interface. Defaults
             to nothing if not specified..
         :return: True if object was changed.
@@ -1317,14 +1342,15 @@
     def configure_vxlan(
         self, source_ipv4=None, description=None, dest_udp_port=4789
     ):
         """
         Configure VXLAN table entry for a logical L3 Interface. If the VXLAN
             Interface already exists and an IPv4 address is given, the function
             will update the IPv4 address.
+
         :param source_ipv4: Optional source IPv4 address to assign to the VXLAN
             interface. Defaults to nothing if not specified. Example:
             '1.1.1.1'.
         :param description: Optional description for the interface. Defaults
             to nothing if not specified.
         :param dest_udp_port: Optional Destination UDP Port that the VXLAN
             will use. Default is set to 4789.
@@ -1344,14 +1370,15 @@
         # Apply changes
         return self.apply()
 
     def set_vlan_mode(self, vlan_mode):
         """
         Set an L2 interface's VLAN mode. The options are 'native-tagged',
             'native-untagged', or 'access'.
+
         :param vlan_mode: A string, either 'native-tagged', 'native-untagged',
             or 'access', specifying the desired VLAN mode.
         :return: True if object was changed.
         """
         if not self.materialized:
             raise VerificationError(
                 "Interface {0}".format(self.name), "Object not materialized"
@@ -1363,14 +1390,15 @@
 
         # Apply changes
         return self.apply()
 
     def set_untagged_vlan(self, vlan):
         """
         Set the untagged VLAN on an access port.
+
         :param vlan: Numeric ID of VLAN to set on access port. A Vlan object is
             also accepted.
         :return: True if object was changed.
         """
         if not self.materialized:
             raise VerificationError(
                 "Interface {0}".format(self.name), "Object not materialized"
@@ -1396,14 +1424,15 @@
         return self.apply()
 
     def add_vlan_trunks(self, vlan_trunk_ids):
         """
         Add specified VLANs to a trunk port. By default, this will also set
             the port to have 'no routing' and if there is not a native VLAN,
             will set the native VLAN to VLAN 1.
+
         :param vlan_trunk_ids: Dictionary of VLANs to specify
             as allowed on the trunk port.  If empty, the interface
             will allow all VLANs on the trunk.
         :return: True if object was changed.
         """
         # Set vlan Trunks
         if vlan_trunk_ids is not None:
@@ -1432,14 +1461,15 @@
         # Apply Changes
         return self.apply()
 
     def set_native_vlan(self, vlan, tagged=True):
         """
         Set a VLAN to be the native VLAN on the trunk. Also gives the option to
             set the VLAN as tagged.
+
         :param vlan: Numeric ID of VLAN to add to trunk port. A Vlan object is
             also accepted
         :param tagged: Boolean to determine if True, the native VLAN will be
             set as the tagged VLAN. If False, the VLAN will be set as the
             native untagged VLAN. Defaults to True.
         :return: True if object was changed.
         """
@@ -1474,14 +1504,15 @@
 
         # Apply Changes
         return self.apply()
 
     def delete_vlan(self, vlan):
         """
         Delete a VLAN from a trunk port.
+
         :param vlan: Numeric ID of VLAN to delete from the trunk port.
             A Vlan object is also accepted.
         :return: True if successfully deleted.
         """
         # Import VLAN to  identify object type
         from pyaoscx.vlan import Vlan
 
@@ -1502,14 +1533,15 @@
 
         return deleted
 
     def add_port_to_lag(self, interface):
         """
         Configure a Port as a LAG member, and also enable the port. Add port
             to list of interfaces inside Interface object.
+
         :param interface: Alphanumeric name of the interface. A Interface
             object is also accepted.
         :return: True if object was changed.
         """
         # Identify interface variable type
         if isinstance(interface, str):
             # Create Interface Object
@@ -1534,14 +1566,15 @@
         # Apply changes
         return self.apply()
 
     def remove_port_from_lag(self, interface):
         """
         Remove a Port from LAG, and also disable the port. Remove port from
             list of interfaces inside Interface object.
+
         :param interface: Alphanumeric name of the interface. A Interface
             object is also accepted
         :return: True if object was changed.
         """
         if not self.__is_special_type:
             raise VerificationError(
                 "Interface {0}".format(self.name),
@@ -1559,66 +1592,117 @@
             if member.name == interface_name:
                 # Remove interface from Member
                 self.interfaces.remove(member)
 
         # When changes are applied, port is disabled and lacp key changed
         return self.apply()
 
-    def clear_acl(self, acl_type):
+    def clear_acl(self, acl_type, acl_direction):
         """
         Clear an interface's ACL.
+
         :param acl_type: Type of ACL: options are 'aclv4_out', 'aclv4_in',
             'aclv6_in', or 'aclv6_out'.
         :return: True if object was changed.
         """
         if acl_type == "ipv6":
-            self.aclv6_in_cfg = None
-            self.aclv6_in_cfg_version = None
+            if acl_direction == "in":
+                self.aclv6_in_cfg = None
+                self.aclv6_in_cfg_version = None
+            else:
+                self.aclv6_out_cfg = None
+                self.aclv6_out_cfg_version = None
         if acl_type == "ipv4":
-            self.aclv4_in_cfg = None
-            self.aclv4_in_cfg_version = None
+            if acl_direction == "in":
+                self.aclv4_in_cfg = None
+                self.aclv4_in_cfg_version = None
+            else:
+                self.aclv4_out_cfg = None
+                self.aclv4_out_cfg_version = None
         if acl_type == "mac":
-            self.aclmac_in_cfg = None
-            self.aclmac_in_cfg_version = None
+            if acl_direction == "in":
+                self.aclmac_in_cfg = None
+                self.aclmac_in_cfg_version = None
+            else:
+                self.aclmac_out_cfg = None
+                self.aclmac_out_cfg_version = None
 
         # Apply Changes
         return self.apply()
 
     def initialize_interface_entry(self):
         """
         Initialize Interface to its default state.
+
         :return: True if object was changed.
         """
         # Set interface to default settings
         return self.__set_to_default()
 
     @property
     def admin_state(self):
         return self.admin
 
     @admin_state.setter
     def admin_state(self, state):
         """
         Set the admin state. This will power the interface on or off
+
         :param state: new power state, "up" to turn interface on, "down" to
             turn it off.
         """
         self.admin = state
         if (
             "lag" not in self.name
             and hasattr(self, "user_config")
             and isinstance(self.user_config, dict)
         ):
             self.user_config["admin"] = state
 
+    @property
+    def mtu(self):
+        if (
+            "lag" not in self.name
+            and hasattr(self, "user_config")
+            and isinstance(self.user_config, dict)
+        ):
+            if "mtu" in self.user_config:
+                return self.user_config["mtu"]
+            else:
+                # default MTU value
+                return 1500
+        else:
+            raise VerificationError(
+                "Interface {0} has not MTU attribute".format(self.name)
+            )
+
+    @mtu.setter
+    def mtu(self, new_mtu):
+        """
+        Set the MTU value
+
+        :param mtu: new MTU value
+        """
+        if (
+            "lag" not in self.name
+            and hasattr(self, "user_config")
+            and isinstance(self.user_config, dict)
+        ):
+            self.user_config["mtu"] = new_mtu
+        else:
+            raise VerificationError(
+                "Interface {0} has not MTU attribute".format(self.name)
+            )
+
     def configure_vsx(
         self, active_forwarding, vsx_sync, act_gw_mac, act_gw_ip
     ):
         """
         Configure VSX IPv4 settings on a VLAN Interface.
+
         :param active_forwarding: True or False Boolean to set VSX active
             forwarding.
         :param vsx_sync: List of alphanumeric values to enable VSX
             configuration synchronization.  The options are
             any combination of 'active-gateways', 'irdp', and 'policies'. VSX
             Sync is mainly used in the Primary.
         :param act_gw_mac: Alphanumeric value of the Virtual MAC address for
@@ -1643,14 +1727,15 @@
 
         # Apply changes
         return self.apply()
 
     def delete_vsx_configuration(self):
         """
         Delete VSX IPv4 settings on a VLAN Interface.
+
         :return: True if object was changed.
         """
         # Set values
         self.vsx_active_forwarding_enable = False
         self.vsx_sync = []
         self.vsx_virtual_gw_mac_v4 = None
         self.vsx_virtual_ip4 = []
@@ -1660,14 +1745,15 @@
 
     def configure_l3_ipv4_port(
         self, ip_address=None, port_desc=None, vrf="default"
     ):
         """
         Function will enable routing on the port and update the IPv4 address
             if given.
+
         :param ip_address: IPv4 address to assign to the interface. Defaults
             to nothing if not specified. Example: '1.1.1.1'
         :param port_desc: Optional description for the interface. Defaults to
             nothing if not specified.
         :param vrf: Name of the VRF to which the Port belongs. Defaults to
             "default" if not specified.
         :return: True if object was changed.
@@ -1694,14 +1780,15 @@
 
     def update_ospf_interface_authentication(
         self, vrf, auth_type, digest_key, auth_pass
     ):
         """
         Perform PUT calls to update an Interface with OSPF to have
             authentication.
+
         :param vrf: Alphanumeric name of the VRF the OSPF ID belongs to.
         :param auth_type: Alphanumeric type of authentication, chosen between
             'md5', 'null', and 'text'.
         :param digest_key: Integer between 1-255 that functions as the digest
             key for the authentication method.
         :param auth_pass: Alphanumeric text for the authentication password.
             Note that this will be translated to a base64 String in the
@@ -1723,14 +1810,15 @@
         # Apply changes
         return self.apply()
 
     def update_ospf_interface_type(self, vrf, interface_type="pointtopoint"):
         """
         Update the Interface's OSPFv2 type, as well as enable routing on the
             interface.
+
         :param vrf: Alphanumeric name of the VRF the OSPF ID belongs to.
         :param interface_type: Alphanumeric type of OSPF interface.
             The options are 'broadcast', 'loopback', 'nbma', 'none',
             'pointomultipoint', 'pointopoint', and 'virtuallink'. Defaults to
             'pointtopoint'.
         :return: True if object was changed.
         """
@@ -1763,14 +1851,15 @@
 
         # Apply changes
         return self.apply()
 
     def set_active_gateway(self, ip_address, gateway_mac):
         """
         Update Active Gateway of a Interface.
+
         :param ip_address: IPv4 address to assign to the interface. Example:
             '1.1.1.1'.
         :param gateway_mac: Active Gateway MAC address to assign to the
             interface. Example: '01:02:03:04:05:06'.
         :return: True if object was changed.
         """
         # Configure Active Gateaway IP
@@ -1781,14 +1870,15 @@
         # Apply changes
         return self.apply()
 
     @PyaoscxModule.materialized
     def update_interface_qos(self, qos):
         """
         Update QoS attached to this Interface.
+
         :param qos: string to define a QoS to operate on this interface. Use
             None to remove the Qos attached to this interface.
         :return: True if object was changed.
         """
         # Verify argument type and value
         if not isinstance(qos, str) and qos is not None:
             raise ParameterError("ERROR: QoS must be in a string format")
@@ -1798,14 +1888,15 @@
         # Apply changes
         return self.apply()
 
     @PyaoscxModule.materialized
     def update_interface_queue_profile(self, queue_profile):
         """
         Update the Queue Profile for this interface.
+
         :param queue_profile: Queue Profile name for this Interface.
             None is used to remove an existing Queue Profile.
         :return: True if object was changed.
         """
         if queue_profile is not None and not isinstance(queue_profile, str):
             raise ParameterError(
                 "ERROR: queue_profile must be a string or None"
@@ -1817,14 +1908,15 @@
 
     @PyaoscxModule.materialized
     def update_interface_qos_trust_mode(
         self, qos_trust_mode, cos_override=None, dscp_override=None
     ):
         """
         Update the QoS trust mode of this port.
+
         :param qos_trust_mode: string to define the QoS trust mode for the
             interface. It can be either "cos", "dscp" or "none". To set the
             interface to use the global configuration use "global" instead.
         :param cos_override: integer with the COS entry id to associate
             with the interface instead of automatic values. In range [0,7]
         :param dscp_override: integer with the DSCP entry id to associate
             with the interface instead of the automatic values. In the
@@ -1867,20 +1959,21 @@
         return self.apply()
 
     @PyaoscxModule.materialized
     def update_interface_qos_rate(self, qos_rate):
         """
         Update the rate limit values configured for
             broadcast/multicast/unknown unicast traffic.
+
         :param qos_rate: dict of the rate limit values; should have the
             format ['<type of traffic>'] = <value><unit> e.g.
             {
-                'unknown-unicast': '100pps',
-                'broadcast': 200pps,
-                'multicast': '200pps'
+            'unknown-unicast': '100pps',
+            'broadcast': 200pps,
+            'multicast': '200pps'
             }.
         :return: True if object was changed.
         """
         rate_limits = {}
         if qos_rate is not None:
             for traffic_type, rate in qos_rate.items():
                 for idx, char in enumerate(rate):
@@ -1897,91 +1990,97 @@
         # Apply changes
         return self.apply()
 
     def update_acl_in(self, acl_name, list_type):
         """
         Perform GET and PUT calls to apply ACL on an interface. This function
             specifically applies an ACL to Ingress traffic of the interface.
+
         :param acl_name: Alphanumeric String that is the name of the ACL
         :param list_type: Alphanumeric String of IPv4, IPv6 or MAC to specify
             the type of ACL.
         :return: True if object was changed.
         """
         # Create Acl object
         acl_obj = self.session.api.get_module(
             self.session, "ACL", index_id=acl_name, list_type=list_type
         )
         # Get the current version
         acl_obj.get()
 
+        new_cfg_version = randint(-9007199254740991, 9007199254740991)
+
         if list_type == "ipv6":
             self.aclv6_in_cfg = acl_obj
             if (
                 hasattr(self, "aclv6_in_cfg_version")
                 and self.aclv6_in_cfg_version is None
             ):
-                self.aclv6_in_cfg_version = acl_obj.cfg_version
+                self.aclv6_in_cfg_version = new_cfg_version
         elif list_type == "ipv4":
             self.aclv4_in_cfg = acl_obj
             if (
                 hasattr(self, "aclv4_in_cfg_version")
                 and self.aclv4_in_cfg_version is None
             ):
-                self.aclv4_in_cfg_version = acl_obj.cfg_version
+                self.aclv4_in_cfg_version = new_cfg_version
         elif list_type == "mac":
             self.aclmac_in_cfg = acl_obj
             if (
                 hasattr(self, "aclmac_in_cfg_version")
                 and self.aclmac_in_cfg_version is None
             ):
-                self.aclmac_in_cfg_version = acl_obj.cfg_version
+                self.aclmac_in_cfg_version = new_cfg_version
 
         # Apply changes
         return self.apply()
 
     def update_acl_out(self, acl_name, list_type):
         """
         Perform GET and PUT calls to apply ACL on an interface. This function
             specifically applies an ACL to Egress traffic of the interface,
             which must be a routing interface.
+
         :param acl_name: Alphanumeric String that is the name of the ACL.
         :param list_type: Alphanumeric String of IPv4, IPv6 or MAC to specify
             the type of ACL.
         :return: True if object was changed.
         """
         # Create Acl object
         acl_obj = self.session.api.get_module(
             self.session, "ACL", index_id=acl_name, list_type=list_type
         )
         # Get the current version
         acl_obj.get()
 
+        new_cfg_version = randint(-9007199254740991, 9007199254740991)
+
         if list_type == "ipv6":
             self.aclv6_out_cfg = acl_obj
             if (
                 hasattr(self, "aclv6_out_cfg_version")
                 and self.aclv6_out_cfg_version is None
             ):
-                self.aclv6_out_cfg_version = acl_obj.cfg_version
+                self.aclv6_out_cfg_version = new_cfg_version
         elif list_type == "ipv4":
             self.aclv4_out_cfg = acl_obj
             if (
                 hasattr(self, "aclv4_out_cfg_version")
                 and self.aclv4_out_cfg_version is None
             ):
-                self.aclv4_out_cfg_version = acl_obj.cfg_version
+                self.aclv4_out_cfg_version = new_cfg_version
         elif list_type == "mac":
             self.aclmac_out_cfg = acl_obj
             if (
                 hasattr(self, "aclmac_out_cfg_version")
                 and self.aclmac_out_cfg_version is None
             ):
-                self.aclmac_out_cfg_version = acl_obj.cfg_version
+                self.aclmac_out_cfg_version = new_cfg_version
 
-        # Routeing
+        # Routing
         self.routing = True
 
         # Apply changes
         return self.apply()
 
     @PyaoscxModule.materialized
     def port_security_enable(
@@ -1992,14 +2091,15 @@
         allowed_sticky_mac_addr=None,
         violation_action=None,
         violation_recovery_time=None,
         violation_shutdown_recovery_enable=None,
     ):
         """
         Enable port security on an specified Interface.
+
         :param client_limit: Integer with the maximum amount of MAC
             addresses that can connect to the port.
         :param sticky_mac_learning: Boolean, If sticky MAC learning
             should be enabled.
         :param allowed_mac_addr: The list of allowed MAC addresses,
             each MAC address is a string, or a netaddr.EUI object.
         :param allowed_sticky_mac_addr: A dictionary where each key is
@@ -2027,122 +2127,117 @@
         self.port_security["enable"] = True
 
         device = Device(self.session)
         device.get()
         max_clients = device.capacities[
             "port_access_port_security_max_client_limit"
         ]
-        if client_limit is not None and (
-            1 > client_limit or client_limit > max_clients
-        ):
+        if client_limit and (1 > client_limit or client_limit > max_clients):
             raise ParameterError(
                 "Can only authorize 1 to {0} clients".format(max_clients)
             )
 
         if client_limit:
             self.port_security["client_limit"] = client_limit
 
-        if sticky_mac_learning:
+        if sticky_mac_learning is not None:
             self.port_security[
                 "sticky_mac_learning_enable"
             ] = sticky_mac_learning
 
-        # Use netaddr.EUI to verify that all static MAC addresses are valid,
-        # and use a colon (:) character as the separator.  Example: accept
-        # '2C:54:91:88:C9:E3', but not '2C-54-91-88-C9-E3', then re-convert to
-        # string because that is what the API accepts.
         mac_format = mac_eui48
         mac_format.word_sep = ":"
-        _valid_static_macs = []
-        allowed_mac_addr = allowed_mac_addr or []
-        for mac_addr in allowed_mac_addr:
-            try:
-                mac = MacAddress(mac_addr, dialect=mac_format)
-                _valid_static_macs.append(str(mac))
-            except AddrFormatError as exc:
-                raise ParameterError("Invalid static MAC address") from exc
-        self.port_security_static_client_mac_addr = _valid_static_macs
-
-        # Use netaddr.EUI to verify that all static MAC addresses are valid,
-        # and use a colon (:) character as the separator.  Example: accept
-        # '2C:54:91:88:C9:E3', but not '2C-54-91-88-C9-E3', then re-convert to
-        # string because that is what the API accepts.
-        _valid_sticky_macs = {}
-        allowed_sticky_mac_addr = allowed_sticky_mac_addr or {}
-        for mac_address, vlans in allowed_sticky_mac_addr.items():
-            try:
-                mac = MacAddress(mac_address, dialect=mac_format)
-                _valid_sticky_macs[str(mac)] = vlans
-            except AddrFormatError as exc:
-                raise ParameterError("Invalid sticky MAC address") from exc
-
-        # Verify all VLAN IDs are valid numbers
-        for mac_address, vlans in _valid_sticky_macs.items():
-            _valid_vlans = []
-            for vlan in vlans:
+
+        if allowed_mac_addr:
+            sw_static_macs = self.port_security_static_client_mac_addr
+            for mac_addr in allowed_mac_addr:
+                mac_addr = mac_addr.upper()
+                if mac_addr not in sw_static_macs:
+                    try:
+                        mac = MacAddress(mac_addr, dialect=mac_format)
+                        sw_static_macs.append(str(mac))
+                    except AddrFormatError as exc:
+                        raise ParameterError(
+                            "Invalid static MAC address"
+                        ) from exc
+
+        if allowed_sticky_mac_addr:
+            _valid_sticky_macs = {}
+            for mac_address, vlans in allowed_sticky_mac_addr.items():
                 try:
-                    vlan = int(vlan)
-                except ValueError as exc:
-                    raise ParameterError("Invalid sticky MAC VLANs") from exc
-                _valid_vlans.append(vlan)
-
-            __status_int = Interface(self.session, self.name)
-            __status_int.get(selector="status")
-            # NOTE: applied_vlan_tag is NOT in the default get() path, so we
-            # get it as a dictionary here
-            _vlan_tag = None
-            _vlan_tag_present = bool(__status_int.applied_vlan_tag)
-            if _vlan_tag_present:
-                _vlan_tag = int(next(iter(__status_int.applied_vlan_tag)))
-            # NOTE: applied_vlan_trunks is NOT in the default get() path, so we
-            # get it as a dictionary here
-            _vlan_trunks = None
-            _vlan_trunks_present = bool(__status_int.applied_vlan_trunks)
-            if _vlan_trunks_present:
-                _vlan_trunks = sorted(
-                    [int(k) for k in __status_int.applied_vlan_trunks]
-                )
-            if _valid_vlans == [] and _vlan_tag_present:
-                _valid_vlans = [_vlan_tag]
+                    mac = MacAddress(mac_address, dialect=mac_format)
+                    _valid_sticky_macs[str(mac)] = vlans
+                except AddrFormatError as exc:
+                    raise ParameterError("Invalid sticky MAC address") from exc
+
+            # Verify all VLAN IDs are valid numbers
+            sw_sticky_macs = self.port_security_static_sticky_client_mac_addr
+            for mac_address, vlans in _valid_sticky_macs.items():
+                _valid_vlans = []
+                if mac_address in sw_sticky_macs:
+                    _valid_vlans = sw_sticky_macs[mac_address]
+                for vlan in vlans:
+                    try:
+                        vlan = int(vlan)
+                    except ValueError as exc:
+                        raise ParameterError(
+                            "Invalid sticky MAC VLANs"
+                        ) from exc
+                    if vlan not in _valid_vlans:
+                        _valid_vlans.append(vlan)
+
+                __status_int = Interface(self.session, self.name)
+                __status_int.get(selector="status")
+                # NOTE: applied_vlan_tag is NOT in the default get() path, so
+                # we get it as a dictionary here
+                _vlan_tag = None
+                _vlan_tag_present = bool(__status_int.applied_vlan_tag)
+                if _vlan_tag_present:
+                    _vlan_tag = int(next(iter(__status_int.applied_vlan_tag)))
+                # NOTE: applied_vlan_trunks is NOT in the default get() path,
+                # so we get it as a dictionary here
+                _vlan_trunks = None
+                _vlan_trunks_present = bool(__status_int.applied_vlan_trunks)
+                if _vlan_trunks_present:
+                    _vlan_trunks = sorted(
+                        [int(k) for k in __status_int.applied_vlan_trunks]
+                    )
+                if _valid_vlans == [] and _vlan_tag_present:
+                    _valid_vlans = [_vlan_tag]
 
-            if not _vlan_tag_present and not _vlan_trunks_present:
-                raise VerificationError(
-                    "No VLANs are configured in this interface"
-                )
-            for vlan in _valid_vlans:
-                if not (
-                    _vlan_tag_present
-                    and vlan == _vlan_tag
-                    or _vlan_trunks_present
-                    and vlan in _vlan_trunks
-                ):
-                    _err_msg_allowed_vlans = []
-                    if _vlan_tag_present:
-                        _err_msg_allowed_vlans.append(
-                            "vlan_access: {0}".format(_vlan_tag)
-                        )
-                    if _vlan_trunks_present:
-                        _err_msg_allowed_vlans.append(
-                            "vlan_trunks: {0}".format(_vlan_trunks)
-                        )
+                if not _vlan_tag_present and not _vlan_trunks_present:
                     raise VerificationError(
-                        "One or more of {0} VLANs are not configured, the "
-                        "allowed VLANs for this interface are: {1}".format(
-                            _valid_vlans, ", ".join(_err_msg_allowed_vlans)
-                        )
+                        "No VLANs are configured in this interface"
                     )
-                _valid_sticky_macs[mac_address] = _valid_vlans
-        self.port_security_static_sticky_client_mac_addr = _valid_sticky_macs
+                for vlan in _valid_vlans:
+                    if not (
+                        _vlan_tag_present
+                        and vlan == _vlan_tag
+                        or _vlan_trunks_present
+                        and vlan in _vlan_trunks
+                    ):
+                        _err_msg_allowed_vlans = []
+                        if _vlan_tag_present:
+                            _err_msg_allowed_vlans.append(
+                                "vlan_access: {0}".format(_vlan_tag)
+                            )
+                        if _vlan_trunks_present:
+                            _err_msg_allowed_vlans.append(
+                                "vlan_trunks: {0}".format(_vlan_trunks)
+                            )
+                        raise VerificationError(
+                            "One or more of {0} VLANs are not configured, the "
+                            "allowed VLANs for this interface are: {1}".format(
+                                _valid_vlans, ", ".join(_err_msg_allowed_vlans)
+                            )
+                        )
+                    _valid_sticky_macs[mac_address] = _valid_vlans
+            sw_sticky_macs.update(_valid_sticky_macs)
 
         if violation_action:
-            if violation_action == "notify" and violation_recovery_time:
-                raise ParameterError(
-                    "Must not specify recovery time when violation action is "
-                    "'notify'"
-                )
             self.port_access_security_violation["action"] = violation_action
 
         if violation_recovery_time:
             if 10 > violation_recovery_time or violation_recovery_time > 600:
                 raise ParameterError(
                     "violation_recovery_time must be between 10s and 600s"
                 )
@@ -2156,14 +2251,15 @@
             ] = violation_shutdown_recovery_enable
 
         return self.apply()
 
     def port_security_disable(self):
         """
         Disable port security on the specified interface.
+
         :return: True if the object was changed.
         """
         if not self.materialized:
             raise VerificationError(
                 "interface {0}".format(self.name), "Object not materialized"
             )
 
@@ -2182,14 +2278,15 @@
         self,
         autoneg=None,
         speeds=None,
         duplex=None,
     ):
         """
         Configure the Interface speed and duplex mode.
+
         :param speeds: List of allowed Interface speeds.
         :param duplex: "full" for full duplex or "half" for half duplex.
         :param autonegotiation: switch autonegotiation "on" or "off".
         :return: True if object changed.
         """
 
         autoneg = "on" if autoneg else "off"
```

### Comparing `pyaoscx-2.3.1/pyaoscx/ipv6.py` & `pyaoscx-2.4.0/pyaoscx/ipv6.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 import re
 
 from urllib.parse import quote_plus, unquote_plus
@@ -56,15 +56,16 @@
         else:
             self.address = address
             self.reference_address = quote_plus(self.address)
 
     def __set_interface(self, parent_int):
         """
         Set parent interface as an attribute for the Ipv6 object.
-        :param parent_int a Interface object.
+
+        :param parent_int: a Interface object.
         """
         # Set Parent Interface
         self.__parent_int = parent_int
         # Set Name for URI purposes
         self.__parent_int_name = self.__parent_int.percents_name
 
         # Set URI
@@ -74,14 +75,15 @@
         )
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a IPv6 table entry and fill the
             object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if no exception is raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -140,14 +142,15 @@
         return True
 
     @classmethod
     def get_all(cls, session, parent_int):
         """
         Perform a GET call to retrieve all system IPv6 addresses inside an
             Interface, and create a dictionary containing them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_int: parent Interface object where IPv6 is stored
         :return: Dictionary containing IPv6 IDs as keys and a Ipv6 object as
             value.
         """
@@ -204,15 +207,16 @@
         self.__modified = modified
         return modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing IPv6 table entry
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         # Variable returned
         modified = False
 
         ip6_data = utils.get_attrs(self, self.config_attrs)
 
@@ -253,15 +257,16 @@
         return modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new IPv6 using the object's attributes
             as POST body. Only returns if an exception is not raised.
-        :return modified: Boolean, True if entry was created.
+
+        :return: Boolean, True if entry was created.
         """
         ipv6_data = utils.get_attrs(self, self.config_attrs)
         ipv6_data["address"] = self.address
 
         post_data = json.dumps(ipv6_data)
 
         try:
@@ -309,38 +314,40 @@
         # Delete object attributes
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, parent_int, response_data):
         """
         Create a IPv6 object given a response_data related to the IP6 address.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_int: parent Interface object where IPv6 is stored
         :param response_data: The response must be a dictionary of the form:
             {
-                <address>: "/rest/v10.04/interface/ip6_addresses/<address>"
+            <address>: "/rest/v10.04/interface/ip6_addresses/<address>"
             }
         :return: IPv6 object.
         """
         ipv6_arr = session.api.get_keys(response_data, Ipv6.resource_uri_name)
         address = ipv6_arr[0]
         return Ipv6(session, address, parent_int)
 
     @classmethod
     def from_uri(cls, session, parent_int, uri):
         """
         Create a Ipv6 object given a URI.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_int: Parent Interface class where IPv6 is stored.
         :param uri: a String with a URI.
-        :return index, ipv6_obj: tuple containing both the Ipv6 Object and
+        :return: tuple containing both the Ipv6 Object and
             the ipv6's address.
         """
         # Obtain ID from URI
         index_pattern = re.compile(r"(.*)ip6_addresses/(?P<index>.+)")
         index = index_pattern.match(uri).group("index")
 
         # Create Ipv6 object
@@ -351,15 +358,16 @@
     def __str__(self):
         return "IPv6 address {0}".format(self.address)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific IPv6 URI.
-        return: Object's URI.
+
+        :return: Object's URI.
         """
         if self._uri is None:
             self._uri = "{0}{1}/{2}".format(
                 self.session.resource_prefix,
                 self.base_uri,
                 self.reference_address,
             )
@@ -367,15 +375,16 @@
         return self._uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
-        return: Object format depending on the API Version.
+
+        :return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     @property
     def modified(self):
         """
         Return boolean with whether this object has been modified.
```

### Comparing `pyaoscx-2.3.1/pyaoscx/mac.py` & `pyaoscx-2.4.0/pyaoscx/mac.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 import re
 
 from copy import deepcopy
@@ -67,36 +67,27 @@
         self.path = self._mac_path()
 
     def _set_vlan(self, parent_vlan):
         """
         Set parent Vlan object as an attribute for the MAC class. It is a
             private method because the user shouldn't be able to change the
             parent vlan.
+
         :param parent_vlan a Vlan object.
         """
         # Set parent VLAN
         self._parent_vlan = parent_vlan
 
         # Set URI
         self.base_uri = "{0}/{1}/{2}".format(
             self._parent_vlan.base_uri,
             self._parent_vlan.id,
             self.resource_uri_name,
         )
 
-        macs = getattr(self._parent_vlan, self.resource_uri_name)
-        found = False
-        for mac in macs:
-            if mac.mac_address == self.mac_address:
-                found = True
-                # Make list element point to current object
-                mac = self
-        if not found:
-            macs.append(self)
-
     def _mac_path(self):
         """
         Get the path for internal purposes.
         """
         return "{0}/{1}{2}{3}".format(
             self.base_uri,
             self.from_id,
@@ -113,14 +104,15 @@
             )
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a MAC table entry and fill
             the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if no exception is raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -159,46 +151,72 @@
 
         # Sets object as materialized
         # Information is loaded from the Device
         self.materialized = True
         return True
 
     @classmethod
-    def get_all(cls, session, parent_vlan):
+    def get_all(cls, session, parent_vlan=None):
         """
         Perform a GET call to retrieve all system MACs inside a BGP Router, and
             create a dictionary containing them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_vlan: parent bgp_router object where MAC is stored.
         :return: Dictionary containing MACs IDs as keys and a Mac objects as
             values.
         """
         logging.info("Retrieving all %s data from switch", cls.__name__)
 
-        path = "{0}/{1}/{2}".format(
-            parent_vlan.base_uri, parent_vlan.id, cls.resource_uri_name
+        if parent_vlan:
+            vlan_id = parent_vlan.id
+            vlan_base_uri = parent_vlan.base_uri
+        else:
+            # Need to get all MACs from VLANS with just one request
+            # Using wildcards
+            vlan_id = quote_plus("*")
+            Vlan = session.api.get_module_class(session, "Vlan")
+            vlan_base_uri = Vlan.base_uri
+
+        path = "{0}/{1}/{2}?depth=2".format(
+            vlan_base_uri, vlan_id, cls.resource_uri_name
         )
 
         try:
             response = session.request("GET", path)
         except Exception as e:
             raise ResponseError("GET", e)
 
         if not utils._response_ok(response, "GET"):
             raise GenericOperationError(response.text, response.status_code)
 
-        data = json.loads(response.text)
+        # If all vlans are requested, this dictionary is indexed by vlan id,
+        # otherwise that index does not exist
+        _data = json.loads(response.text)
+        if parent_vlan:
+            data = {str(vlan_id): _data}
+        else:
+            data = _data
 
         mac_dict = {}
-        for uri in data.values():
-            # Create a Mac object
-            indices, mac = cls.from_uri(session, parent_vlan, uri)
-            mac_dict[indices] = mac
+        for vlan_id, macs_dict in data.items():
+            for indices, mac in macs_dict.items():
+                # Create a Mac object
+                # Need to create objects manually to avoid requests
+                # as possible, depth=2 gives all data from macs
+                Vlan = session.api.get_module_class(session, "Vlan")
+                _parent_vlan = Vlan(session, vlan_id=vlan_id)
+                mac_obj = cls(
+                    session, mac["from"], mac["mac_addr"], _parent_vlan
+                )
+                Interface = session.api.get_module_class(session, "Interface")
+                mac_obj.port = Interface.from_response(session, mac["port"])
+                mac_dict[indices] = mac_obj
 
         return mac_dict
 
     @PyaoscxModule.connected
     def apply(self):
         """
         Not applicable for MAC.
@@ -230,21 +248,22 @@
         """
         pass
 
     @classmethod
     def from_response(cls, session, parent_vlan, response_data):
         """
         Create a Mac object given a response_data related to the MAC ID object.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_vlan: parent VLAN class where MAC is stored.
         :param response_data: The response must be a dictionary of the form:
             {
-                "<id1>,<id2>": "/rest/v10.04/system/vlans/id/macs/id1,id2"
+            "<id1>,<id2>": "/rest/v10.04/system/vlans/id/macs/id1,id2"
             }
         :return: Mac object.
         """
         mac_format = mac_eui48
         mac_format.word_sep = ":"
         mac_pair = session.api.get_keys(response_data, cls.resource_uri_name)
         mac_addr = mac_pair[1]
@@ -256,14 +275,15 @@
 
         return cls(session, from_id, mac_address, parent_vlan)
 
     @classmethod
     def from_uri(cls, session, parent_vlan, uri):
         """
         Create a Mac object.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_vlan: parent VLAN class where MAC is stored.
         :param uri: a String with a URI.
         :return indices, mac: tuple containing both the Mac object and
             the MAC' ID.
         """
@@ -288,25 +308,27 @@
 
     def __str__(self):
         return str(self.mac_address)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
-        Method used to obtain the specific MAC URI.
+        Method used to obtain the specific MAC URI
+
         return: Object's URI.
         """
         # TODO: remove this method in favor of uri_path once all
         # modules have been translated to the 'properties' style
         return self.uri_path
 
     @property
     def uri_path(self):
         """
         Method used to obtain the specific MAC URI.
+
         return: Object's URI.
         """
         if self._uri is None:
             self._uri = "{0}{1}/{2}{3}{4}".format(
                 self.session.resource_prefix,
                 self.base_uri,
                 self.from_id,
@@ -317,25 +339,27 @@
         return self._uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
+
         return: Object format depending on the API Version.
         """
         # TODO: remove in favor of info_format when all modules are translated
         # to 'properties' style
         return self.info_format
 
     @property
     def info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
+
         return: Object format depending on the API Version
         """
         return self.session.api.get_index(self)
 
     @property
     def modified(self):
         """
@@ -343,25 +367,27 @@
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute
+
         :return: Boolean. True if the object was recently modified.
         """
         return self.modified
 
     ####################################################################
     # IMPERATIVE FUNCTIONS
     ####################################################################
 
     def get_info(self):
         """
         Perform a GET call to retrieve data for a MAC table entry and return
             info as a dictionary. Do not apply the configuration.
+
         :return info_dict: Returns a dictionary containing the current MAC
             Address information.
         """
         logging.info("Retrieving the switch MAC info")
 
         return self._get_data(None, None)
```

### Comparing `pyaoscx-2.3.1/pyaoscx/ospf_area.py` & `pyaoscx-2.4.0/pyaoscx/ospf_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
 from pyaoscx.exceptions.response_error import ResponseError
@@ -63,14 +63,15 @@
         return self.__modified
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a OSPF Area and fill the object
             with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if there is no exception raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -105,14 +106,15 @@
         return True
 
     @classmethod
     def get_all(cls, session, parent_ospf_router):
         """
         Perform a GET call to retrieve all system OSPF Area inside a OPSF
             Router, and create a dictionary containing them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_ospf_router: parent OPSF Router object where OPSF Area
             is stored.
         :return: Dictionary containing OSPF Area IDs as keys and a OSPF Area
             objects as values.
@@ -143,27 +145,29 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update an existing Ospf Area.
             Checks whether the OSPF Area exists in the switch. Calls
             self.update() if OSPF Area is being updated. Calls self.create() if
             a new OSPF Area is being created.
-        :return modified: Boolean, True if object was created or modified.
+
+        :return: Boolean, True if object was created or modified.
         """
         if not self.__parent_ospf_router.materialized:
             self.__parent_ospf_router.apply()
         if self.materialized:
             return self.update()
         return self.create()
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing OSPF Area.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         # IMPORTANT: OSPF Area's ipsec_ah, ipsec_esp, and other_config MUST be
         # configured together, so if any of them needs to be updated, existing
         # values MUST be sent for all other attributes that have not changed
         # NOTE: 'other_config' is mistakenly not getting added to
         # self.config_attrs, so this is fixed here
@@ -174,15 +178,16 @@
         return self.__modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new OSPF Area. Only returns if an
             exception is not raised.
-        :return modified: Boolean, True if entry was created.
+
+        :return: Boolean, True if entry was created.
         """
         post_data = utils.get_attrs(self, self.config_attrs)
         post_data["area_id"] = self.area_id
 
         self.__modified = self._post_data(post_data)
         return self.__modified
 
@@ -197,14 +202,15 @@
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, parent_ospf_router, response_data):
         """
         Create an OspfArea object given a response_data related to the ospf
             router ID object
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_ospf_router: parent OspfRouter object where OspfArea
             object is stored.
         :param response_data: The response must be a dictionary of the form:
             { id: URL }, with the URL being of the form:
@@ -217,18 +223,19 @@
         ospf_area_id = ospf_area_arr[0]
         return cls(session, ospf_area_id, parent_ospf_router)
 
     @classmethod
     def from_uri(cls, session, parent_ospf_router, uri):
         """
         Create an OspfArea object given a URI.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param uri: a String with a URI.
-        :return index, ospf_area_obj: tuple containing both the OspfArea object
+        :return: tuple containing both the OspfArea object
             and the OSPF Area's ID.
         """
         # Obtain ID from URI
         # system/vrfs/name/ospf_routers/1/areas/1.1.1.1
         # or
         # system/vrfs/name/ospfv3_routers/1/areas/1.1.1.1
         uri_parts = uri.split("/")
@@ -246,52 +253,57 @@
     def __str__(self):
         return "{0} with area_id {1}".format(type(self).__name__, self.area_id)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific OSPF Area URI.
+
         return: Object's URI.
         """
         return self.path
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
+
         return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     def update_ospf_interfaces(self, new_interface):
         """
         Update references to OSPF Interfaces. If an Interface with the same
             interface_name is found, update the reference to the new interface,
             otherwise, add reference to the new interface.
+
         :param new_interface: Interface to add reference to.
         """
         for interface in self.ospf_interfaces:
             if interface.interface_name == new_interface.interface_name:
                 # Make list element point to current object
                 # See utils.list_attributes.ListDescriptor
                 interface = new_interface
                 return
         self.ospf_interfaces.append(new_interface)
 
     def remove_ospf_interface(self, interface):
         """
         Update references to OSPF Interfaces. If an Interface with the same
             interface_name is found, delete the reference to it.
+
         :param interface: Interface to add reference to.
         """
         for i in self.ospf_interfaces:
             if i.interface_name == interface.interface_name:
                 self.ospf_interfaces.remove(i)
```

### Comparing `pyaoscx-2.3.1/pyaoscx/ospf_interface.py` & `pyaoscx-2.4.0/pyaoscx/ospf_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 
 from urllib.parse import quote_plus, unquote_plus
 
@@ -77,14 +77,15 @@
         self.__port = Interface(self.session, name)
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a OSPF Interfaces table entry
             and fill the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if there is not an exception raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -109,14 +110,15 @@
 
     @classmethod
     def get_all(cls, session, parent_ospf_area):
         """
         Perform a GET call to retrieve all system OSPF Interfaces inside a OSPF
             Area, and create a dictionary containing them as OspfInterface
             objects.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_ospf_area: parent OspfArea object where OspfInterface
             object is stored.
         :return: Dictionary containing OSPF Interface IDs as keys and a
             OspfInterface objects as values.
@@ -147,40 +149,43 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update an existing OSPF Interface.
             Checks whether the OSPF Interface exists in the switch. Calls
             self.update() if OSPF Interface being updated. Calls self.create()
             if a new OSPF Interface is being created.
-        :return modified: Boolean, True if object was created or modified.
+
+        :return: Boolean, True if object was created or modified.
         """
         if not self.__parent_ospf_area.materialized:
             self.__parent_ospf_area.apply()
         if self.materialized:
             return self.update()
         return self.create()
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing OSPF Interface.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         put_data = utils.get_attrs(self, self.config_attrs)
         # Get port uri
         put_data["port"] = self.__port.get_info_format()
         self.__modified = self._put_data(put_data)
         return self.__modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new OSPF Interface table entry. Only
             returns if an exception is not raised.
+
         :return: True if OSPF Interface table entry was added.
         """
         post_data = utils.get_attrs(self, self.config_attrs)
         post_data["port"] = self.__port.get_info_format()
         post_data["interface_name"] = self.interface_name
 
         self.__modified = self._post_data(post_data)
@@ -198,20 +203,21 @@
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, parent_ospf_area, response_data):
         """
         Create a OspfInterface object given a response_data related to the OSPF
             Area ID object.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_ospf_area: parent OspfArea object where OspfInterface
             object is stored.
-        :param response_data: The response must be a dictionary of the form:
+        :param response_data: The response must be a dictionary of the form
             {id: URL}, with the URL being of the form:
             "ospf_routers/<id>/areas/<id>/ospf_interfaces/<interface_name>"
             under the path:
             "/rest/v10.04/system/vrfs/<vrf_name>/"
         :return: OspfInterface object.
         """
         ospf_interface_arr = session.api.get_keys(
@@ -220,18 +226,19 @@
         ospf_interface_name = ospf_interface_arr[0]
         return cls(session, ospf_interface_name, parent_ospf_area)
 
     @classmethod
     def from_uri(cls, session, parent_ospf_area, uri):
         """
         Create a OspfInterface object given a URI.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
-        :return interface_name, ospf_interface_obj: tuple containing both the
+        :return: tuple containing both the
             OspfInterface name, and an OspfInterface object.
         """
         # Obtain ID from URI like:
         # system/vrfs/vrf/ospf_routers/1/areas/1.1.1.1/ospf_interfaces/iface
         interface_name = uri.split("/")[-1]
 
         # Create OspfInterface object
@@ -244,27 +251,30 @@
             type(self).__name__, self.interface_name
         )
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific OSPF Interface uri.
-        return: Object's URI.
+
+        :return: Object's URI.
         """
         return self.path
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
-        return: Object format depending on the API Version.
+
+        :return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
```

### Comparing `pyaoscx-2.3.1/pyaoscx/ospf_router.py` & `pyaoscx-2.4.0/pyaoscx/ospf_router.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
 from pyaoscx.exceptions.response_error import ResponseError
@@ -44,14 +44,20 @@
         utils.set_creation_attrs(self, **kwargs)
         self.passive_interfaces = None
         if kwargs.get("passive_interfaces"):
             self.passive_interfaces = [
                 self.session.api.get_module(self.session, "Interface", i)
                 for i in kwargs["passive_interfaces"]
             ]
+        self.active_interfaces = None
+        if kwargs.get("active_interfaces"):
+            self.active_interfaces = [
+                self.session.api.get_module(self.session, "Interface", i)
+                for i in kwargs["active_interfaces"]
+            ]
         # Use to manage Areas
         self.areas = []
         # Attribute used to know if object was changed recently
         self.__modified = False
         uri_indices = {
             "name": self._parent_vrf.name,
             "version": self.version,
@@ -76,14 +82,15 @@
         return self.__modified
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a OSPF Router table entry and
             fill the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if there is not an exception raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -94,44 +101,45 @@
             del self._original_attributes["areas"]
         # Set original attributes
         if "instance_tag" in self._original_attributes:
             del self._original_attributes["instance_tag"]
         # Sets object as materialized
         # Information is loaded from the Device
         self.materialized = True
-        # Set a list of passive_interfaces as an attribute
-        if self.passive_interfaces:
-            interfaces_list = []
-            # Get all URI elements in the form of a list
-            uri_list = self.session.api.get_uri_from_data(
-                self.passive_interfaces
-            )
-            # gotta use deferred import to avoid cyclical import error
-            from pyaoscx.interface import Interface
-
-            for uri in uri_list:
-                # Create an Interface object
-                _, iface = Interface.from_uri(self.session, uri)
-                # Add interface to list
-                interfaces_list.append(iface)
-            # Set list as Interfaces
-            self.passive_interfaces = interfaces_list
+        # Set a list of passive and/or active_interfaces as an attribute
+        for ospf_interfaces in ["passive_interfaces", "active_interfaces"]:
+            o_intfs = getattr(self, ospf_interfaces)
+            if o_intfs:
+                interfaces_list = []
+                # Get all URI elements in the form of a list
+                uri_list = self.session.api.get_uri_from_data(o_intfs)
+                Interface = self.session.api.get_module_class(
+                    self.session, "Interface"
+                )
+                for uri in uri_list:
+                    # Create an Interface object
+                    _, iface = Interface.from_uri(self.session, uri)
+                    # Add interface to list
+                    interfaces_list.append(iface)
+                # Set list as Interfaces
+                setattr(self, ospf_interfaces, interfaces_list)
         if self.areas == []:
             # Set Areas if any
             # Adds Area to parent OspfRouter
             from pyaoscx.ospf_area import OspfArea
 
             OspfArea.get_all(self.session, self)
         return True
 
     @classmethod
     def get_all(cls, session, parent_vrf):
         """
         Perform a GET call to retrieve all system OSPF Router settings for a
             given VRF, and create a dictionary containing them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_vrf: Vrf object where OspfRouter object is stored.
         :return: Dictionary containing
             (OSPF Router ID, OspfRouter object) (key,value) pairs.
         """
@@ -158,73 +166,89 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create update an existing OSPF Router.
             Checks whether the VRF exists in the switch. Calls self.update() if
             OSPF Router is being updated. Calls self.create() if a new OSPF
             Router is being created.
-        :return modified: Boolean, True if object was created or modified.
+
+        :return: Boolean, True if object was created or modified.
         """
         if not self._parent_vrf.materialized:
             self._parent_vrf.apply()
         if self.materialized:
             return self.update()
         return self.create()
 
-    def __get_passive_interfaces_to_correct_form(self):
+    def __get_interfaces_to_correct_form(self, intf_list):
         """
         Auxiliary method to set passive interfaces to correct form for
             requests.
         """
+        ospf_interfaces = (
+            self.passive_interfaces
+            if intf_list == "passive"
+            else self.active_interfaces
+        )
         formatted_interfaces = {}
-        if self.passive_interfaces is not None:
-            for iface in self.passive_interfaces:
+        if ospf_interfaces is not None:
+            for iface in ospf_interfaces:
                 if isinstance(iface, str):
                     iface = self.session.api.get_module(
                         self.session, "Interface", iface
                     )
                 iface.get()
                 if not iface.materialized:
                     raise VerificationError(
                         "Interface {0}".format(iface.name),
-                        "Object inside passive_interfaces not materialized",
+                        "Object inside {0}_interfaces not materialized".format(
+                            intf_list
+                        ),
                     )
                 formatted_iface = iface.get_info_format()
                 formatted_interfaces.update(formatted_iface)
         return formatted_interfaces
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing OSPF Router.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         ospf_router_data = utils.get_attrs(self, self.config_attrs)
 
-        formatted_ifaces = self.__get_passive_interfaces_to_correct_form()
+        formatted_ifaces = self.__get_interfaces_to_correct_form("passive")
         if formatted_ifaces != {}:
             ospf_router_data["passive_interfaces"] = formatted_ifaces
+        formatted_ifaces = self.__get_interfaces_to_correct_form("active")
+        if formatted_ifaces != {}:
+            ospf_router_data["active_interfaces"] = formatted_ifaces
 
         self.__modified = self._put_data(ospf_router_data)
         return self.__modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new  OSPF Router. Only returns if an
             exception is not raised.
-        :return modified: True if entry was created.
+
+        :return: True if entry was created.
         """
         ospf_router_data = utils.get_attrs(self, self.config_attrs)
         ospf_router_data["instance_tag"] = self.__instance_tag
 
-        formatted_ifaces = self.__get_passive_interfaces_to_correct_form()
+        formatted_ifaces = self.__get_interfaces_to_correct_form("passive")
         if formatted_ifaces != {}:
             ospf_router_data["passive_interfaces"] = formatted_ifaces
+        formatted_ifaces = self.__get_interfaces_to_correct_form("active")
+        if formatted_ifaces != {}:
+            ospf_router_data["active_interfaces"] = formatted_ifaces
 
         self.__modified = self._post_data(ospf_router_data)
         return self.__modified
 
     @PyaoscxModule.connected
     def delete(self):
         """
@@ -235,35 +259,37 @@
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, parent_vrf, response_data):
         """
         Create a OspfRouter object given a response_data related to the
             OspfRouter object.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_vrf: Vrf object where OspfRouter object is stored.
         :param response_data: The response must be a dictionary of the form:
-            {id: URL}, with the URL being of the form:
+            {id: URL}, with the URL being of the form
             "/rest/v10.04/system/vrfs/<name>/ospf_routers/<id>"
         :return: OspfRouter object.
         """
         ospf_arr = session.api.get_keys(response_data, cls.resource_uri_name)
         instance_tag = ospf_arr[0]
         return cls(session, instance_tag, parent_vrf)
 
     @classmethod
     def from_uri(cls, session, parent_vrf, uri):
         """
         Create a OspfRouter object given a URI.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param uri: a String with a URI.
-        :return: tuple(OSPF Instance Tag: int, OSPF Router: OspfRouter).
+        :return: tuple(OSPF Instance Tag, OSPF Router).
         """
         # Obtain ID from URI like:
         # system/vrfs/{name}/ospf{version}_routers/{instance_tag}
         instance_tag = uri.split("/")[-1]
 
         # Create OspfRouter object
         ospf_obj = cls(session, instance_tag, parent_vrf)
@@ -275,53 +301,58 @@
             type(self).__name__, self.instance_tag
         )
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific OSPF Router URI.
+
         return: Object's URI.
         """
         # PyaoscxModule's methods use self.path to store the URI
         return self.path
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
-        return: Object format depending on the API Version.
+
+        :return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     def update_ospf_areas(self, new_area):
         """
         Update references to OSPF Areas. If an Area with the same area_id is
             found, update the reference to the new area, otherwise, add
             reference to the new area.
+
         :param new_area: Area to add reference to.
         """
         for area in self.areas:
             if area.area_id == new_area.area_id:
                 # Make list element point to current object
                 # See utils.list_attributes.ListDescriptor
                 area = new_area
                 return
         self.areas.append(new_area)
 
     def remove_ospf_area(self, area):
         """
         Update references to OSPF Areas. If an Area with the same area_id is
             found, delete the reference to it.
+
         :param new_area: Area to add reference to.
         """
         for area_ in self.areas:
             if area.area_id == area_.area_id:
                 self.areas.remove(area_)
```

### Comparing `pyaoscx-2.3.1/pyaoscx/ospf_virtual_link.py` & `pyaoscx-2.4.0/pyaoscx/ospf_virtual_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,27 +55,29 @@
         Return boolean with whether this object has been modified.
         """
         return self.__modified
 
     def _get_indices(self):
         """
         Get indices to retrieve collection of this object's instances.
+
         :return: a dictionary with each key in the collection_uri, and its
             respective value to perform a GET request, or empty dictionary
             if the collection_uri has no indices.
         """
         indices = {"area_id": self.__parent_ospf_area.area_id}
         indices.update(self.__parent_ospf_area._get_indices())
         return indices
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET request to retrieve data for an OSPF VLink table entry
             and fill the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if there is not an exception raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -96,14 +98,15 @@
         return True
 
     @classmethod
     def get_all(cls, session, parent_ospf_area):
         """
         Perform a GET request to retrieve all system OSPF Virtual Links inside
             a OPSF Router, and create a dictionary containing them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_ospf_area: parent OPSF Area object where OPSF VLink
             is stored.
         :return: Dictionary containing OSPF Virtual Link IDs as keys and a OSPF
             Virtual Link objects as values.
@@ -133,42 +136,45 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update an existing Ospf Virtual
             Link. Checks whether the OSPF Virtual Link exists in the switch.
             Calls self.update() if OSPF Virtual Link is being updated. Calls
             self.create() if a new OSPF Virtual Link is being created.
-        :return modified: Boolean, True if object was created or modified.
+
+        :return: Boolean, True if object was created or modified.
         """
         if not self.__parent_ospf_area.materialized:
             self.__parent_ospf_area.apply()
 
         if self.materialized:
             self.__modified = self.update()
         else:
             self.__modified = self.create()
         return self.__modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT request to apply changes to an existing OSPF VLink.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         ospf_vlink_data = utils.get_attrs(self, self.config_attrs)
         self.__modified = self._put_data(ospf_vlink_data)
         return self.__modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST request to create a new OSPF Virtual Link. Only returns
             if an exception is not raised.
-        :return modified: Boolean, True if object was created.
+
+        :return: Boolean, True if object was created.
         """
         ospf_vlink_data = utils.get_attrs(self, self.config_attrs)
         ospf_vlink_data["peer_router_id"] = self.__peer_router_id
 
         self.__modified = self._post_data(ospf_vlink_data)
         return self.__modified
 
@@ -180,20 +186,21 @@
         self._send_data(self.path, None, "DELETE", "Delete")
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_uri(cls, session, uri, parent_ospf_area=None):
         """
         Create an OspfVlink object given a URI.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_ospf_area: parent OspfArea object where OspfVlink object
             is stored.
         :param uri: an OSPF VLink URI with its index (a peer_router_id).
-        :return peer_router_id, ospf_vlink: tuple with the OspfVlink ID, and
+        :return: tuple with the OspfVlink ID, and
             the object.
         """
         if parent_ospf_area is None:
             raise ParameterError(
                 "{0} requires parent_ospf_area instance".format(cls.__name__)
             )
         # Obtain ID from URI of the form '.../ospf_vlinks/{peer_router_id}'
@@ -203,28 +210,31 @@
 
     def __str__(self):
         return "OSPF Virtual Link ID {0}".format(self.__peer_router_id)
 
     def get_uri(self):
         """
         Method used to obtain the specific OSPF Virtual Link URI.
-        return: Object's URI.
+
+        :return: Object's URI.
         """
         # PyaoscxModule uses the uri with the name self.path
         # so it needs to have that name
         return self.path
 
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
-        return: Object format depending on the API Version.
+
+        :return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
```

### Comparing `pyaoscx-2.3.1/pyaoscx/poe_interface.py` & `pyaoscx-2.4.0/pyaoscx/poe_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2021-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2021-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import logging
 
 from pyaoscx.exceptions.verification_error import VerificationError
 from pyaoscx.pyaoscx_module import PyaoscxModule
 from pyaoscx.utils import util as utils
@@ -17,14 +17,15 @@
     object_uri = collection_uri + "/{interface}/poe_interface"
     resource_uri_name = "poe_interface"
     indices = ["name"]
 
     def __init__(self, session, parent_interface, **kwargs):
         """
         Create an instance of PoEInterface Class.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_interface: parent Inferface object where PoE is stored.
         """
         self.session = session
         # List used to determine attributes related to the PoEInterface
         # configuration
@@ -49,14 +50,15 @@
         self.__modified = False
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a PoE Interface table entry and
             fill the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if no exception is raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -67,63 +69,77 @@
         self._get_and_copy_data(depth, selector, self.indices)
         self.materialized = True
         return True
 
     @PyaoscxModule.connected
     def apply(self):
         """
-        Apply an update of values of this PoE Interface.
-        Calls self.update() to apply changes to an existing PoE Interface.
+        Apply an update of values of this PoE Interface. Calls self.update()
+            to apply changes to an existing PoE Interface.
         """
         modified = False
         if self.materialized:
             modified = self.update()
 
         # Set internal attribute
         self.__modified = modified
         return modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing PoE Interface.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         poe_interface_data = utils.get_attrs(self, self.config_attrs)
         poe_interface_data["config"] = self.config.copy()
         self.__modified = self._put_data(poe_interface_data)
         logging.info("SUCCESS: Updating %s", self)
         self.__original_attributes = poe_interface_data
         return self.__modified
 
     @PyaoscxModule.connected
     def create(self):
+        """
+        Not needed for PoEInterface
+        """
         pass
 
     @PyaoscxModule.connected
     def delete(self):
+        """
+        Not needed for PoEInterface
+        """
         pass
 
     @PyaoscxModule.connected
     def get_all(self):
+        """
+        Not needed for PoEInterface
+        """
         pass
 
     @classmethod
     def from_uri(cls):
+        """
+        Not needed for PoEInterface
+        """
         pass
 
     def __str__(self):
         return "PoE Interface {0}".format(self.name)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific PoE Interface URI.
-        return: Object's URI.
+
+        :return: Object URI.
         """
         uri = "{0}{1}".format(self.session.resource_prefix, self.path)
 
         return uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
@@ -136,23 +152,25 @@
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     @property
     @PyaoscxModule.materialized
     def allocate_by_method(self):
         """
         Getter method for the allocate_by_method attribute.
+
         :return: String value for method.
         """
         return self.config["allocate_by_method"]
 
     @allocate_by_method.setter
     @PyaoscxModule.materialized
     def allocate_by_method(self, new_method):
@@ -169,14 +187,15 @@
         self.config["allocate_by_method"] = new_method
 
     @property
     @PyaoscxModule.materialized
     def assigned_class(self):
         """
         Getter method for the cfg_assigned_class attribute.
+
         :return: String value for assigned class.
         """
         return self.config["cfg_assigned_class"]
 
     @assigned_class.setter
     def assigned_class(self, new_class):
         """
@@ -192,14 +211,15 @@
         self.config["cfg_assigned_class"] = new_class
 
     @property
     @PyaoscxModule.materialized
     def priority(self):
         """
         Getter method for the priority attribute.
+
         :return: String value for priority.
         """
         return self.config["priority"]
 
     @priority.setter
     @PyaoscxModule.materialized
     def priority(self, new_priority):
@@ -216,14 +236,15 @@
         self.config["priority"] = new_priority
 
     @property
     @PyaoscxModule.materialized
     def power_enabled(self):
         """
         Getter method for admin_disabled attribute.
+
         :return: Bool value for priority.
         """
         return not self.config["admin_disable"]
 
     @power_enabled.setter
     @PyaoscxModule.materialized
     def power_enabled(self, state):
@@ -233,14 +254,15 @@
         self.config["admin_disable"] = not state
 
     @property
     @PyaoscxModule.materialized
     def pd_class_override(self):
         """
         Getter method for pd_class_override attribute.
+
         :return: Bool value for pd_class_override.
         """
         return self.config["pd_class_override"]
 
     @pd_class_override.setter
     @PyaoscxModule.materialized
     def pd_class_override(self, new_flag):
@@ -250,14 +272,15 @@
         self.config["pd_class_override"] = new_flag
 
     @property
     @PyaoscxModule.materialized
     def pre_standard_detect(self):
         """
         Getter method for pre_standard_detect attribute.
+
         :return: Bool value for pre_standard_detect.
         """
         return self.config["pre_standard_detect"]
 
     @pre_standard_detect.setter
     @PyaoscxModule.materialized
     def pre_standard_detect(self, new_flag):
```

### Comparing `pyaoscx-2.3.1/pyaoscx/pyaoscx_factory.py` & `pyaoscx-2.4.0/pyaoscx/pyaoscx_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,25 +23,25 @@
         return cls.__instance
 
 
 class PyaoscxFactory(metaclass=Singleton):
     """
     Provide a Factory class to instantiate all pyaoscx Modules through specific
         methods. This class is superseded by the Device class, use the Device
-        class instead of this one.
-    Using the API Version given by the Session.
+        class instead of this one. Using the API Version given by the Session.
     """
 
     def __init__(self, session):
         self.session = session
 
     def configuration(self):
         """
         Create a Configuration class, to obtain device configuration and
             perform other actions such as backup_config.
+
         :return: Configuration object.
         """
         config = Configuration(self.session)
         # Get full configuration
         config.get()
         return config
 
@@ -52,41 +52,42 @@
         domain_list=None,
         domain_servers=None,
         host_v4_address_mapping=None,
         host_v6_address_mapping=None,
     ):
         """
         Create a DNS class, to configure a DNS inside a given VRF.
+
         :param domain_name: Domain name used for name resolution by the DNS
             client, if 'dns_domain_list' is not configured.
         :param domain_list: dict of DNS Domain list names to be used for
             address resolution, keyed by the resolution priority order.
             Example:
-                {
-                    0: "hpe.com"
-                    1: "arubanetworks.com"
-                }
+            {
+            0: "hpe.com"
+            1: "arubanetworks.com"
+            }
         :param domain_servers: dict of DNS Name servers to be used for address
             resolution, keyed by the resolution priority order. Example:
-                {
-                    0: "4.4.4.10"
-                    1: "4.4.4.12"
-                }
+            {
+            0: "4.4.4.10"
+            1: "4.4.4.12"
+            }
         :param host_v4_address_mapping: dict of static host address
             configurations and the IPv4 address associated with them. Example:
-                {
-                    "host1": "5.5.44.5"
-                    "host2": "2.2.44.2"
-                }
+            {
+            "host1": "5.5.44.5"
+            "host2": "2.2.44.2"
+            }
         :param host_v6_address_mapping: dict of static host address
             configurations and the IPv6 address associated with them. Example:
-                {
-                    "host1": "2001:0db8:85a3:0000:0000:8a2e:0370:7334"
-                }
-        : return DNS object.
+            {
+            "host1": "2001:0db8:85a3:0000:0000:8a2e:0370:7334"
+            }
+        :return: DNS object.
         """
         if vrf is None:
             vrf = "default"
 
         if domain_list is None:
             domain_list = {}
         if domain_servers is None:
@@ -115,14 +116,15 @@
         dns.apply()
 
         return dns
 
     def interface(self, name):
         """
         Create an Interface object.
+
         :param name: Alphanumeric name of Interface.
         :return: Interface object.
         """
         interface_obj = self.session.api.get_module(
             self.session, "Interface", name
         )
         try:
@@ -137,14 +139,15 @@
 
         return interface_obj
 
     def ipv6(self, address, interface_name, address_type=None):
         """
         Create a Ipv6 object. If values differ from existing object, incoming
             changes will be applied.
+
         :param address: Alphanumeric address of IPv6. Example:
             '2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff'
         :param interface_name: Alphanumeric name of the Interface parent of the
             IPv6 Address. A Interface object is also accepted.
         :param address_type: Type of IPv6 address. Defaults to "global-unicast"
             if not specified..
         :return: Ipv6 object.
@@ -194,14 +197,15 @@
         name=None,
         description=None,
         vlan_type=None,
         admin_conf_state="up",
     ):
         """
         Create a Vlan object.
+
         :param vlan_id: Numeric ID for VLAN.
         :param name: Alphanumeric name of VLAN, Defaults to "VLAN <ID>".
         :param description: Optional description to add to VLAN.
         :param vlan_type: VLAN type. Defaults to "static" if not specified.
         :param admin_conf_state: Optional administratively-configured state of
             VLAN. Only configurable for static VLANs. Defaults to "up" for
             static VLANs.
@@ -253,25 +257,27 @@
         return vlan_obj
 
     def __get_vrf_from_switch(self, name):
         """
         Get VRF from switch, this avoids making changes to the VRF object. Note
             the __double_leading_underscore that signifies that this is meant
             to be used only inside this module.
+
         :param name: VRF name.
         :return: Materialized Vrf object.
         """
         vrf = self.session.api.get_module(self.session, "Vrf", name)
         vrf.get()
         return vrf
 
     def vrf(self, name, route_distinguisher=None, vrf_type=None):
         """
         Create a Vrf object. If values differ from existing object, incoming
             changes will be applied.
+
         :param name: VRF name.
         :param route_distinguisher: Optional route distinguisher to add.
             Defaults to nothing if not specified.
         :param vrf_type: Optional VRF type. Defaults to "user" if not
             specified.
         :return: Vrf object.
         """
@@ -303,16 +309,16 @@
 
         return vrf_obj
 
     def vsx(self, **kwargs):
         """
         Create a Vsx object.  If values differ from existing object, incoming
             changes will be applied.
+
         :return: A Vsx object.
-        :rtype: Vsx.
         """
         keepalive_vrf = kwargs.get("keepalive_vrf")
         if keepalive_vrf:
             if isinstance(keepalive_vrf, str):
                 keepalive_vrf = self.__get_vrf_from_switch(keepalive_vrf)
             kwargs["keepalive_vrf"] = keepalive_vrf.get_info_format()
         software_update_vrf = kwargs.get("software_update_vrf")
@@ -352,14 +358,15 @@
             vsx_obj.apply()
         return vsx_obj
 
     def bgp_router_asn(self, vrf, asn, router_id=None):
         """
         Create a BgpRouter object as Autonomous System Number. If values differ
             from existing object, incoming changes will be applied.
+
         :param vrf: Alphanumeric name of the VRF the BGP ASN belongs to. A Vrf
             object is also accepted.
         :param asn: Integer that represents the Autonomous System Number.
         :param router_id: Optional IPv4 address that functions as the BGP
             Router ID.
         :return: BgpRouter object.
         """
@@ -385,14 +392,15 @@
         return bgp_router_obj
 
     def bgp_router_vrf(self, vrf, asn, redistribute):
         """
         Create a BgpRouter object with a BGP VRF settings for the associated
             BGP ASN. If values differ from existing object, incoming changes
             will be applied.
+
         :param vrf: Alphanumeric name of the VRF the BGP ASN belongs to. A Vrf
             object is also accepted.
         :param asn: Integer that represents the Autonomous System Number.
         :param redistribute: Alphanumeric to specify which types of routes that
             should be redistributed by BGP. The options are "ipv4-unicast" or
             "ipv6-unicast".
         :return: BgpRouter object.
@@ -437,14 +445,15 @@
         reflector=None,
         send_community=None,
         local_interface="",
     ):
         """
         Create a BgpNeighbor object. If values differ from existing object,
             incoming changes will be applied.
+
         :param vrf: Alphanumeric name of the VRF the BGP ASN belongs to.
             A Vrf object is also accepted.
         :param bgp_router_asn: Integer that represents the Autonomous System
             Number.
         :param group_ip: IPv4 address or name of group of the neighbors that
             functions as the BGP Router link. Example: '1.1.1.1'
         :param family_type: Alphanumeric to specify what type of neighbor
@@ -571,14 +580,15 @@
 
         return bgp_neighbor_obj
 
     def ospf_router(self, vrf, ospf_id, **kwargs):
         """
         Create OspfRouter object. If values differ from existing object,
             incoming changes will be applied.
+
         :param vrf: Alphanumeric name of the VRF the OSPF ID belongs to A Vrf
             object is also accepted.
         :param ospf_id: OSPF process ID between numbers 1-63.
         :param redistribute: List of types of redistribution methods for the
             OSPF Process, with the options being "bgp", "connected", and
             "static".
         :return: OspfRouter object.
@@ -601,20 +611,21 @@
             ospf_router_obj.create()
         return ospf_router_obj
 
     def ospfv3_router(self, vrf, ospfv3_id, **kwargs):
         """
         Create Ospfv3Router object. If values differ from existing object,
             incoming changes will be applied.
+
         :param vrf: Alphanumeric name of the VRF the OSPF ID belongs to.
             A Vrf object is also accepted.
         :param ospfv3_id: OSPF process ID between numbers 1-63.
         :param redistribute: List of types of redistribution methods for the
-        OSPF Process, with the options being "bgp", "connected",
-        "local_loopback", "rip", and "static".
+            OSPF Process, with the options being "bgp", "connected",
+            "local_loopback", "rip", and "static".
         :return: Ospfv3Router object.
         """
         if "redistribute" not in kwargs:
             kwargs["redistribute"] = ["connected", "static"]
         if isinstance(vrf, str):
             vrf = self.__get_vrf_from_switch(vrf)
         ospfv3_router_obj = self.session.api.get_module(
@@ -631,14 +642,15 @@
             ospfv3_router_obj.create()
         return ospfv3_router_obj
 
     def ospf_router_area(self, vrf, ospf_router, area_id, **kwargs):
         """
         Create an OspfArea object. If values differ from existing object,
             incoming changes will be applied.
+
         :param vrf: Alphanumeric name of the VRF the OSPF ID belongs to.
         :param ospf_router: OSPF process ID in [1, 63], an OspfRouter, or
             Ospfv3Router object is also accepted.
         :param area_id: Unique identifier as a string in the form of x.x.x.x.
         :param area_type: Alphanumeric defining how the external routing and
             summary LSAs for this area will be handled. Options are "default",
             "nssa", "nssa_no_summary", "stub", "stub_no_summary". If no value
@@ -683,14 +695,15 @@
         return ospf_area_obj
 
     def __get_ospf_router(self, ospf_id, vrf):
         """
         Get OSPF Router object from switch, this avoids making changes to it.
             Note the __double_leading_underscore that signifies that this is
             meant to be used only inside this module.
+
         :param ospf_id: OSPF process ID in [1,63].
         :param vrf: Vrf (object).
         :return: Materialized OspfRouter (object).
         """
         ospf_router_obj = self.session.api.get_module(
             self.session, "OspfRouter", ospf_id, parent_vrf=vrf
         )
@@ -698,14 +711,15 @@
         return ospf_router_obj
 
     def __get_ospfv3_router(self, ospfv3_id, vrf):
         """
         Get OSPFv3 Router object from switch, this avoids making changes to it.
             Note the __double_leading_underscore that signifies that this is
             meant to be used only inside this module.
+
         :param ospfv3_id: OSPFv3 process ID in [1,63].
         :param vrf: Vrf (object).
         :return: Materialized Ospfv3Router (object).
         """
         ospfv3_router_obj = self.session.api.get_module(
             self.session, "Ospfv3Router", ospfv3_id, parent_vrf=vrf
         )
@@ -713,28 +727,30 @@
         return ospfv3_router_obj
 
     def __get_ospf_area(self, area_id, ospf_router):
         """
         Get OSPFv3 Area object from switch, this avoids making changes to it.
             Note the __double_leading_underscore that signifies that this is
             meant to be used only inside this module.
+
         :param area_id: Unique identifier as a string in the form of x.x.x.x.
         :param ospf_router: OspfRouter (object) or Ospfv3Router (object).
         :return: Materialized Ospfv3Router (object).
         """
         ospf_area_obj = self.session.api.get_module(
             self.session, "OspfArea", area_id, parent_ospf_router=ospf_router
         )
         ospf_area_obj.get()
         return ospf_area_obj
 
     def ospfv3_router_area(self, vrf, ospfv3_id, area_id, **kwargs):
         """
         Create OspfArea object. If values differ from existing object, incoming
             changes will be applied.
+
         :param vrf: Alphanumeric name of the VRF the OSPF ID belongs to.
         :param ospfv3_id: OSPFv3 process ID in [1,63], an Ospfv3Router object
             is also accepted.
         :param area_id: Unique identifier as a string in the form of x.x.x.x.
         :param area_type: Alphanumeric defining how the external routing and
             summary LSAs for this area will be handled. Options are "default",
             "nssa", "nssa_no_summary", "stub", "stub_no_summary" if no value
@@ -747,14 +763,15 @@
         if isinstance(ospfv3_id, int):
             ospfv3_router = self.__get_ospfv3_router(ospfv3_id, vrf)
         return self.ospf_router_area(vrf, ospfv3_router, area_id, **kwargs)
 
     def ospf_interface(self, vrf, ospf_id, area_id, interface_name, **kwargs):
         """
         Create a OspfInterface object.
+
         :param vrf: Alphanumeric name of the VRF the OSPF ID belongs to. A Vrf
             object is also accepted.
         :param ospf_id: OSPF process ID between numbers 1-63. A OSPF Router is
             accepted.
         :param area_id: Unique identifier as a string in the form of x.x.x.x.
         :param interface_name: Alphanumeric name of the interface that will be
             attached to the OSPF area.
@@ -786,14 +803,15 @@
         return ospf_interface
 
     def ospfv3_interface(
         self, vrf, ospf_id, area_id, interface_name, **kwargs
     ):
         """
         Create a OspfInterface object.
+
         :param vrf: Alphanumeric name of the VRF the OSPF ID belongs to. A Vrf
             object is also accepted.
         :param ospfv3_id: OSPFv3 process ID between numbers 1-63. An OSPFv3
             Router is accepted.
         :param area_id: Unique identifier as a string in the form of x.x.x.x.
         :param interface_name: Alphanumeric name of the interface that will be
             attached to the OSPF area.
@@ -808,14 +826,15 @@
             vrf, ospf_router, area_id, interface_name, **kwargs
         )
 
     def ospf_vlink(self, vrf, ospf_router, area_id, peer_router, **kwargs):
         """
         Create a OspfVlink object. Defaults to using OspfRouter, when providing
             the OSPF process ID.
+
         :param vrf: Alphanumeric name of the VRF the OSPF ID belongs to. A Vrf
             object is also accepted.
         :param ospf_router: OSPF process ID number in [1,63]. An OSPF Router
             object is also accepted (both v2, and v3 versions).
         :param area_id: Unique identifier as a string in the form of x.x.x.x.
         :param peer_router: ID of the peer OSPF router as IP address in x.x.x.x
             form.
@@ -844,14 +863,15 @@
         except GenericOperationError:
             vlink.apply()  # if can't get it, create
         return vlink
 
     def ospfv3_vlink(self, vrf, ospf_router, area_id, peer_router, **kwargs):
         """
         Create a OspfVlink object.
+
         :param vrf: Alphanumeric name of the VRF the OSPF ID belongs to. A Vrf
             object is also accepted.
         :param ospf_router: OSPFv3 process ID number in [1, 63]. An
              Ospfv3Router object is also accepted.
         :param area_id: Unique identifier as a string in the form of x.x.x.x.
         :param peer_router: ID of the peer OSPFv3 router as IP address in
             x.x.x.x form.
@@ -872,14 +892,15 @@
         ipv4=None,
         vrf_name="default",
         vlan_port_desc=None,
     ):
         """
         Create VLAN and Interface objects to represent VLAN and SVI,
             respectively.
+
         :param vlan_id: Numeric ID of VLAN.
         :param vlan_name: Alphanumeric name of VLAN.
         :param vlan_int_name: Alphanumeric name for the VLAN interface.
         :param vlan_desc: Optional description to add to VLAN.
         :param ipv4: Optional IPv4 address to assign to the interface. Defaults
             to nothing if not specified. Example: '1.1.1.1'
         :param vrf_name: VRF to attach the SVI to. Defaults to "default".
@@ -896,14 +917,15 @@
         interface_obj.configure_svi(vlan_id, ipv4, vrf_name, vlan_port_desc)
 
         return vlan_obj, interface_obj
 
     def dhcp_relay(self, vrf, port):
         """
         Create a DhcpRelay object.
+
         :param vrf: Alphanumeric name of VRF.
         :param port: Alphanumeric name of Port.
         :return: DhcpRelay object.
         """
         port_obj = self.session.api.get_module(self.session, "Interface", port)
         vrf_obj = self.session.api.get_module(self.session, "Vrf", vrf)
 
@@ -919,14 +941,15 @@
             dhcp_relay.apply()
 
         return dhcp_relay
 
     def acl(self, list_name, list_type):
         """
         Create an Acl object.
+
         :param list_name: Alphanumeric name of ACL.
         :param list_type: Alphanumeric type of ACL. Type should be one of
             "ipv4," "ipv6," or "mac".
         :return: Acl object.
         """
         acl = self.session.api.get_module(
             self.session, "ACL", index_id=list_name, list_type=list_type
@@ -956,41 +979,42 @@
         src_mac=None,
         dst_mac=None,
         ethertype=None,
         **kwargs
     ):
         """
         Create an AclEntry object.
+
         :param list_name: Alphanumeric name of the ACL.
         :param list_type: Type should be one of "ipv4," "ipv6," or "mac".
         :param sequence_num: Integer number of the sequence.
         :param action: Action should be either "permit" or "deny".
         :param count: Optional boolean flag that when true, will make entry
             increment hit count for matched packets.
         :param protocol: Optional integer IP protocol number.
         :param src_ip: Optional source IP address. Both IPv4 and IPv6 are
             supported. Example:
-                10.10.12.11/255.255.255.255
-                2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
+            10.10.12.11/255.255.255.255
+            2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
         :param dst_ip: Optional destination IP address. Both IPv4 and IPv6 are
             supported. Example:
-                10.10.12.11/255.255.255.255
-                2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
+            10.10.12.11/255.255.255.255
+            2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff
         :param dst_l4_port_min: Optional minimum L4 port number in range; used
             in conjunction with dst_l4_port_max.
         :param dst_l4_port_max: Optional maximum L4 port number in range; used
             in conjunction with dst_l4_port_min.
         :param src_mac: Optional source MAC address. Example:
             '01:02:03:04:05:06'
         :param dst_mac: Optional destination MAC address. Example:
             '01:02:03:04:05:06'
         :param ethertype: Optional integer EtherType number.
         :param kwargs: Optional keyword arguments for more detailed
             configuration.
-        :return acl_entry: A AclEntry object.
+        :return: A AclEntry object.
         """
         # Create Acl object
         acl = self.session.api.get_module(
             self.session, "ACL", index_id=list_name, list_type=list_type
         )
 
         # Get ACL data
@@ -1036,14 +1060,15 @@
             acl_entry_obj.apply()
 
         return acl_entry_obj
 
     def vrf_address_family(self, vrf, address_family="ipv4_unicast"):
         """
         Create a VrfAddressFamily object with a VRF.
+
         :param vrf: Alphanumeric name of the VRF the Family Address belongs to.
             A Vrf object is also accepted.
         :param address_family: Alphanumeric type of the Address Family. The
             options are 'ipv4_unicast' and 'ipv6_unicast'. Defaults to
             'ipv4_unicast'.
         :return: VRF_Address_Family object.
         """
@@ -1062,14 +1087,15 @@
             vrf_address_fam_obj.apply()
 
         return vrf_address_fam_obj
 
     def aggregate_address(self, vrf, bgp_router_asn, family_type, ip_prefix):
         """
         Create an AggregateAddress object.
+
         :param vrf: Alphanumeric name of the VRF the BGP ASN belongs to. A Vrf
             object is also accepted.
         :param bgp_router_asn: Integer that represents the Autonomous System
             Number.
         :param family_type: Address Family type for the Aggregate Address.
             The options are: 'ipv4-unicast', 'ipv6-unicast'.
         :param ip_prefix: IP address and mask used to key Aggregate Address.
@@ -1114,21 +1140,22 @@
             aggregate_add_obj.apply()
 
         return aggregate_add_obj
 
     def static_route(self, vrf, destination_address_prefix):
         """
         Create a StaticRoute object with a VRF.
+
         :param vrf: Name of the VRF on which the static route is to be
             configured. Defaults to default vrf. A Vrf object is also accepted.
         :param destination_address_prefix: String IPv4 or IPv6 destination
             prefix and mask in the address/mask format. Example:
-                '1.1.1.1'
-                or
-                '2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff'
+            '1.1.1.1'
+            or
+            '2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff'
         :return: StaticRoute object.
         """
         if isinstance(vrf, str):
             vrf = self.__get_vrf_from_switch(vrf)
 
         static_route_obj = self.session.api.get_module(
             self.session,
@@ -1155,27 +1182,28 @@
         distance=None,
         next_hop_interface=None,
         bfd_enable=None,
     ):
         """
         Create a Static Nexthop, with a VRF and a Destination Address related
             to a Static Route.
+
         :param vrf: Name of the VRF on which the static route is to be
             configured. Defaults to "default". A Vrf object is also accepted.
         :param destination_address_prefix: String IPv4 or IPv6 destination
             prefix and mask in the address/mask format. A StaticRoute object
             is also accepted. Example:
-                '1.1.1.1'
-                or
-                '2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff'
+            '1.1.1.1'
+            or
+            '2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff'
         :param next_hop_ip_address: The IPv4 address or the IPv6 address of
             next hop. Example:
-                '1.1.1.1'
-                or
-                '2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff'
+            '1.1.1.1'
+            or
+            '2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff'
         :param nexthop_type: Specifies whether the static route is a forward,
             blackhole or reject route.
         :param distance: Administrative distance to be used for the next hop in
             the static route instead of default value.
         :param next_hop_interface: The interface through which the next hop can
             be reached.
         :param bfd_enable: Boolean to enable BFD.
@@ -1242,14 +1270,15 @@
             static_nexthop_obj.apply()
 
         return static_nexthop_obj
 
     def poe_interface(self, interface):
         """
         Create a PoE Interface object with associated settings.
+
         :param Interface: Alphanumeric name of the Interface the PoE_Interface
             belongs to. An Interface object is also accepted.
         :return: PoE Interface object.
         """
         if isinstance(interface, str):
             # Make Interface into an object
             interface_obj = self.session.api.get_module(
@@ -1266,14 +1295,15 @@
         poe_interface_obj.get()
 
         return poe_interface_obj
 
     def mac(self, vlan, from_id, mac_address):
         """
         Create an Mac object.
+
         :param vlan_id: Numeric ID for VLAN. A Vlan object is also accepted.
         :param from_id: String source of the MAC address.
             Must be "dynamic", "VSX", "static", "VRRP", "port-access-security",
             "evpn", or "hsc".
         :param mac_address: String MAC address, or netaddr EUI object. Example:
             '01:02:03:04:05:06'.
         :return: Mac object.
@@ -1293,18 +1323,18 @@
         mac_obj.get()
 
         return mac_obj
 
     def static_mac(self, vlan, port, mac_address):
         """
         Create an StaticMac object.
+
         param vlan_id: Numeric ID for VLAN. A Vlan object is also accepted.
-        :param port: String for the Port's name. Example: 1/1/1.
-        :param mac_address: String MAC address, or netaddr EUI object. Example:
-            '01:02:03:04:05:06'.
+        :param port: String for the Port's name. Example 1/1/1.
+        :param mac_address: String MAC address, or netaddr EUI object.
         :return: StaticMac object.
         """
         if isinstance(vlan, int):
             vlan = self.vlan(vlan, "Vlan{0}".format(vlan))
 
         if isinstance(port, str):
             port = self.interface(port)
@@ -1325,14 +1355,15 @@
             static_mac_obj.apply()
 
         return static_mac_obj
 
     def qos(self, name, **kwargs):
         """
         Create a Qos object.
+
         :param name: String representing a user-defined name for a Qos object.
         :return: Returns a Qos object.
         """
         # Check for data type of name
         if not isinstance(name, str):
             raise ValueError("ERROR: Name must be on string format.")
 
@@ -1349,14 +1380,15 @@
             pass  # not present in switch, not an error
         qos_obj.apply()
         return qos_obj
 
     def qos_cos(self, code_point, **kwargs):
         """
         Gets a QoS COS trust mode object.
+
         :param code_point: Integer to identify an entry a QoS COS trust mode
             object.
         :return: Returns a QoS COS trust mode object.
         """
         if not isinstance(code_point, int):
             raise ValueError("ERROR: Code Point must be an integer.")
 
@@ -1378,14 +1410,15 @@
             qos_cos_obj.apply()
 
         return qos_cos_obj
 
     def qos_dscp(self, code_point, **kwargs):
         """
         Retrieves a QoS DSCP trust mode map entry as an object.
+
         :param code_point: Integer to identify an entry a QoS DSCP trust mode
             object.
         :return: Returns a QoS DSCP trust mode object.
         """
         if not isinstance(code_point, int):
             raise Exception("ERROR: Code point must be an integer.")
 
@@ -1407,14 +1440,15 @@
             qos_dscp_obj.apply()
 
         return qos_dscp_obj
 
     def queue(self, qos_name, queue_number, **kwargs):
         """
         Create a Queue object.
+
         :param qos_name: String with a user-defined name for a QoS object.
         :param queue_number: Integer representing a queue priority, with zero
             being the lowest priority. The maximum number of queues is
             hardware-dependent.
         :return: Queue object.
         """
         if not isinstance(qos_name, str):
@@ -1443,14 +1477,15 @@
 
         # return object
         return queue_obj
 
     def queue_profile(self, name, **kwargs):
         """
         Create a Queue Profile object.
+
         :param name: name of the profile.
         :return: Queue Profile object.
         """
         profile = self.session.api.get_module(
             self.session, "QueueProfile", index_id=name, **kwargs
         )
         try:
@@ -1463,14 +1498,15 @@
             # Apply the local configuration to the switch
             profile.apply()
         return profile
 
     def queue_profile_entry(self, queue_number, queue_profile, **kwargs):
         """
         Create a Queue Profile Entry object.
+
         :param queue_number: Number that identifies the entry.
         :param queue_profile: A Queue Profile object.
         :return: Queue Profile Entry object.
         """
         if isinstance(queue_profile, str):
             queue_profile = self.session.api.get_module(
                 self.session, "QueueProfile", index_id=queue_profile
@@ -1502,14 +1538,15 @@
         routing=None,
         vlan=None,
         vrf=None,
         **kwargs
     ):
         """
         Create a Virtual Network ID (VNI).
+
         :param vni_id: VNI identifier.
         :param interface: Attached interface to the VNI.
         :param vni_type: Type of the VNI (for now just vxlan_vni).
         :param vlan: Mapped VLAN to the VNI.
         :param vrf: Mapped VRF to the VNI (if L3 is supported).
         :param routing: Flag that indicates if VNI is L2 or L3.
         :return: VNI object.
@@ -1551,14 +1588,15 @@
         destination,
         origin="static",
         vrf=None,
         **kwargs
     ):
         """
         Create a Tunnel Endpoint
+
         :param interface: Attached interface for tunnel
         :param network_id: Network identifier
         :param destination: Destination IP
         :param origin: Type of tunneling
             'static' for user configuration (default)
             'evpn' for dynamically learnt via EVPN
             'hsc' for dynamically learnt from a remote controller
```

### Comparing `pyaoscx-2.3.1/pyaoscx/pyaoscx_module.py` & `pyaoscx-2.4.0/pyaoscx/pyaoscx_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import functools
 import json
 import logging
 import warnings
 
@@ -24,31 +24,33 @@
     base_uri = ""
     indices = []
 
     def connected(fnct):
         """
         Function used as a decorator to ensure the module has a established
             connection.
+
         :param fnct: function which behavior is modified.
-        :return ensure_connected: Function.
+        :return: Function.
         """
 
         @functools.wraps(fnct)
         def ensure_connected(self, *args, **kwargs):
             if not self.session.connected:
                 self.session.open()
             return fnct(self, *args, **kwargs)
 
         return ensure_connected
 
     def materialized(fnct):
         """
         Function used as a decorator to verify if the object is materialized.
+
         :para fnct: function which behavior is modified.
-        :return is_materialized: Function.
+        :return: Function.
         """
 
         @functools.wraps(fnct)
         def is_materialized(self, *args, **kwargs):
             if not self.materialized:
                 raise VerificationError(
                     "Object {0}".format(self), " not materialized"
@@ -56,16 +58,17 @@
             return fnct(self, *args, **kwargs)
 
         return is_materialized
 
     def deprecated(func):
         """
         Function used as a decorator to show deprecation notice of a method.
+
         :param func: function whose behavior is modified/wrapped.
-        :return func: function whose behavior is modified/wrapped.
+        :return: function whose behavior is modified/wrapped.
         """
 
         @functools.wraps(func)
         def is_deprecated(*args, **kwargs):
             warnings.warn(
                 "{0} will be removed in a future version".format(
                     func.__name__
@@ -79,27 +82,29 @@
 
     @abstractmethod
     @connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a table entry and fill the
             object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if there is not an exception raised.
         """
         pass
 
     @abstractmethod
     def get_all(cls, session):
         """
         Perform a GET call to retrieve all system <pyaoscx_module_type> and
             create a dictionary of each object.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :return: Dictionary containing object IDs as keys their respective
             objects as values.
         """
         pass
@@ -109,36 +114,39 @@
     def apply(self):
         """
         Main method used to either create or update an existing
             <pyaoscx_module_type>. Checks whether the <pyaoscx_module_type>
             exists in the switch. Calls self.update() if object being updated.
             Calls self.create() if a new <pyaoscx_module_type> is being
             created.
-        :return modified: Boolean, True if object was created or modified.
+
+        :return: Boolean, True if object was created or modified.
         """
         pass
 
     @abstractmethod
     @connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing
             <pyaoscx_module_type> table entry.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         pass
 
     @abstractmethod
     @connected
     def create(self):
         """
         Perform a POST call to create a new <pyaoscx_module_type>. Only returns
             if an exception is not raise.
-        :return modified: Boolean, True if entry was created.
+
+        :return: Boolean, True if entry was created.
         """
         pass
 
     @abstractmethod
     @connected
     def delete(self):
         """
@@ -146,20 +154,20 @@
         """
         pass
 
     @abstractmethod
     def from_uri(cls, session, uri):
         """
         Create a <pyaoscx_module_type> object given its URI.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param uri: a String with a URI.
-        :return index, <pyaoscx_module_type>: tuple containing both the
-            <pyaoscx_module_type> object its ID.
+        :return: tuple containing both the <pyaoscx_module_type> object its ID.
         """
         pass
 
     def _get_and_copy_data(
         self, depth=None, selector=None, unwanted_attrs=None
     ):
         """
@@ -182,14 +190,15 @@
         if selector in self.session.api.configurable_selectors:
             # Set self.config_attrs and delete unwanted attributes
             utils.set_config_attrs(self, data, "config_attrs", unwanted_attrs)
 
     def _get_data(self, depth, selector):
         """
         Perform a GET call to retrieve data from a switch.
+
         :param depth: Integer deciding how many levels into the API JSON
             that references will be retrieved from the switch
         :param selector: Alphanumeric option to select specific information
             to return.
         :return: Retrieved data from the switch.
         """
         depth = depth or self.session.api.default_depth
@@ -216,14 +225,15 @@
             raise GenericOperationError(response.text, response.status_code)
 
         return json.loads(response.text)
 
     def _put_data(self, data):
         """
         Perform a PUT request to the switch.
+
         :param data: data to send.
         :return: True if the object was modified.
         """
         if data == self._original_attributes:
             return False
 
         self._send_data(self.path, data, "PUT", "Update")
@@ -231,24 +241,26 @@
         self._original_attributes = data
         # Object was modified
         return True
 
     def _post_data(self, data):
         """
         Perform a POST request to the switch.
+
         :param data: data to send.
         """
         self._send_data(self.base_uri, data, "POST", "Adding")
         # Get the data from the created object
         self.get()
         return True
 
     def _send_data(self, path, data, http_verb, display_verb):
         """
         Perform either PUT or POST operation to the switch.
+
         :param path: path of the resource for the request. This could
             the base URI if this was called in a create method, or
             the VLAN URI if this was called in an update method.
         :param data: data to send.
         :param hrrp_verb: HTTP operation to perfrom.
         :display_module_name: Module to display in logs.
         :display_verb: verb to display in logs.
@@ -275,14 +287,15 @@
         """
         Compares two PYAOSCX modules to determine if a replace (delete+create)
             is required. To do so, all the immutable parameters are checked; in
             case any of them differs a replace is required. Note that if the
             replacement object has a None parameter then a replace is not
             required because they just get ignored, null parameters are
             meant to be taken as 'keep the current value' by PYAOSCX.
+
         :param current: Module representing the current switch configuration.
         :param replacement: Another Module (same type) object to compare to
         :param immutable_parameter_names: the names of parameters that cannot
             change once the module has been created.
         :return: True if a replacement is required.
         """
         for param_name in immutable_parameter_names:
@@ -305,14 +318,15 @@
         """
         Extract the missing configuration parameters from another PYAOSCX
             Module, to incorporate them as their own. This is useful when
             replacing (delete+create) Modules. If the Module has to be
             replaced, the parameters that are not specified (locally) should
             remain unchanged (switch), so it is necessary to extract them from
             the switch before performing the replacement.
+
         :param other: the other module to extract the parameters.
         """
         # Until we are able to read the Schema we need to keep a list of the
         # the names of mutable an immutable parameters. Once we are capable of
         # using the schema, the information can be taken from there.
         all_param_names = (
             self.immutable_parameter_names + self.mutable_parameter_names
@@ -328,10 +342,11 @@
                         setattr(self, param_name, deepcopy(param))
 
     @deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
-        return: Object format depending on the API Version.
+
+        :return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
```

### Comparing `pyaoscx-2.3.1/pyaoscx/qos.py` & `pyaoscx-2.4.0/pyaoscx/qos.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     resource_uri_name = "qos"
 
     indices = ["name"]
 
     def __init__(self, session, name, **kwargs):
         """
         Initialize a Qos object.
+
         :param session: pyaoscx.Session object used to represent logical
             connection to the device.
         :param name: String representing a user-defined name for a Qos object.
         :param uri: a String with an URI.
         """
         self.session = session
         self.__name = name
@@ -48,24 +49,26 @@
         # Build path
         self.path = "{0}/{1}".format(self.base_uri, self.name)
 
     @property
     def name(self):
         """
         Method used to obtain the specific name.
+
         :return: returns the name of this Qos object.
         """
         # This uses the @property decorator to make self.name read-only
         return self.__name
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a QoS table entry and fill the
             object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if no exception is raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -86,14 +89,15 @@
 
         return True
 
     @classmethod
     def get_all(cls, session):
         """
         Perfom GET request to retrieve all Schedule Profiles in a switch.
+
         :param session: pyaoscx.Session object used to represent a logical.
         :return: Dictionary containing all system QoS configurations.
         """
         logging.info("Retrieving all %s data from switch", cls.__name__)
 
         try:
             response = session.request("GET", cls.base_uri)
@@ -116,38 +120,41 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update an existing Schedule
             Profile. Checks whether the QoS configuration exists in the switch.
             Calls self.update() if object is being updated. Calls self.create()
             if a new object is being created.
+
         :return modified: Boolean, True if object was created or modified.
         """
         if self.materialized:
             self.__modified = self.update()
         else:
             self.__modified = self.create()
         return self.__modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing Schedule Profile.
+
         :return modified: True if Object was modified and a PUT request was
             made.
         """
         qos_data = utils.get_attrs(self, self.config_attrs)
         return self._put_data(qos_data)
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST request to create a new QoS configuration using the
             object's attributes as the request's body. An exception is raised
             if object cannot be created.
+
         :return modified: Boolean, True if entry was created.
         """
         qos_data = utils.get_attrs(self, self.config_attrs)
         qos_data["name"] = self.name
         return self._post_data(qos_data)
 
     @PyaoscxModule.connected
@@ -158,32 +165,34 @@
         self._send_data(self.path, None, "DELETE", "delete")
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, response_data):
         """
         Create a Qos object given a response_data related to it.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param response_data: The response must be a dictionary of the form:
             {
-                "<QoS name>": "/rest/v10.08/system/qos/<QoS name>"
+            "<QoS name>": "/rest/v10.08/system/qos/<QoS name>"
             }
         :return: Qos Object.
         """
         qos_name_arr = session.api.get_keys(
             response_data, cls.resource_uri_name
         )
         qos_name = qos_name_arr[0]
         return cls(session, qos_name)
 
     @classmethod
     def from_uri(cls, session, uri):
         """
         Create a Qos object given a QoS URI.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param uri: a String with a URI.
         :return name, qos: tuple with the name of a QoS configuration, and a
             corresponding object.
         """
         # fail if uri is not a valid QoS URI
@@ -196,14 +205,15 @@
 
         return name, qos
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the this instance's URI.
+
         :return: Object's URI.
         """
         # Parent class uses self.path internally to store the value of the URI
         return self.path
 
     @property
     def modified(self):
@@ -212,25 +222,27 @@
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method to check it object has been modified.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     def __str__(self):
         return "Qos {0}".format(self.name)
 
     @classmethod
     def set_global_trust_mode(cls, session, trust_mode):
         """
         Sets the global trust mode for the switch.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param trust_mode: A string to set the global trust mode, which can be
             one of the following: "cos", "dscp", "none", or "default".
             Use the default option to use the switch's default trust mode.
         :return: Returns True if configuration was modified.
         """
@@ -267,14 +279,15 @@
         return modified
 
     @classmethod
     def set_global_schedule_profile(cls, session, profile):
         """
         Sets the global schedule profile (the name of a Qos object) for the
             switch.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param profile: Name of a schedule profile (the name of a Qos object)
             to set as the global schedule profile.
         """
         logging.info("Setting global schedule profile to: %s", profile)
         device = Device(session)
```

### Comparing `pyaoscx-2.3.1/pyaoscx/qos_cos.py` & `pyaoscx-2.4.0/pyaoscx/qos_cos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2021-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2021-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
 from pyaoscx.exceptions.response_error import ResponseError
@@ -21,17 +21,18 @@
     resource_uri_name = "qos_cos_map_entries"
 
     indices = ["code_point"]
 
     def __init__(self, session, code_point, **kwargs):
         """
         Initialize a QoS COS trust mode object.
+
         :param session: pyaoscx.Session object used to represent logical
             connection to the device.
-        :param code_point: Integer to identify a QoS COS trust mode object.
+        :param: Integer to identify a QoS COS trust mode object.
         """
         self.session = session
         self.__code_point = code_point
 
         # List used to determine attributes related to the QoS COS
         # configuration
         self.config_attrs = []
@@ -45,24 +46,26 @@
         # Build path
         self.path = "{0}/{1}".format(self.base_uri, self.code_point)
 
     @property
     def code_point(self):
         """
         Method used to retrieve object's code point.
+
         :return: returns the code point of this QoS COS trust mode object.
         """
         # This uses the @property decorator to make self.code_point read-only
         return self.__code_point
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a QoS COS trust mode table
             entry and fill the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information
             return.
         :return: Returns True if no exception is raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -90,14 +93,15 @@
         return True
 
     @classmethod
     def get_all(cls, session):
         """
         Perform a GET call to retrieve all system QoS COS trust mode
             configurations from of a switch.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :return: Dictionary containing all system Schedule Profiles.
         """
         logging.info("Retrieving all %s data from switch", cls.__name__)
 
         try:
@@ -120,25 +124,27 @@
     @PyaoscxModule.materialized
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to update an existing QoS COS trust mode table entry.
             Checks whether the QoS COS trust mode exists in the switch. Calls
             self.update if object is being updated.
-        :return modified: Boolean, True if object was modified.
+
+        :return: Boolean, True if object was modified.
         """
         # Modify object
         self.__modified = self.update()
         return self.__modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to update an existing QoS COS trust mode object.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         qos_cos_data = utils.get_attrs(self, self.config_attrs)
         return self._put_data(qos_cos_data)
 
     @PyaoscxModule.connected
     def create(self):
@@ -151,33 +157,35 @@
         pass
 
     @classmethod
     def from_response(cls, session, response_data):
         """
         Create a QoS COS trust mode object given a response_data related to the
             existing QoS COS trust mode object.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param response_data: The response must be a dictionary of the form:
             {
-                "3" : "/rest/v10.08/system/qos_cos_map_entries/3"
+            "3" : "/rest/v10.08/system/qos_cos_map_entries/3"
             }
         :return: QoS COS trust mode object.
         """
         code_points_arr = session.api.get_keys(
             response_data, cls.resource_uri_name
         )
         code_point = code_points_arr[0]
 
         return cls(session, code_point)
 
     @classmethod
     def from_uri(cls, session, uri):
         """
         Create an object given a QoS COS trust mode URI.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param uri: s String with an URI.
         :return: returns identifier and object.
         """
         # Separate values from URI
         if cls.base_uri not in uri:
@@ -193,14 +201,15 @@
         # Return identifier and object
         return code_point, qos_cos
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain object's URI.
+
         :return: Object's URI.
         """
         # The self.path variable stores the URI
         return self.path
 
     @property
     def modified(self):
@@ -209,14 +218,15 @@
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method to check it object has been modified.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     def __str__(self):
         return "QoS COS trust mode {0}".format(self.code_point)
 
@@ -227,14 +237,15 @@
         """
         return self.__color
 
     @color.setter
     def color(self, color):
         """
         Updates the value of the color of this QoS COS instance.
+
         :param color: String to identify the color which may be used later in
             the pipeline in packet-drop decision points. Example: "green".
         """
         # Verify data type
         if not isinstance(color, str):
             raise ValueError("ERROR: Color value must be a string.")
 
@@ -247,14 +258,15 @@
         """
         return self.__description
 
     @description.setter
     def description(self, description):
         """
         Updates the description of this QoS COS instance.
+
         :param description: String used for customer documentation.
         """
         # Verify data type
         if not isinstance(description, str):
             raise ValueError("ERROR: Description value must be a string.")
 
         self.__description = description
@@ -266,14 +278,15 @@
         """
         return self.__local_priority
 
     @local_priority.setter
     def local_priority(self, priority):
         """
         Updates the value of the local priority of this QoS COS instance.
+
         :param priority: Integer to represent an internal meta-data value that
             will be associated with the packet. This value will be used later
             to select the egress queue for the packet.
         """
         # Verify data type
         if not isinstance(priority, int):
             raise ValueError("ERROR: Priority must be an integer.")
```

### Comparing `pyaoscx-2.3.1/pyaoscx/qos_dscp.py` & `pyaoscx-2.4.0/pyaoscx/qos_dscp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2021-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2021-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
 from pyaoscx.exceptions.response_error import ResponseError
@@ -26,14 +26,15 @@
     resource_uri_name = "qos_dscp_map_entries"
 
     indices = ["code_point"]
 
     def __init__(self, session, code_point, **kwargs):
         """
         Initialize a QoS DSCP trust mode object.
+
         :param session: pyaoscx.Session object used to represent logical
             connection to the device.
         :param code_point: Integer to identify a QoS DSCP configuration.
         """
         self.session = session
         self.__code_point = code_point
 
@@ -54,25 +55,27 @@
         # Build path
         self.path = "{0}/{1}".format(self.base_uri, self.code_point)
 
     @property
     def code_point(self):
         """
         Method used to obtain the specific code point.
+
         :return: returns the code point of this QoS DSCP trust mode object.
         """
         # Use the @property decorator to make `self.code_point` read-only, and
         # return the actual value here
         return self.__code_point
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a QoS DSCP table entry and fill
             the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to query specific information.
         :return: Returns True if there is not an exception raised.
         """
         logging.info("Retrieving %s from switch", self)
 
@@ -106,17 +109,18 @@
         return True
 
     @classmethod
     def get_all(cls, session):
         """
         Perform a GET call to retrieve all system QoS DSCP configurations from
             a switch.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
-        :return:  containing all system QoS.
+        :return: containing all system QoS.
         """
         logging.info("Retrieving all %s data from switch", cls.__name__)
 
         try:
             response = session.request("GET", cls.base_uri)
         except Exception as e:
             raise ResponseError("GET", e)
@@ -137,24 +141,26 @@
     @PyaoscxModule.materialized
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to update an existing QoS table entry. Checks whether
             the QoS DSCP entry exists in the switch. Calls self.update if
             object is being updated.
-        :return modified: Boolean, True if object was modified.
+
+        :return: Boolean, True if object was modified.
         """
         self.__modified = self.update()
         return self.__modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT request to update an existing QoS DSCP object.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         qos_dscp_data = utils.get_attrs(self, self.config_attrs)
 
         return self._put_data(qos_dscp_data)
 
     @PyaoscxModule.connected
@@ -168,19 +174,20 @@
         pass
 
     @classmethod
     def from_response(cls, session, response_data):
         """
         Create a QoS DSCP trust mode object given a response_data related to
             the QoS DSCP trust mode object.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param response_data: The response must be a dictionary of the form:
             {
-                "3" : "/rest/v10.08/system/qos_dscp_map_entries/3"
+            "3" : "/rest/v10.08/system/qos_dscp_map_entries/3"
             }
         :return: QoS DSCP trust mode object.
         """
         code_points_arr = session.api.get_keys(
             response_data, cls.resource_uri_name
         )
 
@@ -188,14 +195,15 @@
 
         return cls(session, code_point)
 
     @classmethod
     def from_uri(cls, session, uri):
         """
         Create a QoS DSCP object given a QoS DSCP trust mode URI.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param uri: s String with a URI.
         :return: returns identifier and object.
         """
         # Separate values from URI
         if cls.base_uri not in uri:
@@ -209,14 +217,15 @@
         # Return identifier and object
         return code_point, qos_dscp
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific QoS DSCP trust mode URI.
+
         :return: Object's URI.
         """
         # Return self.path containing the object's URI
         return self.path
 
     @property
     def modified(self):
@@ -225,14 +234,15 @@
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method to check it object has been modified.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     def __str__(self):
         return "QoS DSCP trust mode {0}".format(self.code_point)
 
@@ -243,14 +253,15 @@
         """
         return self.__cos
 
     @cos.setter
     def cos(self, cos):
         """
         Updates the value of the cos of this QoS DSCP instance.
+
         :param cos: Priority Code Point (PCP) that will be assigned to any IP
             packet with the specified DSCP codepoint, if that packet's ingress
             port has an effective trust mode of trust dscp. The new PCP is used
             when the packet is transmitted out a port or trunk with a VLAN tag.
             If the key is not specified, then no remark will occur.
         """
         # Verify data type
@@ -269,14 +280,15 @@
         """
         return self.__priority_code_point
 
     @priority_code_point.setter
     def priority_code_point(self, priority_code_point):
         """
         Updates the value of the priority_code_point of this QoS DSCP instance.
+
         :param priority_code_point: Priority Code Point (PCP) that will be
             assigned to any IP packet with the specified DSCP codepoint, if
             that packet's ingress port has an effective trust mode of trust
             dscp. The new PCP is used when the packet is transmitted out a port
             or trunk with a VLAN tag.  If the key is not specified, then no
             remark will occur.
         """
@@ -298,14 +310,15 @@
         """
         return self.__color
 
     @color.setter
     def color(self, color):
         """
         Updates the value of the color of this QoS DSCP instance.
+
         :param color: String to identify the color which may be used later in
             the pipeline in packet-drop decision points. Example: "green".
         """
         # Verify data type
         if not isinstance(color, str):
             raise ValueError("ERROR: Color value must be a string.")
         self.__color = color
@@ -317,14 +330,15 @@
         """
         return self.__description
 
     @description.setter
     def description(self, description):
         """
         Updates the description of this QoS DSCP instance.
+
         :param description: String used for customer documentation.
         """
         # Verify data type
         if not isinstance(description, str):
             raise ValueError("ERROR: Description value must be a string.")
         self.__description = description
 
@@ -335,14 +349,15 @@
         """
         return self.__local_priority
 
     @local_priority.setter
     def local_priority(self, priority):
         """
         Updates the value of the local priority of this QoS DSCP instance.
+
         :param priority: Integer to represent an internal meta-data value that
             will be associated with the packet. This value will be used later
             to select the egress queue for the packet.
         """
         # Verify data type
         if not isinstance(priority, int):
             raise ValueError("ERROR: Priority must be an integer.")
```

### Comparing `pyaoscx-2.3.1/pyaoscx/queue.py` & `pyaoscx-2.4.0/pyaoscx/queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2021-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2021-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
 from pyaoscx.exceptions.response_error import ResponseError
@@ -89,31 +89,34 @@
             )
         self.__gmb_percent = value
 
     @property
     def queue_number(self):
         """
         Method to retrieve the queue_number identifier of this object.
+
         :return: returns the queue number of this object.
         """
         return self.__queue_number
 
     @property
     def qos_name(self):
         """
         Method to retrieve the qos_name identifier of this object.
+
         :return: returns the Qos name of this object.
         """
         return self.__qos_name
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a Queue table entry and fill
             object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if no exception is raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -137,14 +140,15 @@
         return True
 
     @classmethod
     def get_all(cls, session, qos_name):
         """
         Perform a GET call to retrieve all system Queues for given Schedule
             Profile from a switch.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :return: Dictionary containing all system Schedule Profile's Queues.
         """
         logging.info("Retrieving all %s data from switch", cls.__name__)
 
         uri = "{0}{1}/{2}/{3}".format(
@@ -170,41 +174,44 @@
         return queues_dict
 
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update an existing Queue. Checks
             whether the Queue exists in the switch. Calls self.update() if
-            object is being updated.
-        Calls self.create() if a new object is being created.
-        :return modified: Boolean, True if object was created or modified.
+            object is being updated. Calls self.create() if a new object is
+            being created.
+
+        :return: Boolean, True if object was created or modified.
         """
         if self.materialized:
             self.__modified = self.update()
         else:
             self.__modified = self.create()
         return self.__modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing Queue table entry.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         queue_data = utils.get_attrs(self, self.config_attrs)
         return self._put_data(queue_data)
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST request to create a new Queue using the object's
             attributes as the request body. An exception is raised if object
             cannot be created.
-        :return modified: Boolean, True if entry was created.
+
+        :return: Boolean, True if entry was created.
         """
         queue_data = utils.get_attrs(self, self.config_attrs)
         queue_data["queue_number"] = self.queue_number
 
         return self._post_data(queue_data)
 
     @PyaoscxModule.connected
@@ -214,19 +221,20 @@
         """
         self._send_data(self.path, None, "DELETE", "delete")
 
     @classmethod
     def from_response(cls, session, response_data):
         """
         Create a Queue object given a related response_data.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param response_data: The response must be a dictionary of the form:
             {
-                "strict": "/rest/v10.08/system/qos/"<Qos name>/queues/7"
+            "strict": "/rest/v10.08/system/qos/"<Qos name>/queues/7"
             }
         :return: Queue Object.
         """
         # Check if response is a dictionary, if so, get its value
         if isinstance(response_data, dict):
             data = list(response_data.items())[0][1]
         else:
@@ -240,31 +248,33 @@
 
         return cls(session, qos_name, queue_number)
 
     @classmethod
     def from_uri(cls, session, uri):
         """
         Create a Queue object given a Queue URI.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param uri: a String with a URI.
-        :return name, queue: tuple with the Queue object and its name.
+        :return: tuple with the Queue object and its name.
         """
         # Get queue number from uri
         uri_arr = uri.split("/")
         queue_number = uri_arr[-1]
         qos_name = uri_arr[uri_arr.index(Qos.resource_uri_name) + 1]
         queue = cls(session, qos_name, queue_number)
 
         return queue_number, queue
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain this instance's URI.
+
         :return: Object's URI.
         """
         return self.path
 
     @property
     def modified(self):
         """
@@ -272,13 +282,14 @@
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method to check it object has been modified.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     def __str__(self):
         return "Queue {0}".format(self.queue_number)
```

### Comparing `pyaoscx-2.3.1/pyaoscx/queue_profile.py` & `pyaoscx-2.4.0/pyaoscx/queue_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2021-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2021-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
 from pyaoscx.exceptions.response_error import ResponseError
@@ -51,14 +51,15 @@
         return self.__name
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a Queue profile and fill
             the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information
             to return.
         :return: Returns True if no exception is raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -77,14 +78,15 @@
         return True
 
     @classmethod
     def get_all(cls, session):
         """
         Perform a GET call to retrieve all Queue profiles and create a
             dictionary containing each of them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :return: Dictionary containing Queue profile names as keys and a Queue
             profile object as value.
         """
         logging.info("Retrieving all %s data from switch", cls.__name__)
@@ -111,41 +113,44 @@
 
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update an existing Queue Profile.
             Checks whether the Queue Profile exists in the switch and calls
             self.update() or self.create() accordingly.
-        :return modified: True if the object was modified.
+
+        :return: True if the object was modified.
         """
         if self.materialized:
             return self.update()
         else:
             return self.create()
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing Queue Profile.
-        :return modified: True if the object was modified and a PUT request was
+
+        :return: True if the object was modified and a PUT request was
             made.
         """
         data = utils.get_attrs(self, self.config_attrs)
         # Manually remove the name
         if "name" in data:
             del data["name"]
         self.__modified = self._put_data(data)
         logging.info("SUCCESS: Updating %s", self)
         return self.__modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new Queue profile in the switch.
-        :return modified: True if the object was modified.
+
+        :return: True if the object was modified.
         """
         data = utils.get_attrs(self, self.config_attrs)
         # Manually add the name
         data["name"] = self.name
         self.__modified = self._post_data(data)
         logging.info("SUCCESS: Adding %s", self)
         return self.__modified
@@ -159,28 +164,30 @@
         logging.info("SUCCESS: Deleting %s", self)
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_uri(cls, session, uri):
         """
         Create a Queue profile object given an URI.
+
         :param cls: Object's class.
         :param session: Pyaoscx.Session objec used to represent a logical
             connection to the device.
         :param uri: a string with the URI
-        :return id, object: tuple with the name and the Profile.
+        :return: tuple with the name and the Profile.
         """
         # Obtain the ID from URI
         name = uri.split("/")[-1]
         return name, cls(session, name)
 
     @classmethod
     def get_facts(cls, session):
         """
         Retrieve the information of all Queue profiles.
+
         :param cls: Class reference.
         :param session: Pyaoscx.Session object used to represent a logical
             connection to the device.
         :return: Dictionary containing the name as key and the materialized
             object as value.
         """
         logging.info("Retrieving Queue Profiles facts")
@@ -210,14 +217,15 @@
     def was_modified(self):
         return self.modified
 
     @classmethod
     def set_global_queue_profile(cls, session, profile):
         """
         Sets the global queue profile for the switch.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param profile: Name of a queue profile to set as the global queue
             profile.
         """
         logging.info("Setting global queue profile to: %s", profile)
         device = Device(session)
```

### Comparing `pyaoscx-2.3.1/pyaoscx/queue_profile_entry.py` & `pyaoscx-2.4.0/pyaoscx/queue_profile_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2021-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2021-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
 from pyaoscx.exceptions.response_error import ResponseError
@@ -54,14 +54,15 @@
         return self.__queue_number
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a Queue Profile Entry and fill
             the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information
             to return.
         :return: Returns True if there is not an exception raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -80,14 +81,15 @@
         return True
 
     @classmethod
     def get_all(cls, session, queue_profile_name):
         """
         Perform a GET call to retrieve all Queue Profile Entries  of the same
             profile and create a dictionary containing them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param queue_profile_name: Name of the profile to which the entries
             belong.
         :return: Dictionary containing Queue Profile Entry names as keys
             and a Queue Profile Entry object as value.
@@ -118,40 +120,43 @@
 
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update an existing Queue
             Profile Entry. Checks whether the Queue Profile exists in the
             switch and calls self.update() or self.create() accordingly.
+
         :return modified: True if the object was modified.
         """
         if self.materialized:
             return self.update()
         else:
             return self.create()
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing Queue Profile Entry.
-        :return modified: True if the object was modified and a PUT request was
+
+        :return: True if the object was modified and a PUT request was
             made.
         """
         data = utils.get_attrs(self, self.config_attrs)
         # Manually remove the queue_number
         if "queue_number" in data:
             del data["queue_number"]
         self.__modified = self._put_data(data)
         return self.__modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new Queue Profile Entry in the switch.
-        :return modified: True if the object was modified.
+
+        :return: True if the object was modified.
         """
         data = utils.get_attrs(self, self.config_attrs)
         # Manually add the queue_number
         data["queue_number"] = self.queue_number
         self.__modified = self._post_data(data)
         return self.__modified
 
@@ -163,33 +168,35 @@
         self._send_data(self.path, None, "DELETE", "Delete")
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_uri(cls, session, uri):
         """
         Create a Queue profile object given an URI.
+
         :param cls: Object's class.
         :param session: Pyaoscx.Session objec used to represent a logical
             connection to the device.
         :param uri: a string with the URI.
-        :return id, object: tuple with the name and the Profile.
+        :return: tuple with the name and the Profile.
         """
         # Obtain the ID from URI
         # URI format is /system/q_profile/{name}/q_entry/{queue_number}
         parts = uri.split("/")
         profile_name = parts[-3]
         queue_number = parts[-1]
         profile = QueueProfile(session, profile_name)
         entry = cls(session, queue_number, profile)
         return queue_number, entry
 
     @classmethod
     def get_facts(cls, session, queue_profile_name):
         """
         Retrieve the information of all Queue profiles.
+
         :param cls: Class reference.
         :param session: Pyaoscx.Session object used to represent a logical
             connection to the device.
         :param queue_profile_name: Name of the profile to which the entries
             belong.
         :return: Dictionary containing the name as key and the facts as value.
         """
```

### Comparing `pyaoscx-2.3.1/pyaoscx/rest/v1/api.py` & `pyaoscx-2.4.0/pyaoscx/rest/v1/api.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.3.1/pyaoscx/rest/v1/interface.py` & `pyaoscx-2.4.0/pyaoscx/rest/v1/interface.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.3.1/pyaoscx/rest/v10_04/api.py` & `pyaoscx-2.4.0/pyaoscx/rest/v10_04/api.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.3.1/pyaoscx/rest/v10_08/api.py` & `pyaoscx-2.4.0/pyaoscx/rest/v10_08/api.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.3.1/pyaoscx/rest/v10_09/api.py` & `pyaoscx-2.4.0/pyaoscx/rest/v10_09/api.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.3.1/pyaoscx/session.py` & `pyaoscx-2.4.0/pyaoscx/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import getpass
 import json
 import logging
 import re
 
@@ -27,23 +27,23 @@
         address (both IPv4 and IPv6 are supported), and API version. The IP
         address should be similar to:
         '1.1.1.1'
         or
         '2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff'
     """
 
-    _login_headers = {"Accept": "*/*", "x-use-csrf-token": "true"}
-
     def __init__(self, ip_address, api, proxy=None):
 
         self.api = API.create(api)
         self.ip = ip_address
         self.connected = False
         self.proxy = (
-            {"no_proxy": self.ip} if proxy is None else {"https": proxy}
+            {"no_proxy": self.ip}
+            if proxy is None
+            else {"http": proxy, "https": proxy}
         )
         self.scheme = "https"
         self.version_path = "rest/v{0}/".format(self.api)
 
         # TODO: remove base_url once all modules use the internal
         # request methods
         self.base_url = "https://{0}/rest/v{1}/".format(self.ip, self.api)
@@ -58,20 +58,21 @@
 
     @classmethod
     def from_session(cls, req_session, base_url, credentials=None):
         """
         Create a session from an existing request Session. It allows to create
             an internal session from an already-authenticated and serialized
             session.
+
         :param req_session: Existing Request Session object.
         :param base_url: Url needed to create Session Object.
         :param credentials: Dictionary with user and password credentials.
             Example: {
-                username: <username>,
-                password: <password>
+            username: <username>,
+            password: <password>
             }
         :return session: Request Session Object.
         """
         ip_address = version = ""
 
         # From base url retrieve the ip address and the version
         url_pattern = re.compile(
@@ -106,14 +107,15 @@
         return session
 
     def open(self, username=None, password=None, use_proxy=True):
         """
         Perform a POST call to login and gain access to other API calls. If
             either username or password is not specified, user will be prompted
             to enter the missing credential(s).
+
         :param username: username
         :param password: password
         """
         if self.__username is None:
             if username is None:
                 username = input("Enter username: ")
             else:
@@ -180,14 +182,15 @@
         use_proxy=True,
         handle_zeroized_device=False,
     ):
         """
         Perform a POST call to login and gain access to other API calls. If
             either username or password is not specified, user will be prompted
             to enter the missing credential(s).
+
         :param base_url: URL in main() function
         :param username: username
         :param password: password
         :param use_proxy: Whether the system proxy should be used, defaults to
             True.
         :param handle_zeroized_device: Whether a zeroized device should be
             initialized, if so sets the admin password to the provided one,
@@ -195,30 +198,31 @@
         :return: requests.session object with loaded cookie jar
         """
         if username is None and password is None:
             username = input("Enter username: ")
             password = getpass.getpass()
 
         login_data = {"username": username, "password": password}
+        login_headers = {"Accept": "*/*", "x-use-csrf-token": "true"}
 
         s = requests.Session()
+        o = requests.utils.urlparse(base_url)
 
         if use_proxy is False:
-            s.proxies["https"] = None
-            s.proxies["http"] = None
+            s.proxies["no_proxy"] = o.hostname
 
         try:
             print(base_url + "login")
             response = s.post(
                 base_url + "login",
                 data=login_data,
                 verify=False,
                 timeout=5,
                 proxies=s.proxies,
-                headers=cls._login_headers,
+                headers=login_headers,
             )
             cls.__assign_csrftoken(response, s)
         except requests.exceptions.ConnectTimeout:
             logging.warning(
                 "ERROR: Error connecting to host: "
                 "connection attempt timed out."
             )
@@ -237,15 +241,15 @@
                 ztp_login_data = {"username": username}
                 response = s.post(
                     base_url + "login",
                     data=ztp_login_data,
                     verify=False,
                     timeout=5,
                     proxies=s.proxies,
-                    headers=cls._login_headers,
+                    headers=login_headers,
                 )
                 cls.__assign_csrftoken(response, s)
                 if response.status_code == ZEROIZED:
                     data = {"password": password}
                     response = s.put(
                         base_url + "system/users/admin",
                         data=json.dumps(data),
@@ -271,17 +275,18 @@
             logging.info("SUCCESS: Login succeeded")
             return s
 
     @classmethod
     def logout(cls, **kwargs):
         """
         Perform a POST call to logout and end session.
+
         :param kwargs:
-            keyword s: requests.session object with loaded cookie jar
-            keyword url: URL in main() function
+            keyword "s" requests.session object with loaded cookie jar
+            keyword "url" URL in main() function
         :return: True if successful.
         """
         response = kwargs["s"].post(
             kwargs["url"] + "logout", verify=False, proxies=kwargs["s"].proxies
         )
         # Response OK check needs to be passed 'PUT' since this POST
         # call returns 200 instead of conventional 201
@@ -295,40 +300,44 @@
         else:
             logging.info("SUCCESS: Logout succeeded")
             return True
 
     def username(self):
         """
         Get username.
+
         :return username.
         """
         return self.__username
 
     def password(self):
         """
         Get password.
+
         :return password.
         """
         return self.__password
 
     def _build_uri(self, resource_path):
         """
         Build a URI representing a resource.
+
         :param resource_path: Resource path before adding version prefix.
         :return: String of the uri
         """
         complete_path = self.version_path + resource_path
         uri = requests.utils.urlunparse(
             (self.scheme, self.ip, complete_path, "", "", "")
         )
         return uri
 
     def request(self, operation, path, params=None, data=None, verify=False):
         """
         Perform a Request to the switch.
+
         :param operation: type of operation: PUT, GET, POST, DELETE.
         :param path: Path to the resource.
         :param params: Extra request parameters.
         :param data: Data to send in the resquest.
         :param verify: If session should verify.
         :return: response object from the request.
         """
```

### Comparing `pyaoscx-2.3.1/pyaoscx/static_nexthop.py` & `pyaoscx-2.4.0/pyaoscx/static_nexthop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 import re
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
@@ -43,15 +43,16 @@
         # Attribute used to know if object was changed recently
         self.__modified = False
 
     def __set_static_route(self, parent_static_route):
         """
         Set parent StaticRoute object as an attribute for the StaticNexthop
             object.
-        :param parent_static_route a Static_Route object.
+
+        :param parent_static_route: a Static_Route object.
         """
         # Set parent Static Route
         self.__parent_static_route = parent_static_route
 
         # Set URI
         self.base_uri = "{0}/{1}/static_nexthops".format(
             self.__parent_static_route.base_uri,
@@ -68,14 +69,15 @@
                 self.__parent_static_route.static_nexthops.append(self)
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a Static Nexthop table entry
             and fill the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if there is no exception is raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -142,14 +144,15 @@
 
     @classmethod
     def get_all(cls, session, parent_static_route):
         """
         Perform a GET call to retrieve all system Static Nexthop objects
             related to a Static Route, and create a dictionary containing
             StaticNexthop objects.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_static_route: StaticRoute object, parent for the Static
             Nexthops.
         :return: Dictionary containing Static Nexthop IDs as keys and a Static
             NexthopThis objects as values.
@@ -189,15 +192,16 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update an existing Static Nexthop.
             Checks whether the static_nexthop exists in the switch. Calls
             self.update() if Static Nexthop being updated. Calls self.create()
             if a new Static Nexthop is being created.
-        :return modified: Boolean, True if object was created or modified.
+
+        :return: Boolean, True if object was created or modified.
         """
         if not self.__parent_static_route.materialized:
             self.__parent_static_route.apply()
 
         modified = False
         if self.materialized:
             modified = self.update()
@@ -207,14 +211,15 @@
         self.__modified = modified
         return modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing static_nexthop.
+
         :return modified: True if Object was modified and a PUT request was
             made.
         """
         # Variable returned
         modified = False
 
         static_nexthop_data = utils.get_attrs(self, self.config_attrs)
@@ -254,15 +259,16 @@
         return modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new static_nexthop. Only returns if no
             exception is raised.
-        :return modified: Boolean, True if entry was created
+
+        :return: Boolean, True if entry was created
         """
         static_nexthop_data = utils.get_attrs(self, self.config_attrs)
         static_nexthop_data["id"] = self.id
 
         # Get port uri
         if hasattr(self, "port") and self.port:
             static_nexthop_data["port"] = self.port.get_info_format()
@@ -316,42 +322,44 @@
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, parent_static_route, response_data):
         """
         Create a StaticNexthop object given a response_data related to the
             Static Nexthop ID object.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_static_route: parent StaticRoute object where Static
             Nexthop is stored.
         :param response_data: The response must be a dictionary of the form:
             {
-                id: "/rest/v10.04/system/static_routes/static_nexthops/id"
+            id: "/rest/v10.04/system/static_routes/static_nexthops/id"
             }
         :return: StaticNexthop object.
         """
         static_nexthop_arr = session.api.get_keys(
             response_data, StaticNexthop.resource_uri_name
         )
         _id = static_nexthop_arr[0]
         return StaticNexthop(session, _id, parent_static_route)
 
     @classmethod
     def from_uri(cls, session, parent_static_route, uri):
         """
         Create a StaticNexthop object given a URI.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_static_route: parent static_route class where
             static_nexthop is stored.
         :param uri: a String with a URI.
-        :return index, static_nexthop: tuple containing both the Static Nexthop
+        :return: tuple containing both the Static Nexthop
             object and the Static Nexthop's ID.
         """
         # Obtain ID from URI
         index_pattern = re.compile(r"(.*)static_nexthops/(?P<index>.+)")
         index = index_pattern.match(uri).group("index")
 
         # Create static_nexthop object
@@ -364,15 +372,16 @@
     def __str__(self):
         return "Static Nexthop: {0}".format(self.id)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific Static Nexthop URI.
-        return: Object's URI.
+
+        :return: Object's URI.
         """
         if self._uri is None:
             self._uri = "{0}{1}/{2}".format(
                 self.session.resource_id,
                 self.base_uri,
                 self.id,
             )
@@ -380,45 +389,48 @@
         return self._uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
-        return: Object format depending on the API Version
+
+        :return: Object format depending on the API Version
         """
         return self.session.api.get_index(self)
 
     @property
     def modified(self):
         """
         Return boolean with whether this object has been modified.
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     @classmethod
     def get_next_id(cls, session, parent_static_route):
         """
         Method used to obtain the ID for the next Static Nexthop. Thus perform
             a GET call to retrieve all system Static Nexthop inside a Static
             Route, and with it determine the next ID.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_static_route: StaticRoute object, parent for the Static
             Nexthops.
-        :return new_id: Integer with the new Id for the next Static Nexthop.
+        :return: Integer with the new Id for the next Static Nexthop.
         """
         logging.info("Retrieving the switch static_nexthop")
 
         uri = "{0}/{1}/static_nexthops".format(
             parent_static_route.base_uri, parent_static_route.reference_address
         )
```

### Comparing `pyaoscx-2.3.1/pyaoscx/static_route.py` & `pyaoscx-2.4.0/pyaoscx/static_route.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 import re
 
 from urllib.parse import quote_plus, unquote_plus
@@ -51,14 +51,15 @@
 
         # Attribute used to know if object was changed recently
         self.__modified = False
 
     def __set_vrf(self, parent_vrf):
         """
         Set parent Vrf object as an attribute for the StaticRoute object.
+
         :param parent_vrf: a Vrf object.
         """
         # Set parent Vrf object
         self.__parent_vrf = parent_vrf
 
         # Set URI
         self.base_uri = "{0}/{1}/static_routes".format(
@@ -76,14 +77,15 @@
                 self.__parent_vrf.static_routes.append(self)
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a Static Route table entry and
             fill the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if there is not an exception raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -150,14 +152,15 @@
         return True
 
     @classmethod
     def get_all(cls, session, parent_vrf):
         """
         Perform a GET call to retrieve all system Static Routes inside a VRF,
             and create a dictionary containing them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_vrf: parent Vrf object where vrf is stored.
         :return: Dictionary containing Static Route IDs as keys and a Static
             Route objects as values.
         """
@@ -195,15 +198,16 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create a new or update an existing Static
             Route table entry. Checks whether the Static Route exists in the
             switch. Calls self.update() if object being updated. Calls
             self.create() if a new Static Route is being created.
-        :return modified: Boolean, True if object was created or modified.
+
+        :return: Boolean, True if object was created or modified.
         """
         if not self.__parent_vrf.materialized:
             self.__parent_vrf.apply()
 
         modified = False
         if self.materialized:
             modified = self.update()
@@ -214,15 +218,16 @@
         return modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing Static Route table
             entry.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         # Variable returned
         modified = False
 
         static_route_data = utils.get_attrs(self, self.config_attrs)
 
@@ -257,14 +262,15 @@
         return modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new Static Route table entry. Only
             returns if no exception is raised.
+
         :return: Boolean, True if entry was created
         """
         # Add 'address_family' as a config attribute and remove duplicates
         self.config_attrs.append("address_family")
         self.config_attrs = list(set(self.config_attrs))
 
         static_route_data = utils.get_attrs(self, self.config_attrs)
@@ -318,40 +324,42 @@
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, parent_vrf, response_data):
         """
         Create a StaticRoute object given a response_data related to the Static
             Route prefix object.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_vrf: parent Vrf object where Static Route is stored.
         :param response_data: The response must be a dictionary of the form:
             {
-                prefix: "/rest/v10.04/system/vrfs/static_routes/prefix"
+            prefix: "/rest/v10.04/system/vrfs/static_routes/prefix"
             }
         :return: Static Route Object.
         """
         static_route_arr = session.api.get_keys(
             response_data, StaticRoute.resource_uri_name
         )
         prefix = static_route_arr[0]
         return StaticRoute(session, prefix, parent_vrf)
 
     @classmethod
     def from_uri(cls, session, parent_vrf, uri):
         """
         Create a StaticRoute object given a URI.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_vrf: parent Vrf object where Static Route is stored.
         :param uri: a String with a URI.
-        :return index, static_route: tuple containing both the static_route
+        :return: tuple containing both the static_route
             object and the static_route's prefix.
         """
         # Obtain ID from URI
         index_pattern = re.compile(r"(.*)static_routes/(?P<index>.+)")
         index = index_pattern.match(uri).group("index")
 
         # Create StaticRoute object
@@ -362,15 +370,16 @@
     def __str__(self):
         return "Static Route: {0}".format(self.prefix)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific static route URI.
-        return: Object's URI.
+
+        :return: Object's URI.
         """
         if self._uri is None:
             self._uri = "{0}{1}/{2}".format(
                 self.session.resource_prefix,
                 self.base_uri,
                 self.reference_address,
             )
@@ -378,29 +387,31 @@
         return self._uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
-        return: Object format depending on the API Version.
+
+        :return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     @property
     def modified(self):
         """
         Return boolean with whether this object has been modified.
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     ####################################################################
     # IMPERATIVE FUNCTIONS
     ####################################################################
@@ -412,20 +423,21 @@
         distance=None,
         nexthop_type=None,
         bfd_enable=None,
     ):
         """
         Create a Static Nexthop, with a VRF and a Destination Address related
             to a Static Route.
+
         :param next_hop_ip_address: The IPv4 address or the IPv6 address of
             next hop.
             Example:
-                '1.1.1.1'
-                or
-                '2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff'
+            '1.1.1.1'
+            or
+            '2001:db8::11/ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff'
         :param next_hop_interface: The interface through which the next hop
             can be reached.
         :param distance: Administrative distance to be used for the next
             hop in the static route instead of default value.
         :param nexthop_type: Specifies whether the static route is a forward,
             blackhole or reject route.
         :param bfd_enable: Boolean to enable BFD.
```

### Comparing `pyaoscx-2.3.1/pyaoscx/tunnel_endpoint.py` & `pyaoscx-2.4.0/pyaoscx/tunnel_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         self.path = self.object_uri.format(**uri_indices)
         self.__modified = False
 
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a TEP table entry and fill the
             object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if no exception is raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -83,14 +84,15 @@
         return True
 
     @classmethod
     def get_all(cls, session, parent_interface):
         """
         Perform a GET call to retrieve all Tunnel Endpoints and create a
             dictionary containing each respective TEP.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_interface: Interface attached to this tunnel
         :return: Dictionary containing TEP IDs as keys and a TEP object as
             value.
         """
@@ -116,39 +118,42 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create a TEP, or update an existing one.
             Checks whether the TEP exists in the switch. Calls self.update()
             if TEP is being updated. Calls self.create() if the TEP doesn't
             exist in the switch.
-        :return modified: Boolean, True if object was created or modified.
+
+        :return: Boolean, True if object was created or modified.
         """
         if self.materialized:
             return self.update()
         return self.create()
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing TEP table entry.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         tep_data = {}
         tep_data["network_id"] = self.network_id.get_info_format()
         self.__modified = self._put_data(tep_data)
         return self.__modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new TEP using the object's attributes
             as POST body. Exception is raised if object is unable to be
             created.
-        :return modified: Boolean, True if TEP was created.
+
+        :return: Boolean, True if TEP was created.
         """
         tep_data = {}
         tep_data["destination"] = self.destination
         tep_data["interface"] = self.interface.get_info_format()
         tep_data["network_id"] = self.network_id.get_info_format()
         tep_data["origin"] = self.origin
         tep_data["vrf"] = self.vrf.get_info_format()
@@ -209,35 +214,38 @@
 
         return tep.tep_id, tep
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific TEP URI.
-        return: Object's URI.
+
+        :return: Object's URI.
         """
         uri = "{0}{1}".format(self.session.resource_prefix, self.path)
         return uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
-        return: Object format depending on the API Version.
+
+        :return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     @property
     def modified(self):
         """
         Return boolean with whether this object has been modified.
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
```

### Comparing `pyaoscx-2.3.1/pyaoscx/utils/list_attributes.py` & `pyaoscx-2.4.0/pyaoscx/utils/list_attributes.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.3.1/pyaoscx/vlan.py` & `pyaoscx-2.4.0/pyaoscx/vlan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 import random
 import re
 
@@ -53,14 +53,15 @@
         self.path = "{0}/{1}".format(Vlan.base_uri, self.id)
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a VLAN table entry and fill the
             object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if no exception is raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -130,14 +131,15 @@
         return True
 
     @classmethod
     def get_all(cls, session):
         """
         Perform a GET call to retrieve all system VLAN and create a dictionary
             containing each respective VLAN.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :return: Dictionary containing VLAN IDs as keys and a Vlan object as
             value.
         """
         logging.info("Retrieving all %s data from switch", cls.__name__)
@@ -167,14 +169,15 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create a VLAN, or update an existing one.
             Checks whether the VLAN exists in the switch. Calls self.update()
             if VLAN is being updated. Calls self.create() if the VLAN doesn't
             exist in the switch.
+
         :return modified: Boolean, True if object was created or modified.
         """
         modified = False
         if self.materialized:
             modified = self.update()
         else:
             modified = self.create()
@@ -182,14 +185,15 @@
         self.__modified = modified
         return modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing VLAN table entry.
+
         :return modified: True if Object was modified and a PUT request was
             made.
         """
         vlan_data = utils.get_attrs(self, self.config_attrs)
 
         # Set all ACLs
         if "aclmac_in_cfg" in vlan_data and self.aclmac_in_cfg is not None:
@@ -208,14 +212,15 @@
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new VLAN using the object's attributes
             as POST body. Exception is raised if object is unable to be
             created.
+
         :return modified: Boolean, True if VLAN was created.
         """
         # Get all VLAN data given by the user
         vlan_data = utils.get_attrs(self, self.config_attrs)
         if isinstance(self.id, str):
             self.id = int(self.id)
         vlan_data["id"] = self.id
@@ -231,33 +236,35 @@
         # Delete object attributes
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, response_data):
         """
         Create a Vlan object given a response_data related to the Vlan object.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param response_data: The response must be a dictionary of the form:
             {
-                1: "/rest/v10.04/system/vlans/1"
+            1: "/rest/v10.04/system/vlans/1"
             }
         :return: Vlan Object.
         """
         vlan_id_arr = session.api.get_keys(
             response_data, Vlan.resource_uri_name
         )
         vlan_id = vlan_id_arr[0]
         return Vlan(session, vlan_id)
 
     @classmethod
     def from_uri(cls, session, uri):
         """
         Create a Vlan object given a VLAN URI.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param uri: a String with a URI.
         :return vlan_id, vlan: tuple with the Vlan object its ID.
         """
         # Obtain ID from URI
@@ -270,14 +277,15 @@
         return vlan_id, vlan_obj
 
     @classmethod
     def get_facts(cls, session):
         """
         Modify this to Perform a GET call to retrieve all VLANs and their
             respective data.
+
         :param cls: Class reference.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :return facts: Dictionary containing VLAN IDs as keys and Vlan objects
             as values.
         """
         logging.info("Retrieving switch VLANs facts")
@@ -320,28 +328,30 @@
         except Exception:
             return "Vlan, ID: '{0}'".format(self.id)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific VLAN URI.
+
         return: Object's URI.
         """
         if self._uri is None:
             self._uri = "{0}{1}/{2}".format(
                 self.session.resource_prefix, Vlan.base_uri, self.id
             )
 
         return self._uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
+
         return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     @property
     def modified(self):
         """
@@ -349,25 +359,27 @@
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     ####################################################################
     # IMPERATIVE FUNCTIONS
     ####################################################################
 
     def modify(self, vlan_name=None, vlan_desc=None, admin_conf_state=None):
         """
         Perform a PUT calls to modify an existing VLAN.
+
         :param vlan_name: Optional Alphanumeric name of VLAN. Won't be modified
             if not specified.
         :param vlan_desc: Optional description to add to VLAN. Won't be
             modified if not specified.
         :param admin_conf_state: Optional administratively-configured state of
             VLAN. Won't be modified if not specified. Only configurable for
             static VLANs.
@@ -385,14 +397,15 @@
 
         # Apply changes inside switch
         return self.apply()
 
     def attach_acl_in(self, acl_name, list_type):
         """
         Update ACL IN values inside a Vlan object.
+
         :param acl_name: Alphanumeric String that is the name of the ACL.
         :param list_type: Alphanumeric String of ipv4, ipv6, or mac to specify
             the type of ACL.
         :return: True if object was changed.
         """
         # Create Acl object
         acl_obj = self.session.api.get_module(
@@ -420,14 +433,15 @@
 
         # Apply changes
         return self.apply()
 
     def attach_acl_out(self, acl_name, list_type):
         """
         Update ACL OUT values inside a Vlan object.
+
         :param acl_name: Alphanumeric String that is the name of the ACL.
         :param list_type: Alphanumeric String of ipv4, ipv6, or mac to specify
             the type of ACL.
         :return: True if object was changed.
         """
         # Create Acl object
         acl_obj = self.session.api.get_module(
@@ -455,14 +469,15 @@
 
         # Apply changes
         return self.apply()
 
     def detach_acl_in(self, acl_name, list_type):
         """
         Detach an ACL from a VLAN.
+
         :param acl_name: Alphanumeric String that is the name of the ACL.
         :param list_type: Alphanumeric String of ipv4, ipv6, or mac to specify
             the type of ACL.
         :return: True if object was changed.
         """
         if list_type == "ipv6":
             self.aclv6_in_cfg = None
@@ -476,14 +491,15 @@
 
         # Apply changes
         return self.apply()
 
     def detach_acl_out(self, acl_name, list_type):
         """
         Detach an ACL from a VLAN.
+
         :param acl_name: Alphanumeric String that is the name of the ACL.
         :param list_type: Alphanumeric String of ipv4, ipv6, or mac to specify
             the type of ACL.
         :return: True if object was changed.
         """
         if list_type == "ipv6":
             self.aclv6_out_cfg = None
@@ -497,14 +513,15 @@
 
         # Apply changes
         return self.apply()
 
     def get_mac(self, from_id, mac_address):
         """
         Create an Mac object.
+
         :param from_id: String source of the MAC address. Must be "dynamic",
             "VSX", "static", "VRRP", "port-access-security", "evpn", or "hsc".
         :param mac_address: String MAC address. Example: '01:02:03:04:05:06'
         :return: Mac object.
         """
         mac_obj = self.session.api.get_module(
             self.session,
@@ -517,14 +534,15 @@
         # Get MAC data
         mac_obj.get()
         return mac_obj
 
     def add_static_mac(self, port, mac_address):
         """
         Create an StaticMac object.
+
         :param port: String for the Port's name. Example: 1/1/1
         :param mac_address: String MAC address. Example: '01:02:03:04:05:06'
         :return: StaticMac object
         """
         if isinstance(port, str):
             # Make Interface into an object
             port = self.session.api.get_module(self.session, "Interface", port)
```

### Comparing `pyaoscx-2.3.1/pyaoscx/vni.py` & `pyaoscx-2.4.0/pyaoscx/vni.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         self.path = self.object_uri.format(**uri_indices)
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for VNI table entry and fill
             the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if there is not an exception raised
         """
         logging.info("Retrieving %s from switch", self)
@@ -103,14 +104,15 @@
         return True
 
     @classmethod
     def get_all(cls, session, parent_intf):
         """
         Perform a GET call to retrieve all system VNI and create a dictionary
             containing each respective VNI
+
         :param cls: Object's class
         :param session: pyaoscx.Session object used to represent a logical
             connection to the switch
         :param parent_intf: Interface attached to this tunnel
         :return: Dictionary containing VNI IDs and a VNI object as value
         """
         logging.info("Retrieving all %s data from switch", cls.__name__)
@@ -133,25 +135,27 @@
         return vni_collection
 
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update a
             VNI table entry
+
         :return: True if the object was modified
         """
         if self.materialized:
             return self.update()
         return self.create()
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing VNI table entry
-        :return modified: True if object was modified and a PUT request was
+
+        :return: True if object was modified and a PUT request was
             made. False otherwise
         """
         vni_data = utils.get_attrs(self, self.config_attrs)
         vni_data["interface"] = self.__interface.get_info_format()
         if hasattr(self, "routing"):
             vni_data["routing"] = self.routing
         if hasattr(self, "vrf") and self.vrf:
@@ -163,15 +167,16 @@
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new VNI using the object's
             attributes as POST body. Exception is raised if object is unable
             to be created
-        :return modified: Boolean, True if entry was created
+
+        :return: Boolean, True if entry was created
         """
         vni_data = utils.get_attrs(self, self.config_attrs)
         vni_data["id"] = self.id
         vni_data["interface"] = self.__interface.get_info_format()
         vni_data["type"] = self.type
         if hasattr(self, "routing"):
             vni_data["routing"] = self.routing
@@ -190,14 +195,15 @@
         self._send_data(self.path, None, "DELETE", "Delete")
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, parent_intf, response_data):
         """
         Create a VNI object given a response_data related to a VNI object
+
         :param cls: Object's class
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device
         :param parent_intf: Interface attached to this tunnel
         :param response_data: The response must be a dictionary of the form:
             {id: URL}
         :return: VNI object
@@ -206,20 +212,21 @@
 
         return cls.from_uri(session, parent_intf, uri)
 
     @classmethod
     def from_uri(cls, session, parent_intf, uri):
         """
         Create a Vni object given a VNI URI
+
         :param cls: Object's class
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device
         :param parent_intf: Interface attached to this tunnel
         :param uri: A String with a URI
-        :return VNI_ids, Vni: tuple containing the VNI ids (type, and actual
+        :return: tuple containing the VNI ids (type, and actual
             ID) and the VNI object.
         """
         index_pattern = re.compile(
             r"(.*)virtual_network_ids/(?P<vni_type>.+),(?P<vni_id>.+)"
         )
         pattern_match = index_pattern.match(uri)
         vni_id = pattern_match.group("vni_id")
@@ -231,48 +238,59 @@
     def __str__(self):
         return "VNI {0}, type {1}".format(self.id, self.type)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific VNI URI
+
         :return: Object's URI
         """
         uri = "{0}{1}".format(self.session.resource_prefix, self.path)
         return uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method to obtain correct object format for referencing inside
             other objects
-        return: Object format depending on the API Version
+
+        :return: Object format depending on the API Version
         """
         return self.session.api.get_index(self)
 
     @property
     def modified(self):
         """
         Return boolean with whether this object has been modified.
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     @property
     def interface(self):
+        """
+        Getter method for the interface attribute.
+
+        :return: Interface object for method.
+        """
         return self.__interface
 
     @interface.setter
     def interface(self, new_interface):
+        """
+        Setter method for the interface attribute.
+        """
         if self.type == "vxlan_vni" and new_interface.type != "vxlan":
             raise VerificationError(
                 "Incompatible VNI and Interface types: "
                 "{0} and {1}".format(self.type, new_interface.type)
             )
         self.__interface = new_interface
```

### Comparing `pyaoscx-2.3.1/pyaoscx/vrf.py` & `pyaoscx-2.4.0/pyaoscx/vrf.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         self.__modified = False
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a VRF table entry and fill the
             class with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information
             to return.
         :return: Returns True if no exception is raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -213,14 +214,15 @@
         return True
 
     @classmethod
     def get_all(cls, session):
         """
         Perform a GET call to retrieve all system VRFs and create a dictionary
             containing them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :return: Dictionary containing VRF names as keys and a Vrf objects as
             values.
         """
         logging.info("Retrieving all %s data from switch", cls.__name__)
@@ -250,14 +252,15 @@
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update an existing VRF table
             entry. Checks whether the VRF exists in the switch. Calls
             self.update() if VRF is being updated. Calls self.create() if a new
             VRF is being created.
+
         :return modified: Boolean, True if object was created or modified.
         """
         modified = False
         if self.materialized:
             modified = self.update()
         else:
             modified = self.create()
@@ -265,14 +268,15 @@
         self.__modified = modified
         return modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing VRF table entry.
+
         :return modified: True if Object was modified and a PUT request was
             made.
         """
         vrf_data = utils.get_attrs(self, self.config_attrs)
 
         uri = "{0}/{1}".format(Vrf.base_uri, self.name)
 
@@ -305,14 +309,15 @@
         return modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new VRF using the object's attributes
             as POST body. Only returns if no exception is raised.
+
         :return modified: Boolean, True if entry was created
         """
         vrf_data = utils.get_attrs(self, self.config_attrs)
 
         vrf_data["name"] = self.name
 
         post_data = json.dumps(vrf_data)
@@ -356,20 +361,21 @@
 
         logging.info("SUCCESS: Deleting %s", self)
 
     @classmethod
     def from_response(cls, session, response_data):
         """
         Create a Vrf object given a response_data related to the Vrf object.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param response_data: The response must be a dictionary of the form:
             {
-                "test_vrf": "/rest/v10.04/system/vrfs/test_vrf"
+            "test_vrf": "/rest/v10.04/system/vrfs/test_vrf"
             }
         :return: Vrf object
         """
         # An interfaces's VRF is returned with an empty index in some
         # switch models (confirmed with a 4100), this empty index causes a
         # subsequent GET request to fail, because the constructed URI is
         # not correct, this may be due to these models supporting a single
@@ -387,14 +393,15 @@
             vrf_name = vrf_name_arr[0]
         return cls(session, vrf_name)
 
     @classmethod
     def from_uri(cls, session, uri):
         """
         Create a Vrf object given a VRF URI.
+
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param uri: a String with a URI.
         :return name, vrf_obj: tuple containing both the VRF's name and a Vrf
             object.
         """
         # Obtain ID from URI
@@ -406,14 +413,15 @@
         return name, vrf_obj
 
     @classmethod
     def get_facts(cls, session):
         """
         Modify this to Perform a GET call to retrieve all VRFs and their
             respective data.
+
         :param cls: Class reference.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :return facts: Dictionary containing VRF IDs as keys and VRF objects as
             values.
         """
         logging.info("Retrieving switch VRF facts")
@@ -438,14 +446,15 @@
 
         return facts
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific VRF URI.
+
         return: Object's URI.
         """
         if self._uri is None:
             self._uri = "{0}{1}/{2}".format(
                 self.session.resource_prefix,
                 Vrf.base_uri,
                 self.name,
@@ -454,14 +463,15 @@
         return self._uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
+
         return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     def __str__(self):
         return "VRF name: '{0}'".format(self.name)
 
@@ -472,27 +482,29 @@
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
 
     ####################################################################
     # IMPERATIVE FUNCTIONS
     ####################################################################
 
     def add_address_family(
         self, family_type="ipv4_unicast", export_target=[], import_targets=[]
     ):
         """
         Add a VRF Address Family to the current Vrf object.
+
         :param family_type: Alphanumeric type of the Address Family.
             The options are 'ipv4_unicast' and 'ipv6_unicast'.
             The default value is set to 'ipv4_unicast'.
         :param export_target: Optional list of export route targets.
         :param import_targets: Optional list of import route targets
         :return address_family: VrfAddressFamily Object
         """
@@ -528,14 +540,15 @@
         self.apply()
 
         return vrf_address_family
 
     def delete_address_family(self, family_type="ipv4_unicast"):
         """
         Given an address family type, delete that address from the current Vrf.
+
         :param family_type: Alphanumeric type of the Address Family.
             The options are 'ipv4_unicast' and 'ipv6_unicast'.
             A VrfAddressFamily object is accepted.
             The default value is set to 'ipv4_unicast'.
         """
         if not self.materialized:
             raise VerificationError(
@@ -563,41 +576,42 @@
         domain_list=None,
         domain_servers=None,
         host_v4_address_mapping=None,
         host_v6_address_mapping=None,
     ):
         """
         Setup DNS client configuration within a VRF.
+
         :param domain_name: Domain name used for name resolution by the DNS
             client, if 'dns_domain_list' is not configured.
         :param domain_list: dict of DNS Domain list names to be used for
             address resolution, keyed by the resolution priority order.
             Example:
-                {
-                    0: "hpe.com"
-                    1: "arubanetworks.com"
-                }
+            {
+            0: "hpe.com"
+            1: "arubanetworks.com"
+            }
         :param domain_servers: dict of DNS Name servers to be used for address
             resolution, keyed by the resolution priority order. Example:
-                {
-                    0: "4.4.4.10"
-                    1: "4.4.4.12"
-                }
+            {
+            0: "4.4.4.10"
+            1: "4.4.4.12"
+            }
         :param host_v4_address_mapping: dict of static host
             address configurations and the IPv4 address associated with them.
             Example:
-                {
-                    "host1": "5.5.44.5"
-                    "host2": "2.2.44.2"
-                }
+            {
+            "host1": "5.5.44.5"
+            "host2": "2.2.44.2"
+            }
         :param host_v6_address_mapping: dict of static host address
             configurations and the IPv6 address associated with them. Example:
-                {
-                    "host1": "2001:0db8:85a3:0000:0000:8a2e:0370:7334"
-                }
+            {
+            "host1": "2001:0db8:85a3:0000:0000:8a2e:0370:7334"
+            }
         :return modified: Returns True if modified.
         """
         # Update Values
 
         if domain_name is not None:
             self.dns_domain_name = domain_name
 
@@ -621,14 +635,15 @@
         domain_list=None,
         domain_servers=None,
         host_v4_address_mapping=None,
         host_v6_address_mapping=None,
     ):
         """
         Delete DNS client configuration within a Vrf object.
+
         :param domain_name: If value is not None, it is deleted
         :param domain_list: If value is not None, it is deleted
         :param domain_servers: If value is not None, it is deleted
         :param host_v4_address_mapping: If value is not None, it is deleted
         :param host_v6_address_mapping: If value is not None, it is deleted
         :return modified: Returns True if modified.
         """
```

### Comparing `pyaoscx-2.3.1/pyaoscx/vrf_address_family.py` & `pyaoscx-2.4.0/pyaoscx/vrf_address_family.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 import re
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
@@ -64,14 +64,15 @@
         self.path = self.object_uri.format(**uri_indices)
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a VRF Address Family table
             entry and fill the object with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if no exception is raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -127,14 +128,15 @@
         return True
 
     @classmethod
     def get_all(cls, session, parent_vrf):
         """
         Perform a GET call to retrieve all system VRF Address Families inside a
             VRF, and create a dictionary containing them.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_vrf: Vrf object where VRF Address Families are stored.
         :return: Dictionary containing VRF Address Family IDs as keys and a
             VrfAddressFamily objects as values.
         """
@@ -174,15 +176,16 @@
     def apply(self):
         """
         Main method used to either create or update an existing
             VrfAddressFamily object. Checks whether the VRF Address Family
             exists in the switch. Calls self.update() if VRF Address Family
             being updated. Calls self.create() if a new VRF Address Family is
             being created.
-        :return modified: Boolean, True if object was created or modified.
+
+        :return: Boolean, True if object was created or modified.
         """
         if not self.parent_vrf.materialized:
             self.parent_vrf.apply()
 
         modified = False
 
         if self.materialized:
@@ -194,15 +197,16 @@
         return modified
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing VRF Address Family
             table entry.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         vrf_address_family_data = utils.get_attrs(self, self.config_attrs)
 
         uri = "{0}/{1}".format(self.base_uri, self.address_family)
 
         # Compare dictionaries
@@ -233,15 +237,16 @@
         return modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new VRF Address Family table entry.
             Only returns if no exception raised.
-        return: True if entry was created
+
+        :return: True if entry was created
         """
         vrf_address_family_data = utils.get_attrs(self, self.config_attrs)
         vrf_address_family_data["address_family"] = self.address_family
 
         post_data = json.dumps(vrf_address_family_data)
 
         try:
@@ -289,42 +294,44 @@
         utils.delete_attrs(self, self.config_attrs)
 
     @classmethod
     def from_response(cls, session, parent_vrf, response_data):
         """
         Create a VrfAddressFamily object given a response_data related to the
             VRF Address Family's address_family.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_vrf: parent Vrf object where VrfAddressFamlily object is
             stored.
         :param response_data: The response must be a dictionary of the form:
             {
-                addr_fam: <URL>
+            addr_fam: <URL>
             }
             with URL: "/rest/v10.04/system/vrfs/vrf_address_families/addr_fam"
         :return: VrfAddressFamily object.
         """
         vrf_address_family_arr = session.api.get_keys(
             response_data, VrfAddressFamily.resource_uri_name
         )
         address_family = vrf_address_family_arr[0]
         return VrfAddressFamily(session, address_family, parent_vrf)
 
     @classmethod
     def from_uri(cls, session, parent_vrf, uri):
         """
         Create a VrfAddressFamily object given a URI and parent VRF.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param parent_vrf: parent vrf class where VRF Address Family is stored.
         :param uri: a String with a URI.
-        :return index, vrf_address_family_obj: tuple containing both the VRF
+        :return: tuple containing both the VRF
             Address Family object and the VRF Address Family's address_family.
         """
         # Obtain ID from URI
         index_pattern = re.compile(r"(.*)vrf_address_families/(?P<index>.+)")
         index = index_pattern.match(uri).group("index")
         # Create VrfAddressFamily object
         vrf_address_family_obj = VrfAddressFamily(
@@ -336,15 +343,16 @@
     def __str__(self):
         return "VRF Address Family ID {0}".format(self.address_family)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific VRF Address Family URI.
-        return: Object's URI.
+
+        :return: Object's URI.
         """
         if self._uri is None:
             self._uri = "{0}{1}/{2}".format(
                 self.session.resource_prefix,
                 self.base_uri,
                 self.address_family,
             )
@@ -352,25 +360,27 @@
         return self._uri
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Method used to obtain correct object format for referencing inside
             other objects.
-        return: Object format depending on the API Version.
+
+        :return: Object format depending on the API Version.
         """
         return self.session.api.get_index(self)
 
     @property
     def modified(self):
         """
         Return boolean with whether this object has been modified.
         """
         return self.__modified
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: Boolean True if the object was recently modified.
         """
         return self.modified
```

### Comparing `pyaoscx-2.3.1/pyaoscx/vsx.py` & `pyaoscx-2.4.0/pyaoscx/vsx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import logging
 
 from pyaoscx.utils import util as utils
 
 from pyaoscx.pyaoscx_module import PyaoscxModule
@@ -38,14 +38,15 @@
         return vrf.get_info_format()
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for a VSX table entry and fill the
             class with the incoming attributes.
+
         :param depth: Integer deciding how many levels into the API JSON that
             references will be returned.
         :param selector: Alphanumeric option to select specific information to
             return.
         :return: Returns True if there is not an exception raised.
         """
         logging.info("Retrieving %s from switch", self)
@@ -87,30 +88,32 @@
         Not applicable for VSX.
         """
 
     @classmethod
     def from_uri(cls, session, uri):
         """
         Create a Vsx object given a VSX URI.
+
         :param cls: Object's class.
         :param session: pyaoscx.Session object used to represent a logical
             connection to the device.
         :param uri: a String with a URI.
-        :return Vsx object.
+        :return: Vsx object.
         """
         return cls(session, uri=uri)
 
     @PyaoscxModule.connected
     def apply(self):
         """
         Main method used to either create or update an existing VSX
             configuration. Checks whether the VSX configuration exists in the
             switch. Calls self.update() if VSX configuration being updated.
             Calls self.create() if a new VSX configuration is being created.
-        :return modified: True if object was created or modified.
+
+        :return: True if object was created or modified.
         """
         if self.materialized:
             return self.update()
         return self.create()
 
     def _set_isl_port_for_requests(self):
         """
@@ -130,15 +133,16 @@
             # dictionary
             self.isl_port = self.isl_port.get_info_format()
 
     @PyaoscxModule.connected
     def update(self):
         """
         Perform a PUT call to apply changes to an existing VSX inside switch.
-        :return modified: True if Object was modified and a PUT request was
+
+        :return: True if Object was modified and a PUT request was
             made.
         """
         put_data = utils.get_attrs(self, self.config_attrs)
         if hasattr(self, "keepalive_vrf") and self.keepalive_vrf:
             put_data["keepalive_vrf"] = self.keepalive_vrf
         if hasattr(self, "software_update_vrf") and self.software_update_vrf:
             put_data["software_update_vrf"] = self.software_update_vrf
@@ -149,15 +153,16 @@
         return self.__modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new VSX. Only returns if no exception
             is raised.
-        return: True if entry was created.
+
+        :return: True if entry was created.
         """
         post_data = utils.get_attrs(self, self.config_attrs)
         if hasattr(self, "keepalive_vrf") and self.keepalive_vrf:
             if isinstance(self.keepalive_vrf, str):
                 self.keepalive_vrf = self.__get_vrf(self.keepalive_vrf)
             post_data["keepalive_vrf"] = self.keepalive_vrf
         if hasattr(self, "software_update_vrf") and self.software_update_vrf:
@@ -196,24 +201,26 @@
         self._send_data(self.path, None, "DELETE", "Delete")
         utils.delete_attrs(self, self.config_attrs)
 
     @PyaoscxModule.deprecated
     def get_uri(self):
         """
         Method used to obtain the specific VSX URI.
-        return: Object's URI.
+
+        :return: Object's URI.
         """
         return self.path
 
     @PyaoscxModule.deprecated
     def get_info_format(self):
         """
         Not applicable for VSX.
         """
 
     @PyaoscxModule.deprecated
     def was_modified(self):
         """
         Getter method for the __modified attribute.
+
         :return: True if the object was recently modified.
         """
         return self.modified
```

### Comparing `pyaoscx-2.3.1/pyaoscx.egg-info/PKG-INFO` & `pyaoscx-2.4.0/pyaoscx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaoscx
-Version: 2.3.1
+Version: 2.4.0
 Summary: AOS-CX Python Modules
 Home-page: https://github.com/aruba/pyaoscx
 Author: Aruba Automation
 Author-email: aruba-automation@hpe.com
 License: Apache 2.0
 Keywords: networking aruba aos-cx switch rest api python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyaoscx-2.3.1/pyaoscx.egg-info/SOURCES.txt` & `pyaoscx-2.4.0/pyaoscx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.3.1/setup.py` & `pyaoscx-2.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pyaoscx",
-    version="2.3.1",
+    version="2.4.0",
     description="AOS-CX Python Modules",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aruba/pyaoscx",
     author="Aruba Automation",
     author_email="aruba-automation@hpe.com",
     license="Apache 2.0",
@@ -23,10 +23,16 @@
         "Intended Audience :: System Administrators",
         "Topic :: System :: Networking",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords="networking aruba aos-cx switch rest api python",
     packages=find_packages(exclude=["docs"]),
-    install_requires=["requests", "PyYAML", "netaddr"],
+    install_requires=[
+        "requests",
+        "PyYAML",
+        "netaddr",
+        "requests_toolbelt",
+        "wheel",
+    ],
     zip_safe=False,
 )
```

### Comparing `pyaoscx-2.3.1/workflows/workflow.py` & `pyaoscx-2.4.0/workflows/workflow.py`

 * *Files identical despite different names*

