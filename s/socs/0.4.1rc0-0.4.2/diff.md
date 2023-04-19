# Comparing `tmp/socs-0.4.1rc0.tar.gz` & `tmp/socs-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socs-0.4.1rc0.tar", last modified: Fri Feb 10 16:18:17 2023, max compression
+gzip compressed data, was "socs-0.4.2.tar", last modified: Wed Apr 19 16:58:31 2023, max compression
```

## Comparing `socs-0.4.1rc0.tar` & `socs-0.4.2.tar`

### file list

```diff
@@ -1,181 +1,190 @@
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.153991 socs-0.4.1rc0/
--rw-r--r--   0 koopman   (1000) koopman   (1000)     1294 2022-10-28 16:13:43.000000 socs-0.4.1rc0/LICENSE.txt
--rw-r--r--   0 koopman   (1000) koopman   (1000)       47 2019-06-25 15:16:09.000000 socs-0.4.1rc0/MANIFEST.in
--rw-r--r--   0 koopman   (1000) koopman   (1000)     5551 2023-02-10 16:18:17.153991 socs-0.4.1rc0/PKG-INFO
--rw-r--r--   0 koopman   (1000) koopman   (1000)     4764 2023-02-08 22:52:14.000000 socs-0.4.1rc0/README.rst
--rw-r--r--   0 koopman   (1000) koopman   (1000)      127 2022-10-28 16:13:43.000000 socs-0.4.1rc0/pyproject.toml
--rw-r--r--   0 koopman   (1000) koopman   (1000)      192 2023-02-10 16:18:17.153991 socs-0.4.1rc0/setup.cfg
--rw-r--r--   0 koopman   (1000) koopman   (1000)     3259 2023-02-08 22:52:14.000000 socs-0.4.1rc0/setup.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.153991 socs-0.4.1rc0/socs/
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.140658 socs-0.4.1rc0/socs/Lakeshore/
--rw-r--r--   0 koopman   (1000) koopman   (1000)    15686 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/Lakeshore/Lakeshore240.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    40327 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/Lakeshore/Lakeshore336.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    56866 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/Lakeshore/Lakeshore370.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    57733 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/Lakeshore/Lakeshore372.py
--rwxr-xr-x   0 koopman   (1000) koopman   (1000)     1444 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/Lakeshore/Lakeshore425.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2019-06-25 15:16:09.000000 socs-0.4.1rc0/socs/Lakeshore/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)       94 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)      500 2023-02-10 16:18:17.153991 socs-0.4.1rc0/socs/_version.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.140658 socs-0.4.1rc0/socs/agents/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/__init__.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.140658 socs-0.4.1rc0/socs/agents/acu/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/acu/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    49985 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/acu/agent.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    13726 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/acu/drivers.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.140658 socs-0.4.1rc0/socs/agents/bluefors/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/bluefors/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    19253 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/bluefors/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.140658 socs-0.4.1rc0/socs/agents/cryomech_cpa/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/cryomech_cpa/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    14370 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/cryomech_cpa/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.140658 socs-0.4.1rc0/socs/agents/fts_aerotech/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/fts_aerotech/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    12424 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/fts_aerotech/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.140658 socs-0.4.1rc0/socs/agents/holo_fpga/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/holo_fpga/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     6362 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/holo_fpga/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.140658 socs-0.4.1rc0/socs/agents/holo_synth/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/holo_synth/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     8587 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/holo_synth/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.140658 socs-0.4.1rc0/socs/agents/hwp_encoder/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/hwp_encoder/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    29096 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/hwp_encoder/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.140658 socs-0.4.1rc0/socs/agents/hwp_picoscope/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/hwp_picoscope/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     7498 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/hwp_picoscope/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.143991 socs-0.4.1rc0/socs/agents/hwp_picoscope/drivers/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/hwp_picoscope/drivers/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    21269 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/hwp_picoscope/drivers/class_ps3000a.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.143991 socs-0.4.1rc0/socs/agents/hwp_rotation/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/hwp_rotation/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    18596 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/hwp_rotation/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.143991 socs-0.4.1rc0/socs/agents/hwp_rotation/drivers/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/hwp_rotation/drivers/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    10418 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/hwp_rotation/drivers/pid_controller.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.143991 socs-0.4.1rc0/socs/agents/labjack/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/labjack/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    20201 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/labjack/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.143991 socs-0.4.1rc0/socs/agents/labjack/cal_curves/
--rw-r--r--   0 koopman   (1000) koopman   (1000)     1085 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/labjack/cal_curves/GA10K4D25_cal_curve.txt
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.143991 socs-0.4.1rc0/socs/agents/lakeshore240/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/lakeshore240/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    12026 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/lakeshore240/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.143991 socs-0.4.1rc0/socs/agents/lakeshore336/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/lakeshore336/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    48306 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/lakeshore336/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.143991 socs-0.4.1rc0/socs/agents/lakeshore370/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/lakeshore370/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    36049 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/lakeshore370/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.143991 socs-0.4.1rc0/socs/agents/lakeshore372/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/lakeshore372/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    51099 2023-02-10 14:20:40.000000 socs-0.4.1rc0/socs/agents/lakeshore372/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.143991 socs-0.4.1rc0/socs/agents/lakeshore425/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/lakeshore425/__init__.py
--rwxr-xr-x   0 koopman   (1000) koopman   (1000)     9229 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/lakeshore425/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.143991 socs-0.4.1rc0/socs/agents/magpie/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/magpie/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    37829 2023-02-10 14:20:40.000000 socs-0.4.1rc0/socs/agents/magpie/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.143991 socs-0.4.1rc0/socs/agents/meinberg_m1000/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/meinberg_m1000/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    17785 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/meinberg_m1000/agent.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     2285 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/ocs_plugin_so.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.143991 socs-0.4.1rc0/socs/agents/pfeiffer_tc400/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/pfeiffer_tc400/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     8828 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/pfeiffer_tc400/agent.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     6851 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/pfeiffer_tc400/drivers.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.147324 socs-0.4.1rc0/socs/agents/pfeiffer_tpg366/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/pfeiffer_tpg366/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     6588 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/pfeiffer_tpg366/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.147324 socs-0.4.1rc0/socs/agents/pysmurf_controller/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/pysmurf_controller/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    35232 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/pysmurf_controller/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.147324 socs-0.4.1rc0/socs/agents/pysmurf_monitor/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/pysmurf_monitor/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     9127 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/pysmurf_monitor/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.147324 socs-0.4.1rc0/socs/agents/scpi_psu/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/scpi_psu/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     6719 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/scpi_psu/agent.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     2582 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/scpi_psu/drivers.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.147324 socs-0.4.1rc0/socs/agents/smurf_crate_monitor/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/smurf_crate_monitor/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    11231 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/smurf_crate_monitor/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.147324 socs-0.4.1rc0/socs/agents/smurf_file_emulator/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/smurf_file_emulator/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    23200 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/smurf_file_emulator/agent.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)   105526 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/smurf_file_emulator/status_sample.yaml
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.147324 socs-0.4.1rc0/socs/agents/smurf_stream_simulator/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/smurf_stream_simulator/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    12307 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/smurf_stream_simulator/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.147324 socs-0.4.1rc0/socs/agents/suprsync/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/suprsync/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     8736 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/suprsync/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.147324 socs-0.4.1rc0/socs/agents/synacc/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/synacc/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     8494 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/synacc/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.147324 socs-0.4.1rc0/socs/agents/tektronix3021c/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/tektronix3021c/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     5526 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/tektronix3021c/agent.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)      408 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/tektronix3021c/drivers.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.147324 socs-0.4.1rc0/socs/agents/ups/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/ups/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    14778 2023-02-10 14:24:29.000000 socs-0.4.1rc0/socs/agents/ups/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.147324 socs-0.4.1rc0/socs/agents/vantagepro2/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/vantagepro2/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     6984 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/vantagepro2/agent.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    13703 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/vantagepro2/drivers.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.150658 socs-0.4.1rc0/socs/agents/wiregrid_actuator/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/wiregrid_actuator/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    34937 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/wiregrid_actuator/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.150658 socs-0.4.1rc0/socs/agents/wiregrid_actuator/drivers/
--rw-r--r--   0 koopman   (1000) koopman   (1000)    14540 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/wiregrid_actuator/drivers/Actuator.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     7945 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/wiregrid_actuator/drivers/DigitalIO.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/wiregrid_actuator/drivers/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)      831 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/wiregrid_actuator/limitswitch_config.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)      503 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/wiregrid_actuator/stopper_config.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.150658 socs-0.4.1rc0/socs/agents/wiregrid_encoder/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/wiregrid_encoder/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    14735 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/wiregrid_encoder/agent.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     9427 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/wiregrid_encoder/drivers.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.150658 socs-0.4.1rc0/socs/agents/wiregrid_kikusui/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/wiregrid_kikusui/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    24161 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/wiregrid_kikusui/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.150658 socs-0.4.1rc0/socs/agents/wiregrid_kikusui/drivers/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/wiregrid_kikusui/drivers/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     1087 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/wiregrid_kikusui/drivers/common.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.150658 socs-0.4.1rc0/socs/agents/xy_stage/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/xy_stage/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     9898 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/agents/xy_stage/agent.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.150658 socs-0.4.1rc0/socs/common/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/common/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     6763 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/common/moxa_serial.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    17376 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/common/pmx.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     1002 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/common/prologix_interface.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.150658 socs-0.4.1rc0/socs/db/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2022-10-28 16:13:43.000000 socs-0.4.1rc0/socs/db/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    16264 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/db/suprsync.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.153991 socs-0.4.1rc0/socs/mibs/
--rw-r--r--   0 koopman   (1000) koopman   (1000)    17434 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/mibs/IBOOTPDU-MIB.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)   143372 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/mibs/MBG-SNMP-LTNG-MIB.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     2141 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/mibs/MBG-SNMP-ROOT-MIB.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    16838 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/mibs/SNMPv2-MIB.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    38813 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/mibs/UPS-MIB.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/mibs/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     3339 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/plugin.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)     7993 2023-02-10 14:20:40.000000 socs-0.4.1rc0/socs/snmp.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.153991 socs-0.4.1rc0/socs/testing/
--rw-r--r--   0 koopman   (1000) koopman   (1000)        0 2022-10-28 16:13:43.000000 socs-0.4.1rc0/socs/testing/__init__.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    11075 2023-02-08 22:52:14.000000 socs-0.4.1rc0/socs/testing/device_emulator.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)      152 2022-10-28 16:13:43.000000 socs-0.4.1rc0/socs/util.py
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.140658 socs-0.4.1rc0/socs.egg-info/
--rw-r--r--   0 koopman   (1000) koopman   (1000)     5551 2023-02-10 16:18:17.000000 socs-0.4.1rc0/socs.egg-info/PKG-INFO
--rw-r--r--   0 koopman   (1000) koopman   (1000)     4273 2023-02-10 16:18:17.000000 socs-0.4.1rc0/socs.egg-info/SOURCES.txt
--rw-r--r--   0 koopman   (1000) koopman   (1000)        1 2023-02-10 16:18:17.000000 socs-0.4.1rc0/socs.egg-info/dependency_links.txt
--rw-r--r--   0 koopman   (1000) koopman   (1000)       33 2023-02-10 16:18:17.000000 socs-0.4.1rc0/socs.egg-info/entry_points.txt
--rw-r--r--   0 koopman   (1000) koopman   (1000)      315 2023-02-10 16:18:17.000000 socs-0.4.1rc0/socs.egg-info/requires.txt
--rw-r--r--   0 koopman   (1000) koopman   (1000)        5 2023-02-10 16:18:17.000000 socs-0.4.1rc0/socs.egg-info/top_level.txt
-drwxr-xr-x   0 koopman   (1000) koopman   (1000)        0 2023-02-10 16:18:17.153991 socs-0.4.1rc0/tests/
--rw-r--r--   0 koopman   (1000) koopman   (1000)      911 2023-02-08 22:52:14.000000 socs-0.4.1rc0/tests/test_device_emulator.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)       33 2023-02-08 22:52:14.000000 socs-0.4.1rc0/tests/test_plugin.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)       36 2022-10-28 16:13:43.000000 socs-0.4.1rc0/tests/test_snmp.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)       36 2022-10-28 16:13:43.000000 socs-0.4.1rc0/tests/test_util.py
--rw-r--r--   0 koopman   (1000) koopman   (1000)    69022 2023-02-08 22:52:14.000000 socs-0.4.1rc0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.646277 socs-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-19 16:58:14.000000 socs-0.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-19 16:58:14.000000 socs-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-04-19 16:58:31.646277 socs-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-19 16:58:14.000000 socs-0.4.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-19 16:58:14.000000 socs-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-19 16:58:31.646277 socs-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-19 16:58:14.000000 socs-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.646277 socs-0.4.2/socs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/Lakeshore/
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-04-19 16:58:14.000000 socs-0.4.2/socs/Lakeshore/Lakeshore240.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40327 2023-04-19 16:58:14.000000 socs-0.4.2/socs/Lakeshore/Lakeshore336.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56866 2023-04-19 16:58:14.000000 socs-0.4.2/socs/Lakeshore/Lakeshore370.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57733 2023-04-19 16:58:14.000000 socs-0.4.2/socs/Lakeshore/Lakeshore372.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1444 2023-04-19 16:58:14.000000 socs-0.4.2/socs/Lakeshore/Lakeshore425.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/Lakeshore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-19 16:58:14.000000 socs-0.4.2/socs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-19 16:58:31.646277 socs-0.4.2/socs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/acu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/acu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60407 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/acu/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/acu/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/bluefors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/bluefors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/bluefors/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/cryomech_cpa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/cryomech_cpa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/cryomech_cpa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/fts_aerotech/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/fts_aerotech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12424 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/fts_aerotech/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/holo_fpga/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/holo_fpga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/holo_fpga/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/holo_synth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/holo_synth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/holo_synth/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/hwp_encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29096 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_encoder/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/hwp_picoscope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_picoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_picoscope/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/hwp_picoscope/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_picoscope/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21269 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_picoscope/drivers/class_ps3000a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/hwp_rotation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_rotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18596 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_rotation/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/hwp_rotation/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_rotation/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_rotation/drivers/pid_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/ibootbar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/ibootbar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/ibootbar/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/labjack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/labjack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20201 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/labjack/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/labjack/cal_curves/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/labjack/cal_curves/GA10K4D25_cal_curve.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/lakeshore240/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore240/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore240/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/lakeshore336/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore336/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48306 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore336/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/lakeshore370/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore370/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36049 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore370/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.630276 socs-0.4.2/socs/agents/lakeshore372/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore372/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64295 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore372/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.630276 socs-0.4.2/socs/agents/lakeshore425/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore425/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9229 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore425/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.630276 socs-0.4.2/socs/agents/magpie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/magpie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37829 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/magpie/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.630276 socs-0.4.2/socs/agents/meinberg_m1000/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/meinberg_m1000/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17785 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/meinberg_m1000/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/ocs_plugin_so.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.630276 socs-0.4.2/socs/agents/pfeiffer_tc400/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pfeiffer_tc400/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pfeiffer_tc400/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pfeiffer_tc400/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.630276 socs-0.4.2/socs/agents/pfeiffer_tpg366/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pfeiffer_tpg366/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pfeiffer_tpg366/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.630276 socs-0.4.2/socs/agents/pysmurf_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pysmurf_controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35232 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pysmurf_controller/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.634276 socs-0.4.2/socs/agents/pysmurf_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pysmurf_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pysmurf_monitor/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.634276 socs-0.4.2/socs/agents/scpi_psu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/scpi_psu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/scpi_psu/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/scpi_psu/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.634276 socs-0.4.2/socs/agents/smurf_crate_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_crate_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_crate_monitor/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.634276 socs-0.4.2/socs/agents/smurf_file_emulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_file_emulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25842 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_file_emulator/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105526 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_file_emulator/status_sample.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.634276 socs-0.4.2/socs/agents/smurf_stream_simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_stream_simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_stream_simulator/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.634276 socs-0.4.2/socs/agents/smurf_timing_card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_timing_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_timing_card/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.634276 socs-0.4.2/socs/agents/suprsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/suprsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/suprsync/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.638277 socs-0.4.2/socs/agents/synacc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/synacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/synacc/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.638277 socs-0.4.2/socs/agents/tektronix3021c/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/tektronix3021c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/tektronix3021c/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/tektronix3021c/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.638277 socs-0.4.2/socs/agents/thorlabs_mc2000b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/thorlabs_mc2000b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/thorlabs_mc2000b/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.638277 socs-0.4.2/socs/agents/ups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/ups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/ups/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.638277 socs-0.4.2/socs/agents/vantagepro2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/vantagepro2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/vantagepro2/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/vantagepro2/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.638277 socs-0.4.2/socs/agents/wiregrid_actuator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_actuator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34937 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_actuator/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.638277 socs-0.4.2/socs/agents/wiregrid_actuator/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_actuator/drivers/Actuator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_actuator/drivers/DigitalIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_actuator/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_actuator/limitswitch_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_actuator/stopper_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.642277 socs-0.4.2/socs/agents/wiregrid_encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_encoder/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_encoder/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.642277 socs-0.4.2/socs/agents/wiregrid_kikusui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_kikusui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_kikusui/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.642277 socs-0.4.2/socs/agents/wiregrid_kikusui/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_kikusui/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_kikusui/drivers/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.642277 socs-0.4.2/socs/agents/xy_stage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/xy_stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/xy_stage/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.642277 socs-0.4.2/socs/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-19 16:58:14.000000 socs-0.4.2/socs/common/moxa_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-04-19 16:58:14.000000 socs-0.4.2/socs/common/pmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-19 16:58:14.000000 socs-0.4.2/socs/common/prologix_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.642277 socs-0.4.2/socs/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16265 2023-04-19 16:58:14.000000 socs-0.4.2/socs/db/suprsync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.646277 socs-0.4.2/socs/mibs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17434 2023-04-19 16:58:14.000000 socs-0.4.2/socs/mibs/IBOOTPDU-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143372 2023-04-19 16:58:14.000000 socs-0.4.2/socs/mibs/MBG-SNMP-LTNG-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-19 16:58:14.000000 socs-0.4.2/socs/mibs/MBG-SNMP-ROOT-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-04-19 16:58:14.000000 socs-0.4.2/socs/mibs/SNMPv2-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38813 2023-04-19 16:58:14.000000 socs-0.4.2/socs/mibs/UPS-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/mibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-19 16:58:14.000000 socs-0.4.2/socs/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-04-19 16:58:14.000000 socs-0.4.2/socs/snmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.646277 socs-0.4.2/socs/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-04-19 16:58:14.000000 socs-0.4.2/socs/testing/device_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-19 16:58:14.000000 socs-0.4.2/socs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.618276 socs-0.4.2/socs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-04-19 16:58:31.000000 socs-0.4.2/socs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-19 16:58:31.000000 socs-0.4.2/socs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:58:31.000000 socs-0.4.2/socs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 16:58:31.000000 socs-0.4.2/socs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-19 16:58:31.000000 socs-0.4.2/socs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 16:58:31.000000 socs-0.4.2/socs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.646277 socs-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-19 16:58:14.000000 socs-0.4.2/tests/test_device_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 16:58:14.000000 socs-0.4.2/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-19 16:58:14.000000 socs-0.4.2/tests/test_snmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-19 16:58:14.000000 socs-0.4.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69022 2023-04-19 16:58:14.000000 socs-0.4.2/versioneer.py
```

### Comparing `socs-0.4.1rc0/LICENSE.txt` & `socs-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/PKG-INFO` & `socs-0.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socs
-Version: 0.4.1rc0
+Version: 0.4.2
 Summary: Simons Observatory Control System
 Home-page: https://github.com/simonsobs/socs
 Project-URL: Source Code, https://github.com/simonsobs/ocs
 Project-URL: Documentation, https://ocs.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/simonsobs/ocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -15,40 +15,41 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: labjack
 Provides-Extra: magpie
 Provides-Extra: pfeiffer
 Provides-Extra: smurf_sim
 Provides-Extra: synacc
