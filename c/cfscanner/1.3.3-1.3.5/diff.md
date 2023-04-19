# Comparing `tmp/cfscanner-1.3.3.tar.gz` & `tmp/cfscanner-1.3.5.tar.gz`

## Comparing `cfscanner-1.3.3.tar` & `cfscanner-1.3.5.tar`

### file list

```diff
@@ -1,112 +1,36 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cfscanner-1.3.3/build_and_run.sh
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cfscanner-1.3.3/requirements.txt
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.vscode/settings.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.101.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.133.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.137.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.140.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.158.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.16.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.177.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.180.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.204.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.222.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.225.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.26.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.32.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.33.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.39.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.48.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.66.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.71.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.75.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-154.84.175.92.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-173.245.58.201.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-173.245.58.55.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-173.245.59.188.json
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.176.26.0.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.176.26.109.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.176.26.220.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.124.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.125.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.133.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.136.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.152.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.154.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.17.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.171.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.172.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.178.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.197.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.203.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.209.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.232.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.240.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.39.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.48.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.50.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.18.250.53.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.120.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.126.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.153.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.160.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.182.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.187.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.196.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.200.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.205.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.212.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.216.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.222.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.226.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.227.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.242.json
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.246.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.33.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.38.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.42.json
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.xray-configs/config-185.238.228.74.json
--rw-r--r--   0        0        0    10915 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/__main__.py
--rwxr-xr-x   0        0        0 25346048 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/xray-linux-64
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/args/__init__.py
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/args/parser.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/args/testconfig.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/report/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/report/colors.py
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/report/print.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/report/result.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/result/20230419_182123_result.csv
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/result/20230419_182334_result.csv
--rw-r--r--   0        0        0    19708 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/result/20230419_183458_result.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/speedtest/__init__.py
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/speedtest/conduct.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/speedtest/download.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/speedtest/fronting.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/speedtest/tools.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/speedtest/upload.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/subnets/__init__.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/subnets/cidr.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/subnets/regex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/utils/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/utils/decorators.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/utils/exceptions.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/utils/os.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/utils/requests.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/utils/socket.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/xray/__init__.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/xray/binary.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/xray/config.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/xray/service.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cfscanner-1.3.3/cfscanner/xray/templates.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.3/log/20230419_192854.log
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.3/log/20230419_193744.log
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.3/log/20230419_194036.log
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 cfscanner-1.3.3/result/20230419_192854_result.csv
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.3/result/20230419_193744_result.csv
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.3/result/20230419_194036_result.csv
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 cfscanner-1.3.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cfscanner-1.3.3/LICENSE
--rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 cfscanner-1.3.3/README.md
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 cfscanner-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 cfscanner-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cfscanner-1.3.5/.vscode/settings.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/__main__.py
+-rw-r--r--   0        0        0    10940 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/cfscanner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/args/__init__.py
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/args/parser.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/args/testconfig.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/report/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/report/colors.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/report/print.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/report/result.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/speedtest/__init__.py
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/speedtest/conduct.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/speedtest/download.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/speedtest/fronting.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/speedtest/tools.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/speedtest/upload.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/subnets/__init__.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/subnets/cidr.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/subnets/regex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/utils/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/utils/decorators.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/utils/exceptions.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/utils/os.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/utils/requests.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/utils/socket.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/xray/__init__.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/xray/binary.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/xray/config.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/xray/service.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cfscanner-1.3.5/cfscanner/xray/templates.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 cfscanner-1.3.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cfscanner-1.3.5/LICENSE
+-rw-r--r--   0        0        0     8764 2020-02-02 00:00:00.000000 cfscanner-1.3.5/README.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 cfscanner-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 cfscanner-1.3.5/PKG-INFO
```

