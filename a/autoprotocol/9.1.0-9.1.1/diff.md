# Comparing `tmp/autoprotocol-9.1.0.tar.gz` & `tmp/autoprotocol-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/autoprotocol-python/autoprotocol-python/dist/.tmp-yp05gij4/autoprotocol-9.1.0.tar", last modified: Wed Jan  4 21:03:54 2023, max compression
+gzip compressed data, was "/home/runner/work/autoprotocol-python/autoprotocol-python/dist/.tmp-wvoxw9dz/autoprotocol-9.1.1.tar", last modified: Thu Feb  2 21:30:29 2023, max compression
```

## Comparing `autoprotocol-9.1.0.tar` & `autoprotocol-9.1.1.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 21:03:54.000000 autoprotocol-9.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-01-04 21:03:54.000000 autoprotocol-9.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 21:03:54.000000 autoprotocol-9.1.0/autoprotocol/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    96925 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    40288 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    42922 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/container_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    27983 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/harness.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/informatics.py
--rw-r--r--   0 runner    (1001) docker     (123)    59426 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/instruction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 21:03:54.000000 autoprotocol-9.1.0/autoprotocol/liquid_handle/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/liquid_handle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/liquid_handle/dispense.py
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/liquid_handle/liquid_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    27341 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/liquid_handle/liquid_handle_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/liquid_handle/mix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/liquid_handle/tip_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    24740 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/liquid_handle/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)   308761 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 21:03:54.000000 autoprotocol-9.1.0/autoprotocol/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/types/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/types/ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/autoprotocol/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 21:03:54.000000 autoprotocol-9.1.0/autoprotocol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-01-04 21:03:54.000000 autoprotocol-9.1.0/autoprotocol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-01-04 21:03:54.000000 autoprotocol-9.1.0/autoprotocol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 21:03:54.000000 autoprotocol-9.1.0/autoprotocol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-04 21:03:54.000000 autoprotocol-9.1.0/autoprotocol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-04 21:03:54.000000 autoprotocol-9.1.0/autoprotocol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-04 21:03:54.000000 autoprotocol-9.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2825 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 21:03:54.000000 autoprotocol-9.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-04 21:03:44.000000 autoprotocol-9.1.0/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 21:30:29.000000 autoprotocol-9.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-02-02 21:30:29.000000 autoprotocol-9.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 21:30:29.000000 autoprotocol-9.1.1/autoprotocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94250 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40288 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42806 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/container_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27995 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/harness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/informatics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59426 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/instruction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 21:30:29.000000 autoprotocol-9.1.1/autoprotocol/liquid_handle/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/liquid_handle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/liquid_handle/dispense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12938 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/liquid_handle/liquid_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26548 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/liquid_handle/liquid_handle_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/liquid_handle/mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/liquid_handle/tip_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24902 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/liquid_handle/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   308765 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 21:30:29.000000 autoprotocol-9.1.1/autoprotocol/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/types/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/autoprotocol/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 21:30:29.000000 autoprotocol-9.1.1/autoprotocol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-02-02 21:30:29.000000 autoprotocol-9.1.1/autoprotocol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-02 21:30:29.000000 autoprotocol-9.1.1/autoprotocol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 21:30:29.000000 autoprotocol-9.1.1/autoprotocol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-02-02 21:30:29.000000 autoprotocol-9.1.1/autoprotocol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-02 21:30:29.000000 autoprotocol-9.1.1/autoprotocol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-02 21:30:29.000000 autoprotocol-9.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2825 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 21:30:29.000000 autoprotocol-9.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-02 21:30:21.000000 autoprotocol-9.1.1/test/test_util.py
```

### Comparing `autoprotocol-9.1.0/AUTHORS.rst` & `autoprotocol-9.1.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `autoprotocol-9.1.0/LICENSE.rst` & `autoprotocol-9.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `autoprotocol-9.1.0/PKG-INFO` & `autoprotocol-9.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoprotocol
-Version: 9.1.0
+Version: 9.1.1
 Summary: Python library for generating Autoprotocol
 Home-page: https://github.com/autoprotocol/autoprotocol-python
 Maintainer: The Autoprotocol Development Team
 Maintainer-email: support@strateos.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `autoprotocol-9.1.0/README.rst` & `autoprotocol-9.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `autoprotocol-9.1.0/autoprotocol/builders.py` & `autoprotocol-9.1.1/autoprotocol/builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,20 @@
 builders attribute (e.g. `Spectrophotometry.Builders.mode_params`).
 
 See Also
 --------
 Instruction
     Instructions corresponding to each of the builders
 """
-import enum
 
 from collections import defaultdict
 from collections.abc import Iterable  # pylint: disable=no-name-in-module
-from dataclasses import dataclass
 from functools import reduce
 from numbers import Number
-from typing import Any, Dict, List, Optional, Union
+from typing import List, Optional, Union
 
 from .constants import SBS_FORMAT_SHAPES
 from .container import Container, Well, WellGroup
 from .unit import Unit
 from .util import is_valid_well, parse_unit
 
 
@@ -406,31 +404,31 @@
     """
     These builders are meant for helping to construct arguments for the
     `SPE` instruction.
     """
 
     def spe_params(self, params, is_elute=False):
         if not isinstance(params, list):
-            raise ValueError(f"SPE mobile phase parameters {params} must be a list.")
+            raise ValueError("SPE mobile phase parameters {} must be a list.")
         parsed_params = []
         for param in params:
             parsed_params.append(self.mobile_phase_params(is_elute=is_elute, **param))
         return parsed_params
 
     def mobile_phase_params(
         self,
-        volume: Union[str, Unit],
-        loading_flowrate: Union[str, Unit],
-        settle_time: Optional[bool],
-        processing_time: Union[str, Unit],
-        flow_pressure: Union[str, Unit],
-        resource_id: Optional[str] = None,
-        is_sample: bool = False,
-        destination_well: Optional[Well] = None,
-        is_elute: bool = False,
+        volume,
+        loading_flowrate,
+        settle_time,
+        processing_time,
+        flow_pressure,
+        resource_id=None,
+        is_sample=False,
+        destination_well=None,
+        is_elute=False,
     ):
         """
         Create a dictionary with mobile phase parameters which can be
         used as input for instructions.
 
         Parameters
         ----------
@@ -1081,21 +1079,15 @@
         dict
             Formatted mode_params for a shake mode.
         """
         return self._shake(
             duration=duration, frequency=frequency, path=path, amplitude=amplitude
         )
 
-    def shake_before(
-        self,
-        duration: Union[str, Unit],
-        frequency: Optional[Union[str, Unit]] = None,
-        path: Optional[str] = None,
-        amplitude: Optional[Union[str, Unit]] = None,
-    ):
+    def shake_before(self, duration, frequency=None, path=None, amplitude=None):
         """
         Parameters
         ----------
         duration : Unit or str
             The duration of the shaking incubation.
         frequency : Unit or str, optional
             The frequency of the shaking motion.
@@ -2019,51 +2011,42 @@
 
         return {
             "duration": duration,
             "shaking": {"amplitude": amplitude, "orbital": orbital},
         }
 
 
-class EvaporateModeParamsMode(enum.Enum):
-    rotate = enum.auto()
-    centrifuge = enum.auto()
-    vortex = enum.auto()
-    blowdown = enum.auto()
-
-
 class EvaporateBuilders(InstructionBuilders):
     """
     Helpers for building Evaporate instructions
     """
 
     def __init__(self):
         super(EvaporateBuilders, self).__init__()
         self.valid_modes = ["rotate", "centrifuge", "vortex", "blowdown"]
         self.valid_gases = ["nitrogen", "argon", "helium"]
