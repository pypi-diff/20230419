# Comparing `tmp/iqrfpy-0.1.7.tar.gz` & `tmp/iqrfpy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqrfpy-0.1.7.tar", last modified: Mon Apr 17 12:38:20 2023, max compression
+gzip compressed data, was "iqrfpy-0.1.8.tar", last modified: Wed Apr 19 11:31:25 2023, max compression
```

## Comparing `iqrfpy-0.1.7.tar` & `iqrfpy-0.1.8.tar`

### file list

```diff
@@ -1,198 +1,219 @@
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.462592 iqrfpy-0.1.7/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      309 2023-03-12 10:44:36.000000 iqrfpy-0.1.7/.editorconfig
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      113 2023-03-27 06:23:13.000000 iqrfpy-0.1.7/.gitignore
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      937 2023-03-22 19:16:00.000000 iqrfpy-0.1.7/.gitlab-ci.yml
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      203 2023-03-22 19:16:00.000000 iqrfpy-0.1.7/.pylintrc
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    11346 2023-03-24 07:47:59.000000 iqrfpy-0.1.7/LICENSE
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      699 2023-04-15 05:33:58.000000 iqrfpy-0.1.7/Makefile
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-17 12:38:20.462592 iqrfpy-0.1.7/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        9 2023-03-07 12:47:49.000000 iqrfpy-0.1.7/README.md
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.442591 iqrfpy-0.1.7/examples/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2151 2023-04-17 12:28:14.000000 iqrfpy-0.1.7/examples/response_factories.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.442591 iqrfpy-0.1.7/iqrfpy/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      111 2023-04-17 12:36:47.000000 iqrfpy-0.1.7/iqrfpy/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.446591 iqrfpy-0.1.7/iqrfpy/enums/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       90 2023-03-24 10:27:58.000000 iqrfpy-0.1.7/iqrfpy/enums/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5379 2023-03-24 10:38:31.000000 iqrfpy-0.1.7/iqrfpy/enums/commands.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4646 2023-03-24 10:31:05.000000 iqrfpy-0.1.7/iqrfpy/enums/message_types.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      708 2023-03-24 10:49:19.000000 iqrfpy-0.1.7/iqrfpy/enums/peripherals.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4173 2023-04-07 15:58:03.000000 iqrfpy-0.1.7/iqrfpy/exceptions.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.446591 iqrfpy-0.1.7/iqrfpy/messages/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       61 2023-03-24 07:14:54.000000 iqrfpy-0.1.7/iqrfpy/messages/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.446591 iqrfpy-0.1.7/iqrfpy/messages/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2454 2023-04-15 07:42:07.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/IRequest.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      184 2023-04-15 05:52:25.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.446591 iqrfpy-0.1.7/iqrfpy/messages/requests/binaryoutput/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:27.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/binaryoutput/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1024 2023-04-15 07:16:20.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/AddrInfo.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2730 2023-04-17 12:15:28.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/AuthorizeBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1595 2023-04-15 07:21:20.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/Backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2400 2023-04-15 07:23:56.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/BondNode.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1044 2023-04-15 07:22:26.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/BondedDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1046 2023-04-15 07:24:16.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/ClearAllBonds.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1060 2023-04-15 07:24:30.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/DiscoveredDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2044 2023-04-15 07:26:04.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/Discovery.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1677 2023-04-15 07:26:47.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/RemoveBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1879 2023-04-15 07:28:01.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/Restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1465 2023-04-15 07:28:26.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SetDpaParams.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2389 2023-04-15 08:13:58.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SetHops.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2135 2023-04-15 07:33:11.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SetMID.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5293 2023-04-15 07:39:44.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SmartConnect.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      955 2023-03-16 15:28:35.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/dali/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:18.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/dali/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/eeeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:26.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/eeeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/eeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:21.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/eeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/exploration/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/exploration/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/frc/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:40.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/frc/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/generic/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/generic/Raw.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/generic/RawHdp.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/generic/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/io/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:21.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/io/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/ledg/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:15.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/ledg/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/ledr/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:11.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/ledr/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/light/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:37.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/light/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/node/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      957 2023-04-15 07:43:28.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/node/Read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:41:43.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/node/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/os/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:14.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/os/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/ram/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:31.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/ram/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/sensor/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:31.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/sensor/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/thermometer/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:27.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/thermometer/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/uart/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:32.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/uart/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     8383 2023-04-15 07:00:07.000000 iqrfpy-0.1.7/iqrfpy/messages/response_factory.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2735 2023-04-15 08:08:05.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/AsyncResponse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2484 2023-04-15 08:09:36.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/Confirmation.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3277 2023-04-15 08:09:43.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/IResponse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      214 2023-04-15 05:57:36.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/responses/binaryoutput/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:04.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/binaryoutput/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2548 2023-04-15 07:49:09.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/AddrInfo.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2659 2023-04-15 07:51:29.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/AuthorizeBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2468 2023-04-15 07:52:33.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/Backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2582 2023-04-15 07:55:01.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/BondNode.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2023-04-15 07:54:09.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/BondedDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2231 2023-04-15 07:56:16.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/ClearAllBonds.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2627 2023-04-15 07:57:08.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/DiscoveredDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2475 2023-04-15 07:58:02.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/Discovery.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2480 2023-04-15 07:58:52.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/RemoveBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2039 2023-04-15 07:59:57.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/Restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2622 2023-04-15 08:01:05.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SetDpaParams.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2634 2023-04-15 08:02:04.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SetHops.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2033 2023-04-15 08:03:57.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SetMID.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2650 2023-04-15 08:04:34.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SmartConnect.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      983 2023-03-24 07:27:46.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/dali/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:58.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/dali/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/eeeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:01.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/eeeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/eeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:56.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/eeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/exploration/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-04-15 05:56:54.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/exploration/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/frc/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:43.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/frc/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/generic/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-04-15 05:56:49.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/generic/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/io/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:27.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/io/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/ledg/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:23.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/ledg/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/ledr/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:19.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/ledr/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/light/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:14.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/light/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/node/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2579 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/node/Read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:49.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/node/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/os/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:52.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/os/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/ram/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:05.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/ram/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/sensor/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:09.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/sensor/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/thermometer/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:32.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/thermometer/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/uart/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:37.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/uart/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/transports/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      300 2023-03-22 19:16:00.000000 iqrfpy-0.1.7/iqrfpy/transports/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2786 2023-04-17 12:36:20.000000 iqrfpy-0.1.7/iqrfpy/transports/itransport.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2076 2023-03-24 09:57:48.000000 iqrfpy-0.1.7/iqrfpy/transports/mqtt_transport.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3788 2023-03-24 09:57:48.000000 iqrfpy-0.1.7/iqrfpy/transports/udp_transport.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/utils/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       50 2023-03-24 11:33:36.000000 iqrfpy-0.1.7/iqrfpy/utils/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    20492 2023-04-15 08:13:29.000000 iqrfpy-0.1.7/iqrfpy/utils/common.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1810 2023-04-15 07:47:59.000000 iqrfpy-0.1.7/iqrfpy/utils/dpa.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      343 2023-04-15 06:15:47.000000 iqrfpy-0.1.7/iqrfpy/utils/enums.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.442591 iqrfpy-0.1.7/iqrfpy.egg-info/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-17 12:38:20.000000 iqrfpy-0.1.7/iqrfpy.egg-info/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     6218 2023-04-17 12:38:20.000000 iqrfpy-0.1.7/iqrfpy.egg-info/SOURCES.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2023-04-17 12:38:20.000000 iqrfpy-0.1.7/iqrfpy.egg-info/dependency_links.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      159 2023-04-17 12:38:20.000000 iqrfpy-0.1.7/iqrfpy.egg-info/requires.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2023-04-17 12:38:20.000000 iqrfpy-0.1.7/iqrfpy.egg-info/top_level.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      138 2023-03-24 09:25:00.000000 iqrfpy-0.1.7/pyproject.toml
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       85 2023-03-24 07:40:43.000000 iqrfpy-0.1.7/requirements.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1162 2023-04-17 12:38:20.462592 iqrfpy-0.1.7/setup.cfg
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      102 2023-03-22 19:16:00.000000 iqrfpy-0.1.7/test_requirements.txt
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/tests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-07 12:49:34.000000 iqrfpy-0.1.7/tests/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/tests/enums/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1241 2023-03-24 10:31:41.000000 iqrfpy-0.1.7/tests/enums/Peripherals_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/tests/messages/
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.458591 iqrfpy-0.1.7/tests/messages/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1292 2023-03-18 09:19:32.000000 iqrfpy-0.1.7/tests/messages/requests/IRequest_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.458591 iqrfpy-0.1.7/tests/messages/requests/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      869 2023-03-18 09:24:49.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/AddrInfoRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4015 2023-04-02 10:26:13.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/AuthorizeBondRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2194 2023-03-18 09:44:00.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/BackupRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3758 2023-03-18 09:50:37.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/BondNodeRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      903 2023-03-18 09:24:46.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/BondedDevicesRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      904 2023-03-18 09:57:38.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/ClearAllBondsRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      925 2023-03-18 09:59:43.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3445 2023-03-18 10:11:35.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/DiscoveryRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2322 2023-03-18 10:17:19.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/RemoveBondRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4241 2023-03-18 10:45:18.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/RestoreRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2257 2023-03-18 10:55:51.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/SetDpaParamsRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3672 2023-03-18 11:08:56.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/SetHopsRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3511 2023-03-18 11:37:09.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/SetMIDRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    11030 2023-03-19 07:20:25.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/SmartConnectRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4827 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/response_factory_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.458591 iqrfpy-0.1.7/tests/messages/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2162 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/AsyncResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1280 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/Confirmation_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.462592 iqrfpy-0.1.7/tests/messages/responses/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4325 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/AddrInfoResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4514 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/AuthorizeBondResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4765 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/BackupResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4391 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/BondNodeResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4212 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/BondedDevicesResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3155 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/ClearAllBondsResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4344 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3785 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/DiscoveryResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3795 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/RemoveNodeResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3055 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/RestoreResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3931 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/SetDpaParamsResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4491 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/SetHopsResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3053 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/SetMIDResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4487 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/SmartConnectResponse_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.462592 iqrfpy-0.1.7/tests/utils/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    16223 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/utils/Common_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       78 2023-03-22 19:16:00.000000 iqrfpy-0.1.7/tox.ini
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.523062 iqrfpy-0.1.8/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      309 2023-03-12 10:44:36.000000 iqrfpy-0.1.8/.editorconfig
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      113 2023-03-27 06:23:13.000000 iqrfpy-0.1.8/.gitignore
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      937 2023-03-22 19:16:00.000000 iqrfpy-0.1.8/.gitlab-ci.yml
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      203 2023-03-22 19:16:00.000000 iqrfpy-0.1.8/.pylintrc
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    11346 2023-03-24 07:47:59.000000 iqrfpy-0.1.8/LICENSE
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      699 2023-04-15 05:33:58.000000 iqrfpy-0.1.8/Makefile
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-19 11:31:25.523062 iqrfpy-0.1.8/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        9 2023-03-07 12:47:49.000000 iqrfpy-0.1.8/README.md
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.515062 iqrfpy-0.1.8/examples/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1007 2023-04-19 09:16:46.000000 iqrfpy-0.1.8/examples/mqtt_transport_async.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2081 2023-04-19 10:00:28.000000 iqrfpy-0.1.8/examples/response_factories.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.515062 iqrfpy-0.1.8/iqrfpy/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      111 2023-04-19 11:29:52.000000 iqrfpy-0.1.8/iqrfpy/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.515062 iqrfpy-0.1.8/iqrfpy/enums/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       88 2023-04-18 07:35:52.000000 iqrfpy-0.1.8/iqrfpy/enums/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     6909 2023-04-18 07:34:49.000000 iqrfpy-0.1.8/iqrfpy/enums/commands.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5553 2023-04-18 08:53:31.000000 iqrfpy-0.1.8/iqrfpy/enums/message_types.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      692 2023-04-18 07:35:22.000000 iqrfpy-0.1.8/iqrfpy/enums/peripherals.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4173 2023-04-07 15:58:03.000000 iqrfpy-0.1.8/iqrfpy/exceptions.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.515062 iqrfpy-0.1.8/iqrfpy/messages/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       61 2023-03-24 07:14:54.000000 iqrfpy-0.1.8/iqrfpy/messages/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.515062 iqrfpy-0.1.8/iqrfpy/messages/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      184 2023-04-15 05:52:25.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.515062 iqrfpy-0.1.8/iqrfpy/messages/requests/binaryoutput/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:27.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/binaryoutput/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.515062 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      968 2023-04-18 07:04:34.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1024 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/addr_info.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2730 2023-04-18 07:12:41.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/authorize_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1595 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2400 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/bond_node.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1044 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/bonded_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1046 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/clear_all_bonds.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1060 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/discovered_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2044 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/discovery.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1677 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/remove_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1879 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1465 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/set_dpa_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2389 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/set_hops.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2135 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/set_mid.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5293 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/smart_connect.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.515062 iqrfpy-0.1.8/iqrfpy/messages/requests/dali/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:18.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/dali/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.515062 iqrfpy-0.1.8/iqrfpy/messages/requests/eeeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/eeeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.515062 iqrfpy-0.1.8/iqrfpy/messages/requests/eeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:21.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/eeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.515062 iqrfpy-0.1.8/iqrfpy/messages/requests/exploration/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/exploration/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/requests/frc/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:40.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/frc/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/requests/generic/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/generic/Raw.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/generic/RawHdp.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/generic/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/requests/io/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:21.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/io/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2516 2023-04-19 05:31:16.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/irequest.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/requests/ledg/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:15.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/ledg/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/requests/ledr/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:11.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/ledr/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      971 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/ledr/flashing.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      959 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/ledr/pulse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      965 2023-04-18 08:55:28.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/ledr/set_off.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      961 2023-04-18 08:55:31.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/ledr/set_on.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/requests/light/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:37.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/light/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/requests/node/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:41:43.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/node/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      957 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/node/read.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/requests/os/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:14.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/os/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      947 2023-04-19 06:17:42.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/os/read.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/requests/ram/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:31.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/ram/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/requests/sensor/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:31.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/sensor/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/requests/thermometer/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:27.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/thermometer/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/requests/uart/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:32.000000 iqrfpy-0.1.8/iqrfpy/messages/requests/uart/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    12115 2023-04-19 05:44:49.000000 iqrfpy-0.1.8/iqrfpy/messages/response_factory.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      215 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2735 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/async_response.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/binaryoutput/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:04.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/binaryoutput/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2484 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/confirmation.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      996 2023-04-18 07:07:52.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2548 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/addr_info.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2659 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/authorize_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2468 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2582 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/bond_node.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/bonded_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2231 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/clear_all_bonds.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2627 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/discovered_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2475 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/discovery.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2480 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/remove_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2039 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2624 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/set_dpa_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2634 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/set_hops.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2033 2023-04-18 08:18:33.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/set_mid.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2650 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/smart_connect.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/dali/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:58.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/dali/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/eeeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:01.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/eeeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/eeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:56.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/eeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/exploration/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-04-15 05:56:54.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/exploration/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/frc/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:43.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/frc/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/generic/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-04-15 05:56:49.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/generic/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/io/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:27.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/io/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3277 2023-04-15 08:09:43.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/iresponse.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/ledg/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:23.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/ledg/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/ledr/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      244 2023-04-18 08:29:27.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/ledr/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2108 2023-04-19 05:44:14.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/ledr/flashing.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2084 2023-04-18 08:13:48.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/ledr/pulse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2094 2023-04-18 08:55:48.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/ledr/set_off.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2086 2023-04-18 08:55:48.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/ledr/set_on.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/light/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:14.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/light/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/node/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:49.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/node/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2579 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/node/read.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/os/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:52.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/os/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4879 2023-04-19 09:56:21.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/os/read.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/ram/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:05.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/ram/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/sensor/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:09.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/sensor/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/thermometer/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:32.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/thermometer/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/messages/responses/uart/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:37.000000 iqrfpy-0.1.8/iqrfpy/messages/responses/uart/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/transports/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      300 2023-03-22 19:16:00.000000 iqrfpy-0.1.8/iqrfpy/transports/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2414 2023-04-19 11:27:33.000000 iqrfpy-0.1.8/iqrfpy/transports/itransport.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3741 2023-04-19 11:26:32.000000 iqrfpy-0.1.8/iqrfpy/transports/mqtt_transport.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3788 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/iqrfpy/transports/udp_transport.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/iqrfpy/utils/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       50 2023-03-24 11:33:36.000000 iqrfpy-0.1.8/iqrfpy/utils/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    20492 2023-04-15 08:13:29.000000 iqrfpy-0.1.8/iqrfpy/utils/common.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1810 2023-04-15 07:47:59.000000 iqrfpy-0.1.8/iqrfpy/utils/dpa.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      343 2023-04-15 06:15:47.000000 iqrfpy-0.1.8/iqrfpy/utils/enums.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.515062 iqrfpy-0.1.8/iqrfpy.egg-info/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-19 11:31:25.000000 iqrfpy-0.1.8/iqrfpy.egg-info/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     7050 2023-04-19 11:31:25.000000 iqrfpy-0.1.8/iqrfpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2023-04-19 11:31:25.000000 iqrfpy-0.1.8/iqrfpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      159 2023-04-19 11:31:25.000000 iqrfpy-0.1.8/iqrfpy.egg-info/requires.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2023-04-19 11:31:25.000000 iqrfpy-0.1.8/iqrfpy.egg-info/top_level.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      138 2023-03-24 09:25:00.000000 iqrfpy-0.1.8/pyproject.toml
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       85 2023-03-24 07:40:43.000000 iqrfpy-0.1.8/requirements.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1162 2023-04-19 11:31:25.523062 iqrfpy-0.1.8/setup.cfg
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2104 2023-04-19 10:05:41.000000 iqrfpy-0.1.8/test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      102 2023-03-22 19:16:00.000000 iqrfpy-0.1.8/test_requirements.txt
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/tests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-07 12:49:34.000000 iqrfpy-0.1.8/tests/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/tests/enums/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1241 2023-03-24 10:31:41.000000 iqrfpy-0.1.8/tests/enums/peripherals_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/tests/messages/
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.519062 iqrfpy-0.1.8/tests/messages/requests/
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.523062 iqrfpy-0.1.8/tests/messages/requests/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      870 2023-04-18 07:02:34.000000 iqrfpy-0.1.8/tests/messages/requests/coordinator/addr_info_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3893 2023-04-18 07:14:42.000000 iqrfpy-0.1.8/tests/messages/requests/coordinator/authorize_bond_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2194 2023-04-18 07:02:34.000000 iqrfpy-0.1.8/tests/messages/requests/coordinator/backup_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3759 2023-04-18 07:02:54.000000 iqrfpy-0.1.8/tests/messages/requests/coordinator/bond_node_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      904 2023-04-18 07:02:54.000000 iqrfpy-0.1.8/tests/messages/requests/coordinator/bonded_devices_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      906 2023-04-18 07:02:54.000000 iqrfpy-0.1.8/tests/messages/requests/coordinator/clear_all_bonds_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      926 2023-04-18 07:04:34.000000 iqrfpy-0.1.8/tests/messages/requests/coordinator/discovered_devices_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3445 2023-04-18 07:04:34.000000 iqrfpy-0.1.8/tests/messages/requests/coordinator/discovery_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2323 2023-04-18 07:04:34.000000 iqrfpy-0.1.8/tests/messages/requests/coordinator/remove_bond_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4241 2023-04-18 07:04:34.000000 iqrfpy-0.1.8/tests/messages/requests/coordinator/restore_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2259 2023-04-18 07:04:34.000000 iqrfpy-0.1.8/tests/messages/requests/coordinator/set_dpa_params_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3673 2023-04-18 07:04:34.000000 iqrfpy-0.1.8/tests/messages/requests/coordinator/set_hops_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3512 2023-04-18 07:04:34.000000 iqrfpy-0.1.8/tests/messages/requests/coordinator/set_mid_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    11031 2023-04-18 07:04:34.000000 iqrfpy-0.1.8/tests/messages/requests/coordinator/smart_connect_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1293 2023-04-18 07:06:09.000000 iqrfpy-0.1.8/tests/messages/requests/irequest_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.523062 iqrfpy-0.1.8/tests/messages/requests/ledr/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      860 2023-04-19 05:58:57.000000 iqrfpy-0.1.8/tests/messages/requests/ledr/flashing_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      842 2023-04-19 05:57:37.000000 iqrfpy-0.1.8/tests/messages/requests/ledr/pulse_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      849 2023-04-19 05:56:05.000000 iqrfpy-0.1.8/tests/messages/requests/ledr/set_off_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      843 2023-04-19 05:29:51.000000 iqrfpy-0.1.8/tests/messages/requests/ledr/set_on_request_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.523062 iqrfpy-0.1.8/tests/messages/requests/os/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      835 2023-04-19 06:19:40.000000 iqrfpy-0.1.8/tests/messages/requests/os/read_request_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4828 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/tests/messages/response_factory_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.523062 iqrfpy-0.1.8/tests/messages/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2163 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/tests/messages/responses/async_response_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1280 2023-04-18 07:05:26.000000 iqrfpy-0.1.8/tests/messages/responses/confirmation_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.523062 iqrfpy-0.1.8/tests/messages/responses/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4326 2023-04-18 07:06:09.000000 iqrfpy-0.1.8/tests/messages/responses/coordinator/addr_info_response_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4515 2023-04-18 07:06:09.000000 iqrfpy-0.1.8/tests/messages/responses/coordinator/authorize_bond_response_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4765 2023-04-18 07:06:09.000000 iqrfpy-0.1.8/tests/messages/responses/coordinator/backup_response_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4392 2023-04-18 07:06:51.000000 iqrfpy-0.1.8/tests/messages/responses/coordinator/bond_node_response_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4213 2023-04-18 07:06:21.000000 iqrfpy-0.1.8/tests/messages/responses/coordinator/bonded_devices_response_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3157 2023-04-18 07:06:51.000000 iqrfpy-0.1.8/tests/messages/responses/coordinator/clear_all_bonds_response_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4345 2023-04-18 07:07:52.000000 iqrfpy-0.1.8/tests/messages/responses/coordinator/discovered_devices_response_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3785 2023-04-18 07:07:52.000000 iqrfpy-0.1.8/tests/messages/responses/coordinator/discovery_response_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3796 2023-04-18 07:07:52.000000 iqrfpy-0.1.8/tests/messages/responses/coordinator/remove_node_response_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3055 2023-04-18 07:07:52.000000 iqrfpy-0.1.8/tests/messages/responses/coordinator/restore_response_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3933 2023-04-18 07:07:52.000000 iqrfpy-0.1.8/tests/messages/responses/coordinator/set_dpa_params_response_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4492 2023-04-18 07:07:52.000000 iqrfpy-0.1.8/tests/messages/responses/coordinator/set_hops_response_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3054 2023-04-18 07:07:52.000000 iqrfpy-0.1.8/tests/messages/responses/coordinator/set_mid_response_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4488 2023-04-18 07:07:52.000000 iqrfpy-0.1.8/tests/messages/responses/coordinator/smart_connect_response_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.523062 iqrfpy-0.1.8/tests/messages/responses/os/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4173 2023-04-19 09:43:38.000000 iqrfpy-0.1.8/tests/messages/responses/os/read_response_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-19 11:31:25.523062 iqrfpy-0.1.8/tests/utils/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    16223 2023-04-15 05:36:55.000000 iqrfpy-0.1.8/tests/utils/common_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       78 2023-03-22 19:16:00.000000 iqrfpy-0.1.8/tox.ini
```

### Comparing `iqrfpy-0.1.7/.gitlab-ci.yml` & `iqrfpy-0.1.8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.7/LICENSE` & `iqrfpy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.7/Makefile` & `iqrfpy-0.1.8/Makefile`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.7/PKG-INFO` & `iqrfpy-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqrfpy
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python library for communication with IQRF Network
 Home-page: https://gitlab.iqrf.org/microrisc/libiqrf-python
 Author: Karel Hanák
 Author-email: karel.hanak@iqrf.org
 License: Apache-2.0
 Keywords: iqrf,dpa
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iqrfpy-0.1.7/examples/response_factories.py` & `iqrfpy-0.1.8/examples/response_factories.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from iqrfpy.messages.requests.coordinator import AuthorizeBondRequest
 from iqrfpy.messages.responses.coordinator import *
 from iqrfpy.messages.response_factory import ResponseFactory
 
 
 def handle_addr_info_response(response: AddrInfoResponse) -> None:
     print(f'peripheral: {response.get_pnum()}')
     print(f'peripheral command: {response.get_pcmd()}')
```