### Comparing `cfscanner-1.3.3/.xray-configs/config-154.84.175.137.json` & `cfscanner-1.3.5/cfscanner/xray/templates.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,66 @@
-00000000: 7b0a 2020 2269 6e62 6f75 6e64 7322 3a20  {.  "inbounds": 
-00000010: 5b0a 2020 2020 7b0a 2020 2020 2020 2270  [.    {.      "p
-00000020: 6f72 7422 3a20 3439 3935 352c 0a20 2020  ort": 49955,.   
-00000030: 2020 2022 6c69 7374 656e 223a 2022 3132     "listen": "12
-00000040: 372e 302e 302e 3122 2c0a 2020 2020 2020  7.0.0.1",.      
-00000050: 2274 6167 223a 2022 736f 636b 732d 696e  "tag": "socks-in
-00000060: 626f 756e 6422 2c0a 2020 2020 2020 2270  bound",.      "p
-00000070: 726f 746f 636f 6c22 3a20 2273 6f63 6b73  rotocol": "socks
-00000080: 222c 0a20 2020 2020 2022 7365 7474 696e  ",.      "settin
-00000090: 6773 223a 207b 0a20 2020 2020 2020 2022  gs": {.        "
-000000a0: 6175 7468 223a 2022 6e6f 6175 7468 222c  auth": "noauth",
-000000b0: 0a20 2020 2020 2020 2022 7564 7022 3a20  .        "udp": 
-000000c0: 6661 6c73 652c 0a20 2020 2020 2020 2022  false,.        "
-000000d0: 6970 223a 2022 3132 372e 302e 302e 3122  ip": "127.0.0.1"
-000000e0: 0a20 2020 2020 207d 2c0a 2020 2020 2020  .      },.      
-000000f0: 2273 6e69 6666 696e 6722 3a20 7b0a 2020  "sniffing": {.  
-00000100: 2020 2020 2020 2265 6e61 626c 6564 223a        "enabled":
-00000110: 2074 7275 652c 0a20 2020 2020 2020 2022   true,.        "
-00000120: 6465 7374 4f76 6572 7269 6465 223a 205b  destOverride": [
-00000130: 0a20 2020 2020 2020 2020 2022 6874 7470  .          "http
-00000140: 222c 0a20 2020 2020 2020 2020 2022 746c  ",.          "tl
-00000150: 7322 0a20 2020 2020 2020 205d 0a20 2020  s".        ].   
-00000160: 2020 207d 0a20 2020 207d 0a20 205d 2c0a     }.    }.  ],.
-00000170: 2020 226f 7574 626f 756e 6473 223a 205b    "outbounds": [
-00000180: 0a20 2020 207b 0a20 2020 2020 2022 7072  .    {.      "pr
-00000190: 6f74 6f63 6f6c 223a 2022 766d 6573 7322  otocol": "vmess"
-000001a0: 2c0a 2020 2020 2020 2273 6574 7469 6e67  ,.      "setting
-000001b0: 7322 3a20 7b0a 2020 2020 2020 2020 2276  s": {.        "v
-000001c0: 6e65 7874 223a 205b 0a20 2020 2020 2020  next": [.       
-000001d0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-000001e0: 2022 6164 6472 6573 7322 3a20 2231 3534   "address": "154
-000001f0: 2e38 342e 3137 352e 3133 3722 2c0a 2020  .84.175.137",.  
-00000200: 2020 2020 2020 2020 2020 2270 6f72 7422            "port"
-00000210: 3a20 3434 332c 0a20 2020 2020 2020 2020  : 443,.         
-00000220: 2020 2022 7573 6572 7322 3a20 5b0a 2020     "users": [.  
-00000230: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00000240: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00000250: 6422 3a20 2232 3031 6236 3263 352d 3066  d": "201b62c5-0f
-00000260: 3834 2d35 6536 312d 6132 3230 2d34 3931  84-5e61-a220-491
-00000270: 3163 3063 3232 3162 3422 0a20 2020 2020  1c0c221b4".     
-00000280: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00000290: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-000002a0: 2020 207d 0a20 2020 2020 2020 205d 0a20     }.        ]. 
-000002b0: 2020 2020 207d 2c0a 2020 2020 2020 2273       },.      "s
-000002c0: 7472 6561 6d53 6574 7469 6e67 7322 3a20  treamSettings": 
-000002d0: 7b0a 2020 2020 2020 2020 226e 6574 776f  {.        "netwo
-000002e0: 726b 223a 2022 7773 222c 0a20 2020 2020  rk": "ws",.     
-000002f0: 2020 2022 7365 6375 7269 7479 223a 2022     "security": "
-00000300: 746c 7322 2c0a 2020 2020 2020 2020 2277  tls",.        "w
-00000310: 7353 6574 7469 6e67 7322 3a20 7b0a 2020  sSettings": {.  
-00000320: 2020 2020 2020 2020 2268 6561 6465 7273          "headers
-00000330: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00000340: 2022 486f 7374 223a 2022 7363 6865 7265   "Host": "schere
-00000350: 6874 7a68 656c 3031 2e65 6572 7363 682e  htzhel01.eersch.
-00000360: 6e65 7422 0a20 2020 2020 2020 2020 207d  net".          }
-00000370: 2c0a 2020 2020 2020 2020 2020 2270 6174  ,.          "pat
-00000380: 6822 3a20 222f 6170 6930 3122 0a20 2020  h": "/api01".   
-00000390: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000003a0: 2274 6c73 5365 7474 696e 6773 223a 207b  "tlsSettings": {
-000003b0: 0a20 2020 2020 2020 2020 2022 7365 7276  .          "serv
-000003c0: 6572 4e61 6d65 223a 2022 6365 6266 6635  erName": "cebff5
-000003d0: 6437 2d61 3733 352d 3461 3734 2d61 3437  d7-a735-4a74-a47
-000003e0: 612d 3431 3933 6461 6564 3962 6364 2e65  a-4193daed9bcd.e
-000003f0: 6572 7363 682e 6e65 7422 2c0a 2020 2020  ersch.net",.    
-00000400: 2020 2020 2020 2261 6c6c 6f77 496e 7365        "allowInse
-00000410: 6375 7265 223a 2066 616c 7365 0a20 2020  cure": false.   
-00000420: 2020 2020 207d 0a20 2020 2020 207d 0a20       }.      }. 
-00000430: 2020 207d 0a20 205d 2c0a 2020 226f 7468     }.  ],.  "oth
-00000440: 6572 223a 207b 7d0a 7d                   er": {}.}
+00000000: 766d 6573 735f 7773 5f74 6c73 203d 2027  vmess_ws_tls = '
+00000010: 2727 7b0a 2020 2269 6e62 6f75 6e64 7322  ''{.  "inbounds"
+00000020: 3a20 5b0a 2020 2020 7b0a 2020 2020 2020  : [.    {.      
+00000030: 2270 6f72 7422 3a20 504f 5254 504f 5254  "port": PORTPORT
+00000040: 2c0a 2020 2020 2020 226c 6973 7465 6e22  ,.      "listen"
+00000050: 3a20 2231 3237 2e30 2e30 2e31 222c 0a20  : "127.0.0.1",. 
+00000060: 2020 2020 2022 7461 6722 3a20 2273 6f63       "tag": "soc
+00000070: 6b73 2d69 6e62 6f75 6e64 222c 0a20 2020  ks-inbound",.   
+00000080: 2020 2022 7072 6f74 6f63 6f6c 223a 2022     "protocol": "
+00000090: 736f 636b 7322 2c0a 2020 2020 2020 2273  socks",.      "s
+000000a0: 6574 7469 6e67 7322 3a20 7b0a 2020 2020  ettings": {.    
+000000b0: 2020 2020 2261 7574 6822 3a20 226e 6f61      "auth": "noa
+000000c0: 7574 6822 2c0a 2020 2020 2020 2020 2275  uth",.        "u
+000000d0: 6470 223a 2066 616c 7365 2c0a 2020 2020  dp": false,.    
+000000e0: 2020 2020 2269 7022 3a20 2231 3237 2e30      "ip": "127.0
+000000f0: 2e30 2e31 220a 2020 2020 2020 7d2c 0a20  .0.1".      },. 
+00000100: 2020 2020 2022 736e 6966 6669 6e67 223a       "sniffing":
+00000110: 207b 0a20 2020 2020 2020 2022 656e 6162   {.        "enab
+00000120: 6c65 6422 3a20 7472 7565 2c0a 2020 2020  led": true,.    
+00000130: 2020 2020 2264 6573 744f 7665 7272 6964      "destOverrid
+00000140: 6522 3a20 5b0a 2020 2020 2020 2020 2020  e": [.          
+00000150: 2268 7474 7022 2c0a 2020 2020 2020 2020  "http",.        
+00000160: 2020 2274 6c73 220a 2020 2020 2020 2020    "tls".        
+00000170: 5d0a 2020 2020 2020 7d0a 2020 2020 7d0a  ].      }.    }.
+00000180: 2020 5d2c 0a20 2022 6f75 7462 6f75 6e64    ],.  "outbound
+00000190: 7322 3a20 5b0a 2020 2020 7b0a 2020 2020  s": [.    {.    
+000001a0: 2020 2270 726f 746f 636f 6c22 3a20 2276    "protocol": "v
+000001b0: 6d65 7373 222c 0a20 2020 2020 2022 7365  mess",.      "se
+000001c0: 7474 696e 6773 223a 207b 0a20 2020 2020  ttings": {.     
+000001d0: 2020 2022 766e 6578 7422 3a20 5b0a 2020     "vnext": [.  
+000001e0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000001f0: 2020 2020 2020 2261 6464 7265 7373 223a        "address":
+00000200: 2022 4950 2e49 502e 4950 2e49 5022 2c0a   "IP.IP.IP.IP",.
+00000210: 2020 2020 2020 2020 2020 2020 2270 6f72              "por
+00000220: 7422 3a20 4346 504f 5254 4346 504f 5254  t": CFPORTCFPORT
+00000230: 2c0a 2020 2020 2020 2020 2020 2020 2275  ,.            "u
+00000240: 7365 7273 223a 205b 0a20 2020 2020 2020  sers": [.       
+00000250: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00000260: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
+00000270: 4944 4944 220a 2020 2020 2020 2020 2020  IDID".          
+00000280: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00000290: 2020 5d0a 2020 2020 2020 2020 2020 7d0a    ].          }.
+000002a0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+000002b0: 7d2c 0a20 2020 2020 2022 7374 7265 616d  },.      "stream
+000002c0: 5365 7474 696e 6773 223a 207b 0a20 2020  Settings": {.   
+000002d0: 2020 2020 2022 6e65 7477 6f72 6b22 3a20       "network": 
+000002e0: 2277 7322 2c0a 2020 2020 2020 2020 2273  "ws",.        "s
+000002f0: 6563 7572 6974 7922 3a20 2274 6c73 222c  ecurity": "tls",
+00000300: 0a20 2020 2020 2020 2022 7773 5365 7474  .        "wsSett
+00000310: 696e 6773 223a 207b 0a20 2020 2020 2020  ings": {.       
+00000320: 2020 2022 6865 6164 6572 7322 3a20 7b0a     "headers": {.
+00000330: 2020 2020 2020 2020 2020 2020 2248 6f73              "Hos
+00000340: 7422 3a20 2248 4f53 5448 4f53 5422 0a20  t": "HOSTHOST". 
+00000350: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00000360: 2020 2020 2020 2270 6174 6822 3a20 2245        "path": "E
+00000370: 4e44 504f 494e 5445 4e44 504f 494e 5422  NDPOINTENDPOINT"
+00000380: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00000390: 2020 2020 2274 6c73 5365 7474 696e 6773      "tlsSettings
+000003a0: 223a 207b 0a20 2020 2020 2020 2020 2022  ": {.          "
+000003b0: 7365 7276 6572 4e61 6d65 223a 2022 5241  serverName": "RA
+000003c0: 4e44 4f4d 484f 5354 222c 0a20 2020 2020  NDOMHOST",.     
+000003d0: 2020 2020 2022 616c 6c6f 7749 6e73 6563       "allowInsec
+000003e0: 7572 6522 3a20 6661 6c73 650a 2020 2020  ure": false.    
+000003f0: 2020 2020 7d0a 2020 2020 2020 7d0a 2020      }.      }.  
+00000400: 2020 7d0a 2020 5d2c 0a20 2022 6f74 6865    }.  ],.  "othe
+00000410: 7222 3a20 7b7d 0a7d 2727 27              r": {}.}'''
```

### Comparing `cfscanner-1.3.3/cfscanner/__init__.py` & `cfscanner-1.3.5/cfscanner/cfscanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,28 +56,28 @@
     args = parse_args()
 
     if not args.no_vpn:
         with console.status(f"[green]Creating config dir \"{CONFIGDIR}\"[/green]"):
             try:
                 create_dir(CONFIGDIR)
             except Exception as e:
