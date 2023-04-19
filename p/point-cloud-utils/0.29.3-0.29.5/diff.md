# Comparing `tmp/point-cloud-utils-0.29.3.tar.gz` & `tmp/point-cloud-utils-0.29.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "point-cloud-utils-0.29.3.tar", last modified: Fri Apr 14 15:39:32 2023, max compression
+gzip compressed data, was "point-cloud-utils-0.29.5.tar", last modified: Wed Apr 19 13:31:43 2023, max compression
```

## Comparing `point-cloud-utils-0.29.3.tar` & `point-cloud-utils-0.29.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:39:32.645808 point-cloud-utils-0.29.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-04-14 15:39:15.000000 point-cloud-utils-0.29.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    34321 2023-04-14 15:39:32.641807 point-cloud-utils-0.29.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33838 2023-04-14 15:39:15.000000 point-cloud-utils-0.29.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:39:32.641807 point-cloud-utils-0.29.3/point_cloud_utils/
--rw-r--r--   0 runner    (1001) docker     (123)    20299 2023-04-14 15:39:16.000000 point-cloud-utils-0.29.3/point_cloud_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-04-14 15:39:16.000000 point-cloud-utils-0.29.3/point_cloud_utils/_mesh_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-14 15:39:16.000000 point-cloud-utils-0.29.3/point_cloud_utils/_octree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-04-14 15:39:16.000000 point-cloud-utils-0.29.3/point_cloud_utils/_pointcloud_normals.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-14 15:39:16.000000 point-cloud-utils-0.29.3/point_cloud_utils/_ray_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-14 15:39:16.000000 point-cloud-utils-0.29.3/point_cloud_utils/_ray_mesh_intersector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-04-14 15:39:16.000000 point-cloud-utils-0.29.3/point_cloud_utils/_ray_point_cloud_intersector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-14 15:39:16.000000 point-cloud-utils-0.29.3/point_cloud_utils/_sinkhorn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:39:32.641807 point-cloud-utils-0.29.3/point_cloud_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34321 2023-04-14 15:39:32.000000 point-cloud-utils-0.29.3/point_cloud_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-14 15:39:32.000000 point-cloud-utils-0.29.3/point_cloud_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:39:32.000000 point-cloud-utils-0.29.3/point_cloud_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:39:32.000000 point-cloud-utils-0.29.3/point_cloud_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 15:39:32.000000 point-cloud-utils-0.29.3/point_cloud_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 15:39:32.000000 point-cloud-utils-0.29.3/point_cloud_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 15:39:16.000000 point-cloud-utils-0.29.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:39:32.645808 point-cloud-utils-0.29.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-14 15:39:16.000000 point-cloud-utils-0.29.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:39:32.641807 point-cloud-utils-0.29.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    32170 2023-04-14 15:39:16.000000 point-cloud-utils-0.29.3/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:31:43.473127 point-cloud-utils-0.29.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-04-19 13:31:26.000000 point-cloud-utils-0.29.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36230 2023-04-19 13:31:43.469127 point-cloud-utils-0.29.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35746 2023-04-19 13:31:26.000000 point-cloud-utils-0.29.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:31:43.469127 point-cloud-utils-0.29.5/point_cloud_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/_mesh_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/_point_cloud_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/_pointcloud_normals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/_ray_mesh_intersector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/_ray_point_cloud_intersector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/_sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/_voxels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:31:43.469127 point-cloud-utils-0.29.5/point_cloud_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36230 2023-04-19 13:31:43.000000 point-cloud-utils-0.29.5/point_cloud_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 13:31:43.000000 point-cloud-utils-0.29.5/point_cloud_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:31:43.000000 point-cloud-utils-0.29.5/point_cloud_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:31:43.000000 point-cloud-utils-0.29.5/point_cloud_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 13:31:43.000000 point-cloud-utils-0.29.5/point_cloud_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 13:31:43.000000 point-cloud-utils-0.29.5/point_cloud_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:31:43.473127 point-cloud-utils-0.29.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:31:43.469127 point-cloud-utils-0.29.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    32125 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/tests/test_examples.py
```

### Comparing `point-cloud-utils-0.29.3/LICENSE` & `point-cloud-utils-0.29.5/LICENSE`

 * *Files identical despite different names*

### Comparing `point-cloud-utils-0.29.3/PKG-INFO` & `point-cloud-utils-0.29.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: point-cloud-utils
-Version: 0.29.3
+Version: 0.29.5
 Summary: A Python library for common tasks on 3D point clouds and meshes
 Home-page: https://github.com/fwilliams/point-cloud-utils
 Author: Francis Williams
 Author-email: francis@fwilliams.info
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -111,14 +111,17 @@
 - [Computing connected componentes](#computing-connected-components)
 - [Decimating a triangle mesh](#decimating-a-triangle-mesh)
 - [Making a mesh watertight](#making-a-mesh-watertight)
 - [Ray/Mesh intersection](#ray-mesh-intersection)
 - [Ray/Surfel intersection](#ray-surfel-intersection)
 - [Computing curvature on a mesh](#computing-curvature-on-a-mesh)
 - [Computing a consistent inside/outside for a triangle soup](#computing-a-consistent-inside-and-outside-for-a-triangle-soup)
+- [Voxelizing a triangle mesh](#voxelizing-a-triangle-mesh)
+- [Flood filling a dense grid](#flood-filling-a-dense-grid)
+- [Generating a mesh for a voxel grid](#generating-a-mesh-for-a-voxel-grid)
 
 
 ### Loading meshes and point clouds
 Point-Cloud-Utils supports reading many common mesh formats (PLY, STL, OFF, OBJ, 3DS, VRML 2.0, X3D, COLLADA).
 If it can be imported into MeshLab, we can read it! The type of file is inferred from its file extension.
 
 If you only need a few attributes of a point cloud or mesh, the quickest way to load a mesh is using one of
@@ -840,8 +843,51 @@
 # We're going to evaluate the inside/outside sign of 1000 points
 p = np.random.rand(1000, 3)
 
 # w has shape (1000,) where w[i] is the sign (positive for outside, negative for inside) of p[i]
 w = pcu.triangle_soup_fast_winding_number(v, f, p.astype(v.dtype))
 ```
 
+### Voxelizing a triangle mesh
+You can get a list of voxels which intersect a mesh as follows:
+```python
+import point_cloud_utils as pcu
+
+v, f = pcu.load_mesh_vf("mesh.ply")  # Load some mesh
+
+voxel_size = 1.0 / 128  # size of each voxel
+voxel_origin = [0., 0., 0.]  # Coordinate mapping to the bottom-left-back corner of the (0, 0, 0) voxel
+
+# [num_vox, 3] array of integer coordinates for each voxel intersecting the mesh
+ijk = pcu.voxelize_triangle_mesh(v, f, voxel_size, voxel_origin)
+```
+
+### Flood filling a dense grid
+If you have a 3D grid, you can flood fill it starting from a coordinate as follows:
+```python
+import point_cloud_utils as pcu
+
+# Grid of 0/1 values (but we also support floats/doubles/etc...)
+grid = (np.random.rand([128, 128, 128]) > 0.5).astype(np.int32)
+
+fill_value = 2  # Fill starting from [0, 0, 0] with the value 2
 
+pcu.flood_fill_3d(grid, [0, 0, 0], fill_value)
+```
+
+### Generating a mesh for a voxel grid
+Suppose you an array `ijk` of integer voxel coordinates. You may wish to plot the associated voxel grid.
+You can do this via the `voxel_grid_geometry` function as follows
+
+```python
+import point_cloud_utils as pcu
+
+voxel_size = 1.0 / 200.0 # Size of each voxel
+voxel_origin = [0.0, 0.0, 0.0]  # The position of the bottom-back-left corner of the (0, 0, 0) voxel
+
+gap_fraction = 0.01  # Generate an optional small gap between voxels which can look nice -- this is a fraction of the voxel size
+
+ijk = np.random.randint(-100, 100, size=(128, 3))  # Generate 128 random voxels in [-100, 100]^3
+
+# vox_v, vox_f are vertices/faces of mesh for voxel grid
+vox_v, vox_f = pcu.voxel_grid_geoemtry(ijk, v, gap_fraction=gap_fraction, voxel_size=voxel_size, voxel_origin=voxel_origin)
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: point-cloud-utils Version: 0.29.3 Summary: A Python
+Metadata-Version: 2.1 Name: point-cloud-utils Version: 0.29.5 Summary: A Python
 library for common tasks on 3D point clouds and meshes Home-page: https://
 github.com/fwilliams/point-cloud-utils Author: Francis Williams Author-email:
 francis@fwilliams.info Classifier: Programming Language :: C++ Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v3 (GPLv3) Description-Content-Type: text/markdown
 License-File: LICENSE ![Point Cloud Utils Logo](docs/docs/imgs/logo_crop.png) !
 [Point Cloud Utils Teaser](docs/docs/imgs/pcu_teaser_3.png)
@@ -69,33 +69,36 @@
 - [Calculating face areas of a mesh](#calculating-face-areas-of-a-mesh) -
 [Smoothing a mesh](#smoothing-a-mesh) - [Computing connected componentes]
 (#computing-connected-components) - [Decimating a triangle mesh](#decimating-a-
 triangle-mesh) - [Making a mesh watertight](#making-a-mesh-watertight) - [Ray/
 Mesh intersection](#ray-mesh-intersection) - [Ray/Surfel intersection](#ray-
 surfel-intersection) - [Computing curvature on a mesh](#computing-curvature-on-
 a-mesh) - [Computing a consistent inside/outside for a triangle soup]
-(#computing-a-consistent-inside-and-outside-for-a-triangle-soup) ### Loading
-meshes and point clouds Point-Cloud-Utils supports reading many common mesh
-formats (PLY, STL, OFF, OBJ, 3DS, VRML 2.0, X3D, COLLADA). If it can be
-imported into MeshLab, we can read it! The type of file is inferred from its
-file extension. If you only need a few attributes of a point cloud or mesh, the
-quickest way to load a mesh is using one of the `read_mesh_*` utility functions
-```python import point_cloud_utils as pcu # Load vertices and faces for a mesh
-v, f = pcu.load_mesh_vf("path/to/mesh") # Load vertices and per-vertex normals
-v, n = pcu.load_mesh_vn("path/to/mesh") # Load vertices, per-vertex normals,
-and per-vertex-colors v, n, c = pcu.load_mesh_vnc("path/to/mesh") # Load
-vertices, faces, and per-vertex normals v, f, n = pcu.load_mesh_vfn("path/to/
-mesh") # Load vertices, faces, per-vertex normals, and per-vertex colors v, f,
-n, c = pcu.load_mesh_vfnc("path/to/mesh") ``` For meshes and point clouds with
-more complex attributes, use `load_triangle_mesh` which returns a
-`TriangleMesh` object. ```python import point_cloud_utils as pcu # mesh is a
-lightweight TriangleMesh container object holding mesh vertices, faces, and
-their attributes. # Any attributes which aren't loaded (because they aren't
-present in the file) are set to None. # The data in TriangleMesh is layed out
-as follows (run help(pcu.TriangleMesh) for more details): # TriangleMesh: #
+(#computing-a-consistent-inside-and-outside-for-a-triangle-soup) - [Voxelizing
+a triangle mesh](#voxelizing-a-triangle-mesh) - [Flood filling a dense grid]
+(#flood-filling-a-dense-grid) - [Generating a mesh for a voxel grid]
+(#generating-a-mesh-for-a-voxel-grid) ### Loading meshes and point clouds
+Point-Cloud-Utils supports reading many common mesh formats (PLY, STL, OFF,
+OBJ, 3DS, VRML 2.0, X3D, COLLADA). If it can be imported into MeshLab, we can
+read it! The type of file is inferred from its file extension. If you only need
+a few attributes of a point cloud or mesh, the quickest way to load a mesh is
+using one of the `read_mesh_*` utility functions ```python import
+point_cloud_utils as pcu # Load vertices and faces for a mesh v, f =
+pcu.load_mesh_vf("path/to/mesh") # Load vertices and per-vertex normals v, n =
+pcu.load_mesh_vn("path/to/mesh") # Load vertices, per-vertex normals, and per-
+vertex-colors v, n, c = pcu.load_mesh_vnc("path/to/mesh") # Load vertices,
+faces, and per-vertex normals v, f, n = pcu.load_mesh_vfn("path/to/mesh") #
+Load vertices, faces, per-vertex normals, and per-vertex colors v, f, n, c =
+pcu.load_mesh_vfnc("path/to/mesh") ``` For meshes and point clouds with more
+complex attributes, use `load_triangle_mesh` which returns a `TriangleMesh`
+object. ```python import point_cloud_utils as pcu # mesh is a lightweight
+TriangleMesh container object holding mesh vertices, faces, and their
+attributes. # Any attributes which aren't loaded (because they aren't present
+in the file) are set to None. # The data in TriangleMesh is layed out as
+follows (run help(pcu.TriangleMesh) for more details): # TriangleMesh: #
 vertex_data: # positions: [V, 3]-shaped numpy array of per-vertex positions #
 normals: [V, 3]-shaped numpy array of per-vertex normals (or None) # texcoords:
 [V, 2]-shaped numpy array of per-vertex uv coordinates (or None) # tex_ids:
 [V,]-shaped numpy array of integer indices into TriangleMesh.textures
 indicating which texture to # use at this vertex (or None) # colors: [V, 4]-
 shaped numpy array of per-vertex RBGA colors in [0.0, 1.0] (or None) # radius:
 [V,]-shaped numpy array of per-vertex curvature radii (or None) # quality:
@@ -432,8 +435,31 @@
 (kg) curvatures using using a radius. # This method is much more robust but
 requires tuning the radius kh, kg = pcu.mesh_mean_and_gaussian_curvatures(v, f,
 r=0.1) ``` ### Computing a consistent inside and outside for a triangle soup
 ```python import point_cloud_utils as pcu import numpy as np v, f =
 pcu.load_mesh_vf("my_model.ply") # We're going to evaluate the inside/outside
 sign of 1000 points p = np.random.rand(1000, 3) # w has shape (1000,) where w
 [i] is the sign (positive for outside, negative for inside) of p[i] w =
-pcu.triangle_soup_fast_winding_number(v, f, p.astype(v.dtype)) ```
+pcu.triangle_soup_fast_winding_number(v, f, p.astype(v.dtype)) ``` ###
+Voxelizing a triangle mesh You can get a list of voxels which intersect a mesh
+as follows: ```python import point_cloud_utils as pcu v, f = pcu.load_mesh_vf
+("mesh.ply") # Load some mesh voxel_size = 1.0 / 128 # size of each voxel
+voxel_origin = [0., 0., 0.] # Coordinate mapping to the bottom-left-back corner
+of the (0, 0, 0) voxel # [num_vox, 3] array of integer coordinates for each
+voxel intersecting the mesh ijk = pcu.voxelize_triangle_mesh(v, f, voxel_size,
+voxel_origin) ``` ### Flood filling a dense grid If you have a 3D grid, you can
+flood fill it starting from a coordinate as follows: ```python import
+point_cloud_utils as pcu # Grid of 0/1 values (but we also support floats/
+doubles/etc...) grid = (np.random.rand([128, 128, 128]) > 0.5).astype(np.int32)
+fill_value = 2 # Fill starting from [0, 0, 0] with the value 2
+pcu.flood_fill_3d(grid, [0, 0, 0], fill_value) ``` ### Generating a mesh for a
+voxel grid Suppose you an array `ijk` of integer voxel coordinates. You may
+wish to plot the associated voxel grid. You can do this via the
+`voxel_grid_geometry` function as follows ```python import point_cloud_utils as
+pcu voxel_size = 1.0 / 200.0 # Size of each voxel voxel_origin = [0.0, 0.0,
+0.0] # The position of the bottom-back-left corner of the (0, 0, 0) voxel
+gap_fraction = 0.01 # Generate an optional small gap between voxels which can
+look nice -- this is a fraction of the voxel size ijk = np.random.randint(-100,
+100, size=(128, 3)) # Generate 128 random voxels in [-100, 100]^3 # vox_v,
+vox_f are vertices/faces of mesh for voxel grid vox_v, vox_f =
+pcu.voxel_grid_geoemtry(ijk, v, gap_fraction=gap_fraction,
+voxel_size=voxel_size, voxel_origin=voxel_origin) ```
```

### Comparing `point-cloud-utils-0.29.3/README.md` & `point-cloud-utils-0.29.5/point_cloud_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: point-cloud-utils
+Version: 0.29.5
+Summary: A Python library for common tasks on 3D point clouds and meshes
+Home-page: https://github.com/fwilliams/point-cloud-utils
+Author: Francis Williams
+Author-email: francis@fwilliams.info
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![Point Cloud Utils Logo](docs/docs/imgs/logo_crop.png)
 ![Point Cloud Utils Teaser](docs/docs/imgs/pcu_teaser_3.png)
 <!-- <h4 align="center"><i>A Python library for common tasks on 3D point clouds and meshes</i></h4> -->
 <h3 align="center"><b>Point Cloud Utils</b> is an <i>easy-to-use</i> Python library for processing and manipulating 3D point clouds and meshes. </h3>
 
 <h2 align="center"><a href="https://www.fwilliams.info/point-cloud-utils/"><u>Documentation</u></a></h2>
 
@@ -98,14 +111,17 @@
 - [Computing connected componentes](#computing-connected-components)
 - [Decimating a triangle mesh](#decimating-a-triangle-mesh)
 - [Making a mesh watertight](#making-a-mesh-watertight)
 - [Ray/Mesh intersection](#ray-mesh-intersection)
 - [Ray/Surfel intersection](#ray-surfel-intersection)
 - [Computing curvature on a mesh](#computing-curvature-on-a-mesh)
 - [Computing a consistent inside/outside for a triangle soup](#computing-a-consistent-inside-and-outside-for-a-triangle-soup)
+- [Voxelizing a triangle mesh](#voxelizing-a-triangle-mesh)
+- [Flood filling a dense grid](#flood-filling-a-dense-grid)
+- [Generating a mesh for a voxel grid](#generating-a-mesh-for-a-voxel-grid)
 
 
 ### Loading meshes and point clouds
 Point-Cloud-Utils supports reading many common mesh formats (PLY, STL, OFF, OBJ, 3DS, VRML 2.0, X3D, COLLADA).
 If it can be imported into MeshLab, we can read it! The type of file is inferred from its file extension.
 
 If you only need a few attributes of a point cloud or mesh, the quickest way to load a mesh is using one of
@@ -827,8 +843,51 @@
 # We're going to evaluate the inside/outside sign of 1000 points
 p = np.random.rand(1000, 3)
 
 # w has shape (1000,) where w[i] is the sign (positive for outside, negative for inside) of p[i]
 w = pcu.triangle_soup_fast_winding_number(v, f, p.astype(v.dtype))
 ```
 
+### Voxelizing a triangle mesh
+You can get a list of voxels which intersect a mesh as follows:
+```python
+import point_cloud_utils as pcu
+
+v, f = pcu.load_mesh_vf("mesh.ply")  # Load some mesh
+
+voxel_size = 1.0 / 128  # size of each voxel
+voxel_origin = [0., 0., 0.]  # Coordinate mapping to the bottom-left-back corner of the (0, 0, 0) voxel
+
+# [num_vox, 3] array of integer coordinates for each voxel intersecting the mesh
+ijk = pcu.voxelize_triangle_mesh(v, f, voxel_size, voxel_origin)
+```
+
+### Flood filling a dense grid
+If you have a 3D grid, you can flood fill it starting from a coordinate as follows:
+```python
+import point_cloud_utils as pcu
+
+# Grid of 0/1 values (but we also support floats/doubles/etc...)
+grid = (np.random.rand([128, 128, 128]) > 0.5).astype(np.int32)
+
+fill_value = 2  # Fill starting from [0, 0, 0] with the value 2
+
+pcu.flood_fill_3d(grid, [0, 0, 0], fill_value)
+```
+
+### Generating a mesh for a voxel grid
+Suppose you an array `ijk` of integer voxel coordinates. You may wish to plot the associated voxel grid.
+You can do this via the `voxel_grid_geometry` function as follows
 
+```python
+import point_cloud_utils as pcu
+
+voxel_size = 1.0 / 200.0 # Size of each voxel
+voxel_origin = [0.0, 0.0, 0.0]  # The position of the bottom-back-left corner of the (0, 0, 0) voxel
+
+gap_fraction = 0.01  # Generate an optional small gap between voxels which can look nice -- this is a fraction of the voxel size
+
+ijk = np.random.randint(-100, 100, size=(128, 3))  # Generate 128 random voxels in [-100, 100]^3
+
+# vox_v, vox_f are vertices/faces of mesh for voxel grid
+vox_v, vox_f = pcu.voxel_grid_geoemtry(ijk, v, gap_fraction=gap_fraction, voxel_size=voxel_size, voxel_origin=voxel_origin)
+```
```

#### html2text {}

```diff
@@ -1,9 +1,15 @@
-![Point Cloud Utils Logo](docs/docs/imgs/logo_crop.png) ![Point Cloud Utils
-Teaser](docs/docs/imgs/pcu_teaser_3.png)
+Metadata-Version: 2.1 Name: point-cloud-utils Version: 0.29.5 Summary: A Python
+library for common tasks on 3D point clouds and meshes Home-page: https://
+github.com/fwilliams/point-cloud-utils Author: Francis Williams Author-email:
+francis@fwilliams.info Classifier: Programming Language :: C++ Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
+General Public License v3 (GPLv3) Description-Content-Type: text/markdown
+License-File: LICENSE ![Point Cloud Utils Logo](docs/docs/imgs/logo_crop.png) !
+[Point Cloud Utils Teaser](docs/docs/imgs/pcu_teaser_3.png)
   **** Point Cloud Utils is an easy-to-use Python library for processing and
                  manipulating 3D point clouds and meshes. ****
                            ***** Documentation *****
 -------------------------- ![build workflow](https://github.com/fwilliams/
 point-cloud-utils/actions/workflows/build-wheels-and-publish-to-pipy.yml/
 badge.svg) Author: [Francis Williams](https://www.fwilliams.info) If Point
 Cloud Utils contributes to an academic publication, cite it as: ``` @misc
@@ -63,33 +69,36 @@
 - [Calculating face areas of a mesh](#calculating-face-areas-of-a-mesh) -
 [Smoothing a mesh](#smoothing-a-mesh) - [Computing connected componentes]
 (#computing-connected-components) - [Decimating a triangle mesh](#decimating-a-
 triangle-mesh) - [Making a mesh watertight](#making-a-mesh-watertight) - [Ray/
 Mesh intersection](#ray-mesh-intersection) - [Ray/Surfel intersection](#ray-
 surfel-intersection) - [Computing curvature on a mesh](#computing-curvature-on-
 a-mesh) - [Computing a consistent inside/outside for a triangle soup]
-(#computing-a-consistent-inside-and-outside-for-a-triangle-soup) ### Loading
-meshes and point clouds Point-Cloud-Utils supports reading many common mesh
-formats (PLY, STL, OFF, OBJ, 3DS, VRML 2.0, X3D, COLLADA). If it can be
-imported into MeshLab, we can read it! The type of file is inferred from its
-file extension. If you only need a few attributes of a point cloud or mesh, the
-quickest way to load a mesh is using one of the `read_mesh_*` utility functions
-```python import point_cloud_utils as pcu # Load vertices and faces for a mesh
-v, f = pcu.load_mesh_vf("path/to/mesh") # Load vertices and per-vertex normals
-v, n = pcu.load_mesh_vn("path/to/mesh") # Load vertices, per-vertex normals,
-and per-vertex-colors v, n, c = pcu.load_mesh_vnc("path/to/mesh") # Load
-vertices, faces, and per-vertex normals v, f, n = pcu.load_mesh_vfn("path/to/
-mesh") # Load vertices, faces, per-vertex normals, and per-vertex colors v, f,
-n, c = pcu.load_mesh_vfnc("path/to/mesh") ``` For meshes and point clouds with
-more complex attributes, use `load_triangle_mesh` which returns a
-`TriangleMesh` object. ```python import point_cloud_utils as pcu # mesh is a
-lightweight TriangleMesh container object holding mesh vertices, faces, and
-their attributes. # Any attributes which aren't loaded (because they aren't
-present in the file) are set to None. # The data in TriangleMesh is layed out
-as follows (run help(pcu.TriangleMesh) for more details): # TriangleMesh: #
+(#computing-a-consistent-inside-and-outside-for-a-triangle-soup) - [Voxelizing
+a triangle mesh](#voxelizing-a-triangle-mesh) - [Flood filling a dense grid]
+(#flood-filling-a-dense-grid) - [Generating a mesh for a voxel grid]
+(#generating-a-mesh-for-a-voxel-grid) ### Loading meshes and point clouds
+Point-Cloud-Utils supports reading many common mesh formats (PLY, STL, OFF,
+OBJ, 3DS, VRML 2.0, X3D, COLLADA). If it can be imported into MeshLab, we can
+read it! The type of file is inferred from its file extension. If you only need
+a few attributes of a point cloud or mesh, the quickest way to load a mesh is
+using one of the `read_mesh_*` utility functions ```python import
+point_cloud_utils as pcu # Load vertices and faces for a mesh v, f =
+pcu.load_mesh_vf("path/to/mesh") # Load vertices and per-vertex normals v, n =
+pcu.load_mesh_vn("path/to/mesh") # Load vertices, per-vertex normals, and per-
+vertex-colors v, n, c = pcu.load_mesh_vnc("path/to/mesh") # Load vertices,
+faces, and per-vertex normals v, f, n = pcu.load_mesh_vfn("path/to/mesh") #
+Load vertices, faces, per-vertex normals, and per-vertex colors v, f, n, c =
+pcu.load_mesh_vfnc("path/to/mesh") ``` For meshes and point clouds with more
+complex attributes, use `load_triangle_mesh` which returns a `TriangleMesh`
+object. ```python import point_cloud_utils as pcu # mesh is a lightweight
+TriangleMesh container object holding mesh vertices, faces, and their
+attributes. # Any attributes which aren't loaded (because they aren't present
+in the file) are set to None. # The data in TriangleMesh is layed out as
+follows (run help(pcu.TriangleMesh) for more details): # TriangleMesh: #
 vertex_data: # positions: [V, 3]-shaped numpy array of per-vertex positions #
 normals: [V, 3]-shaped numpy array of per-vertex normals (or None) # texcoords:
 [V, 2]-shaped numpy array of per-vertex uv coordinates (or None) # tex_ids:
 [V,]-shaped numpy array of integer indices into TriangleMesh.textures
 indicating which texture to # use at this vertex (or None) # colors: [V, 4]-
 shaped numpy array of per-vertex RBGA colors in [0.0, 1.0] (or None) # radius:
 [V,]-shaped numpy array of per-vertex curvature radii (or None) # quality:
@@ -426,8 +435,31 @@
 (kg) curvatures using using a radius. # This method is much more robust but
 requires tuning the radius kh, kg = pcu.mesh_mean_and_gaussian_curvatures(v, f,
 r=0.1) ``` ### Computing a consistent inside and outside for a triangle soup
 ```python import point_cloud_utils as pcu import numpy as np v, f =
 pcu.load_mesh_vf("my_model.ply") # We're going to evaluate the inside/outside
 sign of 1000 points p = np.random.rand(1000, 3) # w has shape (1000,) where w
 [i] is the sign (positive for outside, negative for inside) of p[i] w =
-pcu.triangle_soup_fast_winding_number(v, f, p.astype(v.dtype)) ```
+pcu.triangle_soup_fast_winding_number(v, f, p.astype(v.dtype)) ``` ###
+Voxelizing a triangle mesh You can get a list of voxels which intersect a mesh
+as follows: ```python import point_cloud_utils as pcu v, f = pcu.load_mesh_vf
+("mesh.ply") # Load some mesh voxel_size = 1.0 / 128 # size of each voxel
+voxel_origin = [0., 0., 0.] # Coordinate mapping to the bottom-left-back corner
+of the (0, 0, 0) voxel # [num_vox, 3] array of integer coordinates for each
+voxel intersecting the mesh ijk = pcu.voxelize_triangle_mesh(v, f, voxel_size,
+voxel_origin) ``` ### Flood filling a dense grid If you have a 3D grid, you can
+flood fill it starting from a coordinate as follows: ```python import
+point_cloud_utils as pcu # Grid of 0/1 values (but we also support floats/
+doubles/etc...) grid = (np.random.rand([128, 128, 128]) > 0.5).astype(np.int32)
+fill_value = 2 # Fill starting from [0, 0, 0] with the value 2
+pcu.flood_fill_3d(grid, [0, 0, 0], fill_value) ``` ### Generating a mesh for a
+voxel grid Suppose you an array `ijk` of integer voxel coordinates. You may
+wish to plot the associated voxel grid. You can do this via the
+`voxel_grid_geometry` function as follows ```python import point_cloud_utils as
+pcu voxel_size = 1.0 / 200.0 # Size of each voxel voxel_origin = [0.0, 0.0,
+0.0] # The position of the bottom-back-left corner of the (0, 0, 0) voxel
+gap_fraction = 0.01 # Generate an optional small gap between voxels which can
+look nice -- this is a fraction of the voxel size ijk = np.random.randint(-100,
+100, size=(128, 3)) # Generate 128 random voxels in [-100, 100]^3 # vox_v,
+vox_f are vertices/faces of mesh for voxel grid vox_v, vox_f =
+pcu.voxel_grid_geoemtry(ijk, v, gap_fraction=gap_fraction,
+voxel_size=voxel_size, voxel_origin=voxel_origin) ```
```

### Comparing `point-cloud-utils-0.29.3/point_cloud_utils/_mesh_io.py` & `point-cloud-utils-0.29.5/point_cloud_utils/_mesh_io.py`

 * *Files identical despite different names*

### Comparing `point-cloud-utils-0.29.3/point_cloud_utils/_pointcloud_normals.py` & `point-cloud-utils-0.29.5/point_cloud_utils/_pointcloud_normals.py`

 * *Files identical despite different names*

### Comparing `point-cloud-utils-0.29.3/point_cloud_utils/_ray_mesh_intersector.py` & `point-cloud-utils-0.29.5/point_cloud_utils/_ray_mesh_intersector.py`

 * *Files identical despite different names*

### Comparing `point-cloud-utils-0.29.3/point_cloud_utils/_ray_point_cloud_intersector.py` & `point-cloud-utils-0.29.5/point_cloud_utils/_ray_point_cloud_intersector.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,20 @@
 import numpy as np
 
-
-def _validate_point_radius_internal(p, r):
-    if not isinstance(r, np.ndarray):
-        if np.isscalar(r):
-            r = r * np.ones(p.shape[0])
-        elif isinstance(r, list) or isinstance(r, tuple):
-            r = np.array(r).astype(p.dtype)
-        else:
-            raise ValueError("Argument r must be a scalar or numpy array with the same number of rows as p")
-
-    if r.shape[0] != p.shape[0]:
-        raise ValueError("Argument r have the same number of rows as p")
-
-    if len(r.shape) != 1:
-        r = np.squeeze(r)
-
-    if len(r.shape) != 1:
-        raise ValueError("Invalid shape for argument r, must have shape (N,) or (N, 1)")
-
-    return r
-
-
-def surfel_geometry(p, n, r=0.1, subdivs=7):
-    """
-    Generate geometry for a point cloud encoded as surfels (i.e. circular patches centered at each point and oriented
-    perpendicularly to each normal)
-
-    Args:
-        p : \#p by 3 array of vertex positions (each row is a vertex)
-        n : \#p by 3 array of vertex normals (each row is a vertex)
-        r : Array or Scalar describing the size of each geometry element (Either one radius per vertex, or a global size for the whole point cloud)
-        subdivs : Number of times to subdivide the patch geometry for each point (i.e. # tris per cicle)
-
-    Returns:
-        verts : an array of shape (#output_vertices, 3)
-        faces : an array of shape (#output_faces, 3) indexing into verts
-
-    """
-    from ._pcu_internal import point_cloud_splatting_geometry_internal_
-    r = _validate_point_radius_internal(p, r)
-    return point_cloud_splatting_geometry_internal_(p, n, "circle", r.astype(p.dtype), subdivs)
+from ._point_cloud_geometry import _validate_point_radius_internal
 
 
 def ray_surfel_intersection(p, n, ray_o, ray_d, r=0.1, subdivs=4, ray_near=0.0, ray_far=np.inf):
     """
     Compute intersection between a set of rays and a point cloud converted to surfels (i.e. circular patches oriented
     with the point normals)
 
     Args:
-        p : \#p by 3 array of vertex positions (each row is a vertex)
-        n : \#p by 3 Matrix of vertex normals (each row is a vertex)
+        p : \\#p by 3 array of vertex positions (each row is a vertex)
+        n : \\#p by 3 Matrix of vertex normals (each row is a vertex)
         ray_o : array of shape (#rays, 3) of ray origins (one per row) or a single array of shape (3,) to use
         ray_d : array of shape (#rays, 3) of ray directions (one per row)
         r : Array or Scalar describing the size of each geometry element (Either one radius per vertex, or a global size for the whole point cloud)
         subdivs : Number of times to subdivide the patch geometry for each point (i.e. # tris per cicle)
         ray_near : an optional floating point value indicating the distance along each ray to start searching (default 0.0)
         ray_far : an optional floating point value indicating the maximum distance along each ray to search (default inf)
 
@@ -74,16 +34,16 @@
     """
     def __init__(self, p, n, r=0.1, subdivs=7):
         """
         Construct a RayPointCloudIntersector which can be used to compute the intersection between a set of rays and a
         point cloud converted to circular patches oriented with the point normals
 
         Args:
-            p : \#p by 3 array of vertex positions (each row is a vertex)
-            n : \#p by 3 Matrix of vertex normals (each row is a vertex)
+            p : \\#p by 3 array of vertex positions (each row is a vertex)
+            n : \\#p by 3 Matrix of vertex normals (each row is a vertex)
             r : Array or Scalar describing the size of each geometry element (Either one radius per vertex, or a global size for the whole point cloud)
             subdivs : Number of times to subdivide the patch geometry for each point (i.e. # tris per cicle)
         """
         from ._pcu_internal import _RayMeshIntersectorInternal, _populate_ray_point_cloud_intersector_internal
         r = _validate_point_radius_internal(p, r)
 
         self.p = p
```

### Comparing `point-cloud-utils-0.29.3/point_cloud_utils/_sinkhorn.py` & `point-cloud-utils-0.29.5/point_cloud_utils/_sinkhorn.py`

 * *Files identical despite different names*

### Comparing `point-cloud-utils-0.29.3/point_cloud_utils.egg-info/PKG-INFO` & `point-cloud-utils-0.29.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: point-cloud-utils
-Version: 0.29.3
-Summary: A Python library for common tasks on 3D point clouds and meshes
-Home-page: https://github.com/fwilliams/point-cloud-utils
-Author: Francis Williams
-Author-email: francis@fwilliams.info
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![Point Cloud Utils Logo](docs/docs/imgs/logo_crop.png)
 ![Point Cloud Utils Teaser](docs/docs/imgs/pcu_teaser_3.png)
 <!-- <h4 align="center"><i>A Python library for common tasks on 3D point clouds and meshes</i></h4> -->
 <h3 align="center"><b>Point Cloud Utils</b> is an <i>easy-to-use</i> Python library for processing and manipulating 3D point clouds and meshes. </h3>
 
 <h2 align="center"><a href="https://www.fwilliams.info/point-cloud-utils/"><u>Documentation</u></a></h2>
 
@@ -111,14 +98,17 @@
 - [Computing connected componentes](#computing-connected-components)
 - [Decimating a triangle mesh](#decimating-a-triangle-mesh)
 - [Making a mesh watertight](#making-a-mesh-watertight)
 - [Ray/Mesh intersection](#ray-mesh-intersection)
 - [Ray/Surfel intersection](#ray-surfel-intersection)
 - [Computing curvature on a mesh](#computing-curvature-on-a-mesh)
 - [Computing a consistent inside/outside for a triangle soup](#computing-a-consistent-inside-and-outside-for-a-triangle-soup)
+- [Voxelizing a triangle mesh](#voxelizing-a-triangle-mesh)
+- [Flood filling a dense grid](#flood-filling-a-dense-grid)
+- [Generating a mesh for a voxel grid](#generating-a-mesh-for-a-voxel-grid)
 
 
 ### Loading meshes and point clouds
 Point-Cloud-Utils supports reading many common mesh formats (PLY, STL, OFF, OBJ, 3DS, VRML 2.0, X3D, COLLADA).
 If it can be imported into MeshLab, we can read it! The type of file is inferred from its file extension.
 
 If you only need a few attributes of a point cloud or mesh, the quickest way to load a mesh is using one of
@@ -840,8 +830,51 @@
 # We're going to evaluate the inside/outside sign of 1000 points
 p = np.random.rand(1000, 3)
 
 # w has shape (1000,) where w[i] is the sign (positive for outside, negative for inside) of p[i]
 w = pcu.triangle_soup_fast_winding_number(v, f, p.astype(v.dtype))
 ```
 
+### Voxelizing a triangle mesh
+You can get a list of voxels which intersect a mesh as follows:
+```python
+import point_cloud_utils as pcu
+
+v, f = pcu.load_mesh_vf("mesh.ply")  # Load some mesh
+
+voxel_size = 1.0 / 128  # size of each voxel
+voxel_origin = [0., 0., 0.]  # Coordinate mapping to the bottom-left-back corner of the (0, 0, 0) voxel
+
+# [num_vox, 3] array of integer coordinates for each voxel intersecting the mesh
+ijk = pcu.voxelize_triangle_mesh(v, f, voxel_size, voxel_origin)
+```
+
+### Flood filling a dense grid
+If you have a 3D grid, you can flood fill it starting from a coordinate as follows:
+```python
+import point_cloud_utils as pcu
+
+# Grid of 0/1 values (but we also support floats/doubles/etc...)
+grid = (np.random.rand([128, 128, 128]) > 0.5).astype(np.int32)
+
+fill_value = 2  # Fill starting from [0, 0, 0] with the value 2
+
+pcu.flood_fill_3d(grid, [0, 0, 0], fill_value)
+```
+
+### Generating a mesh for a voxel grid
+Suppose you an array `ijk` of integer voxel coordinates. You may wish to plot the associated voxel grid.
+You can do this via the `voxel_grid_geometry` function as follows
+
+```python
+import point_cloud_utils as pcu
+
+voxel_size = 1.0 / 200.0 # Size of each voxel
+voxel_origin = [0.0, 0.0, 0.0]  # The position of the bottom-back-left corner of the (0, 0, 0) voxel
+
+gap_fraction = 0.01  # Generate an optional small gap between voxels which can look nice -- this is a fraction of the voxel size
+
+ijk = np.random.randint(-100, 100, size=(128, 3))  # Generate 128 random voxels in [-100, 100]^3
 
+# vox_v, vox_f are vertices/faces of mesh for voxel grid
+vox_v, vox_f = pcu.voxel_grid_geoemtry(ijk, v, gap_fraction=gap_fraction, voxel_size=voxel_size, voxel_origin=voxel_origin)
+```
```

#### html2text {}

```diff
@@ -1,15 +1,9 @@
-Metadata-Version: 2.1 Name: point-cloud-utils Version: 0.29.3 Summary: A Python
-library for common tasks on 3D point clouds and meshes Home-page: https://
-github.com/fwilliams/point-cloud-utils Author: Francis Williams Author-email:
-francis@fwilliams.info Classifier: Programming Language :: C++ Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
-General Public License v3 (GPLv3) Description-Content-Type: text/markdown
-License-File: LICENSE ![Point Cloud Utils Logo](docs/docs/imgs/logo_crop.png) !
-[Point Cloud Utils Teaser](docs/docs/imgs/pcu_teaser_3.png)
+![Point Cloud Utils Logo](docs/docs/imgs/logo_crop.png) ![Point Cloud Utils
+Teaser](docs/docs/imgs/pcu_teaser_3.png)
   **** Point Cloud Utils is an easy-to-use Python library for processing and
                  manipulating 3D point clouds and meshes. ****
                            ***** Documentation *****
 -------------------------- ![build workflow](https://github.com/fwilliams/
 point-cloud-utils/actions/workflows/build-wheels-and-publish-to-pipy.yml/
 badge.svg) Author: [Francis Williams](https://www.fwilliams.info) If Point
 Cloud Utils contributes to an academic publication, cite it as: ``` @misc
@@ -69,33 +63,36 @@
 - [Calculating face areas of a mesh](#calculating-face-areas-of-a-mesh) -
 [Smoothing a mesh](#smoothing-a-mesh) - [Computing connected componentes]
 (#computing-connected-components) - [Decimating a triangle mesh](#decimating-a-
 triangle-mesh) - [Making a mesh watertight](#making-a-mesh-watertight) - [Ray/
 Mesh intersection](#ray-mesh-intersection) - [Ray/Surfel intersection](#ray-
 surfel-intersection) - [Computing curvature on a mesh](#computing-curvature-on-
 a-mesh) - [Computing a consistent inside/outside for a triangle soup]
-(#computing-a-consistent-inside-and-outside-for-a-triangle-soup) ### Loading
-meshes and point clouds Point-Cloud-Utils supports reading many common mesh
-formats (PLY, STL, OFF, OBJ, 3DS, VRML 2.0, X3D, COLLADA). If it can be
-imported into MeshLab, we can read it! The type of file is inferred from its
-file extension. If you only need a few attributes of a point cloud or mesh, the
-quickest way to load a mesh is using one of the `read_mesh_*` utility functions
-```python import point_cloud_utils as pcu # Load vertices and faces for a mesh
-v, f = pcu.load_mesh_vf("path/to/mesh") # Load vertices and per-vertex normals
-v, n = pcu.load_mesh_vn("path/to/mesh") # Load vertices, per-vertex normals,
-and per-vertex-colors v, n, c = pcu.load_mesh_vnc("path/to/mesh") # Load
-vertices, faces, and per-vertex normals v, f, n = pcu.load_mesh_vfn("path/to/
-mesh") # Load vertices, faces, per-vertex normals, and per-vertex colors v, f,
-n, c = pcu.load_mesh_vfnc("path/to/mesh") ``` For meshes and point clouds with
-more complex attributes, use `load_triangle_mesh` which returns a
-`TriangleMesh` object. ```python import point_cloud_utils as pcu # mesh is a
-lightweight TriangleMesh container object holding mesh vertices, faces, and
-their attributes. # Any attributes which aren't loaded (because they aren't
-present in the file) are set to None. # The data in TriangleMesh is layed out
-as follows (run help(pcu.TriangleMesh) for more details): # TriangleMesh: #
+(#computing-a-consistent-inside-and-outside-for-a-triangle-soup) - [Voxelizing
+a triangle mesh](#voxelizing-a-triangle-mesh) - [Flood filling a dense grid]
+(#flood-filling-a-dense-grid) - [Generating a mesh for a voxel grid]
+(#generating-a-mesh-for-a-voxel-grid) ### Loading meshes and point clouds
+Point-Cloud-Utils supports reading many common mesh formats (PLY, STL, OFF,
+OBJ, 3DS, VRML 2.0, X3D, COLLADA). If it can be imported into MeshLab, we can
+read it! The type of file is inferred from its file extension. If you only need
+a few attributes of a point cloud or mesh, the quickest way to load a mesh is
+using one of the `read_mesh_*` utility functions ```python import
+point_cloud_utils as pcu # Load vertices and faces for a mesh v, f =
+pcu.load_mesh_vf("path/to/mesh") # Load vertices and per-vertex normals v, n =
+pcu.load_mesh_vn("path/to/mesh") # Load vertices, per-vertex normals, and per-
+vertex-colors v, n, c = pcu.load_mesh_vnc("path/to/mesh") # Load vertices,
+faces, and per-vertex normals v, f, n = pcu.load_mesh_vfn("path/to/mesh") #
+Load vertices, faces, per-vertex normals, and per-vertex colors v, f, n, c =
+pcu.load_mesh_vfnc("path/to/mesh") ``` For meshes and point clouds with more
+complex attributes, use `load_triangle_mesh` which returns a `TriangleMesh`
+object. ```python import point_cloud_utils as pcu # mesh is a lightweight
+TriangleMesh container object holding mesh vertices, faces, and their
+attributes. # Any attributes which aren't loaded (because they aren't present
+in the file) are set to None. # The data in TriangleMesh is layed out as
+follows (run help(pcu.TriangleMesh) for more details): # TriangleMesh: #
 vertex_data: # positions: [V, 3]-shaped numpy array of per-vertex positions #
 normals: [V, 3]-shaped numpy array of per-vertex normals (or None) # texcoords:
 [V, 2]-shaped numpy array of per-vertex uv coordinates (or None) # tex_ids:
 [V,]-shaped numpy array of integer indices into TriangleMesh.textures
 indicating which texture to # use at this vertex (or None) # colors: [V, 4]-
 shaped numpy array of per-vertex RBGA colors in [0.0, 1.0] (or None) # radius:
 [V,]-shaped numpy array of per-vertex curvature radii (or None) # quality:
@@ -432,8 +429,31 @@
 (kg) curvatures using using a radius. # This method is much more robust but
 requires tuning the radius kh, kg = pcu.mesh_mean_and_gaussian_curvatures(v, f,
 r=0.1) ``` ### Computing a consistent inside and outside for a triangle soup
 ```python import point_cloud_utils as pcu import numpy as np v, f =
 pcu.load_mesh_vf("my_model.ply") # We're going to evaluate the inside/outside
 sign of 1000 points p = np.random.rand(1000, 3) # w has shape (1000,) where w
 [i] is the sign (positive for outside, negative for inside) of p[i] w =
-pcu.triangle_soup_fast_winding_number(v, f, p.astype(v.dtype)) ```
+pcu.triangle_soup_fast_winding_number(v, f, p.astype(v.dtype)) ``` ###
+Voxelizing a triangle mesh You can get a list of voxels which intersect a mesh
+as follows: ```python import point_cloud_utils as pcu v, f = pcu.load_mesh_vf
+("mesh.ply") # Load some mesh voxel_size = 1.0 / 128 # size of each voxel
+voxel_origin = [0., 0., 0.] # Coordinate mapping to the bottom-left-back corner
+of the (0, 0, 0) voxel # [num_vox, 3] array of integer coordinates for each
+voxel intersecting the mesh ijk = pcu.voxelize_triangle_mesh(v, f, voxel_size,
+voxel_origin) ``` ### Flood filling a dense grid If you have a 3D grid, you can
+flood fill it starting from a coordinate as follows: ```python import
+point_cloud_utils as pcu # Grid of 0/1 values (but we also support floats/
+doubles/etc...) grid = (np.random.rand([128, 128, 128]) > 0.5).astype(np.int32)
+fill_value = 2 # Fill starting from [0, 0, 0] with the value 2
+pcu.flood_fill_3d(grid, [0, 0, 0], fill_value) ``` ### Generating a mesh for a
+voxel grid Suppose you an array `ijk` of integer voxel coordinates. You may
+wish to plot the associated voxel grid. You can do this via the
+`voxel_grid_geometry` function as follows ```python import point_cloud_utils as
+pcu voxel_size = 1.0 / 200.0 # Size of each voxel voxel_origin = [0.0, 0.0,
+0.0] # The position of the bottom-back-left corner of the (0, 0, 0) voxel
+gap_fraction = 0.01 # Generate an optional small gap between voxels which can
+look nice -- this is a fraction of the voxel size ijk = np.random.randint(-100,
+100, size=(128, 3)) # Generate 128 random voxels in [-100, 100]^3 # vox_v,
+vox_f are vertices/faces of mesh for voxel grid vox_v, vox_f =
+pcu.voxel_grid_geoemtry(ijk, v, gap_fraction=gap_fraction,
+voxel_size=voxel_size, voxel_origin=voxel_origin) ```
```

### Comparing `point-cloud-utils-0.29.3/point_cloud_utils.egg-info/SOURCES.txt` & `point-cloud-utils-0.29.5/point_cloud_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 point_cloud_utils/__init__.py
 point_cloud_utils/_mesh_io.py
-point_cloud_utils/_octree.py
+point_cloud_utils/_point_cloud_geometry.py
 point_cloud_utils/_pointcloud_normals.py
-point_cloud_utils/_ray_mesh.py
 point_cloud_utils/_ray_mesh_intersector.py
 point_cloud_utils/_ray_point_cloud_intersector.py
 point_cloud_utils/_sinkhorn.py
+point_cloud_utils/_voxels.py
 point_cloud_utils.egg-info/PKG-INFO
 point_cloud_utils.egg-info/SOURCES.txt
 point_cloud_utils.egg-info/dependency_links.txt
 point_cloud_utils.egg-info/not-zip-safe
 point_cloud_utils.egg-info/requires.txt
 point_cloud_utils.egg-info/top_level.txt
 tests/test_examples.py
```

### Comparing `point-cloud-utils-0.29.3/setup.py` & `point-cloud-utils-0.29.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         sys.argv.remove('--use-mkl')
     if 'EXCLUDE_ARCH' in os.environ or '--exclude-arch' in sys.argv:
         exclude_arch = True
         sys.argv.remove('--exclude-arch')
 
     setuptools.setup(
         name="point-cloud-utils",
-        version="0.29.3",
+        version="0.29.5",
         author="Francis Williams",
         author_email="francis@fwilliams.info",
         description="A Python library for common tasks on 3D point clouds and meshes",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/fwilliams/point-cloud-utils",
         packages=setuptools.find_packages(exclude=["tests"]),
```

### Comparing `point-cloud-utils-0.29.3/tests/test_examples.py` & `point-cloud-utils-0.29.5/tests/test_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         _, n = pcu.estimate_point_cloud_normals_knn(v, 12)
         self.assertEqual(n.shape, v.shape)
 
         # Estimate normals for the point set, v using 12 nearest neighbors per point
         _, n = pcu.estimate_point_cloud_normals_ball(v, 0.2)
         self.assertEqual(n.shape, v.shape)
 
-    def skip_test_morton_coding_big_data(self):
+    def test_morton_coding_big_data(self):
         import point_cloud_utils as pcu
         import numpy as np
         import os
         if os.name == 'nt':
             num_pts = 1000
             num_qpts = 10
         else:
@@ -460,18 +460,17 @@
         codes = pcu.morton_encode(pts_int)
         codes_sort_idx = np.argsort(codes)
         codes_sorted = codes[codes_sort_idx]
 
         qcodes = pcu.morton_encode(qpts_int)
 
         nn_idx = pcu.morton_knn(codes_sorted, qcodes, 7)
-        codes_sorted[nn_idx]
         self.assertEqual(nn_idx.shape, (num_qpts, 7))
 
-    def skip_test_morton_coding_small_data(self):
+    def test_morton_coding_small_data(self):
         import point_cloud_utils as pcu
         import numpy as np
         div = 1.0 / 1000.0
         pts = np.random.rand(10, 3) / div
         pts_int = pts.astype(np.int32)
 
         qpts = np.random.rand(10000, 3) / div
@@ -483,15 +482,15 @@
 
         qcodes = pcu.morton_encode(qpts_int)
 
         nn_idx = pcu.morton_knn(codes_sorted, qcodes, 7)
         codes_sorted[nn_idx]
         self.assertEqual(nn_idx.shape, (10000, 7))
 
-    def skip_test_morton_coding_tiny_data(self):
+    def test_morton_coding_tiny_data(self):
         import point_cloud_utils as pcu
         import numpy as np
         div = 1.0 / 1000.0
         pts = np.random.rand(10, 3) / div
         pts_int = pts.astype(np.int32)
 
         qpts = np.random.rand(10000, 3) / div
@@ -711,15 +710,14 @@
         f = np.concatenate([f, f + v.shape[0]])
         v = np.concatenate([v, v + 1.0])
 
         cv, nv, cf, nf = pcu.connected_components(v, f)
         self.assertEqual(nv.sum(), v.shape[0])
         self.assertEqual(nf.sum(), f.shape[0])
 
-
     def test_triangle_soup_fast_winding_number(self):
         import point_cloud_utils as pcu
         import numpy as np
 
         v, f = pcu.load_mesh_vf(os.path.join(self.test_path, "bunny.ply"))
 
         p = np.random.rand(1000, 3)
```