### Comparing `iqrfpy-0.1.7/iqrfpy/enums/message_types.py` & `iqrfpy-0.1.8/iqrfpy/enums/message_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,33 +27,47 @@
     'BinaryOutputMessages',
     'SensorMessages',
     'LightMessages'
 ]
 
 
 class MessageType(enum.Enum):
+    """JSON API message type base enum."""
+
     pass
 
     @classmethod
     def has_value(cls, value):
+        """
+        Check if enum class has member value.
+
+        :param value: value to check
+        :return: True if value is a member of enum, False otherwise
+        """
         return value in cls._value2member_map_
 
 
 class GenericMessages(MessageType):
+    """Generic message types enum."""
+
     RAW = 'iqrfRaw'
     RAW_HDP = 'iqrfRawHdp'
 
 
 class ExplorationMessages(MessageType):
+    """Exploration message types enum."""
+
     ENUMERATE = 'iqrfEmbedExplore_Enumerate'
     PERIPHERAL_INFORMATION = 'iqrfEmbedExplore_PeripheralInformation'
     MORE_PERIPHERALS_INFORMATION = 'iqrfEmbedExplore_MorePeripheralsInformation'
 
 
 class CoordinatorMessages(MessageType):
+    """Coordinator message types enum."""
+
     ADDR_INFO = 'iqrfEmbedCoordinator_AddrInfo'
     DISCOVERED_DEVICES = 'iqrfEmbedCoordinator_DiscoveredDevices'
     BONDED_DEVICES = 'iqrfEmbedCoordinator_BondedDevices'
     CLEAR_ALL_BONDS = 'iqrfEmbedCoordinator_ClearAllBonds'
     BOND_NODE = 'iqrfEmbedCoordinator_BondNode'
     REMOVE_BOND = 'iqrfEmbedCoordinator_RemoveBond'
     DISCOVERY = 'iqrfEmbedCoordinator_Discovery'
