# Comparing `tmp/ansys_materials_manager-0.2.0.tar.gz` & `tmp/ansys_materials_manager-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_materials_manager-0.2.0.tar", max compression
+gzip compressed data, was "ansys_materials_manager-0.2.1.tar", max compression
```

## Comparing `ansys_materials_manager-0.2.0.tar` & `ansys_materials_manager-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1089 2023-04-18 16:17:46.452172 ansys_materials_manager-0.2.0/LICENSE
--rw-r--r--   0        0        0     6343 2023-04-18 16:17:46.452172 ansys_materials_manager-0.2.0/README.rst
--rw-r--r--   0        0        0     2119 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      368 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/__init__.py
--rw-r--r--   0        0        0      512 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/__init__.py
--rw-r--r--   0        0        0     2111 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/_base.py
--rw-r--r--   0        0        0      480 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/_exceptions.py
--rw-r--r--   0        0        0      189 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/_packages.py
--rw-r--r--   0        0        0     3974 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/constant.py
--rw-r--r--   0        0        0     6199 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/piecewise_linear.py
--rw-r--r--   0        0        0     6052 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/polynomial.py
--rw-r--r--   0        0        0        0 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_fluent/__init__.py
--rw-r--r--   0        0        0     2981 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_fluent/ideal_gas.py
--rw-r--r--   0        0        0      334 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_fluent/simple_properties.py
--rw-r--r--   0        0        0        0 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_mapdl/__init__.py
--rw-r--r--   0        0        0    14912 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_mapdl/anisotropic_elasticity.py
--rw-r--r--   0        0        0     2033 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_mapdl/simple_properties.py
--rw-r--r--   0        0        0        0 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/py.typed
--rw-r--r--   0        0        0     2967 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/material.py
--rw-r--r--   0        0        0     3070 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/material_manager.py
--rw-r--r--   0        0        0     1495 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/serialize.py
--rw-r--r--   0        0        0        0 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/__init__.py
--rw-r--r--   0        0        0     2972 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/common.py
--rw-r--r--   0        0        0        0 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/mapdl/__init__.py
--rw-r--r--   0        0        0     1073 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/mapdl/mapdl_reader.py
--rw-r--r--   0        0        0     6565 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/mapdl/mpdata_parser.py
--rw-r--r--   0        0        0     3217 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/mapdl/tbdata_parser.py
--rw-r--r--   0        0        0      117 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/__init__.py
--rw-r--r--   0        0        0     9013 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_from_material.py
--rw-r--r--   0        0        0     7378 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_parser.py
--rw-r--r--   0        0        0     2993 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_property_map.py
--rw-r--r--   0        0        0     3081 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_to_material.py
--rw-r--r--   0        0        0     7963 1970-01-01 00:00:00.000000 ansys_materials_manager-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6343 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/README.rst
+-rw-r--r--   0        0        0     2119 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      368 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/__init__.py
+-rw-r--r--   0        0        0      512 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_common/__init__.py
+-rw-r--r--   0        0        0     2111 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_common/_base.py
+-rw-r--r--   0        0        0      480 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_common/_exceptions.py
+-rw-r--r--   0        0        0      189 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_common/_packages.py
+-rw-r--r--   0        0        0     3974 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_common/constant.py
+-rw-r--r--   0        0        0     6199 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_common/piecewise_linear.py
+-rw-r--r--   0        0        0     6052 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_common/polynomial.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_fluent/__init__.py
+-rw-r--r--   0        0        0     2981 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_fluent/ideal_gas.py
+-rw-r--r--   0        0        0      334 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_fluent/simple_properties.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_mapdl/__init__.py
+-rw-r--r--   0        0        0    14912 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_mapdl/anisotropic_elasticity.py
+-rw-r--r--   0        0        0     2033 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_mapdl/simple_properties.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/py.typed
+-rw-r--r--   0        0        0     2967 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/material.py
+-rw-r--r--   0        0        0     3070 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/material_manager.py
+-rw-r--r--   0        0        0     1495 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/serialize.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/__init__.py
+-rw-r--r--   0        0        0     2972 2023-04-19 14:05:41.546421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/common.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:05:41.550421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/mapdl/__init__.py
+-rw-r--r--   0        0        0     1073 2023-04-19 14:05:41.550421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/mapdl/mapdl_reader.py
+-rw-r--r--   0        0        0     6565 2023-04-19 14:05:41.550421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/mapdl/mpdata_parser.py
+-rw-r--r--   0        0        0     3217 2023-04-19 14:05:41.550421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/mapdl/tbdata_parser.py
+-rw-r--r--   0        0        0      117 2023-04-19 14:05:41.550421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/matml/__init__.py
+-rw-r--r--   0        0        0     9361 2023-04-19 14:05:41.550421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/matml/matml_from_material.py
+-rw-r--r--   0        0        0     7378 2023-04-19 14:05:41.550421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/matml/matml_parser.py
+-rw-r--r--   0        0        0     2993 2023-04-19 14:05:41.550421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/matml/matml_property_map.py
+-rw-r--r--   0        0        0     3081 2023-04-19 14:05:41.550421 ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/matml/matml_to_material.py
+-rw-r--r--   0        0        0     7963 1970-01-01 00:00:00.000000 ansys_materials_manager-0.2.1/PKG-INFO
```

### Comparing `ansys_materials_manager-0.2.0/LICENSE` & `ansys_materials_manager-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/README.rst` & `ansys_materials_manager-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/pyproject.toml` & `ansys_materials_manager-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-materials-manager"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python package to unify material management across the ansys portfolio"
 license = "MIT"
 authors = ["ANSYS, Inc. <ansys.support@ansys.com>"]
 maintainers = ["PyAnsys developers <pyansys.core@ansys.com>"]
 readme = "README.rst"
 repository = "https://github.com/pyansys/pymaterials-manager"
 documentation = "https://manager.materials.docs.pyansys.com"
