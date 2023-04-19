# Comparing `tmp/paitest-0.0.11-py3-none-any.whl.zip` & `tmp/paitest-0.0.12-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 24594 bytes, number of entries: 13
+Zip file size: 24739 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       40 b- defN 80-Jan-01 00:00 paitest/__init__.py
 -rw-r--r--  2.0 unx      267 b- defN 80-Jan-01 00:00 paitest/frames/__init__.py
 -rw-r--r--  2.0 unx     2581 b- defN 80-Jan-01 00:00 paitest/frames/coord.py
 -rw-r--r--  2.0 unx      805 b- defN 80-Jan-01 00:00 paitest/frames/coord.pyi
--rw-r--r--  2.0 unx    14155 b- defN 80-Jan-01 00:00 paitest/frames/frame.py
+-rw-r--r--  2.0 unx    14188 b- defN 80-Jan-01 00:00 paitest/frames/frame.py
 -rw-r--r--  2.0 unx     4706 b- defN 80-Jan-01 00:00 paitest/frames/frame_params.py
 -rw-r--r--  2.0 unx      230 b- defN 80-Jan-01 00:00 paitest/log.py
--rw-r--r--  2.0 unx    17670 b- defN 80-Jan-01 00:00 paitest/paitest.py
--rw-r--r--  2.0 unx     2045 b- defN 80-Jan-01 00:00 paitest/paitest.pyi
--rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 paitest-0.0.11.dist-info/LICENSE
--rw-r--r--  2.0 unx     3379 b- defN 80-Jan-01 00:00 paitest-0.0.11.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 paitest-0.0.11.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1005 b- defN 16-Jan-01 00:00 paitest-0.0.11.dist-info/RECORD
-13 files, 81494 bytes uncompressed, 22940 bytes compressed:  71.9%
+-rw-r--r--  2.0 unx    18563 b- defN 80-Jan-01 00:00 paitest/paitest.py
+-rw-r--r--  2.0 unx     1692 b- defN 80-Jan-01 00:00 paitest/paitest.pyi
+-rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 paitest-0.0.12.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3451 b- defN 80-Jan-01 00:00 paitest-0.0.12.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 paitest-0.0.12.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1005 b- defN 16-Jan-01 00:00 paitest-0.0.12.dist-info/RECORD
+13 files, 82139 bytes uncompressed, 23085 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: paitest/paitest.py
 Comment: 
 
 Filename: paitest/paitest.pyi
 Comment: 
 
-Filename: paitest-0.0.11.dist-info/LICENSE
+Filename: paitest-0.0.12.dist-info/LICENSE
 Comment: 
 
-Filename: paitest-0.0.11.dist-info/METADATA
+Filename: paitest-0.0.12.dist-info/METADATA
 Comment: 
 
-Filename: paitest-0.0.11.dist-info/WHEEL
+Filename: paitest-0.0.12.dist-info/WHEEL
 Comment: 
 
-Filename: paitest-0.0.11.dist-info/RECORD
+Filename: paitest-0.0.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## paitest/frames/frame.py