+Provides-Extra: timing_master
 License-File: LICENSE.txt
 
 ========================================
 SOCS - Simons Observatory Control System
 ========================================
 
-.. image:: https://img.shields.io/github/actions/workflow/status/simonsobs/socs/develop.yml?branch=develop
-    :target: https://github.com/simonsobs/socs/actions?query=workflow%3A%22Build+Develop+Images%22
+.. image:: https://img.shields.io/github/actions/workflow/status/simonsobs/socs/develop.yml?branch=main
+    :target: https://github.com/simonsobs/socs/actions?query=workflow%3A%22Build+Test+Images%22
     :alt: GitHub Workflow Status
 
-.. image:: https://readthedocs.org/projects/socs/badge/?version=develop
-    :target: https://socs.readthedocs.io/en/develop/?badge=develop
+.. image:: https://readthedocs.org/projects/socs/badge/?version=main
+    :target: https://socs.readthedocs.io/en/main/?badge=main
     :alt: Documentation Status
 
-.. image:: https://coveralls.io/repos/github/simonsobs/socs/badge.svg?branch=develop
-    :target: https://coveralls.io/github/simonsobs/socs?branch=develop
+.. image:: https://coveralls.io/repos/github/simonsobs/socs/badge.svg
+    :target: https://coveralls.io/github/simonsobs/socs
 
 .. image:: https://img.shields.io/badge/dockerhub-latest-blue
     :target: https://hub.docker.com/r/simonsobs/ocs/tags
 
 .. image:: https://img.shields.io/pypi/v/socs
    :target: https://pypi.org/project/socs/
    :alt: PyPI Package
 