-        self.rotate_params = [
+        self.rotary_params = [
             "flask_volume",
             "rotation_speed",
             "vacuum_pressure",
             "condenser_temperature",
         ]
-        self.centrifuge_params = [
+        self.centrifugal_params = [
             "spin_acceleration",
             "vacuum_pressure",
             "condenser_temperature",
         ]
         self.vortex_params = [
             "vortex_speed",
             "vacuum_pressure",
             "condenser_temperature",
         ]
         self.blowdown_params = ["gas", "blow_rate", "vortex_speed"]
 
-    def get_mode_params(
-        self, mode: EvaporateModeParamsMode, mode_params: Dict[str, Any]
-    ):
+    def get_mode_params(self, mode, mode_params):
         """
         Checks on the validity of mode and mode_params, and
         creates a dictionary for mode_params
 
         Parameters
         ----------
         mode : Str
@@ -2090,16 +2073,16 @@
         ValueError
             If container agitation speed is less than 0.
         ValueError
             If vacuum_pressure is less than 0 torr.
 
         """
         mode_to_param_dict = {
-            "rotate": self.rotate_params,
-            "centrifuge": self.centrifuge_params,
+            "rotary": self.rotary_params,
+            "centrifugal": self.centrifugal_params,
             "vortex": self.vortex_params,
             "blowdown": self.blowdown_params,
         }
         if mode not in self.valid_modes:
             raise ValueError(
                 f"Specified mode: {mode} is not valid. Make sure it is one "
                 f"of {self.valid_modes}"
@@ -2157,40 +2140,18 @@
             if not blow_rate is None:
                 blow_rate = parse_unit(blow_rate, "mL/min")
                 mode_param_output["blow_rate"] = blow_rate
 
         return mode_param_output
 
 
-@dataclass()
-class GelPurifyBandSizeRange:
-    min_bp: int
-    max_bp: int
-
-
-@dataclass
-class GelPurifyBand:
-    elution_buffer: str
-    elution_volume: Union[str, Unit]
-    destination: Well
-    min_bp: Optional[int]
-    max_bp: Optional[int]
-    band_size_range: Optional[GelPurifyBandSizeRange]
-
-
 class GelPurifyBuilders(InstructionBuilders):
     """Helpers for building GelPurify instructions"""
 
-    def extract(
-        self,
-        source: Well,
-        band_list: List[GelPurifyBand],
-        lane: Optional[int] = None,
-        gel: Optional[int] = None,
-    ):
+    def extract(self, source, band_list, lane=None, gel=None):
         """Helper for building extract params for gel_purify
 
         Parameters
         ----------
         source : Well
             The Well that contains the sample be purified
         band_list : list(dict)
@@ -2213,15 +2174,15 @@
         """
         if not isinstance(source, Well):
             raise TypeError(f"source: {source} is not a Well")
 
         if not isinstance(band_list, list):
             band_list = [band_list]
 
-        band_list = [self.band(**i) for i in band_list]
+        band_list = [self.band(**_) for _ in band_list]
 
         return {"source": source, "band_list": band_list, "lane": lane, "gel": gel}
 
     def band(
         self,
         elution_buffer,
         elution_volume,
@@ -2582,75 +2543,24 @@
             "center": center,
             "amplitude": amplitude,
             "magnetize": magnetize,
             "temperature": temperature,
         }
 
 
-class FlowCytometryChannelTriggerLogicEnum(enum.Enum):
-    and_ = enum.auto()
-    or_ = enum.auto()
-
-
-@dataclass
-class FlowCytometryChannelTriggerLogic:
-    value: FlowCytometryChannelTriggerLogicEnum
-
-    def __post_init__(self):
-        trigger_modes = ("and_", "or_")
-        if self.value is not None and self.value not in trigger_modes:
-            raise ValueError(f"trigger_logic must be one of {trigger_modes}.")
-
-
-@dataclass
-class FlowCytometryChannelMeasurments:
-    area: Optional[bool] = None
-    height: Optional[bool] = None
-    width: Optional[bool] = None
-
-
-@dataclass
-class FlowCytometryChannelEmissionFilter:
-    channel_name: str
-    shortpass: Union[str, Unit] = None
-    longpass: Union[str, Unit] = None
-
-
-@dataclass
-class FlowCytometryChannel:
-    emission_filter: FlowCytometryChannelEmissionFilter
-    detector_gain: Union[str, Unit]
-    measurements: Optional[FlowCytometryChannelMeasurments] = None
-    trigger_threshold: Optional[int] = None
-    trigger_logic: Optional[FlowCytometryChannelTriggerLogic] = None
-
-
-@dataclass()
-class FlowCytometryCollectionConditionStopCriteria:
-    volume: Optional[Union[str, Unit]] = None
-    events: Optional[int] = None
-    time: Union[str, Unit] = None
-
-
 class FlowCytometryBuilders(InstructionBuilders):
     """
     Builders for FlowCytometry instructions.
     """
 
     def __init__(self):
         super(FlowCytometryBuilders, self).__init__()
         self.gating_modes = ("FSC", "SSC")
 
-    def laser(
-        self,
-        channels: List[FlowCytometryChannel],
-        excitation: Union[str, Unit] = None,
-        power: Union[str, Unit] = None,
-        area_scaling_factor: Optional[int] = None,
-    ):
+    def laser(self, channels, excitation=None, power=None, area_scaling_factor=None):
         """
         Generates a dict of laser parameters.
 
         Parameters
         ----------
         channels : list(dict)
             See :meth:`FlowCytometryBuilders.channel`.
@@ -2690,15 +2600,15 @@
 
         if power is not None:
             power = parse_unit(power, "milliwatts")
 
         if excitation is not None:
             excitation = parse_unit(excitation, "nanometers")
 
-        channels = [self.channel(**c) for c in channels]
+        channels = [self.channel(**_) for _ in channels]
 
         # Gating modes do not allow specification of excitation parameter
         channel_names = set(
             [chn["emission_filter"]["channel_name"] for chn in channels]
         )
         if channel_names.intersection(self.gating_modes) and excitation is not None:
             raise ValueError(
@@ -2710,19 +2620,19 @@
             "power": power,
             "area_scaling_factor": area_scaling_factor,
             "channels": channels,
         }
 
     def channel(
         self,
-        emission_filter: FlowCytometryChannelEmissionFilter,
-        detector_gain: Union[str, Unit],
-        measurements: Optional[FlowCytometryChannelMeasurments] = None,
-        trigger_threshold: Optional[int] = None,
-        trigger_logic: Optional[FlowCytometryChannelTriggerLogic] = None,
+        emission_filter,
+        detector_gain,
+        measurements=None,
+        trigger_threshold=None,
+        trigger_logic=None,
     ):
         """
         Generates a dict of channel parameters.
 
         Parameters
         ----------
         emission_filter : dict
@@ -2748,14 +2658,18 @@
         -------
         dict
             A dict of channel parameters.
         """
         if trigger_threshold is not None and not isinstance(trigger_threshold, int):
             raise TypeError("trigger_threshold must be of type int.")
 
+        trigger_modes = ("and", "or")
+        if trigger_logic is not None and trigger_logic not in trigger_modes:
+            raise ValueError(f"trigger_logic must be one of {trigger_modes}.")
+
         if measurements is None:
             measurements = self.measurements()
         else:
             measurements = self.measurements(**measurements)
 
         emission_filter = self.emission_filter(**emission_filter)
         detector_gain = parse_unit(detector_gain, "millivolts")
@@ -2764,20 +2678,15 @@
             "emission_filter": emission_filter,
             "detector_gain": detector_gain,
             "measurements": measurements,
             "trigger_threshold": trigger_threshold,
             "trigger_logic": trigger_logic,
         }
 
-    def emission_filter(
-        self,
-        channel_name: str,
-        shortpass: Union[str, Unit] = None,
-        longpass: Union[str, Unit] = None,
-    ):
+    def emission_filter(self, channel_name, shortpass=None, longpass=None):
         """
         Generates a dict of emission filter parameters.
 
         Parameters
         ----------
         channel_name : str
             Specifies the channel name.
@@ -2814,19 +2723,15 @@
         return {
             "channel_name": channel_name,
             "shortpass": shortpass,
             "longpass": longpass,
         }
 
     @staticmethod
-    def measurements(
-        area: Optional[bool] = None,
-        height: Optional[bool] = None,
-        width: Optional[bool] = None,
-    ):
+    def measurements(area=None, height=None, width=None):
         """
         Generates a dict of measurements parameters.
 
         Parameters
         ----------
         area : bool, optional
             Area measurement.
@@ -2849,21 +2754,21 @@
         if any(not isinstance(_, (bool, type(None))) for _ in (area, height, width)):
             raise TypeError("area, height, and width must be of type bool.")
 
         return {"area": area, "height": height, "width": width}
 
     def collection_conditions(
         self,
-        acquisition_volume: Union[str, Unit],
-        flowrate: Union[str, Unit],
-        wait_time: Union[str, Unit],
-        mix_cycles: int,
-        mix_volume: Union[str, Unit],
-        rinse_cycles: int,
-        stop_criteria: Optional[FlowCytometryCollectionConditionStopCriteria],
+        acquisition_volume,
+        flowrate,
+        wait_time,
+        mix_cycles,
+        mix_volume,
+        rinse_cycles,
+        stop_criteria=None,
     ):
         """
         Generates a dict of collection_conditions parameters.
 
         Parameters
         ----------
         acquisition_volume : Unit or str
@@ -2916,19 +2821,15 @@
             "wait_time": wait_time,
             "mix_cycles": mix_cycles,
             "mix_volume": mix_volume,
             "rinse_cycles": rinse_cycles,
         }
 
     @staticmethod
-    def stop_criteria(
-        volume: Optional[Union[str, Unit]] = None,
-        events: Optional[int] = None,
-        time: Union[str, Unit] = None,
-    ):
+    def stop_criteria(volume=None, events=None, time=None):
         """
         Generates a dict of stop_criteria parameters.
 
         Parameters
         ----------
         volume : Unit or str, optional
             Stopping volume.
```

### Comparing `autoprotocol-9.1.0/autoprotocol/compound.py` & `autoprotocol-9.1.1/autoprotocol/compound.py`

 * *Files identical despite different names*

### Comparing `autoprotocol-9.1.0/autoprotocol/constants.py` & `autoprotocol-9.1.1/autoprotocol/constants.py`

 * *Files identical despite different names*

### Comparing `autoprotocol-9.1.0/autoprotocol/container.py` & `autoprotocol-9.1.1/autoprotocol/container.py`

 * *Files identical despite different names*

### Comparing `autoprotocol-9.1.0/autoprotocol/container_type.py` & `autoprotocol-9.1.1/autoprotocol/container_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,15 +461,14 @@
         "liquid_handle",
         "seal",
         "spin",
         "incubate",
         "dispense",
         "cover",
         "provision",
-        "acoustic_transfer",
     ],
     shortname="384-echo",
     col_count=24,
     dead_volume_ul=Unit(15, "microliter"),
     safe_min_volume_ul=Unit(15, "microliter"),
     true_max_vol_ul=Unit(135, "microliter"),
     vendor="Labcyte",
@@ -1254,15 +1253,14 @@
         "liquid_handle",
         "seal",
         "spin",
         "incubate",
         "dispense",
         "cover",
         "provision",
-        "acoustic_transfer",
     ],
     shortname="384-echo-ldv",
     col_count=24,
     dead_volume_ul=Unit(2.5, "microliter"),
     safe_min_volume_ul=Unit(2.5, "microliter"),
     vendor="Labcyte",
     cat_no="LP-0200",
@@ -1284,15 +1282,14 @@
         "liquid_handle",
         "seal",
         "spin",
         "incubate",
         "dispense",
         "cover",
         "provision",
-        "acoustic_transfer",
     ],
     shortname="384-echo-ldv-plus",
     col_count=24,
     dead_volume_ul=Unit(4.5, "microliter"),
     safe_min_volume_ul=Unit(4.5, "microliter"),
     vendor="Labcyte",
     cat_no="LPL-0200",
@@ -1314,15 +1311,14 @@
         "liquid_handle",
         "seal",
         "spin",
         "incubate",
         "dispense",
         "cover",
         "provision",
-        "acoustic_transfer",
     ],
     shortname="1536-echo-ldv-beckman-001-6969",
     col_count=48,
     dead_volume_ul=Unit(1, "microliter"),
     safe_min_volume_ul=Unit(1, "microliter"),
     true_max_vol_ul=Unit(5.5, "microliter"),
     vendor="Beckman",
```

### Comparing `autoprotocol-9.1.0/autoprotocol/harness.py` & `autoprotocol-9.1.1/autoprotocol/harness.py`

 * *Files 1% similar despite different names*

```diff
@@ -796,15 +796,15 @@
                   "op": "seal"
                 }
               ]
             }
 
     """
     for _, ref in protocol.refs.items():
-        if ref.opts.store:
+        if "store" in ref.opts.keys():
             if not (ref.container.is_covered() or ref.container.is_sealed()):
                 default_method = ref.container.container_type.prioritize_seal_or_cover
                 sealable = "seal" in ref.container.container_type.capabilities
                 coverable = "cover" in ref.container.container_type.capabilities
                 if default_method == "seal" and sealable:
                     protocol.seal(
                         ref.container, ref.container.container_type.seal_types[0]
```

### Comparing `autoprotocol-9.1.0/autoprotocol/informatics.py` & `autoprotocol-9.1.1/autoprotocol/informatics.py`

 * *Files identical despite different names*

### Comparing `autoprotocol-9.1.0/autoprotocol/instruction.py` & `autoprotocol-9.1.1/autoprotocol/instruction.py`

 * *Files identical despite different names*

### Comparing `autoprotocol-9.1.0/autoprotocol/liquid_handle/dispense.py` & `autoprotocol-9.1.1/autoprotocol/liquid_handle/dispense.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """Dispense LiquidHandleMethod
 
 Base LiquidHandleMethod used by Protocol.liquid_handle_dispense to generate a
 series of movements that define a dispense from a source into a destination
 """
-from dataclasses import dataclass
 from typing import List, Optional, Union
 
 from ..instruction import LiquidHandle
 from ..unit import Unit
 from ..util import parse_unit
 from .liquid_handle_method import LiquidHandleMethod
 
 
 # pylint: disable=protected-access
-@dataclass
 class Dispense(LiquidHandleMethod):
     """LiquidHandleMethod for generating dispense transports
 
     LiquidHandleMethod for moving volume from a source well to destination wells
 
     Attributes
     ----------
@@ -36,22 +34,23 @@
         - _dispense_transports : generates transports for a destination location
 
     See Also
     --------
     LiquidHandleMethod : base LiquidHandleMethod with reused functionality
     """
 
-    volume_resolution: Optional[Unit] = None
-    prime: bool = True
-    predispense: bool = True
+    def __init__(self, volume_resolution=None, prime=True, predispense=True):
+        super(Dispense, self).__init__()
+
+        # parameters for required behavior
+        self.volume_resolution = volume_resolution
 
-    def __post_init__(self):
         # parameters for optional behavior
-        self._set_prime(self.prime)
-        self._set_predispense(self.predispense)
+        self._set_prime(prime)
+        self._set_predispense(predispense)
 
         # LiquidHandle parameters that are generated and modified at runtime
         self._liquid = None
 
     def _set_predispense(self, predispense: Union[Unit, str, bool]) -> None:
         if isinstance(predispense, Unit):
             self.predispense = predispense
```

### Comparing `autoprotocol-9.1.0/autoprotocol/liquid_handle/liquid_class.py` & `autoprotocol-9.1.1/autoprotocol/liquid_handle/liquid_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,21 @@
 
     :copyright: 2021 by The Autoprotocol Development Team, see AUTHORS
         for more details.
     :license: BSD, see LICENSE for more details
 
 """
 from collections import namedtuple
-from dataclasses import dataclass
 from numbers import Number
-from typing import Optional
 
 from ..util import parse_unit
 
 
 # pylint: disable=too-many-instance-attributes,too-few-public-methods
-@dataclass
-class LiquidClass:
+class LiquidClass(object):
     """Contains properties intrinsic to individual LiquidClasses
 
     Attributes
     ----------
     name : str
         the name of the liquid_class may be used by vendors to generate more
         sensible defaults for unspecified behavior
@@ -107,45 +104,53 @@
     --------
     VolumeCalibration : used to specify calibration_curves
     LiquidHandleMethod : used to specify liquid handling movement behavior
     Protocol.transfer : accepts LiquidClass arguments to determine behavior
     Protocol.mix : accepts a LiquidClass argument to determine behavior
     """
 
-    calibrated_volume: Optional["Unit"] = None
-    aspirate_flowrate: Optional[dict] = None
-    dispense_flowrate: Optional[dict] = None
-    delay_time: Optional["Unit"] = None
-    clld_threshold: Optional["Unit"] = None
-    plld_threshold: Optional["Unit"] = None
+    def __init__(
+        self,
+        calibrated_volume=None,
+        aspirate_flowrate=None,
+        dispense_flowrate=None,
+        delay_time=None,
+        clld_threshold=None,
+        plld_threshold=None,
+    ):
+        """
+        Parameters
+        ----------
+        calibrated_volume : Unit, optional
+            used to specify a calibrated volume, if not specified then will
+            default to the calibration from `volume_calibration_curve`
+        aspirate_flowrate : dict, optional
+            used to specify an aspirate flowrate, if not specified then will
+            default to the calibration using
+            `aspirate_flowrate_calibration_curve`
+        dispense_flowrate : dict, optional
+            used to specify a dispense flowrate, if not specified then will
+            default to the calibration using
+            `dispense_flowrate_calibration_curve`
+        delay_time : Unit, optional
+            the amount of time to wait after each liquid handling step.
+            this is helpful for cases such as pressure equilibration
+        clld_threshold : Unit, optional
+            the capacitive liquid level detection threshold
+        plld_threshold : Unit, optional
+            the pressure liquid level detection threshold
+        """
+
+        self.calibrated_volume = calibrated_volume
+        self.aspirate_flowrate = aspirate_flowrate
+        self.dispense_flowrate = dispense_flowrate
+        self.delay_time = delay_time
+        self.clld_threshold = clld_threshold
+        self.plld_threshold = plld_threshold
 
-    """
-    Parameters
-    ----------
-    calibrated_volume : Unit, optional
-        used to specify a calibrated volume, if not specified then will
-        default to the calibration from `volume_calibration_curve`
-    aspirate_flowrate : dict, optional
-        used to specify an aspirate flowrate, if not specified then will
-        default to the calibration using
-        `aspirate_flowrate_calibration_curve`
-    dispense_flowrate : dict, optional
-        used to specify a dispense flowrate, if not specified then will
-        default to the calibration using
-        `dispense_flowrate_calibration_curve`
-    delay_time : Unit, optional
-        the amount of time to wait after each liquid handling step.
-        this is helpful for cases such as pressure equilibration
-    clld_threshold : Unit, optional
-        the capacitive liquid level detection threshold
-    plld_threshold : Unit, optional
-        the pressure liquid level detection threshold
-    """
-
-    def __post_init__(self):
         # Dicts of {tip_type: VolumeCalibration}
         self.volume_calibration_curve = None
         self.aspirate_flowrate_calibration_curve = None
         self.dispense_flowrate_calibration_curve = None
 
         # May be used by vendors to set defaults for different liquid classes
         self.name = None
```

### Comparing `autoprotocol-9.1.0/autoprotocol/liquid_handle/liquid_handle_method.py` & `autoprotocol-9.1.1/autoprotocol/liquid_handle/liquid_handle_method.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,26 +16,22 @@
 Methods in this file should not be used directly, but are intended to be
 extended by other methods depending on desired behavior.
 
 When creating a vendor-specific library it's likely desirable to monkey patch
 `LiquidHandleMethod._get_tip_types` to reference TipTypes that the vendor
 supports.
 """
-from dataclasses import dataclass
-from typing import Optional
-
 from ..instruction import LiquidHandle
 from ..unit import Unit
 from ..util import parse_unit
 from .tip_type import TipType
 
 
 # pylint: disable=too-many-public-methods,protected-access
-@dataclass
-class LiquidHandleMethod:
+class LiquidHandleMethod(object):
     """Base LiquidHandleMethod
 
     General framework for liquid handling abstractions and helpers for
     building a series of liquid_handle transports.
 
     Attributes
     ----------
@@ -102,30 +98,30 @@
     --------
     Transfer : method for handling liquid between two locations
     Mix : method for handling liquid within locations
     LiquidClass : contain properties that are intrinsic to specific liquids
     Protocol : contains methods that accept LiquidHandleMethods as arguments
     """
 
-    tip_type: Optional[TipType] = None
-    blowout: bool = True
-    """
-    Parameters
-    ----------
-    tip_type : str, optional
-        tip_type to be used for the LiquidHandlingMethod
-    blowout : bool or dict, optional
-        whether to execute a blowout step or the parameters for one.
-        this generates two operations, an initial air aspiration before
-        entering any wells, and a corresponding final air dispense
-        after the last operation that involves liquid
-        See Also LiquidHandle.builders.blowout
-    """
+    def __init__(self, tip_type=None, blowout=True):
+        """
+        Parameters
+        ----------
+        tip_type : str, optional
+            tip_type to be used for the LiquidHandlingMethod
+        blowout : bool or dict, optional
+            whether to execute a blowout step or the parameters for one.
+            this generates two operations, an initial air aspiration before
+            entering any wells, and a corresponding final air dispense
+            after the last operation that involves liquid
+            See Also LiquidHandle.builders.blowout
+        """
+        self.tip_type = tip_type
+        self.blowout = blowout
 
-    def __post_init__(self):
         # LiquidHandle parameters that are generated and modified at runtime
         self._shape = None
         self._transports = []
 
     def _get_tip_types(self):
         """Gets a list of TipTypes based on _shape
 
@@ -175,15 +171,15 @@
 
         See Also
         --------
         _get_tip_types : vendor library-specific tip selection method
         """
         return sorted(self._get_tip_types(), key=lambda t: t.volume)
 
-    def _rec_tip_type(self, volume: Unit):
+    def _rec_tip_type(self, volume):
         """For a given volume gets the smallest appropriate tip type
 
         Parameters
         ----------
         volume : Unit
 
         Returns
@@ -248,17 +244,15 @@
         See Also
         --------
         LiquidClass._has_calibration : checks for calibration parameters
         """
         raise NotImplementedError
 
     @staticmethod
-    def _estimate_calibrated_volume(
-        volume: "Unit", liquid: "LiquidClass", tip_type: Optional[str]
-    ):
+    def _estimate_calibrated_volume(volume, liquid, tip_type):
         """Gives an estimation of calibrated volume
 
         If tip_type is specified then gets the actual calibrated volume,
         but if it is None then gets a rough estimate of the maximum volume
         calibration that might be experienced.
 
         This is used for estimates of calibrated volume used for calculating
@@ -289,15 +283,15 @@
             calculated = liquid._get_calibrated_volume(volume, tip_type)
             cal_vol = calculated if calculated is not None else estimated
         else:
             cal_vol = estimated
 
         return cal_vol
 
-    def _calculate_overage_volume(self, volume: "Unit"):
+    def _calculate_overage_volume(self, volume):
         """Calculates extra volume held in the tip besides the target volume
 
         Calculates how much extra volume is contained within the tip besides
         the target volume. This includes things like overage due to
         calibrated volumes being larger than the nominal volume.
 
         Parameters
@@ -319,23 +313,23 @@
         bool
             whether or not the method's shape is single channel-compatible
         """
         return self._shape["rows"] == 1 and self._shape["columns"] == 1
 
     def _aspirate_simple(
         self,
-        volume: "Unit",
-        initial_z: dict,
-        position_x: Optional[dict] = None,
-        position_y: Optional[dict] = None,
-        calibrated_vol: Optional["Unit"] = None,
-        flowrate: Optional[dict] = None,
-        delay_time: Optional["Unit"] = None,
-        liquid_class: Optional[str] = None,
-        density: Optional["Unit"] = None,
+        volume,
+        initial_z,
+        position_x=None,
+        position_y=None,
+        calibrated_vol=None,
+        flowrate=None,
+        delay_time=None,
+        liquid_class=None,
+        density=None,
     ):
         """Helper function for generating aspirate transports
 
         Parameters
         ----------
         volume : Unit
             volume of liquid to be aspirated
@@ -376,25 +370,25 @@
                 mode_params=mode_params,
                 delay_time=delay_time,
             )
         ]
 
     def _aspirate_with_prime(
         self,
-        volume: "Unit",
-        prime_vol: "Unit",
-        initial_z: dict,
-        position_x: Optional[dict] = None,
-        position_y: Optional[dict] = None,
-        calibrated_vol: Optional["Unit"] = None,
-        asp_flowrate: Optional[dict] = None,
-        dsp_flowrate: Optional[dict] = None,
-        delay_time: Optional["Unit"] = None,
-        liquid_class: Optional[str] = None,
-        density: Optional["Unit"] = None,
+        volume,
+        prime_vol,
+        initial_z,
+        position_x=None,
+        position_y=None,
+        calibrated_vol=None,
+        asp_flowrate=None,
+        dsp_flowrate=None,
+        delay_time=None,
+        liquid_class=None,
+        density=None,
     ):
         """Helper function for generating aspiration with priming
 
         Parameters
         ----------
         volume : Unit
             volume of liquid to be aspirated
@@ -454,23 +448,23 @@
                 mode_params=mode_params,
                 delay_time=delay_time,
             ),
         ]
 
     def _dispense_simple(
         self,
-        volume: "Unit",
-        initial_z: dict,
-        position_x: Optional[dict] = None,
-        position_y: Optional[dict] = None,
-        calibrated_vol: Optional["Unit"] = None,
-        flowrate: Optional[dict] = None,
-        delay_time: Optional["Unit"] = None,
-        liquid_class: Optional[str] = None,
-        density: Optional["Unit"] = None,
+        volume,
+        initial_z,
+        position_x=None,
+        position_y=None,
+        calibrated_vol=None,
+        flowrate=None,
+        delay_time=None,
+        liquid_class=None,
+        density=None,
     ):
         """Helper function for generating dispense transports
 
         Parameters
         ----------
         volume : Unit
             volume of liquid to be dispensed
@@ -510,23 +504,23 @@
                 mode_params=mode_params,
                 delay_time=delay_time,
             )
         ]
 
     def _mix(
         self,
-        volume: "Unit",
-        repetitions: int,
-        initial_z: Optional[dict] = None,
-        position_x: Optional[dict] = None,
-        position_y: Optional[dict] = None,
-        asp_flowrate: Optional[dict] = None,
-        dsp_flowrate: Optional[dict] = None,
-        delay_time: Optional["Unit"] = None,
-        liquid_class: Optional[str] = None,
+        volume,
+        repetitions,
+        position_x=None,
+        position_y=None,
+        initial_z=None,
+        asp_flowrate=None,
+        dsp_flowrate=None,
+        delay_time=None,
+        liquid_class=None,
     ):
         """Helper function for generating mix transports
 
         Parameters
         ----------
         volume : Unit
             volume of liquid to be aspirated and expelled during mixing
@@ -570,18 +564,15 @@
                 flowrate=dsp_flowrate,
                 mode_params=mode_params,
                 delay_time=delay_time,
             ),
         ] * repetitions
 
     def _move_to_initial_position(
-        self,
-        position_x: Optional[dict] = None,
-        position_y: Optional[dict] = None,
-        position_z: Optional[dict] = None,
+        self, position_x=None, position_y=None, position_z=None
     ):
         """Moves to a given position_z and then returns a followup one
 
         Takes an initial position_z and moves to it before returning a
         suitable followup.
 
         If sensing is specified, then moves to well top and senses before