```diff
@@ -75,27 +75,26 @@
     @staticmethod
     def GenConfigGroup(
         header: FST,
         chip_coord: Coord,
         core_coord: Coord,
         core_star_coord: Coord,
         test_chip_coord: Coord,
-    ) -> List[int]:
+    ) -> Tuple[int, ...]:
         ConfigFrameGroup: List[int] = []
-
         param_reg = FrameGen._GenParamReg(test_chip_coord)
 
         for i in range(3):
             ConfigFrameGroup.append(
                 FrameGen.GenConfigFrame(
                     header, chip_coord, core_coord, core_star_coord, param_reg[i]
                 )
             )
 
-        return ConfigFrameGroup
+        return tuple(ConfigFrameGroup)
 
     @staticmethod
     def _GenParamReg(
         test_chip_coord: Coord,
         *,
         is_random: bool = True,
         is_legal: bool = False,
@@ -105,15 +104,15 @@
         spike_width_type: Optional[SpikeWidthType] = None,
         neuron_num: Optional[int] = None,
         pool_max_en: Optional[bool] = None,
         tick_wait_start: Optional[int] = None,
         tick_wait_end: Optional[int] = None,
         snn_en: Optional[bool] = None,
         target_lcn: Optional[int] = None,
-    ) -> List[int]:
+    ) -> Tuple[int, ...]:
         high3, low7 = test_chip_coord_split(test_chip_coord)
 
         param_reg: List[int] = []
 
         if is_random:
             if not is_legal:
                 # Don't care 'tick_wait_start' split in #1 and #2
@@ -124,15 +123,15 @@
                 param_reg.append(low7 << CFM.TEST_CHIP_ADDR_LOW7_OFFSET)
             else:
                 # Do legal geenration
                 pass
         else:
             pass
 
-        return param_reg
+        return tuple(param_reg)
 
     """Functions of Test Frames Generation"""
 
     @staticmethod
     def _GenTestFrame(
         header: FST,
         chip_coord: Coord,
@@ -186,15 +185,15 @@
             FST.TEST_TYPE2, test_chip_coord, core_coord, core_star_coord, param_reg
         )
 
 
 class FrameDecoder:
     """Frame decoder"""
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.groups_len: int
         self._frame: int
         self._frames_group: Tuple[int, ...]
 
         # Total attributes dictionary
         self._attr_dict: Dict[str, Any] = {}
```

## paitest/paitest.py