@@ -63,22 +77,26 @@
     RESTORE = 'iqrfEmbedCoordinator_Restore'
     AUTHORIZE_BOND = 'iqrfEmbedCoordinator_AuthorizeBond'
     SMART_CONNECT = 'iqrfEmbedCoordinator_SmartConnect'
     SET_MID = 'iqrfEmbedCoordinator_SetMID'
 
 
 class NodeMessages(MessageType):
+    """Node message types enum."""
+
     READ = 'iqrfEmbedNode_Read'
     REMOVE_BOND = 'iqrfEmbedNode_RemoveBond'
     BACKUP = 'iqrfEmbedNode_Backup'
     RESTORE = 'iqrfEmbedNode_Restore'
     VALIDATE_BONDS = 'iqrfEmbedNode_ValidateBonds'
 
 
 class OSMessages(MessageType):
+    """OS message types enum."""
+
     READ = 'iqrfEmbedOs_Read'
     RESET = 'iqrfEmbedOs_Reset'
     READ_CFG = 'iqrfEmbedOs_ReadCfg'
     RFPGM = 'iqrfEmbedOs_Rfpgm'
     SLEEP = 'iqrfEmbedOs_Sleep'
     BATCH = 'iqrfEmbedOs_Batch'
     SET_SECURITY = 'iqrfEmbedOs_SetSecurity'
@@ -89,81 +107,107 @@
     SELECTIVE_BATCH = 'iqrfEmbedOs_SelectiveBatch'
     TEST_RF_SIGNAL = 'iqrfEmbedOs_TestRfSignal'
     FACTORY_SETTINGS = 'iqrfEmbedOs_FactorySettings'
     WRITE_CFG = 'iqrfEmbedOs_WriteCfg'
 
 
 class RAMMessages(MessageType):
+    """RAM message types enum."""
+
     READ = 'iqrfEmbedRam_Read'
     WRITE = 'iqrfEmbedRam_Write'
 
 
 class EEPROMMessages(MessageType):
+    """EEPROM message types enum."""
+
     READ = 'iqrfEmbedEeprom_Read'
     WRITE = 'iqrfEmbedEeprom_Write'
 
 
 class EEEPROMMessages(MessageType):
+    """EEEPROM message types enum."""
+
     READ = 'iqrfEmbedEeeprom_Read'
     WRITE = 'iqrfEmbedEeeprom_Write'
 
 
 class LEDRMessages(MessageType):
-    SET = 'iqrfEmbedLedr_Set'
-    GET = 'iqrfEmbedLedr_Get'
+    """LEDR message types enum."""
+
+    SET_ON = 'iqrfEmbedLedr_SetOn'
+    SET_OFF = 'iqrfEmbedLedr_SetOff'
     PULSE = 'iqrfEmbedLedr_Pulse'
     FLASHING = 'iqrfEmbedLedr_Flashing'
 
 
 class LEDGMessages(MessageType):
+    """LEDG message types enum."""
+
     SET = 'iqrfEmbedLedg_Set'
     GET = 'iqrfEmbedLedg_Get'
     PULSE = 'iqrfEmbedLedg_Pulse'
     FLASHING = 'iqrfEmbedLedg_Flashing'
 
 
 class IOMessages(MessageType):
+    """IO message types enum."""
+
     DIRECTION = 'iqrfEmbedIo_Direction'
     SET = 'iqrfEmbedIo_Set'
     GET = 'iqrfEmbedIo_Get'
 
 
 class ThermometerMessages(MessageType):
+    """READ message types enum."""
+
     READ = 'iqrfEmbedThermometer_Read'
 
 
 class UartMessages(MessageType):
+    """Uart message types enum."""
+
     OPEN = 'iqrfEmbedUart_Open'
     CLOSE = 'iqrfEmbedUart_Close'
     WRITE_READ = 'iqrfEmbedUart_WriteRead'
     CLEAR_WRITE_READ = 'iqrfEmbedUart_ClearWriteRead'
 
 
 class FrcMessages(MessageType):
+    """FRC message types enum."""
+
     SEND = 'iqrfEmbedFrc_Send'
     EXTRA_RESULT = 'iqrfEmbedFrc_ExtraResult'
     SEND_SELECTIVE = 'iqrfEmbedFrc_SendSelective'
     SET_PARAMS = 'iqrfEmbedFrc_SetParams'
 
 
 class DALIMessages(MessageType):
+    """DALI message types enum."""
+
     SEND_COMMANDS = 'iqrfDali_SendCommands'
     SEND_COMMANDS_ASYNC = 'iqrfDali_SendCommandsAsync'
     FRC = 'iqrfDali_Frc'
 
 
 class BinaryOutputMessages(MessageType):
+    """BinaryOutput message types enum."""
+
     SET_OUTPUT = 'iqrfBinaryOutput_SetOutput'
     ENUMERATE = 'iqrfBinaryOutput_Enumerate'
 
 
 class SensorMessages(MessageType):
+    """Sensor message types enum."""
+
     READ_SENSORS_WITH_TYPES = 'iqrfSensor_ReadSensorsWithTypes'
     ENUMERATE = 'iqrfSensor_Enumerate'
     FRC = 'iqrfSensor_Frc'
 
 
 class LightMessages(MessageType):
+    """Light message types enum."""
+
     SET_POWER = 'iqrfLight_SetPower'
     INCREMENT_POWER = 'iqrfLight_IncrementPower'
     DECREMENT_POWER = 'iqrfLight_DecrementPower'
     ENUMERATE = 'iqrfLight_Enumerate'