-                console.log("[red]Could not create config directory[/red]")
+                console.log("[red1]Could not create config directory[/red1]")
                 logger.exception("Could not create config directory")
                 exit(1)
-        console.log(f"[blue]Config directory created \"{CONFIGDIR}\"[/blue]")
+        console.log(f"[bright_blue]Config directory created \"{CONFIGDIR}\"[/bright_blue]")
         configFilePath = args.config_path
 
     with console.status(f"[green]Creating results directory \"{RESULTDIR}\"[/green]"):
         try:
             create_dir(RESULTDIR)
         except Exception as e:
-            console.log("[red]Could not create results directory[/red]")
+            console.log("[red1]Could not create results directory[/red1]")
             logger.exception("Could not create results directory")
             exit(1)
-    console.log(f"[blue]Results directory created \"{RESULTDIR}\"[/blue]")
+    console.log(f"[bright_blue]Results directory created \"{RESULTDIR}\"[/bright_blue]")
 
     # create empty result file
     with console.status(f"[green]Creating empty result file {INTERIM_RESULTS_PATH}[/green]"):
         try:
             with open(INTERIM_RESULTS_PATH, "w") as empty_file:
                 titles = [
                     "ip", "avg_download_speed", "avg_upload_speed",
@@ -93,47 +93,47 @@
                 ]
                 titles += [
                     f"upload_latency_{i+1}" for i in range(args.n_tries)
                 ]
                 empty_file.write(",".join(titles) + "\n")
         except Exception as e:
             console.log(
-                f"[red]Could not create empty result file:\n\"{INTERIM_RESULTS_PATH}\"[/red]"
+                f"[red1]Could not create empty result file:\n\"{INTERIM_RESULTS_PATH}\"[/red1]"
             )
             logger.exception("Could not create empty result file")
             exit(1)
 
     threadsCount = args.threads
 
     if args.subnets:
         with console.status("[green]Reading subnets from \"{args.subnets}\"[/green]"):
             try:
                 cidr_list = read_cidrs(args.subnets)
             except SubnetsReadError as e:
-                console.log(f"[red]Could not read subnets.[/red]")
+                console.log(f"[red1]Could not read subnets.[/red1]")
                 logger.exception(f"Could not read subnets")
                 exit(1)
             except Exception as e:
                 console.log(f"Unknown error in reading subnets: {e}")
                 logger.exception(f"Unknown error in reading subnets: {e}")
                 exit(1)
         console.log(
-            f"[blue]Subnets successfully read from \"{args.subnets}\"[/blue]")
+            f"[bright_blue]Subnets successfully read from \"{args.subnets}\"[/bright_blue]")
     else:
         subnets_default_address = "https://raw.githubusercontent.com/MortezaBashsiz/CFScanner/main/config/cf.local.iplist"
         console.log(
-            f"[blue]Subnets not provided. Default address will be used:\n\"{subnets_default_address}\"[/blue]"
+            f"[bright_blue]Subnets not provided. Default address will be used:\n\"{subnets_default_address}\"[/bright_blue]"
         )
         with console.status(f"[green]Retrieving subnets from \"{subnets_default_address}\"[/green]"):
             try:
                 cidr_list = read_cidrs(
                     "https://raw.githubusercontent.com/MortezaBashsiz/CFScanner/main/config/cf.local.iplist"
                 )
             except SubnetsReadError as e:
-                console.log(f"[red]Could not read subnets. {e}[/red]")
+                console.log(f"[red1]Could not read subnets. {e}[/red1]")
                 logger.exception(e)
                 exit(1)
             except Exception as e:
                 console.log(f"Unknown error in reading subnets: {e}")
                 logger.exception(e)
                 exit(1)
     
@@ -144,33 +144,33 @@
             console.log("[yellow]Could not shuffle subnets. Using original order[/yellow]")
             logger.exception(e)            
     
     try:
         test_config = TestConfig.from_args(args)
     except TemplateReadError as e:
         console.log(
-            f"[red]Could not read template from file \"{args.template_path}\"[/red]"
+            f"[red1]Could not read template from file \"{args.template_path}\"[/red1]"
         )
         logger.exception(e)        
         exit(1)
     except BinaryNotFoundError:
         console.log(
-            f"[red]Could not find xray/v2ray binary from path \"{args.binpath}\"[/red]")
+            f"[red1]Could not find xray/v2ray binary from path \"{args.binpath}\"[/red1]")
         logger.exception(e)
         exit(1)
     except Exception as e:
         console.print_exception()
         logger.exception(e)
         exit(1)
 
     n_total_ips = sum(get_num_ips_in_cidr(
         cidr,
         sample_size=test_config.sample_size
     ) for cidr in cidr_list)
-    console.log(f"[blue]Starting to scan {n_total_ips} ips...[/blue]")
+    console.log(f"[bright_blue]Starting to scan {n_total_ips} ips...[/bright_blue]")
 
     cidr_ip_lists = [
         cidr_to_ip_list(
             cidr,
             sample_size=test_config.sample_size)
         for cidr in cidr_list
     ]