```diff
@@ -40,21 +40,23 @@
 
     def Get1GroupForNCoresWithNParams(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
+        verbose: bool = False,
     ) -> Tuple[Tuple[int, ...], ...]:
         """
         Generate 1 group(case) for 'N' random cores coordinates with 'N' different parameters.
 
         - `N`: How many cores coordinates under test.
         - `save_dir`: Where to save the frames files.
         - `masked_core_coord`: to avoid generating the specific core coordinate.
+        - `verbose`: whether to display log.
 
         :return: Three tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
         """
         self._ensure_cores(N)
 
         if save_dir:
             work_dir = self._ensure_dir(save_dir)
@@ -76,69 +78,76 @@
         params = self._GetNParams(N, core_coords, False)
 
         cf_list: List[int] = []
         ti_list: List[int] = []
         to_list: List[int] = []
 
         for i in range(N):
-            logger.info(f"Generating test group #{i+1}/{N}...")
+            if verbose:
+                logger.info(f"Generating test group #{i+1}/{N}...")
             core_coord = core_coords[i]
             param = params[i]
 
             for j in range(3):
                 config_frame = FrameGen.GenConfigFrame(
                     FST.CONFIG_TYPE2,
                     self._fixed_chip_coord,
                     core_coord,
                     self._fixed_core_star_coord,
                     param[j],
                 )
-                cf_list.append(config_frame)
-                logger.info(
-                    "Config frame   #%d/3:  0x%x in group #%d/%d"
-                    % (j + 1, config_frame, i + 1, N)
-                )
-
                 testout_frame = FrameGen.GenTest2OutFrame(
                     test_chip_coord, core_coord, self._fixed_core_star_coord, param[j]
                 )
+                cf_list.append(config_frame)
                 to_list.append(testout_frame)
-                logger.info(
-                    "Test out frame #%d/3:  0x%x in group #%d/%d"
-                    % (j + 1, testout_frame, i + 1, N)
-                )
+
+                if verbose:
+                    logger.info(
+                        "Config frame   #%d/3:  0x%x in group #%d/%d"
+                        % (j + 1, config_frame, i + 1, N)
+                    )
+                    logger.info(
+                        "Test out frame #%d/3:  0x%x in group #%d/%d"
+                        % (j + 1, testout_frame, i + 1, N)
+                    )
 
             testin_frame = FrameGen.GenTest2InFrame(
-                test_chip_coord, core_coord, self._fixed_core_star_coord
+                self._fixed_chip_coord, core_coord, self._fixed_core_star_coord
             )
             ti_list.append(testin_frame)
-            logger.info(
-                "Test in frame  #1/1:  0x%x in group #%d/%d" % (testin_frame, i + 1, N)
-            )
+            
+            if verbose:
+                logger.info(
+                    "Test in frame  #1/1:  0x%x in group #%d/%d"
+                    % (testin_frame, i + 1, N)
+                )
 
         if isinstance(work_dir, Path):
-            self.SaveFrames(work_dir / "config.bin", cf_list)
-            self.SaveFrames(work_dir / "testin.bin", ti_list)
-            self.SaveFrames(work_dir / "testout.bin", to_list)
+            self.SaveFrames(work_dir / "config.bin", cf_list, verbose)
+            self.SaveFrames(work_dir / "testin.bin", ti_list, verbose)
+            self.SaveFrames(work_dir / "testout.bin", to_list, verbose)
 
         return tuple(cf_list), tuple(ti_list), tuple(to_list)
 
     def Get1GroupForNCoresWith1Param(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
+        verbose: bool = False,
     ) -> Tuple[Tuple[int, ...], ...]:
         """
         Generate 1 group(case) for 'N' random cores coordinates with the same parameters.
 
         - `N`: How many cores coordinates under test.
         - `save_dir`: Where to save the frames files.
         - `masked_core_coord`: to avoid generating the specific core coordinate.
+        - `verbose`: whether to display log.
 
         :return: Three tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
         """
         self._ensure_cores(N)
 
         if save_dir:
             work_dir = self._ensure_dir(save_dir)
@@ -153,68 +162,74 @@
             _masked_core_coord = Coord(masked_core_coord)
         else:
             _masked_core_coord = None
 
         core_coords = self._GetNCoresCoord(N, _masked_core_coord)
 
         # 3. Get the parameters reg.
-        param: List[int] = self._Get1Param(core_coords, False)
+        param: Tuple[int, ...] = self._Get1Param(core_coords, False)
 
         cf_list: List[int] = []
         ti_list: List[int] = []
         to_list: List[int] = []
 
         for i in range(N):
-            logger.info(f"Generating test group #{i+1}/{N}...")
+            if verbose:
+                logger.info(f"Generating test group #{i+1}/{N}...")
             core_coord = core_coords[i]
 
             for j in range(3):
                 config_frame = FrameGen.GenConfigFrame(
                     FST.CONFIG_TYPE2,
                     self._fixed_chip_coord,
                     core_coord,
                     self._fixed_core_star_coord,
                     param[j],
                 )
-                cf_list.append(config_frame)
-                logger.info(
-                    "Config frame   #%d/3:  0x%x in group #%d/%d"
-                    % (j + 1, config_frame, i + 1, N)
-                )
-
                 testout_frame = FrameGen.GenTest2OutFrame(
                     test_chip_coord, core_coord, self._fixed_core_star_coord, param[j]
                 )
+                cf_list.append(config_frame)
                 to_list.append(testout_frame)
-                logger.info(
-                    "Test out frame #%d/3:  0x%x in group #%d/%d"
-                    % (j + 1, testout_frame, i + 1, N)
-                )
+
+                if verbose:
+                    logger.info(
+                        "Config frame   #%d/3:  0x%x in group #%d/%d"
+                        % (j + 1, config_frame, i + 1, N)
+                    )
+                    logger.info(
+                        "Test out frame #%d/3:  0x%x in group #%d/%d"
+                        % (j + 1, testout_frame, i + 1, N)
+                    )
 
             testin_frame = FrameGen.GenTest2InFrame(
-                test_chip_coord, core_coord, self._fixed_core_star_coord
+                self._fixed_chip_coord, core_coord, self._fixed_core_star_coord
             )
             ti_list.append(testin_frame)
-            logger.info(
-                "Test in frame  #1/1:  0x%x in group #%d/%d" % (testin_frame, i + 1, N)
-            )
+
+            if verbose:
+                logger.info(
+                    "Test in frame  #1/1:  0x%x in group #%d/%d"
+                    % (testin_frame, i + 1, N)
+                )
 
         if isinstance(work_dir, Path):
-            self.SaveFrames(work_dir / "config.bin", cf_list)
-            self.SaveFrames(work_dir / "testin.bin", ti_list)
-            self.SaveFrames(work_dir / "testout.bin", to_list)
+            self.SaveFrames(work_dir / "config.bin", cf_list, verbose)
+            self.SaveFrames(work_dir / "testin.bin", ti_list, verbose)
+            self.SaveFrames(work_dir / "testout.bin", to_list, verbose)
 
         return tuple(cf_list), tuple(ti_list), tuple(to_list)
 
     def GetNGroupsFor1CoreWithNParams(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
+        verbose: bool = False,
     ) -> Tuple[Tuple[int, ...], ...]:
         """
         Generate 'N' groups(cases) for 1 random core coordinate with 'N' different parameters.
 
         - `N`: How many test groups(cases) of 1 core will be generated.
         - `save_dir`: Where to save the frames files.
         - `masked_core_coord`: to avoid generating the specific core coordinate.
@@ -243,52 +258,57 @@
         params = self._GetNParams(N, core_coord, False)
 
         cf_list: List[int] = []
         ti_list: List[int] = []
         to_list: List[int] = []
 
         for i in range(N):
-            logger.info(f"Generating test group #{i+1}/{N}...")
+            if verbose:
+                logger.info(f"Generating test group #{i+1}/{N}...")
             param = params[i]
 
             for j in range(3):
                 config_frame = FrameGen.GenConfigFrame(
                     FST.CONFIG_TYPE2,
                     self._fixed_chip_coord,
                     core_coord,
                     self._fixed_core_star_coord,
                     param[j],
                 )
-                cf_list.append(config_frame)
-                logger.info(
-                    "Config frame   #%d/3:  0x%x in group #%d/%d"
-                    % (j + 1, config_frame, i + 1, N)
-                )
-
                 testout_frame = FrameGen.GenTest2OutFrame(
                     test_chip_coord, core_coord, self._fixed_core_star_coord, param[j]
                 )
+                cf_list.append(config_frame)
                 to_list.append(testout_frame)
-                logger.info(
-                    "Test out frame #%d/3:  0x%x in group #%d/%d"
-                    % (j + 1, testout_frame, i + 1, N)
-                )
+
+                if verbose:
+                    logger.info(
+                        "Config frame   #%d/3:  0x%x in group #%d/%d"
+                        % (j + 1, config_frame, i + 1, N)
+                    )
+                    logger.info(
+                        "Test out frame #%d/3:  0x%x in group #%d/%d"
+                        % (j + 1, testout_frame, i + 1, N)
+                    )
 
             testin_frame = FrameGen.GenTest2InFrame(
-                test_chip_coord, core_coord, self._fixed_core_star_coord
+                self._fixed_chip_coord, core_coord, self._fixed_core_star_coord
             )
             ti_list.append(testin_frame)
-            logger.info(
-                "Test in frame  #1/1:  0x%x in group #%d/%d" % (testin_frame, i + 1, N)
-            )
+
+            if verbose:
+                logger.info(
+                    "Test in frame  #1/1:  0x%x in group #%d/%d"
+                    % (testin_frame, i + 1, N)
+                )
 
         if isinstance(work_dir, Path):
-            self.SaveFrames(work_dir / "config.bin", cf_list)
-            self.SaveFrames(work_dir / "testin.bin", ti_list)
-            self.SaveFrames(work_dir / "testout.bin", to_list)
+            self.SaveFrames(work_dir / "config.bin", cf_list, verbose)
+            self.SaveFrames(work_dir / "testin.bin", ti_list, verbose)
+            self.SaveFrames(work_dir / "testout.bin", to_list, verbose)
 
         return tuple(cf_list), tuple(ti_list), tuple(to_list)
 
     def ReplaceCoreCoord(
         self,
         frames: Union[int, List[int], Tuple[int, ...]],
         new_core_coord: Optional[Union[Tuple[int, int], Coord]] = None,
@@ -322,30 +342,35 @@
             return self._ReplaceCoreCoordIn1Frame(_frame, _new_core_coord)
         else:
             _frames = list(frames)
             return self._ReplaceCoreCoordInNFrames(_frames, _new_core_coord)
 
     @staticmethod
     def SaveFrames(
-        save_path: Union[str, Path], frames: Union[int, List[int], Tuple[int, ...]]
+        save_path: Union[str, Path],
+        frames: Union[int, List[int], Tuple[int, ...]],
+        verbose: bool = False,
     ) -> None:
         """Write frames into specific binary file. Must be '.bin' suffix."""
 
         _path = Path(save_path)
 
         if not _path.suffix == ".bin":
-            raise ValueError
+            raise ValueError(f"Only support .bin file: {_path}")
 
         with open(_path, "wb") as f:
             if isinstance(frames, int):
                 f.write(frames.to_bytes(8, "big"))
             else:
                 for frame in frames:
                     f.write(frame.to_bytes(8, "big"))
 
+            if verbose:
+                logger.info(f"Saved frame(s) into {_path} OK")
+
     def _Get1CoreCoord(self, masked_coord: Optional[Coord] = None) -> Coord:
         """
         Generate a random core coordinate. Indicate the masked one to avoid generating the same one
         """
         return self._GetNCoresCoord(N=1, masked_coord=masked_coord)[0]
 
     def _GetNCoresCoord(
@@ -379,38 +404,37 @@
         generator = _CoordGenerator()
         core_coord_list = [next(generator) for _ in range(N)]
 
         return core_coord_list
 
     def _Get1Param(
         self, core_coords: Union[List[Coord], Coord], is_legal: bool = False
-    ) -> List[int]:
+    ) -> Tuple[int, ...]:
         """Generate one group parameter for parameter register"""
         return self._GetNParams(1, core_coords, is_legal)[0]
 
     def _GetNParams(
         self,
         N: int,
         core_coords: Union[List[Coord], Coord],
         is_legal: bool = False,
-    ) -> List[List[int]]:
+    ) -> List[Tuple[int, ...]]:
         """
         Generate 'N' parameters reg for parameter register.
         - `is_legal`: whether to generate legal parameters for every core
         """
 
         def _ParamGenerator():
             test_chip_coord: Coord = self._direction.value + self._fixed_chip_coord
 
             while True:
                 for core_coord in _core_coords:
                     if is_legal:
                         # TODO: Do legal generation here, including direction config
-                        param = [0, 0, 0]
-                        pass
+                        raise NotImplementedError
                     else:
                         param = FrameGen.GenConfigGroup(
                             FST.CONFIG_TYPE2,
                             self._fixed_chip_coord,
                             core_coord,
                             self._fixed_core_star_coord,
                             test_chip_coord,
```