```

### Comparing `iqrfpy-0.1.7/iqrfpy/enums/peripherals.py` & `iqrfpy-0.1.8/iqrfpy/enums/peripherals.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,23 +5,20 @@
 These enums are extended with has_value() method for member identification.
 """
 
 from ..utils.enums import IntEnumMember
 
 
 class Peripheral(IntEnumMember):
-    """
-    Base peripherals enum class.
-    """
+    """Base peripherals enum class."""
 
 
 class EmbedPeripherals(Peripheral):
-    """
-    Embedded peripherals enum.
-    """
+    """Embedded peripherals enum."""
+
     COORDINATOR = 0
     NODE = 1
     OS = 2
     EEPROM = 3
     EEEPROM = 4
     RAM = 5
     LEDR = 6
@@ -30,14 +27,13 @@
     THERMOMETER = 10
     UART = 12
     FRC = 13
     EXPLORATION = 255
 
 
 class Standards(Peripheral):
-    """
-    Standards enum.
-    """
+    """Standards peripherals enum."""
+
     DALI = 74
     BINARY_OUTPUT = 75
     SENSOR = 94
     LIGHT = 113
```

### Comparing `iqrfpy-0.1.7/iqrfpy/exceptions.py` & `iqrfpy-0.1.8/iqrfpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/IRequest.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/irequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 @typechecked
 class IRequest(ABC):
     __slots__ = '_nadr', '_pnum', '_pcmd', '_m_type', '_hwpid', '_pdata', '_msgid', '_params'
 
     def __init__(self, nadr: int, pnum: Peripheral, pcmd: Command, hwpid: int = DpaConstants.HWPID_MAX,
                  pdata: Optional[List[int]] = None, m_type: Optional[MessageType] = None, params: Optional[dict] = None,
                  msgid: str = str(uuid4())):
+
         self._nadr: int = nadr
         self._pnum: Peripheral = pnum
         self._pcmd: Command = pcmd
         self._hwpid: int = hwpid
         self._pdata: Optional[List[int]] = pdata
         self._m_type: Optional[str] = m_type.value if m_type is not None else m_type
         self._msgid: str = msgid
@@ -31,18 +32,21 @@
 
     def _validate_base(self) -> None:
         if self._nadr < DpaConstants.NADR_MIN or self._nadr > DpaConstants.NADR_MAX:
             raise RequestNadrInvalidError('NADR should be between 0 and 239.')
         if self._hwpid < DpaConstants.HWPID_MIN or self._hwpid > DpaConstants.HWPID_MAX:
             raise RequestHwpidInvalidError('HWPID should be between 0 and 65535.')
 
+    def get_msg_id(self) -> str:
+        return self._msgid
+
     @abstractmethod
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
         self._validate_base()
-        dpa: List[int] = [0, self._nadr, self._pnum, self._pcmd, self._hwpid & 0xFF, (self._hwpid >> 8) & 0xFF]
+        dpa: List[int] = [self._nadr, 0, self._pnum, self._pcmd, self._hwpid & 0xFF, (self._hwpid >> 8) & 0xFF]
         if self._pdata is not None:
             dpa.extend(self._pdata)
         if mutable:
             return bytearray(dpa)
         return bytes(dpa)
 
     @abstractmethod
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/AddrInfo.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/addr_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.commands import CoordinatorRequestCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
 __all__ = ['AddrInfoRequest']
 
 
 @typechecked
 class AddrInfoRequest(IRequest):
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/AuthorizeBond.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/authorize_bond.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,66 +4,67 @@
 from uuid import uuid4
 from typing import List, Union
 from iqrfpy.enums.commands import CoordinatorRequestCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
 __all__ = ['AuthorizeBondRequest', 'AuthorizeBondParams']
 
 
 @dataclass(slots=True)
 @typechecked
 class AuthorizeBondParams:
     reqAddr: int
     mid: int
 
+    def __post_init__(self):
+        if self.reqAddr < DpaConstants.NODE_NADR_MIN or self.reqAddr > DpaConstants.NODE_NADR_MAX:
+            raise RequestParameterInvalidValueError('Requested address value should be between 1 and 239.')
+        if self.mid < DpaConstants.MID_MIN or self.mid > DpaConstants.MID_MAX:
+            raise RequestParameterInvalidValueError('MID value should be an unsigned 32bit integer.')
+
 
 @typechecked
 class AuthorizeBondRequest(IRequest):
 
     __slots__ = '_nodes'
 
     def __init__(self, nodes: List[AuthorizeBondParams], hwpid: int = DpaConstants.HWPID_MAX, msgid: str = str(uuid4())):
+        self._validate(nodes)
         super().__init__(
             nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorRequestCommands.AUTHORIZE_BOND,
             m_type=CoordinatorMessages.AUTHORIZE_BOND,
             hwpid=hwpid,
             msgid=msgid
         ),
         self._nodes: List[AuthorizeBondParams] = nodes
-        self._validate()
 
-    def _validate(self) -> None:
-        if len(self._nodes) == 0:
+    @staticmethod
+    def _validate(nodes: List[AuthorizeBondParams]) -> None:
+        if len(nodes) == 0:
             raise RequestParameterInvalidValueError('At least one pair of requested address and MID is required.')
-        if len(self._nodes) > 11:
+        if len(nodes) > 11:
             raise RequestParameterInvalidValueError('Request can carry at most 11 pairs of address and MID.')
-        for node in self._nodes:
-            if node.reqAddr < DpaConstants.NODE_NADR_MIN or node.reqAddr > DpaConstants.NODE_NADR_MAX:
-                raise RequestParameterInvalidValueError('Requested address value should be between 1 and 239.')
-            if node.mid < DpaConstants.MID_MIN or node.mid > DpaConstants.MID_MAX:
-                raise RequestParameterInvalidValueError('MID value should be an unsigned 32bit integer.')
 
     def set_nodes(self, nodes: List[AuthorizeBondParams]) -> None:
+        self._validate(nodes)
         self._nodes = nodes
 
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
-        self._validate()
         pdata = []
         for node in self._nodes:
             pdata.append(node.reqAddr)
             pdata.append(node.mid & 0xFF)
             pdata.append((node.mid >> 8) & 0xFF)
             pdata.append((node.mid >> 16) & 0xFF)
             pdata.append((node.mid >> 24) & 0xFF)
         self._pdata = pdata
         return super().to_dpa(mutable=mutable)
 
     def to_json(self) -> dict:
-        self._validate()
         self._params = {'nodes': [{'reqAddr': node.reqAddr, 'mid': node.mid} for node in self._nodes]}
         return super().to_json()
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/Backup.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.commands import CoordinatorRequestCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
 __all__ = ['BackupRequest']
 
 
 @typechecked
 class BackupRequest(IRequest):
     __slots__ = '_index'
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/BondNode.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/bond_node.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.commands import CoordinatorRequestCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
 __all__ = ['BondNodeRequest']
 
 
 @typechecked
 class BondNodeRequest(IRequest):
     __slots__ = '_req_addr', '_bonding_test_retries'
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/BondedDevices.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/bonded_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.commands import CoordinatorRequestCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
 __all__ = ['BondedDevicesRequest']
 
 
 @typechecked
 class BondedDevicesRequest(IRequest):
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/ClearAllBonds.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/clear_all_bonds.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.commands import CoordinatorRequestCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
 __all__ = ['ClearAllBondsRequest']
 
 
 @typechecked
 class ClearAllBondsRequest(IRequest):
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/DiscoveredDevices.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/discovered_devices.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.commands import CoordinatorRequestCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
 __all__ = ['DiscoveredDevicesRequest']
 
 
 @typechecked
 class DiscoveredDevicesRequest(IRequest):
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/Discovery.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.commands import CoordinatorRequestCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
 __all__ = ['DiscoveryRequest']
 
 
 @typechecked
 class DiscoveryRequest(IRequest):
     __slots__ = '_tx_power', '_max_addr'
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/RemoveBond.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/remove_bond.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.commands import CoordinatorRequestCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
 __all__ = ['RemoveBondRequest']
 
 
 @typechecked
 class RemoveBondRequest(IRequest):
     __slots__ = '_bond_addr'
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/Restore.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/restore.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List, Union
 from iqrfpy.enums.commands import CoordinatorRequestCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
 __all__ = ['RestoreRequest']
 
 
 @typechecked
 class RestoreRequest(IRequest):
     __slots__ = '_network_data'
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SetDpaParams.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/set_dpa_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from enum import IntEnum
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.commands import CoordinatorRequestCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
 __all__ = ['SetDpaParamsRequest', 'DpaParam']
 
 
 @typechecked
 class DpaParam(IntEnum):
     LAST_RSSI = 0
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SetHops.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/set_hops.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.commands import CoordinatorRequestCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
 __all__ = ['SetHopsRequest']
 
 REQUEST_HOPS_DRM = 0
 REQUEST_HOPS_DOM = 0xFF
 RESPONSE_HOPS_DOM = 0xFF
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SetMID.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/set_mid.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.commands import CoordinatorRequestCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
 __all__ = ['SetMIDRequest']
 
 
 @typechecked
 class SetMIDRequest(IRequest):
     __slots__ = '_bond_addr', '_mid'
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SmartConnect.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/smart_connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List, Union
 from iqrfpy.enums.commands import CoordinatorRequestCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
 __all__ = ['SmartConnectRequest']
 
 
 @typechecked
 class SmartConnectRequest(IRequest):
     __slots__ = '_req_addr', '_bonding_test_retries', '_ibk', '_mid', '_virtual_device_address'
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/__init__.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/coordinator/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from .AddrInfo import AddrInfoRequest
-from .AuthorizeBond import AuthorizeBondRequest
-from .Backup import BackupRequest
-from .BondedDevices import BondedDevicesRequest
-from .BondNode import BondNodeRequest
-from .ClearAllBonds import ClearAllBondsRequest
-from .DiscoveredDevices import DiscoveredDevicesRequest
-from .Discovery import DiscoveryRequest
-from .RemoveBond import RemoveBondRequest
-from .Restore import RestoreRequest
-from .SetDpaParams import SetDpaParamsRequest
-from .SetHops import SetHopsRequest
-from .SetMID import SetMIDRequest
-from .SmartConnect import SmartConnectRequest
+from .addr_info import AddrInfoRequest
+from .authorize_bond import AuthorizeBondRequest
+from .backup import BackupRequest
+from .bonded_devices import BondedDevicesRequest
+from .bond_node import BondNodeRequest
+from .clear_all_bonds import ClearAllBondsRequest
+from .discovered_devices import DiscoveredDevicesRequest
+from .discovery import DiscoveryRequest
+from .remove_bond import RemoveBondRequest
+from .restore import RestoreRequest
+from .set_dpa_params import SetDpaParamsRequest
+from .set_hops import SetHopsRequest
+from .set_mid import SetMIDRequest
+from .smart_connect import SmartConnectRequest
 
 __all__ = [
     'AddrInfoRequest',
     'AuthorizeBondRequest',
     'BackupRequest',
     'BondedDevicesRequest',
     'BondNodeRequest',
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/requests/node/Read.py` & `iqrfpy-0.1.8/iqrfpy/messages/requests/ledr/set_off.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
-from iqrfpy.enums.commands import NodeRequestCommands
-from iqrfpy.enums.message_types import NodeMessages
+from iqrfpy.enums.commands import LEDRequestCommands
+from iqrfpy.enums.message_types import LEDRMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.messages.requests.IRequest import IRequest
+from iqrfpy.messages.requests.irequest import IRequest
 
-__all__ = ['ReadRequest']
+__all__ = ['SetOffRequest']
 
 
 @typechecked
-class ReadRequest(IRequest):
+class SetOffRequest(IRequest):
 
     def __init__(self, nadr: int, hwpid: int = DpaConstants.HWPID_MAX, msgid: str = str(uuid4())):
         super().__init__(
             nadr=nadr,
-            pnum=EmbedPeripherals.NODE,
-            pcmd=NodeRequestCommands.READ,
-            m_type=NodeMessages.READ,
+            pnum=EmbedPeripherals.LEDR,
+            pcmd=LEDRequestCommands.SET_OFF,
+            m_type=LEDRMessages.SET_OFF,
             hwpid=hwpid,
             msgid=msgid
         )
 
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
         return super().to_dpa(mutable=mutable)
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/response_factory.py` & `iqrfpy-0.1.8/iqrfpy/messages/response_factory.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from abc import ABC, abstractmethod
+from typing import Union
+from ..enums.commands import *
 from ..enums.message_types import *
-from .responses.AsyncResponse import AsyncResponse
-from .responses.Confirmation import Confirmation
-from .responses.IResponse import IResponse
+from ..enums.peripherals import *
+from .responses.async_response import AsyncResponse
+from .responses.confirmation import Confirmation
+from .responses.iresponse import IResponse
 from .responses.coordinator import *
+import iqrfpy.messages.responses.ledr as LedrResponses
 from ..utils.common import Common
 from ..utils.dpa import *
-from ..exceptions import UnsupportedMessageTypeError
+from ..exceptions import UnsupportedMessageTypeError, UnsupportedPeripheralError, UnsupportedPeripheralCommandError
 
 __all__ = [
     'ResponseFactory',
     '_get_factory_from_mtype',
     'AsyncResponseFactory',
     'ConfirmationFactory',
     'CoordinatorAddrInfoFactory',
@@ -39,16 +43,17 @@
         pcmd = dpa[ResponsePacketMembers.PCMD]
         rcode = dpa[ResponsePacketMembers.RCODE]
         if rcode == CONFIRMATION_RCODE and len(dpa) == CONFIRMATION_PACKET_LEN:
             factory = ConfirmationFactory()
         elif pcmd <= REQUEST_PCMD_MAX and rcode >= ASYNC_RESPONSE_CODE:
             factory = AsyncResponseFactory()
         else:
-            mtype = Common.mtype_from_dpa_response(pnum, pcmd)
-            factory = _get_factory_from_mtype(mtype)
+            peripheral = Common.pnum_from_dpa(pnum)
+            command = Common.response_pcmd_from_dpa(peripheral, pcmd)
+            factory = _get_factory_from_dpa(peripheral, command)
         return factory.create_from_dpa(dpa)
 
     @staticmethod
     def get_response_from_json(json: dict) -> IResponse:
         msgid = Common.msgid_from_json(json)
         mtype = Common.mtype_str_from_json(json)
         if msgid == IResponse.ASYNC_MSGID and \
@@ -66,14 +71,16 @@
     def create_from_dpa(self, dpa: bytes) -> IResponse:
         """Returns a response object created from DPA message."""
 
     @abstractmethod
     def create_from_json(self, json: dict) -> IResponse:
         """Returns a response object created from JSON API message."""
 
+# Coordinator factories
+
 
 class ConfirmationFactory(BaseFactory):
     def create_from_dpa(self, dpa: bytes) -> Confirmation:
         return Confirmation.from_dpa(dpa=dpa)
 
     def create_from_json(self, json: dict) -> Confirmation:
         return Confirmation.from_json(json=json)
@@ -198,14 +205,85 @@
     def create_from_dpa(self, dpa: bytes) -> SmartConnectResponse:
         return SmartConnectResponse.from_dpa(dpa=dpa)
 
     def create_from_json(self, json: dict) -> SmartConnectResponse:
         return SmartConnectResponse.from_json(json=json)
 
 
+# LEDR factories
+
+
+class LedrSetOnFactory(BaseFactory):
+
+    def create_from_dpa(self, dpa: bytes) -> LedrResponses.SetOnResponse:
+        return LedrResponses.SetOnResponse.from_dpa(dpa)
+
+    def create_from_json(self, json: dict) -> LedrResponses.SetOnResponse:
+        return LedrResponses.SetOnResponse.from_json(json)
+
+
+class LedrSetOffFactory(BaseFactory):
+
+    def create_from_dpa(self, dpa: bytes) -> LedrResponses.SetOffResponse:
+        return LedrResponses.SetOffResponse.from_dpa(dpa)
+
+    def create_from_json(self, json: dict) -> LedrResponses.SetOffResponse:
+        return LedrResponses.SetOffResponse.from_json(json)
+
+
+class LedrPulseFactory(BaseFactory):
+
+    def create_from_dpa(self, dpa: bytes) -> LedrResponses.PulseResponse:
+        return LedrResponses.PulseResponse.from_dpa(dpa=dpa)
+
+    def create_from_json(self, json: dict) -> LedrResponses.PulseResponse:
+        return LedrResponses.PulseResponse.from_json(json=json)
+
+
+class LedrFlashingFactory(BaseFactory):
+
+    def create_from_dpa(self, dpa: bytes) -> LedrResponses.FlashingResponse:
+        return LedrResponses.FlashingResponse.from_dpa(dpa=dpa)
+
+    def create_from_json(self, json: dict) -> LedrResponses.FlashingResponse:
+        return LedrResponses.FlashingResponse.from_json(json=json)
+
+
+def _get_factory_from_dpa(pnum: Union[EmbedPeripherals, Standards], pcmd: Command) -> BaseFactory:
+    factories = {
+        EmbedPeripherals.COORDINATOR: {
+            CoordinatorResponseCommands.ADDR_INFO: CoordinatorAddrInfoFactory(),
+            CoordinatorResponseCommands.AUTHORIZE_BOND: CoordinatorAuthorizeBondFactory(),
+            CoordinatorResponseCommands.BACKUP: CoordinatorBackupFactory(),
+            CoordinatorResponseCommands.BONDED_DEVICES: CoordinatorBondedDevicesFactory(),
+            CoordinatorResponseCommands.BOND_NODE: CoordinatorBondNodeFactory(),
+            CoordinatorResponseCommands.CLEAR_ALL_BONDS: CoordinatorClearAllBondsFactory(),
+            CoordinatorResponseCommands.DISCOVERED_DEVICES: CoordinatorDiscoveredDevicesFactory(),
+            CoordinatorResponseCommands.DISCOVERY: CoordinatorDiscoveryFactory(),
+            CoordinatorResponseCommands.REMOVE_BOND: CoordinatorRemoveBondFactory(),
+            CoordinatorResponseCommands.RESTORE: CoordinatorRestoreFactory(),
+            CoordinatorResponseCommands.SET_DPA_PARAMS: CoordinatorSetDpaParamsFactory(),
+            CoordinatorResponseCommands.SET_HOPS: CoordinatorSetHopsFactory(),
+            CoordinatorResponseCommands.SET_MID: CoordinatorSetMIDFactory(),
+            CoordinatorResponseCommands.SMART_CONNECT: CoordinatorSmartConnectFactory(),
+        },
+        EmbedPeripherals.LEDR: {
+            LEDResponseCommands.SET_ON: LedrSetOnFactory(),
+            LEDResponseCommands.SET_OFF: LedrSetOffFactory(),
+            LEDResponseCommands.PULSE: LedrPulseFactory(),
+            LEDResponseCommands.FLASHING: LedrFlashingFactory(),
+        }
+    }
+    if pnum in factories:
+        if pcmd in factories[pnum]:
+            return factories[pnum][pcmd]
+        raise UnsupportedPeripheralCommandError(f'Unknown or unsupported peripheral command: {pcmd}')
+    raise UnsupportedPeripheralError(f'Unknown or unsupported peripheral: {pnum}')
+
+
 def _get_factory_from_mtype(mtype: MessageType) -> BaseFactory:
     factories = {
         CoordinatorMessages.ADDR_INFO: CoordinatorAddrInfoFactory(),
         CoordinatorMessages.AUTHORIZE_BOND: CoordinatorAuthorizeBondFactory(),
         CoordinatorMessages.BACKUP: CoordinatorBackupFactory(),
         CoordinatorMessages.BONDED_DEVICES: CoordinatorBondedDevicesFactory(),
         CoordinatorMessages.BOND_NODE: CoordinatorBondNodeFactory(),
@@ -214,12 +292,16 @@
         CoordinatorMessages.DISCOVERY: CoordinatorDiscoveryFactory(),
         CoordinatorMessages.REMOVE_BOND: CoordinatorRemoveBondFactory(),
         CoordinatorMessages.RESTORE: CoordinatorRestoreFactory(),
         CoordinatorMessages.SET_DPA_PARAMS: CoordinatorSetDpaParamsFactory(),
         CoordinatorMessages.SET_HOPS: CoordinatorSetHopsFactory(),
         CoordinatorMessages.SET_MID: CoordinatorSetMIDFactory(),
         CoordinatorMessages.SMART_CONNECT: CoordinatorSmartConnectFactory(),
+        LEDRMessages.SET_ON: LedrSetOnFactory(),
+        LEDRMessages.SET_OFF: LedrSetOffFactory(),
+        LEDRMessages.PULSE: LedrPulseFactory(),
+        LEDRMessages.FLASHING: LedrFlashingFactory(),
     }
 
     if mtype in factories:
         return factories[mtype]
     raise UnsupportedMessageTypeError(f'Unknown or unsupported message type: {mtype}')
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/AsyncResponse.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/async_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.enums.peripherals import Peripheral
 from iqrfpy.enums.commands import Command
 from iqrfpy.enums.message_types import GenericMessages
-from .IResponse import IResponse, IResponseGetterMixin
+from .iresponse import IResponse, IResponseGetterMixin
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponsePacketMembers
 
 __all__ = ['AsyncResponse']
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/Confirmation.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/confirmation.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 from iqrfpy.enums.commands import Command
 from iqrfpy.enums.peripherals import Peripheral
 from iqrfpy.exceptions import DpaConfirmationPacketError, DpaConfirmationPacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
-from iqrfpy.messages.responses.IResponse import IResponseGetterMixin
+from iqrfpy.messages.responses.iresponse import IResponseGetterMixin
 
 __all__ = ['Confirmation']
 
 
 class Confirmation(IResponseGetterMixin):
     __slots__ = '_request_hops', '_response_hops', '_timeslot'
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/IResponse.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/iresponse.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/AddrInfo.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/addr_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/AuthorizeBond.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/authorize_bond.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/Backup.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/smart_connect.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,63 @@
 from __future__ import annotations
 from typeguard import typechecked
-from typing import List, Optional
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from typing import Optional
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
 
-__all__ = ['BackupResponse']
+__all__ = ['SmartConnectResponse']
 
 
 @typechecked
-class BackupResponse(IResponseGetterMixin):
-    __slots__ = '_network_data'
+class SmartConnectResponse(IResponseGetterMixin):
+    __slots__ = '_bond_addr', '_dev_nr'
 
     def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
             nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.BACKUP,
-            m_type=CoordinatorMessages.BACKUP,
+            pcmd=CoordinatorResponseCommands.SMART_CONNECT,
+            m_type=CoordinatorMessages.SMART_CONNECT,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
         if rcode == ResponseCodes.OK:
-            self._network_data = result['networkData']
+            self._bond_addr = result['bondAddr']
+            self._dev_nr = result['devNr']
 
-    def get_network_data(self) -> List[int]:
-        return self._network_data
+    def get_bond_addr(self) -> int:
+        return self._bond_addr
+
+    def get_dev_nr(self) -> int:
+        return self._dev_nr
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> BackupResponse:
+    def from_dpa(dpa: bytes) -> SmartConnectResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
         rcode = dpa[ResponsePacketMembers.RCODE]
         result = None
         if rcode == ResponseCodes.OK:
-            if len(dpa) != 57:
+            if len(dpa) != 10:
                 raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'networkData': list(dpa[8:])}
-        return BackupResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], result=result)
+            result = {'bondAddr': dpa[8], 'devNr': dpa[9]}
+        return SmartConnectResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
+                                    result=result)
 
     @staticmethod
-    def from_json(json: dict) -> BackupResponse:
+    def from_json(json: dict) -> SmartConnectResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
         result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
-        return BackupResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+        return SmartConnectResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/BondNode.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/bond_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/BondedDevices.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/bonded_devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
 
 __all__ = ['BondedDevicesResponse']
 
 
 @typechecked
 class BondedDevicesResponse(IResponseGetterMixin):
     __slots__ = '_bonded'
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/ClearAllBonds.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/clear_all_bonds.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/DiscoveredDevices.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/discovered_devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
 
 __all__ = ['DiscoveredDevicesResponse']
 
 
 @typechecked
 class DiscoveredDevicesResponse(IResponseGetterMixin):
     __slots__ = '_discovered'
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/Discovery.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/discovery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/RemoveBond.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/remove_bond.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/Restore.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/restore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponsePacketMembers
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SetDpaParams.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/set_dpa_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
-from iqrfpy.messages.requests.coordinator.SetDpaParams import DpaParam
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
+from iqrfpy.messages.requests.coordinator.set_dpa_params import DpaParam
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SetHops.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/set_hops.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SetMID.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/set_mid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponsePacketMembers
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SmartConnect.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/backup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,58 @@
 from __future__ import annotations
 from typeguard import typechecked
-from typing import Optional
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from typing import List, Optional
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
 
-__all__ = ['SmartConnectResponse']
+__all__ = ['BackupResponse']
 
 
 @typechecked
-class SmartConnectResponse(IResponseGetterMixin):
-    __slots__ = '_bond_addr', '_dev_nr'
+class BackupResponse(IResponseGetterMixin):
+    __slots__ = '_network_data'
 
     def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
             nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.SMART_CONNECT,
-            m_type=CoordinatorMessages.SMART_CONNECT,
+            pcmd=CoordinatorResponseCommands.BACKUP,
+            m_type=CoordinatorMessages.BACKUP,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
         if rcode == ResponseCodes.OK:
-            self._bond_addr = result['bondAddr']
-            self._dev_nr = result['devNr']
+            self._network_data = result['networkData']
 
-    def get_bond_addr(self) -> int:
-        return self._bond_addr
-
-    def get_dev_nr(self) -> int:
-        return self._dev_nr
+    def get_network_data(self) -> List[int]:
+        return self._network_data
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> SmartConnectResponse:
+    def from_dpa(dpa: bytes) -> BackupResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
         rcode = dpa[ResponsePacketMembers.RCODE]
         result = None
         if rcode == ResponseCodes.OK:
-            if len(dpa) != 10:
+            if len(dpa) != 57:
                 raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'bondAddr': dpa[8], 'devNr': dpa[9]}
-        return SmartConnectResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
-                                    result=result)
+            result = {'networkData': list(dpa[8:])}
+        return BackupResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], result=result)
 
     @staticmethod
-    def from_json(json: dict) -> SmartConnectResponse:
+    def from_json(json: dict) -> BackupResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
         result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
-        return SmartConnectResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+        return BackupResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/__init__.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/coordinator/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from .AddrInfo import AddrInfoResponse
-from .AuthorizeBond import AuthorizeBondResponse
-from .Backup import BackupResponse
-from .BondedDevices import BondedDevicesResponse
-from .BondNode import BondNodeResponse
-from .ClearAllBonds import ClearAllBondsResponse
-from .DiscoveredDevices import DiscoveredDevicesResponse
-from .Discovery import DiscoveryResponse
-from .RemoveBond import RemoveBondResponse
-from .Restore import RestoreResponse
-from .SetDpaParams import SetDpaParamsResponse
-from .SetHops import SetHopsResponse
-from .SetMID import SetMIDResponse
-from .SmartConnect import SmartConnectResponse
+from .addr_info import AddrInfoResponse
+from .authorize_bond import AuthorizeBondResponse
+from .backup import BackupResponse
+from .bonded_devices import BondedDevicesResponse
+from .bond_node import BondNodeResponse
+from .clear_all_bonds import ClearAllBondsResponse
+from .discovered_devices import DiscoveredDevicesResponse
+from .discovery import DiscoveryResponse
+from .remove_bond import RemoveBondResponse
+from .restore import RestoreResponse
+from .set_dpa_params import SetDpaParamsResponse
+from .set_hops import SetHopsResponse
+from .set_mid import SetMIDResponse
+from .smart_connect import SmartConnectResponse
 
 __all__ = [
     'AddrInfoResponse',
     'AuthorizeBondResponse',
     'BackupResponse',
     'BondedDevicesResponse',
     'BondNodeResponse',
```

### Comparing `iqrfpy-0.1.7/iqrfpy/messages/responses/node/Read.py` & `iqrfpy-0.1.8/iqrfpy/messages/responses/node/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 from typing import Optional
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.commands import NodeResponseCommands
 from iqrfpy.enums.message_types import NodeMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 
 __all__ = ['ReadResponse']
```

### Comparing `iqrfpy-0.1.7/iqrfpy/transports/itransport.py` & `iqrfpy-0.1.8/iqrfpy/transports/itransport.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,34 @@
 """
 Transport abstract class.
 """
 from abc import ABC, abstractmethod
-from typing import Callable
-from iqrfpy.messages.requests.IRequest import IRequest
-from iqrfpy.messages.responses.IResponse import IResponse
-from iqrfpy.messages.responses.Confirmation import Confirmation
+from typing import Callable, Optional
+from iqrfpy.messages.requests.irequest import IRequest
+from iqrfpy.messages.responses.iresponse import IResponse
+from iqrfpy.messages.responses.confirmation import Confirmation
 
 
 class ITransport(ABC):
     """
     Abstract class providing interface for communication channels.