@@ -231,15 +231,15 @@
                         rprint(res.message)
 
                     cidr_scanned_ips[res.cidr] += 1
                     if cidr_scanned_ips[res.cidr] == get_num_ips_in_cidr(res.cidr, sample_size=test_config.sample_size):
                         progress.remove_task(cidr_prog_tasks[res.cidr])
                 except StartProxyServiceError as e:
                     progress.stop()
-                    console.log(f"[red]{e}[/red]")
+                    console.log(f"[red1]{e}[/red1]")
                     pool.terminate()
                     logger.exception("Error in starting xray service.")
                     break
                 except StopIteration as e:
                     for task in progress.tasks:
                         progress.stop_task(task.id)
                         progress.remove_task(task.id)
@@ -252,14 +252,11 @@
                         progress.remove_task(task_id)
                     progress.stop()
                     progress.log(
                         f"[yellow]KeyboardInterrupt detected (scan phase) - start: {START_DT_STR}[/yellow]")
                     pool.terminate()
                     break
                 except Exception as e:
-                    progress.log("[red]Unknown error![/red]")
+                    progress.log("[red1]Unknown error![/red1]")
                     console.print_exception()
                     logger.exception(e)
                         
-                        
-if __name__ == "__main__":
-    main()
```

### Comparing `cfscanner-1.3.3/cfscanner/args/parser.py` & `cfscanner-1.3.5/cfscanner/args/parser.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/cfscanner/args/testconfig.py` & `cfscanner-1.3.5/cfscanner/args/testconfig.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/cfscanner/report/print.py` & `cfscanner-1.3.5/cfscanner/report/print.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     Args:
         ip (str): the ip that causes the error
         message (str): the message related to the error
         process (Popen): the process (xray) to be killed
     """
     process.kill()
-    return f"[bold red]NO[/bold red] [orange]{ip:15s}[/orange] [yellow]{message}[/yellow]"
+    return f"[bold red1]NO[/bold red1] [orange3]{ip:15s}[/orange3] [yellow1]{message}[/yellow1]"
 
 
 def ok_message(
     scan_result: dict
 ) -> None:
     """prints the result if test is ok
 
@@ -32,23 +32,23 @@
     """
     down_mean_jitter = mean_jitter(scan_result["download"]["latency"])
     up_mean_jitter = mean_jitter(scan_result["upload"]["latency"])
     mean_down_speed = mean(scan_result["download"]["speed"])
     mean_up_speed = mean(scan_result["upload"]["speed"])
     mean_down_latency = mean(scan_result["download"]["latency"])
     mean_up_latency = mean(scan_result["upload"]["latency"])
-    return f"[green]"\
-        f"OK [green][blue_violet]{scan_result['ip']:15s}[/blue_violet][blue] "\
+    return f"[bold green1]"\
+        f"OK [/bold green1][cyan1]{scan_result['ip']:15s}[/cyan1][bright_blue] "\
         f"avg_down_speed: {mean_down_speed:7.4f}mbps "\
         f"avg_up_speed: {mean_up_speed:7.4f}mbps "\
         f"avg_down_latency: {mean_down_latency:7.2f}ms "\
         f"avg_up_latency: {mean_up_latency:7.2f}ms "\
         f"avg_down_jitter: {down_mean_jitter:7.2f}ms "\
         f"avg_up_jitter: {up_mean_jitter:4.2f}ms"\
-        f"[/blue]"
+        f"[/bright_blue]"
 
 
 def color_text(text: str, rgb: tuple, bold: bool = False):
     """prints a colored text in the terminal using ANSI escape codes based on the rgb values
 
     Args:
         text (str): the text to be printed