@@ -619,15 +610,15 @@
                 )
             ]
 
         followup_z = self._get_followup_z(position_z)
 
         return followup_z
 
-    def _move_to_well_top_before_lld(self, position_z: dict):
+    def _move_to_well_top_before_lld(self, position_z):
         """If position_z contains any liquid sensing moves to well top
 
         Parameters
         ----------
         position_z : dict
             position_z to be checked for lld events
         """
@@ -639,15 +630,15 @@
 
         if position_z:
             if position_z.get("reference") == "liquid_surface":
                 if position_z.get("detection", {}).get("method") != "tracked":
                     self._transports.append(well_top_z)
 
     @staticmethod
-    def _get_followup_z(position_z: dict):
+    def _get_followup_z(position_z):
         """Generates a position_z that references preceding position/tracked
 
         Generates a position_z to followup after the specified one. If the
         liquid surface is referenced, then returns a position that similarly
         tracks the surface. Otherwise, generates a reference to the preceding
         position.
 
@@ -671,15 +662,15 @@
                 detection_method="tracked",
             )
         else:
             followup_z = preceding_z
 
         return followup_z
 
-    def _transport_pre_buffer(self, volume: "Unit"):
+    def _transport_pre_buffer(self, volume):
         """Aspirates a pre buffer of air volume above the source location
 
         Parameters
         ----------
         volume : Unit
 
         See Also