-
-    Methods
-    -------
-    initialize() -> None:
-        Initializes transport and creates connection if applicable.
-    send(request: IRequest) -> None:
-        Serialize passed request to format acceptable by the communication channel and send request.
-    receive() -> IResponse:
-        Receive a response synchronously, deserialize data from communication channel to a response object.
-    confirmation() -> Confirmation:
-
-    set_receive_callback(callback: Callable[[IResponse], None]) -> None:
-        Receive a response asynchronously, deserialize data from communication channel to a response object
-        and execute a callback if a function was passed.
     """
 
+    @abstractmethod
     def initialize(self) -> None:
         """
         Initialize transport and create a connection if applicable.
 
         Returns
         -------
         None
         """
         raise NotImplementedError("Abstract method not implemented.")
 
+    @abstractmethod
     def send(self, request: IRequest) -> None:
         """
         Serialize passed request to format acceptable by the communication channel and send request.
 
         Parameters
         ----------
         request: IRequest
@@ -48,36 +36,43 @@
 
         Returns
         -------
         None
         """
         raise NotImplementedError("Abstract method not implemented.")
 
+    @abstractmethod
+    def send_and_receive(self, request: IRequest, timeout: Optional[int] = None) -> IResponse:
+        raise NotImplementedError("Abstract method not implemented.")
+
+    @abstractmethod
     def receive(self) -> IResponse:
         """
         Return first unhandled response.
 
         Returns
         -------
         response: IResponse
             Response object
         """
         raise NotImplementedError("Abstract method not implemented.")
 
+    @abstractmethod
     def confirmation(self) -> Confirmation:
         """
         Return first unhandled confirmation.
 
         Returns
         -------
         confirmation: Confirmation
             Confirmation object
         """
         raise NotImplementedError("Abstract method not implemented.")
 
+    @abstractmethod
     def set_receive_callback(self, callback: Callable[[IResponse], None]) -> None:
         """
         Receive a response asynchronously, deserialize data from communication channel to a response object
         and execute a callback if a function was passed.
 
         Parameters
         ----------