-.. image:: https://results.pre-commit.ci/badge/github/simonsobs/socs/develop.svg
-   :target: https://results.pre-commit.ci/latest/github/simonsobs/socs/develop
+.. image:: https://results.pre-commit.ci/badge/github/simonsobs/socs/main.svg
+   :target: https://results.pre-commit.ci/latest/github/simonsobs/socs/main
    :alt: pre-commit.ci status
 
 Overview
 --------
 
 This repository, `SOCS`_, contains hardware control code for the
 Simons Observatory.  This code operates within the framework provided
@@ -75,22 +76,22 @@
 "all"::
 
     $ pip3 install -U socs[all]
 
 **Note:** Not all optional dependencies can be installed this way. See the
 `Installation Documentation`_ for more info on specific agent dependencies.
 
-.. _`Installation Documentation`: https://socs.readthedocs.io/en/develop/user/installation.html
+.. _`Installation Documentation`: https://socs.readthedocs.io/en/main/user/installation.html
 
 Installing from Source
 ``````````````````````
 
-If you are considering contributing to SOCS, or would like to use the
-development branch, you will want to install from source. To do so,
-clone the repository and install using pip:
+If you are considering contributing to SOCS, or would like to use an unreleased
+feature, you will want to install from source. To do so, clone this repository
+and install using pip:
 
 .. code-block:: bash
 
     git clone https://github.com/simonsobs/socs.git
     cd socs/
     pip3 install -r requirements.txt
     pip3 install .
@@ -105,28 +106,28 @@
   # List of additional paths to Agent plugin modules.
   'agent-paths': [
     '/path/to/socs/agents/',
   ],
 
 See the `ocs docs`_ for more details.
 
-.. _`ocs docs`: https://ocs.readthedocs.io/en/develop/developer/site_config.html
+.. _`ocs docs`: https://ocs.readthedocs.io/en/main/developer/site_config.html
 
 Docker Images
 -------------
 Docker images for SOCS and each Agent are available on `Docker Hub`_. Official
 releases will be tagged with their release version, i.e. ``v0.1.0``. These are
 only built on release, and the ``latest`` tag will point to the latest of these
 released tags. These should be considered stable.
 
-Development images will be tagged with the latest released version tag, the
-number of commits ahead of that release, the latest commit hash, and the tag
-``-dev``, i.e.  ``v0.0.2-81-g9c10ba6-dev``. These get built on each commit to
-the ``develop`` branch, and are useful for testing and development, but should
-be considered unstable.
+Test images will be tagged with the latest released version tag, the number of
+commits ahead of that release, the latest commit hash, i.e.
+``v0.0.2-81-g9c10ba6-dev``. These get built on each commit to the ``main``
+branch, and are useful for testing and development, but should be considered
+unstable.
 
 .. _Docker Hub: https://hub.docker.com/u/simonsobs
 
 Documentation
 -------------
 The SOCS documentation can be built using Sphinx. There is a separate
 ``requirements.txt`` file in the ``docs/`` directory to install Sphinx and any
@@ -147,21 +148,21 @@
 ``tests/`` directory::
 
   $ cd tests/
   $ python3 -m pytest --cov
 
 For more details see `tests/README.rst <tests_>`_.
 
-.. _tests: https://github.com/simonsobs/socs/blob/master/tests/README.rst
+.. _tests: https://github.com/simonsobs/socs/blob/main/tests/README.rst
 
 Contributing
 ------------
 For guidelines on how to contribute to OCS see `CONTRIBUTING.rst`_.
 
-.. _CONTRIBUTING.rst: https://github.com/simonsobs/socs/blob/master/CONTRIBUTING.rst
+.. _CONTRIBUTING.rst: https://github.com/simonsobs/socs/blob/main/CONTRIBUTING.rst
 
 License
 --------
 This project is licensed under the BSD 2-Clause License - see the
 `LICENSE.txt`_ file for details.
 
-.. _LICENSE.txt: https://github.com/simonsobs/socs/blob/master/LICENSE.txt
+.. _LICENSE.txt: https://github.com/simonsobs/socs/blob/main/LICENSE.txt
```

### Comparing `socs-0.4.1rc0/README.rst` & `socs-0.4.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 ========================================
 SOCS - Simons Observatory Control System
 ========================================
 
-.. image:: https://img.shields.io/github/actions/workflow/status/simonsobs/socs/develop.yml?branch=develop
-    :target: https://github.com/simonsobs/socs/actions?query=workflow%3A%22Build+Develop+Images%22
+.. image:: https://img.shields.io/github/actions/workflow/status/simonsobs/socs/develop.yml?branch=main
+    :target: https://github.com/simonsobs/socs/actions?query=workflow%3A%22Build+Test+Images%22
     :alt: GitHub Workflow Status
 
-.. image:: https://readthedocs.org/projects/socs/badge/?version=develop
-    :target: https://socs.readthedocs.io/en/develop/?badge=develop
+.. image:: https://readthedocs.org/projects/socs/badge/?version=main
+    :target: https://socs.readthedocs.io/en/main/?badge=main
     :alt: Documentation Status
 
-.. image:: https://coveralls.io/repos/github/simonsobs/socs/badge.svg?branch=develop
-    :target: https://coveralls.io/github/simonsobs/socs?branch=develop
+.. image:: https://coveralls.io/repos/github/simonsobs/socs/badge.svg
+    :target: https://coveralls.io/github/simonsobs/socs
 
 .. image:: https://img.shields.io/badge/dockerhub-latest-blue
     :target: https://hub.docker.com/r/simonsobs/ocs/tags
 
 .. image:: https://img.shields.io/pypi/v/socs
    :target: https://pypi.org/project/socs/
    :alt: PyPI Package
 
-.. image:: https://results.pre-commit.ci/badge/github/simonsobs/socs/develop.svg
-   :target: https://results.pre-commit.ci/latest/github/simonsobs/socs/develop
+.. image:: https://results.pre-commit.ci/badge/github/simonsobs/socs/main.svg
+   :target: https://results.pre-commit.ci/latest/github/simonsobs/socs/main
    :alt: pre-commit.ci status
 
 Overview
 --------
 
 This repository, `SOCS`_, contains hardware control code for the
 Simons Observatory.  This code operates within the framework provided
@@ -52,22 +52,22 @@
 "all"::
 
     $ pip3 install -U socs[all]
 
 **Note:** Not all optional dependencies can be installed this way. See the
 `Installation Documentation`_ for more info on specific agent dependencies.
 
-.. _`Installation Documentation`: https://socs.readthedocs.io/en/develop/user/installation.html
+.. _`Installation Documentation`: https://socs.readthedocs.io/en/main/user/installation.html
 
 Installing from Source
 ``````````````````````
 
-If you are considering contributing to SOCS, or would like to use the
-development branch, you will want to install from source. To do so,
-clone the repository and install using pip:
+If you are considering contributing to SOCS, or would like to use an unreleased
+feature, you will want to install from source. To do so, clone this repository
+and install using pip:
 
 .. code-block:: bash
 
     git clone https://github.com/simonsobs/socs.git
     cd socs/
     pip3 install -r requirements.txt
     pip3 install .
@@ -82,28 +82,28 @@
   # List of additional paths to Agent plugin modules.
   'agent-paths': [
     '/path/to/socs/agents/',
   ],
 
 See the `ocs docs`_ for more details.
 
-.. _`ocs docs`: https://ocs.readthedocs.io/en/develop/developer/site_config.html
+.. _`ocs docs`: https://ocs.readthedocs.io/en/main/developer/site_config.html
 
 Docker Images
 -------------
 Docker images for SOCS and each Agent are available on `Docker Hub`_. Official
 releases will be tagged with their release version, i.e. ``v0.1.0``. These are
 only built on release, and the ``latest`` tag will point to the latest of these
 released tags. These should be considered stable.
 
-Development images will be tagged with the latest released version tag, the
-number of commits ahead of that release, the latest commit hash, and the tag
-``-dev``, i.e.  ``v0.0.2-81-g9c10ba6-dev``. These get built on each commit to
-the ``develop`` branch, and are useful for testing and development, but should
-be considered unstable.
+Test images will be tagged with the latest released version tag, the number of
+commits ahead of that release, the latest commit hash, i.e.
+``v0.0.2-81-g9c10ba6-dev``. These get built on each commit to the ``main``
+branch, and are useful for testing and development, but should be considered
+unstable.
 
 .. _Docker Hub: https://hub.docker.com/u/simonsobs
 
 Documentation
 -------------
 The SOCS documentation can be built using Sphinx. There is a separate
 ``requirements.txt`` file in the ``docs/`` directory to install Sphinx and any
@@ -124,21 +124,21 @@
 ``tests/`` directory::
 
   $ cd tests/
   $ python3 -m pytest --cov
 
 For more details see `tests/README.rst <tests_>`_.
 
-.. _tests: https://github.com/simonsobs/socs/blob/master/tests/README.rst
+.. _tests: https://github.com/simonsobs/socs/blob/main/tests/README.rst
 
 Contributing
 ------------
 For guidelines on how to contribute to OCS see `CONTRIBUTING.rst`_.
 
-.. _CONTRIBUTING.rst: https://github.com/simonsobs/socs/blob/master/CONTRIBUTING.rst
+.. _CONTRIBUTING.rst: https://github.com/simonsobs/socs/blob/main/CONTRIBUTING.rst
 
 License
 --------
 This project is licensed under the BSD 2-Clause License - see the
 `LICENSE.txt`_ file for details.
 