@@ -694,15 +685,15 @@
                 volume=pre_buffer,
                 initial_z=LiquidHandle.builders.position_z(
                     reference="well_top", offset="1:mm"
                 ),
                 liquid_class="air",
             )
 
-    def _calculate_pre_buffer(self, volume: "Unit"):
+    def _calculate_pre_buffer(self, volume):
         """Calculates a recommended pre_buffer volume
 
         Parameters
         ----------
         volume : Unit
 
         Returns
@@ -719,15 +710,15 @@
         elif self.blowout is False:
             blowout = {}
         else:
             blowout = self.blowout
 
         return blowout.get("volume", Unit("0:uL"))
 
-    def _transport_blowout(self, volume: "Unit"):
+    def _transport_blowout(self, volume):
         """Blows out air volume above the destination location
 
         Parameters
         ----------
         volume : Unit
             liquid handling volume
 
@@ -745,15 +736,15 @@
             blowout = self.blowout
 
         if blowout is not False:
             blowout_params = LiquidHandle.builders.blowout(**blowout)
             self._dispense_simple(liquid_class="air", **blowout_params)
 
     # pylint: disable=missing-param-doc
-    def default_blowout(self, volume: "Unit"):
+    def default_blowout(self, volume: Unit):
         """Default blowout behavior
 
         Parameters
         ----------
         volume : Unit
 
         Returns
@@ -765,15 +756,15 @@
         --------
         blowout : holds any user specified blowout parameters
         _transport_blowout : generates the actual blowout transports
         """
         raise NotImplementedError
 
     @staticmethod
-    def default_lld_position_z(liquid: "LiquidClass"):
+    def default_lld_position_z(liquid):
         """Default lld position_z
 
         Returns
         -------
         dict
             position_z for sensing the liquid surface
         """
```

### Comparing `autoprotocol-9.1.0/autoprotocol/liquid_handle/mix.py` & `autoprotocol-9.1.1/autoprotocol/liquid_handle/mix.py`

 * *Files identical despite different names*

### Comparing `autoprotocol-9.1.0/autoprotocol/liquid_handle/tip_type.py` & `autoprotocol-9.1.1/autoprotocol/liquid_handle/tip_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 """
 Generic tip type and device class mappings for LiquidHandleMethods
 
     :copyright: 2021 by The Autoprotocol Development Team, see AUTHORS
         for more details.
     :license: BSD, see LICENSE for more details
 """
-import dataclasses
-
 from collections import namedtuple
 
 from ..util import parse_unit
 
 
-@dataclasses.dataclass(init=False)
 class TipType(namedtuple("TipType", ["name", "volume"])):
     """
     The TipType class holds the properties of a TipType
     """
 
-    name: str
-    volume: str
-
-    def __new__(cls, name: str, volume: str):
+    def __new__(cls, name, volume):
         """
         Parameters
         ----------
         name : str
           Full name describing a TipType.
         volume : Unit
           The maximum capacity of the TipType.
```

### Comparing `autoprotocol-9.1.0/autoprotocol/liquid_handle/transfer.py` & `autoprotocol-9.1.1/autoprotocol/liquid_handle/transfer.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,113 +3,115 @@
     :copyright: 2021 by The Autoprotocol Development Team, see AUTHORS
         for more details.
     :license: BSD, see LICENSE for more details
 
 Base LiquidHandleMethod used by Protocol.transfer to generate a series of
 movements between pairs of wells.
 """
-import dataclasses
-
-from typing import Optional, Union
-
 from ..instruction import LiquidHandle
 from ..unit import Unit
 from ..util import parse_unit
 from .liquid_handle_method import LiquidHandleMethod
 
 
 # pylint: disable=unused-argument,too-many-instance-attributes,protected-access
-@dataclasses.dataclass
 class Transfer(LiquidHandleMethod):
     """LiquidHandleMethod for generating transfers between pairs of wells
 
     LiquidHandleMethod for transferring volume from one well to another.
 
-
-    Parameters
-    ----------
-    tip_type : str, optional
-        tip_type to be used for the LiquidHandlingMethod
-    blowout : bool or dict, optional
-        whether to execute a blowout step or the parameters for one.
-        this generates a pair of operations: an initial air aspiration
-        before entering any wells and a corresponding air dispense after the
-        last operation that involves liquid
-        See Also LiquidHandle.builders.blowout
-    prime : bool or Unit, optional
-        whether to execute a prime step or the parameters for one.
-        this generates a pair of aspirate/dispense operations around the
-        aspiration step in the sequence:
-        aspirate_prime -> aspirate_target_volume -> dispense_prime
-    transit : bool or Unit, optional
-        whether to execute a transit step or the parameters for one.
-        this generates a pair of operations wherein air is aspirated just
-        before leaving the source location and dispensed immediately
-        after reaching the destination location
-    mix_before : bool or dict, optional
-        whether to execute a mix_before step or the parameters for one.
-        this generates a series of aspirate and dispense steps within the
-        source location before aspirating the target volume
-        See Also LiquidHandle.builders.mix
-    mix_after : bool or dict, optional
-        whether to execute a mix_after step or the parameters for one.
-        this generates a series of aspirate and dispense steps within the
-        destination location after dispensing the target volume
-        See Also LiquidHandle.builders.mix
-    aspirate_z : dict, optional
-        the position that the tip should move to prior to aspirating, if the
-        position references the `liquid_surface` then aspirate movements
-        will track the surface with the defined offset.
-        See Also LiquidHandle.builders.position_z
-    dispense_z : dict, optional
-        the position that the tip should move to prior to dispensing, if the
-        position references the `liquid_surface` then dispense
-        will track the surface with the defined offset.
-        See Also LiquidHandle.builders.position_z
-
-
     Attributes
     ----------
     _source_liquid : LiquidClass
         used to determine calibration, flowrates, and sensing thresholds
     _destination_liquid : LiquidClass
         used to determine calibration, flowrates, and sensing thresholds
 
-
     Notes
     -----
     The primary entry points that for this class are:
         - _aspirate_transports : generates transports for a source location
         - _dispense_transports : generates transports for a destination location
 
 
     See Also
     --------
     LiquidHandleMethod : base LiquidHandleMethod with reused functionality
     Protocol.transfer : the standard interface for interacting with Transfer
     """
 
-    tip_type: Optional[str] = None
-    blowout: Optional[Union[bool, dict]] = True
-    prime: Optional[Union[bool, Unit]] = True
-    transit: Optional[Union[bool, Unit]] = True
-    mix_before: Optional[Union[bool, dict]] = False
-    mix_after: Optional[Union[bool, dict]] = True
-    aspirate_z: Optional[dict] = None
-    dispense_z: Optional[dict] = None
+    def __init__(
+        self,
+        tip_type=None,
+        blowout=True,
+        prime=True,
+        transit=True,
+        mix_before=False,
+        mix_after=True,
+        aspirate_z=None,
+        dispense_z=None,
+    ):
+        """
+        Parameters
+        ----------
+        tip_type : str, optional
+            tip_type to be used for the LiquidHandlingMethod
+        blowout : bool or dict, optional
+            whether to execute a blowout step or the parameters for one.
+            this generates a pair of operations: an initial air aspiration
+            before entering any wells and a corresponding air dispense after the
+            last operation that involves liquid
+            See Also LiquidHandle.builders.blowout
+        prime : bool or Unit, optional
+            whether to execute a prime step or the parameters for one.
+            this generates a pair of aspirate/dispense operations around the
+            aspiration step in the sequence:
+            aspirate_prime -> aspirate_target_volume -> dispense_prime
+        transit : bool or Unit, optional
+            whether to execute a transit step or the parameters for one.
+            this generates a pair of operations wherein air is aspirated just
+            before leaving the source location and dispensed immediately
+            after reaching the destination location
+        mix_before : bool or dict, optional
+            whether to execute a mix_before step or the parameters for one.
+            this generates a series of aspirate and dispense steps within the
+            source location before aspirating the target volume
+            See Also LiquidHandle.builders.mix
+        mix_after : bool or dict, optional
+            whether to execute a mix_after step or the parameters for one.
+            this generates a series of aspirate and dispense steps within the
+            destination location after dispensing the target volume
+            See Also LiquidHandle.builders.mix
+        aspirate_z : dict, optional
+            the position that the tip should move to prior to aspirating, if the
+            position references the `liquid_surface` then aspirate movements
+            will track the surface with the defined offset.
+            See Also LiquidHandle.builders.position_z
+        dispense_z : dict, optional
+            the position that the tip should move to prior to dispensing, if the
+            position references the `liquid_surface` then dispense
+            will track the surface with the defined offset.
+            See Also LiquidHandle.builders.position_z
+        """
+        super(Transfer, self).__init__(tip_type=tip_type, blowout=blowout)
+
+        # parameters for required behavior
+        self.aspirate_z = aspirate_z
+        self.dispense_z = dispense_z
+
+        # parameters for optional behavior
+        self.prime = prime
+        self.transit = transit
+        self.mix_before = mix_before
+        self.mix_after = mix_after
 
-    def __post_init__(self):
         # LiquidHandle parameters that are generated and modified at runtime
         self._source_liquid = None
         self._destination_liquid = None
 