```

### Comparing `cfscanner-1.3.3/cfscanner/report/result.py` & `cfscanner-1.3.5/cfscanner/report/result.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/cfscanner/speedtest/conduct.py` & `cfscanner-1.3.5/cfscanner/speedtest/conduct.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/cfscanner/speedtest/download.py` & `cfscanner-1.3.5/cfscanner/speedtest/download.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/cfscanner/speedtest/upload.py` & `cfscanner-1.3.5/cfscanner/speedtest/upload.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/cfscanner/subnets/cidr.py` & `cfscanner-1.3.5/cfscanner/subnets/cidr.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/cfscanner/utils/decorators.py` & `cfscanner-1.3.5/cfscanner/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/cfscanner/utils/exceptions.py` & `cfscanner-1.3.5/cfscanner/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/cfscanner/utils/os.py` & `cfscanner-1.3.5/cfscanner/utils/os.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/cfscanner/utils/requests.py` & `cfscanner-1.3.5/cfscanner/utils/requests.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/cfscanner/utils/socket.py` & `cfscanner-1.3.5/cfscanner/utils/socket.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/cfscanner/xray/__init__.py` & `cfscanner-1.3.5/cfscanner/xray/__init__.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/cfscanner/xray/binary.py` & `cfscanner-1.3.5/cfscanner/xray/binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             except KeyError as e:
                 raise BinaryDownloadError(
                     f"Failed to get binary from zip file {zip_url}")
             except Exception as e:
                 raise BinaryDownloadError(
                     f"Unknown error - detected system: {str(system_info)}")
     else:
-        console.log(f"[blue]Binary file already exists {bin_path}[/blue]")
+        console.log(f"[bright_blue]Binary file already exists {bin_path}[/bright_blue]")
         return bin_path
 
 
 def get_latest_release() -> dict:
     """Get the latest release info from github
 
     Returns:
```

### Comparing `cfscanner-1.3.3/cfscanner/xray/config.py` & `cfscanner-1.3.5/cfscanner/xray/config.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/cfscanner/xray/service.py` & `cfscanner-1.3.5/cfscanner/xray/service.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/.gitignore` & `cfscanner-1.3.5/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 python/venv/
 python/__pycache__/
 python/*/__pycache__/
 python/.vscode/
 python/*/log/
 python/.xray-configs
 python/result/
+python/*/*/__pycache__/
+python/dist/
 .tmp
 golang/CFScanner
 windows/*.rsuser
 windows/*.suo
 windows/*.user
 windows/*.userosscache
 windows/*.sln.docstates
```

### Comparing `cfscanner-1.3.3/LICENSE` & `cfscanner-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.3/README.md` & `cfscanner-1.3.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -230,10 +230,14 @@
   * Added subnets shuffling option
 * 1.3.1
   * Improved colors in logging
 * 1.3.2 
   * Added __main__ to run on windows using ``python -m cfscanner``
 * 1.3.3
   * fixed an issue with packaging
+* 1.3.4
+  * change the structure to improve module names in the logs
+* 1.3.5
+  * fixed a bug
 
 [python]: https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white
 [version]: https://img.shields.io/badge/Version-1.3.0-blue
```

### Comparing `cfscanner-1.3.3/pyproject.toml` & `cfscanner-1.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cfscanner"
-version = "1.3.3"
+version = "1.3.5"
 authors = [
   { name="tempookian", email="tempookian@gmail.com" },
   { name="Morteza Bashsiz", email="morteza.bashsiz@gmail.com"}
 ]
 description = "Cloudflare's edge IPs scanner to locate ones that are viable for use with v2ray/xray"
 readme = "README.md"
 requires-python = ">=3.6"
@@ -24,8 +24,8 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/MortezaBashsiz/CFScanner/tree/main/python"
 "Bug Tracker" = "https://github.com/MortezaBashsiz/CFScanner/issues"
 
 [project.scripts]
-cfscanner = "cfscanner:main"
+cfscanner = "cfscanner:cfscanner"
```

### Comparing `cfscanner-1.3.3/PKG-INFO` & `cfscanner-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfscanner
-Version: 1.3.3
+Version: 1.3.5
 Summary: Cloudflare's edge IPs scanner to locate ones that are viable for use with v2ray/xray
 Project-URL: Homepage, https://github.com/MortezaBashsiz/CFScanner/tree/main/python
 Project-URL: Bug Tracker, https://github.com/MortezaBashsiz/CFScanner/issues
 Author-email: tempookian <tempookian@gmail.com>, Morteza Bashsiz <morteza.bashsiz@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -247,10 +247,14 @@
   * Added subnets shuffling option
 * 1.3.1
   * Improved colors in logging
 * 1.3.2 
   * Added __main__ to run on windows using ``python -m cfscanner``
 * 1.3.3
   * fixed an issue with packaging
+* 1.3.4
+  * change the structure to improve module names in the logs
+* 1.3.5
+  * fixed a bug
 
 [python]: https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white
 [version]: https://img.shields.io/badge/Version-1.3.0-blue
```