```

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/__init__.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/_base.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_common/_base.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/constant.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_common/constant.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/piecewise_linear.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_common/piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/polynomial.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_common/polynomial.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_fluent/ideal_gas.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_fluent/ideal_gas.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_mapdl/anisotropic_elasticity.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_mapdl/anisotropic_elasticity.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_mapdl/simple_properties.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/_models/_mapdl/simple_properties.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/material.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/material.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/material_manager.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/material_manager.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/serialize.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/serialize.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/common.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/common.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/mapdl/mapdl_reader.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/mapdl/mapdl_reader.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/mapdl/mpdata_parser.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/mapdl/mpdata_parser.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/mapdl/tbdata_parser.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/mapdl/tbdata_parser.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_from_material.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/matml/matml_from_material.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 para_key = self._metadata_parameters[matml_key]
             else:
                 index = len(self._metadata_parameters) + 1
                 para_key = f"pa{index}"
                 self._metadata_parameters[matml_key] = para_key
 
             param_element = ET.SubElement(
-                property_element, "ParameterValue", {"parameter": para_key, "format": "float"}
+                property_element, "ParameterValue", {"format": "float", "parameter": para_key}
             )
             data_element = ET.SubElement(param_element, "Data")
             data_element.text = str(material.get_model_by_name(mat_key)[0].value)
             qualifier_element = ET.SubElement(param_element, "Qualifier", {"name": "Variable Type"})
             qualifier_element.text = "Dependent"
 
     def _add_property_set(
@@ -196,34 +196,40 @@
         buffer:
             buffer to write to
         **kwargs : bool, optional
             Optional keyword arguments.
             indent : bool, optional
                 Whether to add an indent to format the XML output(python 3.9+).
                 Defaults to ``false``.
+            xml_declaration: bool, optional
+                Whether to add the XML declaration to the output
         """
         tree = self._to_etree()
 
         if kwargs.get("indent", False):
             self._indent(tree)
-        buffer.write(ET.tostring(tree.getroot()))
+        buffer.write(
+            ET.tostring(tree.getroot(), xml_declaration=kwargs.get("xml_declaration", False))
+        )
 
     def export(self, path: _PATH_TYPE, **kwargs) -> None:
         """
         Write a Matml (engineering data xml format) representation of materials to file.
 
         Parameters
         ----------
         path:
             File path
         **kwargs : bool, optional
             Optional keyword arguments.
             indent : bool, optional
                 Whether to add an indent to format the XML output(python 3.9+).
                 Defaults to ``false``.
+            xml_declaration: bool, optional
+                Whether to add the XML declaration to the output
         """
         tree = self._to_etree()
 
         print(f"write xml to {path}")
         if kwargs.get("indent", False):
             self._indent(tree)
-        tree.write(path)
+        tree.write(path, xml_declaration=kwargs.get("xml_declaration", False))
```

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_parser.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/matml/matml_parser.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_property_map.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/matml/matml_property_map.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_to_material.py` & `ansys_materials_manager-0.2.1/src/ansys/materials/manager/util/matml/matml_to_material.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.0/PKG-INFO` & `ansys_materials_manager-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-materials-manager
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package to unify material management across the ansys portfolio
 Home-page: https://github.com/pyansys/pymaterials-manager
 License: MIT
 Author: ANSYS, Inc.
 Author-email: ansys.support@ansys.com
 Maintainer: PyAnsys developers
 Maintainer-email: pyansys.core@ansys.com
```