```

### Comparing `iqrfpy-0.1.7/iqrfpy/transports/udp_transport.py` & `iqrfpy-0.1.8/iqrfpy/transports/udp_transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import IntEnum
 import socket
 from typing import Callable
 from crc import Calculator, Crc16
-from iqrfpy.messages.requests.IRequest import IRequest
-from iqrfpy.messages.responses.IResponse import IResponse
+from iqrfpy.messages.requests.irequest import IRequest
+from iqrfpy.messages.responses.iresponse import IResponse
 from iqrfpy.transports.itransport import ITransport
 
 __all__ = ['UdpTransport', 'UdpPacketHeader']
 
 BUF_SIZE = 1024
 CMD_WRITE_DATA = 0x03
 RESERVED = 0x00
```

### Comparing `iqrfpy-0.1.7/iqrfpy/utils/common.py` & `iqrfpy-0.1.8/iqrfpy/utils/common.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.7/iqrfpy/utils/dpa.py` & `iqrfpy-0.1.8/iqrfpy/utils/dpa.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.7/iqrfpy.egg-info/PKG-INFO` & `iqrfpy-0.1.8/iqrfpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqrfpy
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python library for communication with IQRF Network
 Home-page: https://gitlab.iqrf.org/microrisc/libiqrf-python
 Author: Karel Hanák
 Author-email: karel.hanak@iqrf.org
 License: Apache-2.0
 Keywords: iqrf,dpa
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iqrfpy-0.1.7/iqrfpy.egg-info/SOURCES.txt` & `iqrfpy-0.1.8/iqrfpy.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,140 +4,158 @@
 .pylintrc
 LICENSE
 Makefile
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
+test.py
 test_requirements.txt
 tox.ini
+examples/mqtt_transport_async.py
 examples/response_factories.py
 iqrfpy/__init__.py
 iqrfpy/exceptions.py
 iqrfpy.egg-info/PKG-INFO
 iqrfpy.egg-info/SOURCES.txt
 iqrfpy.egg-info/dependency_links.txt
 iqrfpy.egg-info/requires.txt
 iqrfpy.egg-info/top_level.txt
 iqrfpy/enums/__init__.py
 iqrfpy/enums/commands.py
 iqrfpy/enums/message_types.py
 iqrfpy/enums/peripherals.py
 iqrfpy/messages/__init__.py
 iqrfpy/messages/response_factory.py
-iqrfpy/messages/requests/IRequest.py
 iqrfpy/messages/requests/__init__.py
+iqrfpy/messages/requests/irequest.py
 iqrfpy/messages/requests/binaryoutput/__init__.py
-iqrfpy/messages/requests/coordinator/AddrInfo.py
-iqrfpy/messages/requests/coordinator/AuthorizeBond.py
-iqrfpy/messages/requests/coordinator/Backup.py
-iqrfpy/messages/requests/coordinator/BondNode.py
-iqrfpy/messages/requests/coordinator/BondedDevices.py
-iqrfpy/messages/requests/coordinator/ClearAllBonds.py
-iqrfpy/messages/requests/coordinator/DiscoveredDevices.py
-iqrfpy/messages/requests/coordinator/Discovery.py
-iqrfpy/messages/requests/coordinator/RemoveBond.py
-iqrfpy/messages/requests/coordinator/Restore.py
-iqrfpy/messages/requests/coordinator/SetDpaParams.py
-iqrfpy/messages/requests/coordinator/SetHops.py
-iqrfpy/messages/requests/coordinator/SetMID.py
-iqrfpy/messages/requests/coordinator/SmartConnect.py
 iqrfpy/messages/requests/coordinator/__init__.py
+iqrfpy/messages/requests/coordinator/addr_info.py
+iqrfpy/messages/requests/coordinator/authorize_bond.py
+iqrfpy/messages/requests/coordinator/backup.py
+iqrfpy/messages/requests/coordinator/bond_node.py
+iqrfpy/messages/requests/coordinator/bonded_devices.py
+iqrfpy/messages/requests/coordinator/clear_all_bonds.py
+iqrfpy/messages/requests/coordinator/discovered_devices.py
+iqrfpy/messages/requests/coordinator/discovery.py
+iqrfpy/messages/requests/coordinator/remove_bond.py
+iqrfpy/messages/requests/coordinator/restore.py
+iqrfpy/messages/requests/coordinator/set_dpa_params.py
+iqrfpy/messages/requests/coordinator/set_hops.py
+iqrfpy/messages/requests/coordinator/set_mid.py
+iqrfpy/messages/requests/coordinator/smart_connect.py
 iqrfpy/messages/requests/dali/__init__.py
 iqrfpy/messages/requests/eeeprom/__init__.py
 iqrfpy/messages/requests/eeprom/__init__.py
 iqrfpy/messages/requests/exploration/__init__.py
 iqrfpy/messages/requests/frc/__init__.py
 iqrfpy/messages/requests/generic/Raw.py
 iqrfpy/messages/requests/generic/RawHdp.py
 iqrfpy/messages/requests/generic/__init__.py
 iqrfpy/messages/requests/io/__init__.py
 iqrfpy/messages/requests/ledg/__init__.py
 iqrfpy/messages/requests/ledr/__init__.py
+iqrfpy/messages/requests/ledr/flashing.py
+iqrfpy/messages/requests/ledr/pulse.py
+iqrfpy/messages/requests/ledr/set_off.py
+iqrfpy/messages/requests/ledr/set_on.py
 iqrfpy/messages/requests/light/__init__.py
-iqrfpy/messages/requests/node/Read.py
 iqrfpy/messages/requests/node/__init__.py
+iqrfpy/messages/requests/node/read.py
 iqrfpy/messages/requests/os/__init__.py
+iqrfpy/messages/requests/os/read.py
 iqrfpy/messages/requests/ram/__init__.py
 iqrfpy/messages/requests/sensor/__init__.py
 iqrfpy/messages/requests/thermometer/__init__.py
 iqrfpy/messages/requests/uart/__init__.py
-iqrfpy/messages/responses/AsyncResponse.py
-iqrfpy/messages/responses/Confirmation.py
-iqrfpy/messages/responses/IResponse.py
 iqrfpy/messages/responses/__init__.py
+iqrfpy/messages/responses/async_response.py
+iqrfpy/messages/responses/confirmation.py
+iqrfpy/messages/responses/iresponse.py
 iqrfpy/messages/responses/binaryoutput/__init__.py
-iqrfpy/messages/responses/coordinator/AddrInfo.py
-iqrfpy/messages/responses/coordinator/AuthorizeBond.py
-iqrfpy/messages/responses/coordinator/Backup.py
-iqrfpy/messages/responses/coordinator/BondNode.py
-iqrfpy/messages/responses/coordinator/BondedDevices.py
-iqrfpy/messages/responses/coordinator/ClearAllBonds.py
-iqrfpy/messages/responses/coordinator/DiscoveredDevices.py
-iqrfpy/messages/responses/coordinator/Discovery.py
-iqrfpy/messages/responses/coordinator/RemoveBond.py
-iqrfpy/messages/responses/coordinator/Restore.py
-iqrfpy/messages/responses/coordinator/SetDpaParams.py
-iqrfpy/messages/responses/coordinator/SetHops.py
-iqrfpy/messages/responses/coordinator/SetMID.py
-iqrfpy/messages/responses/coordinator/SmartConnect.py
 iqrfpy/messages/responses/coordinator/__init__.py