-.. _LICENSE.txt: https://github.com/simonsobs/socs/blob/master/LICENSE.txt
+.. _LICENSE.txt: https://github.com/simonsobs/socs/blob/main/LICENSE.txt
```

### Comparing `socs-0.4.1rc0/setup.py` & `socs-0.4.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,24 +41,27 @@
 
 # SMuRF File Emulator, SMuRF Stream Simulator
 smurf_sim_deps = ['so3g']
 
 # Synaccess Agent
 synacc_deps = ['requests']
 
+# Timing Master Monitor
+timing_master_deps = ['pyepics']
+
 # LATRt XY Stage Agent
 # xy_stage_deps = [
 #     'xy_stage_control @ git+https://github.com/kmharrington/xy_stage_control.git@main',
 # ]
 
 # Note: Not including the holograph deps, which are Python 3.8 only
 # all_deps = acu_deps + labjack_deps + magpie_deps + pfeiffer_deps + \
 #    pysmurf_deps + smurf_sim_deps + synacc_deps + xy_stage_deps
 all_deps = labjack_deps + magpie_deps + pfeiffer_deps + \
-    smurf_sim_deps + synacc_deps
+    smurf_sim_deps + synacc_deps + timing_master_deps
 all_deps = list(set(all_deps))
 
 setup(
     name='socs',
     long_description=long_description,
     long_description_content_type="text/x-rst",
     version=versioneer.get_version(),
@@ -106,10 +109,11 @@
         # 'holography': holography_deps,
         'labjack': labjack_deps,
         'magpie': magpie_deps,
         'pfeiffer': pfeiffer_deps,
         # 'pysmurf': pysmurf_deps,
         'smurf_sim': smurf_sim_deps,
         'synacc': synacc_deps,
+        'timing_master': timing_master_deps,
         # 'xy_stage': xy_stage_deps,
     },
 )
```

### Comparing `socs-0.4.1rc0/socs/Lakeshore/Lakeshore240.py` & `socs-0.4.2/socs/Lakeshore/Lakeshore240.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/Lakeshore/Lakeshore336.py` & `socs-0.4.2/socs/Lakeshore/Lakeshore336.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/Lakeshore/Lakeshore370.py` & `socs-0.4.2/socs/Lakeshore/Lakeshore370.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/Lakeshore/Lakeshore372.py` & `socs-0.4.2/socs/Lakeshore/Lakeshore372.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/Lakeshore/Lakeshore425.py` & `socs-0.4.2/socs/Lakeshore/Lakeshore425.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/bluefors/agent.py` & `socs-0.4.2/socs/agents/bluefors/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/cryomech_cpa/agent.py` & `socs-0.4.2/socs/agents/cryomech_cpa/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/fts_aerotech/agent.py` & `socs-0.4.2/socs/agents/fts_aerotech/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/holo_fpga/agent.py` & `socs-0.4.2/socs/agents/holo_fpga/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/holo_synth/agent.py` & `socs-0.4.2/socs/agents/holo_synth/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/hwp_encoder/agent.py` & `socs-0.4.2/socs/agents/hwp_encoder/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/hwp_picoscope/agent.py` & `socs-0.4.2/socs/agents/hwp_picoscope/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/hwp_picoscope/drivers/class_ps3000a.py` & `socs-0.4.2/socs/agents/hwp_picoscope/drivers/class_ps3000a.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/hwp_rotation/agent.py` & `socs-0.4.2/socs/agents/hwp_rotation/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/hwp_rotation/drivers/pid_controller.py` & `socs-0.4.2/socs/agents/hwp_rotation/drivers/pid_controller.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/labjack/agent.py` & `socs-0.4.2/socs/agents/labjack/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/labjack/cal_curves/GA10K4D25_cal_curve.txt` & `socs-0.4.2/socs/agents/labjack/cal_curves/GA10K4D25_cal_curve.txt`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/lakeshore240/agent.py` & `socs-0.4.2/socs/agents/lakeshore240/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/lakeshore336/agent.py` & `socs-0.4.2/socs/agents/lakeshore336/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/lakeshore370/agent.py` & `socs-0.4.2/socs/agents/lakeshore370/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/lakeshore372/agent.py` & `socs-0.4.2/socs/agents/lakeshore372/agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 from ocs import ocs_agent, site_config
 from ocs.ocs_twisted import Pacemaker, TimeoutLock
 from twisted.internet import reactor
 
 from socs.Lakeshore.Lakeshore372 import LS372
 
 
+def still_power_to_perc(power, res, lead, max_volts):
+    cur = np.sqrt(power / res)
+    volt = (lead + res) * cur
+    return 100 * volt / max_volts
+
+
 class YieldingLock:
     """A lock protected by a lock.  This braided arrangement guarantees
     that a thread waiting on the lock will get priority over a thread
     that has just released the lock and wants to reacquire it.
 
     The typical use case is a Process that wants to hold the lock as
     much as possible, but occasionally release the lock (without
@@ -745,15 +751,14 @@
         """servo_to_temperature(temperature)
 
         **Task** - Servo to a given temperature using a closed loop PID on a
         fixed channel. This will automatically disable autoscan if enabled.
 
         Parameters:
             temperature (float): Temperature to servo to in units of Kelvin.
-
         """
         with self._lock.acquire_timeout(job='servo_to_temperature') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
@@ -783,14 +788,298 @@
             if params["temperature"] > 1:
                 return False, 'Servo temperature is set above 1K. Aborting.'
 
             self.module.sample_heater.set_setpoint(params["temperature"])
 
         return True, f'Setpoint now set to {params["temperature"]} K'
 
+    @ocs_agent.param('channel', type=int)
+    @ocs_agent.param('state', type=str, choices=['on', 'off'])
+    def engage_channel(self, session, params):
+        """engage_channel(channel, state)
+
+        **Task** - Enables/disables a channel on the LS372
+
+        Parameters:
+            channel (int): Channel number to enable
+            state (str): Desired power state of channel; 'on' or 'off'
+        """
+        with self._lock.acquire_timeout(job='engage_channel') as acquired:
+            if not acquired:
+                self.log.warn(f"Could not start Task because "
+                              f"{self._lock.job} is already running")
+                return False, "Could not acquire lock"
+
+            session.set_status('running')
+
+            channel = params['channel']
+            state = params['state']
+            if state == 'on':
+                self.module.channels[channel].enable_channel()
+            else:
+                self.module.channels[channel].disable_channel()
+
+        return True, "Channel {} powered {}".format(channel, state)
+
+    @ocs_agent.param('channel', type=int, check=lambda x: 0 <= x <= 16)
+    @ocs_agent.param('curve_number', type=int, check=lambda x: 21 <= x <= 59)
+    def set_calibration_curve(self, session, params):
+        """set_calibration_curve(channel, curve_number)
+
+        **Task** - Sets the calibration curve number for a particular channel.
+
+        Parameters:
+            channel (int): Channel number to set calibration curve to. Channel
+                ranges are 1 to 16, and 0 for control channel A.
+            curve_number (int): Curve number of calibration curve uploaded to
+                the LS372. Curve number ranges are 21 to 59.
+        """
+        with self._lock.acquire_timeout(job='set_calibration_curve') as acquired:
+            if not acquired:
+                self.log.warn(f"Could not start Task because "
+                              f"{self._lock.job} is already running")
+                return False, "Could not acquire lock"
+
+            session.set_status('running')
+
+            channel = params['channel']
+            curve_number = params['curve_number']
+            self.module.channels[channel].set_calibration_curve(curve_number)
+
+        return True, f"Assigned channel {channel} to curve number {curve_number}."
+
+    @ocs_agent.param('channel', type=int)
+    def get_input_setup(self, session, params):
+        """get_input_setup(channel)
+
+        **Task** - Gets measurement inputs for a specific channel on the LS372
+
+        Parameters:
+            channel (int): Channel number to get input setup
+
+        Notes:
+            The most recent data collected is stored in session data in the
+            structure::
+
+                >>> response.session['data']
+                {"mode": 'voltage',
+                 "excitation": 6.32e-05,
+                 "excitation_units": 'volts',
+                 "autorange": 'on',
+                 "range": 2000.0,
+                 "csshunt": 'on',
+                 "units": 'kelvin'}
+
+        """
+        with self._lock.acquire_timeout(job='get_input_setup') as acquired:
+            if not acquired:
+                self.log.warn(f"Could not start Task because "
+                              f"{self._lock.job} is already running")
+                return False, "Could not acquire lock"
+
+            session.set_status('running')
+
+            channel = params['channel']
+
+            ls_chann_setting = self.module.channels[channel]
+            input_setup = ls_chann_setting.get_input_setup()
+
+            session.data = {"mode": ls_chann_setting.mode,
+                            "excitation": ls_chann_setting.excitation,
+                            "excitation_units": ls_chann_setting.excitation_units,
+                            "autorange": ls_chann_setting.autorange,
+                            "range": ls_chann_setting.range,
+                            "csshunt": ls_chann_setting.csshunt,
+                            "units": ls_chann_setting.units}
+
+        return True, f"Channel {channel} has measurement inputs {input_setup} = [mode," \
+                     "excitation, auto range, range, cs_shunt, units]"
+
+    @ocs_agent.param('setpoint', type=float)
+    @ocs_agent.param('heater', type=str)
+    @ocs_agent.param('channel', type=int)
+    @ocs_agent.param('P', type=int)
+    @ocs_agent.param('I', type=float)
+    @ocs_agent.param('update_time', type=int)
+    @ocs_agent.param('sample_heater_range', type=float, default=10e-3)
+    @ocs_agent.param('test_mode', type=bool, default=False)
+    def start_custom_pid(self, session, params):
+        """start_custom_pid(setpoint, heater, channel, P, \
+                            I, update_time, sample_heater_range=10e-3, \
+                            test_mode=False)
+
+        **Task** - Set custom software PID parameters for servo control of fridge
+        using still or sample heater. Currently only P and I implemented.
+
+        Parameters:
+            setpoint (float): Setpoint in Kelvin
+            heater (str): 'still' or 'sample'
+            channel (int): LS372 Channel to PID off of
+            P (int): Proportional value in Watts/Kelvin
+            I (int): Integral Value in Hz
+            update_time (int): Time between PID updates in seconds
+            sample_heater_range (float): Range for sample heater in Amps.
+                                         Default is 10e-3.
+            test_mode (bool, optional): Run the Process loop only once.
+                                        This is meant only for testing.
+                                        Default is False.
+
+        Notes:
+            The most recent data collected is stored in session data in the structure.
+            The channel number noted below depends upon which channel is being used
+            to servo::
+
+                >>> response.session['data']
+                {"fields":
+                    {"Channel_02": {"T": 293.644, "R": 33.752, "timestamps": 1601924482.722671}}
+                }
+        """
+
+        with self._acq_proc_lock.acquire_timeout(timeout=0, job='custom_pid') \
+                as acq_acquired, \
+                self._lock.acquire_timeout(job='custom_pid') as acquired:
+            if not acq_acquired:
+                self.log.warn(f"Could not start Process because "
+                              f"{self._acq_proc_lock.job} is already running")
+                return False, "Could not acquire lock"
+            if not acquired:
+                self.log.warn(f"Could not start Process because "
+                              f"{self._lock.job} is holding the lock")
+                return False, "Could not acquire lock"
+
+            session.set_status('running')
+            session.data = {"fields": {}}
+
+            setpoint = params['setpoint']
+            heater = params['heater']
+            ch = params['channel']
+            P_val = params['P']
+            I_val = params['I']
+            update_time = params['update_time']
+            sample_heater_range = params['sample_heater_range']
+
+            # Constants
+            still_heater_R = 120  # [ohms]
+            still_lead_R = 14.679  # [ohms]
+            delta_t = 0.32  # rough intrinsic sampling period of the LS372 (s)
+            max_voltage = 10  # [V]
+
+            # Get heaters in the correct configuration
+            if heater == 'sample':
+                # Set heater range
+                if sample_heater_range == self.module.sample_heater.get_heater_range():
+                    self.log.info(f"Heater range already set to {sample_heater_range} amps")
+                else:
+                    self.module.sample_heater.set_heater_range(sample_heater_range)
+
+                # Check we're in correct control mode for servo.
+                if self.module.sample_heater.mode != 'Open Loop':
+                    session.add_message('Changing control to Open Loop mode for sample PID.')
+                    self.module.sample_heater.set_mode("Open Loop")
+
+            if heater == 'still':
+                # Check we're in correct control mode for servo.
+                if self.module.still_heater.mode != 'Open Loop':
+                    session.add_message('Changing control to Open Loop mode for still PID.')
+                    self.module.still_heater.set_mode("Open Loop")
+
+            # Check we aren't autoscanning.
+            if self.module.get_autoscan() is True:
+                session.add_message('Autoscan is enabled, disabling for still PID control on dedicated channel.')
+                self.module.disable_autoscan()
+
+            # Check we're scanning same channel expected by heater for control.
+            if self.module.get_active_channel().channel_num != ch:
+                session.add_message(f'Changing active channel to {ch} for still PID')
+                self.module.set_active_channel(ch)
+
+            # Start the PID
+            self.custom_pid = True
+            active_channel = self.module.get_active_channel()
+            channel_str = active_channel.name.replace(' ', '_')
+            last_pid = time.time()
+            heater_I = 0
+            temps, resistances, times = [], [], []
+            self.log.info(f"Starting PID on heater {heater}, ch {ch} to setpoint {setpoint} K")
+
+            while self.custom_pid:
+                # Get a list of T and R at the maximum sample frequency
+                temps.append(self.module.get_temp(unit='kelvin', chan=ch))
+                resistances.append(self.module.get_temp(unit='ohms', chan=ch))
+                times.append(time.time())
+
+                # Calculate and apply the PID based on the most recent temperature set
+                if times[-1] - last_pid > update_time:
+                    heater_P = P_val * (setpoint - np.mean(np.array(temps)))
+                    heater_I += P_val * I_val * (delta_t * np.sum(setpoint - np.array(temps)))
+                    heater_pow = max(0.0, heater_P + heater_I)
+                    if heater == 'still':
+                        heater_frac = still_power_to_perc(heater_pow, still_heater_R, still_lead_R, max_voltage)
+                        self.module.still_heater.set_heater_output(heater_frac)
+                    if heater == 'sample':
+                        self.module.sample_heater.set_heater_output(heater_pow)
+
+                    # Publish heater values
+                    if heater == 'still':
+                        heater_data = {
+                            'timestamp': last_pid,
+                            'block_name': 'still_heater_out',
+                            'data': {'still_heater_out': heater_frac}
+                        }
+                        session.app.publish_to_feed('temperatures', heater_data)
+
+                    if heater == 'sample':
+                        heater_data = {
+                            'timestamp': last_pid,
+                            'block_name': 'sample_heater_out',
+                            'data': {'sample_heater_out': heater_pow}
+                        }
+                        session.app.publish_to_feed('temperatures', heater_data)
+
+                    # Publish T and R values
+                    temp_data = {
+                        'timestamps': times,
+                        'block_name': active_channel.name,
+                        'data': {channel_str + '_T': temps,
+                                 channel_str + '_R': resistances}
+                    }
+                    session.app.publish_to_feed('temperatures', temp_data)
+
+                    # For session.data
+                    field_dict = {channel_str: {"T": temps,
+                                                "R": resistances,
+                                                "timestamps": times}}
+                    session.data['fields'].update(field_dict)
+                    self.log.debug("{data}", data=session.data)
+
+                    # Reset for the next PID iteration
+                    temps, resistances, times = [], [], []
+                    last_pid = time.time()
+
+                    # Relinquish sampling lock temporarily
+                    if not self._lock.release_and_acquire(timeout=10):
+                        self.log.warn(f"Failed to re-acquire sampling lock, "
+                                      f"currently held by {self._lock.job}.")
+                        continue
+
+                if params['test_mode']:
+                    break
+
+        return True, 'PID exited cleanly.'
+
+    def _stop_custom_pid(self, session, params=None):
+        """
+        Stops acq process.
+        """
+        if self.custom_pid:
+            self.custom_pid = False
+            return True, 'Stopping the custom PID'
+        else:
+            return False, 'PID is not currently running'
+
     @ocs_agent.param('measurements', type=int)
     @ocs_agent.param('threshold', type=float)
     def check_temperature_stability(self, session, params):
         """check_temperature_stability(measurements, threshold)
 
         Check servo temperature stability is within threshold.
 
@@ -1142,24 +1431,28 @@
     agent.register_task('set_excitation_mode', lake_agent.set_excitation_mode)
     agent.register_task('set_excitation', lake_agent.set_excitation)
     agent.register_task('get_excitation', lake_agent.get_excitation)
     agent.register_task('set_resistance_range', lake_agent.set_resistance_range)
     agent.register_task('get_resistance_range', lake_agent.get_resistance_range)
     agent.register_task('set_dwell', lake_agent.set_dwell)
     agent.register_task('get_dwell', lake_agent.get_dwell)
+    agent.register_task('engage_channel', lake_agent.engage_channel)
+    agent.register_task('get_input_setup', lake_agent.get_input_setup)
+    agent.register_task('set_calibration_curve', lake_agent.set_calibration_curve)
     agent.register_task('set_pid', lake_agent.set_pid)
     agent.register_task('set_autoscan', lake_agent.set_autoscan)
     agent.register_task('set_active_channel', lake_agent.set_active_channel)
     agent.register_task('servo_to_temperature', lake_agent.servo_to_temperature)
     agent.register_task('check_temperature_stability', lake_agent.check_temperature_stability)
     agent.register_task('set_output_mode', lake_agent.set_output_mode)
     agent.register_task('set_heater_output', lake_agent.set_heater_output)
     agent.register_task('set_still_output', lake_agent.set_still_output)
     agent.register_task('get_still_output', lake_agent.get_still_output)
     agent.register_process('acq', lake_agent.acq, lake_agent._stop_acq)
+    agent.register_process('custom_pid', lake_agent.start_custom_pid, lake_agent._stop_custom_pid)
     agent.register_task('enable_control_chan', lake_agent.enable_control_chan)
     agent.register_task('disable_control_chan', lake_agent.disable_control_chan)
     agent.register_task('input_configfile', lake_agent.input_configfile)
 
     runner.run(agent, auto_reconnect=True)
```