## paitest/paitest.pyi

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, List, Optional, Union, overload
+from typing import Tuple, List, Optional, Union
 import sys
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 from pathlib import Path
 
 class paitest:
@@ -20,43 +20,37 @@
         ) -> None: ...
 
     def Get1GroupForNCoresWithNParams(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
-        masked_core_coord: Optional[Tuple[int, int]] = None
+        masked_core_coord: Optional[Tuple[int, int]] = None,
+        verbose: bool = False
     ) -> Tuple[Tuple[int, ...], ...]: ...
     def Get1GroupForNCoresWith1Param(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
-        masked_core_coord: Optional[Tuple[int, int]] = None
+        masked_core_coord: Optional[Tuple[int, int]] = None,
+        verbose: bool = False
     ) -> Tuple[Tuple[int, ...], ...]: ...
     def GetNGroupsFor1CoreWithNParams(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
-        masked_core_coord: Optional[Tuple[int, int]] = None
+        masked_core_coord: Optional[Tuple[int, int]] = None,
+        verbose: bool = False
     ) -> Tuple[Tuple[int, ...], ...]: ...
-    @overload
-    def ReplaceCoreCoord(self, frames: int) -> int: ...
-    @overload
-    def ReplaceCoreCoord(self, frames: List[int]) -> Tuple[int, ...]: ...
-    @overload
-    def ReplaceCoreCoord(self, frames: Tuple[int, ...]) -> Tuple[int, ...]: ...
-    @overload
-    def ReplaceCoreCoord(self, frames: int, new_core_coord: Tuple[int, int]) -> int: ...
-    @overload
     def ReplaceCoreCoord(
-        self, frames: List[int], new_core_coord: Tuple[int, int]
-    ) -> Tuple[int, ...]: ...
-    @overload
-    def ReplaceCoreCoord(
-        self, frames: Tuple[int, ...], new_core_coord: Tuple[int, int]
-    ) -> Tuple[int, ...]: ...
+        self,
+        frames: Union[int, List[int], Tuple[int, ...]],
+        new_core_coord: Tuple[int, int],
+    ) -> int: ...
     @staticmethod
     def SaveFrames(
-        save_path: Union[str, Path], frames: Union[int, List[int], Tuple[int, ...]]
+        save_path: Union[str, Path],
+        frames: Union[int, List[int], Tuple[int, ...]],
+        verbose: bool = False,
     ) -> None: ...