-    def _rec_tip_type(self, volume: Unit):
-        self.tip_type = super(Transfer, self)._rec_tip_type(volume=volume)
-        return self.tip_type
-
     def _has_calibration(self):
         liquids = [self._source_liquid, self._destination_liquid]
         return any(_ and _._has_calibration() for _ in liquids)
 
     def _calculate_overage_volume(self, volume):
         calibration_overage = (
             self._estimate_calibrated_volume(volume, self._source_liquid, self.tip_type)
```

### Comparing `autoprotocol-9.1.0/autoprotocol/protocol.py` & `autoprotocol-9.1.1/autoprotocol/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,38 +2,50 @@
 Module containing the main `Protocol` object and associated functions
 
     :copyright: 2021 by The Autoprotocol Development Team, see AUTHORS
         for more details.
     :license: BSD, see LICENSE for more details
 
 """
+
 import json
 import warnings
 
-from typing import Dict, List, Tuple
+from typing import Dict, List, Tuple, Union
 
 from .compound import Compound
 from .constants import AGAR_CLLD_THRESHOLD, SPREAD_PATH
 from .container import COVER_TYPES, SEAL_TYPES, Container, Well
 from .container_type import _CONTAINER_TYPES, ContainerType
+from .informatics import Informatics
 from .instruction import *  # pylint: disable=unused-wildcard-import
 from .liquid_handle import Dispense as DispenseMethod
 from .liquid_handle import LiquidClass, Mix, Transfer
-from .types.protocol import *  # pylint: disable=unused-wildcard-import
-from .types.ref import Ref, RefOpts, StorageLocation
+from .types.protocol import AutopickGroup
 from .unit import Unit, UnitError
 from .util import _check_container_type_with_shape, _validate_as_instance
 
 
-@dataclass
-class Protocol:
-    refs: Optional[Dict[str, Ref]] = None
-    instructions: List[Instruction] = field(default_factory=list)
-    propagate_properties: bool = False
-    time_constraints: List[TimeConstraint] = field(default_factory=list)
+class Ref(object):
+    """
+    Link a ref name (string) to a Container instance.
+
+    """
+
+    def __init__(self, name, opts, container):
+        self.name = name
+        self.opts = opts
+        self.container = container
+
+    def __repr__(self):
+        return f"Ref({self.name}, {self.container}, {self.opts})"
+
+
+# noinspection PyCompatibility
+class Protocol(object):
     """
     A Protocol is a sequence of instructions to be executed, and a set of
     containers on which those instructions act.
 
     Parameters
     ----------
     refs : list(Ref)
@@ -118,17 +130,26 @@
                   ],
                   "op": "thermocycle"
                 }
               ]
             }
     """
 
-    def __post_init__(self):
-        if not self.refs:
-            self.refs: Dict[str, Ref] = {}
+    def __init__(
+        self,
+        refs: Optional[List[Ref]] = None,
+        instructions: List[Instruction] = None,
+        propagate_properties: bool = False,
+        time_constraints: List[dict] = None,
+    ):
+        super(Protocol, self).__init__()
+        self.refs = refs or {}
+        self.instructions = instructions or []
+        self.propagate_properties = propagate_properties
+        self.time_constraints = time_constraints or []
 
     def __repr__(self):
         return f"Protocol({self.__dict__})"
 
     def container_type(self, shortname: str):
         """
         Convert a ContainerType shortname into a ContainerType object.
@@ -167,16 +188,16 @@
         self,
         name: str,
         id: Optional[str] = None,
         cont_type: Optional[Union[str, ContainerType]] = None,
         storage: Optional[str] = None,
         discard: Optional[bool] = None,
         cover: Optional[str] = None,
-        properties: Optional[Dict[str, str]] = None,
-        ctx_properties: Optional[Dict[str, str]] = None,
+        properties: Optional[dict] = None,
+        ctx_properties: Optional[dict] = None,
     ):
         """
         Add a Ref object to the dictionary of Refs associated with this protocol
         and return a Container with the id, container type and storage or
         discard conditions specified.
 
         Example Usage:
@@ -257,63 +278,63 @@
 
         """
 
         if name in self.refs.keys():
             raise RuntimeError(
                 "Two containers within the same protocol cannot have the same " "name."
             )
-        opts: RefOpts = RefOpts()
+        opts = {}
 
         # Check container type
         try:
             cont_type = self.container_type(cont_type)
             if id and cont_type:
-                opts.id = id
+                opts["id"] = id
             elif cont_type:
-                opts.new = cont_type.shortname
+                opts["new"] = cont_type.shortname
         except ValueError as e:
             raise RuntimeError(
                 f"{cont_type} is not a recognized container type."
             ) from e
 
         if storage:
-            opts.store = StorageLocation(**{"where": storage})
+            opts["store"] = {"where": storage}
         elif discard and not storage:
-            opts.discard = discard
+            opts["discard"] = discard
         else:
             raise RuntimeError(
                 "You must specify either a valid storage condition or set "
                 "discard=True for a Ref."
             )
 
         if cover:
-            opts.cover = cover
+            opts["cover"] = cover
 
         container = Container(
-            id=id,
-            container_type=cont_type,
+            id,
+            cont_type,
             name=name,
             storage=storage if storage else None,
             cover=cover if cover else None,
             properties=properties,
             ctx_properties=ctx_properties,
         )
         self.refs[name] = Ref(name, opts, container)
         return container
 
     # pragma pylint: enable=redefined-builtin
 
     def add_time_constraint(
         self,
-        from_dict: TimeConstraintFromToDict,
-        to_dict: TimeConstraintFromToDict,
-        less_than: Optional[TIME] = None,
-        more_than: Optional[TIME] = None,
+        from_dict: dict,
+        to_dict: dict,
+        less_than: Optional[Union[str, Unit]] = None,
+        more_than: Optional[Union[str, Unit]] = None,
         mirror: bool = False,
-        ideal: Optional[TIME] = None,
+        ideal: Optional[Union[str, Unit]] = None,
         optimization_cost: Optional[str] = None,
     ):
         """Constraint the time between two instructions
 
         Add time constraints from `from_dict` to `to_dict`. Time constraints
         guarantee that the time from the `from_dict` to the `to_dict` is less
         than or greater than some specified duration. Care should be taken when
@@ -703,16 +724,16 @@
             self.instructions.append(instructions)
 
         return instructions
 
     def batch_containers(
         self,
         containers: List[Container],
-        batch_in: bool = True,
-        batch_out: bool = False,
+        batch_in: Optional[bool] = True,
+        batch_out: Optional[bool] = False,
     ):
         """
         Batch containers such that they all enter or exit together.
 
         Example Usage:
 
         .. code-block:: python
@@ -868,22 +889,22 @@
         RuntimeError
             If either refs or instructions attribute is empty
         """
         outs = defaultdict(lambda: defaultdict(dict))
         # pragma pylint: disable=protected-access
         for n, ref in self.refs.items():
             # assign any storage or discard condition changes to ref
-            if ref.opts.store:
-                ref.opts.store.where = ref.container.storage
-            if not ref.container.storage and not ref.opts.discard:
-                ref.opts.discard = True
-                ref.opts.store = None
-            elif ref.container.storage and ref.opts.discard:
-                ref.opts.store = StorageLocation(**{"where": ref.container.storage})
-                ref.opts.discard = None
+            if "store" in ref.opts:
+                ref.opts["store"]["where"] = ref.container.storage
+            if ref.container.storage is None and "discard" not in ref.opts:
+                ref.opts["discard"] = True
+                del ref.opts["store"]
+            elif ref.container.storage is not None and "discard" in ref.opts:
+                ref.opts["store"] = {"where": ref.container.storage}
+                del ref.opts["discard"]
 
             if ref.container.properties:
                 outs[n]["properties"] = ref.container.properties
 
             if ref.container.ctx_properties:
                 outs[n]["contextual_custom_properties"] = ref.container.ctx_properties
 
@@ -924,16 +945,16 @@
         }
 
     # pylint: disable=protected-access
     # pylint: disable=no-member
     def liquid_handle_dispense(
         self,
         source: Union[Well, List[Well], List[Tuple[Well, int]]],
-        destination: Union[WellParam, List[WellGroup]],
-        volume: Union[VOLUME, List[VOLUME]],
+        destination: Union[Well, WellGroup, List[Well], List[WellGroup]],
+        volume: Union[str, Unit, List[str], List[Unit]],
         rows: int = 8,
         columns: int = 1,
         method: DispenseMethod = DispenseMethod,
         liquid: LiquidClass = LiquidClass,
         model: Optional[str] = None,
         chip_material: Optional[str] = None,
         nozzle: Optional[str] = None,
@@ -1420,19 +1441,19 @@
             r.opts["store"] = {"where": str(condition)}
         else:
             r.opts.pop("store")
             r.opts["discard"] = True
 
     def acoustic_transfer(
         self,
-        source: WellParam,
-        dest: WellParam,
-        volume: VOLUME,
+        source: Union[Well, WellGroup, List[Well]],
+        dest: Union[Well, WellGroup, List[Well]],
+        volume: Union[str, Unit],
         one_source: bool = False,
-        droplet_size: VOLUME = "25:nanoliter",
+        droplet_size: Union[str, Unit] = "25:nanoliter",
     ):
         """
         Specify source and destination wells for transferring liquid via an
         acoustic liquid handler.  Droplet size is usually device-specific.
 
         Example Usage:
 
@@ -1519,16 +1540,15 @@
             Returns the :py:class:`autoprotocol.instruction.AcousticTransfer`
             instruction created from the specified parameters
 
         Raises
         ------
         TypeError
             Incorrect input types, e.g. source/dest are not Well or WellGroup
-            or list of Well; or container_type does not have 'acoustic_transfer'
-            capability.
+            or list of Well
         RuntimeError
             Incorrect length for source and destination
         RuntimeError
             Transfer volume not being a multiple of droplet size
         RuntimeError
             Insufficient volume in source wells
 
@@ -1538,31 +1558,14 @@
             raise TypeError("Source must be of type Well, list of Wells, or WellGroup.")
         if not is_valid_well(dest):
             raise TypeError(
                 "Destination (dest) must be of type Well, list of Wells, or "
                 "WellGroup."
             )
 
-        # Check valid container_type capability
-        wells = []
-        if isinstance(source, Well):
-            wells.append(source)
-        elif isinstance(source, WellGroup):
-            wells = source.wells
-        elif isinstance(source, list):
-            wells = source
-        for well in wells:
-            if "acoustic_transfer" not in well.container.container_type.capabilities:
-                raise TypeError(
-                    f"AcousticTransfer: Source does not have 'acoustic_transfer' "
-                    f"capability for well '{well.index}' of container name "
-                    f"'{well.container.name}' with container ID '{well.container.id}' "
-                    f"and container type '{well.container.container_type.shortname}'!"
-                )
-
         transfers = []
         source = WellGroup(source)
         dest = WellGroup(dest)
         len_source = len(source.wells)
         len_dest = len(dest.wells)
         droplet_size = Unit(droplet_size)
         max_decimal_places = 12  # for rounding after floating point arithmetic
@@ -1690,15 +1693,15 @@
         return self._append_and_return(
             AcousticTransfer([{"transfer": transfers}], droplet_size)
         )
 
     def illuminaseq(
         self,
         flowcell: str,
-        lanes: List[IlluminaSeqLane],
+        lanes: List[dict],
         sequencer: str,
         mode: str,
         index: str,
         library_size: int,
         dataref: str,
         cycles: Optional[str] = None,
     ):
@@ -1938,15 +1941,15 @@
             )
         )
 
     # pylint: disable=redefined-builtin
     def sangerseq(
         self,
         cont: Union[Container, str],
-        wells: WellParam,
+        wells: Union[List[Well], WellGroup, Well],
         dataref: str,
         type: str = "standard",
         primer: Optional[Container] = None,
     ):
         """
         Send the indicated wells of the container specified for Sanger
         sequencing.
@@ -2044,22 +2047,22 @@
 
         return self._append_and_return(SangerSeq(cont, wells, dataref, type, primer))
 
     def dispense(
         self,
         ref: Container,
         reagent: Union[str, Well],
-        columns: List[DispenseColumn],
+        columns: List[Dict[str, Union[str, Unit]]],
         is_resource_id: bool = False,
-        step_size: VOLUME = "5:uL",
-        flowrate: Optional[FLOW_RATE] = None,
-        nozzle_position: Optional[DispenseNozzlePosition] = None,
-        pre_dispense: Optional[VOLUME] = None,
-        shape: Optional[DispenseShape] = None,
-        shake_after: Optional[DispenseShakeAfter] = None,
+        step_size: Union[str, Unit] = "5:uL",
+        flowrate: Optional[Union[str, Unit]] = None,
+        nozzle_position: Optional[Union[str, Unit]] = None,
+        pre_dispense: Optional[Union[str, Unit]] = None,
+        shape: Optional[dict] = None,
+        shake_after: Optional[dict] = None,
     ):
         """
         Dispense specified reagent to specified columns.
 
         Example Usage:
 
         .. code-block:: python