### Comparing `socs-0.4.1rc0/socs/agents/lakeshore425/agent.py` & `socs-0.4.2/socs/agents/lakeshore425/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/magpie/agent.py` & `socs-0.4.2/socs/agents/magpie/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/meinberg_m1000/agent.py` & `socs-0.4.2/socs/agents/meinberg_m1000/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/ocs_plugin_so.py` & `socs-0.4.2/socs/agents/ocs_plugin_so.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         ('PfeifferTC400Agent', 'pfeiffer_tc400/agent.py'),
         ('PysmurfController', 'pysmurf_controller/agent.py'),
         ('PysmurfMonitor', 'pysmurf_monitor/agent.py'),
         ('RotationAgent', 'hwp_rotation/agent.py'),
         ('ScpiPsuAgent', 'scpi_psu/agent.py'),
         ('SmurfFileEmulator', 'smurf_file_emulator/agent.py'),
         ('SmurfStreamSimulator', 'smurf_stream_simulator/agent.py'),
+        ('SmurfTimingCardAgent', 'smurf_timing_card/agent.py'),
         ('SupRsync', 'suprsync/agent.py'),
         ('SynaccessAgent', 'synacc/agent.py'),
         ('SynthAgent', 'holo_synth/agent.py'),
         ('TektronixAWGAgent', 'tektronix3021c/agent.py'),
         ('ThorlabsMC2000BAgent', 'thorlabs_mc2000b/agent.py'),
         ('UPSAgent', 'ups/agent.py'),
         ('VantagePro2Agent', 'vantagepro2/agent.py'),
```

### Comparing `socs-0.4.1rc0/socs/agents/pfeiffer_tc400/agent.py` & `socs-0.4.2/socs/agents/pfeiffer_tc400/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/pfeiffer_tc400/drivers.py` & `socs-0.4.2/socs/agents/pfeiffer_tc400/drivers.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/pfeiffer_tpg366/agent.py` & `socs-0.4.2/socs/agents/pfeiffer_tpg366/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/pysmurf_controller/agent.py` & `socs-0.4.2/socs/agents/pysmurf_controller/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/pysmurf_monitor/agent.py` & `socs-0.4.2/socs/agents/pysmurf_monitor/agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -147,20 +147,27 @@
 
             feed_data = {'block_name': field_name,
                          'timestamp': data['time'],
                          'data': {field_name: val}}
 
             self.agent.publish_to_feed(feed_name, feed_data, from_reactor=True)
 
+    @ocs_agent.param('test_mode', default=False, type=bool)
     def run(self, session, params=None):
-        """run()
+        """run(test_mode=False)
 
         **Process** - Main process for the pysmurf monitor agent. Processes
         files that have been added to the queue, adding them to the suprsync
         database.