```

## Comparing `paitest-0.0.11.dist-info/LICENSE` & `paitest-0.0.12.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `paitest-0.0.11.dist-info/METADATA` & `paitest-0.0.12.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paitest
-Version: 0.0.11
+Version: 0.0.12
 Summary: Test module for PAICORE 2.0
 Home-page: https://github.com/PAICookers/PAITest
 License: AGPL v3.0
 Keywords: PAICookers,PAITest,PAICORE
 Author: KafCoppelia
 Author-email: k740677208@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -24,15 +24,15 @@
 
 # PAITest
 
 </div>
 
 ## 📦 版本
 
-[v0.0.11 Prerelease](https://github.com/PAICookers/PAITest/releases/tag/v0.0.11)
+[v0.0.12 Prerelease](https://github.com/PAICookers/PAITest/releases/tag/v0.0.12)
 
 ## 🛠️ 使用生成
 
 配置帧及对应测试输入帧，以实现硬件通路的简单测试，后续将芯片实际测试输出帧与预期结果进行对比即可。
 
 ⚠️ 由于配置帧/测试帧I型需要配合串口配置使用，因此目前仅采用**配置/测试帧II型**方案，且 `CHIP_ADDR` 与 `CORE*_ADDR` 均固定为 `(0, 0)`。
 
@@ -40,58 +40,54 @@
 
    ```python
    from paitest import paitest
 
    # Define the direction of test chip
    PAITestManager = paitest("EAST")
    ```
+2. `Get1GroupForNCoresWithNParams`，产生一组针对 `N` 个核的配置-测试帧，每个核配置不同参数。可以指定单个需要**屏蔽**的核坐标。`verbose=True` 以开启日志显示，默认关闭。
 
-2. `Get1GroupForNCoresWithNParams`，产生一组针对 `N` 个核的配置-测试帧，每个核配置不同参数。可以指定单个需要**屏蔽**的核坐标
+   ```python
+   groups = 10             # Generate 10 groups
+   save_to_dir="./test"    # Save frames into ./test directory
 