+iqrfpy/messages/responses/coordinator/addr_info.py
+iqrfpy/messages/responses/coordinator/authorize_bond.py
+iqrfpy/messages/responses/coordinator/backup.py
+iqrfpy/messages/responses/coordinator/bond_node.py
+iqrfpy/messages/responses/coordinator/bonded_devices.py
+iqrfpy/messages/responses/coordinator/clear_all_bonds.py
+iqrfpy/messages/responses/coordinator/discovered_devices.py
+iqrfpy/messages/responses/coordinator/discovery.py
+iqrfpy/messages/responses/coordinator/remove_bond.py
+iqrfpy/messages/responses/coordinator/restore.py
+iqrfpy/messages/responses/coordinator/set_dpa_params.py
+iqrfpy/messages/responses/coordinator/set_hops.py
+iqrfpy/messages/responses/coordinator/set_mid.py
+iqrfpy/messages/responses/coordinator/smart_connect.py
 iqrfpy/messages/responses/dali/__init__.py
 iqrfpy/messages/responses/eeeprom/__init__.py
 iqrfpy/messages/responses/eeprom/__init__.py
 iqrfpy/messages/responses/exploration/__init__.py
 iqrfpy/messages/responses/frc/__init__.py
 iqrfpy/messages/responses/generic/__init__.py
 iqrfpy/messages/responses/io/__init__.py
 iqrfpy/messages/responses/ledg/__init__.py
 iqrfpy/messages/responses/ledr/__init__.py
+iqrfpy/messages/responses/ledr/flashing.py
+iqrfpy/messages/responses/ledr/pulse.py
+iqrfpy/messages/responses/ledr/set_off.py
+iqrfpy/messages/responses/ledr/set_on.py
 iqrfpy/messages/responses/light/__init__.py
-iqrfpy/messages/responses/node/Read.py
 iqrfpy/messages/responses/node/__init__.py
+iqrfpy/messages/responses/node/read.py
 iqrfpy/messages/responses/os/__init__.py
+iqrfpy/messages/responses/os/read.py
 iqrfpy/messages/responses/ram/__init__.py
 iqrfpy/messages/responses/sensor/__init__.py
 iqrfpy/messages/responses/thermometer/__init__.py
 iqrfpy/messages/responses/uart/__init__.py
 iqrfpy/transports/__init__.py
 iqrfpy/transports/itransport.py
 iqrfpy/transports/mqtt_transport.py
 iqrfpy/transports/udp_transport.py
 iqrfpy/utils/__init__.py
 iqrfpy/utils/common.py
 iqrfpy/utils/dpa.py
 iqrfpy/utils/enums.py
 tests/__init__.py
-tests/enums/Peripherals_test.py
+tests/enums/peripherals_test.py
 tests/messages/response_factory_test.py