+
+        Parameters:
+            test_mode (bool, optional):
+                Stop the Process loop after processing any file(s).
+                This is meant only for testing. Default is False.
+
         """
         srfm = SupRsyncFilesManager(self.db_path, create_all=True, echo=self.echo_sql)
 
         self.running = True
         session.set_status('running')
         while self.running:
             files = []
@@ -199,19 +206,25 @@
                         meta=meta, e=e
                     )
 
             if files:
                 with srfm.Session.begin() as session:
                     session.add_all(files)
 
+            if params['test_mode']:
+                break
+
             time.sleep(1)
 
+        return True, 'Monitor exited cleanly.'
+
     def _stop(self, session, params=None):
         self.running = False
         session.set_status('stopping')
+        return True, 'Done monitoring.'
 
 
 def make_parser(parser=None):
     if parser is None:
         parser = argparse.ArgumentParser()
 
     pgroup = parser.add_argument_group('Agent Options')
@@ -219,27 +232,36 @@
                         help="Port for upd-publisher")
     pgroup.add_argument('--create-table', type=bool,
                         help="Specifies whether agent should create or update "
                              "pysmurf_files table if non exists.", default=True)
     pgroup.add_argument('--db-path', type=str, default='/data/so/databases/suprsync.db',
                         help="Path to suprsync sqlite database")
     pgroup.add_argument('--echo-sql', action='store_true')
+    pgroup.add_argument("--test-mode", action='store_true',
+                        help="Specifies whether agent should run in test mode, "
+                        "meaning it shuts down after processing any file(s).")
     return parser
 
 
 def main(args=None):
     parser = make_parser()
     args = site_config.parse_args(agent_class='PysmurfMonitor',
                                   parser=parser,
                                   args=args)
 
     agent, runner = ocs_agent.init_site_agent(args)
     monitor = PysmurfMonitor(agent, args)
 
-    agent.register_process('run', monitor.run, monitor._stop, startup=True)
+    # do not run at startup if in 'test-mode'
+    run_startup = True
+    if args.test_mode:
+        run_startup = False
+
+    agent.register_process('run', monitor.run, monitor._stop,
+                           startup=run_startup)
 
     reactor.listenUDP(args.udp_port, monitor)
 
     runner.run(agent, auto_reconnect=True)
 
 
 if __name__ == '__main__':
```

### Comparing `socs-0.4.1rc0/socs/agents/scpi_psu/agent.py` & `socs-0.4.2/socs/agents/scpi_psu/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/scpi_psu/drivers.py` & `socs-0.4.2/socs/agents/scpi_psu/drivers.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/smurf_crate_monitor/agent.py` & `socs-0.4.2/socs/agents/smurf_crate_monitor/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/smurf_file_emulator/agent.py` & `socs-0.4.2/socs/agents/smurf_file_emulator/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -145,24 +145,26 @@
 
 class G3FrameGenerator:
     """
     Helper class for generating G3 Streams.
     """
 
     def __init__(self, stream_id, sample_rate, tune,
-                 action=None, action_time=None):
+                 action=None, action_time=None, quantize=True, drop_chance=0):
         self.frame_num = 0
         self.sample_num = 0
         self.session_id = int(time.time())
         self.tune = tune
         self.nchans = np.sum(tune.channels != -1)
         self.sample_rate = sample_rate
         self.stream_id = stream_id
         self.action = action
         self.action_time = action_time
+        self.quantize = quantize
+        self.drop_chance = drop_chance
 
     def tag_frame(self, fr):
         fr['frame_num'] = self.frame_num
         fr['session_id'] = self.session_id
         fr['sostream_id'] = self.stream_id
         fr['sostream_version'] = SOSTREAM_VERSION
         fr['time'] = core.G3Time(time.time() * core.G3Units.s)
@@ -177,21 +179,24 @@
 
     def get_obs_end_frame(self):
         fr = core.G3Frame(core.G3FrameType.Observation)
         fr['stream_placement'] = 'end'
         self.tag_frame(fr)
         return fr
 
-    def get_status_frame(self):
+    def get_status_frame(self, tag=''):
         fr = core.G3Frame(core.G3FrameType.Wiring)
         s = get_smurf_status()
 
         tune_key = 'AMCc.FpgaTopLevel.AppTop.AppCore.SysgenCryo.tuneFilePath'
         s[tune_key] = self.tune.tune_path
 
+        tag_key = 'AMCc.SmurfProcessor.SOStream.stream_tag'
+        s[tag_key] = tag
+
         m = self.tune.channels != -1
         chmask = self.tune.channels[m] + self.tune.bands[m] * CHANS_PER_BAND
 
         s['AMCc.SmurfProcessor.ChannelMapper.Mask'] = str(chmask.tolist())
         s['AMCc.SmurfProcessor.ChannelMapper.NumChannels'] = self.nchans.item()
 
         pysmurf_root = "AMCc.SmurfProcessor.SOStream"
@@ -202,28 +207,45 @@
 
         fr['status'] = yaml.dump(s)
         fr['dump'] = True
         self.tag_frame(fr)
         return fr
 
     def get_data_frame(self, start, stop):
+        if self.quantize:
+            # When "quantized", this clamps (start) and (stop) to integers so
+            # timestamps created by np.arange are lined up when there's an
+            # integer sample rate
+            t0, t1 = int(start) - 1, int(stop) + 1
+            nsamp = int((t1 - t0) * self.sample_rate)
+            times = np.linspace(t0, t1, nsamp + 1, endpoint=True)
+            m = (start <= times) & (times < stop)
+            times = times[m]
+        else:
+            times = np.arange(start, stop, 1. / self.sample_rate)
 
-        times = np.arange(start, stop, 1. / self.sample_rate)
         nsamps = len(times)
         frame_counter = np.arange(self.sample_num, self.sample_num + nsamps, dtype=int)
         self.sample_num += nsamps
         chans = np.arange(self.nchans)
         names = [f'r{ch:0>4}' for ch in chans]
 
         count_per_phi0 = 2**16
         data = np.zeros((self.nchans, nsamps), dtype=np.int32)
         data += count_per_phi0 * chans[:, None]
         data += (count_per_phi0 * 0.2 * np.sin(2 * np.pi * 8 * times)).astype(int)
         data += (count_per_phi0 * np.random.normal(0, 0.03, (self.nchans, nsamps))).astype(int)
 
+        # Toss samples based on drop_chance
+        m = self.drop_chance < np.random.uniform(0, 1, len(times))
+        times = times[m]
+        frame_counter = frame_counter[m]
+        data = data[:, m]
+        nsamps = len(times)
+
         fr = core.G3Frame(core.G3FrameType.Scan)
 
         g3times = core.G3VectorTime(times * core.G3Units.s)
         fr['data'] = so3g.G3SuperTimestream(names, g3times, data)
 
         primary_data = np.zeros((len(primary_names), nsamps), dtype=np.int64)
         primary_data[primary_idxs['UnixTime'], :] = (times * 1e9).astype(int)
@@ -243,26 +265,31 @@
 
 class DataStreamer:
     """
     Helper class for streaming G3 data
     """
 
     def __init__(self, stream_id, sample_rate, tune, timestreamdir,
-                 file_duration, frame_len, action=None, action_time=None):
+                 file_duration, frame_len, action=None, action_time=None, drop_chance=0,
+                 tag=''):
         self.frame_gen = G3FrameGenerator(stream_id, sample_rate, tune,
-                                          action=action, action_time=action_time)
+                                          action=action, action_time=action_time,
+                                          drop_chance=drop_chance)
+
         self.session_id = self.frame_gen.session_id
         self.stream_id = stream_id
         self.timestreamdir = timestreamdir
         self.seq = 0
         self.file_duration = file_duration
         self.file_start = 0
         self.writer = None
         self.file_list = []
         self.frame_len = frame_len
+        self.tag = tag
+        self._last_stop = None
 
     def _get_g3_filename(self):
         """
         Returns the file path for a g3-file with specified session id and seq
         idx.
         """
         timecode = f"{self.session_id}"[:5]
@@ -277,15 +304,15 @@
         """
         self.end_file()
         fname = self._get_g3_filename()
         os.makedirs(os.path.dirname(fname), exist_ok=True)
         self.writer = core.G3Writer(fname)
         if self.seq == 0:
             self.writer(self.frame_gen.get_obs_start_frame())
-            self.writer(self.frame_gen.get_status_frame())
+            self.writer(self.frame_gen.get_status_frame(tag=self.tag))
         self.file_start = time.time()
         self.file_list.append(fname)
         self.seq += 1
 
     def end_file(self):
         """
         Ends the current file by sending a G3EndProcessing Frame.
@@ -296,19 +323,24 @@
 
     def write_next(self):
         """
         Writes the next data frame to disk. Will rotate files based on the
         current file start time and the file duration. This sleep wait
         for the frame-duration before writing the G3Frame to disk.
         """
-        start = time.time()
+        if self._last_stop is None:
+            start = time.time()
+        else:
+            start = self._last_stop
+
         if (start - self.file_start > self.file_duration) or (self.writer is None):
             self._new_file()
         time.sleep(self.frame_len)
         stop = time.time()
+        self._last_stop = stop
         self.writer(self.frame_gen.get_data_frame(start, stop))
 
     def stream_between(self, start, stop, wait=False):
         """
         This function will create a new observation and "stream" data between
         a specified start and stop time. This function will by default generate
         and write the data without sleeping for the specified amount of time.
@@ -334,15 +366,15 @@
 
         self._new_file()
         for t0, t1 in zip(frame_starts, frame_stops):
             if wait:
                 now = time.time()
                 if now < t1:
                     time.sleep(t1 - now)
-            self.writer(self.frame_gen.get_data_frame(start, stop))
+            self.writer(self.frame_gen.get_data_frame(t0, t1))
         self.end_file()
 
 
 class SmurfFileEmulator:
     """
     OCS Agent for emulating file creation for the smurf system.
     """
@@ -356,23 +388,25 @@
             raise ValueError(f"Basedir {self.basedir} does not exist")
 
         self.smurfdir = os.path.join(self.basedir, 'smurf')
         self.timestreamdir = os.path.join(self.basedir, 'timestreams')
         self.nchans = args.nchans
         self.sample_rate = args.sample_rate
         self.frame_len = args.frame_len
+        self.drop_chance = args.drop_chance
 
         self.streaming = False
         self.tune = None
 