-    ```python
-    groups = 10             # Generate 10 groups
-    save_to_dir="./test"    # Save frames into ./test directory
-
-    # Generate configuration frames, testin & testout frames
-    cf, ti, to = PAITestManager.Get1GroupForNCoresWithNParams(groups, save_dir=save_to_dir)
-
-    # Mask a cord coordinate so that avoid generating the same coordinate.
-    cf, ti, to = PAITestManager.Get1GroupForNCoresWithNParams(groups, 
-        save_dir=save_to_dir, masked_core_coord=(12, 16))
-    ```
+   # Generate configuration frames, testin & testout frames
+   cf, ti, to = PAITestManager.Get1GroupForNCoresWithNParams(groups, save_dir=save_to_dir)
 
+   # Mask a cord coordinate so that avoid generating the same coordinate.
+   # And enable verbose logging
+   cf, ti, to = PAITestManager.Get1GroupForNCoresWithNParams(groups, 
+       save_dir=save_to_dir, masked_core_coord=(12, 16), verbose=True)
+   ```
 3. `Get1GroupForNCoresWith1Param`，产生1组针对 `N` 个核的配置-测试帧，每个核配置相同参数。可以指定单个需要**屏蔽**的核坐标
 
-    ```python
-    # Same as Get1GroupForNCoresWithNParams
-    cf, ti, to = PAITestManager.Get1GroupForNCoresWith1Param(10, save_dir="./test")
-    ```
-
+   ```python
+   # Same as Get1GroupForNCoresWithNParams
+   cf, ti, to = PAITestManager.Get1GroupForNCoresWith1Param(10, save_dir="./test")
+   ```
 4. `GetNGroupsFor1CoreWithNParams`，产生 `N` 组针对1个核的配置-测试帧，每个核配置不同参数。可以指定单个需要**屏蔽**的核坐标
 
-    ```python
-    # Same as Get1GroupForNCoresWithNParams
-    cf, ti, to = PAITestManager.GetNGroupsFor1CoreWithNParams(1, save_dir="./test")
-    ```
-
+   ```python
+   # Same as Get1GroupForNCoresWithNParams
+   cf, ti, to = PAITestManager.GetNGroupsFor1CoreWithNParams(1, save_dir="./test")
+   ```
 5. `ReplaceCoreCoord`，替换单个或**一组**帧中的 `CORE_ADDR` 为指定坐标。
 
-    ```python
-    # Replaced core coordinate with (9, 9)
-    replaced = PAITestManager.ReplaceCoreCoord(original_frames, (9, 9))
-    ```
-
-    ⚠️ 一组指一组完整的配置帧，包含3帧。对于测试输入帧，即为单帧。
+   ```python
+   # Replaced core coordinate with (9, 9)
+   replaced = PAITestManager.ReplaceCoreCoord(original_frames, (9, 9))
+   ```
 
+   ⚠️ 一组指一组完整的配置帧，包含3帧。对于测试输入帧，即为单帧。
 6. `SaveFrames`，保存帧数据至 `.bin` 文件
 
-    ```python
-    # Save into ./test/config.bin
-    PAITestManager.SaveFrames("./test/config.bin", replaced)
-    ```
+   ```python
+   # Save into ./test/config.bin
+   PAITestManager.SaveFrames("./test/config.bin", replaced)
+   ```
 
 ## 🗓️ TODO
 
 - [ ] 上板验证
 - [ ] 参数检验
 - [ ] 配置/测试帧III/IV型
```