@@ -2323,22 +2326,22 @@
             )
         )
 
     def dispense_full_plate(
         self,
         ref: Container,
         reagent: Union[str, Well],
-        volume: VOLUME,
+        volume: Union[Unit, str],
         is_resource_id: bool = False,
-        step_size: VOLUME = "5:uL",
-        flowrate: Optional[FLOW_RATE] = None,
-        nozzle_position: Optional[DispenseNozzlePosition] = None,
-        pre_dispense: Optional[VOLUME] = None,
-        shape: Optional[DispenseShape] = None,
-        shake_after: Optional[DispenseShakeAfter] = None,
+        step_size: Union[str, Unit] = "5:uL",
+        flowrate: Optional[Union[str, Unit]] = None,
+        nozzle_position: Optional[Union[str, Unit]] = None,
+        pre_dispense: Optional[Union[str, Unit]] = None,
+        shape: Optional[dict] = None,
+        shake_after: Optional[dict] = None,
     ):
         """
         Dispense the specified amount of the specified reagent to every well
         of a container using a reagent dispenser.
 
         Example Usage:
 
@@ -2484,15 +2487,15 @@
             shake_after,
         )
 
     def spin(
         self,
         ref: Container,
         acceleration: str,
-        duration: TIME,
+        duration: Union[str, Unit],
         flow_direction: Optional[str] = None,
         spin_direction: Optional[List[str]] = None,
     ):
         """
         Apply acceleration to a container.
 
         Example Usage:
@@ -2601,19 +2604,19 @@
         return self._append_and_return(
             Spin(ref, acceleration, duration, flow_direction, spin_direction)
         )
 
     def agitate(
         self,
         ref: Container,
-        mode: AgitateMode,
-        speed: ACCELERATION,
-        duration: TIME,
-        temperature: Optional[TEMPERATURE] = None,
-        mode_params: Optional[AgitateModeParams] = None,
+        mode: str,
+        speed: Union[str, Unit],
+        duration: Union[str, Unit],
+        temperature: Optional[Union[Unit, str]] = None,
+        mode_params: Optional[dict] = None,
     ):
         """
         Agitate a container in a specific condition for a given duration. If
         temperature is not specified, container is agitated at ambient
         temperature by default.
 
         Example Usage:
@@ -2689,16 +2692,16 @@
             If `bar_length` is less than 0 millimeter
         ValueError
             If `mode` used does not require `mode_params`
         TypeError
             If ref cannot be undergo agitate mode `roll` or `invert`
 
         """
-        valid_modes = AgitateMode.__dict__.get("_member_names_")
-        valid_bar_shapes = AgitateModeParamsBarShape.__dict__.get("_member_names_")
+        valid_modes = ["vortex", "invert", "roll", "stir_bar"]
+        valid_bar_shapes = ["bar", "cross"]
         valid_bar_mode_params = ["wells", "bar_shape", "bar_length"]
 
         speed = parse_unit(speed)
         temperature = parse_unit(temperature, "celsius") if temperature else None
         duration = parse_unit(duration, "minute")
 
         if not isinstance(ref, Container):
@@ -2712,27 +2715,23 @@
             raise ValueError(f"Agitate mode must be one of {valid_modes}")
         if mode == "stir_bar":
             if mode_params is None:
                 raise ValueError(
                     "Dictionary `mode_params` must be specified for the "
                     "mode `stir_bar`"
                 )
-            else:
-                if isinstance(mode_params, dict):
-                    try:
-                        mode_params = AgitateModeParams(**mode_params)
-                    except:
-                        raise ValueError(
-                            f"mode_params {mode_params.keys()} to not match {valid_bar_mode_params}"
-                        )
+            elif not set(mode_params.keys()) == set(valid_bar_mode_params):
+                raise ValueError(
+                    f"Params for `stir_bar` must include " f"{valid_bar_mode_params}"
+                )
 
-            wells = WellGroup(mode_params.wells)
+            wells = WellGroup(mode_params["wells"])
             container = set([w.container for w in wells])
-            shape = mode_params.bar_shape
-            length = parse_unit(mode_params.bar_length, "millimeter")
+            shape = mode_params["bar_shape"]
+            length = parse_unit(mode_params["bar_length"], "millimeter")
 
             if len(container) > 1:
                 raise ValueError(
                     "All wells need to be on the same container for Agitate"
                 )
             if shape not in valid_bar_shapes:
                 raise ValueError(f"Param `bar_shape` must be one of {valid_bar_shapes}")
@@ -2748,23 +2747,23 @@
         return self._append_and_return(
             Agitate(ref, mode, speed, duration, temperature, mode_params)
         )
 
     def thermocycle(
         self,
         ref: Container,
-        groups: List[Union[ThermocycleTemperature, ThermocycleTemperatureGradient]],
-        volume: Optional[VOLUME] = "10:microliter",
+        groups: List[dict],
+        volume: Optional[Union[str, Unit]] = "10:microliter",
         dataref: Optional[str] = None,
         dyes: Optional[Dict[str, str]] = None,
-        melting_start: Optional[TEMPERATURE] = None,
-        melting_end: Optional[TEMPERATURE] = None,
-        melting_increment: Optional[TEMPERATURE] = None,
-        melting_rate: Optional[TEMPERATURE] = None,
-        lid_temperature: Optional[TEMPERATURE] = None,
+        melting_start: Optional[Union[str, Unit]] = None,
+        melting_end: Optional[Union[str, Unit]] = None,
+        melting_increment: Optional[Union[str, Unit]] = None,
+        melting_rate: Optional[Union[str, Unit]] = None,
+        lid_temperature: Optional[Union[str, Unit]] = None,
     ):
         """
         Append a Thermocycle instruction to the list of instructions, with
         groups is a list(dict) in the form of:
 
         .. code-block:: python
 
@@ -3098,22 +3097,22 @@
                 melting=melting,
                 lid_temperature=lid_temperature,
             )
         )
 
     def incubate(
         self,
-        ref: Union[Container, str],
+        ref: Union[Ref, str],
         where: str,
-        duration: TIME,
+        duration: Union[Unit, str],
         shaking: bool = False,
         co2: float = 0,
         uncovered: bool = False,
-        target_temperature: Optional[TEMPERATURE] = None,
-        shaking_params: Optional[IncubateShakingParams] = None,
+        target_temperature: Optional[Union[Unit, str]] = None,
+        shaking_params: Optional[dict] = None,
     ):
         """
         Move plate to designated thermoisolater or ambient area for incubation
         for specified duration.
 
         Example Usage:
 
@@ -3207,21 +3206,21 @@
                 ref, where, duration, shaking, co2, target_temperature, shaking_params
             )
         )
 
     def absorbance(
         self,
         ref: Union[str, Container],
-        wells: WellParam,
-        wavelength: WAVELENGTH,
+        wells: Union[List[Well], WellGroup, Well],
+        wavelength: Union[str, Unit],
         dataref: str,
         flashes: int = 25,
-        incubate_before: Optional[PlateReaderIncubateBefore] = None,
-        temperature: Optional[TEMPERATURE] = None,
-        settle_time: Optional[TIME] = None,
+        incubate_before: Optional[dict] = None,
+        temperature: Optional[Union[str, Unit]] = None,
+        settle_time: Optional[Unit] = None,
     ):
         """
         Read the absorbance for the indicated wavelength for the indicated
         wells. Append an Absorbance instruction to the list of instructions for
         this Protocol object.
 
         Example Usage:
@@ -3339,29 +3338,27 @@
                 settle_time,
             )
         )
 
     def fluorescence(
         self,
         ref: Union[str, Container],
-        wells: WellParam,
-        excitation: WAVELENGTH,
-        emission: WAVELENGTH,
+        wells: Union[List[Well], WellGroup, Well],
+        excitation: Union[str, Unit],
+        emission: Union[str, Unit],
         dataref: str,
         flashes: Optional[int] = 25,
-        temperature: Optional[TEMPERATURE] = None,
+        temperature: Optional[Union[str, Unit]] = None,
         gain: Optional[float] = None,
-        incubate_before: Optional[PlateReaderIncubateBefore] = None,
+        incubate_before: Optional[dict] = None,
         detection_mode: Optional[str] = None,
-        position_z: Optional[
-            Union[PlateReaderPositionZCalculated, PlateReaderPositionZManual]
-        ] = None,
-        settle_time: Optional[TIME] = None,
-        lag_time: Optional[TIME] = None,
-        integration_time: Optional[str] = None,
+        position_z: Optional[dict] = None,
+        settle_time: Optional[Unit] = None,
+        lag_time: Optional[Unit] = None,
+        integration_time: Optional[Unit] = None,
     ):
         """
         Read the fluoresence for the indicated wavelength for the indicated
         wells.  Append a Fluorescence instruction to the list of instructions
         for this Protocol object.
 
         Example Usage:
@@ -3641,20 +3638,20 @@
                 integration_time,
             )
         )
 
     def luminescence(
         self,
         ref: Union[str, Container],
-        wells: WellParam,
+        wells: Union[List[Well], WellGroup, Well],
         dataref: str,
-        incubate_before: Union[PlateReaderIncubateBefore] = None,
-        temperature: Optional[TEMPERATURE] = None,
-        settle_time: Optional[TIME] = None,
-        integration_time: Optional[TIME] = None,
+        incubate_before: Union[dict] = None,
+        temperature: Optional[Union[str, Unit]] = None,
+        settle_time: Optional[Unit] = None,
+        integration_time: Optional[Unit] = None,
     ):
         """
         Read luminescence of indicated wells.
 
         Example Usage:
 
         .. code-block:: python
@@ -3775,19 +3772,19 @@
                 settle_time,
                 integration_time,
             )
         )
 
     def gel_separate(
         self,
-        wells: WellParam,
-        volume: VOLUME,
+        wells: Union[List[Well], WellGroup, Well],
+        volume: Union[str, Unit],
         matrix: str,
         ladder: str,
-        duration: TIME,
+        duration: Union[str, Unit],
         dataref: str,
     ):
         """
         Separate nucleic acids on an agarose gel.
 
         Example Usage:
 
@@ -3882,16 +3879,16 @@
 
         return self._append_and_return(
             GelSeparate(wells, volume, matrix, ladder, duration, dataref)
         )
 
     def gel_purify(
         self,
-        extracts: List[GelPurifyExtract],
-        volume: VOLUME,
+        extracts: List[dict],
+        volume: Union[str, Unit],
         matrix: str,
         ladder: str,
         dataref: str,
     ):
         """
         Separate nucleic acids on an agarose gel and purify according to
         parameters. If gel extract lanes are not specified, they will be
@@ -4106,16 +4103,16 @@
         return instructions
 
     def seal(
         self,
         ref: Container,
         type: Optional[str] = None,
         mode: Optional[str] = None,
-        temperature: Optional[TEMPERATURE] = None,
-        duration: Optional[TEMPERATURE] = None,
+        temperature: Optional[Union[Unit, str]] = None,
+        duration: Optional[Union[Unit, str]] = None,
     ):
         """
         Seal indicated container using the automated plate sealer.
 
         Example Usage:
 
         .. code-block:: python
