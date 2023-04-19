# Comparing `tmp/TrimMCStruct-0.0.4.tar.gz` & `tmp/TrimMCStruct-0.0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrimMCStruct-0.0.4.tar", last modified: Sun Mar 26 11:49:20 2023, max compression
+gzip compressed data, was "TrimMCStruct-0.0.5.5.tar", last modified: Wed Apr 19 13:43:57 2023, max compression
```

## Comparing `TrimMCStruct-0.0.4.tar` & `TrimMCStruct-0.0.5.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 11:49:20.873045 TrimMCStruct-0.0.4/
--rw-rw-rw-   0        0        0     1277 2023-03-26 11:30:36.000000 TrimMCStruct-0.0.4/LICENSE(origin).md
--rw-rw-rw-   0        0        0    13293 2023-03-26 09:57:41.000000 TrimMCStruct-0.0.4/LICENSE.md
--rw-rw-rw-   0        0        0     5028 2023-03-26 11:49:20.871044 TrimMCStruct-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4022 2023-03-26 11:32:56.000000 TrimMCStruct-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-26 11:49:20.853045 TrimMCStruct-0.0.4/TrimMCStruct/
--rw-rw-rw-   0        0        0      201 2023-03-26 11:42:04.000000 TrimMCStruct-0.0.4/TrimMCStruct/__init__.py
--rw-rw-rw-   0        0        0    19854 2023-03-26 11:30:36.000000 TrimMCStruct-0.0.4/TrimMCStruct/main.py
-drwxrwxrwx   0        0        0        0 2023-03-26 11:49:20.868044 TrimMCStruct-0.0.4/TrimMCStruct.egg-info/
--rw-rw-rw-   0        0        0     5028 2023-03-26 11:49:20.000000 TrimMCStruct-0.0.4/TrimMCStruct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-03-26 11:49:20.000000 TrimMCStruct-0.0.4/TrimMCStruct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 11:49:20.000000 TrimMCStruct-0.0.4/TrimMCStruct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-03-26 11:49:20.000000 TrimMCStruct-0.0.4/TrimMCStruct.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-26 11:49:20.000000 TrimMCStruct-0.0.4/TrimMCStruct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-26 11:49:20.873045 TrimMCStruct-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1413 2023-03-26 11:49:15.000000 TrimMCStruct-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 13:43:57.486110 TrimMCStruct-0.0.5.5/
+-rw-rw-rw-   0        0        0     1277 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.5/LICENSE(origin).md
+-rw-rw-rw-   0        0        0    13331 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.5/LICENSE.md
+-rw-rw-rw-   0        0        0     5030 2023-04-19 13:43:57.485110 TrimMCStruct-0.0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4022 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 13:43:57.474103 TrimMCStruct-0.0.5.5/TrimMCStruct/
+-rw-rw-rw-   0        0        0      383 2023-04-19 13:40:40.000000 TrimMCStruct-0.0.5.5/TrimMCStruct/__init__.py
+-rw-rw-rw-   0        0        0    21644 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.5/TrimMCStruct/main.py
+drwxrwxrwx   0        0        0        0 2023-04-19 13:43:57.484103 TrimMCStruct-0.0.5.5/TrimMCStruct.egg-info/
+-rw-rw-rw-   0        0        0     5030 2023-04-19 13:43:57.000000 TrimMCStruct-0.0.5.5/TrimMCStruct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-04-19 13:43:57.000000 TrimMCStruct-0.0.5.5/TrimMCStruct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 13:43:57.000000 TrimMCStruct-0.0.5.5/TrimMCStruct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-19 13:43:57.000000 TrimMCStruct-0.0.5.5/TrimMCStruct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-19 13:43:57.000000 TrimMCStruct-0.0.5.5/TrimMCStruct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 13:43:57.486110 TrimMCStruct-0.0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1432 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.5/setup.py
```

### Comparing `TrimMCStruct-0.0.4/LICENSE(origin).md` & `TrimMCStruct-0.0.5.5/LICENSE(origin).md`

 * *Files identical despite different names*

### Comparing `TrimMCStruct-0.0.4/LICENSE.md` & `TrimMCStruct-0.0.5.5/LICENSE.md`

 * *Files 2% similar despite different names*

```diff
@@ -199,15 +199,15 @@
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
 