## Comparing `paitest-0.0.11.dist-info/RECORD` & `paitest-0.0.12.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 paitest/__init__.py,sha256=ZJN5Lf-VYbem3hDg45chGHznWqQvNQ4qYRHTIY4l_lI,40
 paitest/frames/__init__.py,sha256=xF0aeAVW27e8tCnJaxhR6MHM4qKYLZ0GSfhowLj0mUg,267
 paitest/frames/coord.py,sha256=Jg_YGEcclIFmmFtu5P1CKxaEocXPby6PXREJDI9gv8w,2581
 paitest/frames/coord.pyi,sha256=yogiWEB90vYATDc5SRPMmsVs_F0Ur4GwFM0Mx1hrEc8,805
-paitest/frames/frame.py,sha256=QYB5K-loa8jdSJV6cs8GsgYZ8W8Mb7u5Aoxv2ebVdjQ,14155
+paitest/frames/frame.py,sha256=uwXMi2T-PXRtg-SXoY9_yt8-20Ur5Oe8qyPBLkmkOPo,14188
 paitest/frames/frame_params.py,sha256=nlK23_RL1jZ3oyuCInuFLQ40x7KkKrCIOLgnMCmvzwE,4706
 paitest/log.py,sha256=0wn34g4m7nr837MwHNNsgZiNr9me-ywlGtfV4-iOTe4,230
-paitest/paitest.py,sha256=Oiykj26jCJ4FegzvSQKUDsAflQ4Z87kcMD3Q7DML3jE,17670
-paitest/paitest.pyi,sha256=9RJCwM51vVv9wS8YUOJFbD8oqu6fbqOEnaYLlD4wx0Y,2045
-paitest-0.0.11.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-paitest-0.0.11.dist-info/METADATA,sha256=YRG0sf6n3FovqRXMgyndn6don4ObQR-8iD2SPefLrKs,3379
-paitest-0.0.11.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-paitest-0.0.11.dist-info/RECORD,,
+paitest/paitest.py,sha256=L3H3ZXKwQA_SKriYQ5o1x8UxaBmz1vkunbnGgGtEZTU,18563
+paitest/paitest.pyi,sha256=ENTfqauMvGCjBU69gWo0H85oqDtUMA1JtQapwIezcoQ,1692
+paitest-0.0.12.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+paitest-0.0.12.dist-info/METADATA,sha256=gT8-iUdTWGXfWHeY3heiaLlcuCjmfqpVP646RBF7IY0,3451
+paitest-0.0.12.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+paitest-0.0.12.dist-info/RECORD,,
```