@@ -4445,17 +4442,17 @@
         if ref.is_covered():
             ref.cover = None
             return self._append_and_return(Uncover(ref, store_lid))
 
     def flow_cytometry(
         self,
         dataref: str,
-        samples: WellParam,
-        lasers: List[FlowCytometryLaser],
-        collection_conditions: FlowCytometryCollectionCondition,
+        samples: Union[List[Well], Well, WellGroup],
+        lasers: List[dict],
+        collection_conditions: dict,
         width_threshold: Optional[Union[int, float]] = None,
         window_extension: Optional[Union[int, float]] = None,
         remove_coincident_events: Optional[bool] = None,
     ):
         """
         A non-ambiguous set of parameters for performing flow cytometry.
 
@@ -4587,32 +4584,18 @@
             if not isinstance(window_extension, Number):
                 raise TypeError("window_extension must be a number.")
 
         if remove_coincident_events is not None:
             if not isinstance(remove_coincident_events, bool):
                 raise TypeError("remove_coincident_events must be of type " "bool.")
 
-        lasers = [
-            FlowCytometry.builders.laser(
-                channels=l.channels,
-                excitation=l.excitation,
-                power=l.power,
-                area_scaling_factor=l.area_scaling_factor,
-            )
-            for l in lasers
-        ]
+        lasers = [FlowCytometry.builders.laser(**_) for _ in lasers]
 
         collection_conditions = FlowCytometry.builders.collection_conditions(
-            acquisition_volume=collection_conditions.acquisition_volume,
-            flowrate=collection_conditions.flowrate,
-            wait_time=collection_conditions.wait_time,
-            mix_cycles=collection_conditions.mix_cycles,
-            mix_volume=collection_conditions.mix_volume,
-            rinse_cycles=collection_conditions.rinse_cycles,
-            stop_criteria=collection_conditions.stop_criteria,
+            **collection_conditions
         )
 
         return self._append_and_return(
             FlowCytometry(
                 dataref,
                 samples,
                 lasers,
@@ -4622,20 +4605,20 @@
                 remove_coincident_events,
             )
         )
 
     def flow_analyze(
         self,
         dataref: str,
-        FSC: FlowAnalyzeChannel,
-        SSC: FlowAnalyzeChannel,
-        neg_controls: List[FlowAnalyzeNegControls],
-        samples: List[FlowAnalyzeSample],
-        colors: Optional[List[FlowAnalyzeColors]] = None,
-        pos_controls: Optional[List[FlowAnalyzePosControls]] = None,
+        FSC: dict,
+        SSC: dict,
+        neg_controls: List[dict],
+        samples: List[dict],
+        colors: Optional[List[dict]] = None,
+        pos_controls: Optional[List[dict]] = None,
     ):
         """
         Perform flow cytometry. The instruction will be executed within the
         voltage range specified for each channel, optimized for the best sample
         separation/distribution that can be achieved within these limits. The
         vendor will specify the device that this instruction is executed on and
         which excitation and emission spectra are available. At least one
@@ -4977,15 +4960,15 @@
         for s in sources:
             self._remove_cover(s["well"].container, "flow_analyze")
 
         return self._append_and_return(
             FlowAnalyze(dataref, FSC, SSC, neg_controls, samples, colors, pos_controls)
         )
 
-    def oligosynthesize(self, oligos: List[OligosynthesizeOligo]):
+    def oligosynthesize(self, oligos: List[dict]):
         """
         Specify a list of oligonucleotides to be synthesized and a destination
         for each product.
 
         Example Usage:
 
         .. code-block:: python
@@ -5044,22 +5027,20 @@
         Returns
         -------
         Oligosynthesize
             Returns the :py:class:`autoprotocol.instruction.Oligosynthesize`
             instruction created from the specified parameters
 
         """
-        return self._append_and_return(
-            Oligosynthesize([OligosynthesizeOligo(**o) for o in oligos])
-        )
+        return self._append_and_return(Oligosynthesize(oligos))
 
     def autopick(
         self,
         pick_groups: List[AutopickGroup],
-        criteria: Optional[Dict[str, Any]] = None,
+        criteria: Optional[dict] = None,
         dataref: str = "autopick",
     ):
         """
 
         Pick colonies from the agar-containing location(s) specified in
         `sources` to the location(s) specified in `dests` in highest to lowest
         rank order until there are no more colonies available.  If fewer than
@@ -5117,17 +5098,15 @@
             for d in group["to"]:
                 self._remove_cover(d.container, "autopick")
 
         criteria = {} if criteria is None else criteria
 
         return self._append_and_return(Autopick(groups, criteria, dataref))
 
-    def __process_pick_group(
-        self, pick_group: AutopickGroup
-    ) -> Dict[str, Union[WellGroup, int]]:
+    def __process_pick_group(self, pick_group: AutopickGroup) -> dict:
         if not isinstance(pick_group, AutopickGroup):
             raise TypeError(
                 "Autopick groups must use provided AutopickGroup dataclass."
             )
 
         # Check valid well inputs
         if not is_valid_well(pick_group.source):
@@ -5146,15 +5125,15 @@
         pick["min_abort"] = pick_group.min_abort
         return pick
 
     def mag_dry(
         self,
         head: str,
         container: Container,
-        duration: TIME,
+        duration: Union[str, Unit],
         new_tip: bool = False,
         new_instruction: bool = False,
     ):
         """
 
         Dry beads with magnetized tips above and outside a container for a set
         time.
@@ -5214,18 +5193,18 @@
         self._remove_cover(container, "mag_dry")
         return self._add_mag(mag, head, new_tip, new_instruction, "dry")
 
     def mag_incubate(
         self,
         head: str,
         container: Container,
-        duration: TIME,
+        duration: Union[str, Unit],
         magnetize: bool = False,
         tip_position: float = 1.5,
-        temperature: Optional[TEMPERATURE] = None,
+        temperature: Optional[Union[str, Unit]] = None,
         new_tip: bool = False,
         new_instruction: bool = False,
     ):
         """
 
         Incubate the container for a set time with tips set at `tip_position`.
 
@@ -5300,17 +5279,17 @@
         return self._add_mag(mag, head, new_tip, new_instruction, "incubate")
 
     def mag_collect(
         self,
         head: str,
         container: Container,
         cycles: int,
-        pause_duration: TIME,
+        pause_duration: Union[str, Unit],
         bottom_position: float = 0.0,
-        temperature: TEMPERATURE = None,
+        temperature: Union[str, Unit] = None,
         new_tip: bool = False,
         new_instruction: bool = False,
     ):
         """
 
         Collect beads from a container by cycling magnetized tips in and out
         of the container with an optional pause at the bottom of the insertion.
@@ -5387,19 +5366,19 @@
         self._remove_cover(container, "mag_collect")
         return self._add_mag(mag, head, new_tip, new_instruction, "collect")
 
     def mag_release(
         self,
         head: str,
         container: Container,
-        duration: TIME,
-        frequency: FREQUENCY,
+        duration: Union[str, Unit],
+        frequency: Union[str, Unit],
         center: float = 0.5,
         amplitude: float = 0.5,
-        temperature: Optional[TEMPERATURE] = None,
+        temperature: Optional[Union[str, Unit]] = None,
         new_tip: bool = False,
         new_instruction: bool = False,
     ):
         """
 
         Release beads into a container by cycling tips in and out of the
         container with tips unmagnetized.
@@ -5480,20 +5459,20 @@
         self._remove_cover(container, "mag_release")
         return self._add_mag(mag, head, new_tip, new_instruction, "release")
 
     def mag_mix(
         self,
         head: str,
         container: Container,
-        duration: TIME,
-        frequency: FREQUENCY,
+        duration: Union[str, Unit],
+        frequency: Union[str, Unit],
         center: float = 0.5,
         amplitude: float = 0.5,
         magnetize: bool = False,
-        temperature: Optional[TEMPERATURE] = None,
+        temperature: Optional[Union[str, Unit]] = None,
         new_tip: bool = False,
         new_instruction: bool = False,
     ):
         """
 
         Mix beads in a container by cycling tips in and out of the
         container.
@@ -5654,20 +5633,18 @@
 
         """
         return self._append_and_return(ImagePlate(ref, mode, dataref))
 
     def provision(
         self,
         resource_id: str,
-        dests: WellParam,
-        amounts: Optional[
-            Union[AMOUNT_CONCENTRATION, List[AMOUNT_CONCENTRATION]]
-        ] = None,
-        volumes: Optional[Union[VOLUME, List[VOLUME]]] = None,
-        informatics: Optional[List[Informatics]] = None,
+        dests: Union[Well, WellGroup, List[Well]],
+        amounts: Optional[Union[str, Unit, List[Unit], List[str]]] = None,
+        volumes: Optional[Union[str, Unit, List[Unit], List[str]]] = None,
+        informatics: Optional[List[dict]] = None,
     ):
         """
         Provision a commercial resource from a catalog into the specified
         destination well(s).  A new tip is used for each destination well
         specified to avoid contamination.
 
         Parameters
@@ -5819,15 +5796,17 @@
                     f"Provisioning of resources with measurement unit of {amount.unit} is not supported."
                 )
         if len(unique_measure_modes) != 1:
             raise ValueError("Received amounts with more than one measurement mode")
         measurement_mode = unique_measure_modes.pop()
         return measurement_mode
 
-    def flash_freeze(self, container: Union[str, Container], duration: TIME):
+    def flash_freeze(
+        self, container: Union[str, Container], duration: Union[str, Unit]
+    ):
         """
         Flash freeze the contents of the specified container by submerging it
         in liquid nitrogen for the specified amount of time.
 
         Example Usage:
 
         .. code-block:: python
@@ -5873,20 +5852,20 @@
             instruction created from the specified parameters
         """
 
         return self._append_and_return(FlashFreeze(container, duration))
 
     def sonicate(
         self,
-        wells: WellParam,
-        duration: TIME,
-        mode: SonicateMode,
-        mode_params: Union[SonicateModeParamsBath, SonicateModeParamsHorn],
-        frequency: Optional[FREQUENCY] = None,
-        temperature: Optional[TEMPERATURE] = None,
+        wells: Union[Well, WellGroup, List[Well]],
+        duration: Union[Unit, str],
+        mode: str,
+        mode_params: Dict,
+        frequency: Optional[Union[str, Unit]] = None,
+        temperature: Optional[Union[str, Unit]] = None,
     ):
         """
         Sonicate wells using high intensity ultrasonic vibrations.
 
         Example Usage:
 
         .. code-block:: python
@@ -6048,19 +6027,19 @@
         )
 
     def spe(
         self,
         well: Well,
         cartridge: str,
         pressure_mode: str,
-        load_sample: SpeLoadSample,
-        elute: List[SpeElute],
-        condition: Optional[List[SpeParams]] = None,
-        equilibrate: Optional[List[SpeParams]] = None,
-        rinse: Optional[List[SpeParams]] = None,
+        load_sample: Dict,
+        elute: List[dict],
+        condition: Optional[List[dict]] = None,
+        equilibrate: Optional[List[dict]] = None,
+        rinse: Optional[List[dict]] = None,
     ):
         """
         Apply a solid phase extraction (spe) technique to a sample.
 
         Example Usage:
 
         .. code-block:: python
@@ -6239,21 +6218,21 @@
                 equilibrate,
                 rinse,
             )
         )
 
     def image(
         self,
-        ref: Container,
-        mode: Union[str, ImageMode],
-        num_images: int,
+        ref: Optional[List[dict]],
+        mode: str,
         dataref: str,
-        backlighting: Optional[bool] = None,
+        num_images: int = 1,
+        backlighting: str = None,
+        exposure: Optional[dict] = None,
         magnification: float = 1.0,
-        exposure: Optional[ImageExposure] = None,
     ):
         """
         Capture an image of the specified container.
 
                 Example Usage:
 
                 .. code-block:: python
@@ -6331,21 +6310,54 @@
         Raises
         ------
         TypeError
             Invalid input types, e.g. num_images is not a positive integer
         ValueError
             Invalid exposure parameter supplied
         """
-        allowed_image_modes = ImageMode.__dict__.get("_member_names_")
-        if not mode in allowed_image_modes:
-            raise ValueError(f"image mode must be one of: {allowed_image_modes}")
-        if num_images <= 0:
+        valid_image_modes = ["top", "bottom", "side"]
+        if not isinstance(ref, Container):
+            raise TypeError(f"image ref: {ref} has to be of type Container")
+        if mode not in valid_image_modes:
+            raise ValueError(
+                f"specified mode: {mode} must be one of " f"{valid_image_modes}"
+            )
+        if not isinstance(dataref, str):
+            raise TypeError("dataref must be of type String.")
+        if not isinstance(num_images, int) or num_images <= 0:
             raise TypeError("num_images must be a positive integer.")