-   Copyright 2022 Team-Ryoun 金羿("Eilles Wan") & 诸葛亮与八卦阵("bgArray")
+   Copyright 2023 金羿("Eilles Wan") & 诸葛亮与八卦阵("bgArray") & The-phoenixR & Happy2018new("Eternal Crystal")
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `TrimMCStruct-0.0.4/PKG-INFO` & `TrimMCStruct-0.0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimMCStruct
-Version: 0.0.4
+Version: 0.0.5.5
 Summary: 读写操作《我的世界》.MCSTRUCTURE文件
 Home-page: https://github.com/TriM-Organization/TrimMCStruct
 Author: Eilles Wan, bgArray, phoenixr-codes(original author) 
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `TrimMCStruct-0.0.4/README.md` & `TrimMCStruct-0.0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `TrimMCStruct-0.0.4/TrimMCStruct/main.py` & `TrimMCStruct-0.0.5.5/TrimMCStruct/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from functools import partial
 from itertools import repeat
 import json
 from typing import Any, BinaryIO, Optional, Tuple, Union, Dict
 
 import numpy as np
 from numpy.typing import NDArray
-from pynbt import BaseTag, NBTFile, TAG_Compound, TAG_Int, TAG_List, TAG_String, TAG_Byte  # type: ignore
+from pynbt import BaseTag, NBTFile, TAG_Compound, TAG_Int, TAG_List, TAG_String, TAG_Byte, TAG_Long, TAG_Short  # type: ignore
 
 Coordinate = Tuple[int, int, int]
 
 # Compatibility versioning number for blocks in 1.19.
 COMPABILITY_VERSION: int = 17959425
 
 
@@ -126,20 +126,20 @@
 
     namespace: str
     base_name: str
     states: dict[str, Union[int, str, bool]]
     extra_data: dict[str, Union[int, str, bool]]
 
     def __init__(
-            self,
-            namespace: str,
-            base_name: str,
-            states: dict[str, Union[int, str, bool]] = {},
-            extra_data: dict[str, Union[int, str, bool]] = {},
-            compability_version: int = COMPABILITY_VERSION,
+        self,
+        namespace: str,
+        base_name: str,
+        states: dict[str, Union[int, str, bool]] = {},
+        extra_data: dict[str, Union[int, str, bool]] = {},
+        compability_version: int = COMPABILITY_VERSION,
     ):
         """
         Parameters
         ----------
         namespace
             The namespace of the block (e.g. "minecraft").
         base_name
@@ -159,18 +159,18 @@
         self.base_name = base_name
         self.states = states
         self.extra_data = extra_data
         self.compability_version = compability_version
 
     @classmethod
     def from_identifier(
-            cls,
-            identifier: str,
-            compability_version=COMPABILITY_VERSION,
-            **states: Union[int, str, bool],
+        cls,
+        identifier: str,
+        compability_version=COMPABILITY_VERSION,
+        **states: Union[int, str, bool],
     ):
         """
         Parameters
         ----------
         identifier
             The identifier of the block (e.g. "minecraft:wool").
 
@@ -197,50 +197,50 @@
     def __str__(self) -> str:
         return self.stringify()
 
     def __dict__(self) -> dict:
         return self.dictionarify()
 
     def add_states(
-            self,
-            states: dict[str, Union[int, str, bool]],
+        self,
+        states: dict[str, Union[int, str, bool]],
     ) -> None:
         self.states.update(states)
 
     def add_extra_data(
-            self,
-            extra_data: dict[str, Union[int, str, bool]],
+        self,
+        extra_data: dict[str, Union[int, str, bool]],
     ) -> None:
         self.extra_data.update(extra_data)
 
     def dictionarify(self, *, with_states: bool = True) -> Dict[str, Any]:
         result = {
             "name": self.identifier,
             "states": self.states if with_states else {},
             "version": self.compability_version,
         }
 
         return result
 
     def dictionarify_with_block_entity(
-            self, *, with_states: bool = True
+        self, *, with_states: bool = True
     ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         result = {
             "name": self.identifier,
             "states": self.states if with_states else {},
             "version": self.compability_version,
         }
 
         return result, self.extra_data
 
     def stringify(
-            self,
-            *,
-            with_namespace: bool = True,
-            with_states: bool = True,
+        self,
+        *,
+        with_namespace: bool = True,
+        with_states: bool = True,
     ) -> str:
         result = ""
         if with_namespace:
             result += self.namespace + ":"
         result += self.get_name()
         if with_states:
             result += f" [{json.dumps(self.states)[1:-1]}]"
@@ -273,14 +273,36 @@
     @property
     def identifier(self) -> str:
         """
         The identifier of the block.
         """
         return self.get_identifier()
 
+    def __eq__(self, obj: Block) -> bool:
+
+        if isinstance(obj, Block):
+            if self.dictionarify() == obj.dictionarify():
+                return True
+
+        return False
+
+    def copy(self) -> Block:
+        return Block(
+            namespace=self.namespace,
+            base_name=self.base_name,
+            states=self.states,
+            extra_data=self.extra_data,
+            compability_version=self.compability_version,
+        )
+
+    def clear_extra_data(self) -> Block:
+        another_self = self.copy()
+        another_self.extra_data = {}
+        return another_self
+
 
 class Structure:
     """
     Class representing a Minecraft structure that
     consists of blocks and entities.
 
     Attributes
@@ -288,18 +310,18 @@
     _size
         The size of the structure.
     """
 
     structure_indecis: NDArray[np.intc]
 
     def __init__(
-            self,
-            size: tuple[int, int, int],
-            fill: Optional[Block] = None,
-            compability_version: int = COMPABILITY_VERSION,
+        self,
+        size: tuple[int, int, int],
+        fill: Optional[Block] = None,
+        compability_version: int = COMPABILITY_VERSION,
     ):
         """
         Parameters
         ----------
         size
             The size of the structure.
 
@@ -308,19 +330,20 @@
             creation of a new structure object.
 
             If this is set to ``None`` the structure
             is filled with "Structure Void" blocks.
 
             "minecraft:air" is used as default.
         """
+
         self.structure_indecis: NDArray[np.intc]
 
         self._size = size
         self._palette: list[Block] = []
-        self._special_block_indices: list[int] = []
+        self._special_blocks: Dict[int, Dict] = {}
 
         if fill is None:
             self.structure_indecis = np.full(size, -1, dtype=np.intc)
 
         else:
             self.structure_indecis = np.zeros(size, dtype=np.intc)
             self._palette.append(fill)
@@ -362,33 +385,33 @@
                 for block in nbt["structure"]["palette"]["default"]["block_palette"]
             ]
         )
 
         for block_index, block_eneity_data in nbt["structure"]["palette"]["default"][
             "block_position_data"
         ].items():
-            struct._palette[int(block_index)].add_extra_data(
-                _into_pyobj(block_eneity_data)
-            )
-            struct._special_block_indices.append(int(block_index))
+            # struct._palette[int(block_index)].add_extra_data(
+            #     _into_pyobj(block_eneity_data)
+            # )
+            struct._special_blocks[int(block_index)] = _into_pyobj(block_eneity_data)
 
         return struct
 
     @property
     def size(self) -> tuple[int, int, int]:
         return self._size
 
     def __repr__(self) -> str:
         return repr(self._get_str_array())
 
     def __str__(self) -> str:
         return str(self._get_str_array())
 
     def _get_str_array(
-            self, *, with_namespace: bool = False, with_states: bool = False
+        self, *, with_namespace: bool = False, with_states: bool = False
     ) -> NDArray[Any]:
         """
         Returns a numpy array where each entry is a
         readable string of the corresponding block.
 
         Parameters
         ----------
@@ -420,38 +443,21 @@
         -------
         The position of the block in the palette. This is
         ``-1`` when ``None`` is used as ``block``.
         """
         if block is None:
             return -1
 
-        if block in self._palette:
-            return self._palette.index(block)
+        same_block = block.clear_extra_data()
+        if same_block in self._palette:
+            return self._palette.index(same_block)
 
-        self._palette.append(block)
+        self._palette.append(same_block)
         return len(self._palette) - 1
 
-    def get_structure(self) -> NDArray[Any]:
-        """
-        Returns the structure as a numpy array filled
-        with the corresponding `Block` objects.
-        """
-        arr = np.full(
-            self.structure_indecis.shape,
-            Block(
-                "minecraft",
-                "structure_void",
-                compability_version=self.compability_version,
-            ),
-            dtype=object,
-        )
-        for key, block in enumerate(self._palette):
-            arr[self.structure_indecis == key] = block
-        return arr
-
     def dump(self, file: BinaryIO) -> None:
         """
         Serialize the structure as a ``mcstructure``.
 
         Parameters
         ----------
         file
@@ -509,20 +515,18 @@
                                         ),
                                         block_position_data=TAG_Compound(
                                             dict(
                                                 [
                                                     (
                                                         str(block_index),
                                                         _into_tag(
-                                                            self._palette[
-                                                                block_index
-                                                            ].extra_data
+                                                            extra_data
                                                         ),
                                                     )
-                                                    for block_index in self._special_block_indices
+                                                    for block_index, extra_data in self._special_blocks.items()
                                                 ]
                                             )
                                         ),
                                     )
                                 )
                             )
                         ),
@@ -578,20 +582,50 @@
 
         Parameters
         ----------
         coordinate
             The coordinte of the block.
         """
         x, y, z = coordinate
-        return self._palette[self.structure_indecis[x, y, z]]
+        block = self._palette[self.structure_indecis[x, y, z]].copy()
+        block_index = x * self.size[2] * self.size[1] + y * self.size[2] + z
+        if block_index in self._special_blocks.keys():
+            block.add_extra_data(self._special_blocks[block_index])
+        return block
+
+    def get_structure(self) -> NDArray[Any]:
+        """
+        Returns the structure as a numpy array filled
+        with the corresponding `Block` objects.
+        """
+        arr = np.full(
+            self.structure_indecis.shape,
+            Block(
+                "minecraft",
+                "structure_void",
+                compability_version=self.compability_version,
+            ),
+            dtype=object,
+        )
+        for key, block in enumerate(self._palette):
+            arr[self.structure_indecis == key] = block
+
+        for index, exdata in self._special_blocks.items():
+            arr[int(index / (self.size[2] * self.size[1]))][
+                int(index % (self.size[2] * self.size[1]) / self.size[2])
+            ][
+                (index % (self.size[2] * self.size[1]) % self.size[2])
+            ].extra_data = exdata
+
+        return arr
 
     def set_block(
-            self,
-            coordinate: Coordinate,
-            block: Optional[Block],
+        self,
+        coordinate: Coordinate,
+        block: Optional[Block],
     ) -> Structure:
         """
         Puts a block into the structure.
 
         Parameters
         ----------
         coordinate
@@ -600,25 +634,27 @@
         block
             The block to place. If this is set to ``None``
             "Structure Void" blocks will be used.
         """
         x, y, z = coordinate
 
         ident = self._add_block_to_palette(block)
-        if block.extra_data:
-            self._special_block_indices.append(ident)
 
         self.structure_indecis[x, y, z] = ident
+        if block.extra_data:
+            self._special_blocks[
+                x * self.size[2] * self.size[1] + y * self.size[2] + z
+            ] = block.extra_data
         return self
 
     def fill_blocks(
-            self,
-            from_coordinate: Coordinate,
-            to_coordinate: Coordinate,
-            block: Block,
+        self,
+        from_coordinate: Coordinate,
+        to_coordinate: Coordinate,
+        block: Block,
     ) -> Structure:
         """
         Puts multiple blocks into the structure.
 
         Notes
         -----
         Both start and end points are filled.
@@ -635,21 +671,42 @@
             The block to place. If this is set to ``None``
             "STructure Void" blocks will be used to fill.
         """
         fx, fy, fz = from_coordinate
         tx, ty, tz = to_coordinate
 
         ident = self._add_block_to_palette(block)
-        if block.extra_data:
-            self._special_block_indices.append(ident)
+        
         # print([[[ident for k in range(abs(fz-tz)+1) ]for j in range(abs(fy-ty)+1)]for i in range(abs(fx-tx)+1)])
-        self.structure_indecis[fx: tx + 1, fy: ty + 1, fz: tz + 1] = np.array(
+        self.structure_indecis[fx : tx + 1, fy : ty + 1, fz : tz + 1] = np.array(
             [
                 [
                     [ident for k in range(abs(fz - tz) + 1)]
                     for j in range(abs(fy - ty) + 1)
                 ]
                 for i in range(abs(fx - tx) + 1)
             ],
             dtype=np.intc,
         ).reshape([abs(i) + 1 for i in (fx - tx, fy - ty, fz - tz)])
+
+        if block.extra_data:
+            self._special_blocks.update(
+                dict(
+                    zip(
+                        [
+                            (x * self.size[2] * self.size[1] + y * self.size[2] + z)
+                            for x in range(fx, tx)
+                            for y in range(fy, ty)
+                            for z in range(fz, tz)
+                        ],
+                        [
+                            block.extra_data
+                            for i in range(
+                                abs((fz - tz) + 1)
+                                * (abs(fy - ty) + 1)
+                                * (abs(fx - tx) + 1)
+                            )
+                        ],
+                    )
+                )
+            )
         return self
```

### Comparing `TrimMCStruct-0.0.4/TrimMCStruct.egg-info/PKG-INFO` & `TrimMCStruct-0.0.5.5/TrimMCStruct.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimMCStruct
-Version: 0.0.4
+Version: 0.0.5.5
 Summary: 读写操作《我的世界》.MCSTRUCTURE文件
 Home-page: https://github.com/TriM-Organization/TrimMCStruct
 Author: Eilles Wan, bgArray, phoenixr-codes(original author) 
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `TrimMCStruct-0.0.4/setup.py` & `TrimMCStruct-0.0.5.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,12 +27,9 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     # 需要安装的依赖
-    install_requires=[
-        "numpy>=1.21",
-        "pynbt>=2",
-    ],
+    install_requires=open("requirements.txt",'r',encoding='utf-8').read().strip().split("\n"),
 )
```

