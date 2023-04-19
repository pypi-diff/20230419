# Comparing `tmp/secsgem-0.2.0a3.tar.gz` & `tmp/secsgem-0.2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secsgem-0.2.0a3.tar", max compression
+gzip compressed data, was "secsgem-0.2.0a4.tar", max compression
```

## Comparing `secsgem-0.2.0a3.tar` & `secsgem-0.2.0a4.tar`

### file list

```diff
@@ -1,329 +1,333 @@
--rw-r--r--   0        0        0    26444 2023-04-12 06:57:27.336893 secsgem-0.2.0a3/LICENSE
--rw-r--r--   0        0        0     2164 2023-04-12 06:57:27.336893 secsgem-0.2.0a3/README.md
--rw-r--r--   0        0        0     1442 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/pyproject.toml
--rw-r--r--   0        0        0      756 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/__init__.py
--rw-r--r--   0        0        0     1123 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/common/__init__.py
--rw-r--r--   0        0        0     3636 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/common/callbacks.py
--rw-r--r--   0        0        0     1651 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/common/codec_jis_x_0201.py
--rw-r--r--   0        0        0     5908 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/common/events.py
--rw-r--r--   0        0        0    13116 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/common/fysom.py
--rw-r--r--   0        0        0     2867 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/common/helpers.py
--rw-r--r--   0        0        0     2118 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/__init__.py
--rw-r--r--   0        0        0     2202 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/alarm.py
--rw-r--r--   0        0        0     2200 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/collection_event.py
--rw-r--r--   0        0        0     1823 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/collection_event_link.py
--rw-r--r--   0        0        0     1764 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/collection_event_report.py
--rw-r--r--   0        0        0     2450 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/data_value.py
--rw-r--r--   0        0        0     3232 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/equipment_constant.py
--rw-r--r--   0        0        0    47111 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/equipmenthandler.py
--rw-r--r--   0        0        0    13257 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/handler.py
--rw-r--r--   0        0        0    10249 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/hosthandler.py
--rw-r--r--   0        0        0     2249 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/remote_command.py
--rw-r--r--   0        0        0     2356 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/status_variable.py
--rw-r--r--   0        0        0     1718 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/__init__.py
--rw-r--r--   0        0        0     5571 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/active_connection.py
--rw-r--r--   0        0        0    10898 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/connection.py
--rw-r--r--   0        0        0     6111 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/connectionmanager.py
--rw-r--r--   0        0        0     3377 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/connectionstatemachine.py
--rw-r--r--   0        0        0     1583 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/deselect_req_header.py
--rw-r--r--   0        0        0     1586 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/deselect_rsp_header.py
--rw-r--r--   0        0        0    21678 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/handler.py
--rw-r--r--   0        0        0     2870 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/header.py
--rw-r--r--   0        0        0     1583 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/linktest_req_header.py
--rw-r--r--   0        0        0     1587 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/linktest_rsp_header.py
--rw-r--r--   0        0        0     2869 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/multi_passive_connection.py
--rw-r--r--   0        0        0     6666 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/multi_passive_server.py
--rw-r--r--   0        0        0     4093 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/packet.py
--rw-r--r--   0        0        0     5168 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/hsms/passive_connection.py
--rw-r--r--   0        0        0     1749 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/hsms/reject_req_header.py
--rw-r--r--   0        0        0     1570 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/hsms/select_req_header.py
--rw-r--r--   0        0        0     1573 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/hsms/select_rsp_header.py
--rw-r--r--   0        0        0     1591 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/hsms/separate_req_header.py
--rw-r--r--   0        0        0     2076 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/hsms/stream_function_header.py
--rw-r--r--   0        0        0     1001 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/__init__.py
--rw-r--r--   0        0        0     5646 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/__init__.py
--rw-r--r--   0        0        0     1119 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/abs.py
--rw-r--r--   0        0        0     1434 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/acka.py
--rw-r--r--   0        0        0     2449 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ackc10.py
--rw-r--r--   0        0        0     1792 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ackc5.py
--rw-r--r--   0        0        0     1792 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ackc6.py
--rw-r--r--   0        0        0     3262 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ackc7.py
--rw-r--r--   0        0        0     4279 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/alcd.py
--rw-r--r--   0        0        0     2051 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/aled.py
--rw-r--r--   0        0        0     1863 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/alid.py
--rw-r--r--   0        0        0     1218 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/altx.py
--rw-r--r--   0        0        0     2297 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/attrdata.py
--rw-r--r--   0        0        0     1621 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/attrid.py
--rw-r--r--   0        0        0     3261 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/attrreln.py
--rw-r--r--   0        0        0     2541 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/base.py
--rw-r--r--   0        0        0     1266 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/bcequ.py
--rw-r--r--   0        0        0     1518 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/binlt.py
--rw-r--r--   0        0        0     1332 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ceed.py
--rw-r--r--   0        0        0     2155 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ceid.py
--rw-r--r--   0        0        0     1066 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/cename.py
--rw-r--r--   0        0        0     2795 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/cepack.py
--rw-r--r--   0        0        0     2103 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/cepval.py
--rw-r--r--   0        0        0     2481 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/cmda.py
--rw-r--r--   0        0        0     1396 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/colct.py
--rw-r--r--   0        0        0     1976 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/commack.py
--rw-r--r--   0        0        0     2430 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/cpack.py
--rw-r--r--   0        0        0     1900 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/cpname.py
--rw-r--r--   0        0        0     1869 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/cpval.py
--rw-r--r--   0        0        0     2215 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/dataid.py
--rw-r--r--   0        0        0     1634 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/datalength.py
--rw-r--r--   0        0        0     1043 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/datlc.py
--rw-r--r--   0        0        0     2878 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/drack.py
--rw-r--r--   0        0        0     1685 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/dsid.py
--rw-r--r--   0        0        0     1060 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/dsper.py
--rw-r--r--   0        0        0     1128 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/dutms.py
--rw-r--r--   0        0        0     1695 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/dvname.py
--rw-r--r--   0        0        0     2078 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/dvval.py
--rw-r--r--   0        0        0     1069 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/dvvalname.py
--rw-r--r--   0        0        0     2587 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/eac.py
--rw-r--r--   0        0        0     2020 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ecdef.py
--rw-r--r--   0        0        0     1893 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ecid.py
--rw-r--r--   0        0        0     2020 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ecmax.py
--rw-r--r--   0        0        0     2020 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ecmin.py
--rw-r--r--   0        0        0     1068 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ecname.py
--rw-r--r--   0        0        0     2152 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ecv.py
--rw-r--r--   0        0        0     1785 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/edid.py
--rw-r--r--   0        0        0     2078 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/erack.py
--rw-r--r--   0        0        0    17058 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/errcode.py
--rw-r--r--   0        0        0     1381 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/errtext.py
--rw-r--r--   0        0        0     1490 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/exid.py
--rw-r--r--   0        0        0     1137 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/exmessage.py
--rw-r--r--   0        0        0     1177 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/exrecvra.py
--rw-r--r--   0        0        0     1125 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/extype.py
--rw-r--r--   0        0        0     1140 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/fcnid.py
--rw-r--r--   0        0        0     1213 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ffrot.py
--rw-r--r--   0        0        0     1279 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/fnloc.py
--rw-r--r--   0        0        0     2177 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/grant6.py
--rw-r--r--   0        0        0     3179 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/grnt1.py
--rw-r--r--   0        0        0     3503 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/hcack.py
--rw-r--r--   0        0        0     2981 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/idtyp.py
--rw-r--r--   0        0        0     1627 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/length.py
--rw-r--r--   0        0        0     3868 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/limitack.py
--rw-r--r--   0        0        0     1221 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/limitid.py
--rw-r--r--   0        0        0     1972 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/limitmax.py
--rw-r--r--   0        0        0     1972 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/limitmin.py
--rw-r--r--   0        0        0     2043 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/lowerdb.py
--rw-r--r--   0        0        0     3081 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/lrack.py
--rw-r--r--   0        0        0     2792 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/lvack.py
--rw-r--r--   0        0        0     2130 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/maper.py
--rw-r--r--   0        0        0     2208 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/mapft.py
--rw-r--r--   0        0        0     2510 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/mdack.py
--rw-r--r--   0        0        0     1226 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/mdln.py
--rw-r--r--   0        0        0     1088 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/mexp.py
--rw-r--r--   0        0        0     1360 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/mhead.py
--rw-r--r--   0        0        0     2024 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/mid.py
--rw-r--r--   0        0        0     1387 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/mlcl.py
--rw-r--r--   0        0        0     1332 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/nulbc.py
--rw-r--r--   0        0        0     1974 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/objack.py
--rw-r--r--   0        0        0     1608 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/objid.py
--rw-r--r--   0        0        0     1204 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/objspec.py
--rw-r--r--   0        0        0     1491 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/objtype.py
--rw-r--r--   0        0        0     1745 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/oflack.py
--rw-r--r--   0        0        0     2209 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/onlack.py
--rw-r--r--   0        0        0     2731 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/orloc.py
--rw-r--r--   0        0        0     1847 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ppbody.py
--rw-r--r--   0        0        0     2927 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ppgnt.py
--rw-r--r--   0        0        0     1574 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ppid.py
--rw-r--r--   0        0        0     3536 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/praxi.py
--rw-r--r--   0        0        0     1393 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/prdct.py
--rw-r--r--   0        0        0     1394 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rcmd.py
--rw-r--r--   0        0        0     1388 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/refp.py
--rw-r--r--   0        0        0     1700 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/repgsz.py
--rw-r--r--   0        0        0     1393 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rowct.py
--rw-r--r--   0        0        0     1118 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rpsel.py
--rw-r--r--   0        0        0     2016 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rptid.py
--rw-r--r--   0        0        0     2397 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rsda.py
--rw-r--r--   0        0        0     1991 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rsdc.py
--rw-r--r--   0        0        0     1426 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rsinf.py
--rw-r--r--   0        0        0     2122 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rspack.py
--rw-r--r--   0        0        0     1678 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/sdack.py
--rw-r--r--   0        0        0     2016 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/sdbin.py
--rw-r--r--   0        0        0     1096 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/shead.py
--rw-r--r--   0        0        0     1607 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/smpln.py
--rw-r--r--   0        0        0     1008 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/softrev.py
--rw-r--r--   0        0        0     1053 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/stime.py
--rw-r--r--   0        0        0     2459 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/strack.py
--rw-r--r--   0        0        0     1138 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/strid.py
--rw-r--r--   0        0        0     1423 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/strp.py
--rw-r--r--   0        0        0     2146 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/sv.py
--rw-r--r--   0        0        0     1890 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/svid.py
--rw-r--r--   0        0        0     1065 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/svname.py
--rw-r--r--   0        0        0     1841 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/text.py
--rw-r--r--   0        0        0     2947 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/tiaack.py
--rw-r--r--   0        0        0     1146 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/tid.py
--rw-r--r--   0        0        0     1085 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/time.py
--rw-r--r--   0        0        0     1230 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/timestamp.py
--rw-r--r--   0        0        0     1693 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/totsmp.py
--rw-r--r--   0        0        0     1756 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/trid.py
--rw-r--r--   0        0        0     1256 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/units.py
--rw-r--r--   0        0        0     2043 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/upperdb.py
--rw-r--r--   0        0        0     2267 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/v.py
--rw-r--r--   0        0        0     2210 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/vid.py
--rw-r--r--   0        0        0     2523 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/vlaack.py
--rw-r--r--   0        0        0     1539 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/xdies.py
--rw-r--r--   0        0        0     1432 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/xypos.py
--rw-r--r--   0        0        0     1539 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/ydies.py
--rw-r--r--   0        0        0    10811 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/__init__.py
--rw-r--r--   0        0        0     6099 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/base.py
--rw-r--r--   0        0        0     1399 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s00f00.py
--rw-r--r--   0        0        0     1407 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f00.py
--rw-r--r--   0        0        0     1405 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f01.py
--rw-r--r--   0        0        0     2127 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f02.py
--rw-r--r--   0        0        0     1716 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f03.py
--rw-r--r--   0        0        0     1778 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f04.py
--rw-r--r--   0        0        0     1753 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f11.py
--rw-r--r--   0        0        0     2297 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f12.py
--rw-r--r--   0        0        0     2153 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f13.py
--rw-r--r--   0        0        0     2485 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f14.py
--rw-r--r--   0        0        0     1399 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f15.py
--rw-r--r--   0        0        0     1594 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f16.py
--rw-r--r--   0        0        0     1398 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f17.py
--rw-r--r--   0        0        0     1600 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f18.py
--rw-r--r--   0        0        0     1695 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f21.py
--rw-r--r--   0        0        0     2138 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f22.py
--rw-r--r--   0        0        0     1701 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f23.py
--rw-r--r--   0        0        0     2297 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f24.py
--rw-r--r--   0        0        0     1407 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f00.py
--rw-r--r--   0        0        0     1750 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f13.py
--rw-r--r--   0        0        0     1722 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f14.py
--rw-r--r--   0        0        0     2152 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f15.py
--rw-r--r--   0        0        0     1594 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f16.py
--rw-r--r--   0        0        0     1406 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f17.py
--rw-r--r--   0        0        0     1576 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f18.py
--rw-r--r--   0        0        0     1569 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f21.py
--rw-r--r--   0        0        0     1591 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f22.py
--rw-r--r--   0        0        0     2665 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f23.py
--rw-r--r--   0        0        0     1615 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f24.py
--rw-r--r--   0        0        0     1571 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f25.py
--rw-r--r--   0        0        0     1568 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f26.py
--rw-r--r--   0        0        0     1759 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f29.py
--rw-r--r--   0        0        0     3308 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f30.py
--rw-r--r--   0        0        0     2662 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f33.py
--rw-r--r--   0        0        0     1607 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f34.py
--rw-r--r--   0        0        0     2465 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f35.py
--rw-r--r--   0        0        0     1609 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f36.py
--rw-r--r--   0        0        0     1937 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f37.py
--rw-r--r--   0        0        0     1616 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f38.py
--rw-r--r--   0        0        0     2496 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f41.py
--rw-r--r--   0        0        0     2644 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f42.py
--rw-r--r--   0        0        0     2267 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f43.py
--rw-r--r--   0        0        0     2963 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f44.py
--rw-r--r--   0        0        0     3470 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f45.py
--rw-r--r--   0        0        0     3147 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f46.py
--rw-r--r--   0        0        0     1697 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f47.py
--rw-r--r--   0        0        0     3848 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f48.py
--rw-r--r--   0        0        0     2870 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f49.py
--rw-r--r--   0        0        0     2655 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f50.py
--rw-r--r--   0        0        0     1407 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f00.py
--rw-r--r--   0        0        0     2139 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f01.py
--rw-r--r--   0        0        0     1598 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f02.py
--rw-r--r--   0        0        0     1851 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f03.py
--rw-r--r--   0        0        0     1603 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f04.py
--rw-r--r--   0        0        0     1675 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f05.py
--rw-r--r--   0        0        0     2270 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f06.py
--rw-r--r--   0        0        0     1411 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f07.py
--rw-r--r--   0        0        0     2278 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f08.py
--rw-r--r--   0        0        0     2667 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f09.py
--rw-r--r--   0        0        0     1408 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f10.py
--rw-r--r--   0        0        0     2310 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f11.py
--rw-r--r--   0        0        0     1409 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f12.py
--rw-r--r--   0        0        0     1853 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f13.py
--rw-r--r--   0        0        0     2566 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f14.py
--rw-r--r--   0        0        0     2852 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f15.py
--rw-r--r--   0        0        0     1420 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f16.py
--rw-r--r--   0        0        0     1576 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f17.py
--rw-r--r--   0        0        0     2603 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f18.py
--rw-r--r--   0        0        0     1407 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f00.py
--rw-r--r--   0        0        0     2374 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f01.py
--rw-r--r--   0        0        0     1596 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f02.py
--rw-r--r--   0        0        0     1888 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f05.py
--rw-r--r--   0        0        0     1596 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f06.py
--rw-r--r--   0        0        0     1580 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f07.py
--rw-r--r--   0        0        0     3424 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f08.py
--rw-r--r--   0        0        0     2783 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f11.py
--rw-r--r--   0        0        0     1600 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f12.py
--rw-r--r--   0        0        0     1577 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f15.py
--rw-r--r--   0        0        0     2788 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f16.py
--rw-r--r--   0        0        0     1614 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f19.py
--rw-r--r--   0        0        0     1686 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f20.py
--rw-r--r--   0        0        0     1624 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f21.py
--rw-r--r--   0        0        0     2075 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f22.py
--rw-r--r--   0        0        0     1584 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f23.py
--rw-r--r--   0        0        0     1595 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f24.py
--rw-r--r--   0        0        0     1407 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f00.py
--rw-r--r--   0        0        0     1848 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f01.py
--rw-r--r--   0        0        0     1593 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f02.py
--rw-r--r--   0        0        0     1895 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f03.py
--rw-r--r--   0        0        0     1607 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f04.py
--rw-r--r--   0        0        0     1572 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f05.py
--rw-r--r--   0        0        0     1895 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f06.py
--rw-r--r--   0        0        0     1694 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f17.py
--rw-r--r--   0        0        0     1618 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f18.py
--rw-r--r--   0        0        0     1427 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f19.py
--rw-r--r--   0        0        0     1704 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f20.py
--rw-r--r--   0        0        0     1407 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f00.py
--rw-r--r--   0        0        0     1615 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f01.py
--rw-r--r--   0        0        0     1617 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f03.py
--rw-r--r--   0        0        0     1619 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f05.py
--rw-r--r--   0        0        0     1605 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f07.py
--rw-r--r--   0        0        0     1618 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f09.py
--rw-r--r--   0        0        0     1608 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f11.py
--rw-r--r--   0        0        0     1835 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f13.py
--rw-r--r--   0        0        0     1410 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s10f00.py
--rw-r--r--   0        0        0     1818 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s10f01.py
--rw-r--r--   0        0        0     1602 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s10f02.py
--rw-r--r--   0        0        0     1825 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s10f03.py
--rw-r--r--   0        0        0     1623 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s10f04.py
--rw-r--r--   0        0        0     1410 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s12f00.py
--rw-r--r--   0        0        0     4534 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s12f01.py
--rw-r--r--   0        0        0     1597 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s12f02.py
--rw-r--r--   0        0        0     3302 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s12f03.py
--rw-r--r--   0        0        0     4510 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s12f04.py
--rw-r--r--   0        0        0     2281 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s12f05.py
--rw-r--r--   0        0        0     1604 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f06.py
--rw-r--r--   0        0        0     2711 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f07.py
--rw-r--r--   0        0        0     1604 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f08.py
--rw-r--r--   0        0        0     2285 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f09.py
--rw-r--r--   0        0        0     1600 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f10.py
--rw-r--r--   0        0        0     2703 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f11.py
--rw-r--r--   0        0        0     1609 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f12.py
--rw-r--r--   0        0        0     1856 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f13.py
--rw-r--r--   0        0        0     2706 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f14.py
--rw-r--r--   0        0        0     1856 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f15.py
--rw-r--r--   0        0        0     2280 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f16.py
--rw-r--r--   0        0        0     2109 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f17.py
--rw-r--r--   0        0        0     2696 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f18.py
--rw-r--r--   0        0        0     1847 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f19.py
--rw-r--r--   0        0        0     1410 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s14f00.py
--rw-r--r--   0        0        0     3293 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s14f01.py
--rw-r--r--   0        0        0     4411 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s14f02.py
--rw-r--r--   0        0        0     2963 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s14f03.py
--rw-r--r--   0        0        0     4411 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s14f04.py
--rw-r--r--   0        0        0    16343 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/handler.py
--rw-r--r--   0        0        0     1387 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/__init__.py
--rw-r--r--   0        0        0     6592 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/array.py
--rw-r--r--   0        0        0     4112 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/base.py
--rw-r--r--   0        0        0     7238 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/base_number.py
--rw-r--r--   0        0        0     6513 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/base_text.py
--rw-r--r--   0        0        0     6685 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/binary.py
--rw-r--r--   0        0        0     6681 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/boolean.py
--rw-r--r--   0        0        0     8973 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/dynamic.py
--rw-r--r--   0        0        0     1190 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/f4.py
--rw-r--r--   0        0        0     1192 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/f8.py
--rw-r--r--   0        0        0     2417 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/functions.py
--rw-r--r--   0        0        0     1182 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/i1.py
--rw-r--r--   0        0        0     1186 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/i2.py
--rw-r--r--   0        0        0     1196 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/i4.py
--rw-r--r--   0        0        0     1214 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/i8.py
--rw-r--r--   0        0        0     1261 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/jis8.py
--rw-r--r--   0        0        0     8800 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/list_type.py
--rw-r--r--   0        0        0     1233 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/string.py
--rw-r--r--   0        0        0     1183 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/u1.py
--rw-r--r--   0        0        0     1185 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/u2.py
--rw-r--r--   0        0        0     1190 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/u4.py
--rw-r--r--   0        0        0     1200 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/u8.py
--rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 secsgem-0.2.0a3/PKG-INFO
+-rw-r--r--   0        0        0    26444 2023-04-19 05:26:26.273741 secsgem-0.2.0a4/LICENSE
+-rw-r--r--   0        0        0     2164 2023-04-19 05:26:26.273741 secsgem-0.2.0a4/README.md
+-rw-r--r--   0        0        0     1442 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/pyproject.toml
+-rw-r--r--   0        0        0      756 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/__init__.py
+-rw-r--r--   0        0        0     1283 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/common/__init__.py
+-rw-r--r--   0        0        0     3636 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/common/callbacks.py
+-rw-r--r--   0        0        0     1651 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/common/codec_jis_x_0201.py
+-rw-r--r--   0        0        0     5908 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/common/events.py
+-rw-r--r--   0        0        0    13248 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/common/fysom.py
+-rw-r--r--   0        0        0     1794 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/common/header.py
+-rw-r--r--   0        0        0     2867 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/common/helpers.py
+-rw-r--r--   0        0        0     1035 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/common/packet.py
+-rw-r--r--   0        0        0     3852 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/common/protocol.py
+-rw-r--r--   0        0        0     1168 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/common/timeouts.py
+-rw-r--r--   0        0        0     2118 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/gem/__init__.py
+-rw-r--r--   0        0        0     2242 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/gem/alarm.py
+-rw-r--r--   0        0        0     2200 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/gem/collection_event.py
+-rw-r--r--   0        0        0     2022 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/gem/collection_event_link.py
+-rw-r--r--   0        0        0     1764 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/gem/collection_event_report.py
+-rw-r--r--   0        0        0     2442 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/gem/data_value.py
+-rw-r--r--   0        0        0     3280 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/gem/equipment_constant.py
+-rw-r--r--   0        0        0    49002 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/gem/equipmenthandler.py
+-rw-r--r--   0        0        0    13535 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/gem/handler.py
+-rw-r--r--   0        0        0    10385 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/gem/hosthandler.py
+-rw-r--r--   0        0        0     2249 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/gem/remote_command.py
+-rw-r--r--   0        0        0     2356 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/gem/status_variable.py
+-rw-r--r--   0        0        0     1721 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/hsms/__init__.py
+-rw-r--r--   0        0        0     5628 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/hsms/active_connection.py
+-rw-r--r--   0        0        0    11252 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/hsms/connection.py
+-rw-r--r--   0        0        0     6140 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/hsms/connectionmanager.py
+-rw-r--r--   0        0        0     3367 2023-04-19 05:26:26.277741 secsgem-0.2.0a4/secsgem/hsms/connectionstatemachine.py
+-rw-r--r--   0        0        0     1458 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/deselect_req_header.py
+-rw-r--r--   0        0        0     1461 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/deselect_rsp_header.py
+-rw-r--r--   0        0        0     3879 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/header.py
+-rw-r--r--   0        0        0     1458 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/linktest_req_header.py
+-rw-r--r--   0        0        0     1462 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/linktest_rsp_header.py
+-rw-r--r--   0        0        0     2873 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/multi_passive_connection.py
+-rw-r--r--   0        0        0     6766 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/multi_passive_server.py
+-rw-r--r--   0        0        0     4257 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/packet.py
+-rw-r--r--   0        0        0     5208 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/passive_connection.py
+-rw-r--r--   0        0        0    22040 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/protocol.py
+-rw-r--r--   0        0        0     1631 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/reject_req_header.py
+-rw-r--r--   0        0        0     1445 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/select_req_header.py
+-rw-r--r--   0        0        0     1448 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/select_rsp_header.py
+-rw-r--r--   0        0        0     1466 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/separate_req_header.py
+-rw-r--r--   0        0        0     1918 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/hsms/stream_function_header.py
+-rw-r--r--   0        0        0     1001 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/__init__.py
+-rw-r--r--   0        0        0     5646 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/__init__.py
+-rw-r--r--   0        0        0     1119 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/abs.py
+-rw-r--r--   0        0        0     1434 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/acka.py
+-rw-r--r--   0        0        0     2449 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ackc10.py
+-rw-r--r--   0        0        0     1792 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ackc5.py
+-rw-r--r--   0        0        0     1792 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ackc6.py
+-rw-r--r--   0        0        0     3262 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ackc7.py
+-rw-r--r--   0        0        0     4279 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/alcd.py
+-rw-r--r--   0        0        0     2051 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/aled.py
+-rw-r--r--   0        0        0     1863 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/alid.py
+-rw-r--r--   0        0        0     1218 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/altx.py
+-rw-r--r--   0        0        0     2297 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/attrdata.py
+-rw-r--r--   0        0        0     1621 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/attrid.py
+-rw-r--r--   0        0        0     3261 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/attrreln.py
+-rw-r--r--   0        0        0     2590 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/base.py
+-rw-r--r--   0        0        0     1266 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/bcequ.py
+-rw-r--r--   0        0        0     1518 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/binlt.py
+-rw-r--r--   0        0        0     1332 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ceed.py
+-rw-r--r--   0        0        0     2155 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ceid.py
+-rw-r--r--   0        0        0     1066 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/cename.py
+-rw-r--r--   0        0        0     2795 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/cepack.py
+-rw-r--r--   0        0        0     2103 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/cepval.py
+-rw-r--r--   0        0        0     2481 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/cmda.py
+-rw-r--r--   0        0        0     1396 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/colct.py
+-rw-r--r--   0        0        0     1976 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/commack.py
+-rw-r--r--   0        0        0     2430 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/cpack.py
+-rw-r--r--   0        0        0     1900 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/cpname.py
+-rw-r--r--   0        0        0     1869 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/cpval.py
+-rw-r--r--   0        0        0     2215 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/dataid.py
+-rw-r--r--   0        0        0     1634 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/datalength.py
+-rw-r--r--   0        0        0     1043 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/datlc.py
+-rw-r--r--   0        0        0     2878 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/drack.py
+-rw-r--r--   0        0        0     1685 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/dsid.py
+-rw-r--r--   0        0        0     1060 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/dsper.py
+-rw-r--r--   0        0        0     1128 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/dutms.py
+-rw-r--r--   0        0        0     1695 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/dvname.py
+-rw-r--r--   0        0        0     2078 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/dvval.py
+-rw-r--r--   0        0        0     1069 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/dvvalname.py
+-rw-r--r--   0        0        0     2587 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/eac.py
+-rw-r--r--   0        0        0     2020 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ecdef.py
+-rw-r--r--   0        0        0     1893 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ecid.py
+-rw-r--r--   0        0        0     2020 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ecmax.py
+-rw-r--r--   0        0        0     2020 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ecmin.py
+-rw-r--r--   0        0        0     1068 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ecname.py
+-rw-r--r--   0        0        0     2152 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ecv.py
+-rw-r--r--   0        0        0     1785 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/edid.py
+-rw-r--r--   0        0        0     2078 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/erack.py
+-rw-r--r--   0        0        0    17058 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/errcode.py
+-rw-r--r--   0        0        0     1381 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/errtext.py
+-rw-r--r--   0        0        0     1490 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/exid.py
+-rw-r--r--   0        0        0     1137 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/exmessage.py
+-rw-r--r--   0        0        0     1177 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/exrecvra.py
+-rw-r--r--   0        0        0     1125 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/extype.py
+-rw-r--r--   0        0        0     1140 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/fcnid.py
+-rw-r--r--   0        0        0     1213 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ffrot.py
+-rw-r--r--   0        0        0     1279 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/fnloc.py
+-rw-r--r--   0        0        0     2177 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/grant6.py
+-rw-r--r--   0        0        0     3179 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/grnt1.py
+-rw-r--r--   0        0        0     3503 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/hcack.py
+-rw-r--r--   0        0        0     2981 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/idtyp.py
+-rw-r--r--   0        0        0     1627 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/length.py
+-rw-r--r--   0        0        0     3868 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/limitack.py
+-rw-r--r--   0        0        0     1221 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/limitid.py
+-rw-r--r--   0        0        0     1972 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/limitmax.py
+-rw-r--r--   0        0        0     1972 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/limitmin.py
+-rw-r--r--   0        0        0     2043 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/lowerdb.py
+-rw-r--r--   0        0        0     3081 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/lrack.py
+-rw-r--r--   0        0        0     2792 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/lvack.py
+-rw-r--r--   0        0        0     2130 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/maper.py
+-rw-r--r--   0        0        0     2208 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/mapft.py
+-rw-r--r--   0        0        0     2510 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/mdack.py
+-rw-r--r--   0        0        0     1226 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/mdln.py
+-rw-r--r--   0        0        0     1088 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/mexp.py
+-rw-r--r--   0        0        0     1360 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/mhead.py
+-rw-r--r--   0        0        0     2024 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/mid.py
+-rw-r--r--   0        0        0     1387 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/mlcl.py
+-rw-r--r--   0        0        0     1332 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/nulbc.py
+-rw-r--r--   0        0        0     1974 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/objack.py
+-rw-r--r--   0        0        0     1608 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/objid.py
+-rw-r--r--   0        0        0     1204 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/objspec.py
+-rw-r--r--   0        0        0     1491 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/objtype.py
+-rw-r--r--   0        0        0     1745 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/oflack.py
+-rw-r--r--   0        0        0     2209 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/onlack.py
+-rw-r--r--   0        0        0     2731 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/orloc.py
+-rw-r--r--   0        0        0     1847 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ppbody.py
+-rw-r--r--   0        0        0     2927 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ppgnt.py
+-rw-r--r--   0        0        0     1574 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ppid.py
+-rw-r--r--   0        0        0     3536 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/praxi.py
+-rw-r--r--   0        0        0     1393 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/prdct.py
+-rw-r--r--   0        0        0     1394 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/rcmd.py
+-rw-r--r--   0        0        0     1388 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/refp.py
+-rw-r--r--   0        0        0     1700 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/repgsz.py
+-rw-r--r--   0        0        0     1393 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/rowct.py
+-rw-r--r--   0        0        0     1118 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/rpsel.py
+-rw-r--r--   0        0        0     2016 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/rptid.py
+-rw-r--r--   0        0        0     2397 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/rsda.py
+-rw-r--r--   0        0        0     1991 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/rsdc.py
+-rw-r--r--   0        0        0     1426 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/rsinf.py
+-rw-r--r--   0        0        0     2122 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/rspack.py
+-rw-r--r--   0        0        0     1678 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/sdack.py
+-rw-r--r--   0        0        0     2016 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/sdbin.py
+-rw-r--r--   0        0        0     1096 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/shead.py
+-rw-r--r--   0        0        0     1607 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/smpln.py
+-rw-r--r--   0        0        0     1008 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/softrev.py
+-rw-r--r--   0        0        0     1053 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/stime.py
+-rw-r--r--   0        0        0     2459 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/strack.py
+-rw-r--r--   0        0        0     1138 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/strid.py
+-rw-r--r--   0        0        0     1423 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/strp.py
+-rw-r--r--   0        0        0     2146 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/sv.py
+-rw-r--r--   0        0        0     1890 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/svid.py
+-rw-r--r--   0        0        0     1065 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/svname.py
+-rw-r--r--   0        0        0     1841 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/text.py
+-rw-r--r--   0        0        0     2947 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/tiaack.py
+-rw-r--r--   0        0        0     1146 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/tid.py
+-rw-r--r--   0        0        0     1085 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/time.py
+-rw-r--r--   0        0        0     1230 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/timestamp.py
+-rw-r--r--   0        0        0     1693 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/totsmp.py
+-rw-r--r--   0        0        0     1756 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/trid.py
+-rw-r--r--   0        0        0     1256 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/units.py
+-rw-r--r--   0        0        0     2043 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/upperdb.py
+-rw-r--r--   0        0        0     2299 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/v.py
+-rw-r--r--   0        0        0     2210 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/vid.py
+-rw-r--r--   0        0        0     2523 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/vlaack.py
+-rw-r--r--   0        0        0     1539 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/xdies.py
+-rw-r--r--   0        0        0     1432 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/xypos.py
+-rw-r--r--   0        0        0     1539 2023-04-19 05:26:26.281741 secsgem-0.2.0a4/secsgem/secs/data_items/ydies.py
+-rw-r--r--   0        0        0    10811 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/__init__.py
+-rw-r--r--   0        0        0     6128 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/base.py
+-rw-r--r--   0        0        0     1399 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s00f00.py
+-rw-r--r--   0        0        0     1407 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f00.py
+-rw-r--r--   0        0        0     1405 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f01.py
+-rw-r--r--   0        0        0     2127 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f02.py
+-rw-r--r--   0        0        0     1716 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f03.py
+-rw-r--r--   0        0        0     1778 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f04.py
+-rw-r--r--   0        0        0     1753 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f11.py
+-rw-r--r--   0        0        0     2297 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f12.py
+-rw-r--r--   0        0        0     2153 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f13.py
+-rw-r--r--   0        0        0     2485 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f14.py
+-rw-r--r--   0        0        0     1399 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f15.py
+-rw-r--r--   0        0        0     1594 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f16.py
+-rw-r--r--   0        0        0     1398 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f17.py
+-rw-r--r--   0        0        0     1600 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f18.py
+-rw-r--r--   0        0        0     1695 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f21.py
+-rw-r--r--   0        0        0     2138 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f22.py
+-rw-r--r--   0        0        0     1701 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f23.py
+-rw-r--r--   0        0        0     2297 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s01f24.py
+-rw-r--r--   0        0        0     1407 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f00.py
+-rw-r--r--   0        0        0     1750 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f13.py
+-rw-r--r--   0        0        0     1722 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f14.py
+-rw-r--r--   0        0        0     2152 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f15.py
+-rw-r--r--   0        0        0     1594 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f16.py
+-rw-r--r--   0        0        0     1406 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f17.py
+-rw-r--r--   0        0        0     1576 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f18.py
+-rw-r--r--   0        0        0     1569 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f21.py
+-rw-r--r--   0        0        0     1591 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f22.py
+-rw-r--r--   0        0        0     2665 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f23.py
+-rw-r--r--   0        0        0     1615 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f24.py
+-rw-r--r--   0        0        0     1571 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f25.py
+-rw-r--r--   0        0        0     1568 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f26.py
+-rw-r--r--   0        0        0     1759 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f29.py
+-rw-r--r--   0        0        0     3308 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f30.py
+-rw-r--r--   0        0        0     2662 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f33.py
+-rw-r--r--   0        0        0     1607 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f34.py
+-rw-r--r--   0        0        0     2465 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f35.py
+-rw-r--r--   0        0        0     1609 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f36.py
+-rw-r--r--   0        0        0     1937 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f37.py
+-rw-r--r--   0        0        0     1616 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f38.py
+-rw-r--r--   0        0        0     2496 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f41.py
+-rw-r--r--   0        0        0     2644 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f42.py
+-rw-r--r--   0        0        0     2267 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f43.py
+-rw-r--r--   0        0        0     2963 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f44.py
+-rw-r--r--   0        0        0     3470 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f45.py
+-rw-r--r--   0        0        0     3147 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f46.py
+-rw-r--r--   0        0        0     1697 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f47.py
+-rw-r--r--   0        0        0     3848 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f48.py
+-rw-r--r--   0        0        0     2870 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f49.py
+-rw-r--r--   0        0        0     2655 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s02f50.py
+-rw-r--r--   0        0        0     1407 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f00.py
+-rw-r--r--   0        0        0     2139 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f01.py
+-rw-r--r--   0        0        0     1598 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f02.py
+-rw-r--r--   0        0        0     1851 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f03.py
+-rw-r--r--   0        0        0     1603 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f04.py
+-rw-r--r--   0        0        0     1675 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f05.py
+-rw-r--r--   0        0        0     2270 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f06.py
+-rw-r--r--   0        0        0     1411 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f07.py
+-rw-r--r--   0        0        0     2278 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f08.py
+-rw-r--r--   0        0        0     2667 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f09.py
+-rw-r--r--   0        0        0     1408 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f10.py
+-rw-r--r--   0        0        0     2310 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f11.py
+-rw-r--r--   0        0        0     1409 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f12.py
+-rw-r--r--   0        0        0     1853 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f13.py
+-rw-r--r--   0        0        0     2566 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f14.py
+-rw-r--r--   0        0        0     2852 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f15.py
+-rw-r--r--   0        0        0     1420 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f16.py
+-rw-r--r--   0        0        0     1576 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f17.py
+-rw-r--r--   0        0        0     2603 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s05f18.py
+-rw-r--r--   0        0        0     1407 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f00.py
+-rw-r--r--   0        0        0     2374 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f01.py
+-rw-r--r--   0        0        0     1596 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f02.py
+-rw-r--r--   0        0        0     1888 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f05.py
+-rw-r--r--   0        0        0     1596 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f06.py
+-rw-r--r--   0        0        0     1580 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f07.py
+-rw-r--r--   0        0        0     3424 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f08.py
+-rw-r--r--   0        0        0     2783 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f11.py
+-rw-r--r--   0        0        0     1600 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f12.py
+-rw-r--r--   0        0        0     1577 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f15.py
+-rw-r--r--   0        0        0     2788 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f16.py
+-rw-r--r--   0        0        0     1614 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f19.py
+-rw-r--r--   0        0        0     1686 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f20.py
+-rw-r--r--   0        0        0     1624 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f21.py
+-rw-r--r--   0        0        0     2075 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f22.py
+-rw-r--r--   0        0        0     1584 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f23.py
+-rw-r--r--   0        0        0     1595 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s06f24.py
+-rw-r--r--   0        0        0     1407 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s07f00.py
+-rw-r--r--   0        0        0     1848 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s07f01.py
+-rw-r--r--   0        0        0     1593 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s07f02.py
+-rw-r--r--   0        0        0     1895 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s07f03.py
+-rw-r--r--   0        0        0     1607 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s07f04.py
+-rw-r--r--   0        0        0     1572 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s07f05.py
+-rw-r--r--   0        0        0     1895 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s07f06.py
+-rw-r--r--   0        0        0     1694 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s07f17.py
+-rw-r--r--   0        0        0     1618 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s07f18.py
+-rw-r--r--   0        0        0     1427 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s07f19.py
+-rw-r--r--   0        0        0     1704 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s07f20.py
+-rw-r--r--   0        0        0     1407 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s09f00.py
+-rw-r--r--   0        0        0     1615 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s09f01.py
+-rw-r--r--   0        0        0     1617 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s09f03.py
+-rw-r--r--   0        0        0     1619 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s09f05.py
+-rw-r--r--   0        0        0     1605 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s09f07.py
+-rw-r--r--   0        0        0     1618 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s09f09.py
+-rw-r--r--   0        0        0     1608 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s09f11.py
+-rw-r--r--   0        0        0     1835 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s09f13.py
+-rw-r--r--   0        0        0     1410 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s10f00.py
+-rw-r--r--   0        0        0     1818 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s10f01.py
+-rw-r--r--   0        0        0     1602 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s10f02.py
+-rw-r--r--   0        0        0     1825 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s10f03.py
+-rw-r--r--   0        0        0     1623 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s10f04.py
+-rw-r--r--   0        0        0     1410 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f00.py
+-rw-r--r--   0        0        0     4534 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f01.py
+-rw-r--r--   0        0        0     1597 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f02.py
+-rw-r--r--   0        0        0     3302 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f03.py
+-rw-r--r--   0        0        0     4510 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f04.py
+-rw-r--r--   0        0        0     2281 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f05.py
+-rw-r--r--   0        0        0     1604 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f06.py
+-rw-r--r--   0        0        0     2711 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f07.py
+-rw-r--r--   0        0        0     1604 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f08.py
+-rw-r--r--   0        0        0     2285 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f09.py
+-rw-r--r--   0        0        0     1600 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f10.py
+-rw-r--r--   0        0        0     2703 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f11.py
+-rw-r--r--   0        0        0     1609 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f12.py
+-rw-r--r--   0        0        0     1856 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f13.py
+-rw-r--r--   0        0        0     2706 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f14.py
+-rw-r--r--   0        0        0     1856 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f15.py
+-rw-r--r--   0        0        0     2280 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f16.py
+-rw-r--r--   0        0        0     2109 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f17.py
+-rw-r--r--   0        0        0     2696 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f18.py
+-rw-r--r--   0        0        0     1847 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s12f19.py
+-rw-r--r--   0        0        0     1410 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s14f00.py
+-rw-r--r--   0        0        0     3293 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s14f01.py
+-rw-r--r--   0        0        0     4411 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s14f02.py
+-rw-r--r--   0        0        0     2963 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s14f03.py
+-rw-r--r--   0        0        0     4411 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/functions/s14f04.py
+-rw-r--r--   0        0        0    16392 2023-04-19 05:26:26.285741 secsgem-0.2.0a4/secsgem/secs/handler.py
+-rw-r--r--   0        0        0     1387 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/__init__.py
+-rw-r--r--   0        0        0     6592 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/array.py
+-rw-r--r--   0        0        0     4112 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/base.py
+-rw-r--r--   0        0        0     7238 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/base_number.py
+-rw-r--r--   0        0        0     6513 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/base_text.py
+-rw-r--r--   0        0        0     6685 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/binary.py
+-rw-r--r--   0        0        0     6681 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/boolean.py
+-rw-r--r--   0        0        0     8965 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/dynamic.py
+-rw-r--r--   0        0        0     1190 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/f4.py
+-rw-r--r--   0        0        0     1192 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/f8.py
+-rw-r--r--   0        0        0     2417 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/functions.py
+-rw-r--r--   0        0        0     1182 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/i1.py
+-rw-r--r--   0        0        0     1186 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/i2.py
+-rw-r--r--   0        0        0     1196 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/i4.py
+-rw-r--r--   0        0        0     1214 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/i8.py
+-rw-r--r--   0        0        0     1261 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/jis8.py
+-rw-r--r--   0        0        0     8800 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/list_type.py
+-rw-r--r--   0        0        0     1233 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/string.py
+-rw-r--r--   0        0        0     1183 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/u1.py
+-rw-r--r--   0        0        0     1185 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/u2.py
+-rw-r--r--   0        0        0     1190 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/u4.py
+-rw-r--r--   0        0        0     1200 2023-04-19 05:26:26.289741 secsgem-0.2.0a4/secsgem/secs/variables/u8.py
+-rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 secsgem-0.2.0a4/PKG-INFO
```

### Comparing `secsgem-0.2.0a3/LICENSE` & `secsgem-0.2.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/README.md` & `secsgem-0.2.0a4/README.md`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/pyproject.toml` & `secsgem-0.2.0a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secsgem"
-version = "0.2.0-alpha.3"
+version = "0.2.0-alpha.4"
 description = "Python SECS/GEM implementation"
 readme = "README.md"
 
 authors = ["Benjamin Parzella <bparzella@gmail.com>"]
 
 license = "LGPL-2.1-or-later"
 
@@ -32,15 +32,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
 python-dateutil = "^2.8.1"
 transitions = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.3.0"
+pytest = "^7.3.1"
 coverage = "^7.2.3"
 prospector = "^1.9.0"
 mypy = "^1.2.0"
 Jinja2 = "^3.1.2"
 PyYAML = "^6.0"
 types-PyYAML = "^6.0.12.9"
 types-python-dateutil = "^2.8.19.12"
```