-        if magnification <= 0:
-            raise TypeError("magnification must be a number.")
+        if magnification:
+            if not isinstance(magnification, (float, int)) or magnification <= 0:
+                raise TypeError("magnification must be a number.")
+        if backlighting:
+            if not isinstance(backlighting, bool):
+                raise TypeError("backlighting must be a boolean.")
+        if exposure:
+            valid_exposure_params = ["shutter_speed", "iso", "aperture"]
+            if not isinstance(exposure, dict):
+                raise TypeError(
+                    f"exposure must be a dict with optional keys: "
+                    f"{valid_exposure_params}."
+                )
+            if not all(k in valid_exposure_params for k in exposure):
+                raise ValueError(
+                    f"Invalid exposure param.  Valid params: "
+                    f"{valid_exposure_params}."
+                )
+            shutter_speed = exposure.get("shutter_speed")
+            if shutter_speed:
+                shutter_speed = parse_unit(shutter_speed, "millimeter/s")
+            iso = exposure.get("iso")
+            if iso:
+                if not isinstance(iso, (float, int)):
+                    raise TypeError("iso must be a number.")
+            aperture = exposure.get("aperture")
+            if aperture:
+                if not isinstance(aperture, (float, int)):
+                    raise TypeError("aperture must be a number.")
 
         return self._append_and_return(
             Image(ref, mode, dataref, num_images, backlighting, exposure, magnification)
         )
 
     def _ref_for_well(self, well: Well):
         return f"{self._ref_for_container(well.container)}/{well.index}"
@@ -6434,29 +6446,15 @@
             return last_instruction
         else:
             return self._append_and_return(
                 MagneticTransfer(groups=[[{sub_op_name: sub_op}]], magnetic_head=head)
             )
 
     # pylint: disable=protected-access
-    def _refify(
-        self,
-        op_data: Union[
-            Dict[str, Any],
-            List[Any],
-            Well,
-            WellGroup,
-            Container,
-            Unit,
-            Instruction,
-            Ref,
-            Compound,
-            Informatics,
-        ],
-    ):
+    def _refify(self, op_data: Union[dict, str, list]):
         """
         Unpacks protocol objects into Autoprotocol compliant ones
 
         Used by as_dict().
 
         Parameters
         ----------
@@ -6479,23 +6477,23 @@
         elif isinstance(op_data, Container):
             return self._ref_for_container(op_data)
         elif isinstance(op_data, Unit):
             return str(op_data)
         elif isinstance(op_data, Instruction):
             return self._refify(op_data._as_AST())
         elif isinstance(op_data, Ref):
-            return op_data.opts.as_dict()
+            return op_data.opts
         elif isinstance(op_data, Compound):
             return op_data.as_dict()
         elif isinstance(op_data, Informatics):
             return self._refify(op_data.as_dict())
         else:
             return op_data
 
-    def _ref_containers_and_wells(self, params: Dict[Any, Any]):
+    def _ref_containers_and_wells(self, params: dict):
         """
         Used by harness.run() to process JSON container and well references
 
         .. code-block:: python
 
             parameters = {
                 "sample": {
@@ -6604,15 +6602,15 @@
             else:
                 parameters[str(k)] = v
 
         return parameters
 
     def measure_concentration(
         self,
-        wells: WellParam,
+        wells: Union[List[Well], WellGroup, Well],
         dataref: str,
         measurement: str,
         volume: str = "2:microliter",
     ):
         """
         Measure the concentration of DNA, ssDNA, RNA or protein in the
         specified volume of the source aliquots.
@@ -6749,15 +6747,15 @@
 
         """
         if not isinstance(container, Container):
             raise TypeError(f"{container} has to be of type Container")
 
         return self._append_and_return(MeasureMass(container, dataref))
 
-    def measure_volume(self, wells: WellParam, dataref: str):
+    def measure_volume(self, wells: Union[List[Well], WellGroup, Well], dataref: str):
         """
         Measure the volume of each well in wells.
 
         Example Usage:
 
         .. code-block:: python
 
@@ -6814,16 +6812,16 @@
         if not is_valid_well(wells):
             raise TypeError("Wells must be of type Well, list of Wells, or WellGroup.")
         wells = WellGroup(wells)
         return self._append_and_return(MeasureVolume(wells, dataref))
 
     def count_cells(
         self,
-        wells: WellParam,
-        volume: VOLUME,
+        wells: Union[List[Well], WellGroup, Well],
+        volume: Unit,
         dataref: str,
         labels: Optional[List[str]] = None,
     ):
         """
         Count the number of cells in a sample that are positive/negative
         for a given set of labels.
 
@@ -6916,18 +6914,18 @@
         )
 
     def spectrophotometry(
         self,
         dataref: str,
         obj: Union[Container, str],
         groups: List,
-        interval: Optional[TIME] = None,
+        interval: Optional[Union[Unit, str]] = None,
         num_intervals: Optional[int] = None,
-        temperature: Optional[TEMPERATURE] = None,
-        shake_before: Optional[SpectrophotometryShakeBefore] = None,
+        temperature: Optional[Union[Unit, str]] = None,
+        shake_before: Optional[dict] = None,
     ):
         """
         Generates an instruction with one or more plate reading steps
         executed on a single plate with the same device. This could be
         executed once, or at a defined interval, across some total duration.
 
 
@@ -7141,20 +7139,15 @@
         if num_intervals and not isinstance(num_intervals, int):
             raise TypeError(f"Invalid num_intervals {num_intervals}, must be an int.")
 
         if temperature is not None:
             temperature = parse_unit(temperature, "celsius")
 
         if shake_before is not None:
-            shake_before = Spectrophotometry.builders.shake_before(
-                duration=shake_before.duration,
-                frequency=shake_before.frequency,
-                path=shake_before.path,
-                amplitude=shake_before.amplitude,
-            )
+            shake_before = Spectrophotometry.builders.shake_before(**shake_before)
 
         shake_groups = [_ for _ in groups if _["mode"] == "shake"]
 
         any_shake_duration_undefined = any(
             _["mode_params"].get("duration") is None for _ in shake_groups
         )
 
@@ -7175,26 +7168,26 @@
                 shake_before=shake_before,
             )
         )
 
     # pylint: disable=protected-access
     def transfer(
         self,
-        source: WellParam,
-        destination: WellParam,
-        volume: Union[VOLUME, List[VOLUME]],
+        source: Union[Well, WellGroup, List[Well]],
+        destination: Union[Well, WellGroup, List[Well]],
+        volume: Union[str, Unit, List[str], List[Unit]],
         rows: int = 1,
         columns: int = 1,
         source_liquid: LiquidClass = LiquidClass,
         destination_liquid: LiquidClass = LiquidClass,
         method: Transfer = Transfer,
         one_tip: bool = False,
-        density: Optional[DENSITY] = None,
+        density: Optional[Union[Unit, str]] = None,
         mode: Optional[str] = None,
-        informatics: Optional[List[Informatics]] = None,
+        informatics: Optional[List[dict]] = None,
     ):
         """Generates LiquidHandle instructions between wells
 
         Transfer liquid between specified pairs of source & destination wells.
 
         Parameters
         ----------
@@ -7781,18 +7774,17 @@
         for src, des, met in zip(source_liquid, destination_liquid, method):
             met._shape = LiquidHandle.builders.shape(**shape)
             met._source_liquid = src
             met._destination_liquid = des
 
         # apply tip types to transfer methods
         for vol, met in zip(volume, method):
-            if not met.tip_type:
+            if met._has_calibration() and not met.tip_type:
                 try:
-                    # met.tip_type = met._rec_tip_type(vol)
-                    met._rec_tip_type(vol)
+                    met.tip_type = met._rec_tip_type(vol)
                 except RuntimeError:
                     met.tip_type = met._get_sorted_tip_types()[-1].name
 
         # if one tip is true then all methods need to have the same tip_type
         if one_tip is True:
             tip_types = [_.tip_type for _ in method]
             if not all(_ == tip_types[0] for _ in tip_types):
@@ -7854,16 +7846,16 @@
                 )
             )
         return self._append_and_return(instructions)
 
     # pylint: disable=protected-access
     def mix(
         self,
-        well: WellParam,
-        volume: Union[VOLUME, List[VOLUME]],
+        well: Union[Well, WellGroup, List[Well]],
+        volume: Union[str, Unit, List[str], List[Unit]],
         rows: int = 1,
         columns: int = 1,
         liquid: LiquidClass = LiquidClass,
         method: Mix = Mix,
         one_tip: bool = False,
         mode: Optional[str] = None,
     ):
@@ -7967,15 +7959,15 @@
             )
 
         See Also
         --------
         Mix : base LiquidHandleMethod for mix operations
         """
 
-        def location_helper(aliquot: Well, volume: Unit, method: Mix):
+        def location_helper(aliquot, volume, method):
             """Generates LiquidHandle mix locations
 
             Parameters
             ----------
             aliquot : Well
                 Wells to transfer mix liquid in.
             volume : Unit
@@ -8101,16 +8093,16 @@
             )
         return self._append_and_return(instructions)
 
     def spread(
         self,
         source: Well,
         dest: Well,
-        volume: VOLUME = "50:microliter",
-        dispense_speed: ACCELERATION = "20:microliter/second",
+        volume: Union[str, Unit] = "50:microliter",
+        dispense_speed: Union[str, Unit] = "20:microliter/second",
     ):
         """
         Spread the specified volume of the source aliquot across the surface of
         the agar contained in the object container.
 
         Uses a spiral pattern generated by a set of liquid_handle instructions.
 
@@ -8253,15 +8245,15 @@
                 location=dest, transports=dispense_transport_list
             ),
         ]
 
         return self._append_and_return(LiquidHandle(location))
 
     def _transfer_volume(
-        self, source: Well, destination: Well, volume: Unit, shape: DispenseShape
+        self, source: Well, destination: Well, volume: Unit, shape: dict
     ):
         """
         Transfers volume and properties between aliquots.
 
         Parameters
         ----------
         source : Well
@@ -8296,18 +8288,18 @@
                 dest_well.volume += volume
             else:
                 dest_well.volume = volume
 
     def evaporate(
         self,
         ref: Container,
-        mode: EvaporateMode,
-        duration: TIME,
-        evaporator_temperature: TEMPERATURE,
-        mode_params: Optional[EvaporateModeParams] = None,
+        mode: str,
+        duration: Union[Unit, str],
+        evaporator_temperature: Union[Unit, str],
+        mode_params: Optional[dict] = None,
     ):
         """
         Removes liquid or moisture from a container using the mode specified.
 
         Example Usage:
 
         .. code-block:: python
```

### Comparing `autoprotocol-9.1.0/autoprotocol/unit.py` & `autoprotocol-9.1.1/autoprotocol/unit.py`

 * *Files identical despite different names*

### Comparing `autoprotocol-9.1.0/autoprotocol/util.py` & `autoprotocol-9.1.1/autoprotocol/util.py`

 * *Files identical despite different names*

### Comparing `autoprotocol-9.1.0/autoprotocol.egg-info/PKG-INFO` & `autoprotocol-9.1.1/autoprotocol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoprotocol
-Version: 9.1.0
+Version: 9.1.1
 Summary: Python library for generating Autoprotocol
 Home-page: https://github.com/autoprotocol/autoprotocol-python
 Maintainer: The Autoprotocol Development Team
 Maintainer-email: support@strateos.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `autoprotocol-9.1.0/autoprotocol.egg-info/SOURCES.txt` & `autoprotocol-9.1.1/autoprotocol.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -26,9 +26,8 @@
 autoprotocol/liquid_handle/liquid_class.py
 autoprotocol/liquid_handle/liquid_handle_method.py
 autoprotocol/liquid_handle/mix.py
 autoprotocol/liquid_handle/tip_type.py
 autoprotocol/liquid_handle/transfer.py
 autoprotocol/types/__init__.py
 autoprotocol/types/protocol.py
-autoprotocol/types/ref.py
 test/test_util.py
```

### Comparing `autoprotocol-9.1.0/setup.py` & `autoprotocol-9.1.1/setup.py`

 * *Files identical despite different names*