-tests/messages/requests/IRequest_test.py
-tests/messages/requests/coordinator/AddrInfoRequest_test.py
-tests/messages/requests/coordinator/AuthorizeBondRequest_test.py
-tests/messages/requests/coordinator/BackupRequest_test.py
-tests/messages/requests/coordinator/BondNodeRequest_test.py
-tests/messages/requests/coordinator/BondedDevicesRequest_test.py
-tests/messages/requests/coordinator/ClearAllBondsRequest_test.py
-tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py
-tests/messages/requests/coordinator/DiscoveryRequest_test.py
-tests/messages/requests/coordinator/RemoveBondRequest_test.py
-tests/messages/requests/coordinator/RestoreRequest_test.py
-tests/messages/requests/coordinator/SetDpaParamsRequest_test.py
-tests/messages/requests/coordinator/SetHopsRequest_test.py
-tests/messages/requests/coordinator/SetMIDRequest_test.py
-tests/messages/requests/coordinator/SmartConnectRequest_test.py
-tests/messages/responses/AsyncResponse_test.py
-tests/messages/responses/Confirmation_test.py
-tests/messages/responses/coordinator/AddrInfoResponse_test.py
-tests/messages/responses/coordinator/AuthorizeBondResponse_test.py
-tests/messages/responses/coordinator/BackupResponse_test.py
-tests/messages/responses/coordinator/BondNodeResponse_test.py
-tests/messages/responses/coordinator/BondedDevicesResponse_test.py
-tests/messages/responses/coordinator/ClearAllBondsResponse_test.py
-tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py
-tests/messages/responses/coordinator/DiscoveryResponse_test.py
-tests/messages/responses/coordinator/RemoveNodeResponse_test.py
-tests/messages/responses/coordinator/RestoreResponse_test.py
-tests/messages/responses/coordinator/SetDpaParamsResponse_test.py
-tests/messages/responses/coordinator/SetHopsResponse_test.py
-tests/messages/responses/coordinator/SetMIDResponse_test.py
-tests/messages/responses/coordinator/SmartConnectResponse_test.py
-tests/utils/Common_test.py
+tests/messages/requests/irequest_test.py
+tests/messages/requests/coordinator/addr_info_request_test.py
+tests/messages/requests/coordinator/authorize_bond_request_test.py
+tests/messages/requests/coordinator/backup_request_test.py
+tests/messages/requests/coordinator/bond_node_request_test.py
+tests/messages/requests/coordinator/bonded_devices_request_test.py
+tests/messages/requests/coordinator/clear_all_bonds_request_test.py
+tests/messages/requests/coordinator/discovered_devices_request_test.py
+tests/messages/requests/coordinator/discovery_request_test.py
+tests/messages/requests/coordinator/remove_bond_request_test.py
+tests/messages/requests/coordinator/restore_request_test.py
+tests/messages/requests/coordinator/set_dpa_params_request_test.py
+tests/messages/requests/coordinator/set_hops_request_test.py
+tests/messages/requests/coordinator/set_mid_request_test.py
+tests/messages/requests/coordinator/smart_connect_request_test.py
+tests/messages/requests/ledr/flashing_request_test.py
+tests/messages/requests/ledr/pulse_request_test.py
+tests/messages/requests/ledr/set_off_request_test.py
+tests/messages/requests/ledr/set_on_request_test.py
+tests/messages/requests/os/read_request_test.py
+tests/messages/responses/async_response_test.py
+tests/messages/responses/confirmation_test.py
+tests/messages/responses/coordinator/addr_info_response_test.py
+tests/messages/responses/coordinator/authorize_bond_response_test.py
+tests/messages/responses/coordinator/backup_response_test.py
+tests/messages/responses/coordinator/bond_node_response_test.py
+tests/messages/responses/coordinator/bonded_devices_response_test.py
+tests/messages/responses/coordinator/clear_all_bonds_response_test.py
+tests/messages/responses/coordinator/discovered_devices_response_test.py
+tests/messages/responses/coordinator/discovery_response_test.py
+tests/messages/responses/coordinator/remove_node_response_test.py
+tests/messages/responses/coordinator/restore_response_test.py
+tests/messages/responses/coordinator/set_dpa_params_response_test.py
+tests/messages/responses/coordinator/set_hops_response_test.py
+tests/messages/responses/coordinator/set_mid_response_test.py
+tests/messages/responses/coordinator/smart_connect_response_test.py
+tests/messages/responses/os/read_response_test.py
+tests/utils/common_test.py
```

### Comparing `iqrfpy-0.1.7/setup.cfg` & `iqrfpy-0.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.7/tests/enums/Peripherals_test.py` & `iqrfpy-0.1.8/tests/enums/peripherals_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.7/tests/messages/requests/IRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/irequest_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.messages.requests.coordinator.AddrInfo import AddrInfoRequest
-from iqrfpy.messages.requests.node.Read import ReadRequest
+from iqrfpy.messages.requests.coordinator.addr_info import AddrInfoRequest
+from iqrfpy.messages.requests.node.read import ReadRequest
 
 
 class IRequestTestCase(unittest.TestCase):
 
     def setUp(self) -> None:
         self.request = AddrInfoRequest(msgid='addrInfoTest')
         self.json = {
```

### Comparing `iqrfpy-0.1.7/tests/messages/requests/coordinator/AddrInfoRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/coordinator/addr_info_request_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from iqrfpy.messages.requests.coordinator.AddrInfo import AddrInfoRequest
+from iqrfpy.messages.requests.coordinator.addr_info import AddrInfoRequest
 
 
 class AddrInfoRequestTestCase(unittest.TestCase):
 
     def setUp(self) -> None:
         self.request = AddrInfoRequest(msgid='addrInfoTest')
         self.dpa = b'\x00\x00\x00\x00\xff\xff'
```

### Comparing `iqrfpy-0.1.7/tests/messages/requests/coordinator/AuthorizeBondRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/coordinator/authorize_bond_request_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.messages.requests.coordinator.AuthorizeBond import AuthorizeBondParams, AuthorizeBondRequest
+from iqrfpy.messages.requests.coordinator.authorize_bond import AuthorizeBondParams, AuthorizeBondRequest
 
 
 class AuthorizeBondRequestTestCase(unittest.TestCase):
 
     def setUp(self) -> None:
         self.dpa = b'\x00\x00\x00\x0d\xff\xff\x01\x00\x00\x00\x00'
         self.json = {
@@ -107,15 +107,15 @@
         )
         self.assertEqual(
             request.to_json(),
             self.json
         )
 
     @parameterized.expand([
-        [[AuthorizeBondParams(reqAddr=0, mid=0)]],
-        [[AuthorizeBondParams(reqAddr=1, mid=-1)]],
-        [[AuthorizeBondParams(reqAddr=250, mid=10)]],
-        [[AuthorizeBondParams(reqAddr=2, mid=4294967297)]],
+        [0, 0],
+        [1, -1],
+        [250, 10],
+        [2, 4294967297],
     ])
-    def test_construct_invalid(self, params):
+    def test_construct_invalid(self, reqAddr, mid):
         with self.assertRaises(ValueError):
-            AuthorizeBondRequest(nodes=params)
+            AuthorizeBondParams(reqAddr=reqAddr, mid=mid)
```

### Comparing `iqrfpy-0.1.7/tests/messages/requests/coordinator/BackupRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/coordinator/backup_request_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.messages.requests.coordinator.Backup import BackupRequest
+from iqrfpy.messages.requests.coordinator.backup import BackupRequest
 
 
 class BackupRequestTestCase(unittest.TestCase):
 
     def setUp(self) -> None:
         self.dpa = b'\x00\x00\x00\x0b\xff\xff\x00'
         self.json = {
```

### Comparing `iqrfpy-0.1.7/tests/messages/requests/coordinator/BondNodeRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/coordinator/bond_node_request_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.messages.requests.coordinator.BondNode import BondNodeRequest
+from iqrfpy.messages.requests.coordinator.bond_node import BondNodeRequest
 
 
 class BondNodeRequestTestCase(unittest.TestCase):
 
     def setUp(self) -> None:
         self.dpa = b'\x00\x00\x00\x04\xff\xff\x01\x00'
         self.json = {
```

### Comparing `iqrfpy-0.1.7/tests/messages/requests/coordinator/BondedDevicesRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/coordinator/bonded_devices_request_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from iqrfpy.messages.requests.coordinator.BondedDevices import BondedDevicesRequest
+from iqrfpy.messages.requests.coordinator.bonded_devices import BondedDevicesRequest
 
 
 class BondedDevicesRequestTestCase(unittest.TestCase):
 
     def setUp(self) -> None:
         self.request = BondedDevicesRequest(msgid='bondedDevicesTest')
         self.dpa = b'\x00\x00\x00\x02\xff\xff'
```

### Comparing `iqrfpy-0.1.7/tests/messages/requests/coordinator/ClearAllBondsRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/coordinator/clear_all_bonds_request_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from iqrfpy.messages.requests.coordinator.ClearAllBonds import ClearAllBondsRequest
+from iqrfpy.messages.requests.coordinator.clear_all_bonds import ClearAllBondsRequest
 
 
 class ClearAllBondsRequestTestCase(unittest.TestCase):
 
     def setUp(self) -> None:
         self.request = ClearAllBondsRequest(msgid='clearAllBondsTest')
         self.dpa = b'\x00\x00\x00\x03\xff\xff'
```

### Comparing `iqrfpy-0.1.7/tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/coordinator/discovered_devices_request_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from iqrfpy.messages.requests.coordinator.DiscoveredDevices import DiscoveredDevicesRequest
+from iqrfpy.messages.requests.coordinator.discovered_devices import DiscoveredDevicesRequest
 
 
 class DiscoveredDevicesTestCase(unittest.TestCase):
 
     def setUp(self) -> None:
         self.request = DiscoveredDevicesRequest(msgid='discoveredDevicesTest')
         self.dpa = b'\x00\x00\x00\x01\xff\xff'
```

### Comparing `iqrfpy-0.1.7/tests/messages/requests/coordinator/DiscoveryRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/coordinator/discovery_request_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.messages.requests.coordinator.Discovery import DiscoveryRequest
+from iqrfpy.messages.requests.coordinator.discovery import DiscoveryRequest
 
 
 class BackupRequestTestCase(unittest.TestCase):
 
     def setUp(self) -> None:
         self.dpa = b'\x00\x00\x00\x07\xff\xff\x06\x00'
         self.json = {
```

### Comparing `iqrfpy-0.1.7/tests/messages/requests/coordinator/RemoveBondRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/coordinator/remove_bond_request_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.messages.requests.coordinator.RemoveBond import RemoveBondRequest
+from iqrfpy.messages.requests.coordinator.remove_bond import RemoveBondRequest
 
 
 class RemoveBondRequestTestCase(unittest.TestCase):
 
     def setUp(self) -> None:
         self.dpa = b'\x00\x00\x00\x05\xff\xff\x01'
         self.json = {
```

### Comparing `iqrfpy-0.1.7/tests/messages/requests/coordinator/RestoreRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/coordinator/restore_request_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 import unittest
 from parameterized import parameterized
-from iqrfpy.messages.requests.coordinator.Restore import RestoreRequest
+from iqrfpy.messages.requests.coordinator.restore import RestoreRequest
 
 
 class RestoreRequestTestCase(unittest.TestCase):
 
     def setUp(self) -> None:
         self.dpa = b''.join(
             [b'\x00\x00\x00\x0c\xff\xff\xed\x60\x14\x51\x82\xde\x7c\x72\xde\xf8\x90\xa3\xee\x82\x75\xed\x90\x54',
```

### Comparing `iqrfpy-0.1.7/tests/messages/requests/coordinator/SetDpaParamsRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/coordinator/set_dpa_params_request_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.messages.requests.coordinator.SetDpaParams import SetDpaParamsRequest, DpaParam
+from iqrfpy.messages.requests.coordinator.set_dpa_params import SetDpaParamsRequest, DpaParam
 
 
 class SetDpaParamsRequestTestCase(unittest.TestCase):
 
     def setUp(self) -> None:
         self.dpa = b'\x00\x00\x00\x08\xff\xff\x00'
         self.json = {
```

### Comparing `iqrfpy-0.1.7/tests/messages/requests/coordinator/SetHopsRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/coordinator/set_hops_request_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.messages.requests.coordinator.SetHops import SetHopsRequest
+from iqrfpy.messages.requests.coordinator.set_hops import SetHopsRequest
 
 
 class SetHopsRequestTestCase(unittest.TestCase):
 
     def setUp(self) -> None:
         self.dpa = b'\x00\x00\x00\x09\xff\xff\xff\xff'
         self.json = {
```

### Comparing `iqrfpy-0.1.7/tests/messages/requests/coordinator/SetMIDRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/coordinator/set_mid_request_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.messages.requests.coordinator.SetMID import SetMIDRequest
+from iqrfpy.messages.requests.coordinator.set_mid import SetMIDRequest
 
 
 class SetMIDRequestTestCase(unittest.TestCase):
 
     def setUp(self) -> None:
         self.dpa = b'\x00\x00\x00\x13\xff\xff\x00\x00\x00\x00\x0a'
         self.json = {
```

### Comparing `iqrfpy-0.1.7/tests/messages/requests/coordinator/SmartConnectRequest_test.py` & `iqrfpy-0.1.8/tests/messages/requests/coordinator/smart_connect_request_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 from dataclasses import dataclass
 from typing import Union
 from parameterized import parameterized
-from iqrfpy.messages.requests.coordinator.SmartConnect import SmartConnectRequest
+from iqrfpy.messages.requests.coordinator.smart_connect import SmartConnectRequest
 
 
 @dataclass
 class DataRegular:
     req_addr = 10
     bonding_test_retries = 3
     ibk = '201c5e762f75d7e244c3fa09b3de0ea1'
```

### Comparing `iqrfpy-0.1.7/tests/messages/response_factory_test.py` & `iqrfpy-0.1.8/tests/messages/response_factory_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.message_types import *
 from iqrfpy.exceptions import JsonMsgidMissingError, JsonMTypeMissingError, UnsupportedMessageTypeError
 from iqrfpy.messages.response_factory import *
-from iqrfpy.messages.responses.AsyncResponse import AsyncResponse
-from iqrfpy.messages.responses.Confirmation import Confirmation
+from iqrfpy.messages.responses.async_response import AsyncResponse
+from iqrfpy.messages.responses.confirmation import Confirmation
 from iqrfpy.messages.responses.coordinator import *
 
 
 class ResponseFactoryTestCase(unittest.TestCase):
 
     @parameterized.expand([
         [CoordinatorMessages.ADDR_INFO, CoordinatorAddrInfoFactory],
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/AsyncResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/async_response_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import ExplorationRequestCommands
 from iqrfpy.enums.message_types import GenericMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.AsyncResponse import AsyncResponse
+from iqrfpy.messages.responses.async_response import AsyncResponse
 
 data_ok: dict = {
     'msgid': 'async',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 128,
     'dpa_value': 0,
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/Confirmation_test.py` & `iqrfpy-0.1.8/tests/messages/responses/confirmation_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from iqrfpy.enums.commands import NodeRequestCommands
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.Confirmation import Confirmation
+from iqrfpy.messages.responses.confirmation import Confirmation
 
 
 class ConfirmationTestCase(unittest.TestCase):
 
     def test_from_dpa_ok(self):
         message = Confirmation.from_dpa(b'\x01\x00\x01\x00\xff\xff\xff\x36\x01\x04\x01')
         self.assertEqual(message.get_nadr(), 1)
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/coordinator/AddrInfoResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/coordinator/addr_info_response_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.coordinator.AddrInfo import AddrInfoResponse
+from iqrfpy.messages.responses.coordinator.addr_info import AddrInfoResponse
 
 data_ok: dict = {
     'msgid': 'addrInfoTest',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 0,
     'dpa_value': 64,
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/coordinator/AuthorizeBondResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/coordinator/authorize_bond_response_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.coordinator.AuthorizeBond import AuthorizeBondResponse
+from iqrfpy.messages.responses.coordinator.authorize_bond import AuthorizeBondResponse
 
 data_ok: dict = {
     'msgid': 'authorizeBondTest',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 0,
     'dpa_value': 64,
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/coordinator/BackupResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/coordinator/backup_response_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.coordinator.Backup import BackupResponse
+from iqrfpy.messages.responses.coordinator.backup import BackupResponse
 
 data_ok: dict = {
     'msgid': 'backupTest',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 0,
     'dpa_value': 90,
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/coordinator/BondNodeResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/coordinator/bond_node_response_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.coordinator.BondNode import BondNodeResponse
+from iqrfpy.messages.responses.coordinator.bond_node import BondNodeResponse
 
 data_ok: dict = {
     'msgid': 'bondNodeTest',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 0,
     'dpa_value': 71,
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/coordinator/BondedDevicesResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/coordinator/bonded_devices_response_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.coordinator.BondedDevices import BondedDevicesResponse
+from iqrfpy.messages.responses.coordinator.bonded_devices import BondedDevicesResponse
 
 data_ok: dict = {
     'msgid': 'bondedDevicesTest',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 0,
     'dpa_value': 71,
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/coordinator/ClearAllBondsResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/coordinator/clear_all_bonds_response_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.coordinator.ClearAllBonds import ClearAllBondsResponse
+from iqrfpy.messages.responses.coordinator.clear_all_bonds import ClearAllBondsResponse
 
 data_ok: dict = {
     'msgid': 'clearAllBondsTest',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 0,
     'dpa_value': 64,
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/coordinator/discovered_devices_response_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.coordinator.DiscoveredDevices import DiscoveredDevicesResponse
+from iqrfpy.messages.responses.coordinator.discovered_devices import DiscoveredDevicesResponse
 
 data_ok: dict = {
     'msgid': 'discoveredDevicesTest',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 0,
     'dpa_value': 71,
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/coordinator/DiscoveryResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/coordinator/discovery_response_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.coordinator.Discovery import DiscoveryResponse
+from iqrfpy.messages.responses.coordinator.discovery import DiscoveryResponse
 
 data_ok: dict = {
     'msgid': 'discoveryTest',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 0,
     'dpa_value': 55,
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/coordinator/RemoveNodeResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/coordinator/remove_node_response_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.coordinator.RemoveBond import RemoveBondResponse
+from iqrfpy.messages.responses.coordinator.remove_bond import RemoveBondResponse
 
 data_ok: dict = {
     'msgid': 'removeBondTest',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 0,
     'dpa_value': 55,
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/coordinator/RestoreResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/coordinator/restore_response_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.coordinator.Restore import RestoreResponse
+from iqrfpy.messages.responses.coordinator.restore import RestoreResponse
 
 data_ok: dict = {
     'msgid': 'restoreTest',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 0,
     'dpa_value': 64,
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/coordinator/SetDpaParamsResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/coordinator/set_dpa_params_response_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.coordinator.SetDpaParams import SetDpaParamsResponse, DpaParam
+from iqrfpy.messages.responses.coordinator.set_dpa_params import SetDpaParamsResponse, DpaParam
 
 data_ok: dict = {
     'msgid': 'setDpaParamsTest',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 0,
     'dpa_value': 64,
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/coordinator/SetHopsResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/coordinator/set_hops_response_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.coordinator.SetHops import SetHopsResponse
+from iqrfpy.messages.responses.coordinator.set_hops import SetHopsResponse
 
 data_ok: dict = {
     'msgid': 'setHopsTest',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 0,
     'dpa_value': 64,
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/coordinator/SetMIDResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/coordinator/set_mid_response_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.coordinator.SetMID import SetMIDResponse
+from iqrfpy.messages.responses.coordinator.set_mid import SetMIDResponse
 
 data_ok: dict = {
     'msgid': 'setMidResponse',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 0,
     'dpa_value': 64,
```

### Comparing `iqrfpy-0.1.7/tests/messages/responses/coordinator/SmartConnectResponse_test.py` & `iqrfpy-0.1.8/tests/messages/responses/coordinator/smart_connect_response_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.messages.responses.coordinator.SmartConnect import SmartConnectResponse
+from iqrfpy.messages.responses.coordinator.smart_connect import SmartConnectResponse
 
 data_ok: dict = {
     'msgid': 'smartConnectTest',
     'nadr': 0,
     'hwpid': 0,
     'rcode': 0,
     'dpa_value': 71,
```

### Comparing `iqrfpy-0.1.7/tests/utils/Common_test.py` & `iqrfpy-0.1.8/tests/utils/common_test.py`

 * *Files identical despite different names*