-    def _new_streamer(self, action=None, action_time=None):
+    def _new_streamer(self, action=None, action_time=None, tag=''):
         return DataStreamer(
             self.stream_id, self.sample_rate, self.tune, self.timestreamdir,
             self.file_duration, self.frame_len,
-            action=action, action_time=action_time,
+            action=action, action_time=action_time, drop_chance=self.drop_chance,
+            tag=tag
         )
 
     def _get_action_dir(self, action, action_time=None, is_plot=False):
         t = int(time.time())
         if action_time is None:
             action_time = t
         action_time = int(action_time)
@@ -457,29 +491,37 @@
         # Short g3 stream
         streamer = self._new_streamer(action=action, action_time=action_time)
         now = time.time()
         streamer.stream_between(now, now + 30, wait=False)
         if session is not None:
             session.data['noise_file'] = streamer.file_list[0]
 
+    @ocs_agent.param('sleep', default=True)
     def uxm_setup(self, session, params):
-        """uxm_setup(test_mode=False)
+        """uxm_setup(sleep=True)
 
         **Task** - Emulates files that might come from a general tune dets
         function. These are some of the files found on simons1 registered when
         running the following ops with a single band:
 
              1. Find-freq
              2. setup_notches
              3. tracking_setup
              4. short g3 stream
+
+        Parameters:
+            sleep (bool, optional):
+                If True, will sleep for 1 sec after creating the tunefile,
+                which is required for preventing filename collisions in
+                end-to-end testing.
         """
         self._run_setup(action='uxm_setup', action_time=time.time(),
                         session=session)
-        time.sleep(1)
+        if params.get('sleep', True):
+            time.sleep(1)
         return True, "Wrote tune files"
 
     def take_noise(self, session, params=None):
         """take_noise()
 
         **Task** - Takes a short noise timestream
         """
@@ -566,27 +608,37 @@
 
         **Task** - Creates files associated with biasing dets, which is none.
         """
         time.sleep(1)
         return True, 'Wrote det biasing files'
 
     @ocs_agent.param('duration', default=None)
+    @ocs_agent.param('use_stream_between', default=False, type=bool)
+    @ocs_agent.param('start_offset', default=0, type=float)
     def stream(self, session, params):
         """stream(duration=None)
 
         **Process** - Generates example fake-files organized in the same way as
         they would be a regular smurf-stream. For end-to-end testing, we want
         an example of a pysmurf-ancilliary file, and then regular g3 that rotate
         at regular intervals. The content of the files here don't match what
         actual G3 or pysmurf files look like, however the directory structure
         is the same.
 
         Parameters:
             duration (float, optional):
                 If set, will stop stream after specified amount of time (sec).
+            use_stream_between (bool, optional):
+                If True, will use the DataStreamer's `stream_between` function
+                instead of writing frames one at a time. This allows you to write
+                an entire timestream for the specified duration without waiting.
+            start_offset (float, optional):
+                If set, this will add an offset to the start time passed to the
+                `stream_between` function, allowing you to create offsets between
+                streams taken at the same time.
         """
         session.set_status('starting')
 
         if self.tune is None:
             raise ValueError("No tune loaded!")
 
         # Write initial smurf metadata
@@ -596,23 +648,28 @@
             action = 'stream_g3_on'
 
         action_time = time.time()
         files = ['freq.txt', 'mask.txt']
         for f in files:
             self._write_smurf_file(f, action, action_time=action_time)
 
+        start_time = time.time() + params['start_offset']
         end_time = None
         if params.get('duration') is not None:
-            end_time = time.time() + params['duration']
+            end_time = start_time + params['duration']
 
         session.set_status('running')
-        streamer = self._new_streamer(action=action, action_time=action_time)
+        streamer = self._new_streamer(action=action, action_time=action_time, tag='obs,cmb')
         session.data['session_id'] = streamer.session_id
         session.data['g3_files'] = streamer.file_list
 
+        if params['use_stream_between']:
+            streamer.stream_between(start_time, end_time)
+            return True, "Finished Stream"
+
         self.streaming = True
         while self.streaming:
             streamer.write_next()
 
             if end_time is not None:
                 if time.time() > end_time:
                     break
@@ -644,14 +701,16 @@
                         help="Time in sec before rotating g3 files")
     pgroup.add_argument('--nchans', default=1024, type=int,
                         help="Number of channels to stream from")
     pgroup.add_argument('--sample-rate', default=200, type=float,
                         help="Sample rate for streaming data")
     pgroup.add_argument('--frame-len', default=2, type=float,
                         help="Time per G3 data frame (seconds)")