### Comparing `secsgem-0.2.0a3/secsgem/__init__.py` & `secsgem-0.2.0a4/secsgem/__init__.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/common/__init__.py` & `secsgem-0.2.0a4/secsgem/common/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,12 +14,16 @@
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Contains helper functions."""
 
 from .callbacks import CallbackHandler
 from .events import EventProducer
 from .fysom import Fysom
+from .header import Header
 from .helpers import format_hex, function_name, indent_block, is_windows, is_errorcode_ewouldblock
+from .packet import Packet
+from .protocol import Protocol
+from .timeouts import Timeouts
 
 
 __all__ = ["CallbackHandler", "EventProducer", "Fysom", "format_hex", "function_name", "indent_block", "is_windows",
-           "is_errorcode_ewouldblock"]
+           "is_errorcode_ewouldblock", "Protocol", "Packet", "Header", "Timeouts"]
```

### Comparing `secsgem-0.2.0a3/secsgem/common/callbacks.py` & `secsgem-0.2.0a4/secsgem/common/callbacks.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/common/codec_jis_x_0201.py` & `secsgem-0.2.0a4/secsgem/common/codec_jis_x_0201.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/common/events.py` & `secsgem-0.2.0a4/secsgem/common/events.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/common/fysom.py` & `secsgem-0.2.0a4/secsgem/common/fysom.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         return event in self._map and self.current in self._map[event] \
             and not hasattr(self, 'transition')
 
     def cannot(self, event):
         """Check if transition is not possible."""
         return not self.can(event)
 
-    def _apply(self, cfg):
+    def _apply(self, cfg):  # noqa: MC0001
         init = cfg['initial'] if 'initial' in cfg else None
         if isinstance(init, (str, bytes)):
             init = {'state': init}
         events = cfg['events'] if 'events' in cfg else []
         callbacks = cfg['callbacks'] if 'callbacks' in cfg else {}
         tmap = {}
         self._map = tmap
@@ -272,15 +272,15 @@
     class _EventObject:
         def __init__(self, fsm, event, src, dst):
             self.fsm = fsm
             self.event = event
             self.src = src
             self.dst = dst
 
-    def _build_event(self, event):
+    def _build_event(self, event):  # noqa: MC0001
         def function(**kwargs):
             evt = event
 
             if hasattr(self, 'transition'):
                 raise FysomError(f"event {evt} inappropriate because previous transition did not complete")
             if not self.can(evt):
                 raise FysomError(f"event {evt} inappropriate in current state {self.current}")
@@ -296,19 +296,19 @@
 
                 if self.current != dst:
                     if self._before_event(event_object) is False:
                         return
 
                     def _tran():
                         delattr(self, 'transition')
-                        self.current = dst
+                        self.current = dst  # pylint: disable=attribute-defined-outside-init
                         self._enter_state(event_object)
                         self._change_state(event_object)
                         self._after_event(event_object)
-                    self.transition = _tran
+                    self.transition = _tran  # pylint: disable=attribute-defined-outside-init
 
                 if self._leave_state(event_object) is not False:
                     if hasattr(self, 'transition'):
                         self.transition()
 
                 if self.current in self._autoforward:
                     src = dst
```

### Comparing `secsgem-0.2.0a3/secsgem/common/helpers.py` & `secsgem-0.2.0a4/secsgem/common/helpers.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/gem/__init__.py` & `secsgem-0.2.0a4/secsgem/gem/__init__.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/gem/alarm.py` & `secsgem-0.2.0a4/secsgem/gem/alarm.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #####################################################################
 """Wrapper for GEM alarm."""
 import typing
 
 import secsgem.secs
 
 
-class Alarm:
+class Alarm:  # pylint: disable=too-many-instance-attributes
     """Alarm definition."""
 
     def __init__(self,
                  alid: typing.Union[str, int],
                  name: str,
                  text: str,
                  code: int,
@@ -52,15 +52,15 @@
         self.code = code
         self.ce_on = ce_on
         self.ce_off = ce_off
         self.enabled = False
         self.set = False
 
         self.id_type: typing.Type[secsgem.secs.variables.Base]
-        
+
         if isinstance(self.alid, int):
             self.id_type = secsgem.secs.variables.U4
         else:
             self.id_type = secsgem.secs.variables.String
 
         for key, value in kwargs.items():
             setattr(self, key, value)
```

### Comparing `secsgem-0.2.0a3/secsgem/gem/collection_event.py` & `secsgem-0.2.0a4/secsgem/gem/collection_event.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/gem/collection_event_link.py` & `secsgem-0.2.0a4/secsgem/gem/collection_event_link.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,37 +15,43 @@
 #####################################################################
 """Wrapper for GEM collection event link."""
 import typing
 
 from .collection_event import CollectionEvent
 from .collection_event_report import CollectionEventReport
 
+
 class CollectionEventLink:
     """Representation for registered/linked collection event."""
 
     def __init__(self,
-                 ce: CollectionEvent,
+                 collection_event: CollectionEvent,
                  reports: typing.List[CollectionEventReport],
                  **kwargs):
         """
         Initialize a collection event link.
 
         :param ce: ID of the collection event
         :type ce: :class:`gem.CollectionEvent`
         :param reports: list of the linked reports
         :type reports: list of :class:`gem.CollectionEventReport`
         """
-        self.ce = ce
+        self._collection_event = collection_event
         self._reports = reports
         self.enabled = False
 
         for key, value in kwargs.items():
             setattr(self, key, value)
 
     @property
+    def collection_event(self) -> CollectionEvent:
+        """Get the associated collection event."""
+        return self._collection_event
+
+    @property
     def reports(self):
         """
         Get list of the data values.
 
         :returns: List of linked reports
         :rtype: list of :class:`gem.CollectionEventReport`
         """
```

### Comparing `secsgem-0.2.0a3/secsgem/gem/collection_event_report.py` & `secsgem-0.2.0a4/secsgem/gem/collection_event_report.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/gem/data_value.py` & `secsgem-0.2.0a4/secsgem/gem/data_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self.dvid = dvid
         self.name = name
         self.value_type = value_type
         self.use_callback = use_callback
         self.value = 0
 
         self.id_type: typing.Type[secsgem.secs.variables.Base]
-        
+
         if isinstance(self.dvid, int):
             self.id_type = secsgem.secs.variables.U4
         else:
             self.id_type = secsgem.secs.variables.String
 
         for key, value in kwargs.items():
             setattr(self, key, value)
```

### Comparing `secsgem-0.2.0a3/secsgem/gem/equipment_constant.py` & `secsgem-0.2.0a4/secsgem/gem/equipment_constant.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #####################################################################
 """Wrapper for GEM equipment constant."""
 import typing
 
 import secsgem.secs
 
 
-class EquipmentConstant:
+class EquipmentConstant:  # pylint: disable=too-many-instance-attributes
     """Equipment constant definition."""
 
     def __init__(self,
                  ecid: typing.Union[int, str],
                  name: str,
                  min_value: typing.Union[int, float],
                  max_value: typing.Union[int, float],
```

### Comparing `secsgem-0.2.0a3/secsgem/gem/equipmenthandler.py` & `secsgem-0.2.0a4/secsgem/gem/equipmenthandler.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
+# pylint: disable=too-many-lines
 """Handler for GEM equipment."""
 from datetime import datetime
 import typing
 
 from dateutil.tz import tzlocal
 
 import secsgem.common
-import secsgem.hsms
 import secsgem.secs.variables
 import secsgem.secs.data_items
 
 from .status_variable import StatusVariable
 from .alarm import Alarm
 from .collection_event import CollectionEvent
 from .collection_event_link import CollectionEventLink
@@ -51,39 +51,39 @@
 CEID_CMD_START_DONE = 20
 CEID_CMD_STOP_DONE = 21
 
 RCMD_START = "START"
 RCMD_STOP = "STOP"
 
 
-class GemEquipmentHandler(GemHandler):
+class GemEquipmentHandler(GemHandler):  # pylint: disable=too-many-instance-attributes
     """Baseclass for creating equipment models. Inherit from this class and override required functions."""
 
     def __init__(self,
-                 connection: secsgem.hsms.HsmsHandler,
+                 connection: secsgem.common.Protocol,
                  initial_control_state: str = "ATTEMPT_ONLINE",
                  initial_online_control_state: str = "REMOTE"):
         """
         Initialize a gem equipment handler.
 
         :param connection: Base connection
         :type address: string
         :param initial_control_state: initial state for the control state model, one of ["EQUIPMENT_OFFLINE",
         "ATTEMPT_ONLINE", "HOST_OFFLINE", "ONLINE"]
         :type initial_control_state: string
         """
         super().__init__(connection)
 
-        self.isHost = False
+        self._is_host = False
 
-        self.initialControlStates = ["EQUIPMENT_OFFLINE", "ATTEMPT_ONLINE", "HOST_OFFLINE", "ONLINE"]
-        self.initialControlState = initial_control_state
+        self._initial_control_states = ["EQUIPMENT_OFFLINE", "ATTEMPT_ONLINE", "HOST_OFFLINE", "ONLINE"]
+        self._initial_control_state = initial_control_state
 
-        self.onlineControlStates = ["LOCAL", "REMOTE"]
-        self.onlineControlState = initial_online_control_state
+        self._online_control_states = ["LOCAL", "REMOTE"]
+        self._online_control_state = initial_online_control_state
 
         self._time_format = 1
 
         self._data_values: typing.Dict[typing.Union[int, str], DataValue] = {
         }
 
         self._status_variables: typing.Dict[typing.Union[int, str], StatusVariable] = {
@@ -116,15 +116,15 @@
             RCMD_START: RemoteCommand(RCMD_START, "Start", [], CEID_CMD_START_DONE),
             RCMD_STOP: RemoteCommand(RCMD_STOP, "Stop", [], CEID_CMD_STOP_DONE),
         }
 
         self._registered_reports: typing.Dict[typing.Union[int, str], CollectionEventReport] = {}
         self._registered_collection_events: typing.Dict[typing.Union[int, str], CollectionEventLink] = {}
 
-        self.controlState = secsgem.common.Fysom({
+        self._control_state = secsgem.common.Fysom({
             'initial': "INIT",
             'events': [
                 {'name': 'start', 'src': 'INIT', 'dst': 'CONTROL'},  # 1
                 {'name': 'initial_offline', 'src': 'CONTROL', 'dst': 'OFFLINE'},  # 1
                 {'name': 'initial_equipment_offline', 'src': 'OFFLINE', 'dst': 'EQUIPMENT_OFFLINE'},  # 2
                 {'name': 'initial_attempt_online', 'src': 'OFFLINE', 'dst': 'ATTEMPT_ONLINE'},  # 2
                 {'name': 'initial_host_offline', 'src': 'OFFLINE', 'dst': 'HOST_OFFLINE'},  # 2
@@ -157,283 +157,296 @@
             'autoforward': [
                 # {'src': 'OFFLINE', 'dst': 'EQUIPMENT_OFFLINE'},  # 2
                 # {'src': 'EQUIPMENT_INITIATED_CONNECT', 'dst': 'WAIT_CRA'},  # 5
                 # {'src': 'HOST_INITIATED_CONNECT', 'dst': 'WAIT_CR_FROM_HOST'},  # 10
             ]
         })
 
-        self.controlState.start()  # type: ignore
+        self._control_state.start()  # type: ignore
+
+    @property
+    def control_state(self) -> secsgem.common.Fysom:
+        """Get control state."""
+        return self._control_state
 
     # control state model
 
     def _on_control_state_control(self, _):
-        if self.initialControlState == "ONLINE":
-            self.controlState.initial_online()
+        if self._initial_control_state == "ONLINE":
+            self._control_state.initial_online()
         else:
-            self.controlState.initial_offline()
+            self._control_state.initial_offline()
 
     def _on_control_state_offline(self, _):
-        if self.initialControlState == "EQUIPMENT_OFFLINE":
-            self.controlState.initial_equipment_offline()
-        elif self.initialControlState == "ATTEMPT_ONLINE":
-            self.controlState.initial_attempt_online()
-        elif self.initialControlState == "HOST_OFFLINE":
-            self.controlState.initial_host_offline()
+        if self._initial_control_state == "EQUIPMENT_OFFLINE":
+            self._control_state.initial_equipment_offline()
+        elif self._initial_control_state == "ATTEMPT_ONLINE":
+            self._control_state.initial_attempt_online()
+        elif self._initial_control_state == "HOST_OFFLINE":
+            self._control_state.initial_host_offline()
 
     def _on_control_state_attempt_online(self, _):
-        if not self.communicationState.isstate("COMMUNICATING"):
-            self.controlState.attempt_online_fail_host_offline()
+        if not self._communication_state.isstate("COMMUNICATING"):
+            self._control_state.attempt_online_fail_host_offline()
             return
 
         response = self.are_you_there()
 
         if response is None:
-            self.controlState.attempt_online_fail_host_offline()
+            self._control_state.attempt_online_fail_host_offline()
             return
 
         if response.header.stream != 1 or response.header.function != 2:
-            self.controlState.attempt_online_fail_host_offline()
+            self._control_state.attempt_online_fail_host_offline()
             return
 
-        self.controlState.attempt_online_success()
+        self._control_state.attempt_online_success()
 
     def _on_control_state_online(self, _):
-        if self.onlineControlState == "REMOTE":
-            self.controlState.initial_online_remote()
+        if self._online_control_state == "REMOTE":
+            self._control_state.initial_online_remote()
         else:
-            self.controlState.initial_online_local()
+            self._control_state.initial_online_local()
 
     def _on_control_state_initial_online_local(self, _):
         self.trigger_collection_events([CEID_CONTROL_STATE_LOCAL])
 
     def _on_control_state_initial_online_remote(self, _):
         self.trigger_collection_events([CEID_CONTROL_STATE_REMOTE])
 
     def control_switch_online(self):
         """Operator switches to online control state."""
-        self.controlState.switch_online()
+        self._control_state.switch_online()
 
     def control_switch_offline(self):
         """Operator switches to offline control state."""
-        self.controlState.switch_offline()
+        self._control_state.switch_offline()
         self.trigger_collection_events([CEID_EQUIPMENT_OFFLINE])
 
     def control_switch_online_local(self):
         """Operator switches to the local online control state."""
-        self.controlState.switch_online_local()
-        self.onlineControlState = "LOCAL"
+        self._control_state.switch_online_local()
+        self._online_control_state = "LOCAL"
 
     def control_switch_online_remote(self):
         """Operator switches to the local online control state."""
-        self.controlState.switch_online_remote()
-        self.onlineControlState = "REMOTE"
+        self._control_state.switch_online_remote()
+        self._online_control_state = "REMOTE"
 
     def _on_s01f15(self, 
                    handler: secsgem.secs.SecsHandler, 
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 1, Function 15, Request offline.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler, packet  # unused parameters
 
-        OFLACK = 0
+        oflack = 0
 
-        if self.controlState.current in ["ONLINE", "ONLINE_LOCAL", "ONLINE_REMOTE"]:
-            self.controlState.remote_offline()  # type: ignore
+        if self._control_state.current in ["ONLINE", "ONLINE_LOCAL", "ONLINE_REMOTE"]:
+            self._control_state.remote_offline()  # type: ignore
             self.trigger_collection_events([CEID_EQUIPMENT_OFFLINE])
 
-        return self.stream_function(1, 16)(OFLACK)
+        return self.stream_function(1, 16)(oflack)
 
     def _on_s01f17(self,
                    handler: secsgem.secs.SecsHandler,
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 1, Function 17, Request online.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler, packet  # unused parameters
 
-        ONLACK = 1
+        onlack = 1
 
-        if self.controlState.isstate("HOST_OFFLINE"):
-            self.controlState.remote_online()  # type: ignore
-            ONLACK = 0
-        elif self.controlState.current in ["ONLINE", "ONLINE_LOCAL", "ONLINE_REMOTE"]:
-            ONLACK = 2
+        if self._control_state.isstate("HOST_OFFLINE"):
+            self._control_state.remote_online()  # type: ignore
+            onlack = 0
+        elif self._control_state.current in ["ONLINE", "ONLINE_LOCAL", "ONLINE_REMOTE"]:
+            onlack = 2
 
-        return self.stream_function(1, 18)(ONLACK)
+        return self.stream_function(1, 18)(onlack)
 
     # data values
 
     @property
     def data_values(self) -> typing.Dict[typing.Union[int, str], DataValue]:
         """
         Get list of the data values.
 
         :returns: Data value list
         :rtype: list of :class:`secsgem.gem.DataValue`
         """
         return self._data_values
 
     def on_dv_value_request(self, 
-                            dvid: secsgem.secs.variables.Base, 
-                            dv: DataValue) -> secsgem.secs.variables.Base:
+                            data_value_id: secsgem.secs.variables.Base, 
+                            data_value: DataValue) -> secsgem.secs.variables.Base:
         """
         Get the data value depending on its configuation.
 
         Override in inherited class to provide custom data value request handling.
 
         :param dvid: Id of the data value encoded in the corresponding type
         :type dvid: :class:`secsgem.secs.variables.Base`
         :param dv: The data value requested
         :type dv: :class:`secsgem.gem.DataValue`
         :returns: The value encoded in the corresponding type
         :rtype: :class:`secsgem.secs.variables.Base`
         """
-        del dvid  # unused variable
+        del data_value_id  # unused variable
 
-        return dv.value_type(dv.value)
+        return data_value.value_type(data_value.value)
 
-    def _get_dv_value(self, dv: DataValue) -> secsgem.secs.variables.Base:
+    def _get_dv_value(self, data_value: DataValue) -> secsgem.secs.variables.Base:
         """
         Get the data value depending on its configuation.
 
         :param dv: The data value requested
         :type dv: :class:`secsgem.gem.DataValue`
         :returns: The value encoded in the corresponding type
         :rtype: :class:`secsgem.secs.variables.Base`
         """
-        if dv.use_callback:
-            return self.on_dv_value_request(dv.id_type(dv.dvid), dv)
+        if data_value.use_callback:
+            return self.on_dv_value_request(data_value.id_type(data_value.dvid), data_value)
 
-        return dv.value_type(dv.value)
+        return data_value.value_type(data_value.value)
 
     # status variables
 
     @property
     def status_variables(self) -> typing.Dict[typing.Union[int, str], StatusVariable]:
         """
         Get list of the status variables.
 
         :returns: Status variable list
         :rtype: list of :class:`secsgem.gem.StatusVariables`
         """
         return self._status_variables
 
-    def on_sv_value_request(self, svid: secsgem.secs.variables.Base, sv: StatusVariable) -> secsgem.secs.variables.Base:
+    def on_sv_value_request(self,
+                            svid: secsgem.secs.variables.Base,
+                            status_variable: StatusVariable) -> secsgem.secs.variables.Base:
         """
         Get the status variable value depending on its configuation.
 
         Override in inherited class to provide custom status variable request handling.
 
         :param svid: Id of the status variable encoded in the corresponding type
         :type svid: :class:`secsgem.secs.variables.Base`
         :param sv: The status variable requested
         :type sv: :class:`secsgem.gem.StatusVariable`
         :returns: The value encoded in the corresponding type
         :rtype: :class:`secsgem.secs.variables.Base`
         """
         del svid  # unused variable
 
-        return sv.value_type(sv.value)
+        return status_variable.value_type(status_variable.value)
 
-    def _get_sv_value(self, sv: StatusVariable) -> secsgem.secs.variables.Base:
+    def _get_sv_value(self, status_variable: StatusVariable) -> secsgem.secs.variables.Base:
         """
         Get the status variable value depending on its configuation.
 
         :param sv: The status variable requested
         :type sv: :class:`secsgem.gem.StatusVariable`
         :returns: The value encoded in the corresponding type
         :rtype: :class:`secsgem.secs.variables.Base`
         """
-        if sv.svid == SVID_CLOCK:
-            return sv.value_type(self._get_clock())
-        if sv.svid == SVID_CONTROL_STATE:
-            return sv.value_type(self._get_control_state_id())
-        if sv.svid == SVID_EVENTS_ENABLED:
+        if status_variable.svid == SVID_CLOCK:
+            result = status_variable.value_type(self._get_clock())
+        elif status_variable.svid == SVID_CONTROL_STATE:
+            result = status_variable.value_type(self._get_control_state_id())
+        elif status_variable.svid == SVID_EVENTS_ENABLED:
             events = self._get_events_enabled()
-            return sv.value_type(secsgem.secs.data_items.SV, events)
-        if sv.svid == SVID_ALARMS_ENABLED:
+            result = status_variable.value_type(secsgem.secs.data_items.SV, events)
+        elif status_variable.svid == SVID_ALARMS_ENABLED:
             alarms = self._get_alarms_enabled()
-            return sv.value_type(secsgem.secs.data_items.SV, alarms)
-        if sv.svid == SVID_ALARMS_SET:
+            result = status_variable.value_type(secsgem.secs.data_items.SV, alarms)
+        elif status_variable.svid == SVID_ALARMS_SET:
             alarms = self._get_alarms_set()
-            return sv.value_type(secsgem.secs.data_items.SV, alarms)
-
-        if sv.use_callback:
-            return self.on_sv_value_request(sv.id_type(sv.svid), sv)
+            result = status_variable.value_type(secsgem.secs.data_items.SV, alarms)
+        else:
+            if status_variable.use_callback:
+                result = self.on_sv_value_request(status_variable.id_type(status_variable.svid), status_variable)
+            else:
+                result = status_variable.value_type(status_variable.value)
 
-        return sv.value_type(sv.value)
+        return result
 
     def _on_s01f03(self,
                    handler: secsgem.secs.SecsHandler,
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 1, Function 3, Equipment status request.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler  # unused parameters
 
         message = self.secs_decode(packet)
 
         responses = []
 
         if len(message) == 0:
-            for svid, sv in self._status_variables.items():
-                responses.append(self._get_sv_value(sv))
+            for status_variable_id, status_variable in self._status_variables.items():
+                responses.append(self._get_sv_value(status_variable))
         else:
-            for svid in message:
-                if svid not in self._status_variables:
+            for status_variable_id in message:
+                if status_variable_id not in self._status_variables:
                     responses.append(secsgem.secs.variables.Array(secsgem.secs.data_items.SV, []))
                 else:
-                    sv = self._status_variables[svid]
-                    responses.append(self._get_sv_value(sv))
+                    status_variable = self._status_variables[status_variable_id]
+                    responses.append(self._get_sv_value(status_variable))
 
         return self.stream_function(1, 4)(responses)
 
     def _on_s01f11(self,
                    handler: secsgem.secs.SecsHandler,
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 1, Function 11, SV namelist request.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler  # unused parameters
 
         message = self.secs_decode(packet)
 
         responses = []
 
         if len(message) == 0:
-            for svid, sv in self._status_variables.items():
-                responses.append({"SVID": sv.svid, "SVNAME": sv.name, "UNITS": sv.unit})
+            for status_variable_id, status_variable in self._status_variables.items():
+                responses.append({"SVID": status_variable.svid,
+                                  "SVNAME": status_variable.name,
+                                  "UNITS": status_variable.unit})
         else:
-            for svid in message:
-                if svid not in self._status_variables:
-                    responses.append({"SVID": svid, "SVNAME": "", "UNITS": ""})
+            for status_variable_id in message:
+                if status_variable_id not in self._status_variables:
+                    responses.append({"SVID": status_variable_id, "SVNAME": "", "UNITS": ""})
                 else:
-                    sv = self._status_variables[svid]
-                    responses.append({"SVID": sv.svid, "SVNAME": sv.name, "UNITS": sv.unit})
+                    status_variable = self._status_variables[status_variable_id]
+                    responses.append({"SVID": status_variable.svid,
+                                      "SVNAME": status_variable.name,
+                                      "UNITS": status_variable.unit})
 
         return self.stream_function(1, 12)(responses)
 
     # collection events
 
     @property
     def collection_events(self) -> typing.Dict[typing.Union[int, str], CollectionEvent]:
@@ -480,58 +493,58 @@
             if ceid in self._registered_collection_events:
                 if self._registered_collection_events[ceid].enabled:
                     reports = self._build_collection_event(ceid)
 
                     self.send_and_waitfor_response(self.stream_function(6, 11)(
                         {"DATAID": 1, "CEID": ceid, "RPT": reports}))
 
-    def _on_s02f33(self,
+    def _on_s02f33(self,  # noqa: MC0001
                    handler: secsgem.secs.SecsHandler,
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 2, Function 33, Define Report.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler  # unused parameters
 
         message = self.secs_decode(packet)
 
         # 0  = Accept
         # 1  = Denied. Insufficient space.
         # 2  = Denied. Invalid format.
         # 3  = Denied. At least one RPTID already defined.
         # 4  = Denied. At least VID does not exist.
         # >4 = Other errors
-        DRACK = 0
+        drack = 0
 
         # pre check message for errors
         for report in message.DATA:
             if report.RPTID in self._registered_reports and len(report.VID) > 0:
-                DRACK = 3
+                drack = 3
             else:
                 for vid in report.VID:
                     if (vid not in self._data_values) and (vid not in self._status_variables):
-                        DRACK = 4
+                        drack = 4
 
-        result = self.stream_function(2, 34)(DRACK)
+        result = self.stream_function(2, 34)(drack)
 
-        if DRACK != 0:
+        if drack != 0:
             return result
 
         # no data -> remove all reports and links
         if not message.DATA:
             self._registered_collection_events.clear()
             self._registered_reports.clear()
 
             return result
-        
+
         for report in message.DATA:
             # no vids -> remove this reports and links
             if not report.VID:
                 # remove report from linked collection events
                 for collection_event in list(self._registered_collection_events):
                     if report.RPTID in self._registered_collection_events[collection_event].reports:
                         self._registered_collection_events[collection_event].reports.remove(report.RPTID)
@@ -543,102 +556,102 @@
                     del self._registered_reports[report.RPTID]
             else:
                 # add report
                 self._registered_reports[report.RPTID] = CollectionEventReport(report.RPTID, report.VID)
 
         return result
 
-    def _on_s02f35(self,
+    def _on_s02f35(self,  # noqa: MC0001
                    handler: secsgem.secs.SecsHandler,
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 2, Function 35, Link event report.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler  # unused parameters
 
         message = self.secs_decode(packet)
 
         # 0  = Accepted
         # 1  = Denied. Insufficient space
         # 2  = Denied. Invalid format
         # 3  = Denied. At least one CEID link already defined
         # 4  = Denied. At least one CEID does not exist
         # 5  = Denied. At least one RPTID does not exist
         # >5 = Other errors
-        LRACK = 0
+        lrack = 0
 
         # pre check message for errors
         for event in message.DATA:
             if event.CEID.get() not in self._collection_events:
-                LRACK = 4
+                lrack = 4
             for rptid in event.RPTID:
                 if event.CEID.get() in self._registered_collection_events:
-                    ce = self._registered_collection_events[event.CEID.get()]
-                    if rptid.get() in ce.reports:
-                        LRACK = 3
+                    collection_event = self._registered_collection_events[event.CEID.get()]
+                    if rptid.get() in collection_event.reports:
+                        lrack = 3
                 if rptid.get() not in self._registered_reports:
-                    LRACK = 5
+                    lrack = 5
 
         # pre check okay
-        if LRACK == 0:
+        if lrack == 0:
             for event in message.DATA:
                 # no report ids, remove all links for collection event
                 if not event.RPTID:
                     if event.CEID.get() in self._registered_collection_events:
                         del self._registered_collection_events[event.CEID.get()]
                 else:
                     if event.CEID.get() in self._registered_collection_events:
-                        ce = self._registered_collection_events[event.CEID.get()]
+                        collection_event = self._registered_collection_events[event.CEID.get()]
                         for rptid in event.RPTID.get():
-                            ce.reports.append(rptid)
+                            collection_event.reports.append(rptid)
                     else:
                         self._registered_collection_events[event.CEID.get()] = \
                             CollectionEventLink(self._collection_events[event.CEID.get()], event.RPTID.get())
 
-        return self.stream_function(2, 36)(LRACK)
+        return self.stream_function(2, 36)(lrack)
 
     def _on_s02f37(self,
                    handler: secsgem.secs.SecsHandler,
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Callback handler for Stream 2, Function 37, En-/Disable Event Report.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler  # unused parameters
 
         message = self.secs_decode(packet)
 
         # 0  = Accepted
         # 1  = Denied. At least one CEID does not exist
-        ERACK = 0
+        erack = 0
 
         if not self._set_ce_state(message.CEED.get(), message.CEID.get()):
-            ERACK = 1
+            erack = 1
 
-        return self.stream_function(2, 38)(ERACK)
+        return self.stream_function(2, 38)(erack)
 
     def _on_s06f15(self,
                    handler: secsgem.secs.SecsHandler,
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Callback handler for Stream 6, Function 15, event report request.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler  # unused parameters
 
         message = self.secs_decode(packet)
 
         ceid = message.get()
 
@@ -686,19 +699,19 @@
         reports = []
 
         for rptid in self._registered_collection_events[ceid].reports:
             report = self._registered_reports[rptid]
             variables = []
             for var in report.vars:
                 if var in self._status_variables:
-                    v = self._get_sv_value(self._status_variables[var])
-                    variables.append(v)
+                    value = self._get_sv_value(self._status_variables[var])
+                    variables.append(value)
                 elif var in self._data_values:
-                    v = self._get_dv_value(self._data_values[var])
-                    variables.append(v)
+                    value = self._get_dv_value(self._data_values[var])
+                    variables.append(value)
 
             reports.append({"RPTID": rptid, "V": variables})
 
         return reports
 
     # equipment constants
 
@@ -709,166 +722,166 @@
 
         :returns: Equipment constant list
         :rtype: list of :class:`secsgem.gem.EquipmentConstant`
         """
         return self._equipment_constants
 
     def on_ec_value_request(self,
-                            ecid: secsgem.secs.variables.Base,
-                            ec: EquipmentConstant) -> secsgem.secs.variables.Base:
+                            equipment_constant_id: secsgem.secs.variables.Base,
+                            equipment_constant: EquipmentConstant) -> secsgem.secs.variables.Base:
         """
         Get the equipment constant value depending on its configuation.
 
         Override in inherited class to provide custom equipment constant request handling.
 
         :param ecid: Id of the equipment constant encoded in the corresponding type
         :type ecid: :class:`secsgem.secs.variables.Base`
         :param ec: The equipment constant requested
         :type ec: :class:`secsgem.gem.EquipmentConstant`
         :returns: The value encoded in the corresponding type
         :rtype: :class:`secsgem.secs.variables.Base`
         """