+    pgroup.add_argument('--drop-chance', default=0, type=float,
+                        help="Fractional chance to drop samples")
 
     return parser
 
 
 def main(args=None):
     parser = make_parser()
     args = site_config.parse_args(agent_class='SmurfFileEmulator',
```

### Comparing `socs-0.4.1rc0/socs/agents/smurf_file_emulator/status_sample.yaml` & `socs-0.4.2/socs/agents/smurf_file_emulator/status_sample.yaml`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/smurf_stream_simulator/agent.py` & `socs-0.4.2/socs/agents/smurf_stream_simulator/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/suprsync/agent.py` & `socs-0.4.2/socs/agents/suprsync/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/synacc/agent.py` & `socs-0.4.2/socs/agents/synacc/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/tektronix3021c/agent.py` & `socs-0.4.2/socs/agents/tektronix3021c/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/ups/agent.py` & `socs-0.4.2/socs/agents/ups/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,18 +102,21 @@
 
     The OID Value Cache is used to store each unique OID and will be passed to
     session.data
 
     The cache consists of a dictionary, with the unique OIDs as keys, and
     another dictionary as the value. Each of these nested dictionaries contains the
     OID values, name, and description (decoded string). An example for a single OID::
+
         {"upsBatteryStatus":
             {"status": 2,
                 "description": "batteryNormal"}}
+
     Additionally there is connection status and timestamp information under::
+
         {"ups_connection":
             {"last_attempt": 1598543359.6326838,
             "connected": True}
         {"timestamp": 1656085022.680916}
 
     Parameters
     ----------
```

### Comparing `socs-0.4.1rc0/socs/agents/vantagepro2/agent.py` & `socs-0.4.2/socs/agents/vantagepro2/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/vantagepro2/drivers.py` & `socs-0.4.2/socs/agents/vantagepro2/drivers.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/wiregrid_actuator/agent.py` & `socs-0.4.2/socs/agents/wiregrid_actuator/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/wiregrid_actuator/drivers/Actuator.py` & `socs-0.4.2/socs/agents/wiregrid_actuator/drivers/Actuator.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/wiregrid_actuator/drivers/DigitalIO.py` & `socs-0.4.2/socs/agents/wiregrid_actuator/drivers/DigitalIO.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/wiregrid_actuator/limitswitch_config.py` & `socs-0.4.2/socs/agents/wiregrid_actuator/limitswitch_config.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/wiregrid_encoder/agent.py` & `socs-0.4.2/socs/agents/wiregrid_encoder/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/wiregrid_encoder/drivers.py` & `socs-0.4.2/socs/agents/wiregrid_encoder/drivers.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/wiregrid_kikusui/agent.py` & `socs-0.4.2/socs/agents/wiregrid_kikusui/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/wiregrid_kikusui/drivers/common.py` & `socs-0.4.2/socs/agents/wiregrid_kikusui/drivers/common.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/agents/xy_stage/agent.py` & `socs-0.4.2/socs/agents/xy_stage/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/common/moxa_serial.py` & `socs-0.4.2/socs/common/moxa_serial.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/common/pmx.py` & `socs-0.4.2/socs/common/pmx.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/common/prologix_interface.py` & `socs-0.4.2/socs/common/prologix_interface.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/db/suprsync.py` & `socs-0.4.2/socs/db/suprsync.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,11 +454,11 @@
                         file.removed = time.time()
                     except PermissionError:
                         self.log.error(
                             f"Permission error: Could not remove {file.local_path}"
                         )
                 else:
                     self.log.warn(
-                        "File {file.local_path} no longer exists! "
+                        f"File {file.local_path} no longer exists! "
                         "Updating remove time to be 0"
                     )
                     file.removed = 0
```

### Comparing `socs-0.4.1rc0/socs/mibs/IBOOTPDU-MIB.py` & `socs-0.4.2/socs/mibs/IBOOTPDU-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/mibs/MBG-SNMP-LTNG-MIB.py` & `socs-0.4.2/socs/mibs/MBG-SNMP-LTNG-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/mibs/MBG-SNMP-ROOT-MIB.py` & `socs-0.4.2/socs/mibs/MBG-SNMP-ROOT-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/mibs/SNMPv2-MIB.py` & `socs-0.4.2/socs/mibs/SNMPv2-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/mibs/UPS-MIB.py` & `socs-0.4.2/socs/mibs/UPS-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/plugin.py` & `socs-0.4.2/socs/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     'PfeifferTC400Agent': {'module': 'socs.agents.pfeiffer_tc400.agent', 'entry_point': 'main'},
     'PysmurfController': {'module': 'socs.agents.pysmurf_controller.agent', 'entry_point': 'main'},
     'PysmurfMonitor': {'module': 'socs.agents.pysmurf_monitor.agent', 'entry_point': 'main'},
     'RotationAgent': {'module': 'socs.agents.hwp_rotation.agent', 'entry_point': 'main'},
     'ScpiPsuAgent': {'module': 'socs.agents.scpi_psu.agent', 'entry_point': 'main'},
     'SmurfFileEmulator': {'module': 'socs.agents.smurf_file_emulator.agent', 'entry_point': 'main'},
     'SmurfStreamSimulator': {'module': 'socs.agents.smurf_stream_simulator.agent', 'entry_point': 'main'},
+    'SmurfTimingCardAgent': {'module': 'socs.agents.smurf_timing_card.agent', 'entry_point': 'main'},
     'SupRsync': {'module': 'socs.agents.suprsync.agent', 'entry_point': 'main'},
     'SynaccessAgent': {'module': 'socs.agents.synacc.agent', 'entry_point': 'main'},
     'SynthAgent': {'module': 'socs.agents.holo_synth.agent', 'entry_point': 'main'},
     'TektronixAWGAgent': {'module': 'socs.agents.tektronix3021c.agent', 'entry_point': 'main'},
     'ThorlabsMC2000BAgent': {'module': 'socs.agents.thorlabs_mc2000b.agent', 'entry_point': 'main'},
     'UPSAgent': {'module': 'socs.agents.ups.agent', 'entry_point': 'main'},
     'VantagePro2Agent': {'module': 'socs.agents.vantagepro2.agent', 'entry_point': 'main'},
```

### Comparing `socs-0.4.1rc0/socs/snmp.py` & `socs-0.4.2/socs/snmp.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/socs/testing/device_emulator.py` & `socs-0.4.2/socs/testing/device_emulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,15 +221,21 @@
             port (int): Port for the TCP relay to listen for connections on.
 
         """
         self._read = True
 
         # Listen for connections
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self._sock.bind(('127.0.0.1', port))
+        while not self._sock_bound:
+            try:
+                self._sock.bind(('127.0.0.1', port))
+                self._sock_bound = True
+            except OSError:
+                print(f"Failed to bind to port {port}, trying again...")
+                time.sleep(1)
         self._sock.listen(1)
         print("Device emulator waiting for tcp client connection")
         self._conn, client_address = self._sock.accept()
         print(f"Client connection made from {client_address}")
 
         while self._read:
             try:
@@ -270,21 +276,32 @@
         background. This allows responses to be defined within a test using
         DeviceEmulator.define_responses() after instantiation of the
         DeviceEmulator object within a given test.
 
         Args:
             port (int): Port for the TCP relay to listen for connections on.
 
+        Notes:
+            This will not return until the socket is properly bound to the
+            given port. If this setup is not working it is likely another
+            device emulator instance is not yet finished or has not been
+            properly shutdown.
+
         """
         self._type = 'tcp'
+        self._sock_bound = False
         bkg_read = threading.Thread(name='background',
                                     target=self._read_socket,
                                     kwargs={'port': port})
         bkg_read.start()
 
+        # wait for socket to bind properly before returning
+        while not self._sock_bound:
+            time.sleep(0.1)
+
     def define_responses(self, responses, default_response=None):
         """Define what responses are available to reply with on the configured
         communication relay.
 
         Args:
             responses (dict): Dictionary of commands: response. Values can be a
                 list, in which case the responses in the list are popped and
```

### Comparing `socs-0.4.1rc0/socs.egg-info/PKG-INFO` & `socs-0.4.2/socs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socs
-Version: 0.4.1rc0
+Version: 0.4.2
 Summary: Simons Observatory Control System
 Home-page: https://github.com/simonsobs/socs
 Project-URL: Source Code, https://github.com/simonsobs/ocs
 Project-URL: Documentation, https://ocs.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/simonsobs/ocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -15,40 +15,41 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: labjack
 Provides-Extra: magpie
 Provides-Extra: pfeiffer
 Provides-Extra: smurf_sim
 Provides-Extra: synacc
+Provides-Extra: timing_master
 License-File: LICENSE.txt
 
 ========================================
 SOCS - Simons Observatory Control System
 ========================================
 
-.. image:: https://img.shields.io/github/actions/workflow/status/simonsobs/socs/develop.yml?branch=develop
-    :target: https://github.com/simonsobs/socs/actions?query=workflow%3A%22Build+Develop+Images%22
+.. image:: https://img.shields.io/github/actions/workflow/status/simonsobs/socs/develop.yml?branch=main
+    :target: https://github.com/simonsobs/socs/actions?query=workflow%3A%22Build+Test+Images%22
     :alt: GitHub Workflow Status
 
-.. image:: https://readthedocs.org/projects/socs/badge/?version=develop
-    :target: https://socs.readthedocs.io/en/develop/?badge=develop
+.. image:: https://readthedocs.org/projects/socs/badge/?version=main
+    :target: https://socs.readthedocs.io/en/main/?badge=main
     :alt: Documentation Status
 
-.. image:: https://coveralls.io/repos/github/simonsobs/socs/badge.svg?branch=develop
-    :target: https://coveralls.io/github/simonsobs/socs?branch=develop
+.. image:: https://coveralls.io/repos/github/simonsobs/socs/badge.svg
+    :target: https://coveralls.io/github/simonsobs/socs
 
 .. image:: https://img.shields.io/badge/dockerhub-latest-blue
     :target: https://hub.docker.com/r/simonsobs/ocs/tags
 
 .. image:: https://img.shields.io/pypi/v/socs
    :target: https://pypi.org/project/socs/
    :alt: PyPI Package
 
-.. image:: https://results.pre-commit.ci/badge/github/simonsobs/socs/develop.svg
-   :target: https://results.pre-commit.ci/latest/github/simonsobs/socs/develop
+.. image:: https://results.pre-commit.ci/badge/github/simonsobs/socs/main.svg
+   :target: https://results.pre-commit.ci/latest/github/simonsobs/socs/main
    :alt: pre-commit.ci status
 
 Overview
 --------
 
 This repository, `SOCS`_, contains hardware control code for the
 Simons Observatory.  This code operates within the framework provided
@@ -75,22 +76,22 @@
 "all"::
 
     $ pip3 install -U socs[all]
 
 **Note:** Not all optional dependencies can be installed this way. See the
 `Installation Documentation`_ for more info on specific agent dependencies.
 
-.. _`Installation Documentation`: https://socs.readthedocs.io/en/develop/user/installation.html
+.. _`Installation Documentation`: https://socs.readthedocs.io/en/main/user/installation.html
 
 Installing from Source
 ``````````````````````
 
-If you are considering contributing to SOCS, or would like to use the
-development branch, you will want to install from source. To do so,
-clone the repository and install using pip:
+If you are considering contributing to SOCS, or would like to use an unreleased
+feature, you will want to install from source. To do so, clone this repository
+and install using pip:
 
 .. code-block:: bash
 
     git clone https://github.com/simonsobs/socs.git
     cd socs/
     pip3 install -r requirements.txt
     pip3 install .
@@ -105,28 +106,28 @@
   # List of additional paths to Agent plugin modules.
   'agent-paths': [
     '/path/to/socs/agents/',
   ],
 
 See the `ocs docs`_ for more details.
 
-.. _`ocs docs`: https://ocs.readthedocs.io/en/develop/developer/site_config.html
+.. _`ocs docs`: https://ocs.readthedocs.io/en/main/developer/site_config.html
 
 Docker Images
 -------------
 Docker images for SOCS and each Agent are available on `Docker Hub`_. Official
 releases will be tagged with their release version, i.e. ``v0.1.0``. These are
 only built on release, and the ``latest`` tag will point to the latest of these
 released tags. These should be considered stable.
 
-Development images will be tagged with the latest released version tag, the
-number of commits ahead of that release, the latest commit hash, and the tag
-``-dev``, i.e.  ``v0.0.2-81-g9c10ba6-dev``. These get built on each commit to
-the ``develop`` branch, and are useful for testing and development, but should
-be considered unstable.
+Test images will be tagged with the latest released version tag, the number of
+commits ahead of that release, the latest commit hash, i.e.
+``v0.0.2-81-g9c10ba6-dev``. These get built on each commit to the ``main``
+branch, and are useful for testing and development, but should be considered
+unstable.
 
 .. _Docker Hub: https://hub.docker.com/u/simonsobs
 
 Documentation
 -------------
 The SOCS documentation can be built using Sphinx. There is a separate
 ``requirements.txt`` file in the ``docs/`` directory to install Sphinx and any
@@ -147,21 +148,21 @@
 ``tests/`` directory::
 
   $ cd tests/
   $ python3 -m pytest --cov
 
 For more details see `tests/README.rst <tests_>`_.
 
-.. _tests: https://github.com/simonsobs/socs/blob/master/tests/README.rst
+.. _tests: https://github.com/simonsobs/socs/blob/main/tests/README.rst
 
 Contributing
 ------------
 For guidelines on how to contribute to OCS see `CONTRIBUTING.rst`_.
 
-.. _CONTRIBUTING.rst: https://github.com/simonsobs/socs/blob/master/CONTRIBUTING.rst
+.. _CONTRIBUTING.rst: https://github.com/simonsobs/socs/blob/main/CONTRIBUTING.rst
 
 License
 --------
 This project is licensed under the BSD 2-Clause License - see the
 `LICENSE.txt`_ file for details.
 
-.. _LICENSE.txt: https://github.com/simonsobs/socs/blob/master/LICENSE.txt
+.. _LICENSE.txt: https://github.com/simonsobs/socs/blob/main/LICENSE.txt
```

### Comparing `socs-0.4.1rc0/socs.egg-info/SOURCES.txt` & `socs-0.4.2/socs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 socs/agents/hwp_picoscope/agent.py
 socs/agents/hwp_picoscope/drivers/__init__.py
 socs/agents/hwp_picoscope/drivers/class_ps3000a.py
 socs/agents/hwp_rotation/__init__.py
 socs/agents/hwp_rotation/agent.py
 socs/agents/hwp_rotation/drivers/__init__.py
 socs/agents/hwp_rotation/drivers/pid_controller.py
+socs/agents/ibootbar/__init__.py
+socs/agents/ibootbar/agent.py
 socs/agents/labjack/__init__.py
 socs/agents/labjack/agent.py
 socs/agents/labjack/cal_curves/GA10K4D25_cal_curve.txt
 socs/agents/lakeshore240/__init__.py
 socs/agents/lakeshore240/agent.py
 socs/agents/lakeshore336/__init__.py
 socs/agents/lakeshore336/agent.py
@@ -79,21 +81,25 @@
 socs/agents/smurf_crate_monitor/__init__.py
 socs/agents/smurf_crate_monitor/agent.py
 socs/agents/smurf_file_emulator/__init__.py
 socs/agents/smurf_file_emulator/agent.py
 socs/agents/smurf_file_emulator/status_sample.yaml
 socs/agents/smurf_stream_simulator/__init__.py
 socs/agents/smurf_stream_simulator/agent.py
+socs/agents/smurf_timing_card/__init__.py
+socs/agents/smurf_timing_card/agent.py
 socs/agents/suprsync/__init__.py
 socs/agents/suprsync/agent.py
 socs/agents/synacc/__init__.py
 socs/agents/synacc/agent.py
 socs/agents/tektronix3021c/__init__.py
 socs/agents/tektronix3021c/agent.py
 socs/agents/tektronix3021c/drivers.py
+socs/agents/thorlabs_mc2000b/__init__.py
+socs/agents/thorlabs_mc2000b/agent.py
 socs/agents/ups/__init__.py
 socs/agents/ups/agent.py
 socs/agents/vantagepro2/__init__.py
 socs/agents/vantagepro2/agent.py
 socs/agents/vantagepro2/drivers.py
 socs/agents/wiregrid_actuator/__init__.py
 socs/agents/wiregrid_actuator/agent.py
```

### Comparing `socs-0.4.1rc0/tests/test_device_emulator.py` & `socs-0.4.2/tests/test_device_emulator.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.1rc0/versioneer.py` & `socs-0.4.2/versioneer.py`

 * *Files identical despite different names*