-        del ecid  # unused variable
+        del equipment_constant_id  # unused variable
 
-        return ec.value_type(ec.value)
+        return equipment_constant.value_type(equipment_constant.value)
 
     def on_ec_value_update(self,
-                           ecid: secsgem.secs.variables.Base,
-                           ec: EquipmentConstant, 
+                           equipment_constant_id: secsgem.secs.variables.Base,
+                           equipment_constant: EquipmentConstant, 
                            value: typing.Union[int, float]):
         """
         Set the equipment constant value depending on its configuation.
 
         Override in inherited class to provide custom equipment constant update handling.
 
         :param ecid: Id of the equipment constant encoded in the corresponding type
         :type ecid: :class:`secsgem.secs.variables.Base`
         :param ec: The equipment constant to be updated
         :type ec: :class:`secsgem.gem.EquipmentConstant`
         :param value: The value encoded in the corresponding type
         :type value: :class:`secsgem.secs.variables.Base`
         """
-        del ecid  # unused variable
+        del equipment_constant_id  # unused variable
 
-        ec.value = value
+        equipment_constant.value = value
 
-    def _get_ec_value(self, ec: EquipmentConstant) -> secsgem.secs.variables.Base:
+    def _get_ec_value(self, equipment_constant: EquipmentConstant) -> secsgem.secs.variables.Base:
         """
         Get the equipment constant value depending on its configuation.
 
         :param ec: The equipment requested
         :type ec: :class:`secsgem.gem.EquipmentConstant`
         :returns: The value encoded in the corresponding type
         :rtype: :class:`secsgem.secs.variables.Base`
         """
-        if ec.ecid == ECID_ESTABLISH_COMMUNICATIONS_TIMEOUT:
-            return ec.value_type(self.establishCommunicationTimeout)
-        if ec.ecid == ECID_TIME_FORMAT:
-            return ec.value_type(self._time_format)
-
-        if ec.use_callback:
-            return self.on_ec_value_request(ec.id_type(ec.ecid), ec)
-        return ec.value_type(ec.value)
+        if equipment_constant.ecid == ECID_ESTABLISH_COMMUNICATIONS_TIMEOUT:
+            return equipment_constant.value_type(self._establish_communication_timeout)
+        if equipment_constant.ecid == ECID_TIME_FORMAT:
+            return equipment_constant.value_type(self._time_format)
+
+        if equipment_constant.use_callback:
+            return self.on_ec_value_request(equipment_constant.id_type(equipment_constant.ecid), equipment_constant)
+        return equipment_constant.value_type(equipment_constant.value)
 
-    def _set_ec_value(self, ec: EquipmentConstant, value: typing.Union[int, float]):
+    def _set_ec_value(self, equipment_constant: EquipmentConstant, value: typing.Union[int, float]):
         """
         Get the equipment constant value depending on its configuation.
 
         :param ec: The equipment requested
         :type ec: :class:`secsgem.gem.EquipmentConstant`
         :param value: The value encoded in the corresponding type
         :type value: :class:`secsgem.secs.variables.Base`
         """
-        if ec.ecid == ECID_ESTABLISH_COMMUNICATIONS_TIMEOUT:
-            self.establishCommunicationTimeout = int(value)
-        if ec.ecid == ECID_TIME_FORMAT:
+        if equipment_constant.ecid == ECID_ESTABLISH_COMMUNICATIONS_TIMEOUT:
+            self._establish_communication_timeout = int(value)
+        if equipment_constant.ecid == ECID_TIME_FORMAT:
             self._time_format = int(value)
 
-        if ec.use_callback:
-            self.on_ec_value_update(ec.id_type(ec.ecid), ec, value)
+        if equipment_constant.use_callback:
+            self.on_ec_value_update(equipment_constant.id_type(equipment_constant.ecid), equipment_constant, value)
         else:
-            ec.value = value
+            equipment_constant.value = value
 
     def _on_s02f13(self,
                    handler: secsgem.secs.SecsHandler,
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 2, Function 13, Equipment constant request.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler  # unused parameters
 
         message = self.secs_decode(packet)
 
         responses = []
 
         if len(message) == 0:
-            for ecid, ec in self._equipment_constants.items():
-                responses.append(self._get_ec_value(ec))
+            for equipment_constant_id, equipment_constant in self._equipment_constants.items():
+                responses.append(self._get_ec_value(equipment_constant))
         else:
-            for ecid in message:
-                if ecid not in self._equipment_constants:
+            for equipment_constant_id in message:
+                if equipment_constant_id not in self._equipment_constants:
                     responses.append(secsgem.secs.variables.Array(secsgem.secs.data_items.ECV, []))
                 else:
-                    ec = self._equipment_constants[ecid]
-                    responses.append(self._get_ec_value(ec))
+                    equipment_constant = self._equipment_constants[equipment_constant_id]
+                    responses.append(self._get_ec_value(equipment_constant))
 
         return self.stream_function(2, 14)(responses)
 
     def _on_s02f15(self,
                    handler: secsgem.secs.SecsHandler,
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 2, Function 15, Equipment constant send.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler  # unused parameters
 
         message = self.secs_decode(packet)
 
         eac = 0
 
-        for ec in message:
-            if ec.ECID not in self._equipment_constants:
+        for equipment_constant in message:
+            if equipment_constant.ECID not in self._equipment_constants:
                 eac = 1
             else:
-                constant = self.equipment_constants[ec.ECID.get()]
+                constant = self.equipment_constants[equipment_constant.ECID.get()]
 
                 if constant.min_value is not None:
-                    if ec.ECV.get() < constant.min_value:
+                    if equipment_constant.ECV.get() < constant.min_value:
                         eac = 3
 
                 if constant.max_value is not None:
-                    if ec.ECV.get() > constant.max_value:
+                    if equipment_constant.ECV.get() > constant.max_value:
                         eac = 3
 
         if eac == 0:
-            for ec in message:
-                self._set_ec_value(self._equipment_constants[ec.ECID], ec.ECV.get())
+            for equipment_constant in message:
+                self._set_ec_value(self._equipment_constants[equipment_constant.ECID], equipment_constant.ECV.get())
 
         return self.stream_function(2, 16)(eac)
 
     def _on_s02f29(self,
                    handler: secsgem.secs.SecsHandler,
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 2, Function 29, EC namelist request.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler  # unused parameters
 
         message = self.secs_decode(packet)
 
         responses = []
 
@@ -947,49 +960,49 @@
 
         self.alarms[alid].set = False
 
         self.trigger_collection_events([self.alarms[alid].ce_off])
 
     def _on_s05f03(self,
                    handler: secsgem.secs.SecsHandler, 
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 5, Function 3, Alarm en-/disabled.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler  # unused parameters
 
         message = self.secs_decode(packet)
 
         # 0  = Accepted
         # 1  = Error
         result = secsgem.secs.data_items.ACKC5.ACCEPTED
 
         alid = message.ALID.get()
         if alid not in self._alarms:
             result = secsgem.secs.data_items.ACKC5.ERROR
         else:
-            self.alarms[alid].enabled = (message.ALED.get() == secsgem.secs.data_items.ALED.ENABLE)
+            self.alarms[alid].enabled = message.ALED.get() == secsgem.secs.data_items.ALED.ENABLE
 
         return self.stream_function(5, 4)(result)
 
     def _on_s05f05(self,
                    handler: secsgem.secs.SecsHandler,
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 5, Function 5, Alarm list.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler  # unused parameters
 
         message = self.secs_decode(packet)
 
         result = []
 
@@ -1004,22 +1017,22 @@
                            "ALID": alid,
                            "ALTX": self.alarms[alid].text})
 
         return self.stream_function(5, 6)(result)
 
     def _on_s05f07(self,
                    handler: secsgem.secs.SecsHandler,
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 5, Function 7, Enabled alarm list.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler, packet  # unused parameters
 
         result = []
 
         for alid in list(self.alarms.keys()):
             if self.alarms[alid].enabled:
@@ -1039,45 +1052,45 @@
         :returns: Remote command list
         :rtype: list of :class:`secsgem.gem.RemoteCommand`
         """
         return self._remote_commands
 
     def _on_s02f41(self,
                    handler: secsgem.secs.SecsHandler,
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 2, Function 41, host command send.
 
         The remote command handing differs from usual stream function handling, because we send the ack with later
         completion first.
         Then we run the actual remote command callback and signal success with the matching collection event.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler  # unused parameters
 
         message = self.secs_decode(packet)
 
         rcmd_name = message.RCMD.get()
         rcmd_callback_name = "rcmd_" + rcmd_name
 
         if rcmd_name not in self._remote_commands:
-            self.logger.info("remote command %s not registered", rcmd_name)
+            self._logger.info("remote command %s not registered", rcmd_name)
             return self.stream_function(2, 42)({"HCACK": secsgem.secs.data_items.HCACK.INVALID_COMMAND, "PARAMS": []})
 
         if rcmd_callback_name not in self._callback_handler:
-            self.logger.warning("callback for remote command %s not available", rcmd_name)
+            self._logger.warning("callback for remote command %s not available", rcmd_name)
             return self.stream_function(2, 42)({"HCACK": secsgem.secs.data_items.HCACK.INVALID_COMMAND, "PARAMS": []})
 
         for param in message.PARAMS:
             if param.CPNAME.get() not in self._remote_commands[rcmd_name].params:
-                self.logger.warning("parameter %s for remote command %s not available", param.CPNAME.get(), rcmd_name)
+                self._logger.warning("parameter %s for remote command %s not available", param.CPNAME.get(), rcmd_name)
                 return self.stream_function(2, 42)({"HCACK": secsgem.secs.data_items.HCACK.PARAMETER_INVALID,
                                                     "PARAMS": []})
 
         self.send_response(self.stream_function(2, 42)({"HCACK": secsgem.secs.data_items.HCACK.ACK_FINISH_LATER,
                                                         "PARAMS": []}),
                            packet.header.system)
 
@@ -1089,19 +1102,19 @@
 
         callback(**kwargs)
 
         self.trigger_collection_events([self._remote_commands[rcmd_name].ce_finished])
 
         return None
 
-    def _on_rcmd_START(self):
-        self.logger.warning("remote command START not implemented, this is required for GEM compliance")
+    def _on_rcmd_START(self):  # noqa: N802
+        self._logger.warning("remote command START not implemented, this is required for GEM compliance")
 
-    def _on_rcmd_STOP(self):
-        self.logger.warning("remote command STOP not implemented, this is required for GEM compliance")
+    def _on_rcmd_STOP(self):  # noqa: N802
+        self._logger.warning("remote command STOP not implemented, this is required for GEM compliance")
 
     # helpers
 
     def _get_clock(self) -> str:
         """
         Get the clock depending on configured time format.
 
@@ -1120,23 +1133,23 @@
     def _get_control_state_id(self) -> int:
         """
         Get id of the control state for the current control state.
 
         :returns: control state
         :rtype: integer
         """
-        if self.controlState.isstate("EQUIPMENT_OFFLINE"):
+        if self._control_state.isstate("EQUIPMENT_OFFLINE"):
             return 1
-        if self.controlState.isstate("ATTEMPT_ONLINE"):
+        if self._control_state.isstate("ATTEMPT_ONLINE"):
             return 2
-        if self.controlState.isstate("HOST_OFFLINE"):
+        if self._control_state.isstate("HOST_OFFLINE"):
             return 3
-        if self.controlState.isstate("ONLINE_LOCAL"):
+        if self._control_state.isstate("ONLINE_LOCAL"):
             return 4
-        if self.controlState.isstate("ONLINE_REMOTE"):
+        if self._control_state.isstate("ONLINE_REMOTE"):
             return 5
 
         return -1
 
     def _get_events_enabled(self) -> typing.List[typing.Union[int, str]]:
         """
         List of the enabled collection events.
@@ -1184,12 +1197,12 @@
 
     def on_connection_closed(self, connection):
         """Handle connection was closed event."""
         # call parent handlers
         super().on_connection_closed(connection)
 
         # update control state
-        if self.controlState.current in ["ONLINE", "ONLINE_LOCAL", "ONLINE_REMOTE"]:
-            self.controlState.switch_offline()
+        if self._control_state.current in ["ONLINE", "ONLINE_LOCAL", "ONLINE_REMOTE"]:
+            self._control_state.switch_offline()
 
-        if self.controlState.current in ["EQUIPMENT_OFFLINE"]:
-            self.controlState.switch_online()
+        if self._control_state.current in ["EQUIPMENT_OFFLINE"]:
+            self._control_state.switch_online()
```

### Comparing `secsgem-0.2.0a3/secsgem/gem/handler.py` & `secsgem-0.2.0a4/secsgem/gem/handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,48 +9,47 @@
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Handler for GEM commands. Used in combination with :class:`secsgem.HsmsHandler.HsmsConnectionManager`."""
+"""Handler for GEM commands. Used in combination with :class:`secsgem.hsms.HsmsConnectionManager`."""
 import logging
 import threading
 import typing
 
 import secsgem.common
-import secsgem.hsms
 import secsgem.secs
 
 
-class GemHandler(secsgem.secs.SecsHandler):
+class GemHandler(secsgem.secs.SecsHandler):  # pylint: disable=too-many-instance-attributes
     """Baseclass for creating Host/Equipment models. This layer contains GEM functionality."""
 
-    def __init__(self, connection: secsgem.hsms.HsmsHandler):
+    def __init__(self, connection: secsgem.common.Protocol):
         """
         Initialize a gem handler.
 
         Inherit from this class and override required functions.
 
         :param connection: connection to use
         """
         super().__init__(connection)
-        self._connection.events.hsms_selected += self._on_hsms_select
+        self._protocol.events.hsms_selected += self._on_hsms_select
 
-        self.MDLN = "secsgem"  #: model number returned by S01E13/14
-        self.SOFTREV = "0.1.0"  #: software version returned by S01E13/14
+        self._mdln = "secsgem"  #: model number returned by S01E13/14
+        self._softrev = "0.1.0"  #: software version returned by S01E13/14
 
-        self.logger = logging.getLogger(self.__module__ + "." + self.__class__.__name__)
+        self._logger = logging.getLogger(self.__module__ + "." + self.__class__.__name__)
 
-        self.isHost = True
+        self._is_host = True
 
         # not going to HOST_INITIATED_CONNECT because fysom doesn't support two states.
         # but there is a transistion to get out of EQUIPMENT_INITIATED_CONNECT when the HOST_INITIATED_CONNECT happens
-        self.communicationState = secsgem.common.Fysom({
+        self._communication_state = secsgem.common.Fysom({
             'initial': 'DISABLED',  # 1
             'events': [
                 {'name': 'enable', 'src': 'DISABLED', 'dst': 'ENABLED'},  # 2
                 {'name': 'disable', 'src': ['ENABLED', 'NOT_COMMUNICATING', 'COMMUNICATING',
                                             'EQUIPMENT_INITIATED_CONNECT', 'WAIT_DELAY', 'WAIT_CRA',
                                             "HOST_INITIATED_CONNECT", "WAIT_CR_FROM_HOST"], 'dst': 'DISABLED'},  # 3
                 {'name': 'select', 'src': 'NOT_COMMUNICATING', 'dst': 'EQUIPMENT_INITIATED_CONNECT'},  # 5
@@ -75,166 +74,172 @@
             'autoforward': [
                 {'src': 'ENABLED', 'dst': 'NOT_COMMUNICATING'},  # 4
                 {'src': 'EQUIPMENT_INITIATED_CONNECT', 'dst': 'WAIT_CRA'},  # 5
                 {'src': 'HOST_INITIATED_CONNECT', 'dst': 'WAIT_CR_FROM_HOST'},  # 10
             ]
         })
 
-        self.waitCRATimer = None
-        self.commDelayTimer = None
-        self.establishCommunicationTimeout = 10
+        self._wait_cra_timer = None
+        self._comm_delay_timer = None
+        self._establish_communication_timeout = 10
 
-        self.reportIDCounter = 1000
+        self._report_id_counter = 1000
 
-        self.waitEventList: typing.List[threading.Event] = []
+        self._wait_event_list: typing.List[threading.Event] = []
 
     def __repr__(self) -> str:
         """Generate textual representation for an object of this class."""
-        return f"{self.__class__.__name__} {str(self._serialize_data())}"
+        return f"{self.__class__.__name__} {str(self.serialize_data())}"
 
-    def _serialize_data(self)-> typing.Dict[str, typing.Any]:
+    @property
+    def communication_state(self) -> secsgem.common.Fysom:
+        """Get the communication state model."""
+        return self._communication_state
+
+    def serialize_data(self) -> typing.Dict[str, typing.Any]:
         """
         Get serialized data.
 
         :returns: data to serialize for this object
         :rtype: dict
         """
-        data = self.connection._serialize_data()  # pylint: disable=protected-access
-        data.update({'communicationState': self.communicationState.current,
-                     'commDelayTimeout': self.establishCommunicationTimeout,
-                     'reportIDCounter': self.reportIDCounter})
+        data = self.protocol.serialize_data()
+        data.update({'communicationState': self._communication_state.current,
+                     'commDelayTimeout': self._establish_communication_timeout,
+                     'reportIDCounter': self._report_id_counter})
         return data
 
     def enable(self) -> None:
         """Enable the connection."""
-        self.connection.enable()
-        self.communicationState.enable()  # type: ignore
+        self.protocol.enable()
+        self._communication_state.enable()  # type: ignore
 
-        self.logger.info("Connection enabled")
+        self._logger.info("Connection enabled")
 
     def disable(self) -> None:
         """Disable the connection."""
-        self.connection.disable()
-        self.communicationState.disable()  # type: ignore
+        self.protocol.disable()
+        self._communication_state.disable()  # type: ignore
 
-        self.logger.info("Connection disabled")
+        self._logger.info("Connection disabled")
 
     def _on_hsms_packet_received(self, data: typing.Dict[str, typing.Any]):
         """
         Packet received from hsms layer.
 
         :param data: received event data
         """
         packet = data["packet"]
-        if self.communicationState.isstate('WAIT_CRA'):
+        if self._communication_state.isstate('WAIT_CRA'):
             if packet.header.stream == 1 and packet.header.function == 13:
-                if self.isHost:
+                if self._is_host:
                     self.send_response(self.stream_function(1, 14)({"COMMACK": self.on_commack_requested(),
                                                                     "MDLN": []}),
                                        packet.header.system)
                 else:
                     self.send_response(self.stream_function(1, 14)({"COMMACK": self.on_commack_requested(),
-                                                                    "MDLN": [self.MDLN, self.SOFTREV]}),
+                                                                    "MDLN": [self._mdln, self._softrev]}),
                                        packet.header.system)
 
-                self.communicationState.s1f13received()  # type: ignore
+                self._communication_state.s1f13received()  # type: ignore
             elif packet.header.stream == 1 and packet.header.function == 14:
-                self.communicationState.s1f14received()  # type: ignore
-        elif self.communicationState.isstate('WAIT_DELAY'):
+                self._communication_state.s1f14received()  # type: ignore
+        elif self._communication_state.isstate('WAIT_DELAY'):
             pass
-        elif self.communicationState.isstate('COMMUNICATING'):
+        elif self._communication_state.isstate('COMMUNICATING'):
             threading.Thread(target=self._handle_stream_function, args=(packet, ),
                              name=f"secsgem_gemHandler_callback_S{packet.header.stream}F{packet.header.function}"
                              ).start()
 
     def _on_hsms_select(self, _):
         """Selected received from hsms layer."""
-        self.communicationState.select()
+        self._communication_state.select()
 
     def _on_wait_cra_timeout(self):
         """Linktest time timed out, so send linktest request."""
-        self.communicationState.communicationreqfail()
+        self._communication_state.communicationreqfail()
 
     def _on_wait_comm_delay_timeout(self):
         """Linktest time timed out, so send linktest request."""
-        self.communicationState.delayexpired()
+        self._communication_state.delayexpired()
 
     def _on_state_wait_cra(self, _):
         """
         Connection state model changed to state WAIT_CRA.
 
         :param data: event attributes
         :type data: object
         """
-        self.logger.debug("connectionState -> WAIT_CRA")
+        self._logger.debug("connectionState -> WAIT_CRA")
 
-        self.waitCRATimer = threading.Timer(self.connection.connection.T3, self._on_wait_cra_timeout)
-        self.waitCRATimer.start()
+        self._wait_cra_timer = threading.Timer(self.protocol.timeouts.t3, self._on_wait_cra_timeout)
+        self._wait_cra_timer.start()
 
-        if self.isHost:
+        if self._is_host:
             self.send_stream_function(self.stream_function(1, 13)())
         else:
-            self.send_stream_function(self.stream_function(1, 13)([self.MDLN, self.SOFTREV]))
+            self.send_stream_function(self.stream_function(1, 13)([self._mdln, self._softrev]))
 
     def _on_state_wait_delay(self, _):
         """
         Connection state model changed to state WAIT_DELAY.
 
         :param data: event attributes
         :type data: object
         """
-        self.logger.debug("connectionState -> WAIT_DELAY")
+        self._logger.debug("connectionState -> WAIT_DELAY")
 
-        self.commDelayTimer = threading.Timer(self.establishCommunicationTimeout, self._on_wait_comm_delay_timeout)
-        self.commDelayTimer.start()
+        self._comm_delay_timer = threading.Timer(self._establish_communication_timeout,
+                                                 self._on_wait_comm_delay_timeout)
+        self._comm_delay_timer.start()
 
     def _on_state_leave_wait_cra(self, _):
         """
         Connection state model changed to state WAIT_CRA.
 
         :param data: event attributes
         :type data: object
         """
-        if self.waitCRATimer is not None:
-            self.waitCRATimer.cancel()
+        if self._wait_cra_timer is not None:
+            self._wait_cra_timer.cancel()
 
     def _on_state_leave_wait_delay(self, _):
         """
         Connection state model changed to state WAIT_DELAY.
 
         :param data: event attributes
         :type data: object
         """
-        if self.commDelayTimer is not None:
-            self.commDelayTimer.cancel()
+        if self._comm_delay_timer is not None:
+            self._comm_delay_timer.cancel()
 
     def _on_state_communicating(self, _):
         """
         Connection state model changed to state COMMUNICATING.
 
         :param data: event attributes
         :type data: object
         """
-        self.logger.debug("connectionState -> COMMUNICATING")
+        self._logger.debug("connectionState -> COMMUNICATING")
 
         self.events.fire("handler_communicating", {'handler': self})
 
-        for event in self.waitEventList:
+        for event in self._wait_event_list:
             event.set()
 
     def on_connection_closed(self, connection):
         """Handle connection was closed event."""
-        self.logger.info("Connection was closed")
+        self._logger.info("Connection was closed")
 
         # call parent handlers
         super().on_connection_closed(connection)
 
-        if self.communicationState.current == "COMMUNICATING":
+        if self._communication_state.current == "COMMUNICATING":
             # update communication state
-            self.communicationState.communicationfail()
+            self._communication_state.communicationfail()
 
     def on_commack_requested(self) -> int:
         """
         Get the acknowledgement code for the connection request.
 
         override to accept or deny connection request
 
@@ -251,28 +256,28 @@
 
         :param ppid: Transferred process programs ID
         :type ppid: string
         :param ppbody: Content of process program
         :type ppbody: string
         """
         # send remote command
-        self.logger.info("Send process program %s", ppid)
+        self._logger.info("Send process program %s", ppid)
 
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(7, 3)(
             {"PPID": ppid, "PPBODY": ppbody}))).get()
 
     def request_process_program(self, 
                                 ppid: typing.Union[int, str]) -> typing.Tuple[typing.Union[int, str], str]:
         """
         Request a process program.
 
         :param ppid: Transferred process programs ID
         :type ppid: string
         """
-        self.logger.info("Request process program %s", ppid)
+        self._logger.info("Request process program %s", ppid)
 
         # send remote command
         s7f6 = self.secs_decode(self.send_and_waitfor_response(self.stream_function(7, 5)(ppid)))
         return s7f6.PPID.get(), s7f6.PPBODY.get()
 
     def waitfor_communicating(self, timeout: typing.Optional[float] = None) -> bool:
         """
@@ -280,55 +285,55 @@
 
         :param timeout: seconds to wait before aborting
         :type timeout: float
         :returns: True if state is communicating, False if timed out
         :rtype: bool
         """
         event = threading.Event()
-        self.waitEventList.append(event)
+        self._wait_event_list.append(event)
 
-        if self.communicationState.isstate("COMMUNICATING"):
-            self.waitEventList.remove(event)
+        if self._communication_state.isstate("COMMUNICATING"):
+            self._wait_event_list.remove(event)
             return True
 
         result = event.wait(timeout)
 
-        self.waitEventList.remove(event)
+        self._wait_event_list.remove(event)
 
         return result
 
     def _on_s01f01(self, 
                    handler: secsgem.secs.SecsHandler, 
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 1, Function 1, Are You There.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler, packet  # unused parameters
 
-        if self.isHost:
+        if self._is_host:
             return self.stream_function(1, 2)()
 
-        return self.stream_function(1, 2)([self.MDLN, self.SOFTREV])
+        return self.stream_function(1, 2)([self._mdln, self._softrev])
 
     def _on_s01f13(self, 
                    handler: secsgem.secs.SecsHandler, 
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 1, Function 13, Establish Communication Request.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler, packet  # unused parameters
 
-        if self.isHost:
+        if self._is_host:
             return self.stream_function(1, 14)({"COMMACK": self.on_commack_requested(), "MDLN": []})
 
         return self.stream_function(1, 14)({"COMMACK": self.on_commack_requested(),
-                                            "MDLN": [self.MDLN, self.SOFTREV]})
+                                            "MDLN": [self._mdln, self._softrev]})
```

### Comparing `secsgem-0.2.0a3/secsgem/gem/hosthandler.py` & `secsgem-0.2.0a4/secsgem/gem/hosthandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,41 +13,41 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Handler for GEM host."""
 import collections
 import typing
 
-import secsgem.hsms
+import secsgem.common
 import secsgem.secs
 
 from .handler import GemHandler
 
 
 class GemHostHandler(GemHandler):
     """Baseclass for creating host models. Inherit from this class and override required functions."""
 
-    def __init__(self, connection: secsgem.hsms.HsmsHandler):
+    def __init__(self, connection: secsgem.common.Protocol):
         """
         Initialize a gem host handler.
 
         :param connection: Connection
         """
         GemHandler.__init__(self, connection)
 
-        self.isHost = True
+        self.is_host = True
 
-        self.reportSubscriptions: typing.Dict[typing.Union[int, str], typing.List[typing.Union[int, str]]] = {}
+        self.report_subscriptions: typing.Dict[typing.Union[int, str], typing.List[typing.Union[int, str]]] = {}
 
     def clear_collection_events(self) -> None:
         """Clear all collection events."""
-        self.logger.info("Clearing collection events")
+        self._logger.info("Clearing collection events")
 
         # clear subscribed reports
-        self.reportSubscriptions = {}
+        self.report_subscriptions = {}
 
         # disable all ceids
         self.disable_ceids()
 
         # delete all reports
         self.disable_ceid_reports()
 
@@ -61,22 +61,22 @@
         :param ceid: ID of the collection event
         :type ceid: integer
         :param dvs: DV IDs to add for collection event
         :type dvs: list of integers
         :param report_id: optional - ID for report, autonumbering if None
         :type report_id: integer
         """
-        self.logger.info("Subscribing to collection event %s", ceid)
+        self._logger.info("Subscribing to collection event %s", ceid)
 
         if report_id is None:
-            report_id = self.reportIDCounter
-            self.reportIDCounter += 1
+            report_id = self._report_id_counter
+            self._report_id_counter += 1
 
         # note subscribed reports
-        self.reportSubscriptions[report_id] = dvs
+        self.report_subscriptions[report_id] = dvs
 
         # create report
         self.send_and_waitfor_response(self.stream_function(2, 33)(
             {"DATAID": 0, "DATA": [{"RPTID": report_id, "VID": dvs}]}))
 
         # link event report to collection event
         self.send_and_waitfor_response(self.stream_function(2, 35)(
@@ -92,15 +92,15 @@
         Send a remote command.
 
         :param rcmd: Name of command
         :type rcmd: string
         :param params: DV IDs to add for collection event
         :type params: list of strings
         """
-        self.logger.info("Send RCMD %s", rcmd)
+        self._logger.info("Send RCMD %s", rcmd)
 
         s2f41 = self.stream_function(2, 41)()
         s2f41.RCMD = rcmd
         if isinstance(params, list):
             for param in params:
                 s2f41.PARAMS.append({"CPNAME": param[0], "CPVAL": param[1]})
         elif isinstance(params, collections.OrderedDict):
@@ -114,159 +114,161 @@
                                 ppids: typing.List[typing.Union[int, str]]):
         """
         Delete a list of process program.
 
         :param ppids: Process programs to delete
         :type ppids: list of strings
         """
-        self.logger.info("Delete process programs %s", ppids)
+        self._logger.info("Delete process programs %s", ppids)
 
         # send remote command
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(7, 17)(ppids))).get()
 
     def get_process_program_list(self) -> secsgem.secs.SecsStreamFunction:
         """Get process program list."""
-        self.logger.info("Get process program list")
+        self._logger.info("Get process program list")
 
         # send remote command
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(7, 19)())).get()
 
     def go_online(self) -> typing.Optional[str]:
         """Set control state to online."""
-        self.logger.info("Go online")
+        self._logger.info("Go online")
 
         # send remote command
         resp = self.secs_decode(self.send_and_waitfor_response(self.stream_function(1, 17)()))
         if resp is None:
             return None
 
         return resp.get()
 
     def go_offline(self) -> typing.Optional[str]:
         """Set control state to offline."""
-        self.logger.info("Go offline")
+        self._logger.info("Go offline")
 
         # send remote command
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(1, 15)())).get()
 
     def enable_alarm(self, alid: typing.Union[int, str]):
         """
         Enable alarm.
 
         :param alid: alarm id to enable
         :type alid: :class:`secsgem.secs.dataitems.ALID`
         """
-        self.logger.info("Enable alarm %d", alid)
+        self._logger.info("Enable alarm %d", alid)
 
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(5, 3)(
             {"ALED": secsgem.secs.data_items.ALED.ENABLE, "ALID": alid}))).get()
 
     def disable_alarm(self, alid: typing.Union[int, str]):
         """
         Disable alarm.
 
         :param alid: alarm id to disable
         :type alid: :class:`secsgem.secs.dataitems.ALID`
         """
-        self.logger.info("Disable alarm %d", alid)
+        self._logger.info("Disable alarm %d", alid)
 
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(5, 3)(
             {"ALED": secsgem.secs.data_items.ALED.DISABLE, "ALID": alid}))).get()
 
     def list_alarms(self, 
                     alids: typing.Optional[typing.List[typing.Union[int, str]]] = None):
         """
         List alarms.
 
         :param alids: alarms to list details for
         :type alids: array of int/str
         """
         if alids is None:
             alids = []
-            self.logger.info("List all alarms")
+            self._logger.info("List all alarms")
         else:
-            self.logger.info("List alarms %s", alids)
+            self._logger.info("List alarms %s", alids)
 
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(5, 5)(alids))).get()
 
     def list_enabled_alarms(self):
         """List enabled alarms."""
-        self.logger.info("List all enabled alarms")
+        self._logger.info("List all enabled alarms")
 
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(5, 7)())).get()
 
-    def _on_alarm_received(self, handler, ALID, ALCD, ALTX):
-        del handler, ALID, ALCD, ALTX  # unused variables
+    def _on_alarm_received(self, handler, alarm_id, alarm_code, alarm_text):
+        del handler, alarm_id, alarm_code, alarm_text  # unused variables
         return secsgem.secs.data_items.ACKC5.ACCEPTED
 
     def _on_s05f01(self, 
                    handler: secsgem.secs.SecsHandler, 
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 5, Function 1, Alarm request.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         s5f1 = self.secs_decode(packet)
 
         result = self._callback_handler.alarm_received(handler, s5f1.ALID, s5f1.ALCD, s5f1.ALTX)
 
         self.events.fire("alarm_received", {"code": s5f1.ALCD, "alid": s5f1.ALID, "text": s5f1.ALTX,
-                                            "handler": self.connection, 'peer': self})
+                                            "handler": self.protocol, 'peer': self})
 
         return self.stream_function(5, 2)(result)
 
     def _on_s06f11(self, 
                    handler: secsgem.secs.SecsHandler, 
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 6, Function 11, Establish Communication Request.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         del handler  # unused parameters
 
         message = self.secs_decode(packet)
 
         for report in message.RPT:
-            report_dvs = self.reportSubscriptions[report.RPTID.get()]
+            report_dvs = self.report_subscriptions[report.RPTID.get()]
             report_values = report.V.get()
 
             values = []
 
-            for i, s in enumerate(report_dvs):
-                values.append({"dvid": s, "value": report_values[i], "name": self.get_dvid_name(s)})
+            for index, data_value_id in enumerate(report_dvs):
+                values.append({"dvid": data_value_id,
+                               "value": report_values[index],
+                               "name": self.get_dvid_name(data_value_id)})
 
             data = {"ceid": message.CEID, "rptid": report.RPTID, "values": values,
-                    "name": self.get_ceid_name(message.CEID), "handler": self.connection, 'peer': self}
+                    "name": self.get_ceid_name(message.CEID), "handler": self.protocol, 'peer': self}
             self.events.fire("collection_event_received", data)
 
         return self.stream_function(6, 12)(0)
 
-    def _on_terminal_received(self, handler, TID, TEXT):
-        del handler, TID, TEXT  # unused variables
+    def _on_terminal_received(self, handler, terminal_id, text):
+        del handler, terminal_id, text  # unused variables
         return secsgem.secs.data_items.ACKC10.ACCEPTED
 
     def _on_s10f01(self, 
                    handler: secsgem.secs.SecsHandler, 
-                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
+                   packet: secsgem.common.Packet) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 10, Function 1, Terminal Request.
 
         :param handler: handler the message was received on
-        :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
+        :type handler: :class:`secsgem.secs.SecsHandler`
         :param packet: complete message received
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         """
         s10f1 = self.secs_decode(packet)
 
         result = self._callback_handler.terminal_received(handler, s10f1.TID, s10f1.TEXT)
-        self.events.fire("terminal_received", {"text": s10f1.TEXT, "terminal": s10f1.TID, "handler": self.connection,
+        self.events.fire("terminal_received", {"text": s10f1.TEXT, "terminal": s10f1.TID, "handler": self.protocol,
                                                'peer': self})
 
         return self.stream_function(10, 2)(result)
```

### Comparing `secsgem-0.2.0a3/secsgem/gem/remote_command.py` & `secsgem-0.2.0a4/secsgem/gem/remote_command.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/gem/status_variable.py` & `secsgem-0.2.0a4/secsgem/gem/status_variable.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/hsms/__init__.py` & `secsgem-0.2.0a4/secsgem/hsms/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """module imports."""
 
 from .connectionmanager import HsmsConnectionManager
-from .handler import HsmsHandler
+from .protocol import HsmsProtocol
 from .packet import HsmsPacket
 from .stream_function_header import HsmsStreamFunctionHeader
 from .separate_req_header import HsmsSeparateReqHeader
 from .reject_req_header import HsmsRejectReqHeader
 from .linktest_rsp_header import HsmsLinktestRspHeader
 from .linktest_req_header import HsmsLinktestReqHeader
 from .deselect_rsp_header import HsmsDeselectRspHeader
 from .deselect_req_header import HsmsDeselectReqHeader
 from .select_rsp_header import HsmsSelectRspHeader
 from .select_req_header import HsmsSelectReqHeader
 from .header import HsmsHeader
 
-__all__ = ["HsmsConnectionManager", "HsmsHandler", "HsmsPacket", "HsmsStreamFunctionHeader", "HsmsSeparateReqHeader",
+__all__ = ["HsmsConnectionManager", "HsmsProtocol", "HsmsPacket", "HsmsStreamFunctionHeader", "HsmsSeparateReqHeader",
            "HsmsRejectReqHeader", "HsmsLinktestRspHeader", "HsmsLinktestReqHeader", "HsmsDeselectRspHeader",
            "HsmsDeselectReqHeader", "HsmsSelectRspHeader", "HsmsSelectReqHeader", "HsmsHeader"]
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/active_connection.py` & `secsgem-0.2.0a4/secsgem/hsms/active_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,19 +46,19 @@
         # initialize super class
         HsmsConnection.__init__(self, True, address, port, session_id, delegate)
 
         # initially not enabled
         self.enabled = False
 
         # reconnect thread required for active connection
-        self.connectionThread = None
-        self.stopConnectionThread = False
+        self.connection_thread = None
+        self.stop_connection_thread = False
 
         # flag if this is the first connection since enable
-        self.firstConnection = True
+        self.first_connection = True
 
     def _on_hsms_connection_close(self, data):
         """
         Signal from super that the connection was closed.
 
         This is required to initiate the reconnect if the connection is still enabled
         """
@@ -70,15 +70,15 @@
         Enable the connection.
 
         Starts the connection process to the passive remote.
         """
         # only start if not already enabled
         if not self.enabled:
             # reset first connection to eliminate reconnection timeout
-            self.firstConnection = True
+            self.first_connection = True
 
             # mark connection as enabled
             self.enabled = True
 
             # start the connection thread
             self.__start_connect_thread()
 
@@ -90,19 +90,19 @@
         """
         # only stop if enabled
         if self.enabled:
             # mark connection as disabled
             self.enabled = False
 
             # stop connection thread if it is running
-            if self.connectionThread and self.connectionThread.is_alive():
-                self.stopConnectionThread = True
+            if self.connection_thread and self.connection_thread.is_alive():
+                self.stop_connection_thread = True
 
             # wait for connection thread to stop
-            while self.stopConnectionThread:
+            while self.stop_connection_thread:
                 time.sleep(0.2)
 
             # disconnect super class
             self.disconnect()
 
     def __idle(self, timeout):
         """
@@ -113,66 +113,66 @@
         :returns: False if thread was stopped
         :rtype: boolean
         """
         for _ in range(int(timeout) * 5):
             time.sleep(0.2)
 
             # check if connection was disabled
-            if self.stopConnectionThread:
-                self.stopConnectionThread = False
+            if self.stop_connection_thread:
+                self.stop_connection_thread = False
                 return False
 
         return True
 
     def __start_connect_thread(self):
-        self.connectionThread = threading.Thread(
+        self.connection_thread = threading.Thread(
             target=self.__connect_thread,
-            name=f"secsgem_HsmsActiveConnection_connectThread_{self.remoteAddress}")
-        self.connectionThread.start()
+            name=f"secsgem_HsmsActiveConnection_connectThread_{self._remote_address}")
+        self.connection_thread.start()
 
     def __connect_thread(self):
         """
         Thread function to (re)connect active connection to remote host.
 
         .. warning:: Do not call this directly, for internal use only.
         """
         # wait for timeout if this is not the first connection
-        if not self.firstConnection:
-            if not self.__idle(self.T5):
+        if not self.first_connection:
+            if not self.__idle(self.timeouts.t5):
                 return
 
-        self.firstConnection = False
+        self.first_connection = False
 
         # try to connect to remote
         while not self.__connect():
-            if not self.__idle(self.T5):
+            if not self.__idle(self.timeouts.t5):
                 return
 
     def __connect(self):
         """
         Open connection to remote host.
 
         :returns: True if connection was established, False if connection failed
         :rtype: boolean
         """
         # create socket
-        self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self._sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
         # setup socket
-        self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
+        self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
 
-        self.logger.debug("connecting to %s:%d", self.remoteAddress, self.remotePort)
+        self._logger.debug("connecting to %s:%d", self._remote_address, self._remote_port)
 
         # try to connect socket
         try:
-            self.sock.connect((self.remoteAddress, self.remotePort))
+            self._sock.connect((self._remote_address, self._remote_port))
         except socket.error:
-            self.logger.debug("connecting to %s:%d failed", self.remoteAddress, self.remotePort)
+            self._logger.debug("connecting to %s:%d failed", self._remote_address, self._remote_port)
             return False
 
         # make socket nonblocking
-        self.sock.setblocking(0)
+        self._sock.setblocking(0)
 
         # start the receiver thread
         self._start_receiver()
 
         return True
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/connection.py` & `secsgem-0.2.0a4/secsgem/hsms/connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,144 +36,148 @@
     6: "Linktest.rsp",
     7: "Reject.req",
     9: "Separate.req"
 }
 """Names for hsms header SType."""
 
 
-class HsmsConnection:  # pragma: no cover
+class HsmsConnection:  # pragma: no cover # pylint: disable=too-many-instance-attributes
     """Connection class used for active and passive hsms connections."""
 
     select_timeout = 0.5
     """ Timeout for select calls ."""
 
     send_block_size = 1024 * 1024
     """ Block size for outbound data ."""
 
-    T3 = 45.0
-    """ Reply Timeout ."""
-
-    T5 = 10.0
-    """ Connect Separation Time ."""
-
-    T6 = 5.0
-    """ Control Transaction Timeout ."""
-
     def __init__(self, active, address, port, session_id=0, delegate=None):
         """
         Initialize a hsms connection.
 
         :param active: Is the connection active (*True*) or passive (*False*)
         :type active: boolean
         :param address: IP address of remote host
         :type address: string
         :param port: TCP port of remote host
         :type port: integer
         :param session_id: session / device ID to use for connection
         :type session_id: integer
         :param delegate: target for messages
-        :type delegate: inherited from :class:`secsgem.hsms.handler.HsmsHandler`
+        :type delegate: inherited from :class:`secsgem.hsms.protocol.HsmsProtocol`
         """
-        self.logger = logging.getLogger(self.__module__ + "." + self.__class__.__name__)
+        self._logger = logging.getLogger(self.__module__ + "." + self.__class__.__name__)
 
         # set parameters
-        self.active = active
-        self.remoteAddress = address
-        self.remotePort = port
-        self.sessionID = session_id
-        self.delegate = delegate
+        self._active = active
+        self._remote_address = address
+        self._remote_port = port
+        self._session_id = session_id
+        self._delegate = delegate
 
         # connection socket
-        self.sock = None
+        self._sock = None
 
         # buffer for received data
-        self.receiveBuffer = b""
+        self._receive_buffer = b""
 
         # receiving thread flags
-        self.threadRunning = False
-        self.stopThread = False
+        self._thread_running = False
+        self._stop_thread = False
 
         # connected flag
-        self.connected = False
+        self._connected = False
 
         # flag set during disconnection
-        self.disconnecting = False
+        self._disconnecting = False
+
+        self._timeouts = secsgem.common.Timeouts()
+
+    @property
+    def timeouts(self) -> secsgem.common.Timeouts:
+        """Get connection timeouts."""
+        return self._timeouts
+
+    @property
+    def disconnecting(self) -> bool:
+        """Connection is disconnecting."""
+        return self._disconnecting
 
     def _serialize_data(self):
         """
         Return data for serialization.
 
         :returns: data to serialize for this object
         :rtype: dict
         """
         return {
-            'active': self.active,
-            'remoteAddress': self.remoteAddress,
-            'remotePort': self.remotePort,
-            'sessionID': self.sessionID,
-            'connected': self.connected}
+            'active': self._active,
+            'remoteAddress': self._remote_address,
+            'remotePort': self._remote_port,
+            'session_id': self._session_id,
+            'connected': self._connected}
 
     def __str__(self):
         """Get the contents of this object as a string."""
-        return f"{('Active' if self.active else 'Passive')} connection to {self.remoteAddress}:{str(self.remotePort)}" \
-               f" sessionID={str(self.sessionID)}"
+        return f"{('Active' if self._active else 'Passive')} connection to " \
+               f"{self._remote_address}:{str(self._remote_port)}" \
+               f" session_id={str(self._session_id)}"
 
     def _start_receiver(self):
         """
         Start the thread for receiving and handling incoming messages.
 
         Will also do the initial Select and Linktest requests.
 
         .. warning:: Do not call this directly, will be called from HSMS client/server class.
         .. seealso:: :class:`secsgem.hsms.connections.HsmsActiveConnection`,
             :class:`secsgem.hsms.connections.HsmsPassiveConnection`,
             :class:`secsgem.hsms.connections.HsmsMultiPassiveConnection`
         """
         # mark connection as connected
-        self.connected = True
+        self._connected = True
 
         # start data receiving thread
         threading.Thread(target=self.__receiver_thread, args=(),
-                         name=f"secsgem_hsmsConnection_receiver_{self.remoteAddress}:{self.remotePort}").start()
+                         name=f"secsgem_hsmsConnection_receiver_{self._remote_address}:{self._remote_port}").start()
 
         # wait until thread is running
-        while not self.threadRunning:
+        while not self._thread_running:
             pass
 
         # send event
-        if self.delegate and hasattr(self.delegate, 'on_connection_established') \
-                and callable(getattr(self.delegate, 'on_connection_established')):
+        if self._delegate and hasattr(self._delegate, 'on_connection_established') \
+                and callable(getattr(self._delegate, 'on_connection_established')):
             try:
-                self.delegate.on_connection_established(self)
+                self._delegate.on_connection_established(self)
             except Exception:  # pylint: disable=broad-except
-                self.logger.exception('ignoring exception for on_connection_established handler')
+                self._logger.exception('ignoring exception for on_connection_established handler')
 
     def _on_hsms_connection_close(self, data):
         pass
 
     def disconnect(self):
         """Close connection."""
         # return if thread isn't running
-        if not self.threadRunning:
+        if not self._thread_running:
             return
 
         # set disconnecting flag to avoid another select
-        self.disconnecting = True
+        self._disconnecting = True
 
         # set flag to stop the thread
-        self.stopThread = True
+        self._stop_thread = True
 
         # wait until thread stopped
-        while self.threadRunning:
+        while self._thread_running:
             pass
 
         # clear disconnecting flag, no selects coming any more
-        self.disconnecting = False
+        self._disconnecting = False
 
-    def send_packet(self, packet):
+    def send_packet(self, packet) -> bool:
         """
         Send the ASCII coded packet to the remote host.
 
         :param packet: encoded data to be transmitted
         :type packet: string / byte array
         """
         # encode the packet
@@ -184,20 +188,20 @@
 
         for block in blocks:
             retry = True
 
             # not sent yet, retry
             while retry:
                 # wait until socket is writable
-                while not select.select([], [self.sock], [], self.select_timeout)[1]:
+                while not select.select([], [self._sock], [], self.select_timeout)[1]:
                     pass
 
                 try:
                     # send packet
-                    self.sock.send(block)
+                    self._sock.send(block)
 
                     # retry will be cleared if send succeeded
                     retry = False
                 except OSError as exc:
                     if not secsgem.common.is_errorcode_ewouldblock(exc.errno):
                         # raise if not EWOULDBLOCK
                         return False
@@ -209,69 +213,69 @@
         """
         Parse the receive buffer and dispatch callbacks.
 
         .. warning:: Do not call this directly, will be called from
         :func:`secsgem.hsmsConnections.hsmsConnection.__receiver_thread` method.
         """
         # check if enough data in input buffer
-        if len(self.receiveBuffer) < 4:
+        if len(self._receive_buffer) < 4:
             return False
 
         # unpack length from input buffer
-        length = struct.unpack(">L", self.receiveBuffer[0:4])[0] + 4
+        length = struct.unpack(">L", self._receive_buffer[0:4])[0] + 4
 
         # check if enough data in input buffer
-        if len(self.receiveBuffer) < length:
+        if len(self._receive_buffer) < length:
             return False
 
         # extract and remove packet from input buffer
-        data = self.receiveBuffer[0:length]
-        self.receiveBuffer = self.receiveBuffer[length:]
+        data = self._receive_buffer[0:length]
+        self._receive_buffer = self._receive_buffer[length:]
 
         # decode received packet
         response = HsmsPacket.decode(data)
 
         # redirect packet to hsms handler
-        if self.delegate and hasattr(self.delegate, 'on_connection_packet_received') \
-                and callable(getattr(self.delegate, 'on_connection_packet_received')):
+        if self._delegate and hasattr(self._delegate, 'on_connection_packet_received') \
+                and callable(getattr(self._delegate, 'on_connection_packet_received')):
             try:
-                self.delegate.on_connection_packet_received(self, response)
+                self._delegate.on_connection_packet_received(self, response)
             except Exception:  # pylint: disable=broad-except
-                self.logger.exception('ignoring exception for on_connection_packet_received handler')
+                self._logger.exception('ignoring exception for on_connection_packet_received handler')
 
         # return True if more data is available
-        if len(self.receiveBuffer) > 0:
+        if len(self._receive_buffer) > 0:
             return True
 
         return False
 
     def __receiver_thread_read_data(self):
         # check if shutdown requested
-        while not self.stopThread:
+        while not self._stop_thread:
             # check if data available
-            select_result = select.select([self.sock], [], [self.sock], self.select_timeout)
+            select_result = select.select([self._sock], [], [self._sock], self.select_timeout)
 
             # check if disconnection was started
-            if self.disconnecting:
+            if self._disconnecting:
                 time.sleep(0.2)
                 continue
 
             if select_result[0]:
                 try:
                     # get data from socket
-                    recv_data = self.sock.recv(1024)
+                    recv_data = self._sock.recv(1024)
 
                     # check if socket was closed
                     if len(recv_data) == 0:
-                        self.connected = False
-                        self.stopThread = True
+                        self._connected = False
+                        self._stop_thread = True
                         continue
 
                     # add received data to input buffer
-                    self.receiveBuffer += recv_data
+                    self._receive_buffer += recv_data
                 except OSError as exc:
                     if not secsgem.common.is_errorcode_ewouldblock(exc.errno):
                         raise exc
 
                 # handle data in input buffer
                 while self._process_receive_buffer():
                     pass
@@ -279,43 +283,43 @@
     def __receiver_thread(self):
         """
         Thread for receiving incoming data and adding it to the receive buffer.
 
         .. warning:: Do not call this directly, will be called from
         :func:`secsgem.hsmsConnections.hsmsConnection._startReceiver` method.
         """
-        self.threadRunning = True
+        self._thread_running = True
 
         try:
             self.__receiver_thread_read_data()
         except Exception:  # pylint: disable=broad-except
-            self.logger.exception('exception')
+            self._logger.exception('exception')
 
         # notify listeners of disconnection
-        if self.delegate and hasattr(self.delegate, 'on_connection_before_closed') \
-                and callable(getattr(self.delegate, 'on_connection_before_closed')):
+        if self._delegate and hasattr(self._delegate, 'on_connection_before_closed') \
+                and callable(getattr(self._delegate, 'on_connection_before_closed')):
             try:
-                self.delegate.on_connection_before_closed(self)
+                self._delegate.on_connection_before_closed(self)
             except Exception:  # pylint: disable=broad-except
-                self.logger.exception('ignoring exception for on_connection_before_closed handler')
+                self._logger.exception('ignoring exception for on_connection_before_closed handler')
 
         # close the socket
-        self.sock.close()
+        self._sock.close()
 
         # notify listeners of disconnection
-        if self.delegate and hasattr(self.delegate, 'on_connection_closed') \
-                and callable(getattr(self.delegate, 'on_connection_closed')):
+        if self._delegate and hasattr(self._delegate, 'on_connection_closed') \
+                and callable(getattr(self._delegate, 'on_connection_closed')):
             try:
-                self.delegate.on_connection_closed(self)
+                self._delegate.on_connection_closed(self)
             except Exception:  # pylint: disable=broad-except
-                self.logger.exception('ignoring exception for on_connection_closed handler')
+                self._logger.exception('ignoring exception for on_connection_closed handler')
 
         # reset all flags
-        self.connected = False
-        self.threadRunning = False
-        self.stopThread = False
+        self._connected = False
+        self._thread_running = False
+        self._stop_thread = False
 
         # clear receive buffer
-        self.receiveBuffer = b""
+        self._receive_buffer = b""
 
         # notify inherited classes of disconnection
         self._on_hsms_connection_close({'connection': self})
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/connectionmanager.py` & `secsgem-0.2.0a4/secsgem/hsms/connectionmanager.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,39 +15,39 @@
 #####################################################################
 """Contains class for handling multiple connections."""
 
 import logging
 
 import secsgem.common
 
-from .handler import HsmsHandler
+from .protocol import HsmsProtocol
 from .multi_passive_server import HsmsMultiPassiveServer
 
 
 class HsmsConnectionManager:
     """High level class that handles multiple active and passive connections and the model for them."""
 
     def __init__(self):
         """Initialize a hsms connection manager."""
-        self._eventProducer = secsgem.common.EventProducer()
+        self._event_producer = secsgem.common.EventProducer()
 
         self.logger = logging.getLogger(self.__module__ + "." + self.__class__.__name__)
 
         self.handlers = {}
 
         self.servers = {}
 
         self.stopping = False
 
-        self._testServerObject = None
+        self._test_server_object = None
 
     @property
     def events(self):
         """Property for event handling."""
-        return self._eventProducer
+        return self._event_producer
 
     def has_connection_to(self, index):
         """
         Check if connection to certain peer exists.
 
         :param index: Name of the reqested handler.
         :type index: string
@@ -76,74 +76,74 @@
 
     def _update_required_servers(self, additional_port=-1):  # pragma: no cover
         """
         Start server if any active handler is found.
 
         .. warning:: Do not call this directly, for internal use only.
         """
-        if self._testServerObject:
+        if self._test_server_object:
             return
 
         required_ports = []
 
         if additional_port > 0:
             required_ports.append(additional_port)
 
         for handler in self.handlers.values():
             if not handler.active:
                 if handler.port not in required_ports:
                     required_ports.append(handler.port)
 
-        for serverPort, server in self.servers.items():
-            if serverPort not in required_ports:
-                self.logger.debug("stopping server on port %d", serverPort)
+        for server_port, server in self.servers.items():
+            if server_port not in required_ports:
+                self.logger.debug("stopping server on port %d", server_port)
                 server.stop()
-                del self.servers[serverPort]
+                del self.servers[server_port]
 
-        for requiredPort in required_ports:
-            if requiredPort not in self.servers:
-                self.logger.debug("starting server on port %d", requiredPort)
-                self.servers[requiredPort] = HsmsMultiPassiveServer(requiredPort)
-                self.servers[requiredPort].start()
+        for required_port in required_ports:
+            if required_port not in self.servers:
+                self.logger.debug("starting server on port %d", required_port)
+                self.servers[required_port] = HsmsMultiPassiveServer(required_port)
+                self.servers[required_port].start()
 
-    def add_peer(self, name, address, port, active, session_id, connection_handler=HsmsHandler):
+    def add_peer(self, name, address, port, active, session_id, connection_handler=HsmsProtocol):
         """
         Add a new connection.
 
         :param name: Name of the peers configuration
         :type name: string
         :param address: IP address of peer
         :type address: string
         :param port: TCP port of peer
         :type port: integer
         :param active: Is the connection active (*True*) or passive (*False*)
         :type active: boolean
         :param session_id: session / device ID of peer
         :type session_id: integer
         :param connection_handler: Model handling this connection
-        :type connection_handler: inherited from :class:`secsgem.hsms.handler.HsmsHandler`
+        :type connection_handler: inherited from :class:`secsgem.hsms.protocol.HsmsProtocol`
         """
         self.logger.debug("new remote %s at %s:%d", name, address, port)
 
         connection_id = self.get_connection_id(address)
 
         self._update_required_servers(port)
 
-        if self._testServerObject:
+        if self._test_server_object:
             if active:
-                handler = connection_handler(address, port, active, session_id, name, self._testServerObject)
+                handler = connection_handler(address, port, active, session_id, name, self._test_server_object)
             else:
-                handler = connection_handler(address, port, active, session_id, name, self._testServerObject)
+                handler = connection_handler(address, port, active, session_id, name, self._test_server_object)
         else:  # pragma: no cover
             if active:
                 handler = connection_handler(address, port, active, session_id, name)
             else:
                 handler = connection_handler(address, port, active, session_id, name, self.servers[port])
 
-        handler._eventProducer += self._eventProducer
+        handler._event_producer += self._event_producer
         handler.enable()
 
         self.handlers[connection_id] = handler
 
         return handler
 
     def remove_peer(self, name, address, port):
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/connectionstatemachine.py` & `secsgem-0.2.0a4/secsgem/hsms/connectionstatemachine.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,42 +36,42 @@
 
         :param callbacks: callbacks for the state machine
         """
         self.callbacks = {}
 
         self.states = [STATE_NOT_CONNECTED,
                        {
-                            'name': STATE_CONNECTED,
-                            'on_enter': self._on_enter_CONNECTED,
-                            'on_exit': self._on_exit_CONNECTED,
-                            'children': [
-                                STATE_NOT_SELECTED,
-                                {
-                                    'name': STATE_SELECTED,
-                                    'on_enter': self._on_enter_CONNECTED_SELECTED
-                                }
-                            ]
+                           'name': STATE_CONNECTED,
+                           'on_enter': self._on_enter_connected,
+                           'on_exit': self._on_exit_connected,
+                           'children': [
+                               STATE_NOT_SELECTED,
+                               {
+                                   'name': STATE_SELECTED,
+                                   'on_enter': self._on_enter_connected_selected
+                               }
+                           ]
                        }]
 
         # transition 1
         self.machine = Machine(model=self, states=self.states, initial=STATE_NOT_CONNECTED, auto_transitions=False)
 
         if callbacks:
             self.callbacks = callbacks
 
         self.machine.add_transition('connect', STATE_NOT_CONNECTED, STATE_CONNECTED_NOT_SELECTED)  # transition 2
         self.machine.add_transition('disconnect', STATE_CONNECTED, STATE_NOT_CONNECTED)  # transition 3
         self.machine.add_transition('select', STATE_CONNECTED_NOT_SELECTED, STATE_CONNECTED_SELECTED)  # transition 4
         self.machine.add_transition('deselect', STATE_CONNECTED_SELECTED, STATE_CONNECTED_NOT_SELECTED)  # transition 5
         self.machine.add_transition('timeoutT7', STATE_CONNECTED_NOT_SELECTED, STATE_NOT_CONNECTED)  # transition 6
 
-    def _on_enter_CONNECTED(self):
+    def _on_enter_connected(self):
         if "on_enter_CONNECTED" in self.callbacks:
             self.callbacks["on_enter_CONNECTED"]()
 
-    def _on_exit_CONNECTED(self):
+    def _on_exit_connected(self):
         if "on_exit_CONNECTED" in self.callbacks:
             self.callbacks["on_exit_CONNECTED"]()
 
-    def _on_enter_CONNECTED_SELECTED(self):
+    def _on_enter_connected_selected(self):
         if "on_enter_CONNECTED_SELECTED" in self.callbacks:
             self.callbacks["on_enter_CONNECTED_SELECTED"]()
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/deselect_req_header.py` & `secsgem-0.2.0a4/secsgem/hsms/select_req_header.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 #####################################################################
-# deselect_req_header.py
+# select_req_header.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Header for the hsms deselect request."""
+"""Header for the hsms select request."""
 
 from .header import HsmsHeader
 
 
-class HsmsDeselectReqHeader(HsmsHeader):
+class HsmsSelectReqHeader(HsmsHeader):
     """
-    Header for Deselect Request.
+    Header for Select Request.
 
-    Header for message with SType 3.
+    Header for message with SType 1.
     """
 
     def __init__(self, system):
         """
-        Initialize a hsms deselect request.
+        Initialize a hsms select request.
 
         :param system: message ID
         :type system: integer
 
         **Example**::
 
             >>> import secsgem.hsms
             >>>
-            >>> secsgem.hsms.HsmsDeselectReqHeader(1)
-            HsmsDeselectReqHeader({sessionID:0xffff, stream:00, function:00, pType:0x00, sType:0x03, \
-system:0x00000001, requireResponse:False})
+            >>> secsgem.hsms.HsmsSelectReqHeader(14)
+            HsmsSelectReqHeader({session_id:0xffff, stream:00, function:00, p_type:0x00, s_type:0x01, \
+system:0x0000000e, require_response:False})
         """
-        HsmsHeader.__init__(self, system, 0xFFFF)
-        self.requireResponse = False
-        self.stream = 0x00
-        self.function = 0x00
-        self.pType = 0x00
-        self.sType = 0x03
+        super().__init__(system, 0xFFFF, 0, 0, False, 0x00, 0x01)
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/deselect_rsp_header.py` & `secsgem-0.2.0a4/secsgem/hsms/deselect_rsp_header.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,16 +33,11 @@
         :type system: integer
 
         **Example**::
 
             >>> import secsgem.hsms
             >>>
             >>> secsgem.hsms.HsmsDeselectRspHeader(1)
-            HsmsDeselectRspHeader({sessionID:0xffff, stream:00, function:00, pType:0x00, sType:0x04, \
-system:0x00000001, requireResponse:False})
+            HsmsDeselectRspHeader({session_id:0xffff, stream:00, function:00, p_type:0x00, s_type:0x04, \
+system:0x00000001, require_response:False})
         """
-        HsmsHeader.__init__(self, system, 0xFFFF)
-        self.requireResponse = False
-        self.stream = 0x00
-        self.function = 0x00
-        self.pType = 0x00
-        self.sType = 0x04
+        super().__init__(system, 0xFFFF, 0, 0, False, 0x00, 0x04)
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/handler.py` & `secsgem-0.2.0a4/secsgem/hsms/protocol.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,31 +18,33 @@
 import queue
 import random
 import threading
 import typing
 
 import secsgem.common
 
-from .connection import HSMS_STYPES
+from .connection import HSMS_STYPES, HsmsConnection
 from .active_connection import HsmsActiveConnection
 from .passive_connection import HsmsPassiveConnection
 from .packet import HsmsPacket
 from .select_req_header import HsmsSelectReqHeader
 from .select_rsp_header import HsmsSelectRspHeader
 from .deselect_req_header import HsmsDeselectReqHeader
 from .deselect_rsp_header import HsmsDeselectRspHeader
 from .linktest_req_header import HsmsLinktestReqHeader
 from .linktest_rsp_header import HsmsLinktestRspHeader
 from .reject_req_header import HsmsRejectReqHeader
 from .separate_req_header import HsmsSeparateReqHeader
 from .stream_function_header import HsmsStreamFunctionHeader
 from .connectionstatemachine import ConnectionStateMachine
 
+from ..secs.functions.base import SecsStreamFunction
 
-class HsmsHandler:
+
+class HsmsProtocol(secsgem.common.Protocol):  # pylint: disable=too-many-instance-attributes
     """
     Baseclass for creating Host/Equipment models.
 
     This layer contains the HSMS functionality.
     Inherit from this class and override required functions.
     """
 
@@ -66,141 +68,144 @@
         **Example**::
 
             import secsgem.hsms
 
             def onConnect(event, data):
                 print "Connected"
 
-            client = secsgem.hsms.HsmsHandler("10.211.55.33", 5000, True, 0, "test")
+            client = secsgem.hsms.HsmsProtocol("10.211.55.33", 5000, True, 0, "test")
             client.events.hsms_connected += onConnect
 
             client.enable()
 
             time.sleep(3)
 
             client.disable()
 
         """
-        self._eventProducer = secsgem.common.EventProducer()
-        self._eventProducer.targets += self
-
-        self.logger = logging.getLogger(self.__module__ + "." + self.__class__.__name__)
-        self.communicationLogger = logging.getLogger("hsms_communication")
+        super().__init__()
 
-        self.address = address
-        self.port = port
-        self.active = active
-        self.sessionID = session_id
-        self.name = name
+        self._logger = logging.getLogger(self.__module__ + "." + self.__class__.__name__)
+        self._communication_logger = logging.getLogger("hsms_communication")
 
-        self.connected = False
+        self._address = address
+        self._port = port
+        self._active = active
+        self._session_id = session_id
+        self._name = name
 
-        self._secs_decode = None
+        self._connected = False
 
         # system id counter
-        self.systemCounter = random.randint(0, (2 ** 32) - 1)
+        self._system_counter = random.randint(0, (2 ** 32) - 1)
 
         # repeating linktest variables
-        self.linktestTimer = None
-        self.linktestTimeout = 30
+        self._linktest_timer = None
+        self._linktest_timeout = 30
 
         # select request thread for active connections, to avoid blocking state changes
-        self.selectReqThread = None
+        self._select_req_thread = None
 
         # response queues
-        self._systemQueues = {}
+        self._system_queues = {}
 
         # hsms connection state fsm
-        self.connectionState = ConnectionStateMachine({"on_enter_CONNECTED": self._on_state_connect,
-                                                       "on_exit_CONNECTED": self._on_state_disconnect,
-                                                       "on_enter_CONNECTED_SELECTED": self._on_state_select})
+        self._connection_state = ConnectionStateMachine({"on_enter_CONNECTED": self._on_state_connect,
+                                                         "on_exit_CONNECTED": self._on_state_disconnect,
+                                                         "on_enter_CONNECTED_SELECTED": self._on_state_select})
 
         # setup connection
-        if self.active:
+        if self._active:
             if custom_connection_handler is None:
-                self.connection = HsmsActiveConnection(self.address, self.port, self.sessionID, self)
+                self._connection = HsmsActiveConnection(self._address, self._port, self._session_id, self)
             else:
-                self.connection = custom_connection_handler.create_connection(self.address, self.port,
-                                                                              self.sessionID, self)
+                self._connection = custom_connection_handler.create_connection(self._address, self._port,
+                                                                               self._session_id, self)
         else:
             if custom_connection_handler is None:
-                self.connection = HsmsPassiveConnection(self.address, self.port, self.sessionID, self)
+                self._connection = HsmsPassiveConnection(self._address, self._port, self._session_id, self)
             else:
-                self.connection = custom_connection_handler.create_connection(self.address, self.port,
-                                                                              self.sessionID, self)
+                self._connection = custom_connection_handler.create_connection(self._address, self._port,
+                                                                               self._session_id, self)
+
+    @property
+    def timeouts(self) -> secsgem.common.Timeouts:
+        """Property for timeout."""
+        return self._connection.timeouts
 
     @property
-    def events(self):
-        """Property for event handling."""
-        return self._eventProducer
+    def name(self) -> str:
+        """Property for name."""
+        return self._name
 
     @property
-    def secs_decode(self) -> typing.Optional[typing.Callable[[HsmsPacket], typing.Any]]:
-        """Get secs decode."""
-        return self._secs_decode
-
-    @secs_decode.setter
-    def secs_decode(self, value: typing.Optional[typing.Callable[[HsmsPacket], typing.Any]]):
-        """Get secs decode."""
-        self._secs_decode = value
+    def connection(self) -> HsmsConnection:
+        """Property for connection."""
+        return self._connection
+
+    @property
+    def connection_state(self) -> HsmsConnection:
+        """Property for connection state."""
+        return self._connection_state
 
     def get_next_system_counter(self):
         """
         Return the next System.
 
         :returns: System for the next command
         :rtype: integer
         """
-        self.systemCounter += 1
+        self._system_counter += 1
 
-        if self.systemCounter > ((2 ** 32) - 1):
-            self.systemCounter = 0
+        if self._system_counter > ((2 ** 32) - 1):
+            self._system_counter = 0
 
-        return self.systemCounter
+        return self._system_counter
 
     def _send_select_req_thread(self):
         response = self.send_select_req()
         if response is None:
-            self.logger.warning("select request failed")
+            self._logger.warning("select request failed")
 
     def _start_linktest_timer(self):
-        self.linktestTimer = threading.Timer(self.linktestTimeout, self._on_linktest_timer)
-        self.linktestTimer.daemon = True  # kill thread automatically on main program termination
-        self.linktestTimer.name = "secsgem_hsmsHandler_linktestTimer"
-        self.linktestTimer.start()
+        self._linktest_timer = threading.Timer(self._linktest_timeout, self._on_linktest_timer)
+        self._linktest_timer.daemon = True  # kill thread automatically on main program termination
+        self._linktest_timer.name = "secsgem_hsmsProtocol_linktestTimer"
+        self._linktest_timer.start()
 
     def _on_state_connect(self):
         """
         Handle connection state model got event connect.
 
         :param data: event attributes
         :type data: object
         """
         # start linktest timer
         self._start_linktest_timer()
 
         # start select process if connection is active
-        if self.active:
-            self.selectReqThread = threading.Thread(target=self._send_select_req_thread,
-                                                    name="secsgem_hsmsHandler_sendSelectReqThread")
-            self.selectReqThread.daemon = True  # kill thread automatically on main program termination
-            self.selectReqThread.start()
+        if self._active:
+            self._select_req_thread = threading.Thread(
+                target=self._send_select_req_thread,
+                name="secsgem_hsmsProtocol_sendSelectReqThread")
+            self._select_req_thread.daemon = True  # kill thread automatically on main program termination
+            self._select_req_thread.start()
 
     def _on_state_disconnect(self):
         """
         Handle connection state model got event disconnect.
 
         :param data: event attributes
         :type data: object
         """
         # stop linktest timer
-        if self.linktestTimer:
-            self.linktestTimer.cancel()
+        if self._linktest_timer:
+            self._linktest_timer.cancel()
 
-        self.linktestTimer = None
+        self._linktest_timer = None
 
     def _on_state_select(self):
         """
         Handle connection state model got event select.
 
         :param data: event attributes
         :type data: object
@@ -214,260 +219,262 @@
         self.send_linktest_req()
 
         # restart the timer
         self._start_linktest_timer()
 
     def on_connection_established(self, _):
         """Handle connection was established event."""
-        self.connected = True
+        self._connected = True
 
         # update connection state
-        self.connectionState.connect()
+        self._connection_state.connect()
 
         self.events.fire("hsms_connected", {'connection': self})
 
     def on_connection_before_closed(self, _):
         """Handle connection is about to be closed event."""
         # send separate request
         self.send_separate_req()
 
     def on_connection_closed(self, _):
         """Handle connection was closed event."""
         # update connection state
-        self.connected = False
-        self.connectionState.disconnect()
+        self._connected = False
+        self._connection_state.disconnect()
 
         self.events.fire("hsms_disconnected", {'connection': self})
 
-    def __handle_hsms_requests(self, packet):
-        self.communicationLogger.info("< %s\n  %s", packet, HSMS_STYPES[packet.header.sType],
-                                      extra=self._get_log_extra())
+    def __handle_hsms_requests(self, packet):  # noqa: MC0001
+        self._communication_logger.info("< %s\n  %s", packet, HSMS_STYPES[packet.header.s_type],
+                                        extra=self._get_log_extra())
 
         # check if it is a select request
-        if packet.header.sType == 0x01:
+        if packet.header.s_type == 0x01:
             # if we are disconnecting send reject else send response
-            if self.connection.disconnecting:
-                self.send_reject_rsp(packet.header.system, packet.header.sType, 4)
+            if self._connection.disconnecting:
+                self.send_reject_rsp(packet.header.system, packet.header.s_type, 4)
             else:
                 self.send_select_rsp(packet.header.system)
 
                 # update connection state
-                self.connectionState.select()
+                self._connection_state.select()
 
         # check if it is a select response
-        elif packet.header.sType == 0x02:
+        elif packet.header.s_type == 0x02:
             # update connection state
-            self.connectionState.select()
+            self._connection_state.select()
 
-            if packet.header.system in self._systemQueues:
+            if packet.header.system in self._system_queues:
                 # send packet to request sender
-                self._systemQueues[packet.header.system].put_nowait(packet)
+                self._system_queues[packet.header.system].put_nowait(packet)
 
             # what to do if no sender for request waiting?
 
         # check if it is a deselect request
-        elif packet.header.sType == 0x03:
+        elif packet.header.s_type == 0x03:
             # if we are disconnecting send reject else send response
-            if self.connection.disconnecting:
-                self.send_reject_rsp(packet.header.system, packet.header.sType, 4)
+            if self._connection.disconnecting:
+                self.send_reject_rsp(packet.header.system, packet.header.s_type, 4)
             else:
                 self.send_deselect_rsp(packet.header.system)
                 # update connection state
-                self.connectionState.deselect()
+                self._connection_state.deselect()
 
         # check if it is a deselect response
-        elif packet.header.sType == 0x04:
+        elif packet.header.s_type == 0x04:
             # update connection state
-            self.connectionState.deselect()
+            self._connection_state.deselect()
 
-            if packet.header.system in self._systemQueues:
+            if packet.header.system in self._system_queues:
                 # send packet to request sender
-                self._systemQueues[packet.header.system].put_nowait(packet)
+                self._system_queues[packet.header.system].put_nowait(packet)
 
             # what to do if no sender for request waiting?
 
         # check if it is a linktest request
-        elif packet.header.sType == 0x05:
+        elif packet.header.s_type == 0x05:
             # if we are disconnecting send reject else send response
-            if self.connection.disconnecting:
-                self.send_reject_rsp(packet.header.system, packet.header.sType, 4)
+            if self._connection.disconnecting:
+                self.send_reject_rsp(packet.header.system, packet.header.s_type, 4)
             else:
                 self.send_linktest_rsp(packet.header.system)
 
         else:
-            if packet.header.system in self._systemQueues:
+            if packet.header.system in self._system_queues:
                 # send packet to request sender
-                self._systemQueues[packet.header.system].put_nowait(packet)
+                self._system_queues[packet.header.system].put_nowait(packet)
 
             # what to do if no sender for request waiting?
 
     def on_connection_packet_received(self, _, packet):
         """
         Packet received by connection.
 
         :param packet: received data packet
         :type packet: :class:`secsgem.hsms.HsmsPacket`
         """
-        if packet.header.sType > 0:
+        if packet.header.s_type > 0:
             self.__handle_hsms_requests(packet)
         else:
             if callable(self._secs_decode):
                 message = self._secs_decode(packet)
-                self.communicationLogger.info("< %s\n%s", packet, message, extra=self._get_log_extra())
+                self._communication_logger.info("< %s\n%s", packet, message, extra=self._get_log_extra())
             else:
-                self.communicationLogger.info("< %s", packet, extra=self._get_log_extra())
+                self._communication_logger.info("< %s", packet, extra=self._get_log_extra())
 
-            if not self.connectionState.is_CONNECTED_SELECTED():
-                self.logger.warning("received message when not selected")
+            if not self._connection_state.is_CONNECTED_SELECTED():
+                self._logger.warning("received message when not selected")
 
-                out_packet = HsmsPacket(HsmsRejectReqHeader(packet.header.system, packet.header.sType, 4))
-                self.communicationLogger.info("> %s\n  %s", out_packet, HSMS_STYPES[out_packet.header.sType],
-                                              extra=self._get_log_extra())
-                self.connection.send_packet(out_packet)
+                out_packet = HsmsPacket(HsmsRejectReqHeader(packet.header.system, packet.header.s_type, 4))
+                self._communication_logger.info(
+                    "> %s\n  %s", out_packet, HSMS_STYPES[out_packet.header.s_type],
+                    extra=self._get_log_extra())
+                self._connection.send_packet(out_packet)
 
                 return
 
             # someone is waiting for this message
-            if packet.header.system in self._systemQueues:
+            if packet.header.system in self._system_queues:
                 # send packet to request sender
-                self._systemQueues[packet.header.system].put_nowait(packet)
+                self._system_queues[packet.header.system].put_nowait(packet)
             # just log if nobody is interested
             else:
                 self.events.fire("hsms_packet_received", {'connection': self, 'packet': packet})
 
     def _get_queue_for_system(self, system_id):
         """
         Create a new queue to receive responses for a certain system.
 
         :param system_id: system id to watch
         :type system_id: int
         :returns: queue to receive responses with
         :rtype: queue.Queue
         """
-        self._systemQueues[system_id] = queue.Queue()
-        return self._systemQueues[system_id]
+        self._system_queues[system_id] = queue.Queue()
+        return self._system_queues[system_id]
 
     def _remove_queue(self, system_id):
         """
         Remove queue for system id from list.
 
         :param system_id: system id to remove
         :type system_id: int
         """
-        del self._systemQueues[system_id]
+        del self._system_queues[system_id]
 
     def __repr__(self):
         """Generate textual representation for an object of this class."""
-        return f"{self.__class__.__name__} {str(self._serialize_data())}"
+        return f"{self.__class__.__name__} {str(self.serialize_data())}"
 
-    def _serialize_data(self):
+    def serialize_data(self) -> typing.Dict[str, typing.Any]:
         """
         Return data for serialization.
 
         :returns: data to serialize for this object
         :rtype: dict
         """
-        return {'address': self.address, 'port': self.port, 'active': self.active, 'sessionID': self.sessionID,
-                'name': self.name, 'connected': self.connected}
+        return {'address': self._address, 'port': self._port, 'active': self._active, 'session_id': self._session_id,
+                'name': self._name, 'connected': self._connected}
 
     def enable(self):
         """Enable the connection."""
-        self.connection.enable()
+        self._connection.enable()
 
     def disable(self):
         """Disable the connection."""
-        self.connection.disable()
+        self._connection.disable()
 
-    def send_stream_function(self, packet):
+    def send_stream_function(self, function: SecsStreamFunction) -> bool:
         """
         Send the packet and wait for the response.
 
         :param packet: packet to be sent
         :type packet: :class:`secsgem.secs.functionbase.SecsStreamFunction`
         """
         out_packet = HsmsPacket(
-            HsmsStreamFunctionHeader(self.get_next_system_counter(), packet.stream, packet.function,
-                                     packet.is_reply_required, self.sessionID),
-            packet.encode())
+            HsmsStreamFunctionHeader(self.get_next_system_counter(), function.stream, function.function,
+                                     function.is_reply_required, self._session_id),
+            function.encode())
 
-        self.communicationLogger.info("> %s\n%s", out_packet, packet, extra=self._get_log_extra())
+        self._communication_logger.info("> %s\n%s", out_packet, function, extra=self._get_log_extra())
 
-        return self.connection.send_packet(out_packet)
+        return self._connection.send_packet(out_packet)
 
-    def send_and_waitfor_response(self, packet):
+    def send_and_waitfor_response(self, function: SecsStreamFunction) -> typing.Optional[secsgem.common.Packet]:
         """
         Send the packet and wait for the response.
 
         :param packet: packet to be sent
         :type packet: :class:`secsgem.secs.functionbase.SecsStreamFunction`
         :returns: Packet that was received
         :rtype: :class:`secsgem.hsms.HsmsPacket`
         """
         system_id = self.get_next_system_counter()
 
         response_queue = self._get_queue_for_system(system_id)
 
-        out_packet = HsmsPacket(HsmsStreamFunctionHeader(system_id, packet.stream, packet.function, True,
-                                                         self.sessionID),
-                                packet.encode())
+        out_packet = HsmsPacket(HsmsStreamFunctionHeader(system_id, function.stream, function.function, True,
+                                                         self._session_id),
+                                function.encode())
 
-        self.communicationLogger.info("> %s\n%s", out_packet, packet, extra=self._get_log_extra())
+        self._communication_logger.info("> %s\n%s", out_packet, function, extra=self._get_log_extra())
 
-        if not self.connection.send_packet(out_packet):
-            self.logger.error("Sending packet failed")
+        if not self._connection.send_packet(out_packet):
+            self._logger.error("Sending packet failed")
             self._remove_queue(system_id)
             return None
 
         try:
-            response = response_queue.get(True, self.connection.T3)
+            response = response_queue.get(True, self.timeouts.t3)
         except queue.Empty:
             response = None
 
         self._remove_queue(system_id)
 
         return response
 
-    def send_response(self, function, system):
+    def send_response(self, function: SecsStreamFunction, system: int) -> bool:
         """
         Send response function for system.
 
         :param function: function to be sent
         :type function: :class:`secsgem.secs.functionbase.SecsStreamFunction`
         :param system: system to reply to
         :type system: integer
         """
         out_packet = HsmsPacket(HsmsStreamFunctionHeader(system, function.stream, function.function, False,
-                                                         self.sessionID),
+                                                         self._session_id),
                                 function.encode())
 
-        self.communicationLogger.info("> %s\n%s", out_packet, function, extra=self._get_log_extra())
+        self._communication_logger.info("> %s\n%s", out_packet, function, extra=self._get_log_extra())
 
-        return self.connection.send_packet(out_packet)
+        return self._connection.send_packet(out_packet)
 
     def send_select_req(self):
         """
         Send a Select Request to the remote host.
 
         :returns: System of the sent request
         :rtype: integer
         """
         system_id = self.get_next_system_counter()
 
         response_queue = self._get_queue_for_system(system_id)
 
         packet = HsmsPacket(HsmsSelectReqHeader(system_id))
-        self.communicationLogger.info("> %s\n  %s", packet, HSMS_STYPES[packet.header.sType],
-                                      extra=self._get_log_extra())
+        self._communication_logger.info(
+            "> %s\n  %s", packet, HSMS_STYPES[packet.header.s_type],
+            extra=self._get_log_extra())
 
-        if not self.connection.send_packet(packet):
+        if not self._connection.send_packet(packet):
             self._remove_queue(system_id)
             return None
 
         try:
-            response = response_queue.get(True, self.connection.T6)
+            response = response_queue.get(True, self.timeouts.t6)
         except queue.Empty:
             response = None
 
         self._remove_queue(system_id)
 
         return response
 
@@ -475,39 +482,41 @@
         """
         Send a Select Response to the remote host.
 
         :param system_id: System of the request to reply for
         :type system_id: integer
         """
         packet = HsmsPacket(HsmsSelectRspHeader(system_id))
-        self.communicationLogger.info("> %s\n  %s", packet, HSMS_STYPES[packet.header.sType],
-                                      extra=self._get_log_extra())
-        return self.connection.send_packet(packet)
+        self._communication_logger.info(
+            "> %s\n  %s", packet, HSMS_STYPES[packet.header.s_type],
+            extra=self._get_log_extra())
+        return self._connection.send_packet(packet)
 
     def send_linktest_req(self):
         """
         Send a Linktest Request to the remote host.
 
         :returns: System of the sent request
         :rtype: integer
         """
         system_id = self.get_next_system_counter()
 
         response_queue = self._get_queue_for_system(system_id)
 
         packet = HsmsPacket(HsmsLinktestReqHeader(system_id))
-        self.communicationLogger.info("> %s\n  %s", packet, HSMS_STYPES[packet.header.sType],
-                                      extra=self._get_log_extra())
+        self._communication_logger.info(
+            "> %s\n  %s", packet, HSMS_STYPES[packet.header.s_type],
+            extra=self._get_log_extra())
 
-        if not self.connection.send_packet(packet):
+        if not self._connection.send_packet(packet):
             self._remove_queue(system_id)
             return None
 
         try:
-            response = response_queue.get(True, self.connection.T6)
+            response = response_queue.get(True, self.timeouts.t6)
         except queue.Empty:
             response = None
 
         self._remove_queue(system_id)
 
         return response
 
@@ -515,39 +524,40 @@
         """
         Send a Linktest Response to the remote host.
 
         :param system_id: System of the request to reply for
         :type system_id: integer
         """
         packet = HsmsPacket(HsmsLinktestRspHeader(system_id))
-        self.communicationLogger.info("> %s\n  %s", packet, HSMS_STYPES[packet.header.sType],
-                                      extra=self._get_log_extra())
-        return self.connection.send_packet(packet)
+        self._communication_logger.info(
+            "> %s\n  %s", packet, HSMS_STYPES[packet.header.s_type],
+            extra=self._get_log_extra())
+        return self._connection.send_packet(packet)
 
     def send_deselect_req(self):
         """
         Send a Deselect Request to the remote host.
 
         :returns: System of the sent request
         :rtype: integer
         """
         system_id = self.get_next_system_counter()
 
         response_queue = self._get_queue_for_system(system_id)
 
         packet = HsmsPacket(HsmsDeselectReqHeader(system_id))
-        self.communicationLogger.info("> %s\n  %s", packet, HSMS_STYPES[packet.header.sType],
-                                      extra=self._get_log_extra())
+        self._communication_logger.info("> %s\n  %s", packet, HSMS_STYPES[packet.header.s_type],
+                                        extra=self._get_log_extra())
 
-        if not self.connection.send_packet(packet):
+        if not self._connection.send_packet(packet):
             self._remove_queue(system_id)
             return None
 
         try:
-            response = response_queue.get(True, self.connection.T6)
+            response = response_queue.get(True, self.timeouts.t6)
         except queue.Empty:
             response = None
 
         self._remove_queue(system_id)
 
         return response
 
@@ -555,44 +565,47 @@
         """
         Send a Deselect Response to the remote host.
 
         :param system_id: System of the request to reply for
         :type system_id: integer
         """
         packet = HsmsPacket(HsmsDeselectRspHeader(system_id))
-        self.communicationLogger.info("> %s\n  %s", packet, HSMS_STYPES[packet.header.sType],
-                                      extra=self._get_log_extra())
-        return self.connection.send_packet(packet)
+        self._communication_logger.info(
+            "> %s\n  %s", packet, HSMS_STYPES[packet.header.s_type],
+            extra=self._get_log_extra())
+        return self._connection.send_packet(packet)
 
     def send_reject_rsp(self, system_id, s_type, reason):
         """
         Send a Reject Response to the remote host.
 
         :param system_id: System of the request to reply for
         :type system_id: integer
         :param s_type: s_type of rejected message
         :type s_type: integer
         :param reason: reason for rejection
         :type reason: integer
         """
         packet = HsmsPacket(HsmsRejectReqHeader(system_id, s_type, reason))
-        self.communicationLogger.info("> %s\n  %s", packet, HSMS_STYPES[packet.header.sType],
-                                      extra=self._get_log_extra())
-        return self.connection.send_packet(packet)
+        self._communication_logger.info(
+            "> %s\n  %s", packet, HSMS_STYPES[packet.header.s_type],
+            extra=self._get_log_extra())
+        return self._connection.send_packet(packet)
 
     def send_separate_req(self):
         """Send a Separate Request to the remote host."""
         system_id = self.get_next_system_counter()
 
         packet = HsmsPacket(HsmsSeparateReqHeader(system_id))
-        self.communicationLogger.info("> %s\n  %s", packet, HSMS_STYPES[packet.header.sType],
-                                      extra=self._get_log_extra())
+        self._communication_logger.info(
+            "> %s\n  %s", packet, HSMS_STYPES[packet.header.s_type],
+            extra=self._get_log_extra())
 
-        if not self.connection.send_packet(packet):
+        if not self._connection.send_packet(packet):
             return None
 
         return system_id
 
     # helpers
 
     def _get_log_extra(self):
-        return {"address": self.address, "port": self.port, "sessionID": self.sessionID, "remoteName": self.name}
+        return {"address": self._address, "port": self._port, "session_id": self._session_id, "remoteName": self._name}
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/header.py` & `secsgem-0.2.0a4/secsgem/hsms/header.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,61 +13,93 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Header for the hsms packets."""
 
 import struct
 
+import secsgem.common
 
-class HsmsHeader:
+
+class HsmsHeader(secsgem.common.Header):
     """
     Generic HSMS header.
 
     Base for different specific headers
     """
 
-    def __init__(self, system, session_id):
+    def __init__(
+            self, 
+            system: int, 
+            session_id: int, 
+            stream: int = 0, 
+            function: int = 0,
+            requires_response: bool = False,
+            p_type: int = 0x00,
+            s_type: int = 0x01):
         """
         Initialize a hsms header.
 
         :param system: message ID
         :type system: integer
         :param session_id: device / session ID
         :type session_id: integer
+        :param stream: stream
+        :type stream: integer
+        :param function: function
+        :type function: integer
+        :param requires_response: is response required
+        :type requires_response: bool
+        :param p_type: P-Type
+        :type p_type: integer
+        :param s_type: S-Type
+        :type s_type: integer
 
         **Example**::
 
             >>> import secsgem.hsms
             >>>
             >>> secsgem.hsms.HsmsHeader(3, 100)
-            HsmsHeader({sessionID:0x0064, stream:00, function:00, pType:0x00, sType:0x01, system:0x00000003, \
-requireResponse:False})
+            HsmsHeader({session_id:0x0064, stream:00, function:00, p_type:0x00, s_type:0x01, system:0x00000003, \
+require_response:False})
         """
-        self.sessionID = session_id
-        self.requireResponse = False
-        self.stream = 0x00
-        self.function = 0x00
-        self.pType = 0x00
-        self.sType = 0x01
-        self.system = system
+        super().__init__(system, session_id, stream, function)
+        self._require_response = requires_response
+        self._p_type = p_type
+        self._s_type = s_type
 
     def __str__(self):
         """Generate string representation for an object of this class."""
-        return f'{{sessionID:0x{self.sessionID:04x}, ' \
+        return f'{{session_id:0x{self.session_id:04x}, ' \
                f'stream:{self.stream:02d}, ' \
                f'function:{self.function:02d}, ' \
-               f'pType:0x{self.pType:02x}, ' \
-               f'sType:0x{self.sType:02x}, ' \
+               f'p_type:0x{self.p_type:02x}, ' \
+               f's_type:0x{self.s_type:02x}, ' \
                f'system:0x{self.system:08x}, ' \
-               f'requireResponse:{self.requireResponse!r}}}'
+               f'require_response:{self.require_response!r}}}'
 
     def __repr__(self):
         """Generate textual representation for an object of this class."""
         return f"{self.__class__.__name__}({self.__str__()})"
 
+    @property
+    def require_response(self) -> bool:
+        """Get require response flag."""
+        return self._require_response
+
+    @property
+    def p_type(self) -> int:
+        """Get P-type."""
+        return self._p_type
+
+    @property
+    def s_type(self) -> int:
+        """Get S-type."""
+        return self._s_type
+
     def encode(self):
         """
         Encode header to hsms packet.
 
         :returns: encoded header
         :rtype: string
 
@@ -78,11 +110,19 @@
             >>>
             >>> header = secsgem.hsms.HsmsLinktestReqHeader(2)
             >>> secsgem.common.format_hex(header.encode())
             'ff:ff:00:00:00:05:00:00:00:02'
 
         """
         header_stream = self.stream
-        if self.requireResponse:
+        if self.require_response:
             header_stream |= 0b10000000
 
-        return struct.pack(">HBBBBL", self.sessionID, header_stream, self.function, self.pType, self.sType, self.system)
+        return struct.pack(
+            ">HBBBBL",
+            self.session_id,
+            header_stream,
+            self.function,
+            self.p_type,
+            self.s_type,
+            self.system
+        )
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/linktest_req_header.py` & `secsgem-0.2.0a4/secsgem/hsms/deselect_req_header.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 #####################################################################
-# linktest_req_header.py
+# deselect_req_header.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Header for the hsms linktest request."""
+"""Header for the hsms deselect request."""
 
 from .header import HsmsHeader
 
 
-class HsmsLinktestReqHeader(HsmsHeader):
+class HsmsDeselectReqHeader(HsmsHeader):
     """
-    Header for Linktest Request.
+    Header for Deselect Request.
 
-    Header for message with SType 5.
+    Header for message with SType 3.
     """
 
     def __init__(self, system):
         """
-        Initialize a hsms linktest request.
+        Initialize a hsms deselect request.
 
         :param system: message ID
         :type system: integer
 
         **Example**::
 
             >>> import secsgem.hsms
             >>>
-            >>> secsgem.hsms.HsmsLinktestReqHeader(2)
-            HsmsLinktestReqHeader({sessionID:0xffff, stream:00, function:00, pType:0x00, sType:0x05, \
-system:0x00000002, requireResponse:False})
+            >>> secsgem.hsms.HsmsDeselectReqHeader(1)
+            HsmsDeselectReqHeader({session_id:0xffff, stream:00, function:00, p_type:0x00, s_type:0x03, \
+system:0x00000001, require_response:False})
         """
-        HsmsHeader.__init__(self, system, 0xFFFF)
-        self.requireResponse = False
-        self.stream = 0x00
-        self.function = 0x00
-        self.pType = 0x00
-        self.sType = 0x05
+        super().__init__(system, 0xFFFF, 0, 0, False, 0x00, 0x03)
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/linktest_rsp_header.py` & `secsgem-0.2.0a4/secsgem/hsms/linktest_rsp_header.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,16 +33,11 @@
         :type system: integer
 
         **Example**::
 
             >>> import secsgem.hsms
             >>>
             >>> secsgem.hsms.HsmsLinktestRspHeader(10)
-            HsmsLinktestRspHeader({sessionID:0xffff, stream:00, function:00, pType:0x00, sType:0x06, \
-system:0x0000000a, requireResponse:False})
+            HsmsLinktestRspHeader({session_id:0xffff, stream:00, function:00, p_type:0x00, s_type:0x06, \
+system:0x0000000a, require_response:False})
         """
-        HsmsHeader.__init__(self, system, 0xFFFF)
-        self.requireResponse = False
-        self.stream = 0x00
-        self.function = 0x00
-        self.pType = 0x00
-        self.sType = 0x06
+        super().__init__(system, 0xFFFF, 0, 0, False, 0x00, 0x06)
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/multi_passive_connection.py` & `secsgem-0.2.0a4/secsgem/hsms/multi_passive_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,19 +59,19 @@
         :type sock: :class:`Socket`
         :param address: IP address of remote host
         :type address: string
         """
         del address  # unused parameter
 
         # setup socket
-        self.sock = sock
-        self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
+        self._sock = sock
+        self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
 
         # make socket nonblocking
-        self.sock.setblocking(0)
+        self._sock.setblocking(0)
 
         # start the receiver thread
         self._start_receiver()
 
     def enable(self):
         """
         Enable the connection.
@@ -83,9 +83,9 @@
     def disable(self):
         """
         Disable the connection.
 
         Stops all connection attempts, and closes the connection
         """
         self.enabled = False
-        if self.connected:
+        if self._connected:
             self.disconnect()
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/multi_passive_server.py` & `secsgem-0.2.0a4/secsgem/secs/functions/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,206 +1,210 @@
 #####################################################################
-# multi_passive_server.py
+# base.py
 #
-# (c) Copyright 2021, Benjamin Parzella. All rights reserved.
+# (c) Copyright 2015-2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Hsms multi passive server."""
-
-import logging
-import select
-import socket
-import threading
+"""Base class for for SECS stream and functions."""
+import typing
 
 import secsgem.common
+from ..data_items import DataItemBase
+from ..variables import functions
+
+DataItemRecursive = typing.Union[typing.Type[DataItemBase], typing.Iterable["DataItemRecursive"]]
+
+
+class StructureDisplayingMeta(type):
+    """Meta class overriding the default __repr__ of a class."""
 
-from .multi_passive_connection import HsmsMultiPassiveConnection
+    def __repr__(cls):
+        """Generate textual representation for an object of this class."""
+        return cls.get_format()
 
 
-class HsmsMultiPassiveServer:  # pragma: no cover
+class SecsStreamFunction(metaclass=StructureDisplayingMeta):  # pylint: disable=too-many-instance-attributes
     """
-    Server class for multiple passive (incoming) connection.
+    Secs stream and function base class.
 
-    The server creates a listening socket and waits for incoming connections on this socket.
+    This class is inherited to create a stream/function class.
+    To create a function specific content the class variables :attr:`_stream`, :attr:`_function`
+    and :attr:`_data_format` must be overridden.
     """
 
-    select_timeout = 0.5
-    """ Timeout for select calls ."""
+    _stream = 0
+    _function = 0
 
-    def __init__(self, port=5000, bind_ip=''):
-        """
-        Initialize a passive hsms server.
+    _data_format: typing.Optional[DataItemRecursive] = None
 
-        :param port: TCP port to listen on
-        :type port: integer
+    _to_host = True
+    _to_equipment = True
 
-        **Example**::
+    _has_reply = False
+    _is_reply_required = False
 
-            # TODO: create example
+    _is_multi_block = False
 
+    def __init__(self, value=None):
         """
-        self.logger = logging.getLogger(self.__module__ + "." + self.__class__.__name__)
+        Initialize a stream function object.
 
-        self.listenSock = None
+        **Example**::
 
-        self.port = port
-        self.bind_ip = bind_ip
+            class SecsS02F30(SecsStreamFunction):
+                _stream = 2
+                _function = 30
 
-        self.threadRunning = False
-        self.stopThread = False
+                _to_host = True
+                _to_equipment = False
 
-        self.connections = {}
+                _has_reply = False
+                _is_reply_required = False
 
-        self.listenThread = None
+                _is_multi_block = True
 
-    def create_connection(self, address, port=5000, session_id=0, delegate=None):
-        """
-        Create and remember connection for the server.
+                _data_format = [
+                    [
+                        ECID,
+                        ECNAME,
+                        ECMIN,
+                        ECMAX,
+                        ECDEF,
+                        UNITS
+                    ]
+                ]
 
-        :param address: IP address of target host
-        :type address: string
-        :param port: TCP port of target host
-        :type port: integer
-        :param session_id: session / device ID to use for connection
-        :type session_id: integer
-        :param delegate: target for messages
-        :type delegate: object
+        :param value: set the value of stream/function parameters
+        :type value: various
         """
-        connection = HsmsMultiPassiveConnection(address, port, session_id, delegate)
-        connection.handler = self
+        self.data = functions.generate(self._data_format)
 
-        self.connections[address] = connection
+        # copy public members from private ones
+        self.stream = self._stream
+        self.function = self._function
 
-        return connection
+        self.data_format = self._data_format
+        self.to_host = self._to_host
+        self.to_equipment = self._to_equipment
 
-    def start(self):
-        """
-        Start the server and return.
-
-        It will launch a listener running in background to wait for incoming connections.
-        """
-        self.listenSock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-
-        if not secsgem.common.is_windows():
-            self.listenSock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        self.has_reply = self._has_reply
+        self.is_reply_required = self._is_reply_required
 
-        self.listenSock.bind((self.bind_ip, self.port))
-        self.listenSock.listen(1)
-        self.listenSock.setblocking(0)
+        self.is_multi_block = self._is_multi_block
 
-        self.listenThread = threading.Thread(target=self._listen_thread, args=(),
-                                             name=f"secsgem_hsmsMultiPassiveServer_listenThread_{self.port}")
-        self.listenThread.start()
+        if value is not None and self.data is not None:
+            self.data.set(value)
 
-        self.logger.debug("listening")
+        self._object_intitialized = True
 
-    def stop(self, terminate_connections=True):
-        """
-        Stop the server. The background job waiting for incoming connections will be terminated.
+    def __repr__(self):
+        """Generate textual representation for an object of this class."""
+        function = f"S{self.stream}F{self.function}"
+        if self.data is None:
+            return f"{function}{' W' if self._is_reply_required else ''} ."
+        data = f"{self.data}"
 
-        Optionally all connections received will be closed.
+        return f"{function}{' W' if self._is_reply_required else ''}\n{secsgem.common.indent_block(data)} ."
 
-        :param terminate_connections: terminate all connection made by this server
-        :type terminate_connections: boolean
-        """
-        self.stopThread = True
+    def __getitem__(self, key):
+        """Get an item using the indexer operator."""
+        return self.data[key]
 
-        if self.listenThread.is_alive():
-            while self.threadRunning:
-                pass
+    def __setitem__(self, key, item):
+        """Set an item using the indexer operator."""
+        self.data[key] = item
 
-        self.listenSock.close()
+    def __len__(self):
+        """Get the length."""
+        return len(self.data)
 
-        self.stopThread = False
+    def __getattr__(self, item):
+        """Get an item as object member."""
+        return self.data.__getattr__(item)
 
-        if terminate_connections:
-            for connection in self.connections.values():
-                connection.disconnect()
+    def __setattr__(self, item, value):
+        """Set an item as object member."""
+        if '_object_intitialized' not in self.__dict__:
+            dict.__setattr__(self, item, value)
+            return
 
-        self.logger.debug("server stopped")
+        if item in self.data.data:
+            self.data.__setattr__(item, value)
+            return
 
-    def _initialize_connection_thread(self, accept_result):
+    def append(self, data):
         """
-        Set connection up.
+        Append data to list, if stream/function parameter is a list.
 
-        .. warning:: Do not call this directly, used internally.
+        :param data: list item to add
+        :type data: various
         """
-        (sock, (source_ip, _)) = accept_result
-
-        sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
-
-        new_connection = None
-
-        # check if connection available with source ip
-        if source_ip not in self.connections:
-            named_connection_found = False
-
-            # check all connections if connection with hostname can be resolved
-            for connection in self.connections.values():
-                try:
-                    if source_ip == socket.gethostbyname(connection.remoteAddress):
-                        new_connection = connection
-                        named_connection_found = True
-                        break
-                except socket.gaierror:
-                    pass
-
-            if not named_connection_found:
-                sock.close()
-                return
+        if hasattr(self.data, 'append') and callable(self.data.append):
+            self.data.append(data)
         else:
-            new_connection = self.connections[source_ip]
+            raise AttributeError(
+                f"class {self.__class__.__name__} has no attribute 'append'")
 
-        if not new_connection.enabled:
-            sock.close()
-            return
+    def encode(self):
+        """
+        Generate the encoded hsms data of the stream/function parameter.
 
-        new_connection.on_connected(sock, source_ip)
+        :returns: encoded data
+        :rtype: string
+        """
+        if self.data is None:
+            return b""
 
-    def _listen_thread(self):
+        return self.data.encode()
+
+    def decode(self, data):
         """
-        Thread listening for incoming connections.
+        Update stream/function parameter data from the passed data.
 
-        .. warning:: Do not call this directly, used internally.
+        :param data: encoded data
+        :type data: string
         """
-        self.threadRunning = True
-        try:
-            while not self.stopThread:
-                # check for data in the input buffer
-                select_result = select.select([self.listenSock], [], [self.listenSock], self.select_timeout)
+        if self.data is not None:
+            self.data.decode(data)
 
-                if select_result[0]:
-                    accept_result = None
+    def set(self, value):
+        """
+        Update the value of the stream/function parameter.
 
-                    try:
-                        accept_result = self.listenSock.accept()
-                    except OSError as exc:
-                        if not secsgem.common.is_errorcode_ewouldblock(exc.errno):
-                            raise exc
+        :param value: new value for the parameter
+        :type value: various
+        """
+        self.data.set(value)
 
-                    if accept_result is None:
-                        continue
+    def get(self):
+        """
+        Get the current value of the stream/function parameter.
 
-                    if self.stopThread:
-                        continue
+        :returns: current parameter value
+        :rtype: various
+        """
+        if self.data is None:
+            return None
 
-                    self.logger.debug("connection from %s:%d", accept_result[1][0], accept_result[1][1])
+        return self.data.get()
 
-                    threading.Thread(
-                        target=self._initialize_connection_thread, args=(accept_result,),
-                        name=f"secsgem_hsmsMultiPassiveServer_InitializeConnectionThread_"
-                             f"{accept_result[1][0]}:{accept_result[1][1]}"
-                    ).start()
+    @classmethod
+    def get_format(cls):
+        """
+        Get the format of the function.
 
-        except Exception:  # pylint: disable=broad-except
-            self.logger.exception('exception')
+        :returns: returns the string representation of the function
+        :rtype: string
+        """
+        if cls._data_format is not None:
+            return functions.get_format(cls._data_format)
 
-        self.threadRunning = False
+        return "Header only"
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/packet.py` & `secsgem-0.2.0a4/secsgem/hsms/packet.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,62 +10,68 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Contains hsms packet class."""
+from __future__ import annotations
 
 import struct
+import typing
+
+import secsgem.common
 
 from .header import HsmsHeader
 
 
-class HsmsPacket:
+class HsmsPacket(secsgem.common.Packet):
     """
     Class for hsms packet.
 
     Contains all required data and functions.
     """
 
-    def __init__(self, header=None, data=b""):
+    def __init__(self, header: typing.Optional[HsmsHeader] = None, data: bytes = b""):
         """
         Initialize a hsms packet.
 
         :param header: header used for this packet
         :type header: :class:`secsgem.hsms.HsmsHeader` and derived
         :param data: data part used for streams and functions (SType 0)
         :type data: string
 
         **Example**::
 
             >>> import secsgem.hsms
             >>>
             >>> secsgem.hsms.HsmsPacket(secsgem.hsms.HsmsLinktestReqHeader(2))
-            HsmsPacket({'header': HsmsLinktestReqHeader({sessionID:0xffff, stream:00, function:00, pType:0x00, \
-sType:0x05, system:0x00000002, requireResponse:False}), 'data': ''})
+            HsmsPacket({'header': HsmsLinktestReqHeader({session_id:0xffff, stream:00, function:00, p_type:0x00, \
+s_type:0x05, system:0x00000002, require_response:False}), 'data': ''})
         """
-        if header is None:
-            self.header = HsmsHeader(0, 0)
-        else:
-            self.header = header
+        self._header = HsmsHeader(0, 0) if header is None else header
 
         self.data = data
 
-    def __str__(self):
+    @property
+    def header(self) -> HsmsHeader:
+        """Get the header."""
+        return self._header
+
+    def __str__(self) -> str:
         """Generate string representation for an object of this class."""
         data = "'header': " + self.header.__str__()
         return data
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """Generate textual representation for an object of this class."""
         return f"{self.__class__.__name__}" \
                f"({{'header': {self.header.__repr__()}, 'data': '{self.data.decode('utf-8')}'}})"
 
-    def encode(self):
+    def encode(self) -> bytes:
         """
         Encode packet data to hsms packet.
 
         :returns: encoded packet
         :rtype: string
 
         **Example**::
@@ -81,15 +87,15 @@
         headerdata = self.header.encode()
 
         length = len(headerdata) + len(self.data)
 
         return struct.pack(">L", length) + headerdata + self.data
 
     @staticmethod
-    def decode(text):
+    def decode(text: bytes) -> HsmsPacket:
         r"""
         Decode byte array hsms packet to HsmsPacket object.
 
         :returns: received packet object
         :rtype: :class:`secsgem.hsms.HsmsPacket`
 
         **Example**::
@@ -99,23 +105,25 @@
             >>>
             >>> packetData = b"\x00\x00\x00\x0b\xff\xff\x00\x00\x00\x05\x00\x00\x00\x02"
             >>>
             >>> secsgem.common.format_hex(packetData)
             '00:00:00:0b:ff:ff:00:00:00:05:00:00:00:02'
             >>>
             >>> secsgem.hsms.HsmsPacket.decode(packetData)
-            HsmsPacket({'header': HsmsHeader({sessionID:0xffff, stream:00, function:00, pType:0x00, sType:0x05, system:0x00000002, requireResponse:False}), 'data': ''})
+            HsmsPacket({'header': HsmsHeader({session_id:0xffff, stream:00, function:00, p_type:0x00, s_type:0x05, system:0x00000002, require_response:False}), 'data': ''})
         """   # noqa pylint: disable=line-too-long
         data_length = len(text) - 14
         data_length_text = str(data_length) + "s"
 
         res = struct.unpack(">LHBBBBL" + data_length_text, text)
 
-        result = HsmsPacket(HsmsHeader(res[6], res[1]))
-        result.header.requireResponse = (((res[2] & 0b10000000) >> 7) == 1)
-        result.header.stream = res[2] & 0b01111111
-        result.header.function = res[3]
-        result.header.pType = res[4]
-        result.header.sType = res[5]
-        result.data = res[7]
+        result = HsmsPacket(HsmsHeader(
+            res[6], 
+            res[1],
+            res[2] & 0b01111111,
+            res[3],
+            (((res[2] & 0b10000000) >> 7) == 1),
+            res[4],
+            res[5]
+        ), res[7])
 
         return result
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/passive_connection.py` & `secsgem-0.2.0a4/secsgem/hsms/passive_connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,112 +52,113 @@
 
         """
         # initialize super class
         HsmsConnection.__init__(self, True, address, port, session_id, delegate)
         self._bind_ip = bind_ip
 
         # initially not enabled
-        self.enabled = False
+        self._enabled = False
 
         # reconnect thread required for passive connection
-        self.serverThread = None
-        self.stopServerThread = False
-        self.serverSock = None
+        self._server_thread = None
+        self._stop_server_thread = False
+        self._server_sock = None
 
     def _on_hsms_connection_close(self, data):
         """
         Signal from super that the connection was closed.
 
         This is required to initiate the reconnect if the connection is still enabled
         """
-        if self.enabled:
+        if self._enabled:
             self.__start_server_thread()
 
     def enable(self):
         """
         Enable the connection.
 
         Starts the connection process to the passive remote.
         """
         # only start if not already enabled
-        if not self.enabled:
+        if not self._enabled:
             # mark connection as enabled
-            self.enabled = True
+            self._enabled = True
 
             # start the connection thread
             self.__start_server_thread()
 
     def disable(self):
         """
         Disable the connection.
 
         Stops all connection attempts, and closes the connection
         """
         # only stop if enabled
-        if self.enabled:
+        if self._enabled:
             # mark connection as disabled
-            self.enabled = False
+            self._enabled = False
 
             # stop connection thread if it is running
-            if self.serverThread and self.serverThread.is_alive():
-                self.stopServerThread = True
+            if self._server_thread and self._server_thread.is_alive():
+                self._stop_server_thread = True
 
-                if self.serverSock:
-                    self.serverSock.close()
+                if self._server_sock:
+                    self._server_sock.close()
 
                 # wait for connection thread to stop
-                while self.stopServerThread:
+                while self._stop_server_thread:
                     time.sleep(0.2)
 
             # disconnect super class
             self.disconnect()
 
     def __start_server_thread(self):
-        self.serverThread = threading.Thread(target=self.__server_thread,
-                                             name=f"secsgem_HsmsPassiveConnection_serverThread_{self.remoteAddress}")
-        self.serverThread.start()
+        self._server_thread = threading.Thread(
+            target=self.__server_thread,
+            name=f"secsgem_HsmsPassiveConnection_serverThread_{self._remote_address}")
+        self._server_thread.start()
 
     def __server_thread(self):
         """
         Thread function to (re)connect active connection to remote host.
 
         .. warning:: Do not call this directly, for internal use only.
         """
-        self.serverSock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self._server_sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
         if not secsgem.common.is_windows():
-            self.serverSock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            self._server_sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
-        self.serverSock.bind((self._bind_ip, self.remotePort))
-        self.serverSock.listen(1)
+        self._server_sock.bind((self._bind_ip, self._remote_port))
+        self._server_sock.listen(1)
 
-        while not self.stopServerThread:
+        while not self._stop_server_thread:
             try:
-                select_result = select.select([self.serverSock], [], [], self.select_timeout)
+                select_result = select.select([self._server_sock], [], [], self.select_timeout)
             except Exception:  # pylint: disable=broad-except
                 continue
 
             if not select_result[0]:
                 # select timed out
                 continue
 
-            accept_result = self.serverSock.accept()
+            accept_result = self._server_sock.accept()
             if accept_result is None:
                 continue
 
-            (self.sock, (_, _)) = accept_result
+            (self._sock, (_, _)) = accept_result
 
             # setup socket
-            self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
+            self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
 
             # make socket nonblocking
-            self.sock.setblocking(0)
+            self._sock.setblocking(0)
 
             # start the receiver thread
             self._start_receiver()
 
-            self.serverSock.shutdown(socket.SHUT_RDWR)
-            self.serverSock.close()
+            self._server_sock.shutdown(socket.SHUT_RDWR)
+            self._server_sock.close()
 
             return
 
-        self.stopServerThread = False
+        self._stop_server_thread = False
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/reject_req_header.py` & `secsgem-0.2.0a4/secsgem/hsms/reject_req_header.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,26 +27,21 @@
 
     def __init__(self, system, s_type, reason):
         """
         Initialize a hsms reject request.
 
         :param system: message ID
         :type system: integer
-        :param s_type: sType of rejected message
+        :param s_type: s_type of rejected message
         :type s_type: integer
         :param reason: reason for rejection
         :type reason: integer
 
         **Example**::
 
             >>> import secsgem.hsms
             >>>
             >>> secsgem.hsms.HsmsRejectReqHeader(17, 3, 4)
-            HsmsRejectReqHeader({sessionID:0xffff, stream:03, function:04, pType:0x00, sType:0x07, system:0x00000011, \
-requireResponse:False})
+            HsmsRejectReqHeader({session_id:0xffff, stream:03, function:04, p_type:0x00, s_type:0x07, \
+system:0x00000011, require_response:False})
         """
-        HsmsHeader.__init__(self, system, 0xFFFF)
-        self.requireResponse = False
-        self.stream = s_type
-        self.function = reason
-        self.pType = 0x00
-        self.sType = 0x07
+        super().__init__(system, 0xFFFF, s_type, reason, False, 0x00, 0x07)
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/select_req_header.py` & `secsgem-0.2.0a4/secsgem/hsms/select_rsp_header.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 #####################################################################
-# select_req_header.py
+# select_rsp_header.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Header for the hsms select request."""
+"""Header for the hsms select response."""
 
 from .header import HsmsHeader
 
 
-class HsmsSelectReqHeader(HsmsHeader):
+class HsmsSelectRspHeader(HsmsHeader):
     """
-    Header for Select Request.
+    Header for Select Response.
 
-    Header for message with SType 1.
+    Header for message with SType 2.
     """
 
     def __init__(self, system):
         """
-        Initialize a hsms select request.
+        Initialize a hsms select response.
 
         :param system: message ID
         :type system: integer
 
         **Example**::
 
             >>> import secsgem.hsms
             >>>
-            >>> secsgem.hsms.HsmsSelectReqHeader(14)
-            HsmsSelectReqHeader({sessionID:0xffff, stream:00, function:00, pType:0x00, sType:0x01, system:0x0000000e, \
-requireResponse:False})
+            >>> secsgem.hsms.HsmsSelectRspHeader(24)
+            HsmsSelectRspHeader({session_id:0xffff, stream:00, function:00, p_type:0x00, s_type:0x02, \
+system:0x00000018, require_response:False})
         """
-        HsmsHeader.__init__(self, system, 0xFFFF)
-        self.requireResponse = False
-        self.stream = 0x00
-        self.function = 0x00
-        self.pType = 0x00
-        self.sType = 0x01
+        super().__init__(system, 0xFFFF, 0, 0, False, 0x00, 0x02)
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/select_rsp_header.py` & `secsgem-0.2.0a4/secsgem/hsms/separate_req_header.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 #####################################################################
-# select_rsp_header.py
+# separate_req_header.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Header for the hsms select response."""
+"""Header for the hsms separate request."""
 
 from .header import HsmsHeader
 
 
-class HsmsSelectRspHeader(HsmsHeader):
+class HsmsSeparateReqHeader(HsmsHeader):
     """
-    Header for Select Response.
+    Header for Separate Request.
 
-    Header for message with SType 2.
+    Header for message with SType 9.
     """
 
     def __init__(self, system):
         """
-        Initialize a hsms select response.
+        Initialize a hsms separate request header.
 
         :param system: message ID
         :type system: integer
 
         **Example**::
 
             >>> import secsgem.hsms
             >>>
-            >>> secsgem.hsms.HsmsSelectRspHeader(24)
-            HsmsSelectRspHeader({sessionID:0xffff, stream:00, function:00, pType:0x00, sType:0x02, system:0x00000018, \
-requireResponse:False})
+            >>> secsgem.hsms.HsmsSeparateReqHeader(17)
+            HsmsSeparateReqHeader({session_id:0xffff, stream:00, function:00, p_type:0x00, s_type:0x09, \
+system:0x00000011, require_response:False})
         """
-        HsmsHeader.__init__(self, system, 0xFFFF)
-        self.requireResponse = False
-        self.stream = 0x00
-        self.function = 0x00
-        self.pType = 0x00
-        self.sType = 0x02
+        super().__init__(system, 0xFFFF, 0, 0, False, 0x00, 0x09)
```

### Comparing `secsgem-0.2.0a3/secsgem/hsms/stream_function_header.py` & `secsgem-0.2.0a4/secsgem/hsms/stream_function_header.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class HsmsStreamFunctionHeader(HsmsHeader):
     """
     Header for SECS message.
 
     Header for message with SType 0.
     """
 
-    def __init__(self, system, stream, function, require_response, session_id):
+    def __init__(self, system: int, stream: int, function: int, require_response: bool, session_id: int):
         """
         Initialize a stream function secs header.
 
         :param system: message ID
         :type system: integer
         :param stream: messages stream
         :type stream: integer
@@ -41,18 +41,11 @@
         :type session_id: integer
 
         **Example**::
 
             >>> import secsgem.hsms
             >>>
             >>> secsgem.hsms.HsmsStreamFunctionHeader(22, 1, 1, True, 100)
-            HsmsStreamFunctionHeader({sessionID:0x0064, stream:01, function:01, pType:0x00, sType:0x00, \
-system:0x00000016, requireResponse:True})
+            HsmsStreamFunctionHeader({session_id:0x0064, stream:01, function:01, p_type:0x00, s_type:0x00, \
+system:0x00000016, require_response:True})
         """
-        HsmsHeader.__init__(self, system, session_id)
-        self.sessionID = session_id
-        self.requireResponse = require_response
-        self.stream = stream
-        self.function = function
-        self.pType = 0x00
-        self.sType = 0x00
-        self.system = system
+        super().__init__(system, session_id, stream, function, require_response, 0x00, 0x00)
```

### Comparing `secsgem-0.2.0a3/secsgem/secs/__init__.py` & `secsgem-0.2.0a4/secsgem/secs/__init__.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/__init__.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/__init__.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/abs.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/abs.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/acka.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/acka.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ackc10.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ackc10.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ackc5.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ackc5.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ackc6.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ackc6.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ackc7.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ackc7.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/alcd.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/alcd.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/aled.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/aled.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/alid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/alid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/altx.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/altx.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/attrdata.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/attrdata.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/attrid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/attrid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/attrreln.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/attrreln.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/base.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from .. import variables
 
 
 class DataItemMeta(type):
     """Meta class for data items."""
 
-    def __new__(mcs, name, bases, attrs):
+    def __new__(mcs, name, bases, attrs):  # noqa: N804
+        """Meta class creation."""
         if name != "DataItemBase":
             bases += (attrs["__type__"], )
         return type.__new__(mcs, name, bases, attrs)
 
 
 class DataItemBase(metaclass=DataItemMeta):
     """
```

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/bcequ.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/bcequ.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/binlt.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/binlt.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ceed.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ceed.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ceid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ceid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/cename.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/cename.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/cepack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/cepack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/cepval.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/cepval.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/cmda.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/cmda.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/colct.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/colct.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/commack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/commack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/cpack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/cpack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/cpname.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/cpname.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/cpval.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/cpval.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/dataid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/dataid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/datalength.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/datalength.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/datlc.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/datlc.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/drack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/drack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/dsid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/dsid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/dsper.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/dsper.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/dutms.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/dutms.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/dvname.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/dvname.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/dvval.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/dvval.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/dvvalname.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/dvvalname.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/eac.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/eac.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ecdef.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ecdef.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ecid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ecid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ecmax.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ecmax.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ecmin.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ecmin.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ecname.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ecname.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ecv.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ecv.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/edid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/edid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/erack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/erack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/errcode.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/errcode.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/errtext.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/errtext.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/exid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/exid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/exmessage.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/exmessage.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/exrecvra.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/exrecvra.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/extype.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/extype.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/fcnid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/fcnid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ffrot.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ffrot.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/fnloc.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/fnloc.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/grant6.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/grant6.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/grnt1.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/grnt1.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/hcack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/hcack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/idtyp.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/idtyp.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/length.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/length.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/limitack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/limitack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/limitid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/limitid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/limitmax.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/limitmax.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/limitmin.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/limitmin.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/lowerdb.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/lowerdb.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/lrack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/lrack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/lvack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/lvack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/maper.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/maper.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/mapft.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/mapft.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/mdack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/mdack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/mdln.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/mdln.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/mexp.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/mexp.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/mhead.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/mhead.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/mid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/mid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/mlcl.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/mlcl.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/nulbc.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/nulbc.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/objack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/objack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/objid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/objid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/objspec.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/objspec.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/objtype.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/objtype.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/oflack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/oflack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/onlack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/onlack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/orloc.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/orloc.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ppbody.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ppbody.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ppgnt.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ppgnt.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ppid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ppid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/praxi.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/praxi.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/prdct.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/prdct.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/rcmd.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/rcmd.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/refp.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/refp.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/repgsz.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/repgsz.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/rowct.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/rowct.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/rpsel.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/rpsel.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/rptid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/rptid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/rsda.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/rsda.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/rsdc.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/rsdc.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/rsinf.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/rsinf.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/rspack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/rspack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/sdack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/sdack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/sdbin.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/sdbin.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/shead.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/shead.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/smpln.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/smpln.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/softrev.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/softrev.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/stime.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/stime.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/strack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/strack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/strid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/strid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/strp.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/strp.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/sv.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/sv.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/svid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/svid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/svname.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/svname.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/text.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/text.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/tiaack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/tiaack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/tid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/tid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/time.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/time.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/timestamp.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/timestamp.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/totsmp.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/totsmp.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/trid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/trid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/units.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/units.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/upperdb.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/upperdb.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/v.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/v.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU Lesser General Public License for more details.
 #####################################################################
 """V data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class V(DataItemBase):
+class V(DataItemBase):  # pylint: disable=invalid-name
     """
     Variable data.
 
     :Types:
        - :class:`Array <secsgem.secs.variables.Array>`
        - :class:`Boolean <secsgem.secs.variables.Boolean>`
        - :class:`U1 <secsgem.secs.variables.U1>`
```

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/vid.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/vid.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/vlaack.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/vlaack.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/xdies.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/xdies.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/xypos.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/xypos.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/data_items/ydies.py` & `secsgem-0.2.0a4/secsgem/secs/data_items/ydies.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/__init__.py` & `secsgem-0.2.0a4/secsgem/secs/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/base.py` & `secsgem-0.2.0a4/secsgem/secs/variables/array.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,210 +1,216 @@
 #####################################################################
-# base.py
+# array.py
 #
-# (c) Copyright 2015-2021, Benjamin Parzella. All rights reserved.
+# (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Base class for for SECS stream and functions."""
-import typing
+"""SECS array variable type."""
 
 import secsgem.common
-from ..data_items import DataItemBase
-from ..variables import functions
 
-DataItemRecursive = typing.Union[typing.Type[DataItemBase], typing.Iterable["DataItemRecursive"]]
+from . import list_type  # pylint: disable=cyclic-import
+from . import functions  # pylint: disable=cyclic-import
 
+from .base import Base
 
-class StructureDisplayingMeta(type):
-    """Meta class overriding the default __repr__ of a class."""
 
-    def __repr__(cls):
-        """Generate textual representation for an object of this class."""
-        return cls.get_format()
-
-
-class SecsStreamFunction(metaclass=StructureDisplayingMeta):
-    """
-    Secs stream and function base class.
-
-    This class is inherited to create a stream/function class.
-    To create a function specific content the class variables :attr:`_stream`, :attr:`_function`
-    and :attr:`_data_format` must be overridden.
-    """
+class Array(Base):
+    """List variable type. List with items of same type."""
 
-    _stream = 0
-    _function = 0
+    format_code = 0
+    text_code = 'L'
+    preferred_types = [list]
 
-    _data_format: typing.Optional[DataItemRecursive] = None
+    class _SecsVarArrayIter:
+        def __init__(self, values):
+            self._values = values
+            self._counter = 0
 
-    _to_host = True
-    _to_equipment = True
+        def __iter__(self):
+            """Get an iterator."""
+            return self
 
-    _has_reply = False
-    _is_reply_required = False
+        def __next__(self):
+            """Get the next item or raise StopIteration if at end of list."""
+            if self._counter < len(self._values):
+                i = self._counter
+                self._counter += 1
+                return self._values[i]
 
-    _is_multi_block = False
+            raise StopIteration()
 
-    def __init__(self, value=None):
+    def __init__(self, data_format, value=None, count=-1):
         """
-        Initialize a stream function object.
-
-        **Example**::
-
-            class SecsS02F30(SecsStreamFunction):
-                _stream = 2
-                _function = 30
-
-                _to_host = True
-                _to_equipment = False
+        Initialize a secs array variable.
 
-                _has_reply = False
-                _is_reply_required = False
-
-                _is_multi_block = True
-
-                _data_format = [
-                    [
-                        ECID,
-                        ECNAME,
-                        ECMIN,
-                        ECMAX,
-                        ECDEF,
-                        UNITS
-                    ]
-                ]
-
-        :param value: set the value of stream/function parameters
-        :type value: various
+        :param data_format: internal data definition/sample
+        :type data_format: :class:`secs.variables.Base`
+        :param value: initial value
+        :type value: list
+        :param count: number of fields in the list
+        :type count: integer
         """
-        self.data = functions.generate(self._data_format)
-
-        # copy public members from private ones
-        self.stream = self._stream
-        self.function = self._function
+        super().__init__()
 
-        self.data_format = self._data_format
-        self.to_host = self._to_host
-        self.to_equipment = self._to_equipment
+        self.item_decriptor = data_format
+        self.count = count
+        self.data = []
+        if isinstance(data_format, list):
+            self.name = list_type.List.get_name_from_format(data_format)
+        elif hasattr(data_format, "__name__"):
+            self.name = data_format.__name__
+        else:
+            self.name = "UNKNOWN"
 
-        self.has_reply = self._has_reply
-        self.is_reply_required = self._is_reply_required
+        if value is not None:
+            self.set(value)
 
-        self.is_multi_block = self._is_multi_block
+    @staticmethod
+    def get_format(data_format, showname=False):
+        """
+        Get the format of the variable.
 
-        if value is not None and self.data is not None:
-            self.data.set(value)
+        :returns: returns the string representation of the function
+        :rtype: string
+        """
+        if showname:
+            array_name = "{}: "
+            if isinstance(data_format, list):
+                array_name = array_name.format(list_type.List.get_name_from_format(data_format))
+            else:
+                array_name = array_name.format(data_format.__name__)
+        else:
+            array_name = ""
 
-        self._object_intitialized = True
+        if isinstance(data_format, list):
+            return f"{array_name}[\n" \
+                   f"{secsgem.common.indent_block(list_type.List.get_format(data_format), 4)}\n" \
+                   f"    ...\n]"
+
+        return f"{array_name}[\n" \
+               f"{secsgem.common.indent_block(data_format.get_format(not showname), 4)}\n" \
+               f"    ...\n]"
 
     def __repr__(self):
         """Generate textual representation for an object of this class."""
-        function = f"S{self.stream}F{self.function}"
-        if self.data is None:
-            return f"{function}{' W' if self._is_reply_required else ''} ."
-        data = f"{self.data.__repr__()}"
+        if len(self.data) == 0:
+            return f"<{self.text_code}>"
 
-        return f"{function}{' W' if self._is_reply_required else ''}\n{secsgem.common.indent_block(data)} ."
+        data = ""
 
-    def __getitem__(self, key):
-        """Get an item using the indexer operator."""
-        return self.data[key]
+        for value in self.data:
+            data += f"{secsgem.common.indent_block(value.__repr__())}\n"
 
-    def __setitem__(self, key, item):
-        """Set an item using the indexer operator."""
-        self.data[key] = item
+        return f"<{self.text_code} [{len(self.data)}]\n{data}\n>"
 
     def __len__(self):
         """Get the length."""
         return len(self.data)
 
-    def __getattr__(self, item):
-        """Get an item as object member."""
-        return self.data.__getattr__(item)
-
-    def __setattr__(self, item, value):
-        """Set an item as object member."""
-        if '_object_intitialized' not in self.__dict__:
-            dict.__setattr__(self, item, value)
-            return
-
-        if item in self.data.data:
-            self.data.__setattr__(item, value)
-            return
+    def __getitem__(self, key):
+        """Get an item using the indexer operator."""
+        return self.data[key]
+
+    def __iter__(self):
+        """Get an iterator."""
+        return Array._SecsVarArrayIter(self.data)
+
+    def __setitem__(self, key, value):
+        """Set an item using the indexer operator."""
+        if isinstance(value, (type(self.data[key]), self.data[key].__class__.__bases__)):
+            self.data[key] = value
+        elif isinstance(value, Base):
+            raise TypeError(f"Wrong type {value.__class__.__name__} when expecting {self.data[key].__class__.__name__}")
+        else:
+            self.data[key].set(value)
 
     def append(self, data):
         """
-        Append data to list, if stream/function parameter is a list.
+        Append data to the internal list.
 
-        :param data: list item to add
-        :type data: various
+        :param value: new value
+        :type value: various
         """
-        if hasattr(self.data, 'append') and callable(self.data.append):
-            self.data.append(data)
-        else:
-            raise AttributeError(
-                f"class {self.__class__.__name__} has no attribute 'append'")
+        new_object = functions.generate(self.item_decriptor)
+        new_object.set(data)
+        self.data.append(new_object)
 
-    def encode(self):
+    def set(self, value):
         """
-        Generate the encoded hsms data of the stream/function parameter.
+        Set the internal value to the provided value.
 
-        :returns: encoded data
-        :rtype: string
+        :param value: new value
+        :type value: list
         """
-        if self.data is None:
-            return b""
+        if not isinstance(value, list):
+            raise ValueError(f"Invalid value type {type(value).__name__} for {self.__class__.__name__}")
 
-        return self.data.encode()
+        if self.count >= 0:
+            if not len(value) == self.count:
+                raise ValueError(f"Value has invalid field count (expected: {self.count}, actual: {len(value)})")
 
-    def decode(self, data):
-        """
-        Update stream/function parameter data from the passed data.
+        self.data = []
 
-        :param data: encoded data
-        :type data: string
-        """
-        if self.data is not None:
-            self.data.decode(data)
+        for item in value:
+            new_object = functions.generate(self.item_decriptor)
+            new_object.set(item)
+            self.data.append(new_object)
 
-    def set(self, value):
+    def get(self):
         """
-        Update the value of the stream/function parameter.
+        Return the internal value.
 
-        :param value: new value for the parameter
-        :type value: various
+        :returns: internal value
+        :rtype: list
         """
-        self.data.set(value)
+        data = []
+        for item in self.data:
+            data.append(item.get())
 
-    def get(self):
-        """
-        Get the current value of the stream/function parameter.
+        return data
 
-        :returns: current parameter value
-        :rtype: various
+    def encode(self):
         """
-        if self.data is None:
-            return None
-        
-        return self.data.get()
+        Encode the value to secs data.
 
-    @classmethod
-    def get_format(cls):
+        :returns: encoded data bytes
+        :rtype: string
         """
-        Get the format of the function.
+        result = self.encode_item_header(len(self.data))
 
-        :returns: returns the string representation of the function
-        :rtype: string
+        for item in self.data:
+            result += item.encode()
+
+        return result
+
+    def decode(self, data, start=0):
         """
-        if cls._data_format is not None:
-            return functions.get_format(cls._data_format)
+        Decode the secs byte data to the value.
+
+        :param data: encoded data bytes
+        :type data: string
+        :param start: start position of value the data
+        :type start: integer
+        :returns: new start position
+        :rtype: integer
+        """
+        (text_pos, _, length) = self.decode_item_header(data, start)
+
+        # list
+        self.data = []
+
+        for _ in range(length):
+            new_object = functions.generate(self.item_decriptor)
+            text_pos = new_object.decode(data, text_pos)
+            self.data.append(new_object)
 
-        return "Header only"
+        return text_pos
```

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s00f00.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s00f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f00.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f01.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f01.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f02.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f02.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f03.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f03.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f04.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f04.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f11.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f11.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f12.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f12.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f13.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f13.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f14.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f14.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f15.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f15.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f16.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f16.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f17.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f17.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f18.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f18.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f21.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f21.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f22.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f22.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f23.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f23.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s01f24.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s01f24.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f00.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f13.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f13.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f14.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f14.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f15.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f15.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f16.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f16.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f17.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f17.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f18.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f18.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f21.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f21.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f22.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f22.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f23.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f23.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f24.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f24.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f25.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f25.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f26.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f26.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f29.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f29.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f30.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f30.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f33.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f33.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f34.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f34.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f35.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f35.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f36.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f36.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f37.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f37.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f38.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f38.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f41.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f41.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f42.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f42.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f43.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f43.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f44.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f44.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f45.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f45.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f46.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f46.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f47.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f47.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f48.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f48.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f49.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f49.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s02f50.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s02f50.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f00.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f01.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f01.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f02.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f02.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f03.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f03.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f04.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f04.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f05.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f05.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f06.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f06.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f07.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f07.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f08.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f08.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f09.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f09.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f10.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f10.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f11.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f11.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f12.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f12.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f13.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f13.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f14.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f14.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f15.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f15.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f16.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f16.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f17.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f17.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s05f18.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s05f18.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f00.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f01.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f01.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f02.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f02.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f05.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f05.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f06.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f06.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f07.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f07.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f08.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f08.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f11.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f11.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f12.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f12.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f15.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f15.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f16.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f16.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f19.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f19.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f20.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f20.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f21.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f21.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f22.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f22.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f23.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f23.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s06f24.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s06f24.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s07f00.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s07f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s07f01.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s07f01.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s07f02.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s07f02.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s07f03.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s07f03.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s07f04.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s07f04.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s07f05.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s07f05.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s07f06.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s07f06.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s07f17.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s07f17.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s07f18.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s07f18.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s07f19.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s07f19.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s07f20.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s07f20.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s09f00.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s09f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s09f01.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s09f01.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s09f03.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s09f03.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s09f05.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s09f05.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s09f07.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s09f07.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s09f09.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s09f09.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s09f11.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s09f11.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s09f13.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s09f13.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s10f00.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s10f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s10f01.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s10f01.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s10f02.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s10f02.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s10f03.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s10f03.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s10f04.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s10f04.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f00.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f01.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f01.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f02.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f02.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f03.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f03.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f04.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f04.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f05.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f05.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f06.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f06.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f07.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f07.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f08.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f08.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f09.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f09.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f10.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f10.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f11.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f11.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f12.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f12.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f13.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f13.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f14.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f14.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f15.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f15.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f16.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f16.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f17.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f17.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f18.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f18.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s12f19.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s12f19.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s14f00.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s14f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s14f01.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s14f01.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s14f02.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s14f02.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s14f03.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s14f03.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/functions/s14f04.py` & `secsgem-0.2.0a4/secsgem/secs/functions/s14f04.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/handler.py` & `secsgem-0.2.0a4/secsgem/secs/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,104 +9,105 @@
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Handler for SECS commands. Used in combination with :class:`secsgem.HsmsHandler.HsmsConnectionManager`."""
+"""Handler for SECS commands. Used in combination with :class:`secsgem.hsms.HsmsConnectionManager`."""
 import copy
 import logging
 import threading
 import typing
 
+import secsgem.common
 import secsgem.hsms
 
 from . import functions
 
 if typing.TYPE_CHECKING:
     from ..gem.collection_event import CollectionEvent
     from ..gem.data_value import DataValue
     from ..gem.alarm import Alarm
     from ..gem.remote_command import RemoteCommand
 
 
-class SecsHandler:
+class SecsHandler:  # pylint: disable=too-many-instance-attributes
     """
     Baseclass for creating Host/Equipment models. This layer contains the SECS functionality.
 
     Inherit from this class and override required functions.
     """
 
-    def __init__(self, connection: secsgem.hsms.HsmsHandler):
+    def __init__(self, connection: secsgem.common.Protocol):
         """
         Initialize a secs handler.
 
         :param connection: connection to use
         """
-        self._connection = connection
-        self._connection.events.hsms_packet_received += self._on_hsms_packet_received
-        self._connection.secs_decode = self.secs_decode
+        self._protocol = connection
+        self._protocol.events.hsms_packet_received += self._on_hsms_packet_received
+        self._protocol.secs_decode = self.secs_decode
 
         self.logger = logging.getLogger(self.__module__ + "." + self.__class__.__name__)
 
-        self._collectionEvents: typing.Dict[typing.Union[int, str], CollectionEvent] = {}
-        self._dataValues: typing.Dict[typing.Union[int, str], DataValue] = {}
+        self._collection_events: typing.Dict[typing.Union[int, str], CollectionEvent] = {}
+        self._data_values: typing.Dict[typing.Union[int, str], DataValue] = {}
         self._alarms: typing.Dict[typing.Union[int, str], Alarm] = {}
-        self._remoteCommands: typing.Dict[typing.Union[int, str], RemoteCommand] = {}
+        self._remote_commands: typing.Dict[typing.Union[int, str], RemoteCommand] = {}
 
         self._callback_handler = secsgem.common.CallbackHandler()
         self._callback_handler.target = self
 
         self.secs_streams_functions = copy.deepcopy(functions.secs_streams_functions)
 
     @classmethod
     def hsms(cls, address, port, active, session_id, name, custom_connection_handler=None, **kwargs) -> "SecsHandler":
         """
         Initialize a secs handler using a hsms connection.
 
         All arguments will be passed to the HSMS handler.
         """
         return cls(
-            secsgem.hsms.HsmsHandler(address, port, active, session_id, name, custom_connection_handler),
+            secsgem.hsms.HsmsProtocol(address, port, active, session_id, name, custom_connection_handler),
             **kwargs)
 
     @staticmethod
     def _generate_sf_callback_name(stream: int, function: int) -> str:
         return f"s{stream:02d}f{function:02d}"
 
     @property
-    def connection(self) -> secsgem.hsms.HsmsHandler:
+    def protocol(self) -> secsgem.common.Protocol:
         """Get the connection for the handler."""
-        return self._connection
+        return self._protocol
 
     def enable(self):
         """Enable the connection."""
-        self.connection.enable()
+        self.protocol.enable()
 
     def disable(self):
         """Disable the connection."""
-        self.connection.disable()
+        self.protocol.disable()
 
     def send_response(self, *args, **kwargs):
         """Wrapper for connections send_response function."""
-        return self.connection.send_response(*args, **kwargs)
+        return self.protocol.send_response(*args, **kwargs)
 
     def send_and_waitfor_response(self, *args, **kwargs):
         """Wrapper for connections send_and_waitfor_response function."""
-        return self.connection.send_and_waitfor_response(*args, **kwargs)
+        return self.protocol.send_and_waitfor_response(*args, **kwargs)
 
     def send_stream_function(self, *args, **kwargs):
         """Wrapper for connections send_stream_function function."""
-        return self.connection.send_stream_function(*args, **kwargs)
+        return self.protocol.send_stream_function(*args, **kwargs)
 
     @property
     def events(self):
         """Wrapper for connections events."""
-        return self.connection.events
+        return self.protocol.events
 
     @property
     def callbacks(self):
         """Property for callback handling."""
         return self._callback_handler
 
     def register_stream_function(self, stream: int, function: int, callback):
@@ -156,15 +157,15 @@
             name
                 Name of the collection event (string)
 
             dvids
                 Data values for the collection event (list of integers)
 
         """
-        return self._collectionEvents
+        return self._collection_events
 
     @property
     def data_values(self):
         """
         Get available data values.
 
         *Example*::
@@ -183,15 +184,15 @@
             name
                 Name of the data value (string)
 
             ceid
                 Collection event the data value is used for (integer)
 
         """
-        return self._dataValues
+        return self._data_values
 
     @property
     def alarms(self):
         """
         Get available alarms.
 
         *Example*::
@@ -248,23 +249,23 @@
                     format
                         format character of the parameter (string)
 
             ceids
                 Collection events ids the remote command might return (list of integers)
 
         """
-        return self._remoteCommands
+        return self._remote_commands
 
     def _handle_stream_function(self, packet):
         sf_callback_index = self._generate_sf_callback_name(packet.header.stream, packet.header.function)
 
         # return S09F05 if no callback present
         if sf_callback_index not in self._callback_handler:
             self.logger.warning("unexpected function received %s\n%s", sf_callback_index, packet.header)
-            if packet.header.requireResponse:
+            if packet.header.require_response:
                 self.send_response(self.stream_function(9, 5)(packet.header.encode()), packet.header.system)
 
             return
 
         try:
             callback = getattr(self._callback_handler, sf_callback_index)
             result = callback(self, packet)
@@ -275,15 +276,15 @@
             self.send_response(self.stream_function(packet.header.stream, 0)(), packet.header.system)
 
     def _on_hsms_packet_received(self, data):
         """
         Packet received from hsms layer.
 
         :param data: received data
-        :type data: :class:`secsgem.hsms.HsmsPacket`
+        :type data: :class:`secsgem.common.Packet`
         """
         packet = data["packet"]
 
         # check if callbacks available for this stream and function
         threading.Thread(
             target=self._handle_stream_function, args=(packet, ),
             name=f"secsgem_secsHandler_callback_S{packet.header.stream}F{packet.header.function}").start()
@@ -431,32 +432,32 @@
         Get the name of a collection event.
 
         :param ceid: ID of collection event
         :type ceid: integer
         :returns: Name of the event or empty string if not found
         :rtype: string
         """
-        if ceid in self._collectionEvents:
-            if "name" in self._collectionEvents[ceid]:
-                return self._collectionEvents[ceid]["name"]
+        if ceid in self._collection_events:
+            if "name" in self._collection_events[ceid]:
+                return self._collection_events[ceid]["name"]
 
         return ""
 
     def get_dvid_name(self, dvid):
         """
         Get the name of a data value.
 
         :param dvid: ID of data value
         :type dvid: integer
         :returns: Name of the event or empty string if not found
         :rtype: string
         """
-        if dvid in self._dataValues:
-            if "name" in self._dataValues[dvid]:
-                return self._dataValues[dvid]["name"]
+        if dvid in self._data_values:
+            if "name" in self._data_values[dvid]:
+                return self._data_values[dvid]["name"]
 
         return ""
 
     def are_you_there(self):
         """Check if remote is still replying."""
         self.logger.info("Requesting 'are you there'")
 
@@ -484,15 +485,15 @@
         return self.secs_streams_functions[stream][function]
 
     def secs_decode(self, packet):
         """
         Get object of decoded stream and function class, or None if no class is available.
 
         :param packet: packet to get object for
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :type packet: :class:`secsgem.common.Packet`
         :return: matching stream and function object
         :rtype: secsSxFx object
         """
         if packet is None:
             return None
 
         if packet.header.stream not in self.secs_streams_functions:
```

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/__init__.py` & `secsgem-0.2.0a4/secsgem/secs/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/array.py` & `secsgem-0.2.0a4/secsgem/secs/variables/dynamic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,216 +1,277 @@
 #####################################################################
-# array.py
+# dynamic.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""SECS array variable type."""
-
-import secsgem.common
-
-from . import list_type  # pylint: disable=cyclic-import
-from . import functions  # pylint: disable=cyclic-import
+"""SECS dynamic variable type."""
 
 from .base import Base
+from .array import Array
+from .binary import Binary
+from .boolean import Boolean
+from .string import String
+from .u1 import U1
+from .u2 import U2
+from .u4 import U4
+from .u8 import U8
+from .i1 import I1
+from .i2 import I2
+from .i4 import I4
+from .i8 import I8
+from .f4 import F4
+from .f8 import F8
+
+
+class Dynamic(Base):
+    """Variable with interchangable type."""
 
-
-class Array(Base):
-    """List variable type. List with items of same type."""
-
-    format_code = 0
-    text_code = 'L'
-    preferred_types = [list]
-
-    class _SecsVarArrayIter:
-        def __init__(self, values):
-            self._values = values
-            self._counter = 0
-
-        def __iter__(self):
-            """Get an iterator."""
-            return self
-
-        def __next__(self):
-            """Get the next item or raise StopIteration if at end of list."""
-            if self._counter < len(self._values):
-                i = self._counter
-                self._counter += 1
-                return self._values[i]
-
-            raise StopIteration()
-
-    def __init__(self, data_format, value=None, count=-1):
+    def __init__(self, types, value=None, count=-1):
         """
-        Initialize a secs array variable.
+        Initialize a dynamic secs variable.
 
-        :param data_format: internal data definition/sample
-        :type data_format: :class:`secs.variables.Base`
+        :param types: list of supported types, default first. empty means all types are support, String default
+        :type types: list of :class:`secsgem.secs.variables.Base` classes
         :param value: initial value
-        :type value: list
-        :param count: number of fields in the list
+        :type value: various
+        :param count: max number of items in type
         :type count: integer
         """
         super().__init__()
 
-        self.item_decriptor = data_format
-        self.count = count
-        self.data = []
-        if isinstance(data_format, list):
-            self.name = list_type.List.get_name_from_format(data_format)
-        elif hasattr(data_format, "__name__"):
-            self.name = data_format.__name__
-        else:
-            self.name = "UNKNOWN"
+        self.value = None
 
+        self.types = types
+        self.count = count
         if value is not None:
             self.set(value)
 
-    @staticmethod
-    def get_format(data_format, showname=False):
-        """
-        Get the format of the variable.
-
-        :returns: returns the string representation of the function
-        :rtype: string
-        """
-        if showname:
-            array_name = "{}: "
-            if isinstance(data_format, list):
-                array_name = array_name.format(list_type.List.get_name_from_format(data_format))
-            else:
-                array_name = array_name.format(data_format.__name__)
-        else:
-            array_name = ""
-
-        if isinstance(data_format, list):
-            return f"{array_name}[\n" \
-                   f"{secsgem.common.indent_block(list_type.List.get_format(data_format), 4)}\n" \
-                   f"    ...\n]"
-
-        return f"{array_name}[\n" \
-               f"{secsgem.common.indent_block(data_format.get_format(not showname), 4)}\n" \
-               f"    ...\n]"
-
     def __repr__(self):
         """Generate textual representation for an object of this class."""
-        if len(self.data) == 0:
-            return f"<{self.text_code}>"
-
-        data = ""
-
-        for value in self.data:
-            data += f"{secsgem.common.indent_block(value.__repr__())}\n"
-
-        return f"<{self.text_code} [{len(self.data)}]\n{data}\n>"
+        return self.value.__repr__()
 
     def __len__(self):
         """Get the length."""
-        return len(self.data)
+        return self.value.__len__()
 
     def __getitem__(self, key):
         """Get an item using the indexer operator."""
-        return self.data[key]
-
-    def __iter__(self):
-        """Get an iterator."""
-        return Array._SecsVarArrayIter(self.data)
+        return self.value.__getitem__(key)
 
-    def __setitem__(self, key, value):
+    def __setitem__(self, key, item):
         """Set an item using the indexer operator."""
-        if isinstance(value, (type(self.data[key]), self.data[key].__class__.__bases__)):
-            self.data[key] = value
-        elif isinstance(value, Base):
-            raise TypeError(f"Wrong type {value.__class__.__name__} when expecting {self.data[key].__class__.__name__}")
-        else:
-            self.data[key].set(value)
+        self.value.__setitem__(key, item)
 
-    def append(self, data):
-        """
-        Append data to the internal list.
+    def __eq__(self, other):
+        """Check equality with other object."""
+        if isinstance(other, Dynamic):
+            return other.value.value == self.value.value
+        if isinstance(other, Base):
+            return other.value == self.value.value
+        if isinstance(other, list):
+            return other == self.value.value
+        if isinstance(other, (bytes, str)) and isinstance(self.value.value, (bytes, str)):
+            return str(other) == str(self.value.value)
+
+        return [other] == self.value.value
+
+    def __hash__(self):
+        """Get data item for hashing."""
+        if isinstance(self.value.value, list):
+            return hash(self.value.value[0])
+        return hash(self.value.value)
+
+    def __type_supported(self, typ):
+        if not self.types:
+            return True
+
+        if typ in self.types:
+            return True
+
+        return False
+
+    @property
+    def preferred_type(self):
+        """Get the preferred type."""
+        types = []
+        for typ in self.__allowedtypes__:
+            types += typ.preferred_types
 
-        :param value: new value
-        :type value: various
-        """
-        new_object = functions.generate(self.item_decriptor)
-        new_object.set(data)
-        self.data.append(new_object)
+        return types[0]
 
     def set(self, value):
         """
         Set the internal value to the provided value.
 
+        In doubt provide the variable wrapped in the matching :class:`secsgem.secs.variables.Base` class,
+        to avoid confusion.
+
+        **Example**::
+
+            >>> import secsgem.secs
+            >>>
+            >>> var = secsgem.secs.variables.Dynamic([secsgem.secs.variables.String,
+            ...                                       secsgem.secs.variables.U1])
+            >>> var.set(secsgem.secs.variables.U1(10))
+            >>> var
+            <U1 10 >
+
+        If no type is provided the default type is used which might not be the expected type.
+
         :param value: new value
-        :type value: list
+        :type value: various
         """
-        if not isinstance(value, list):
-            raise ValueError(f"Invalid value type {type(value).__name__} for {self.__class__.__name__}")
+        if isinstance(value, Base):
+            if isinstance(value, Dynamic):
+                if not isinstance(value.value, tuple(self.types)) and self.types:
+                    raise ValueError(
+                        f"Unsupported type {value.value.__class__.__name__} "
+                        f"for this instance of Dynamic, allowed {self.types}")
+
+                self.value = value.value
+            else:
+                if not isinstance(value, tuple(self.types)) and self.types:
+                    raise ValueError(
+                        f"Unsupported type {value.__class__.__name__} "
+                        f"for this instance of Dynamic, allowed {self.types}")
 
-        if self.count >= 0:
-            if not len(value) == self.count:
-                raise ValueError(f"Value has invalid field count (expected: {self.count}, actual: {len(value)})")
+                self.value = value
+        else:
+            matched_type = self._match_type(value)
 
-        self.data = []
+            if matched_type is None:
+                raise ValueError(
+                    f'Value "{value}" of type {value.__class__.__name__} not valid for SecsDynamic with {self.types}')
 
-        for item in value:
-            new_object = functions.generate(self.item_decriptor)
-            new_object.set(item)
-            self.data.append(new_object)
+            self.value = matched_type(count=self.count)
+            self.value.set(value)
 
     def get(self):
         """
         Return the internal value.
 
         :returns: internal value
-        :rtype: list
+        :rtype: various
         """
-        data = []
-        for item in self.data:
-            data.append(item.get())
+        if self.value is not None:
+            return self.value.get()
 
-        return data
+        return None
 
     def encode(self):
         """
         Encode the value to secs data.
 
         :returns: encoded data bytes
         :rtype: string
         """
-        result = self.encode_item_header(len(self.data))
-
-        for item in self.data:
-            result += item.encode()
-
-        return result
+        return self.value.encode()
 
     def decode(self, data, start=0):
         """
         Decode the secs byte data to the value.
 
         :param data: encoded data bytes
         :type data: string
         :param start: start position of value the data
         :type start: integer
         :returns: new start position
         :rtype: integer
         """
-        (text_pos, _, length) = self.decode_item_header(data, start)
+        (_, format_code, _) = self.decode_item_header(data, start)
 
-        # list
-        self.data = []
+        format_codes = {
+            Array.format_code: Array,
+            Binary.format_code: Binary,
+            Boolean.format_code: Boolean,
+            String.format_code: String,
+            I8.format_code: I8,
+            I1.format_code: I1,
+            I2.format_code: I2,
+            I4.format_code: I4,
+            F8.format_code: F8,
+            F4.format_code: F4,
+            U8.format_code: U8,
+            U1.format_code: U1,
+            U2.format_code: U2,
+            U4.format_code: U4,
+        }
+
+        if format_code not in format_codes or not self.__type_supported(format_codes[format_code]):
+            raise ValueError(
+                f"Unsupported format {format_code} for this instance of Dynamic, allowed {self.types}")
+
+        typ = format_codes[format_code]
+        if typ == Array:
+            self.value = Array(ANYVALUE)
+        else:
+            self.value = typ(count=self.count)
+
+        return self.value.decode(data, start)
 
-        for _ in range(length):
-            new_object = functions.generate(self.item_decriptor)
-            text_pos = new_object.decode(data, text_pos)
-            self.data.append(new_object)
+    def _match_type(self, value):
+        var_types = self.types
+        # if no types are set use internal order
+        if not self.types:
+            var_types = [Boolean, U1, U2, U4, U8, I1, I2, I4,
+                         I8, F4, F8, String, Binary]
+
+        # first try to find the preferred type for the kind of value
+        for var_type in var_types:
+            if isinstance(value, tuple(var_type.preferred_types)):
+                if var_type(count=self.count).supports_value(value):
+                    return var_type
+
+        # when no preferred type was found, then try to match any available type
+        for var_type in var_types:
+            if var_type(count=self.count).supports_value(value):
+                return var_type
+
+        return None
+
+    @property
+    def is_dynamic(self) -> bool:
+        """Check if this instance is Dynamic or derived."""
+        return True
+
+
+class ANYVALUE(Dynamic):
+    """
+    Dummy data item for generation of unknown types.
+
+    :Types:
+       - :class:`Array <secsgem.secs.variables.Array>`
+       - :class:`Binary <secsgem.secs.variables.Binary>`
+       - :class:`Boolean <secsgem.secs.variables.Boolean>`
+       - :class:`String <secsgem.secs.variables.String>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`F8 <secsgem.secs.variables.F8>`
+       - :class:`F4 <secsgem.secs.variables.F4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`U1 <secsgem.secs.variables.U1>`
+       - :class:`U2 <secsgem.secs.variables.U2>`
+       - :class:`U4 <secsgem.secs.variables.U4>`
+
+    """
+
+    def __init__(self, value=None):
+        """
+        Initialize an ANYVALUE variable.
+
+        :param value: value of the variable
+        """
+        self.name = self.__class__.__name__
 
-        return text_pos
+        super().__init__([Array, Boolean, U1, U2, U4, U8, I1, I2, I4, I8, F4, F8, String, Binary], value=value)
```

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/base.py` & `secsgem-0.2.0a4/secsgem/secs/variables/base.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/base_number.py` & `secsgem-0.2.0a4/secsgem/secs/variables/base_number.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/base_text.py` & `secsgem-0.2.0a4/secsgem/secs/variables/base_text.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/binary.py` & `secsgem-0.2.0a4/secsgem/secs/variables/binary.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/boolean.py` & `secsgem-0.2.0a4/secsgem/secs/variables/boolean.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/f4.py` & `secsgem-0.2.0a4/secsgem/secs/variables/f4.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/f8.py` & `secsgem-0.2.0a4/secsgem/secs/variables/f8.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/functions.py` & `secsgem-0.2.0a4/secsgem/secs/variables/functions.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/i1.py` & `secsgem-0.2.0a4/secsgem/secs/variables/i1.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/i2.py` & `secsgem-0.2.0a4/secsgem/secs/variables/i2.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/i4.py` & `secsgem-0.2.0a4/secsgem/secs/variables/i4.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/i8.py` & `secsgem-0.2.0a4/secsgem/secs/variables/i8.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/jis8.py` & `secsgem-0.2.0a4/secsgem/secs/variables/jis8.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/list_type.py` & `secsgem-0.2.0a4/secsgem/secs/variables/list_type.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/string.py` & `secsgem-0.2.0a4/secsgem/secs/variables/string.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/u1.py` & `secsgem-0.2.0a4/secsgem/secs/variables/u1.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/u2.py` & `secsgem-0.2.0a4/secsgem/secs/variables/u2.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/u4.py` & `secsgem-0.2.0a4/secsgem/secs/variables/u4.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/secsgem/secs/variables/u8.py` & `secsgem-0.2.0a4/secsgem/secs/variables/u8.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a3/PKG-INFO` & `secsgem-0.2.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secsgem
-Version: 0.2.0a3
+Version: 0.2.0a4
 Summary: Python SECS/GEM implementation
 Home-page: https://github.com/bparzella/secsgem
 License: LGPL-2.1-or-later
 Keywords: development,hsms,secs,gem
 Author: Benjamin Parzella
 Author-email: bparzella@gmail.com
 Requires-Python: >=3.7.2,<4.0.0
```

