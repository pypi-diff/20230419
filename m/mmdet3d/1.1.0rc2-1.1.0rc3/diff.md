# Comparing `tmp/mmdet3d-1.1.0rc2.tar.gz` & `tmp/mmdet3d-1.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmdet3d-1.1.0rc2.tar", last modified: Sat Dec  3 13:01:02 2022, max compression
+gzip compressed data, was "dist/mmdet3d-1.1.0rc3.tar", last modified: Tue Jan 10 03:25:08 2023, max compression
```

## Comparing `mmdet3d-1.1.0rc2.tar` & `mmdet3d-1.1.0rc3.tar`

### file list

```diff
@@ -1,611 +1,612 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/
--rw-r--r--   0 runner    (1001) docker     (116)      216 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    19586 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    16457 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/3dssd/
--rw-r--r--   0 runner    (1001) docker     (116)     3642 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/3dssd/3dssd_4xb4_kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (116)      914 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/3dssd/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (116)     4516 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)     4422 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (116)     2800 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/kitti-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     3879 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/lyft-3d-range100.py
--rw-r--r--   0 runner    (1001) docker     (116)     4570 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     1960 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/nuim-instance.py
--rw-r--r--   0 runner    (1001) docker     (116)     5007 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     3772 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/nus-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     3460 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/s3dis-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     4656 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/s3dis-seg.py
--rw-r--r--   0 runner    (1001) docker     (116)     3965 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/scannet-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     4551 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (116)     3455 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/sunrgbd-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     5563 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)     5020 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (116)     4906 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/waymoD5-fov-mono3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)     4902 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv-mono3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)     4712 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)      655 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (116)     3077 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/3dssd.py
--rw-r--r--   0 runner    (1001) docker     (116)     6987 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/cascade-mask-rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (116)     3323 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/centerpoint_pillar02_second_secfpn_nus.py
--rw-r--r--   0 runner    (1001) docker     (116)     3415 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/centerpoint_voxel01_second_secfpn_nus.py
--rw-r--r--   0 runner    (1001) docker     (116)     1044 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/dgcnn.py
--rw-r--r--   0 runner    (1001) docker     (116)      723 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/fcaf3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     2702 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/fcos3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     2737 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/groupfree3d.py
--rw-r--r--   0 runner    (1001) docker     (116)    11349 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/h3dnet.py
--rw-r--r--   0 runner    (1001) docker     (116)     3872 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/imvotenet.py
--rw-r--r--   0 runner    (1001) docker     (116)     4165 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/mask-rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (116)     3572 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/multiview_dfm.py
--rw-r--r--   0 runner    (1001) docker     (116)      180 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/paconv_ssg-cuda.py
--rw-r--r--   0 runner    (1001) docker     (116)     2069 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/paconv_ssg.py
--rw-r--r--   0 runner    (1001) docker     (116)     7191 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/parta2.py
--rw-r--r--   0 runner    (1001) docker     (116)     1830 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pgd.py
--rw-r--r--   0 runner    (1001) docker     (116)     5661 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/point_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (116)     1223 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pointnet2_msg.py
--rw-r--r--   0 runner    (1001) docker     (116)     1330 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pointnet2_ssg.py
--rw-r--r--   0 runner    (1001) docker     (116)     1004 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_lyft.py
--rw-r--r--   0 runner    (1001) docker     (116)     3448 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_nus.py
--rw-r--r--   0 runner    (1001) docker     (116)     1016 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_range100_lyft.py
--rw-r--r--   0 runner    (1001) docker     (116)     3318 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_kitti.py
--rw-r--r--   0 runner    (1001) docker     (116)     4115 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_waymo.py
--rw-r--r--   0 runner    (1001) docker     (116)     3065 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_kitti.py
--rw-r--r--   0 runner    (1001) docker     (116)     3859 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_waymo.py
--rw-r--r--   0 runner    (1001) docker     (116)     1983 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/smoke.py
--rw-r--r--   0 runner    (1001) docker     (116)     2610 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/votenet.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (116)      947 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/cosine.py
--rw-r--r--   0 runner    (1001) docker     (116)     2015 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/cyclic-20e.py
--rw-r--r--   0 runner    (1001) docker     (116)     2284 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/cyclic-40e.py
--rw-r--r--   0 runner    (1001) docker     (116)      814 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/mmdet-schedule-1x.py
--rw-r--r--   0 runner    (1001) docker     (116)      995 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/schedule-2x.py
--rw-r--r--   0 runner    (1001) docker     (116)      888 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/schedule-3x.py
--rw-r--r--   0 runner    (1001) docker     (116)      749 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-100e.py
--rw-r--r--   0 runner    (1001) docker     (116)      749 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-150e.py
--rw-r--r--   0 runner    (1001) docker     (116)      736 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-200e.py
--rw-r--r--   0 runner    (1001) docker     (116)      734 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-50e.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/benchmark/
--rw-r--r--   0 runner    (1001) docker     (116)    12862 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/benchmark/hv_PartA2_secfpn_4x8_cyclic_80e_pcdet_kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)     7830 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_3x8_100e_det3d_kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (116)     8950 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_4x8_80e_pcdet_kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)     8750 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/benchmark/hv_second_secfpn_4x8_80e_pcdet_kitti-3d-3class.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/
--rw-r--r--   0 runner    (1001) docker     (116)     4869 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      134 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_head-circlenms_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      493 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_head-dcn-circlenms_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      445 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_head-dcn_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     4447 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      135 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-circlenms_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      494 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn-circlenms_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     1563 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn-circlenms_8xb4-flip-tta-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      446 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     1552 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-flip-tta-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     1641 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-tta-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     4901 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      133 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_head-circlenms_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      492 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_head-dcn-circlenms_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      444 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_head-dcn_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     4378 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dfm/
--rw-r--r--   0 runner    (1001) docker     (116)     1298 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_16xb2_waymoD5-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)     1840 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_centerhead_16xb2_waymoD5-3d-3class.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/
--rw-r--r--   0 runner    (1001) docker     (116)      568 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area1.py
--rw-r--r--   0 runner    (1001) docker     (116)      568 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area2.py
--rw-r--r--   0 runner    (1001) docker     (116)      568 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area3.py
--rw-r--r--   0 runner    (1001) docker     (116)      568 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area4.py
--rw-r--r--   0 runner    (1001) docker     (116)      695 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area5.py
--rw-r--r--   0 runner    (1001) docker     (116)      568 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area6.py
--rw-r--r--   0 runner    (1001) docker     (116)     3575 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dynamic_voxelization/
--rw-r--r--   0 runner    (1001) docker     (116)     2210 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dynamic_voxelization/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)      657 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dynamic_voxelization/pointpillars_dv_secfpn_8xb6-160e_kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (116)      715 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb2-cosine-80e_kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)      601 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb6-80e_kitti-3d-car.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcaf3d/
--rw-r--r--   0 runner    (1001) docker     (116)      700 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_s3dis-3d-5class.py
--rw-r--r--   0 runner    (1001) docker     (116)     2702 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_scannet-3d-18class.py
--rw-r--r--   0 runner    (1001) docker     (116)     2523 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_sunrgbd-3d-10class.py
--rw-r--r--   0 runner    (1001) docker     (116)     1981 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcaf3d/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcos3d/
--rw-r--r--   0 runner    (1001) docker     (116)     2450 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcos3d/fcos3d_r101-caffe-dcn_fpn_head-gn_8xb2-1x_nus-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      275 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcos3d/fcos3d_r101-caffe-dcn_fpn_head-gn_8xb2-1x_nus-mono3d_finetune.py
--rw-r--r--   0 runner    (1001) docker     (116)     1691 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcos3d/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/
--rw-r--r--   0 runner    (1001) docker     (116)     5576 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1628 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      600 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     2595 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      601 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     2724 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      599 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-400mf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/groupfree3d/
--rw-r--r--   0 runner    (1001) docker     (116)     7360 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L12-O256_4xb8_scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (116)     7329 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L6-O256_4xb8_scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (116)     7887 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O256_4xb8_scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (116)     7913 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O512_4xb8_scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (116)     2847 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/groupfree3d/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/h3dnet/
--rw-r--r--   0 runner    (1001) docker     (116)     3270 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/h3dnet/h3dnet_8xb3_scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (116)      969 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/h3dnet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/imvotenet/
--rw-r--r--   0 runner    (1001) docker     (116)     2253 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/imvotenet/imvotenet_faster-rcnn-r50_fpn_4xb2_sunrgbd-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     8035 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/imvotenet/imvotenet_stage2_8xb16_sunrgbd-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     1637 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/imvotenet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/imvoxelnet/
--rw-r--r--   0 runner    (1001) docker     (116)     5488 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_8xb4_kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (116)     1017 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/imvoxelnet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/monoflex/
--rw-r--r--   0 runner    (1001) docker     (116)     1044 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/monoflex/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/mvxnet/
--rw-r--r--   0 runner    (1001) docker     (116)     1100 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/mvxnet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)     8651 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/mvxnet/mvxnet_fpn_dv_second_secfpn_8xb2-80e_kitti-3d-3class.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/
--rw-r--r--   0 runner    (1001) docker     (116)      343 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn-r50-fpn_coco-20e_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)      127 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r101_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)     2335 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r50_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)      263 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r50_fpn_coco-20e-1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)      376 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_x101_32x4d_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)     1164 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)      174 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_coco-20e-1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)      124 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_coco-20e_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)     7778 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_head-without-semantic_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)      859 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/htc_x101_64x4d_fpn_dconv_c3-c5_coco-20e-1xb16_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)      119 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/mask-rcnn_r101_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)     1298 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)     1528 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)     1607 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_20e_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)      286 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)      478 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_coco-2x_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_coco-2x_1x_nus-2d.py
--rw-r--r--   0 runner    (1001) docker     (116)      368 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/mask-rcnn_x101_32x4d_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (116)    10039 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/paconv/
--rw-r--r--   0 runner    (1001) docker     (116)     1590 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/paconv/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1818 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/paconv/paconv_ssg-cuda_8xb8-cosine-200e_s3dis-seg.py
--rw-r--r--   0 runner    (1001) docker     (116)     1729 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/paconv/paconv_ssg_8xb8-cosine-150e_s3dis-seg.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/parta2/
--rw-r--r--   0 runner    (1001) docker     (116)     1593 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/parta2/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)     4746 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)     4736 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-car.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/
--rw-r--r--   0 runner    (1001) docker     (116)     3205 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)     3399 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-1x_nus-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      304 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-1x_nus-mono3d_finetune.py
--rw-r--r--   0 runner    (1001) docker     (116)      170 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-2x_nus-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      304 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-2x_nus-mono3d_finetune.py
--rw-r--r--   0 runner    (1001) docker     (116)     4453 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_4xb3-4x_kitti-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     3675 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-fov-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     3667 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     3674 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-mv-mono3d.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/point_rcnn/
--rw-r--r--   0 runner    (1001) docker     (116)      966 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/point_rcnn/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)     4447 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/point_rcnn/point-rcnn_8xb2_kitti-3d-3class.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/
--rw-r--r--   0 runner    (1001) docker     (116)     3986 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)     3615 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg-xyz-only.py
--rw-r--r--   0 runner    (1001) docker     (116)     1280 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (116)      831 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-80e_s3dis-seg.py
--rw-r--r--   0 runner    (1001) docker     (116)     3521 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg-xyz-only.py
--rw-r--r--   0 runner    (1001) docker     (116)     1186 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (116)      738 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-50e_s3dis-seg.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/
--rw-r--r--   0 runner    (1001) docker     (116)     8125 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)      433 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb2-2x_lyft-3d-range100.py
--rw-r--r--   0 runner    (1001) docker     (116)      415 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb2-2x_lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      460 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      140 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb4-amp-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     4061 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)     2993 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (116)      521 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)     1428 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (116)      194 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)     1342 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (116)     2045 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d-range100.py
--rw-r--r--   0 runner    (1001) docker     (116)     1996 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     2041 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      143 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb4-amp-2x_nus-3d.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pv_rcnn/
--rw-r--r--   0 runner    (1001) docker     (116)     1001 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pv_rcnn/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)    12065 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pv_rcnn/pv_rcnn_8xb2-80e_kitti-3d-3class.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/
--rw-r--r--   0 runner    (1001) docker     (116)     3436 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)      744 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-1.6gf_fpn_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     1035 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb2-2x_lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      793 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     1053 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_range100_8xb2-2x_lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     1677 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb2-2x_lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     1676 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     1728 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_range100_8xb2-2x_lyft-3d.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/sassd/
--rw-r--r--   0 runner    (1001) docker     (116)     3198 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/sassd/sassd_8xb6-80e_kitti-3d-3class.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/second/
--rw-r--r--   0 runner    (1001) docker     (116)     3391 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/second/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)      180 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-80e_kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)      972 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-80e_kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (116)      139 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-amp-80e_kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (116)      136 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-amp-80e_kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (116)     4664 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/second/second_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-3class.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/smoke/
--rw-r--r--   0 runner    (1001) docker     (116)     1039 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/smoke/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/smoke/smoke_dla34_dlaneck_gn-all_4xb8-6x_kitti-mono3d.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/ssn/
--rw-r--r--   0 runner    (1001) docker     (116)     2751 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/ssn/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)      742 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb1-2x_lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      727 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb2-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     9147 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     9774 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_nus-3d.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/votenet/
--rw-r--r--   0 runner    (1001) docker     (116)     1890 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/votenet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/votenet/votenet_8xb16_sunrgbd-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     1773 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/votenet/votenet_8xb8_scannet-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      225 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/votenet/votenet_head-iouloss_8xb8_scannet-3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      821 2022-12-03 13:00:59.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/model-index.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/analysis_tools/
--rw-r--r--   0 runner    (1001) docker     (116)     7535 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/analysis_tools/analyze_logs.py
--rw-r--r--   0 runner    (1001) docker     (116)     2923 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/analysis_tools/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (116)     2694 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/analysis_tools/get_flops.py
--rw-r--r--   0 runner    (1001) docker     (116)    13299 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/create_data.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      565 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/create_data.sh
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/
--rw-r--r--   0 runner    (1001) docker     (116)    25040 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/create_gt_database.py
--rw-r--r--   0 runner    (1001) docker     (116)     5097 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/indoor_converter.py
--rw-r--r--   0 runner    (1001) docker     (116)    24425 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/kitti_converter.py
--rw-r--r--   0 runner    (1001) docker     (116)    24980 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/kitti_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    10712 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/lyft_converter.py
--rw-r--r--   0 runner    (1001) docker     (116)     1411 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/lyft_data_fixer.py
--rw-r--r--   0 runner    (1001) docker     (116)     7644 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/nuimage_converter.py
--rw-r--r--   0 runner    (1001) docker     (116)    24485 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/nuscenes_converter.py
--rw-r--r--   0 runner    (1001) docker     (116)    10109 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/s3dis_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    12779 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/scannet_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     9109 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/sunrgbd_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    47943 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/update_infos_to_v2.py
--rw-r--r--   0 runner    (1001) docker     (116)    24677 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/waymo_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/deployment/
--rw-r--r--   0 runner    (1001) docker     (116)     3820 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/deployment/mmdet3d2torchserve.py
--rw-r--r--   0 runner    (1001) docker     (116)     4246 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/deployment/mmdet3d_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)     1930 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/deployment/test_torchserver.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      479 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dist_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      442 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dist_train.sh
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/misc/
--rw-r--r--   0 runner    (1001) docker     (116)     5207 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/misc/browse_dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)     2246 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/misc/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (116)      643 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/misc/print_config.py
--rw-r--r--   0 runner    (1001) docker     (116)     1456 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/misc/visualize_results.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/model_converters/
--rw-r--r--   0 runner    (1001) docker     (116)     6157 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/model_converters/convert_h3dnet_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (116)     5099 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/model_converters/convert_votenet_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (116)     1076 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/model_converters/publish_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     3063 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/model_converters/regnet2mmdet.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      566 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/slurm_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      574 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/slurm_train.sh
--rw-r--r--   0 runner    (1001) docker     (116)     4265 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/test.py
--rw-r--r--   0 runner    (1001) docker     (116)     4558 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/train.py
--rw-r--r--   0 runner    (1001) docker     (116)     6566 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/update_data_coords.py
--rw-r--r--   0 runner    (1001) docker     (116)      529 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/update_data_coords.sh
--rw-r--r--   0 runner    (1001) docker     (116)     1457 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/apis/
--rw-r--r--   0 runner    (1001) docker     (116)      459 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12522 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/apis/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/
--rw-r--r--   0 runner    (1001) docker     (116)     2359 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1743 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (116)    16167 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/convert_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     2843 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (116)    17076 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/det3d_dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)     8812 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/kitti2d_dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)     7296 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/kitti_dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)     3916 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/lyft_dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)     9827 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/nuscenes_dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)    15383 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/s3dis_dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)    13254 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/scannet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)    12382 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/seg3d_dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)     3319 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/semantickitti_dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)     5470 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/sunrgbd_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/
--rw-r--r--   0 runner    (1001) docker     (116)     1870 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    17093 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/data_augment_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    13086 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/dbsampler.py
--rw-r--r--   0 runner    (1001) docker     (116)     8582 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/formating.py
--rw-r--r--   0 runner    (1001) docker     (116)    37221 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/loading.py
--rw-r--r--   0 runner    (1001) docker     (116)     5608 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (116)    90050 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/transforms_3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     5206 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    11089 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/datasets/waymo_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/engine/
--rw-r--r--   0 runner    (1001) docker     (116)      160 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/engine/hooks/
--rw-r--r--   0 runner    (1001) docker     (116)      200 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/engine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1339 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/engine/hooks/benchmark_hook.py
--rw-r--r--   0 runner    (1001) docker     (116)     7286 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/engine/hooks/visualization_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/
--rw-r--r--   0 runner    (1001) docker     (116)     1406 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/
--rw-r--r--   0 runner    (1001) docker     (116)     1045 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10707 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/indoor_eval.py
--rw-r--r--   0 runner    (1001) docker     (116)     5191 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/instance_seg_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/kitti_utils/
--rw-r--r--   0 runner    (1001) docker     (116)      197 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/kitti_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    37841 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/kitti_utils/eval.py
--rw-r--r--   0 runner    (1001) docker     (116)    13153 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/kitti_utils/rotate_iou.py
--rw-r--r--   0 runner    (1001) docker     (116)    10382 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/lyft_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/scannet_utils/
--rw-r--r--   0 runner    (1001) docker     (116)      167 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/scannet_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15624 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/scannet_utils/evaluate_semantic_instance.py
--rw-r--r--   0 runner    (1001) docker     (116)     2607 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/scannet_utils/util_3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     3720 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/seg_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/waymo_utils/
--rw-r--r--   0 runner    (1001) docker     (116)      131 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/waymo_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16481 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/waymo_utils/prediction_to_waymo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (116)      596 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6790 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/indoor_metric.py
--rw-r--r--   0 runner    (1001) docker     (116)     3556 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/instance_seg_metric.py
--rw-r--r--   0 runner    (1001) docker     (116)    28781 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/kitti_metric.py
--rw-r--r--   0 runner    (1001) docker     (116)    15980 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/lyft_metric.py
--rw-r--r--   0 runner    (1001) docker     (116)    30914 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/nuscenes_metric.py
--rw-r--r--   0 runner    (1001) docker     (116)     5343 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/seg_metric.py
--rw-r--r--   0 runner    (1001) docker     (116)    31097 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/waymo_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/models/
--rw-r--r--   0 runner    (1001) docker     (116)     1622 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (116)      617 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1339 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/backbones/base_pointnet.py
--rw-r--r--   0 runner    (1001) docker     (116)     3688 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/backbones/dgcnn.py
--rw-r--r--   0 runner    (1001) docker     (116)    14804 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/backbones/dla.py
--rw-r--r--   0 runner    (1001) docker     (116)     4202 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/backbones/mink_resnet.py
--rw-r--r--   0 runner    (1001) docker     (116)     4754 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/backbones/multi_backbone.py
--rw-r--r--   0 runner    (1001) docker     (116)     3354 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/backbones/nostem_regnet.py
--rw-r--r--   0 runner    (1001) docker     (116)     7245 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/backbones/pointnet2_sa_msg.py
--rw-r--r--   0 runner    (1001) docker     (116)     5491 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/backbones/pointnet2_sa_ssg.py
--rw-r--r--   0 runner    (1001) docker     (116)     3249 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/backbones/second.py
--rw-r--r--   0 runner    (1001) docker     (116)     4092 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/models/data_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (116)      138 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/data_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16582 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/data_preprocessors/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (116)     2827 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/data_preprocessors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d/models/decode_heads/
--rw-r--r--   0 runner    (1001) docker     (116)      216 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/decode_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6229 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/decode_heads/decode_head.py
--rw-r--r--   0 runner    (1001) docker     (116)     2096 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/decode_heads/dgcnn_head.py
--rw-r--r--   0 runner    (1001) docker     (116)     2562 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/decode_heads/paconv_head.py
--rw-r--r--   0 runner    (1001) docker     (116)     3216 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/decode_heads/pointnet2_head.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:01.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/
--rw-r--r--   0 runner    (1001) docker     (116)     1173 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    18482 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/anchor3d_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    20566 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/anchor_free_mono3d_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    16512 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/base_3d_dense_head.py
--rw-r--r--   0 runner    (1001) docker     (116)     4407 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/base_conv_bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (116)     7535 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/base_mono3d_dense_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    37234 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/centerpoint_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    29985 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/fcaf3d_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    43730 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/fcos_mono3d_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    12085 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/free_anchor3d_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    47843 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/groupfree3d_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    36543 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/monoflex_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    18091 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/parta2_rpn_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    59499 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/pgd_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    21554 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/point_rpn_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    22821 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/shape_aware_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    23223 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/smoke_mono3d_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    25624 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/ssd_3d_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    17338 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/train_mixins.py
--rw-r--r--   0 runner    (1001) docker     (116)    36207 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/vote_head.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:01.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/
--rw-r--r--   0 runner    (1001) docker     (116)     1282 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6566 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     2936 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/centerpoint.py
--rw-r--r--   0 runner    (1001) docker     (116)    10083 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/dfm.py
--rw-r--r--   0 runner    (1001) docker     (116)     1710 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/dynamic_voxelnet.py
--rw-r--r--   0 runner    (1001) docker     (116)     4213 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/fcos_mono3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     3436 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/groupfree3dnet.py
--rw-r--r--   0 runner    (1001) docker     (116)     5825 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/h3dnet.py
--rw-r--r--   0 runner    (1001) docker     (116)    23036 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/imvotenet.py
--rw-r--r--   0 runner    (1001) docker     (116)    10538 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/imvoxelnet.py
--rw-r--r--   0 runner    (1001) docker     (116)     5766 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/mink_single_stage.py
--rw-r--r--   0 runner    (1001) docker     (116)    18515 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/multiview_dfm.py
--rw-r--r--   0 runner    (1001) docker     (116)     2001 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/mvx_faster_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (116)    16714 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/mvx_two_stage.py
--rw-r--r--   0 runner    (1001) docker     (116)     2563 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/parta2.py
--rw-r--r--   0 runner    (1001) docker     (116)     2443 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/point_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (116)     9948 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/pv_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (116)     4016 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/sassd.py
--rw-r--r--   0 runner    (1001) docker     (116)     6800 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/single_stage.py
--rw-r--r--   0 runner    (1001) docker     (116)     3693 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/single_stage_mono3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     1774 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/smoke_mono3d.py
--rw-r--r--   0 runner    (1001) docker     (116)      669 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/ssd3dnet.py
--rw-r--r--   0 runner    (1001) docker     (116)     8191 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/two_stage.py
--rw-r--r--   0 runner    (1001) docker     (116)     6356 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/votenet.py
--rw-r--r--   0 runner    (1001) docker     (116)     1870 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/detectors/voxelnet.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:01.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/
--rw-r--r--   0 runner    (1001) docker     (116)     1655 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10877 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/box3d_nms.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:01.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/dgcnn_modules/
--rw-r--r--   0 runner    (1001) docker     (116)      240 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/dgcnn_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2505 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/dgcnn_modules/dgcnn_fa_module.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/dgcnn_modules/dgcnn_fp_module.py
--rw-r--r--   0 runner    (1001) docker     (116)     8928 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/dgcnn_modules/dgcnn_gf_module.py
--rw-r--r--   0 runner    (1001) docker     (116)     3112 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/edge_fusion_module.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:01.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/fusion_layers/
--rw-r--r--   0 runner    (1001) docker     (116)      367 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/fusion_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8001 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/fusion_layers/coord_transform.py
--rw-r--r--   0 runner    (1001) docker     (116)    17816 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/fusion_layers/point_fusion.py
--rw-r--r--   0 runner    (1001) docker     (116)     9135 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/fusion_layers/vote_fusion.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/mlp.py
--rw-r--r--   0 runner    (1001) docker     (116)     5617 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/norm.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:01.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/paconv/
--rw-r--r--   0 runner    (1001) docker     (116)      123 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/paconv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16190 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/paconv/paconv.py
--rw-r--r--   0 runner    (1001) docker     (116)     3824 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/paconv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:01.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/pointnet_modules/
--rw-r--r--   0 runner    (1001) docker     (116)      590 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/pointnet_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1359 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/pointnet_modules/builder.py
--rw-r--r--   0 runner    (1001) docker     (116)    15034 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/pointnet_modules/paconv_sa_module.py
--rw-r--r--   0 runner    (1001) docker     (116)     3011 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/pointnet_modules/point_fp_module.py
--rw-r--r--   0 runner    (1001) docker     (116)    14492 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/pointnet_modules/point_sa_module.py
--rw-r--r--   0 runner    (1001) docker     (116)     7976 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/pointnet_modules/stack_point_sa_module.py
--rw-r--r--   0 runner    (1001) docker     (116)     7231 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/sparse_block.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:01.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/spconv/
--rw-r--r--   0 runner    (1001) docker     (116)      450 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/spconv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:01.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/spconv/overwrite_spconv/
--rw-r--r--   0 runner    (1001) docker     (116)      124 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/spconv/overwrite_spconv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4632 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/spconv/overwrite_spconv/write_spconv2.py
--rw-r--r--   0 runner    (1001) docker     (116)     6086 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/transformer.py
--rw-r--r--   0 runner    (1001) docker     (116)     7840 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/layers/vote_module.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:01.000000 mmdet3d-1.1.0rc2/mmdet3d/models/losses/
--rw-r--r--   0 runner    (1001) docker     (116)      818 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2810 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/losses/axis_aligned_iou_loss.py
--rw-r--r--   0 runner    (1001) docker     (116)     5524 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/losses/chamfer_distance.py
--rw-r--r--   0 runner    (1001) docker     (116)     3473 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/losses/multibin_loss.py
--rw-r--r--   0 runner    (1001) docker     (116)     4078 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/losses/paconv_regularization_loss.py
--rw-r--r--   0 runner    (1001) docker     (116)     3150 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/losses/rotated_iou_loss.py
--rw-r--r--   0 runner    (1001) docker     (116)     6355 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/losses/uncertain_smooth_l1_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/middle_encoders/
--rw-r--r--   0 runner    (1001) docker     (116)      370 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/middle_encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3651 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/middle_encoders/pillar_scatter.py
--rw-r--r--   0 runner    (1001) docker     (116)    20530 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/middle_encoders/sparse_encoder.py
--rw-r--r--   0 runner    (1001) docker     (116)    11897 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/middle_encoders/sparse_unet.py
--rw-r--r--   0 runner    (1001) docker     (116)    13989 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/middle_encoders/voxel_set_abstraction.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/necks/
--rw-r--r--   0 runner    (1001) docker     (116)      332 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8291 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/necks/dla_neck.py
--rw-r--r--   0 runner    (1001) docker     (116)     3309 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/necks/imvoxel_neck.py
--rw-r--r--   0 runner    (1001) docker     (116)     3204 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/necks/pointnet2_fp_neck.py
--rw-r--r--   0 runner    (1001) docker     (116)     3438 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/necks/second_fpn.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/
--rw-r--r--   0 runner    (1001) docker     (116)      689 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1997 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/base_3droi_head.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/bbox_heads/
--rw-r--r--   0 runner    (1001) docker     (116)      709 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/bbox_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    42934 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/bbox_heads/h3d_bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    26648 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/bbox_heads/parta2_bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    25469 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/bbox_heads/point_rcnn_bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    20941 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/bbox_heads/pv_rcnn_bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (116)     4447 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/h3d_roi_head.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/mask_heads/
--rw-r--r--   0 runner    (1001) docker     (116)      308 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/mask_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6446 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/mask_heads/foreground_segmentation_head.py
--rw-r--r--   0 runner    (1001) docker     (116)     8432 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/mask_heads/pointwise_semantic_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    46441 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/mask_heads/primitive_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    17145 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/part_aggregation_roi_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    13320 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/point_rcnn_roi_head.py
--rw-r--r--   0 runner    (1001) docker     (116)    13976 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/pv_rcnn_roi_head.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/roi_extractors/
--rw-r--r--   0 runner    (1001) docker     (116)      443 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/roi_extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3674 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/roi_extractors/batch_roigridpoint_extractor.py
--rw-r--r--   0 runner    (1001) docker     (116)     2204 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/roi_extractors/single_roiaware_extractor.py
--rw-r--r--   0 runner    (1001) docker     (116)     2460 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/roi_extractors/single_roipoint_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/segmentors/
--rw-r--r--   0 runner    (1001) docker     (116)      179 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6456 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/segmentors/base.py
--rw-r--r--   0 runner    (1001) docker     (116)    22249 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/segmentors/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/
--rw-r--r--   0 runner    (1001) docker     (116)     1736 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/anchor/
--rw-r--r--   0 runner    (1001) docker     (116)      586 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/anchor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    17850 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/anchor/anchor_3d_generator.py
--rw-r--r--   0 runner    (1001) docker     (116)      686 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/anchor/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/assigners/
--rw-r--r--   0 runner    (1001) docker     (116)      130 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/assigners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7574 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/assigners/max_3d_iou_assigner.py
--rw-r--r--   0 runner    (1001) docker     (116)     1015 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/
--rw-r--r--   0 runner    (1001) docker     (116)      827 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4356 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/anchor_free_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (116)     8688 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/centerpoint_bbox_coders.py
--rw-r--r--   0 runner    (1001) docker     (116)     3168 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/delta_xyzwhlr_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (116)     5148 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/fcos3d_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (116)     7243 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/groupfree3d_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (116)    20307 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/monoflex_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (116)     9145 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/partial_bin_based_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (116)     5363 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/pgd_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (116)     4542 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/point_xyzwhlr_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (116)     8291 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/smoke_bbox_coder.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/samplers/
--rw-r--r--   0 runner    (1001) docker     (116)      724 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8352 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/samplers/iou_neg_piecewise_sampler.py
--rw-r--r--   0 runner    (1001) docker     (116)     2180 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/samplers/pseudosample.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/voxel/
--rw-r--r--   0 runner    (1001) docker     (116)      122 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/voxel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11493 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/voxel/voxel_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/test_time_augs/
--rw-r--r--   0 runner    (1001) docker     (116)      127 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/test_time_augs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3570 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/test_time_augs/merge_augs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/utils/
--rw-r--r--   0 runner    (1001) docker     (116)      653 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      419 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/utils/add_prefix.py
--rw-r--r--   0 runner    (1001) docker     (116)      468 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/utils/clip_sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (116)     3090 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/utils/edge_indices.py
--rw-r--r--   0 runner    (1001) docker     (116)     5252 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/utils/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (116)     3152 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/utils/gen_keypoints.py
--rw-r--r--   0 runner    (1001) docker     (116)     5493 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/utils/handle_objs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/models/voxel_encoders/
--rw-r--r--   0 runner    (1001) docker     (116)      329 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/voxel_encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13784 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/voxel_encoders/pillar_encoder.py
--rw-r--r--   0 runner    (1001) docker     (116)     6778 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/voxel_encoders/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    20811 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/models/voxel_encoders/voxel_encoder.py
--rw-r--r--   0 runner    (1001) docker     (116)     3975 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/
--rw-r--r--   0 runner    (1001) docker     (116)     2931 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/
--rw-r--r--   0 runner    (1001) docker     (116)      817 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    21390 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/base_box3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     9735 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/box_3d_mode.py
--rw-r--r--   0 runner    (1001) docker     (116)    14014 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/cam_box3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     9153 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/coord_3d_mode.py
--rw-r--r--   0 runner    (1001) docker     (116)    10806 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/depth_box3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     8330 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/lidar_box3d.py
--rw-r--r--   0 runner    (1001) docker     (116)    12393 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     9073 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/det3d_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/ops/
--rw-r--r--   0 runner    (1001) docker     (116)     2207 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    30923 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/ops/box_np_ops.py
--rw-r--r--   0 runner    (1001) docker     (116)    12785 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/ops/iou3d_calculator.py
--rw-r--r--   0 runner    (1001) docker     (116)     2421 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/ops/transforms.py
--rw-r--r--   0 runner    (1001) docker     (116)     6293 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/point_data.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/points/
--rw-r--r--   0 runner    (1001) docker     (116)      921 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16593 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/points/base_points.py
--rw-r--r--   0 runner    (1001) docker     (116)     2476 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/points/cam_points.py
--rw-r--r--   0 runner    (1001) docker     (116)     2343 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/points/depth_points.py
--rw-r--r--   0 runner    (1001) docker     (116)     2343 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/structures/points/lidar_points.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/testing/
--rw-r--r--   0 runner    (1001) docker     (116)      543 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6782 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/testing/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     5365 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/testing/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/utils/
--rw-r--r--   0 runner    (1001) docker     (116)      732 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13217 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/utils/array_converter.py
--rw-r--r--   0 runner    (1001) docker     (116)      671 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (116)     5970 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/utils/compat_cfg.py
--rw-r--r--   0 runner    (1001) docker     (116)     3753 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (116)     4319 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (116)      805 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (116)      800 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/mmdet3d/visualization/
--rw-r--r--   0 runner    (1001) docker     (116)      485 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    36078 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/visualization/local_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (116)     6186 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/mmdet3d/visualization/vis_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    19586 2022-12-03 13:00:59.000000 mmdet3d-1.1.0rc2/mmdet3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    27618 2022-12-03 13:01:00.000000 mmdet3d-1.1.0rc2/mmdet3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-03 13:00:59.000000 mmdet3d-1.1.0rc2/mmdet3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-03 13:00:59.000000 mmdet3d-1.1.0rc2/mmdet3d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      734 2022-12-03 13:00:59.000000 mmdet3d-1.1.0rc2/mmdet3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2022-12-03 13:00:59.000000 mmdet3d-1.1.0rc2/mmdet3d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/requirements/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (116)      197 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (116)       68 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/requirements/mminstall.txt
--rw-r--r--   0 runner    (1001) docker     (116)      165 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (116)       65 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/requirements/readthedocs.txt
--rw-r--r--   0 runner    (1001) docker     (116)      185 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (116)      193 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (116)      795 2022-12-03 13:01:02.000000 mmdet3d-1.1.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     8183 2022-12-03 12:59:29.000000 mmdet3d-1.1.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (116)      216 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    19584 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    16455 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/3dssd/
+-rw-r--r--   0 runner    (1001) docker     (116)     3642 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/3dssd/3dssd_4xb4_kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (116)      914 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/3dssd/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (116)     4516 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4422 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2800 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/kitti-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3879 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/lyft-3d-range100.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4570 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1960 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/nuim-instance.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5007 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3772 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/nus-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3460 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/s3dis-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4656 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/s3dis-seg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3965 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/scannet-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4551 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3455 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/sunrgbd-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5563 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5020 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4906 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/waymoD5-fov-mono3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4902 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv-mono3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4712 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)      655 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (116)     3077 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/3dssd.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6987 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/cascade-mask-rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3323 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/centerpoint_pillar02_second_secfpn_nus.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3415 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/centerpoint_voxel01_second_secfpn_nus.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1044 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/dgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (116)      723 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/fcaf3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2702 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/fcos3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2737 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/groupfree3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11349 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/h3dnet.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3872 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/imvotenet.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4165 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/mask-rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3572 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/multiview_dfm.py
+-rw-r--r--   0 runner    (1001) docker     (116)      180 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/paconv_ssg-cuda.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2069 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/paconv_ssg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7191 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/parta2.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1830 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pgd.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5661 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/point_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1223 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pointnet2_msg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1330 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pointnet2_ssg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1004 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_lyft.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3448 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_nus.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1016 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_range100_lyft.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3318 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_kitti.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4115 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_waymo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3065 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_kitti.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3859 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_waymo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1983 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/smoke.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2610 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/votenet.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (116)      947 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2015 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/cyclic-20e.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2284 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/cyclic-40e.py
+-rw-r--r--   0 runner    (1001) docker     (116)      814 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/mmdet-schedule-1x.py
+-rw-r--r--   0 runner    (1001) docker     (116)      995 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/schedule-2x.py
+-rw-r--r--   0 runner    (1001) docker     (116)      888 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/schedule-3x.py
+-rw-r--r--   0 runner    (1001) docker     (116)      749 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-100e.py
+-rw-r--r--   0 runner    (1001) docker     (116)      749 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-150e.py
+-rw-r--r--   0 runner    (1001) docker     (116)      736 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-200e.py
+-rw-r--r--   0 runner    (1001) docker     (116)      734 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-50e.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (116)    12862 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/benchmark/hv_PartA2_secfpn_4x8_cyclic_80e_pcdet_kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7830 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_3x8_100e_det3d_kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8950 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_4x8_80e_pcdet_kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8750 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/benchmark/hv_second_secfpn_4x8_80e_pcdet_kitti-3d-3class.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/
+-rw-r--r--   0 runner    (1001) docker     (116)     4869 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      134 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_head-circlenms_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      493 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_head-dcn-circlenms_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      445 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_head-dcn_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4447 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      135 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-circlenms_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      494 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn-circlenms_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1563 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn-circlenms_8xb4-flip-tta-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      446 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1552 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-flip-tta-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1641 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-tta-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4901 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      133 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_head-circlenms_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      492 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_head-dcn-circlenms_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      444 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_head-dcn_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4378 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dfm/
+-rw-r--r--   0 runner    (1001) docker     (116)     1298 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_16xb2_waymoD5-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1840 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_centerhead_16xb2_waymoD5-3d-3class.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/
+-rw-r--r--   0 runner    (1001) docker     (116)      568 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area1.py
+-rw-r--r--   0 runner    (1001) docker     (116)      568 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area2.py
+-rw-r--r--   0 runner    (1001) docker     (116)      568 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area3.py
+-rw-r--r--   0 runner    (1001) docker     (116)      568 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area4.py
+-rw-r--r--   0 runner    (1001) docker     (116)      695 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area5.py
+-rw-r--r--   0 runner    (1001) docker     (116)      568 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area6.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3575 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dynamic_voxelization/
+-rw-r--r--   0 runner    (1001) docker     (116)     2210 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dynamic_voxelization/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      657 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dynamic_voxelization/pointpillars_dv_secfpn_8xb6-160e_kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (116)      715 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb2-cosine-80e_kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)      601 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb6-80e_kitti-3d-car.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcaf3d/
+-rw-r--r--   0 runner    (1001) docker     (116)      700 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_s3dis-3d-5class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2702 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_scannet-3d-18class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2523 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_sunrgbd-3d-10class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1981 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcaf3d/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcos3d/
+-rw-r--r--   0 runner    (1001) docker     (116)     2450 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcos3d/fcos3d_r101-caffe-dcn_fpn_head-gn_8xb2-1x_nus-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      295 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcos3d/fcos3d_r101-caffe-dcn_fpn_head-gn_8xb2-1x_nus-mono3d_finetune.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1691 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcos3d/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/
+-rw-r--r--   0 runner    (1001) docker     (116)     5576 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1628 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      600 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2595 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      601 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2724 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      599 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-400mf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/groupfree3d/
+-rw-r--r--   0 runner    (1001) docker     (116)     7360 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L12-O256_4xb8_scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7329 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L6-O256_4xb8_scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7887 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O256_4xb8_scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7913 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O512_4xb8_scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2847 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/groupfree3d/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/h3dnet/
+-rw-r--r--   0 runner    (1001) docker     (116)     3270 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/h3dnet/h3dnet_8xb3_scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (116)      969 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/h3dnet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/imvotenet/
+-rw-r--r--   0 runner    (1001) docker     (116)     2253 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/imvotenet/imvotenet_faster-rcnn-r50_fpn_4xb2_sunrgbd-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8035 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/imvotenet/imvotenet_stage2_8xb16_sunrgbd-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1637 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/imvotenet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/imvoxelnet/
+-rw-r--r--   0 runner    (1001) docker     (116)     4427 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_2xb4_sunrgbd-3d-10class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5511 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_8xb4_kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1017 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/imvoxelnet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/monoflex/
+-rw-r--r--   0 runner    (1001) docker     (116)     1044 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/monoflex/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/mvxnet/
+-rw-r--r--   0 runner    (1001) docker     (116)     1100 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/mvxnet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     8651 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/mvxnet/mvxnet_fpn_dv_second_secfpn_8xb2-80e_kitti-3d-3class.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/
+-rw-r--r--   0 runner    (1001) docker     (116)      343 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn-r50-fpn_coco-20e_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)      127 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r101_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2335 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r50_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)      263 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r50_fpn_coco-20e-1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)      376 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_x101_32x4d_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1164 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)      174 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_coco-20e-1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)      124 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_coco-20e_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7778 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_head-without-semantic_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)      859 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/htc_x101_64x4d_fpn_dconv_c3-c5_coco-20e-1xb16_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)      119 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/mask-rcnn_r101_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1298 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1528 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1607 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_20e_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)      286 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)      478 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_coco-2x_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1108 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_coco-2x_1x_nus-2d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      368 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/mask-rcnn_x101_32x4d_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10039 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/paconv/
+-rw-r--r--   0 runner    (1001) docker     (116)     1590 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/paconv/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1818 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/paconv/paconv_ssg-cuda_8xb8-cosine-200e_s3dis-seg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1729 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/paconv/paconv_ssg_8xb8-cosine-150e_s3dis-seg.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/parta2/
+-rw-r--r--   0 runner    (1001) docker     (116)     1593 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/parta2/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     4746 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4736 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-car.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/
+-rw-r--r--   0 runner    (1001) docker     (116)     3205 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     3526 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-1x_nus-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      324 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-1x_nus-mono3d_finetune.py
+-rw-r--r--   0 runner    (1001) docker     (116)      403 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-2x_nus-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      324 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-2x_nus-mono3d_finetune.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4508 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_4xb3-4x_kitti-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3660 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-fov-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3652 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3659 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-mv-mono3d.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/point_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (116)      966 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/point_rcnn/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     4447 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/point_rcnn/point-rcnn_8xb2_kitti-3d-3class.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/
+-rw-r--r--   0 runner    (1001) docker     (116)     3986 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     3615 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg-xyz-only.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1280 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (116)      831 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-80e_s3dis-seg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3521 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg-xyz-only.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1186 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (116)      738 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-50e_s3dis-seg.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/
+-rw-r--r--   0 runner    (1001) docker     (116)     8125 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      433 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb2-2x_lyft-3d-range100.py
+-rw-r--r--   0 runner    (1001) docker     (116)      415 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb2-2x_lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      460 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      140 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb4-amp-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4061 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2993 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (116)      521 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1428 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (116)      194 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1342 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2045 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d-range100.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1996 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2041 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      143 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb4-amp-2x_nus-3d.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pv_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (116)     1001 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pv_rcnn/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)    12065 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pv_rcnn/pv_rcnn_8xb2-80e_kitti-3d-3class.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/
+-rw-r--r--   0 runner    (1001) docker     (116)     3436 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      744 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-1.6gf_fpn_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1035 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb2-2x_lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      793 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1053 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_range100_8xb2-2x_lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1677 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb2-2x_lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1676 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1728 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_range100_8xb2-2x_lyft-3d.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/sassd/
+-rw-r--r--   0 runner    (1001) docker     (116)     3198 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/sassd/sassd_8xb6-80e_kitti-3d-3class.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/second/
+-rw-r--r--   0 runner    (1001) docker     (116)     3391 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/second/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      180 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-80e_kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)      972 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-80e_kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (116)      139 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-amp-80e_kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (116)      136 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-amp-80e_kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4664 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/second/second_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-3class.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/smoke/
+-rw-r--r--   0 runner    (1001) docker     (116)     1039 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/smoke/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     2151 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/smoke/smoke_dla34_dlaneck_gn-all_4xb8-6x_kitti-mono3d.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/ssn/
+-rw-r--r--   0 runner    (1001) docker     (116)     2751 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/ssn/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      742 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb1-2x_lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      727 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb2-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9147 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9774 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_nus-3d.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/votenet/
+-rw-r--r--   0 runner    (1001) docker     (116)     1890 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/votenet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1108 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/votenet/votenet_8xb16_sunrgbd-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1773 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/votenet/votenet_8xb8_scannet-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      225 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/votenet/votenet_head-iouloss_8xb8_scannet-3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      821 2023-01-10 03:25:07.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/model-index.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (116)     7535 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/analysis_tools/analyze_logs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2883 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/analysis_tools/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2694 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/analysis_tools/get_flops.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13299 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/create_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)      565 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/create_data.sh
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/
+-rw-r--r--   0 runner    (1001) docker     (116)    25037 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/create_gt_database.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5097 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/indoor_converter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24425 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/kitti_converter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24980 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/kitti_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10712 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/lyft_converter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1411 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/lyft_data_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7644 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/nuimage_converter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24485 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/nuscenes_converter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10109 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/s3dis_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12779 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/scannet_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9109 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/sunrgbd_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    48219 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/update_infos_to_v2.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24687 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/waymo_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/deployment/
+-rw-r--r--   0 runner    (1001) docker     (116)     3820 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/deployment/mmdet3d2torchserve.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4246 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/deployment/mmdet3d_handler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1930 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/deployment/test_torchserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)      479 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dist_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (116)      442 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dist_train.sh
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/misc/
+-rw-r--r--   0 runner    (1001) docker     (116)     5207 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/misc/browse_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2246 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/misc/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (116)      643 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/misc/print_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1456 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/misc/visualize_results.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/model_converters/
+-rw-r--r--   0 runner    (1001) docker     (116)     6149 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/model_converters/convert_h3dnet_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5091 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/model_converters/convert_votenet_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1076 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/model_converters/publish_model.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3063 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/model_converters/regnet2mmdet.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)      566 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/slurm_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (116)      574 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/slurm_train.sh
+-rw-r--r--   0 runner    (1001) docker     (116)     4581 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4558 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/train.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6566 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/update_data_coords.py
+-rw-r--r--   0 runner    (1001) docker     (116)      529 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/update_data_coords.sh
+-rw-r--r--   0 runner    (1001) docker     (116)     1457 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/apis/
+-rw-r--r--   0 runner    (1001) docker     (116)      459 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12476 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/apis/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/
+-rw-r--r--   0 runner    (1001) docker     (116)     2253 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16257 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2843 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17076 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/det3d_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8812 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/kitti2d_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7288 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/kitti_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3916 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/lyft_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9827 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/nuscenes_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15383 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/s3dis_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13254 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/scannet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12382 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/seg3d_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3319 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/semantickitti_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5470 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/sunrgbd_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/
+-rw-r--r--   0 runner    (1001) docker     (116)     1870 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17093 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/data_augment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13086 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/dbsampler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8582 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/formating.py
+-rw-r--r--   0 runner    (1001) docker     (116)    37640 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/loading.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5608 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (116)    90137 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/transforms_3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5206 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10773 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/datasets/waymo_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/engine/
+-rw-r--r--   0 runner    (1001) docker     (116)      160 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/engine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (116)      297 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/engine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1339 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/engine/hooks/benchmark_hook.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2152 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/engine/hooks/disable_object_sample_hook.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7512 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/engine/hooks/visualization_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (116)     1406 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/
+-rw-r--r--   0 runner    (1001) docker     (116)     1045 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10707 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/indoor_eval.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5191 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/instance_seg_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/kitti_utils/
+-rw-r--r--   0 runner    (1001) docker     (116)      197 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/kitti_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    37841 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/kitti_utils/eval.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13153 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/kitti_utils/rotate_iou.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10382 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/lyft_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/scannet_utils/
+-rw-r--r--   0 runner    (1001) docker     (116)      167 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/scannet_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15624 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/scannet_utils/evaluate_semantic_instance.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2607 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/scannet_utils/util_3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3720 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/seg_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/waymo_utils/
+-rw-r--r--   0 runner    (1001) docker     (116)      131 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/waymo_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16481 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/waymo_utils/prediction_to_waymo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (116)      596 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6790 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/indoor_metric.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3556 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/instance_seg_metric.py
+-rw-r--r--   0 runner    (1001) docker     (116)    28781 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/kitti_metric.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15980 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/lyft_metric.py
+-rw-r--r--   0 runner    (1001) docker     (116)    30914 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/nuscenes_metric.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5343 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/seg_metric.py
+-rw-r--r--   0 runner    (1001) docker     (116)    31095 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/waymo_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/
+-rw-r--r--   0 runner    (1001) docker     (116)      750 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (116)      617 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1339 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/backbones/base_pointnet.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3688 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/backbones/dgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14804 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/backbones/dla.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4202 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/backbones/mink_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4702 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/backbones/multi_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3354 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/backbones/nostem_regnet.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7245 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/backbones/pointnet2_sa_msg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5491 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/backbones/pointnet2_sa_ssg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3249 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/backbones/second.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/data_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (116)      138 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/data_preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16582 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/data_preprocessors/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2827 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/data_preprocessors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/decode_heads/
+-rw-r--r--   0 runner    (1001) docker     (116)      216 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/decode_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6235 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/decode_heads/decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2096 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/decode_heads/dgcnn_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2568 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/decode_heads/paconv_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3222 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/decode_heads/pointnet2_head.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/
+-rw-r--r--   0 runner    (1001) docker     (116)     1226 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18494 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/anchor3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20566 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/anchor_free_mono3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16518 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/base_3d_dense_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4407 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/base_conv_bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7535 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/base_mono3d_dense_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    37205 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/centerpoint_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    29985 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/fcaf3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    43730 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/fcos_mono3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12085 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/free_anchor3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    47843 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/groupfree3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    29871 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/imvoxel_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    36543 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/monoflex_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18097 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/parta2_rpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    59511 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/pgd_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21560 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/point_rpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22790 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/shape_aware_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23223 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/smoke_mono3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25624 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/ssd_3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17338 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/train_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (116)    36207 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/vote_head.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/
+-rw-r--r--   0 runner    (1001) docker     (116)     1282 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6614 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2936 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/centerpoint.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10030 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/dfm.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1710 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/dynamic_voxelnet.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4213 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/fcos_mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3436 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/groupfree3dnet.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5825 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/h3dnet.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23036 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/imvotenet.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11896 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/imvoxelnet.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5766 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/mink_single_stage.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18515 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/multiview_dfm.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2001 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/mvx_faster_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16714 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/mvx_two_stage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2563 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/parta2.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2443 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/point_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9948 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/pv_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4016 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/sassd.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6800 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/single_stage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3693 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/single_stage_mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1774 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/smoke_mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)      669 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/ssd3dnet.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8191 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/two_stage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6356 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/votenet.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1870 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/detectors/voxelnet.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/
+-rw-r--r--   0 runner    (1001) docker     (116)     1655 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10877 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/box3d_nms.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/dgcnn_modules/
+-rw-r--r--   0 runner    (1001) docker     (116)      240 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/dgcnn_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2505 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/dgcnn_modules/dgcnn_fa_module.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2163 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/dgcnn_modules/dgcnn_fp_module.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8928 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/dgcnn_modules/dgcnn_gf_module.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3112 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/edge_fusion_module.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/fusion_layers/
+-rw-r--r--   0 runner    (1001) docker     (116)      367 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/fusion_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8001 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/fusion_layers/coord_transform.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17816 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/fusion_layers/point_fusion.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9135 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/fusion_layers/vote_fusion.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2162 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5617 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/norm.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/paconv/
+-rw-r--r--   0 runner    (1001) docker     (116)      123 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/paconv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16190 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/paconv/paconv.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3824 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/paconv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/pointnet_modules/
+-rw-r--r--   0 runner    (1001) docker     (116)      590 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/pointnet_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1359 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/pointnet_modules/builder.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15034 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/pointnet_modules/paconv_sa_module.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3011 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/pointnet_modules/point_fp_module.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14492 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/pointnet_modules/point_sa_module.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7976 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/pointnet_modules/stack_point_sa_module.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7231 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/sparse_block.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/spconv/
+-rw-r--r--   0 runner    (1001) docker     (116)      384 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/spconv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/spconv/overwrite_spconv/
+-rw-r--r--   0 runner    (1001) docker     (116)      124 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/spconv/overwrite_spconv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4632 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/spconv/overwrite_spconv/write_spconv2.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6086 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7840 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/layers/vote_module.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (116)      818 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2810 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/losses/axis_aligned_iou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5524 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/losses/chamfer_distance.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3473 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/losses/multibin_loss.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4078 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/losses/paconv_regularization_loss.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3150 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/losses/rotated_iou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6355 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/losses/uncertain_smooth_l1_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/middle_encoders/
+-rw-r--r--   0 runner    (1001) docker     (116)      370 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/middle_encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3651 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/middle_encoders/pillar_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20530 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/middle_encoders/sparse_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11897 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/middle_encoders/sparse_unet.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13989 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/middle_encoders/voxel_set_abstraction.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (116)      376 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8291 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/necks/dla_neck.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7722 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/necks/imvoxel_neck.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3204 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/necks/pointnet2_fp_neck.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3438 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/necks/second_fpn.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/
+-rw-r--r--   0 runner    (1001) docker     (116)      689 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1997 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/base_3droi_head.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/bbox_heads/
+-rw-r--r--   0 runner    (1001) docker     (116)      709 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/bbox_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    42934 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/bbox_heads/h3d_bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26660 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/bbox_heads/parta2_bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25475 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/bbox_heads/point_rcnn_bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20899 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/bbox_heads/pv_rcnn_bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4447 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/h3d_roi_head.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/mask_heads/
+-rw-r--r--   0 runner    (1001) docker     (116)      308 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/mask_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6402 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/mask_heads/foreground_segmentation_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8432 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/mask_heads/pointwise_semantic_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    46441 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/mask_heads/primitive_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17145 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/part_aggregation_roi_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13326 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/point_rcnn_roi_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13976 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/pv_rcnn_roi_head.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/roi_extractors/
+-rw-r--r--   0 runner    (1001) docker     (116)      443 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/roi_extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3674 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/roi_extractors/batch_roigridpoint_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2204 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/roi_extractors/single_roiaware_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2460 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/roi_extractors/single_roipoint_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/segmentors/
+-rw-r--r--   0 runner    (1001) docker     (116)      179 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6456 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/segmentors/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22249 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/segmentors/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/
+-rw-r--r--   0 runner    (1001) docker     (116)     1736 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/anchor/
+-rw-r--r--   0 runner    (1001) docker     (116)      586 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/anchor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17850 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/anchor/anchor_3d_generator.py
+-rw-r--r--   0 runner    (1001) docker     (116)      686 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/anchor/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/assigners/
+-rw-r--r--   0 runner    (1001) docker     (116)      130 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/assigners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7574 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/assigners/max_3d_iou_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1015 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/
+-rw-r--r--   0 runner    (1001) docker     (116)      827 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4356 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/anchor_free_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8688 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/centerpoint_bbox_coders.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3168 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/delta_xyzwhlr_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5148 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/fcos3d_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7243 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/groupfree3d_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20307 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/monoflex_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9145 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/partial_bin_based_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5363 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/pgd_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4542 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/point_xyzwhlr_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8291 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/smoke_bbox_coder.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/samplers/
+-rw-r--r--   0 runner    (1001) docker     (116)      724 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8352 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/samplers/iou_neg_piecewise_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2180 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/samplers/pseudosample.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/voxel/
+-rw-r--r--   0 runner    (1001) docker     (116)      122 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/voxel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11493 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/voxel/voxel_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/test_time_augs/
+-rw-r--r--   0 runner    (1001) docker     (116)      127 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/test_time_augs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3570 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/test_time_augs/merge_augs.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)      653 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      419 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/utils/add_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (116)      468 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/utils/clip_sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3090 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/utils/edge_indices.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5252 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/utils/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3152 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/utils/gen_keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5493 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/utils/handle_objs.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/models/voxel_encoders/
+-rw-r--r--   0 runner    (1001) docker     (116)      329 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/voxel_encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13784 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/voxel_encoders/pillar_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6778 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/voxel_encoders/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20760 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/models/voxel_encoders/voxel_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3975 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/
+-rw-r--r--   0 runner    (1001) docker     (116)     2931 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/
+-rw-r--r--   0 runner    (1001) docker     (116)      817 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21679 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/base_box3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9735 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/box_3d_mode.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14014 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/cam_box3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9153 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/coord_3d_mode.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10806 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/depth_box3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8330 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/lidar_box3d.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12393 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9073 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/det3d_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/ops/
+-rw-r--r--   0 runner    (1001) docker     (116)     2207 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    30923 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/ops/box_np_ops.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12785 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/ops/iou3d_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2421 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/ops/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6293 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/point_data.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/points/
+-rw-r--r--   0 runner    (1001) docker     (116)      921 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16593 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/points/base_points.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2476 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/points/cam_points.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2343 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/points/depth_points.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2343 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/structures/points/lidar_points.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/testing/
+-rw-r--r--   0 runner    (1001) docker     (116)      543 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6782 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/testing/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5365 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/testing/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)      771 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13217 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/utils/array_converter.py
+-rw-r--r--   0 runner    (1001) docker     (116)      671 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5970 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/utils/compat_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3753 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4319 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (116)      805 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/utils/typing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      800 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d/visualization/
+-rw-r--r--   0 runner    (1001) docker     (116)      485 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    36078 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/visualization/local_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6186 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/mmdet3d/visualization/vis_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    19584 2023-01-10 03:25:07.000000 mmdet3d-1.1.0rc3/mmdet3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    27734 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/mmdet3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-10 03:25:07.000000 mmdet3d-1.1.0rc3/mmdet3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-10 03:25:07.000000 mmdet3d-1.1.0rc3/mmdet3d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      720 2023-01-10 03:25:07.000000 mmdet3d-1.1.0rc3/mmdet3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        8 2023-01-10 03:25:07.000000 mmdet3d-1.1.0rc3/mmdet3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      197 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       68 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/requirements/mminstall.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      158 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       65 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/requirements/readthedocs.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      185 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      193 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      795 2023-01-10 03:25:08.000000 mmdet3d-1.1.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     8183 2023-01-10 03:23:30.000000 mmdet3d-1.1.0rc3/setup.py
```

### Comparing `mmdet3d-1.1.0rc2/PKG-INFO` & `mmdet3d-1.1.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmdet3d
-Version: 1.1.0rc2
+Version: 1.1.0rc3
 Summary: OpenMMLab's next-generation platformfor general 3D object detection.
 Home-page: https://github.com/open-mmlab/mmdetection3d
 Author: MMDetection3D Contributors
 Author-email: zwwdev@gmail.com
 License: Apache License 2.0
 Description: <div align="center">
           <img src="resources/mmdet3d-logo.png" width="600"/>
@@ -30,15 +30,15 @@
         [![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmdetection3d.readthedocs.io/en/1.1/)
         [![badge](https://github.com/open-mmlab/mmdetection3d/workflows/build/badge.svg)](https://github.com/open-mmlab/mmdetection3d/actions)
         [![codecov](https://codecov.io/gh/open-mmlab/mmdetection3d/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmdetection3d)
         [![license](https://img.shields.io/github/license/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/master/LICENSE)
         
         **News**:
         
-        **v1.1.0rc2** was released in 2/12/2022
+        **v1.1.0rc3** was released in 7/1/2023
         
         The compatibilities of models are broken due to the unification and simplification of coordinate systems after v1.0.0rc0. For now, most models are benchmarked with similar performance, though few models are still being benchmarked. In the following release, we will update all the model checkpoints and benchmarks. See more details in the [Changelog](docs/en/notes/changelog.md) and [Changelog-v1.0.x](docs/en/notes/changelog_v1.0.x.md).
         
         Documentation: https://mmdetection3d.readthedocs.io/
         
         ## Introduction
         
@@ -82,15 +82,15 @@
         
         ## License
         
         This project is released under the [Apache 2.0 license](LICENSE).
         
         ## Changelog
         
-        **1.1.0rc2** was released in 2/12/2022.
+        **1.1.0rc3** was released in 7/1/2023.
         
         Please refer to [changelog.md](docs/en/notes/changelog.md) for details and release history.
         
         ## Benchmark and model zoo
         
         Results and models are available in the [model zoo](docs/en/model_zoo.md).
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: mmdet3d Version: 1.1.0rc2 Summary: OpenMMLab's
+Metadata-Version: 2.1 Name: mmdet3d Version: 1.1.0rc3 Summary: OpenMMLab's
 next-generation platformfor general 3D object detection. Home-page: https://
 github.com/open-mmlab/mmdetection3d Author: MMDetection3D Contributors Author-
 email: zwwdev@gmail.com License: Apache License 2.0 Description:
                          [resources/mmdet3d-logo.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
 [![docs](https://img.shields.io/badge/docs-latest-blue)](https://
 mmdetection3d.readthedocs.io/en/1.1/) [![badge](https://github.com/open-mmlab/
 mmdetection3d/workflows/build/badge.svg)](https://github.com/open-mmlab/
 mmdetection3d/actions) [![codecov](https://codecov.io/gh/open-mmlab/
 mmdetection3d/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
 mmdetection3d) [![license](https://img.shields.io/github/license/open-mmlab/
 mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/master/
-LICENSE) **News**: **v1.1.0rc2** was released in 2/12/2022 The compatibilities
+LICENSE) **News**: **v1.1.0rc3** was released in 7/1/2023 The compatibilities
 of models are broken due to the unification and simplification of coordinate
 systems after v1.0.0rc0. For now, most models are benchmarked with similar
 performance, though few models are still being benchmarked. In the following
 release, we will update all the model checkpoints and benchmarks. See more
 details in the [Changelog](docs/en/notes/changelog.md) and [Changelog-v1.0.x]
 (docs/en/notes/changelog_v1.0.x.md). Documentation: https://
 mmdetection3d.readthedocs.io/ ## Introduction English | [ç®ä½ä¸­æ]
@@ -46,16 +46,16 @@
 -------: | :----------------------------------------------------: | :----------
 -------------------------------: | | VoteNet | 358 | Ã | 77 | Ã | |
 PointPillars-car | 141 | Ã | Ã | 140 | | PointPillars-3class | 107 | 44 | Ã
 | Ã | | SECOND | 40 | 30 | Ã | Ã | | Part-A2 | 17 | 14 | Ã | Ã | Like
 [MMDetection](https://github.com/open-mmlab/mmdetection) and [MMCV](https://
 github.com/open-mmlab/mmcv), MMDetection3D can also be used as a library to
 support different projects on top of it. ## License This project is released
-under the [Apache 2.0 license](LICENSE). ## Changelog **1.1.0rc2** was released
-in 2/12/2022. Please refer to [changelog.md](docs/en/notes/changelog.md) for
+under the [Apache 2.0 license](LICENSE). ## Changelog **1.1.0rc3** was released
+in 7/1/2023. Please refer to [changelog.md](docs/en/notes/changelog.md) for
 details and release history. ## Benchmark and model zoo Results and models are
 available in the [model zoo](docs/en/model_zoo.md).
                                   Components
               Backbones                 Heads                   Features
       * PointNet_(CVPR'2017)     * FreeAnchor_        * Dynamic_Voxelization_
       * PointNet++_                (NeurIPS'2019)       (CoRL'2019)
         (NeurIPS'2017)
```

### Comparing `mmdet3d-1.1.0rc2/README.md` & `mmdet3d-1.1.0rc3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 [![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmdetection3d.readthedocs.io/en/1.1/)
 [![badge](https://github.com/open-mmlab/mmdetection3d/workflows/build/badge.svg)](https://github.com/open-mmlab/mmdetection3d/actions)
 [![codecov](https://codecov.io/gh/open-mmlab/mmdetection3d/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmdetection3d)
 [![license](https://img.shields.io/github/license/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/master/LICENSE)
 
 **News**:
 
-**v1.1.0rc2** was released in 2/12/2022
+**v1.1.0rc3** was released in 7/1/2023
 
 The compatibilities of models are broken due to the unification and simplification of coordinate systems after v1.0.0rc0. For now, most models are benchmarked with similar performance, though few models are still being benchmarked. In the following release, we will update all the model checkpoints and benchmarks. See more details in the [Changelog](docs/en/notes/changelog.md) and [Changelog-v1.0.x](docs/en/notes/changelog_v1.0.x.md).
 
 Documentation: https://mmdetection3d.readthedocs.io/
 
 ## Introduction
 
@@ -74,15 +74,15 @@
 
 ## License
 
 This project is released under the [Apache 2.0 license](LICENSE).
 
 ## Changelog
 
-**1.1.0rc2** was released in 2/12/2022.
+**1.1.0rc3** was released in 7/1/2023.
 
 Please refer to [changelog.md](docs/en/notes/changelog.md) for details and release history.
 
 ## Benchmark and model zoo
 
 Results and models are available in the [model zoo](docs/en/model_zoo.md).
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 [![docs](https://img.shields.io/badge/docs-latest-blue)](https://
 mmdetection3d.readthedocs.io/en/1.1/) [![badge](https://github.com/open-mmlab/
 mmdetection3d/workflows/build/badge.svg)](https://github.com/open-mmlab/
 mmdetection3d/actions) [![codecov](https://codecov.io/gh/open-mmlab/
 mmdetection3d/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
 mmdetection3d) [![license](https://img.shields.io/github/license/open-mmlab/
 mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/master/
-LICENSE) **News**: **v1.1.0rc2** was released in 2/12/2022 The compatibilities
+LICENSE) **News**: **v1.1.0rc3** was released in 7/1/2023 The compatibilities
 of models are broken due to the unification and simplification of coordinate
 systems after v1.0.0rc0. For now, most models are benchmarked with similar
 performance, though few models are still being benchmarked. In the following
 release, we will update all the model checkpoints and benchmarks. See more
 details in the [Changelog](docs/en/notes/changelog.md) and [Changelog-v1.0.x]
 (docs/en/notes/changelog_v1.0.x.md). Documentation: https://
 mmdetection3d.readthedocs.io/ ## Introduction English | [ç®ä½ä¸­æ]
@@ -42,16 +42,16 @@
 -------: | :----------------------------------------------------: | :----------
 -------------------------------: | | VoteNet | 358 | Ã | 77 | Ã | |
 PointPillars-car | 141 | Ã | Ã | 140 | | PointPillars-3class | 107 | 44 | Ã
 | Ã | | SECOND | 40 | 30 | Ã | Ã | | Part-A2 | 17 | 14 | Ã | Ã | Like
 [MMDetection](https://github.com/open-mmlab/mmdetection) and [MMCV](https://
 github.com/open-mmlab/mmcv), MMDetection3D can also be used as a library to
 support different projects on top of it. ## License This project is released
-under the [Apache 2.0 license](LICENSE). ## Changelog **1.1.0rc2** was released
-in 2/12/2022. Please refer to [changelog.md](docs/en/notes/changelog.md) for
+under the [Apache 2.0 license](LICENSE). ## Changelog **1.1.0rc3** was released
+in 7/1/2023. Please refer to [changelog.md](docs/en/notes/changelog.md) for
 details and release history. ## Benchmark and model zoo Results and models are
 available in the [model zoo](docs/en/model_zoo.md).
                                   Components
               Backbones                 Heads                   Features
       * PointNet_(CVPR'2017)     * FreeAnchor_        * Dynamic_Voxelization_
       * PointNet++_                (NeurIPS'2019)       (CoRL'2019)
         (NeurIPS'2017)
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/3dssd/3dssd_4xb4_kitti-3d-car.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/3dssd/3dssd_4xb4_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/3dssd/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/3dssd/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-car.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/kitti-mono3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/kitti-mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/lyft-3d-range100.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/lyft-3d-range100.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/lyft-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/nuim-instance.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/nuim-instance.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/nus-mono3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/nus-mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/s3dis-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/s3dis-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/s3dis-seg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/s3dis-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/scannet-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/scannet-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/scannet-seg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/sunrgbd-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/sunrgbd-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-car.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/waymoD5-fov-mono3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/waymoD5-fov-mono3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv-mono3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv-mono3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/default_runtime.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/default_runtime.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/3dssd.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/3dssd.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/cascade-mask-rcnn_r50_fpn.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/cascade-mask-rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/centerpoint_pillar02_second_secfpn_nus.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/centerpoint_pillar02_second_secfpn_nus.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/centerpoint_voxel01_second_secfpn_nus.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/centerpoint_voxel01_second_secfpn_nus.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/dgcnn.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/dgcnn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/fcaf3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/fcaf3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/fcos3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/fcos3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/groupfree3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/groupfree3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/h3dnet.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/h3dnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/imvotenet.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/imvotenet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/mask-rcnn_r50_fpn.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/mask-rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/multiview_dfm.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/multiview_dfm.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/paconv_ssg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/paconv_ssg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/parta2.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/parta2.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pgd.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pgd.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/point_rcnn.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/point_rcnn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pointnet2_msg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pointnet2_msg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pointnet2_ssg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pointnet2_ssg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_lyft.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_lyft.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_nus.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_nus.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_range100_lyft.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_range100_lyft.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_kitti.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_kitti.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_waymo.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_waymo.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,20 +44,20 @@
         num_classes=3,
         in_channels=384,
         feat_channels=384,
         use_direction_classifier=True,
         anchor_generator=dict(
             type='AlignedAnchor3DRangeGenerator',
             ranges=[[-74.88, -74.88, -0.0345, 74.88, 74.88, -0.0345],
-                    [-74.88, -74.88, -0.1188, 74.88, 74.88, -0.1188],
-                    [-74.88, -74.88, 0, 74.88, 74.88, 0]],
+                    [-74.88, -74.88, 0, 74.88, 74.88, 0],
+                    [-74.88, -74.88, -0.1188, 74.88, 74.88, -0.1188]],
             sizes=[
                 [4.73, 2.08, 1.77],  # car
-                [1.81, 0.84, 1.77],  # cyclist
-                [0.91, 0.84, 1.74]  # pedestrian
+                [0.91, 0.84, 1.74],  # pedestrian
+                [1.81, 0.84, 1.77]  # cyclist
             ],
             rotations=[0, 1.57],
             reshape_out=False),
         diff_rad_by_sin=True,
         dir_offset=-0.7854,  # -pi / 4
         bbox_coder=dict(type='DeltaXYZWLHRBBoxCoder', code_size=7),
         loss_cls=dict(
@@ -78,22 +78,22 @@
                 dict(  # car
                     type='Max3DIoUAssigner',
                     iou_calculator=dict(type='BboxOverlapsNearest3D'),
                     pos_iou_thr=0.55,
                     neg_iou_thr=0.4,
                     min_pos_iou=0.4,
                     ignore_iof_thr=-1),
-                dict(  # cyclist
+                dict(  # pedestrian
                     type='Max3DIoUAssigner',
                     iou_calculator=dict(type='BboxOverlapsNearest3D'),
                     pos_iou_thr=0.5,
                     neg_iou_thr=0.3,
                     min_pos_iou=0.3,
                     ignore_iof_thr=-1),
-                dict(  # pedestrian
+                dict(  # cyclist
                     type='Max3DIoUAssigner',
                     iou_calculator=dict(type='BboxOverlapsNearest3D'),
                     pos_iou_thr=0.5,
                     neg_iou_thr=0.3,
                     min_pos_iou=0.3,
                     ignore_iof_thr=-1),
             ],
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_kitti.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_kitti.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_waymo.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_waymo.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/smoke.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/smoke.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/models/votenet.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/models/votenet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/cosine.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/cosine.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/cyclic-20e.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/cyclic-20e.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/cyclic-40e.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/cyclic-40e.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/mmdet-schedule-1x.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/mmdet-schedule-1x.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/schedule-2x.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/schedule-2x.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/schedule-3x.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/schedule-3x.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-100e.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-100e.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-150e.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-150e.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-200e.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-200e.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-50e.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-50e.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/benchmark/hv_PartA2_secfpn_4x8_cyclic_80e_pcdet_kitti-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/benchmark/hv_PartA2_secfpn_4x8_cyclic_80e_pcdet_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_3x8_100e_det3d_kitti-3d-car.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_3x8_100e_det3d_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_4x8_80e_pcdet_kitti-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_4x8_80e_pcdet_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/benchmark/hv_second_secfpn_4x8_80e_pcdet_kitti-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/benchmark/hv_second_secfpn_4x8_80e_pcdet_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_8xb4-cyclic-20e_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_8xb4-cyclic-20e_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_8xb4-cyclic-20e_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_8xb4-cyclic-20e_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn-circlenms_8xb4-flip-tta-cyclic-20e_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn-circlenms_8xb4-flip-tta-cyclic-20e_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-flip-tta-cyclic-20e_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-flip-tta-cyclic-20e_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-tta-cyclic-20e_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-tta-cyclic-20e_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_8xb4-cyclic-20e_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_8xb4-cyclic-20e_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/centerpoint/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/centerpoint/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_16xb2_waymoD5-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_16xb2_waymoD5-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_centerhead_16xb2_waymoD5-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_centerhead_16xb2_waymoD5-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area1.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area1.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area2.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area2.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area3.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area3.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area4.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area4.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area5.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area5.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area6.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area6.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dgcnn/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dgcnn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dynamic_voxelization/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dynamic_voxelization/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dynamic_voxelization/pointpillars_dv_secfpn_8xb6-160e_kitti-3d-car.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dynamic_voxelization/pointpillars_dv_secfpn_8xb6-160e_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb2-cosine-80e_kitti-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb2-cosine-80e_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb6-80e_kitti-3d-car.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb6-80e_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_s3dis-3d-5class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_s3dis-3d-5class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_scannet-3d-18class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_scannet-3d-18class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_sunrgbd-3d-10class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_sunrgbd-3d-10class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcaf3d/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcaf3d/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcos3d/fcos3d_r101-caffe-dcn_fpn_head-gn_8xb2-1x_nus-mono3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcos3d/fcos3d_r101-caffe-dcn_fpn_head-gn_8xb2-1x_nus-mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/fcos3d/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/fcos3d/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-400mf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-400mf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L12-O256_4xb8_scannet-seg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L12-O256_4xb8_scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L6-O256_4xb8_scannet-seg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L6-O256_4xb8_scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O256_4xb8_scannet-seg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O256_4xb8_scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O512_4xb8_scannet-seg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O512_4xb8_scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/groupfree3d/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/groupfree3d/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/h3dnet/h3dnet_8xb3_scannet-seg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/h3dnet/h3dnet_8xb3_scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/h3dnet/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/h3dnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/imvotenet/imvotenet_faster-rcnn-r50_fpn_4xb2_sunrgbd-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/imvotenet/imvotenet_faster-rcnn-r50_fpn_4xb2_sunrgbd-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/imvotenet/imvotenet_stage2_8xb16_sunrgbd-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/imvotenet/imvotenet_stage2_8xb16_sunrgbd-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/imvotenet/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/imvotenet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_8xb4_kitti-3d-car.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_8xb4_kitti-3d-car.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,16 @@
             loss_weight=1.0),
         loss_bbox=dict(
             type='mmdet.SmoothL1Loss', beta=1.0 / 9.0, loss_weight=2.0),
         loss_dir=dict(
             type='mmdet.CrossEntropyLoss', use_sigmoid=False,
             loss_weight=0.2)),
     n_voxels=[216, 248, 12],
-    anchor_generator=dict(
+    coord_type='LIDAR',
+    prior_generator=dict(
         type='AlignedAnchor3DRangeGenerator',
         ranges=[[-0.16, -39.68, -3.08, 68.96, 39.68, 0.76]],
         rotations=[.0]),
     train_cfg=dict(
         assigner=dict(
             type='Max3DIoUAssigner',
             iou_calculator=dict(type='mmdet3d.BboxOverlapsNearest3D'),
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/imvoxelnet/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/imvoxelnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/monoflex/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/monoflex/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/mvxnet/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/mvxnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/mvxnet/mvxnet_fpn_dv_second_secfpn_8xb2-80e_kitti-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/mvxnet/mvxnet_fpn_dv_second_secfpn_8xb2-80e_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r50_fpn_1x_nuim.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r50_fpn_1x_nuim.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_1x_nuim.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_1x_nuim.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_head-without-semantic_1x_nuim.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_head-without-semantic_1x_nuim.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/htc_x101_64x4d_fpn_dconv_c3-c5_coco-20e-1xb16_nuim.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/htc_x101_64x4d_fpn_dconv_c3-c5_coco-20e-1xb16_nuim.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_1x_nuim.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_1x_nuim.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_1x_nuim.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_1x_nuim.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_20e_nuim.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_20e_nuim.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_coco-2x_1x_nus-2d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_coco-2x_1x_nus-2d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/nuimages/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/nuimages/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/paconv/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/paconv/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/paconv/paconv_ssg-cuda_8xb8-cosine-200e_s3dis-seg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/paconv/paconv_ssg-cuda_8xb8-cosine-200e_s3dis-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/paconv/paconv_ssg_8xb8-cosine-150e_s3dis-seg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/paconv/paconv_ssg_8xb8-cosine-150e_s3dis-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/parta2/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/parta2/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-car.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-1x_nus-mono3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-1x_nus-mono3d.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 _base_ = [
     '../_base_/datasets/nus-mono3d.py', '../_base_/models/pgd.py',
     '../_base_/schedules/mmdet-schedule-1x.py', '../_base_/default_runtime.py'
 ]
 # model settings
 model = dict(
+    data_preprocessor=dict(
+        type='Det3DDataPreprocessor',
+        mean=[103.530, 116.280, 123.675],
+        std=[1.0, 1.0, 1.0],
+        bgr_to_rgb=False,
+        pad_size_divisor=32),
     backbone=dict(
         dcn=dict(type='DCNv2', deform_groups=1, fallback_on_stride=False),
         stage_with_dcn=(False, False, True, True)),
     bbox_head=dict(
         pred_bbox2d=True,
         group_reg_dims=(2, 1, 3, 1, 2,
                         4),  # offset, depth, size, rot, velo, bbox2d
@@ -36,62 +42,61 @@
     # set weight 1.0 for base 7 dims (offset, depth, size, rot)
     # 0.05 for 2-dim velocity and 0.2 for 4-dim 2D distance targets
     train_cfg=dict(code_weight=[
         1.0, 1.0, 0.2, 1.0, 1.0, 1.0, 1.0, 0.05, 0.05, 0.2, 0.2, 0.2, 0.2
     ]),
     test_cfg=dict(nms_pre=1000, nms_thr=0.8, score_thr=0.01, max_per_img=200))
 
-class_names = [
-    'car', 'truck', 'trailer', 'bus', 'construction_vehicle', 'bicycle',
-    'motorcycle', 'pedestrian', 'traffic_cone', 'barrier'
-]
 train_pipeline = [
     dict(type='LoadImageFromFileMono3D'),
     dict(
         type='LoadAnnotations3D',
         with_bbox=True,
         with_label=True,
         with_attr_label=True,
         with_bbox_3d=True,
         with_label_3d=True,
         with_bbox_depth=True),
-    dict(type='Resize', img_scale=(1600, 900), keep_ratio=True),
+    dict(type='mmdet.Resize', scale=(1600, 900), keep_ratio=True),
     dict(type='RandomFlip3D', flip_ratio_bev_horizontal=0.5),
     dict(
         type='Pack3DDetInputs',
         keys=[
             'img', 'gt_bboxes', 'gt_bboxes_labels', 'attr_labels',
-            'gt_bboxes_3d', 'gt_labels_3d', 'centers2d', 'depths'
+            'gt_bboxes_3d', 'gt_labels_3d', 'centers_2d', 'depths'
         ]),
 ]
 test_pipeline = [
     dict(type='LoadImageFromFileMono3D'),
-    dict(
-        type='MultiScaleFlipAug',
-        scale_factor=1.0,
-        flip=False,
-        transforms=[
-            dict(type='RandomFlip3D'),
-        ]),
+    dict(type='mmdet.Resize', scale_factor=1.0),
     dict(type='Pack3DDetInputs', keys=['img']),
 ]
-data = dict(
-    samples_per_gpu=2,
-    workers_per_gpu=2,
-    train=dict(pipeline=train_pipeline),
-    val=dict(pipeline=test_pipeline),
-    test=dict(pipeline=test_pipeline))
+train_dataloader = dict(
+    batch_size=2, num_workers=2, dataset=dict(pipeline=train_pipeline))
+test_dataloader = dict(dataset=dict(pipeline=test_pipeline))
+val_dataloader = dict(dataset=dict(pipeline=test_pipeline))
+
 # optimizer
-optimizer = dict(
-    lr=0.004, paramwise_cfg=dict(bias_lr_mult=2., bias_decay_mult=0.))
-optimizer_config = dict(
-    _delete_=True, grad_clip=dict(max_norm=35, norm_type=2))
+optim_wrapper = dict(
+    optimizer=dict(lr=0.004),
+    paramwise_cfg=dict(bias_lr_mult=2., bias_decay_mult=0.),
+    clip_grad=dict(max_norm=35, norm_type=2))
+
 # learning policy
-lr_config = dict(
-    policy='step',
-    warmup='linear',
-    warmup_iters=500,
-    warmup_ratio=1.0 / 3,
-    step=[8, 11])
-total_epochs = 12
-evaluation = dict(interval=4)
-runner = dict(max_epochs=total_epochs)
+param_scheduler = [
+    dict(
+        type='LinearLR',
+        start_factor=1.0 / 3,
+        by_epoch=False,
+        begin=0,
+        end=500),
+    dict(
+        type='MultiStepLR',
+        begin=0,
+        end=12,
+        by_epoch=True,
+        milestones=[8, 11],
+        gamma=0.1)
+]
+
+train_cfg = dict(max_epochs=12, val_interval=4)
+auto_scale_lr = dict(base_batch_size=32)
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_4xb3-4x_kitti-mono3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_4xb3-4x_kitti-mono3d.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,26 +64,26 @@
     # 0.2 for 16-dim keypoint offsets and 1.0 for 4-dim 2D distance targets
     train_cfg=dict(code_weight=[
         1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 0.2, 0.2, 0.2, 0.2, 0.2, 0.2, 0.2,
         0.2, 0.2, 0.2, 0.2, 0.2, 0.2, 0.2, 0.2, 0.2, 1.0, 1.0, 1.0, 1.0
     ]),
     test_cfg=dict(nms_pre=100, nms_thr=0.05, score_thr=0.001, max_per_img=20))
 
-# file_client_args = dict(backend='disk')
+file_client_args = dict(backend='disk')
 # Uncomment the following if use ceph or other file clients.
 # See https://mmcv.readthedocs.io/en/latest/api.html#mmcv.fileio.FileClient
 # for more details.
-file_client_args = dict(
-    backend='petrel',
-    path_mapping=dict({
-        './data/kitti/':
-        's3://openmmlab/datasets/detection3d/kitti/',
-        'data/kitti/':
-        's3://openmmlab/datasets/detection3d/kitti/'
-    }))
+# file_client_args = dict(
+#     backend='petrel',
+#     path_mapping=dict({
+#         './data/kitti/':
+#         's3://openmmlab/datasets/detection3d/kitti/',
+#         'data/kitti/':
+#         's3://openmmlab/datasets/detection3d/kitti/'
+#     }))
 
 train_pipeline = [
     dict(type='LoadImageFromFileMono3D'),
     dict(
         type='LoadAnnotations3D',
         with_bbox=True,
         with_label=True,
@@ -131,7 +131,8 @@
         end=48,
         by_epoch=True,
         milestones=[32, 44],
         gamma=0.1)
 ]
 
 train_cfg = dict(max_epochs=48, val_interval=2)
+auto_scale_lr = dict(base_batch_size=12)
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-fov-mono3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-fov-mono3d.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,12 +101,12 @@
         type='MultiStepLR',
         begin=0,
         end=24,
         by_epoch=True,
         milestones=[16, 22],
         gamma=0.1)
 ]
-total_epochs = 24
-runner = dict(max_epochs=total_epochs)
+
 train_cfg = dict(type='EpochBasedTrainLoop', max_epochs=24, val_interval=24)
 val_cfg = dict(type='ValLoop')
 test_cfg = dict(type='TestLoop')
+auto_scale_lr = dict(base_batch_size=48)
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-mono3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-mono3d.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,12 +100,12 @@
         type='MultiStepLR',
         begin=0,
         end=24,
         by_epoch=True,
         milestones=[16, 22],
         gamma=0.1)
 ]
-total_epochs = 24
-runner = dict(max_epochs=total_epochs)
+
 train_cfg = dict(type='EpochBasedTrainLoop', max_epochs=24, val_interval=24)
 val_cfg = dict(type='ValLoop')
 test_cfg = dict(type='TestLoop')
+auto_scale_lr = dict(base_batch_size=48)
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-mv-mono3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-mv-mono3d.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,12 +101,12 @@
         type='MultiStepLR',
         begin=0,
         end=24,
         by_epoch=True,
         milestones=[16, 22],
         gamma=0.1)
 ]
-total_epochs = 24
-runner = dict(max_epochs=total_epochs)
+
 train_cfg = dict(type='EpochBasedTrainLoop', max_epochs=24, val_interval=24)
 val_cfg = dict(type='ValLoop')
 test_cfg = dict(type='TestLoop')
+auto_scale_lr = dict(base_batch_size=48)
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/point_rcnn/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/point_rcnn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/point_rcnn/point-rcnn_8xb2_kitti-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/point_rcnn/point-rcnn_8xb2_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg-xyz-only.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg-xyz-only.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-80e_s3dis-seg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-80e_s3dis-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg-xyz-only.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg-xyz-only.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-50e_s3dis-seg.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-50e_s3dis-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-car.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-car.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-car.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d-range100.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d-range100.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pv_rcnn/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pv_rcnn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/pv_rcnn/pv_rcnn_8xb2-80e_kitti-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/pv_rcnn/pv_rcnn_8xb2-80e_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-1.6gf_fpn_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-1.6gf_fpn_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb2-2x_lyft-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb2-2x_lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_range100_8xb2-2x_lyft-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_range100_8xb2-2x_lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb2-2x_lyft-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb2-2x_lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_range100_8xb2-2x_lyft-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_range100_8xb2-2x_lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/sassd/sassd_8xb6-80e_kitti-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/sassd/sassd_8xb6-80e_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/second/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/second/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-80e_kitti-3d-car.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-80e_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/second/second_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-3class.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/second/second_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/smoke/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/smoke/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/smoke/smoke_dla34_dlaneck_gn-all_4xb8-6x_kitti-mono3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/smoke/smoke_dla34_dlaneck_gn-all_4xb8-6x_kitti-mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/ssn/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/ssn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb1-2x_lyft-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb1-2x_lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb2-2x_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb2-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_lyft-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_nus-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/votenet/metafile.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/votenet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/votenet/votenet_8xb16_sunrgbd-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/votenet/votenet_8xb16_sunrgbd-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/configs/votenet/votenet_8xb8_scannet-3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/configs/votenet/votenet_8xb8_scannet-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/model-index.yml` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/model-index.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/analysis_tools/analyze_logs.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/analysis_tools/analyze_logs.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/analysis_tools/benchmark.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/analysis_tools/benchmark.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import time
 
 import torch
 from mmcv import Config
 from mmcv.parallel import MMDataParallel
 from mmengine.runner import load_checkpoint
 
-from mmdet3d.datasets import build_dataset
-from mmdet3d.models import build_detector
+from mmdet3d.registry import DATASETS, MODELS
 from tools.misc.fuse_conv_bn import fuse_module
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description='MMDet benchmark a model')
     parser.add_argument('config', help='test config file path')
     parser.add_argument('checkpoint', help='checkpoint file')
@@ -36,30 +35,30 @@
     if cfg.get('cudnn_benchmark', False):
         torch.backends.cudnn.benchmark = True
     cfg.model.pretrained = None
     cfg.data.test.test_mode = True
 
     # build the dataloader
     # TODO: support multiple images per gpu (only minor changes are needed)
-    dataset = build_dataset(cfg.data.test)
+    dataset = DATASETS.build(cfg.data.test)
 
     # TODO fix this
     def build_dataloader():
         pass
 
     data_loader = build_dataloader(
         dataset,
         samples_per_gpu=1,
         workers_per_gpu=cfg.data.workers_per_gpu,
         dist=False,
         shuffle=False)
 
     # build the model and load checkpoint
     cfg.model.train_cfg = None
-    model = build_detector(cfg.model, test_cfg=cfg.get('test_cfg'))
+    model = MODELS.build(cfg.model, test_cfg=cfg.get('test_cfg'))
     load_checkpoint(model, args.checkpoint, map_location='cpu')
     if args.fuse_conv_bn:
         model = fuse_module(model)
 
     model = MMDataParallel(model, device_ids=[0])
 
     model.eval()
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/analysis_tools/get_flops.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/analysis_tools/get_flops.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/create_data.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/create_data.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/create_data.sh` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/create_data.sh`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/create_gt_database.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/create_gt_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 from mmcv.ops import roi_align
 from mmdet.evaluation import bbox_overlaps
 from mmengine import track_iter_progress
 from pycocotools import mask as maskUtils
 from pycocotools.coco import COCO
 
-from mmdet3d.datasets import build_dataset
+from mmdet3d.registry import DATASETS
 from mmdet3d.structures.ops import box_np_ops as box_np_ops
 
 
 def _poly2mask(mask_ann, img_h, img_w):
     if isinstance(mask_ann, list):
         # polygon -- a single object might consist of multiple parts
         # we merge all parts into one mask rle code
@@ -214,15 +214,15 @@
                 dict(
                     type='LoadAnnotations3D',
                     with_bbox_3d=True,
                     with_label_3d=True,
                     file_client_args=file_client_args)
             ])
 
-    dataset = build_dataset(dataset_cfg)
+    dataset = DATASETS.build(dataset_cfg)
 
     if database_save_path is None:
         database_save_path = osp.join(data_path, f'{info_prefix}_gt_database')
     if db_info_save_path is None:
         db_info_save_path = osp.join(data_path,
                                      f'{info_prefix}_dbinfos_train.pkl')
     mmengine.mkdir_or_exist(database_save_path)
@@ -583,15 +583,15 @@
                     dict(
                         type='LoadAnnotations3D',
                         with_bbox_3d=True,
                         with_label_3d=True,
                         file_client_args=file_client_args)
                 ])
 
-        self.dataset = build_dataset(dataset_cfg)
+        self.dataset = DATASETS.build(dataset_cfg)
         self.pipeline = self.dataset.pipeline
         if self.database_save_path is None:
             self.database_save_path = osp.join(
                 self.data_path, f'{self.info_prefix}_gt_database')
         if self.db_info_save_path is None:
             self.db_info_save_path = osp.join(
                 self.data_path, f'{self.info_prefix}_dbinfos_train.pkl')
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/indoor_converter.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/indoor_converter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/kitti_converter.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/kitti_converter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/kitti_data_utils.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/kitti_data_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/lyft_converter.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/lyft_converter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/lyft_data_fixer.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/lyft_data_fixer.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/nuimage_converter.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/nuimage_converter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/nuscenes_converter.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/nuscenes_converter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/s3dis_data_utils.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/s3dis_data_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/scannet_data_utils.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/scannet_data_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/sunrgbd_data_utils.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/sunrgbd_data_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/update_infos_to_v2.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/update_infos_to_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,16 +298,18 @@
                 'lidar2ego'] = convert_quaternion_to_matrix(
                     ori_sweep['sensor2ego_rotation'],
                     ori_sweep['sensor2ego_translation'])
             temp_lidar_sweep['ego2global'] = convert_quaternion_to_matrix(
                 ori_sweep['ego2global_rotation'],
                 ori_sweep['ego2global_translation'])
             lidar2sensor = np.eye(4)
-            lidar2sensor[:3, :3] = ori_sweep['sensor2lidar_rotation'].T
-            lidar2sensor[:3, 3] = -ori_sweep['sensor2lidar_translation']
+            rot = ori_sweep['sensor2lidar_rotation']
+            trans = ori_sweep['sensor2lidar_translation']
+            lidar2sensor[:3, :3] = rot.T
+            lidar2sensor[:3, 3:4] = -1 * np.matmul(rot.T, trans.reshape(3, 1))
             temp_lidar_sweep['lidar_points'][
                 'lidar2sensor'] = lidar2sensor.astype(np.float32).tolist()
             temp_lidar_sweep['timestamp'] = ori_sweep['timestamp'] / 1e6
             temp_lidar_sweep['lidar_points']['lidar_path'] = ori_sweep[
                 'data_path']
             temp_lidar_sweep['sample_data_token'] = ori_sweep[
                 'sample_data_token']
@@ -324,18 +326,18 @@
             # bc-breaking: Timestamp has divided 1e6 in pkl infos.
             empty_img_info[
                 'timestamp'] = ori_info_dict['cams'][cam]['timestamp'] / 1e6
             empty_img_info['cam2ego'] = convert_quaternion_to_matrix(
                 ori_info_dict['cams'][cam]['sensor2ego_rotation'],
                 ori_info_dict['cams'][cam]['sensor2ego_translation'])
             lidar2sensor = np.eye(4)
-            lidar2sensor[:3, :3] = ori_info_dict['cams'][cam][
-                'sensor2lidar_rotation'].T
-            lidar2sensor[:3, 3] = -ori_info_dict['cams'][cam][
-                'sensor2lidar_translation']
+            rot = ori_info_dict['cams'][cam]['sensor2lidar_rotation']
+            trans = ori_info_dict['cams'][cam]['sensor2lidar_translation']
+            lidar2sensor[:3, :3] = rot.T
+            lidar2sensor[:3, 3:4] = -1 * np.matmul(rot.T, trans.reshape(3, 1))
             empty_img_info['lidar2cam'] = lidar2sensor.astype(
                 np.float32).tolist()
             temp_data_info['images'][cam] = empty_img_info
         num_instances = ori_info_dict['gt_boxes'].shape[0]
         ignore_class_name = set()
         for i in range(num_instances):
             empty_instance = get_empty_instance()
@@ -777,16 +779,18 @@
                 'lidar2ego'] = convert_quaternion_to_matrix(
                     ori_sweep['sensor2ego_rotation'],
                     ori_sweep['sensor2ego_translation'])
             temp_lidar_sweep['ego2global'] = convert_quaternion_to_matrix(
                 ori_sweep['ego2global_rotation'],
                 ori_sweep['ego2global_translation'])
             lidar2sensor = np.eye(4)
-            lidar2sensor[:3, :3] = ori_sweep['sensor2lidar_rotation'].T
-            lidar2sensor[:3, 3] = -ori_sweep['sensor2lidar_translation']
+            rot = ori_sweep['sensor2lidar_rotation']
+            trans = ori_sweep['sensor2lidar_translation']
+            lidar2sensor[:3, :3] = rot.T
+            lidar2sensor[:3, 3:4] = -1 * np.matmul(rot.T, trans.reshape(3, 1))
             temp_lidar_sweep['lidar_points'][
                 'lidar2sensor'] = lidar2sensor.astype(np.float32).tolist()
             # bc-breaking: Timestamp has divided 1e6 in pkl infos.
             temp_lidar_sweep['timestamp'] = ori_sweep['timestamp'] / 1e6
             temp_lidar_sweep['lidar_points']['lidar_path'] = ori_sweep[
                 'data_path']
             temp_lidar_sweep['sample_data_token'] = ori_sweep[
@@ -803,18 +807,18 @@
                 'sample_data_token']
             empty_img_info[
                 'timestamp'] = ori_info_dict['cams'][cam]['timestamp'] / 1e6
             empty_img_info['cam2ego'] = convert_quaternion_to_matrix(
                 ori_info_dict['cams'][cam]['sensor2ego_rotation'],
                 ori_info_dict['cams'][cam]['sensor2ego_translation'])
             lidar2sensor = np.eye(4)
-            lidar2sensor[:3, :3] = ori_info_dict['cams'][cam][
-                'sensor2lidar_rotation'].T
-            lidar2sensor[:3, 3] = -ori_info_dict['cams'][cam][
-                'sensor2lidar_translation']
+            rot = ori_info_dict['cams'][cam]['sensor2lidar_rotation']
+            trans = ori_info_dict['cams'][cam]['sensor2lidar_translation']
+            lidar2sensor[:3, :3] = rot.T
+            lidar2sensor[:3, 3:4] = -1 * np.matmul(rot.T, trans.reshape(3, 1))
             empty_img_info['lidar2cam'] = lidar2sensor.astype(
                 np.float32).tolist()
             temp_data_info['images'][cam] = empty_img_info
         num_instances = ori_info_dict['gt_boxes'].shape[0]
         ignore_class_name = set()
         for i in range(num_instances):
             empty_instance = get_empty_instance()
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/dataset_converters/waymo_converter.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/dataset_converters/waymo_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,18 +309,18 @@
                 id_to_bbox[label.id] = bbox
                 id_to_name[label.id] = name - 1
 
         for obj in frame.laser_labels:
             bounding_box = None
             name = None
             id = obj.id
-            for lidar in self.lidar_list:
-                if id + lidar in id_to_bbox:
-                    bounding_box = id_to_bbox.get(id + lidar)
-                    name = str(id_to_name.get(id + lidar))
+            for proj_cam in self.cam_list:
+                if id + proj_cam in id_to_bbox:
+                    bounding_box = id_to_bbox.get(id + proj_cam)
+                    name = str(id_to_name.get(id + proj_cam))
                     break
 
             # NOTE: the 2D labels do not have strict correspondence with
             # the projected 2D lidar labels
             # e.g.: the projected 2D labels can be in camera 2
             # while the most_visible_camera can have id 4
             if cam_sync:
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/deployment/mmdet3d2torchserve.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/deployment/mmdet3d2torchserve.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/deployment/mmdet3d_handler.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/deployment/mmdet3d_handler.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/deployment/test_torchserver.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/deployment/test_torchserver.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/misc/browse_dataset.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/misc/browse_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/misc/fuse_conv_bn.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/misc/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/misc/print_config.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/misc/print_config.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/misc/visualize_results.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/misc/visualize_results.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
 
 import mmengine
-from mmcv import Config
+from mmengine import Config
 
-from mmdet3d.datasets import build_dataset
+from mmdet3d.registry import DATASETS
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description='MMDet3D visualize the results')
     parser.add_argument('config', help='test config file path')
     parser.add_argument('--result', help='results file in pickle format')
@@ -26,15 +26,15 @@
             not args.result.endswith(('.pkl', '.pickle')):
         raise ValueError('The results file must be a pkl file.')
 
     cfg = Config.fromfile(args.config)
     cfg.data.test.test_mode = True
 
     # build the dataset
-    dataset = build_dataset(cfg.data.test)
+    dataset = DATASETS.build(cfg.data.test)
     results = mmengine.load(args.result)
 
     if getattr(dataset, 'show', None) is not None:
         # data loading pipeline for showing
         eval_pipeline = cfg.get('eval_pipeline', {})
         if eval_pipeline:
             dataset.show(results, args.show_dir, pipeline=eval_pipeline)
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/model_converters/convert_h3dnet_checkpoints.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/model_converters/convert_h3dnet_checkpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import argparse
 import tempfile
 
 import torch
 from mmcv import Config
 from mmengine.runner import load_state_dict
 
-from mmdet3d.models import build_detector
+from mmdet3d.registry import MODELS
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description='MMDet3D upgrade model version(before v0.6.0) of H3DNet')
     parser.add_argument('checkpoint', help='checkpoint file')
     parser.add_argument('--out', help='path of the output checkpoint file')
@@ -99,15 +99,15 @@
     and this tool is used for upgrading checkpoints trained with old versions
     (before v0.6.0) to the latest one.
     """
     args = parse_args()
     checkpoint = torch.load(args.checkpoint)
     cfg = parse_config(checkpoint['meta']['config'])
     # Build the model and load checkpoint
-    model = build_detector(
+    model = MODELS.build(
         cfg.model,
         train_cfg=cfg.get('train_cfg'),
         test_cfg=cfg.get('test_cfg'))
     orig_ckpt = checkpoint['state_dict']
     converted_ckpt = orig_ckpt.copy()
 
     if cfg['dataset_type'] == 'ScanNetDataset':
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/model_converters/convert_votenet_checkpoints.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/model_converters/convert_votenet_checkpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import argparse
 import tempfile
 
 import torch
 from mmengine import Config
 from mmengine.runner import load_state_dict
 
-from mmdet3d.models import build_detector
+from mmdet3d.registry import MODELS
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description='MMDet3D upgrade model version(before v0.6.0) of VoteNet')
     parser.add_argument('checkpoint', help='checkpoint file')
     parser.add_argument('--out', help='path of the output checkpoint file')
@@ -75,15 +75,15 @@
     and this tool is used for upgrading checkpoints trained with old versions
     (before v0.6.0) to the latest one.
     """
     args = parse_args()
     checkpoint = torch.load(args.checkpoint)
     cfg = parse_config(checkpoint['meta']['config'])
     # Build the model and load checkpoint
-    model = build_detector(
+    model = MODELS.build(
         cfg.model,
         train_cfg=cfg.get('train_cfg'),
         test_cfg=cfg.get('test_cfg'))
     orig_ckpt = checkpoint['state_dict']
     converted_ckpt = orig_ckpt.copy()
 
     if cfg['dataset_type'] == 'ScanNetDataset':
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/model_converters/publish_model.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/model_converters/publish_model.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/model_converters/regnet2mmdet.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/model_converters/regnet2mmdet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/slurm_test.sh` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/slurm_test.sh`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/slurm_train.sh` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/slurm_train.sh`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/test.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/test.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,22 @@
         '--show', action='store_true', help='show prediction results')
     parser.add_argument(
         '--show-dir',
         help='directory where painted images will be saved. '
         'If specified, it will be automatically saved '
         'to the work_dir/timestamp/show_dir')
     parser.add_argument(
+        '--task',
+        type=str,
+        choices=[
+            'mono_det', 'multi-view_det', 'lidar_det', 'lidar_seg',
+            'multi-modality_det'
+        ],
+        help='Determine the visualization method depending on the task.')
+    parser.add_argument(
         '--wait-time', type=float, default=2, help='the interval of show (s)')
     parser.add_argument(
         '--cfg-options',
         nargs='+',
         action=DictAction,
         help='override some settings in the used config, the key-value pair '
         'in xxx=yyy format will be merged into config file. If the value to '
@@ -59,14 +67,15 @@
         # Turn on visualization
         visualization_hook['draw'] = True
         if args.show:
             visualization_hook['show'] = True
             visualization_hook['wait_time'] = args.wait_time
         if args.show_dir:
             visualization_hook['test_out_dir'] = args.show_dir
+        visualization_hook['vis_task'] = args.task
     else:
         raise RuntimeError(
             'VisualizationHook must be included in default_hooks.'
             'refer to usage '
             '"visualization=dict(type=\'VisualizationHook\')"')
 
     return cfg
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/train.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/train.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/update_data_coords.py` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/update_data_coords.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/.mim/tools/update_data_coords.sh` & `mmdet3d-1.1.0rc3/mmdet3d/.mim/tools/update_data_coords.sh`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/apis/inference.py` & `mmdet3d-1.1.0rc3/mmdet3d/apis/inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,19 +63,18 @@
 
     convert_SyncBN(config.model)
     config.model.train_cfg = None
     model = MODELS.build(config.model)
 
     if checkpoint is not None:
         checkpoint = load_checkpoint(model, checkpoint, map_location='cpu')
-        dataset_meta = checkpoint['meta'].get('dataset_meta', None)
         # save the dataset_meta in the model for convenience
         if 'dataset_meta' in checkpoint.get('meta', {}):
             # mmdet3d 1.x
-            model.dataset_meta = dataset_meta
+            model.dataset_meta = checkpoint['meta']['dataset_meta']
         elif 'CLASSES' in checkpoint.get('meta', {}):
             # < mmdet3d 1.x
             classes = checkpoint['meta']['CLASSES']
             model.dataset_meta = {'CLASSES': classes}
 
             if 'PALETTE' in checkpoint.get('meta', {}):  # 3D Segmentor
                 model.dataset_meta['PALETTE'] = checkpoint['meta']['PALETTE']
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-from .builder import DATASETS, PIPELINES, build_dataset
 from .dataset_wrappers import CBGSDataset
 from .det3d_dataset import Det3DDataset
 from .kitti_dataset import KittiDataset
 from .lyft_dataset import LyftDataset
 from .nuscenes_dataset import NuScenesDataset
 # yapf: enable
 from .s3dis_dataset import S3DISDataset, S3DISSegDataset
@@ -23,22 +22,20 @@
                          PointsRangeFilter, RandomDropPointsColor,
                          RandomFlip3D, RandomJitterPoints, RandomResize3D,
                          RandomShiftScale, Resize3D, VoxelBasedPointSampler)
 from .utils import get_loading_pipeline
 from .waymo_dataset import WaymoDataset
 
 __all__ = [
-    'KittiDataset', 'DATASETS', 'CBGSDataset',
-    'build_dataset', 'NuScenesDataset', 'LyftDataset',
+    'KittiDataset', 'CBGSDataset', 'NuScenesDataset', 'LyftDataset',
     'ObjectSample', 'RandomFlip3D', 'ObjectNoise', 'GlobalRotScaleTrans',
     'PointShuffle', 'ObjectRangeFilter', 'PointsRangeFilter',
     'LoadPointsFromFile', 'S3DISSegDataset', 'S3DISDataset',
     'NormalizePointsColor', 'IndoorPatchPointSample', 'IndoorPointSample',
     'PointSample', 'LoadAnnotations3D', 'GlobalAlignment', 'SUNRGBDDataset',
     'ScanNetDataset', 'ScanNetSegDataset', 'ScanNetInstanceSegDataset',
     'SemanticKITTIDataset', 'Det3DDataset', 'Seg3DDataset',
     'LoadPointsFromMultiSweeps', 'WaymoDataset', 'BackgroundPointsFilter',
     'VoxelBasedPointSampler', 'get_loading_pipeline', 'RandomDropPointsColor',
     'RandomJitterPoints', 'ObjectNameFilter', 'AffineResize',
-    'RandomShiftScale', 'LoadPointsFromDict', 'PIPELINES',
-    'Resize3D', 'RandomResize3D',
+    'RandomShiftScale', 'LoadPointsFromDict', 'Resize3D', 'RandomResize3D',
 ]
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/convert_utils.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/convert_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,24 +249,25 @@
         loc = ann_rec['location'][np.newaxis, :]
         dim = ann_rec['dimensions'][np.newaxis, :]
         rot = ann_rec['rotation_y'][np.newaxis, np.newaxis]
 
         # transform the center from [0.5, 1.0, 0.5] to [0.5, 0.5, 0.5]
         dst = np.array([0.5, 0.5, 0.5])
         src = np.array([0.5, 1.0, 0.5])
-        loc = loc + dim * (dst - src)
-        loc_3d = np.copy(loc)
-        gt_bbox_3d = np.concatenate([loc, dim, rot], axis=1).astype(np.float32)
+        # gravity center
+        loc_center = loc + dim * (dst - src)
+        gt_bbox_3d = np.concatenate([loc_center, dim, rot],
+                                    axis=1).astype(np.float32)
 
         # Filter out the corners that are not in front of the calibrated
         # sensor.
         corners_3d = box_np_ops.center_to_corner_box3d(
             gt_bbox_3d[:, :3],
             gt_bbox_3d[:, 3:6],
-            gt_bbox_3d[:, 6], [0.5, 0.5, 0.5],
+            gt_bbox_3d[:, 6], (0.5, 0.5, 0.5),
             axis=1)
         corners_3d = corners_3d[0].T  # (1, 8, 3) -> (3, 8)
         in_front = np.argwhere(corners_3d[2, :] > 0).flatten()
         corners_3d = corners_3d[:, in_front]
 
         # Project 3d box to 2d.
         corner_coords = view_points(corners_3d, camera_intrinsic,
@@ -287,20 +288,20 @@
 
         # Generate dictionary record to be included in the .json file.
         repro_rec = generate_record(ann_rec, min_x, min_y, max_x, max_y,
                                     dataset)
 
         # If mono3d=True, add 3D annotations in camera coordinates
         if mono3d and (repro_rec is not None):
+            # use bottom center to represent the bbox_3d
             repro_rec['bbox_3d'] = np.concatenate(
-                [loc_3d, dim, rot],
-                axis=1).astype(np.float32).squeeze().tolist()
+                [loc, dim, rot], axis=1).astype(np.float32).squeeze().tolist()
             repro_rec['velocity'] = -1  # no velocity in KITTI
 
-            center_3d = np.array(loc).reshape([1, 3])
+            center_3d = np.array(loc_center).reshape([1, 3])
             center_2d_with_depth = points_cam2img(
                 center_3d, camera_intrinsic, with_depth=True)
             center_2d_with_depth = center_2d_with_depth.squeeze().tolist()
 
             repro_rec['center_2d'] = center_2d_with_depth[:2]
             repro_rec['depth'] = center_2d_with_depth[2]
             # normalized center2D + depth
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/dataset_wrappers.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/det3d_dataset.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/det3d_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import mmengine
 import numpy as np
 import torch
 from mmengine.dataset import BaseDataset
 from mmengine.logging import print_log
 from terminaltables import AsciiTable
 
-from mmdet3d.datasets import DATASETS
+from mmdet3d.registry import DATASETS
 from mmdet3d.structures import get_box_type
 
 
 @DATASETS.register_module()
 class Det3DDataset(BaseDataset):
     """Base Class of 3D dataset.
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/kitti2d_dataset.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/kitti2d_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/kitti_dataset.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/kitti_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from typing import Callable, List, Union
 
 import numpy as np
 
-from mmdet3d.datasets import DATASETS
+from mmdet3d.registry import DATASETS
 from mmdet3d.structures import CameraInstance3DBoxes
 from .det3d_dataset import Det3DDataset
 
 
 @DATASETS.register_module()
 class KittiDataset(Det3DDataset):
     r"""KITTI Dataset.
@@ -20,31 +20,31 @@
         ann_file (str): Path of annotation file.
         pipeline (List[dict]): Pipeline used for data processing.
             Defaults to [].
         modality (dict): Modality to specify the sensor data used as input.
             Defaults to dict(use_lidar=True).
         default_cam_key (str): The default camera name adopted.
             Defaults to 'CAM2'.
+        load_type (str): Type of loading mode. Defaults to 'frame_based'.
+
+            - 'frame_based': Load all of the instances in the frame.
+            - 'mv_image_based': Load all of the instances in the frame and need
+              to convert to the FOV-based data type to support image-based
+              detector.
+            - 'fov_image_based': Only load the instances inside the default
+              cam, and need to convert to the FOV-based data type to support
+              image-based detector.
         box_type_3d (str): Type of 3D box of this dataset.
             Based on the `box_type_3d`, the dataset will encapsulate the box
             to its original format then converted them to `box_type_3d`.
             Defaults to 'LiDAR' in this dataset. Available options includes:
 
             - 'LiDAR': Box in LiDAR coordinates.
             - 'Depth': Box in depth coordinates, usually for indoor dataset.
             - 'Camera': Box in camera coordinates.
-        load_type (str): Type of loading mode. Defaults to 'frame_based'.
-
-            - 'frame_based': Load all of the instances in the frame.
-            - 'mv_image_based': Load all of the instances in the frame and need
-                to convert to the FOV-based data type to support image-based
-                detector.
-            - 'fov_image_based': Only load the instances inside the default
-                cam, and need to convert to the FOV-based data type to support
-                image-based detector.
         filter_empty_gt (bool): Whether to filter the data with empty GT.
             If it's set to be True, the example with empty annotations after
             data pipeline will be dropped and a random example will be chosen
             in `__getitem__`. Defaults to True.
         test_mode (bool): Whether the dataset is in test mode.
             Defaults to False.
         pcd_limit_range (List[float]): The range of point cloud used to filter
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/lyft_dataset.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/lyft_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/nuscenes_dataset.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/nuscenes_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/s3dis_dataset.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/s3dis_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/scannet_dataset.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/scannet_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/seg3d_dataset.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/seg3d_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/semantickitti_dataset.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/semantickitti_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/sunrgbd_dataset.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/sunrgbd_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/data_augment_utils.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/data_augment_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/dbsampler.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/dbsampler.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/formating.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/formating.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/loading.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/loading.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,39 +528,43 @@
             - 'CAMERA': Points in camera coordinates.
         load_dim (int): The dimension of the loaded points. Defaults to 6.
         use_dim (list[int] | int): Which dimensions of the points to use.
             Defaults to [0, 1, 2]. For KITTI dataset, set use_dim=4
             or use_dim=[0, 1, 2, 3] to use the intensity dimension.
         shift_height (bool): Whether to use shifted height. Defaults to False.
         use_color (bool): Whether to use color features. Defaults to False.
+        norm_intensity (bool): Whether to normlize the intensity. Defaults to
+            False.
         file_client_args (dict): Arguments to instantiate a FileClient.
             See :class:`mmengine.fileio.FileClient` for details.
             Defaults to dict(backend='disk').
     """
 
     def __init__(
         self,
         coord_type: str,
         load_dim: int = 6,
         use_dim: Union[int, List[int]] = [0, 1, 2],
         shift_height: bool = False,
         use_color: bool = False,
+        norm_intensity: bool = False,
         file_client_args: dict = dict(backend='disk')
     ) -> None:
         self.shift_height = shift_height
         self.use_color = use_color
         if isinstance(use_dim, int):
             use_dim = list(range(use_dim))
         assert max(use_dim) < load_dim, \
             f'Expect all used dimensions < {load_dim}, got {use_dim}'
         assert coord_type in ['CAMERA', 'LIDAR', 'DEPTH']
 
         self.coord_type = coord_type
         self.load_dim = load_dim
         self.use_dim = use_dim
+        self.norm_intensity = norm_intensity
         self.file_client_args = file_client_args.copy()
         self.file_client = None
 
     def _load_points(self, pts_filename: str) -> np.ndarray:
         """Private function to load point clouds data.
 
         Args:
@@ -595,14 +599,18 @@
 
                 - points (:obj:`BasePoints`): Point clouds data.
         """
         pts_file_path = results['lidar_points']['lidar_path']
         points = self._load_points(pts_file_path)
         points = points.reshape(-1, self.load_dim)
         points = points[:, self.use_dim]
+        if self.norm_intensity:
+            assert len(self.use_dim) >= 4, \
+                f'When using intensity norm, expect used dimensions >= 4, got {len(self.use_dim)}'  # noqa: E501
+            points[:, 3] = np.tanh(points[:, 3])
         attribute_dims = None
 
         if self.shift_height:
             floor_height = np.percentile(points[:, 2], 0.99)
             height = points[:, 2] - floor_height
             points = np.concatenate(
                 [points[:, :3],
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/test_time_aug.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/transforms/transforms_3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/transforms/transforms_3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,14 +355,15 @@
                  use_ground_plane: bool = False) -> None:
         self.sampler_cfg = db_sampler
         self.sample_2d = sample_2d
         if 'type' not in db_sampler.keys():
             db_sampler['type'] = 'DataBaseSampler'
         self.db_sampler = TRANSFORMS.build(db_sampler)
         self.use_ground_plane = use_ground_plane
+        self.disabled = False
 
     @staticmethod
     def remove_points_in_boxes(points: BasePoints,
                                boxes: np.ndarray) -> np.ndarray:
         """Remove the points in the sampled bounding boxes.
 
         Args:
@@ -383,14 +384,17 @@
             input_dict (dict): Result dict from loading pipeline.
 
         Returns:
             dict: Results after object sampling augmentation,
             'points', 'gt_bboxes_3d', 'gt_labels_3d' keys are updated
             in the result dict.
         """
+        if self.disabled:
+            return input_dict
+
         gt_bboxes_3d = input_dict['gt_bboxes_3d']
         gt_labels_3d = input_dict['gt_labels_3d']
 
         if self.use_ground_plane:
             ground_plane = input_dict.get('plane', None)
             assert ground_plane is not None, '`use_ground_plane` is True ' \
                                              'but find plane is None'
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/utils.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/datasets/waymo_dataset.py` & `mmdet3d-1.1.0rc3/mmdet3d/datasets/waymo_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,28 +152,20 @@
         if 'centers_2d' in ann_info:
             centers_2d = ann_info['centers_2d']
             depths = ann_info['depths']
         else:
             centers_2d = np.zeros((0, 2), dtype=np.float32)
             depths = np.zeros((0), dtype=np.float32)
 
-        if self.load_type in ['fov_image_based', 'mv_image_based']:
-            gt_bboxes_3d = CameraInstance3DBoxes(
-                ann_info['gt_bboxes_3d'],
-                box_dim=ann_info['gt_bboxes_3d'].shape[-1],
-                origin=(0.5, 0.5, 0.5))
-
-        else:
-            # in waymo, lidar2cam = R0_rect @ Tr_velo_to_cam
-            # convert gt_bboxes_3d to velodyne coordinates with `lidar2cam`
-            lidar2cam = np.array(
-                info['images'][self.default_cam_key]['lidar2cam'])
-            gt_bboxes_3d = CameraInstance3DBoxes(
-                ann_info['gt_bboxes_3d']).convert_to(self.box_mode_3d,
-                                                     np.linalg.inv(lidar2cam))
+        # in waymo, lidar2cam = R0_rect @ Tr_velo_to_cam
+        # convert gt_bboxes_3d to velodyne coordinates with `lidar2cam`
+        lidar2cam = np.array(info['images'][self.default_cam_key]['lidar2cam'])
+        gt_bboxes_3d = CameraInstance3DBoxes(
+            ann_info['gt_bboxes_3d']).convert_to(self.box_mode_3d,
+                                                 np.linalg.inv(lidar2cam))
         ann_info['gt_bboxes_3d'] = gt_bboxes_3d
 
         anns_results = dict(
             gt_bboxes_3d=gt_bboxes_3d,
             gt_labels_3d=ann_info['gt_labels_3d'],
             gt_bboxes=gt_bboxes,
             gt_bboxes_labels=gt_bboxes_labels,
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/engine/hooks/benchmark_hook.py` & `mmdet3d-1.1.0rc3/mmdet3d/engine/hooks/benchmark_hook.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/engine/hooks/visualization_hook.py` & `mmdet3d-1.1.0rc3/mmdet3d/engine/hooks/visualization_hook.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,41 +36,44 @@
     Args:
         draw (bool): whether to draw prediction results. If it is False,
             it means that no drawing will be done. Defaults to False.
         interval (int): The interval of visualization. Defaults to 50.
         score_thr (float): The threshold to visualize the bboxes
             and masks. Defaults to 0.3.
         show (bool): Whether to display the drawn image. Default to False.
+        vis_task (str): Visualization task. Defaults to 'mono_det'.
         wait_time (float): The interval of show (s). Defaults to 0.
         test_out_dir (str, optional): directory where painted images
             will be saved in testing process.
         file_client_args (dict): Arguments to instantiate a FileClient.
             See :class:`mmengine.fileio.FileClient` for details.
             Defaults to ``dict(backend='disk')``.
     """
 
     def __init__(self,
                  draw: bool = False,
                  interval: int = 50,
                  score_thr: float = 0.3,
                  show: bool = False,
+                 vis_task: str = 'mono_det',
                  wait_time: float = 0.,
                  test_out_dir: Optional[str] = None,
                  file_client_args: dict = dict(backend='disk')):
         self._visualizer: Visualizer = Visualizer.get_current_instance()
         self.interval = interval
         self.score_thr = score_thr
         self.show = show
         if self.show:
             # No need to think about vis backends.
             self._visualizer._vis_backends = {}
             warnings.warn('The show is True, it means that only '
                           'the prediction results are visualized '
                           'without storing data, so vis_backends '
                           'needs to be excluded.')
+        self.vis_task = vis_task
 
         self.wait_time = wait_time
         self.file_client_args = file_client_args.copy()
         self.file_client = None
         self.draw = draw
         self.test_out_dir = test_out_dir
         self._test_index = 0
@@ -115,14 +118,15 @@
 
         if total_curr_iter % self.interval == 0:
             self._visualizer.add_datasample(
                 'val sample',
                 data_input,
                 data_sample=outputs[0],
                 show=self.show,
+                vis_task=self.vis_task,
                 wait_time=self.wait_time,
                 pred_score_thr=self.score_thr,
                 step=total_curr_iter)
 
     def after_test_iter(self, runner: Runner, batch_idx: int, data_batch: dict,
                         outputs: Sequence[Det3DDataSample]) -> None:
         """Run after every testing iterations.
@@ -169,11 +173,12 @@
                 out_file = osp.join(self.test_out_dir, out_file)
 
             self._visualizer.add_datasample(
                 'test sample',
                 data_input,
                 data_sample=data_sample,
                 show=self.show,
+                vis_task=self.vis_task,
                 wait_time=self.wait_time,
                 pred_score_thr=self.score_thr,
                 out_file=out_file,
                 step=self._test_index)
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/indoor_eval.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/indoor_eval.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/instance_seg_eval.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/instance_seg_eval.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/kitti_utils/eval.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/kitti_utils/eval.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/kitti_utils/rotate_iou.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/kitti_utils/rotate_iou.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/lyft_eval.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/lyft_eval.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/scannet_utils/evaluate_semantic_instance.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/scannet_utils/evaluate_semantic_instance.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/scannet_utils/util_3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/scannet_utils/util_3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/seg_eval.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/seg_eval.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/functional/waymo_utils/prediction_to_waymo.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/functional/waymo_utils/prediction_to_waymo.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/indoor_metric.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/indoor_metric.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/instance_seg_metric.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/instance_seg_metric.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/kitti_metric.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/kitti_metric.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/lyft_metric.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/lyft_metric.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/nuscenes_metric.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/nuscenes_metric.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/seg_metric.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/seg_metric.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/evaluation/metrics/waymo_metric.py` & `mmdet3d-1.1.0rc3/mmdet3d/evaluation/metrics/waymo_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
             submission_prefix=self.submission_prefix,
             classes=self.classes)
 
         metric_dict = {}
         for metric in self.metrics:
             ap_dict = self.waymo_evaluate(
                 pklfile_prefix, metric=metric, logger=logger)
-            metric_dict[metric] = ap_dict
+            metric_dict.update(ap_dict)
         if eval_tmp_dir is not None:
             eval_tmp_dir.cleanup()
 
         if tmp_dir is not None:
             tmp_dir.cleanup()
         return metric_dict
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/backbones/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/backbones/base_pointnet.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/backbones/base_pointnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/backbones/dgcnn.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/backbones/dgcnn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/backbones/dla.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/backbones/dla.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/backbones/mink_resnet.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/backbones/mink_resnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/backbones/multi_backbone.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/backbones/multi_backbone.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import warnings
 
 import torch
 from mmcv.cnn import ConvModule
 from mmengine.model import BaseModule
 from torch import nn as nn
 
-from mmdet3d.models.builder import build_backbone
 from mmdet3d.registry import MODELS
 
 
 @MODELS.register_module()
 class MultiBackbone(BaseModule):
     """MultiBackbone with different configs.
 
@@ -53,15 +52,15 @@
         # Rename the ret_dict with different suffixs.
         self.suffixes = suffixes
 
         out_channels = 0
 
         for backbone_cfg in backbones:
             out_channels += backbone_cfg['fp_channels'][-1][-1]
-            self.backbone_list.append(build_backbone(backbone_cfg))
+            self.backbone_list.append(MODELS.build(backbone_cfg))
 
         # Feature aggregation layers
         if aggregation_mlp_channels is None:
             aggregation_mlp_channels = [
                 out_channels, out_channels // 2,
                 out_channels // len(self.backbone_list)
             ]
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/backbones/nostem_regnet.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/backbones/nostem_regnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/backbones/pointnet2_sa_msg.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/backbones/pointnet2_sa_msg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/backbones/pointnet2_sa_ssg.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/backbones/pointnet2_sa_ssg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/backbones/second.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/backbones/second.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/data_preprocessors/data_preprocessor.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/data_preprocessors/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/data_preprocessors/utils.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/data_preprocessors/utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/decode_heads/decode_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/decode_heads/decode_head.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import torch
 from mmengine.model import BaseModule, normal_init
 from torch import Tensor
 from torch import nn as nn
 
 from mmdet3d.registry import MODELS
 from mmdet3d.structures.det3d_data_sample import SampleList
-from mmdet3d.utils.typing import ConfigType
+from mmdet3d.utils.typing_utils import ConfigType
 
 
 class Base3DDecodeHead(BaseModule, metaclass=ABCMeta):
     """Base class for BaseDecodeHead.
 
     1. The ``init_weights`` method is used to initialize decode_head's
     model parameters. After segmentor initialization, ``init_weights``
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/decode_heads/dgcnn_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/decode_heads/dgcnn_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/decode_heads/paconv_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/decode_heads/paconv_head.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from typing import Tuple
 
 from mmcv.cnn.bricks import ConvModule
 from torch import Tensor
 
 from mmdet3d.registry import MODELS
-from mmdet3d.utils.typing import ConfigType
+from mmdet3d.utils.typing_utils import ConfigType
 from .pointnet2_head import PointNet2Head
 
 
 @MODELS.register_module()
 class PAConvHead(PointNet2Head):
     r"""PAConv decoder head.
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/decode_heads/pointnet2_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/decode_heads/pointnet2_head.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from mmcv.cnn.bricks import ConvModule
 from torch import Tensor
 from torch import nn as nn
 
 from mmdet3d.models.layers import PointFPModule
 from mmdet3d.registry import MODELS
-from mmdet3d.utils.typing import ConfigType
+from mmdet3d.utils.typing_utils import ConfigType
 from .decode_head import Base3DDecodeHead
 
 
 @MODELS.register_module()
 class PointNet2Head(Base3DDecodeHead):
     r"""PointNet2 decoder head.
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 from .base_conv_bbox_head import BaseConvBboxHead
 from .base_mono3d_dense_head import BaseMono3DDenseHead
 from .centerpoint_head import CenterHead
 from .fcaf3d_head import FCAF3DHead
 from .fcos_mono3d_head import FCOSMono3DHead
 from .free_anchor3d_head import FreeAnchor3DHead
 from .groupfree3d_head import GroupFree3DHead
+from .imvoxel_head import ImVoxelHead
 from .monoflex_head import MonoFlexHead
 from .parta2_rpn_head import PartA2RPNHead
 from .pgd_head import PGDHead
 from .point_rpn_head import PointRPNHead
 from .shape_aware_head import ShapeAwareHead
 from .smoke_mono3d_head import SMOKEMono3DHead
 from .ssd_3d_head import SSD3DHead
 from .vote_head import VoteHead
 
 __all__ = [
     'Anchor3DHead', 'FreeAnchor3DHead', 'PartA2RPNHead', 'VoteHead',
     'SSD3DHead', 'BaseConvBboxHead', 'CenterHead', 'ShapeAwareHead',
     'BaseMono3DDenseHead', 'AnchorFreeMono3DHead', 'FCOSMono3DHead',
     'GroupFree3DHead', 'PointRPNHead', 'SMOKEMono3DHead', 'PGDHead',
-    'MonoFlexHead', 'Base3DDenseHead', 'FCAF3DHead'
+    'MonoFlexHead', 'Base3DDenseHead', 'FCAF3DHead', 'ImVoxelHead'
 ]
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/anchor3d_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/anchor3d_head.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from mmdet.models.utils import multi_apply
 from torch import Tensor
 from torch import nn as nn
 
 from mmdet3d.models.task_modules import PseudoSampler
 from mmdet3d.models.test_time_augs import merge_aug_bboxes_3d
 from mmdet3d.registry import MODELS, TASK_UTILS
-from mmdet3d.utils.typing import (ConfigType, InstanceList, OptConfigType,
-                                  OptInstanceList)
+from mmdet3d.utils.typing_utils import (ConfigType, InstanceList,
+                                        OptConfigType, OptInstanceList)
 from .base_3d_dense_head import Base3DDenseHead
 from .train_mixins import AnchorTrainMixin
 
 
 @MODELS.register_module()
 class Anchor3DHead(Base3DDenseHead, AnchorTrainMixin):
     """Anchor-based head for SECOND/PointPillars/MVXNet/PartA2.
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/anchor_free_mono3d_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/anchor_free_mono3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/base_3d_dense_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/base_3d_dense_head.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from mmengine.model import BaseModule, constant_init
 from mmengine.structures import InstanceData
 from torch import Tensor
 
 from mmdet3d.models.layers import box3d_multiclass_nms
 from mmdet3d.structures import limit_period, xywhr2xyxyr
 from mmdet3d.structures.det3d_data_sample import SampleList
-from mmdet3d.utils.typing import InstanceList, OptMultiConfig
+from mmdet3d.utils.typing_utils import InstanceList, OptMultiConfig
 
 
 class Base3DDenseHead(BaseModule, metaclass=ABCMeta):
     """Base class for 3D DenseHeads.
 
     1. The ``init_weights`` method is used to initialize densehead's
     model parameters. After detector initialization, ``init_weights``
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/base_conv_bbox_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/base_conv_bbox_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/base_mono3d_dense_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/base_mono3d_dense_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/centerpoint_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/centerpoint_head.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from mmengine.structures import InstanceData
 from torch import Tensor, nn
 
 from mmdet3d.models.utils import (clip_sigmoid, draw_heatmap_gaussian,
                                   gaussian_radius)
 from mmdet3d.registry import MODELS, TASK_UTILS
 from mmdet3d.structures import Det3DDataSample, xywhr2xyxyr
-from .. import builder
 from ..layers import circle_nms, nms_bev
 
 
 @MODELS.register_module()
 class SeparateHead(BaseModule):
     """SeparateHead for CenterHead.
 
@@ -333,15 +332,15 @@
         self.task_heads = nn.ModuleList()
 
         for num_cls in num_classes:
             heads = copy.deepcopy(common_heads)
             heads.update(dict(heatmap=(num_cls, num_heatmap_convs)))
             separate_head.update(
                 in_channels=share_conv_channel, heads=heads, num_cls=num_cls)
-            self.task_heads.append(builder.build_head(separate_head))
+            self.task_heads.append(MODELS.build(separate_head))
 
     def forward_single(self, x: Tensor) -> dict:
         """Forward function for CenterPoint.
 
         Args:
             x (torch.Tensor): Input feature map with the shape of
                 [B, 512, 128, 128].
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/fcaf3d_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/fcaf3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/fcos_mono3d_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/fcos_mono3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/free_anchor3d_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/free_anchor3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/groupfree3d_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/groupfree3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/monoflex_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/monoflex_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/parta2_rpn_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/parta2_rpn_head.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from mmengine import ConfigDict
 from mmengine.structures import InstanceData
 from torch import Tensor
 
 from mmdet3d.models.layers import nms_bev, nms_normal_bev
 from mmdet3d.registry import MODELS
 from mmdet3d.structures import limit_period, xywhr2xyxyr
-from mmdet3d.utils.typing import InstanceList
+from mmdet3d.utils.typing_utils import InstanceList
 from ...structures.det3d_data_sample import SampleList
 from .anchor3d_head import Anchor3DHead
 
 
 @MODELS.register_module()
 class PartA2RPNHead(Anchor3DHead):
     """RPN head for PartA2.
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/pgd_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/pgd_head.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from torch import Tensor
 from torch import nn as nn
 from torch.nn import functional as F
 
 from mmdet3d.models.layers import box3d_multiclass_nms
 from mmdet3d.registry import MODELS
 from mmdet3d.structures import points_cam2img, points_img2cam, xywhr2xyxyr
-from mmdet3d.utils.typing import (ConfigType, InstanceList, OptConfigType,
-                                  OptInstanceList)
+from mmdet3d.utils.typing_utils import (ConfigType, InstanceList,
+                                        OptConfigType, OptInstanceList)
 from .fcos_mono3d_head import FCOSMono3DHead
 
 
 @MODELS.register_module()
 class PGDHead(FCOSMono3DHead):
     r"""Anchor-free head used in `PGD <https://arxiv.org/abs/2107.14160>`_.
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/point_rpn_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/point_rpn_head.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from mmdet3d.models.layers import nms_bev, nms_normal_bev
 from mmdet3d.registry import MODELS, TASK_UTILS
 from mmdet3d.structures import xywhr2xyxyr
 from mmdet3d.structures.bbox_3d import (BaseInstance3DBoxes,
                                         DepthInstance3DBoxes,
                                         LiDARInstance3DBoxes)
 from mmdet3d.structures.det3d_data_sample import SampleList
-from mmdet3d.utils.typing import InstanceList
+from mmdet3d.utils.typing_utils import InstanceList
 
 
 @MODELS.register_module()
 class PointRPNHead(BaseModule):
     """RPN module for PointRCNN.
 
     Args:
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/shape_aware_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/shape_aware_head.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from torch import Tensor
 from torch import nn as nn
 
 from mmdet3d.models.layers import box3d_multiclass_nms
 from mmdet3d.registry import MODELS
 from mmdet3d.structures import limit_period, xywhr2xyxyr
 from mmdet3d.utils import InstanceList, OptInstanceList
-from ..builder import build_head
 from .anchor3d_head import Anchor3DHead
 
 
 @MODELS.register_module()
 class BaseShapeHead(BaseModule):
     """Base Shape-aware Head in Shape Signature Network.
 
@@ -216,15 +215,15 @@
                 type='BaseShapeHead',
                 num_cls=self.num_classes,
                 num_base_anchors=num_base_anchors,
                 box_code_size=self.box_code_size,
                 in_channels=self.in_channels,
                 shared_conv_channels=task['shared_conv_channels'],
                 shared_conv_strides=task['shared_conv_strides'])
-            self.heads.append(build_head(branch))
+            self.heads.append(MODELS.build(branch))
             cls_ptr += task['num_class']
 
     def forward_single(self, x: Tensor) -> Tuple[Tensor]:
         """Forward function on a single-scale feature map.
 
         Args:
             x (torch.Tensor): Input features.
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/smoke_mono3d_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/smoke_mono3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/ssd_3d_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/ssd_3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/train_mixins.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/train_mixins.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/dense_heads/vote_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/dense_heads/vote_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/base.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 from mmdet.models import BaseDetector
 from mmengine.structures import InstanceData
 
 from mmdet3d.registry import MODELS
 from mmdet3d.structures.det3d_data_sample import (ForwardResults,
                                                   OptSampleList, SampleList)
-from mmdet3d.utils.typing import OptConfigType, OptInstanceList, OptMultiConfig
+from mmdet3d.utils.typing_utils import (OptConfigType, OptInstanceList,
+                                        OptMultiConfig)
 
 
 @MODELS.register_module()
 class Base3DDetector(BaseDetector):
     """Base class for 3D detectors.
 
     Args:
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/centerpoint.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/centerpoint.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/dfm.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/dfm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import torch
 from mmdet.models.detectors import BaseDetector
 
 from mmdet3d.registry import MODELS
 from mmdet3d.structures.ops import bbox3d2result
 from mmdet3d.utils import ConfigType
-from ..builder import build_backbone, build_head, build_neck
 
 
 @MODELS.register_module()
 class DfM(BaseDetector):
     r"""`Monocular 3D Object Detection with Depth from Motion.
         <https://arxiv.org/abs/2207.12988>`_.
 
@@ -51,42 +50,42 @@
                  depth_head_2d=None,
                  depth_head=None,
                  train_cfg=None,
                  test_cfg=None,
                  pretrained=None,
                  init_cfg=None):
         super().__init__(init_cfg=init_cfg)
-        self.backbone = build_backbone(backbone)
-        self.neck = build_neck(neck)
+        self.backbone = MODELS.build(backbone)
+        self.neck = MODELS.build(neck)
         if backbone_stereo is not None:
             backbone_stereo.update(cat_img_feature=self.neck.cat_img_feature)
             backbone_stereo.update(in_sem_channels=self.neck.sem_channels[-1])
-            self.backbone_stereo = build_backbone(backbone_stereo)
+            self.backbone_stereo = MODELS.build(backbone_stereo)
             assert self.neck.cat_img_feature == \
                 self.backbone_stereo.cat_img_feature
             assert self.neck.sem_channels[
                 -1] == self.backbone_stereo.in_sem_channels
         if backbone_3d is not None:
-            self.backbone_3d = build_backbone(backbone_3d)
+            self.backbone_3d = MODELS.build(backbone_3d)
         if neck_3d is not None:
-            self.neck_3d = build_neck(neck_3d)
+            self.neck_3d = MODELS.build(neck_3d)
         if neck_2d is not None:
-            self.neck_2d = build_neck(neck_2d)
+            self.neck_2d = MODELS.build(neck_2d)
         if bbox_head_2d is not None:
-            self.bbox_head_2d = build_head(bbox_head_2d)
+            self.bbox_head_2d = MODELS.build(bbox_head_2d)
         if depth_head_2d is not None:
-            self.depth_head_2d = build_head(depth_head_2d)
+            self.depth_head_2d = MODELS.build(depth_head_2d)
         if depth_head is not None:
-            self.depth_head = build_head(depth_head)
+            self.depth_head = MODELS.build(depth_head)
             self.depth_samples = self.depth_head.depth_samples
         self.train_cfg = train_cfg
         self.test_cfg = test_cfg
         bbox_head_3d.update(train_cfg=train_cfg)
         bbox_head_3d.update(test_cfg=test_cfg)
-        self.bbox_head_3d = build_head(bbox_head_3d)
+        self.bbox_head_3d = MODELS.build(bbox_head_3d)
 
     @property
     def with_backbone_3d(self):
         """Whether the detector has a 3D backbone."""
         return hasattr(self, 'backbone_3d') and self.backbone_3d is not None
 
     @property
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/dynamic_voxelnet.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/dynamic_voxelnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/fcos_mono3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/fcos_mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/groupfree3dnet.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/groupfree3dnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/h3dnet.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/h3dnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/imvotenet.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/imvotenet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/imvoxelnet.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/imvoxelnet.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,30 +3,33 @@
 
 import torch
 from mmengine.structures import InstanceData
 
 from mmdet3d.models.detectors import Base3DDetector
 from mmdet3d.models.layers.fusion_layers.point_fusion import point_sample
 from mmdet3d.registry import MODELS, TASK_UTILS
+from mmdet3d.structures.bbox_3d import get_proj_mat_by_coord_type
 from mmdet3d.structures.det3d_data_sample import SampleList
 from mmdet3d.utils import ConfigType, OptConfigType, OptInstanceList
 
 
 @MODELS.register_module()
 class ImVoxelNet(Base3DDetector):
     r"""`ImVoxelNet <https://arxiv.org/abs/2106.01178>`_.
 
     Args:
         backbone (:obj:`ConfigDict` or dict): The backbone config.
         neck (:obj:`ConfigDict` or dict): The neck config.
         neck_3d (:obj:`ConfigDict` or dict): The 3D neck config.
         bbox_head (:obj:`ConfigDict` or dict): The bbox head config.
+        prior_generator (:obj:`ConfigDict` or dict): The prior points
+            generator config.
         n_voxels (list): Number of voxels along x, y, z axis.
-        anchor_generator (:obj:`ConfigDict` or dict): The anchor generator
-            config.
+        coord_type (str): The type of coordinates of points cloud:
+            'DEPTH', 'LIDAR', or 'CAMERA'.
         train_cfg (:obj:`ConfigDict` or dict, optional): Config dict of
             training hyper-parameters. Defaults to None.
         test_cfg (:obj:`ConfigDict` or dict, optional): Config dict of test
             hyper-parameters. Defaults to None.
         data_preprocessor (dict or ConfigDict, optional): The pre-process
             config of :class:`BaseDataPreprocessor`.  it usually includes,
                 ``pad_size_divisor``, ``pad_value``, ``mean`` and ``std``.
@@ -35,84 +38,93 @@
     """
 
     def __init__(self,
                  backbone: ConfigType,
                  neck: ConfigType,
                  neck_3d: ConfigType,
                  bbox_head: ConfigType,
+                 prior_generator: ConfigType,
                  n_voxels: List,
-                 anchor_generator: ConfigType,
+                 coord_type: str,
                  train_cfg: OptConfigType = None,
                  test_cfg: OptConfigType = None,
                  data_preprocessor: OptConfigType = None,
                  init_cfg: OptConfigType = None):
         super().__init__(
             data_preprocessor=data_preprocessor, init_cfg=init_cfg)
         self.backbone = MODELS.build(backbone)
         self.neck = MODELS.build(neck)
         self.neck_3d = MODELS.build(neck_3d)
         bbox_head.update(train_cfg=train_cfg)
         bbox_head.update(test_cfg=test_cfg)
         self.bbox_head = MODELS.build(bbox_head)
+        self.prior_generator = TASK_UTILS.build(prior_generator)
         self.n_voxels = n_voxels
-        self.anchor_generator = TASK_UTILS.build(anchor_generator)
+        self.coord_type = coord_type
         self.train_cfg = train_cfg
         self.test_cfg = test_cfg
 
     def extract_feat(self, batch_inputs_dict: dict,
                      batch_data_samples: SampleList):
         """Extract 3d features from the backbone -> fpn -> 3d projection.
 
+        -> 3d neck -> bbox_head.
+
         Args:
             batch_inputs_dict (dict): The model input dict which include
                 the 'imgs' key.
 
                     - imgs (torch.Tensor, optional): Image of each sample.
             batch_data_samples (list[:obj:`DetDataSample`]): The batch
                 data samples. It usually includes information such
                 as `gt_instance` or `gt_panoptic_seg` or `gt_sem_seg`.
 
         Returns:
-            torch.Tensor: of shape (N, C_out, N_x, N_y, N_z)
+            Tuple:
+            - torch.Tensor: Features of shape (N, C_out, N_x, N_y, N_z).
+            - torch.Tensor: Valid mask of shape (N, 1, N_x, N_y, N_z).
         """
         img = batch_inputs_dict['imgs']
         batch_img_metas = [
             data_samples.metainfo for data_samples in batch_data_samples
         ]
         x = self.backbone(img)
         x = self.neck(x)[0]
-        points = self.anchor_generator.grid_anchors(
-            [self.n_voxels[::-1]], device=img.device)[0][:, :3]
-        volumes = []
+        points = self.prior_generator.grid_anchors([self.n_voxels[::-1]],
+                                                   device=img.device)[0][:, :3]
+        volumes, valid_preds = [], []
         for feature, img_meta in zip(x, batch_img_metas):
             img_scale_factor = (
                 points.new_tensor(img_meta['scale_factor'][:2])
                 if 'scale_factor' in img_meta.keys() else 1)
             img_flip = img_meta['flip'] if 'flip' in img_meta.keys() else False
             img_crop_offset = (
                 points.new_tensor(img_meta['img_crop_offset'])
                 if 'img_crop_offset' in img_meta.keys() else 0)
-            lidar2img = points.new_tensor(img_meta['lidar2img'])
+            proj_mat = points.new_tensor(
+                get_proj_mat_by_coord_type(img_meta, self.coord_type))
             volume = point_sample(
                 img_meta,
                 img_features=feature[None, ...],
                 points=points,
-                proj_mat=lidar2img,
-                coord_type='LIDAR',
+                proj_mat=points.new_tensor(proj_mat),
+                coord_type=self.coord_type,
                 img_scale_factor=img_scale_factor,
                 img_crop_offset=img_crop_offset,
                 img_flip=img_flip,
                 img_pad_shape=img.shape[-2:],
                 img_shape=img_meta['img_shape'][:2],
                 aligned=False)
             volumes.append(
                 volume.reshape(self.n_voxels[::-1] + [-1]).permute(3, 2, 1, 0))
+            valid_preds.append(
+                ~torch.all(volumes[-1] == 0, dim=0, keepdim=True))
         x = torch.stack(volumes)
         x = self.neck_3d(x)
-        return x
+        return x, torch.stack(valid_preds).float()
 
     def loss(self, batch_inputs_dict: dict, batch_data_samples: SampleList,
              **kwargs) -> Union[dict, list]:
         """Calculate losses from a batch of inputs and data samples.
 
         Args:
             batch_inputs_dict (dict): The model input dict which include
@@ -122,16 +134,20 @@
             batch_data_samples (list[:obj:`DetDataSample`]): The batch
                 data samples. It usually includes information such
                 as `gt_instance` or `gt_panoptic_seg` or `gt_sem_seg`.
 
         Returns:
             dict: A dictionary of loss components.
         """
-
-        x = self.extract_feat(batch_inputs_dict, batch_data_samples)
+        x, valid_preds = self.extract_feat(batch_inputs_dict,
+                                           batch_data_samples)
+        # For indoor datasets ImVoxelNet uses ImVoxelHead that handles
+        # mask of visible voxels.
+        if self.coord_type == 'DEPTH':
+            x += (valid_preds, )
         losses = self.bbox_head.loss(x, batch_data_samples, **kwargs)
         return losses
 
     def predict(self, batch_inputs_dict: dict, batch_data_samples: SampleList,
                 **kwargs) -> SampleList:
         """Predict results from a batch of inputs and data samples with post-
         processing.
@@ -155,16 +171,22 @@
                 - scores_3d (Tensor): Classification scores, has a shape
                     (num_instance, )
                 - labels_3d (Tensor): Labels of bboxes, has a shape
                     (num_instances, ).
                 - bboxes_3d (Tensor): Contains a tensor with shape
                     (num_instances, C) where C >=7.
         """
-        x = self.extract_feat(batch_inputs_dict, batch_data_samples)
-        results_list = self.bbox_head.predict(x, batch_data_samples, **kwargs)
+        x, valid_preds = self.extract_feat(batch_inputs_dict,
+                                           batch_data_samples)
+        # For indoor datasets ImVoxelNet uses ImVoxelHead that handles
+        # mask of visible voxels.
+        if self.coord_type == 'DEPTH':
+            x += (valid_preds, )
+        results_list = \
+            self.bbox_head.predict(x, batch_data_samples, **kwargs)
         predictions = self.add_pred_to_datasample(batch_data_samples,
                                                   results_list)
         return predictions
 
     def _forward(self, batch_inputs_dict: dict, batch_data_samples: SampleList,
                  *args, **kwargs) -> Tuple[List[torch.Tensor]]:
         """Network forward process. Usually includes backbone, neck and head
@@ -178,15 +200,20 @@
             batch_data_samples (List[:obj:`Det3DDataSample`]): The Data
                 Samples. It usually includes information such as
                 `gt_instance_3d`, `gt_panoptic_seg_3d` and `gt_sem_seg_3d`.
 
         Returns:
             tuple[list]: A tuple of features from ``bbox_head`` forward.
         """
-        x = self.extract_feat(batch_inputs_dict, batch_data_samples)
+        x, valid_preds = self.extract_feat(batch_inputs_dict,
+                                           batch_data_samples)
+        # For indoor datasets ImVoxelNet uses ImVoxelHead that handles
+        # mask of visible voxels.
+        if self.coord_type == 'DEPTH':
+            x += (valid_preds, )
         results = self.bbox_head.forward(x)
         return results
 
     def convert_to_datasample(
         self,
         data_samples: SampleList,
         data_instances_3d: OptInstanceList = None,
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/mink_single_stage.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/mink_single_stage.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/multiview_dfm.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/multiview_dfm.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/mvx_faster_rcnn.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/mvx_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/mvx_two_stage.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/mvx_two_stage.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/parta2.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/parta2.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/point_rcnn.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/point_rcnn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/pv_rcnn.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/pv_rcnn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/sassd.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/sassd.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/single_stage.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/single_stage.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/single_stage_mono3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/single_stage_mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/smoke_mono3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/smoke_mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/ssd3dnet.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/ssd3dnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/two_stage.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/two_stage.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/votenet.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/votenet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/detectors/voxelnet.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/detectors/voxelnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/box3d_nms.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/box3d_nms.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/dgcnn_modules/dgcnn_fa_module.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/dgcnn_modules/dgcnn_fa_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/dgcnn_modules/dgcnn_fp_module.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/dgcnn_modules/dgcnn_fp_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/dgcnn_modules/dgcnn_gf_module.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/dgcnn_modules/dgcnn_gf_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/edge_fusion_module.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/edge_fusion_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/fusion_layers/coord_transform.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/fusion_layers/coord_transform.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/fusion_layers/point_fusion.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/fusion_layers/point_fusion.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/fusion_layers/vote_fusion.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/fusion_layers/vote_fusion.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/mlp.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/norm.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/norm.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/paconv/paconv.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/paconv/paconv.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/paconv/utils.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/paconv/utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/pointnet_modules/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/pointnet_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/pointnet_modules/builder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/pointnet_modules/builder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/pointnet_modules/paconv_sa_module.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/pointnet_modules/paconv_sa_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/pointnet_modules/point_fp_module.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/pointnet_modules/point_fp_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/pointnet_modules/point_sa_module.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/pointnet_modules/point_sa_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/pointnet_modules/stack_point_sa_module.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/pointnet_modules/stack_point_sa_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/sparse_block.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/sparse_block.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/spconv/overwrite_spconv/write_spconv2.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/spconv/overwrite_spconv/write_spconv2.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/transformer.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/layers/vote_module.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/layers/vote_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/losses/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/losses/axis_aligned_iou_loss.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/losses/axis_aligned_iou_loss.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/losses/chamfer_distance.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/losses/chamfer_distance.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/losses/multibin_loss.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/losses/multibin_loss.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/losses/paconv_regularization_loss.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/losses/paconv_regularization_loss.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/losses/rotated_iou_loss.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/losses/rotated_iou_loss.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/losses/uncertain_smooth_l1_loss.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/losses/uncertain_smooth_l1_loss.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/middle_encoders/pillar_scatter.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/middle_encoders/pillar_scatter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/middle_encoders/sparse_encoder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/middle_encoders/sparse_encoder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/middle_encoders/sparse_unet.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/middle_encoders/sparse_unet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/middle_encoders/voxel_set_abstraction.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/middle_encoders/voxel_set_abstraction.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/necks/dla_neck.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/necks/dla_neck.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/necks/pointnet2_fp_neck.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/necks/pointnet2_fp_neck.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/necks/second_fpn.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/necks/second_fpn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/base_3droi_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/base_3droi_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/bbox_heads/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/bbox_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/bbox_heads/h3d_bbox_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/bbox_heads/h3d_bbox_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/bbox_heads/parta2_bbox_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/bbox_heads/parta2_bbox_head.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 from mmdet.models.utils import multi_apply
 from mmengine.model import normal_init
 from mmengine.structures import InstanceData
 from torch import Tensor
 
 from mmdet3d.models import make_sparse_convmodule
 from mmdet3d.models.layers.spconv import IS_SPCONV2_AVAILABLE
-from mmdet3d.utils.typing import InstanceList
+from mmdet3d.utils.typing_utils import InstanceList
 
 if IS_SPCONV2_AVAILABLE:
     from spconv.pytorch import (SparseConvTensor, SparseMaxPool3d,
                                 SparseSequential)
 else:
     from mmcv.ops import SparseConvTensor, SparseMaxPool3d, SparseSequential
 
 from mmengine.model import BaseModule
 from torch import nn as nn
 
 from mmdet3d.models.layers import nms_bev, nms_normal_bev
 from mmdet3d.registry import MODELS, TASK_UTILS
 from mmdet3d.structures.bbox_3d import (LiDARInstance3DBoxes,
                                         rotation_3d_in_axis, xywhr2xyxyr)
-from mmdet3d.utils.typing import SamplingResultList
+from mmdet3d.utils.typing_utils import SamplingResultList
 
 
 @MODELS.register_module()
 class PartA2BboxHead(BaseModule):
     """PartA2 RoI head.
 
     Args:
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/bbox_heads/point_rcnn_bbox_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/bbox_heads/point_rcnn_bbox_head.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from torch import Tensor
 
 from mmdet3d.models.layers import nms_bev, nms_normal_bev
 from mmdet3d.models.layers.pointnet_modules import build_sa_module
 from mmdet3d.registry import MODELS, TASK_UTILS
 from mmdet3d.structures.bbox_3d import (LiDARInstance3DBoxes,
                                         rotation_3d_in_axis, xywhr2xyxyr)
-from mmdet3d.utils.typing import InstanceList, SamplingResultList
+from mmdet3d.utils.typing_utils import InstanceList, SamplingResultList
 
 
 @MODELS.register_module()
 class PointRCNNBboxHead(BaseModule):
     """PointRCNN RoI Bbox head.
 
     Args:
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/bbox_heads/pv_rcnn_bbox_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/bbox_heads/pv_rcnn_bbox_head.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from mmcv.cnn import ConvModule
 from mmdet.models.task_modules.samplers import SamplingResult
 from mmdet.models.utils import multi_apply
 from mmengine.model import BaseModule
 from mmengine.structures import InstanceData
 from torch import nn as nn
 
-from mmdet3d.models.builder import build_loss
 from mmdet3d.models.layers import nms_bev, nms_normal_bev
 from mmdet3d.registry import MODELS, TASK_UTILS
 from mmdet3d.structures.bbox_3d import (LiDARInstance3DBoxes,
                                         rotation_3d_in_axis, xywhr2xyxyr)
 from mmdet3d.utils import InstanceList
 
 
@@ -72,16 +71,16 @@
     ) -> None:
         super(PVRCNNBBoxHead, self).__init__(init_cfg=init_cfg)
         self.init_cfg = init_cfg
         self.num_classes = num_classes
         self.with_corner_loss = with_corner_loss
         self.class_agnostic = class_agnostic
         self.bbox_coder = TASK_UTILS.build(bbox_coder)
-        self.loss_bbox = build_loss(loss_bbox)
-        self.loss_cls = build_loss(loss_cls)
+        self.loss_bbox = MODELS.build(loss_bbox)
+        self.loss_cls = MODELS.build(loss_cls)
         self.use_sigmoid_cls = loss_cls.get('use_sigmoid', False)
 
         cls_out_channels = 1 if class_agnostic else num_classes
         self.reg_out_channels = self.bbox_coder.code_size * cls_out_channels
         if self.use_sigmoid_cls:
             self.cls_out_channels = cls_out_channels
         else:
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/h3d_roi_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/h3d_roi_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/mask_heads/foreground_segmentation_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/mask_heads/foreground_segmentation_head.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import torch
 from mmcv.cnn.bricks import build_norm_layer
 from mmdet.models.utils import multi_apply
 from mmengine.model import BaseModule
 from mmengine.structures import InstanceData
 from torch import nn as nn
 
-from mmdet3d.models.builder import build_loss
 from mmdet3d.registry import MODELS
 from mmdet3d.utils import InstanceList
 
 
 @MODELS.register_module()
 class ForegroundSegmentationHead(BaseModule):
     """Foreground segmentation head.
@@ -68,15 +67,15 @@
                 nn.ReLU()
             ])
             cin = mlp
         mlps_layers.append(nn.Linear(cin, self.out_channels, bias=True))
 
         self.seg_cls_layer = nn.Sequential(*mlps_layers)
 
-        self.loss_seg = build_loss(loss_seg)
+        self.loss_seg = MODELS.build(loss_seg)
 
     def forward(self, feats: torch.Tensor) -> dict:
         """Forward head.
 
         Args:
             feats (torch.Tensor): Point-wise features.
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/mask_heads/pointwise_semantic_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/mask_heads/pointwise_semantic_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/mask_heads/primitive_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/mask_heads/primitive_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/part_aggregation_roi_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/part_aggregation_roi_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/point_rcnn_roi_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/point_rcnn_roi_head.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import torch
 from mmdet.models.task_modules import AssignResult
 from torch import Tensor
 from torch.nn import functional as F
 
 from mmdet3d.registry import MODELS, TASK_UTILS
 from mmdet3d.structures import bbox3d2roi
-from mmdet3d.utils.typing import InstanceList, SampleList
+from mmdet3d.utils.typing_utils import InstanceList, SampleList
 from .base_3droi_head import Base3DRoIHead
 
 
 @MODELS.register_module()
 class PointRCNNRoIHead(Base3DRoIHead):
     """RoI head for PointRCNN.
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/pv_rcnn_roi_head.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/pv_rcnn_roi_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/roi_extractors/batch_roigridpoint_extractor.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/roi_extractors/batch_roigridpoint_extractor.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/roi_extractors/single_roiaware_extractor.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/roi_extractors/single_roiaware_extractor.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/roi_heads/roi_extractors/single_roipoint_extractor.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/roi_heads/roi_extractors/single_roipoint_extractor.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/segmentors/base.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/segmentors/base.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/segmentors/encoder_decoder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/segmentors/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/anchor/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/anchor/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/anchor/anchor_3d_generator.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/anchor/anchor_3d_generator.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/anchor/builder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/anchor/builder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/assigners/max_3d_iou_assigner.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/assigners/max_3d_iou_assigner.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/builder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/builder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/anchor_free_bbox_coder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/anchor_free_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/centerpoint_bbox_coders.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/centerpoint_bbox_coders.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/delta_xyzwhlr_bbox_coder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/delta_xyzwhlr_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/fcos3d_bbox_coder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/fcos3d_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/groupfree3d_bbox_coder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/groupfree3d_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/monoflex_bbox_coder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/monoflex_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/partial_bin_based_bbox_coder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/partial_bin_based_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/pgd_bbox_coder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/pgd_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/point_xyzwhlr_bbox_coder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/point_xyzwhlr_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/coders/smoke_bbox_coder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/coders/smoke_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/samplers/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/samplers/iou_neg_piecewise_sampler.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/samplers/iou_neg_piecewise_sampler.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/samplers/pseudosample.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/samplers/pseudosample.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/task_modules/voxel/voxel_generator.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/task_modules/voxel/voxel_generator.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/test_time_augs/merge_augs.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/test_time_augs/merge_augs.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/utils/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/utils/edge_indices.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/utils/edge_indices.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/utils/gaussian.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/utils/gaussian.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/utils/gen_keypoints.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/utils/gen_keypoints.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/utils/handle_objs.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/utils/handle_objs.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/voxel_encoders/pillar_encoder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/voxel_encoders/pillar_encoder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/voxel_encoders/utils.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/voxel_encoders/utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/models/voxel_encoders/voxel_encoder.py` & `mmdet3d-1.1.0rc3/mmdet3d/models/voxel_encoders/voxel_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import torch
 from mmcv.cnn import build_norm_layer
 from mmcv.ops import DynamicScatter
 from torch import Tensor, nn
 
 from mmdet3d.registry import MODELS
-from .. import builder
 from .utils import VFELayer, get_paddings_indicator
 
 
 @MODELS.register_module()
 class HardSimpleVFE(nn.Module):
     """Simple voxel feature encoder used in SECOND.
 
@@ -168,15 +167,15 @@
         self.num_vfe = len(vfe_layers)
         self.vfe_scatter = DynamicScatter(voxel_size, point_cloud_range,
                                           (mode != 'max'))
         self.cluster_scatter = DynamicScatter(
             voxel_size, point_cloud_range, average_points=True)
         self.fusion_layer = None
         if fusion_layer is not None:
-            self.fusion_layer = builder.build_fusion_layer(fusion_layer)
+            self.fusion_layer = MODELS.build(fusion_layer)
 
     def map_voxel_center_to_point(self, pts_coors, voxel_mean, voxel_coors):
         """Map voxel features to its corresponding points.
 
         Args:
             pts_coors (torch.Tensor): Voxel coordinate of each point.
             voxel_mean (torch.Tensor): Voxel features to be mapped.
@@ -377,15 +376,15 @@
                     max_out=max_out,
                     cat_max=cat_max))
             self.vfe_layers = nn.ModuleList(vfe_layers)
         self.num_vfe = len(vfe_layers)
 
         self.fusion_layer = None
         if fusion_layer is not None:
-            self.fusion_layer = builder.build_fusion_layer(fusion_layer)
+            self.fusion_layer = MODELS.build(fusion_layer)
 
     def forward(self,
                 features,
                 num_points,
                 coors,
                 img_feats=None,
                 img_metas=None,
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/registry.py` & `mmdet3d-1.1.0rc3/mmdet3d/registry.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/base_box3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/base_box3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -459,19 +459,25 @@
         cols = len(boxes2)
         if rows * cols == 0:
             return boxes1.tensor.new(rows, cols)
 
         # height overlap
         overlaps_h = cls.height_overlaps(boxes1, boxes2)
 
+        # Restrict the min values of W and H to avoid memory overflow in
+        # ``box_iou_rotated``.
+        boxes1_bev, boxes2_bev = boxes1.bev, boxes2.bev
+        boxes1_bev[:, 2:4] = boxes1_bev[:, 2:4].clamp(min=1e-4)
+        boxes2_bev[:, 2:4] = boxes2.bev[:, 2:4].clamp(min=1e-4)
+
         # bev overlap
-        iou2d = box_iou_rotated(boxes1.bev, boxes2.bev)
-        areas1 = (boxes1.bev[:, 2] * boxes1.bev[:, 3]).unsqueeze(1).expand(
+        iou2d = box_iou_rotated(boxes1_bev, boxes2_bev)
+        areas1 = (boxes1_bev[:, 2] * boxes1_bev[:, 3]).unsqueeze(1).expand(
             rows, cols)
-        areas2 = (boxes2.bev[:, 2] * boxes2.bev[:, 3]).unsqueeze(0).expand(
+        areas2 = (boxes2_bev[:, 2] * boxes2_bev[:, 3]).unsqueeze(0).expand(
             rows, cols)
         overlaps_bev = iou2d * (areas1 + areas2) / (1 + iou2d)
 
         # 3d overlaps
         overlaps_3d = overlaps_bev.to(boxes1.device) * overlaps_h
 
         volume1 = boxes1.volume.view(-1, 1)
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/box_3d_mode.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/box_3d_mode.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/cam_box3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/cam_box3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/coord_3d_mode.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/coord_3d_mode.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/depth_box3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/depth_box3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/lidar_box3d.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/lidar_box3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/bbox_3d/utils.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/bbox_3d/utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/det3d_data_sample.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/det3d_data_sample.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/ops/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/ops/box_np_ops.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/ops/box_np_ops.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/ops/iou3d_calculator.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/ops/iou3d_calculator.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/ops/transforms.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/ops/transforms.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/point_data.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/point_data.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/points/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/points/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/points/base_points.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/points/base_points.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/points/cam_points.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/points/cam_points.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/points/depth_points.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/points/depth_points.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/structures/points/lidar_points.py` & `mmdet3d-1.1.0rc3/mmdet3d/structures/points/lidar_points.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/testing/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/testing/data_utils.py` & `mmdet3d-1.1.0rc3/mmdet3d/testing/data_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/testing/model_utils.py` & `mmdet3d-1.1.0rc3/mmdet3d/testing/model_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/utils/__init__.py` & `mmdet3d-1.1.0rc3/mmdet3d/utils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .array_converter import ArrayConverter, array_converter
 from .collect_env import collect_env
 from .compat_cfg import compat_cfg
 from .misc import replace_ceph_backend
 from .setup_env import register_all_modules, setup_multi_processes
-from .typing import (ConfigType, InstanceList, MultiConfig, OptConfigType,
-                     OptInstanceList, OptMultiConfig, OptSamplingResultList)
+from .typing_utils import (ConfigType, InstanceList, MultiConfig,
+                           OptConfigType, OptInstanceList, OptMultiConfig,
+                           OptSamplingResultList)
 
 __all__ = [
     'collect_env', 'setup_multi_processes', 'compat_cfg',
     'register_all_modules', 'array_converter', 'ArrayConverter', 'ConfigType',
     'OptConfigType', 'MultiConfig', 'OptMultiConfig', 'InstanceList',
     'OptInstanceList', 'OptSamplingResultList', 'replace_ceph_backend'
 ]
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/utils/array_converter.py` & `mmdet3d-1.1.0rc3/mmdet3d/utils/array_converter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/utils/collect_env.py` & `mmdet3d-1.1.0rc3/mmdet3d/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/utils/compat_cfg.py` & `mmdet3d-1.1.0rc3/mmdet3d/utils/compat_cfg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/utils/misc.py` & `mmdet3d-1.1.0rc3/mmdet3d/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/utils/setup_env.py` & `mmdet3d-1.1.0rc3/mmdet3d/utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/utils/typing.py` & `mmdet3d-1.1.0rc3/mmdet3d/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/version.py` & `mmdet3d-1.1.0rc3/mmdet3d/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) Open-MMLab. All rights reserved.
 
-__version__ = '1.1.0rc2'
+__version__ = '1.1.0rc3'
 short_version = __version__
 
 
 def parse_version_info(version_str):
     """Parse a version string into a tuple.
 
     Args:
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/visualization/local_visualizer.py` & `mmdet3d-1.1.0rc3/mmdet3d/visualization/local_visualizer.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d/visualization/vis_utils.py` & `mmdet3d-1.1.0rc3/mmdet3d/visualization/vis_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/mmdet3d.egg-info/PKG-INFO` & `mmdet3d-1.1.0rc3/mmdet3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmdet3d
-Version: 1.1.0rc2
+Version: 1.1.0rc3
 Summary: OpenMMLab's next-generation platformfor general 3D object detection.
 Home-page: https://github.com/open-mmlab/mmdetection3d
 Author: MMDetection3D Contributors
 Author-email: zwwdev@gmail.com
 License: Apache License 2.0
 Description: <div align="center">
           <img src="resources/mmdet3d-logo.png" width="600"/>
@@ -30,15 +30,15 @@
         [![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmdetection3d.readthedocs.io/en/1.1/)
         [![badge](https://github.com/open-mmlab/mmdetection3d/workflows/build/badge.svg)](https://github.com/open-mmlab/mmdetection3d/actions)
         [![codecov](https://codecov.io/gh/open-mmlab/mmdetection3d/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmdetection3d)
         [![license](https://img.shields.io/github/license/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/master/LICENSE)
         
         **News**:
         
-        **v1.1.0rc2** was released in 2/12/2022
+        **v1.1.0rc3** was released in 7/1/2023
         
         The compatibilities of models are broken due to the unification and simplification of coordinate systems after v1.0.0rc0. For now, most models are benchmarked with similar performance, though few models are still being benchmarked. In the following release, we will update all the model checkpoints and benchmarks. See more details in the [Changelog](docs/en/notes/changelog.md) and [Changelog-v1.0.x](docs/en/notes/changelog_v1.0.x.md).
         
         Documentation: https://mmdetection3d.readthedocs.io/
         
         ## Introduction
         
@@ -82,15 +82,15 @@
         
         ## License
         
         This project is released under the [Apache 2.0 license](LICENSE).
         
         ## Changelog
         
-        **1.1.0rc2** was released in 2/12/2022.
+        **1.1.0rc3** was released in 7/1/2023.
         
         Please refer to [changelog.md](docs/en/notes/changelog.md) for details and release history.
         
         ## Benchmark and model zoo
         
         Results and models are available in the [model zoo](docs/en/model_zoo.md).
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: mmdet3d Version: 1.1.0rc2 Summary: OpenMMLab's
+Metadata-Version: 2.1 Name: mmdet3d Version: 1.1.0rc3 Summary: OpenMMLab's
 next-generation platformfor general 3D object detection. Home-page: https://
 github.com/open-mmlab/mmdetection3d Author: MMDetection3D Contributors Author-
 email: zwwdev@gmail.com License: Apache License 2.0 Description:
                          [resources/mmdet3d-logo.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
 [![docs](https://img.shields.io/badge/docs-latest-blue)](https://
 mmdetection3d.readthedocs.io/en/1.1/) [![badge](https://github.com/open-mmlab/
 mmdetection3d/workflows/build/badge.svg)](https://github.com/open-mmlab/
 mmdetection3d/actions) [![codecov](https://codecov.io/gh/open-mmlab/
 mmdetection3d/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
 mmdetection3d) [![license](https://img.shields.io/github/license/open-mmlab/
 mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/master/
-LICENSE) **News**: **v1.1.0rc2** was released in 2/12/2022 The compatibilities
+LICENSE) **News**: **v1.1.0rc3** was released in 7/1/2023 The compatibilities
 of models are broken due to the unification and simplification of coordinate
 systems after v1.0.0rc0. For now, most models are benchmarked with similar
 performance, though few models are still being benchmarked. In the following
 release, we will update all the model checkpoints and benchmarks. See more
 details in the [Changelog](docs/en/notes/changelog.md) and [Changelog-v1.0.x]
 (docs/en/notes/changelog_v1.0.x.md). Documentation: https://
 mmdetection3d.readthedocs.io/ ## Introduction English | [ç®ä½ä¸­æ]
@@ -46,16 +46,16 @@
 -------: | :----------------------------------------------------: | :----------
 -------------------------------: | | VoteNet | 358 | Ã | 77 | Ã | |
 PointPillars-car | 141 | Ã | Ã | 140 | | PointPillars-3class | 107 | 44 | Ã
 | Ã | | SECOND | 40 | 30 | Ã | Ã | | Part-A2 | 17 | 14 | Ã | Ã | Like
 [MMDetection](https://github.com/open-mmlab/mmdetection) and [MMCV](https://
 github.com/open-mmlab/mmcv), MMDetection3D can also be used as a library to
 support different projects on top of it. ## License This project is released
-under the [Apache 2.0 license](LICENSE). ## Changelog **1.1.0rc2** was released
-in 2/12/2022. Please refer to [changelog.md](docs/en/notes/changelog.md) for
+under the [Apache 2.0 license](LICENSE). ## Changelog **1.1.0rc3** was released
+in 7/1/2023. Please refer to [changelog.md](docs/en/notes/changelog.md) for
 details and release history. ## Benchmark and model zoo Results and models are
 available in the [model zoo](docs/en/model_zoo.md).
                                   Components
               Backbones                 Heads                   Features
       * PointNet_(CVPR'2017)     * FreeAnchor_        * Dynamic_Voxelization_
       * PointNet++_                (NeurIPS'2019)       (CoRL'2019)
         (NeurIPS'2017)
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d.egg-info/SOURCES.txt` & `mmdet3d-1.1.0rc3/mmdet3d.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -124,14 +124,15 @@
 mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O512_4xb8_scannet-seg.py
 mmdet3d/.mim/configs/groupfree3d/metafile.yml
 mmdet3d/.mim/configs/h3dnet/h3dnet_8xb3_scannet-seg.py
 mmdet3d/.mim/configs/h3dnet/metafile.yml
 mmdet3d/.mim/configs/imvotenet/imvotenet_faster-rcnn-r50_fpn_4xb2_sunrgbd-3d.py
 mmdet3d/.mim/configs/imvotenet/imvotenet_stage2_8xb16_sunrgbd-3d.py
 mmdet3d/.mim/configs/imvotenet/metafile.yml
+mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_2xb4_sunrgbd-3d-10class.py
 mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_8xb4_kitti-3d-car.py
 mmdet3d/.mim/configs/imvoxelnet/metafile.yml
 mmdet3d/.mim/configs/monoflex/metafile.yml
 mmdet3d/.mim/configs/mvxnet/metafile.yml
 mmdet3d/.mim/configs/mvxnet/mvxnet_fpn_dv_second_secfpn_8xb2-80e_kitti-3d-3class.py
 mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn-r50-fpn_coco-20e_nuim.py
 mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r101_fpn_1x_nuim.py
@@ -255,15 +256,14 @@
 mmdet3d/.mim/tools/model_converters/convert_h3dnet_checkpoints.py
 mmdet3d/.mim/tools/model_converters/convert_votenet_checkpoints.py
 mmdet3d/.mim/tools/model_converters/publish_model.py
 mmdet3d/.mim/tools/model_converters/regnet2mmdet.py
 mmdet3d/apis/__init__.py
 mmdet3d/apis/inference.py
 mmdet3d/datasets/__init__.py
-mmdet3d/datasets/builder.py
 mmdet3d/datasets/convert_utils.py
 mmdet3d/datasets/dataset_wrappers.py
 mmdet3d/datasets/det3d_dataset.py
 mmdet3d/datasets/kitti2d_dataset.py
 mmdet3d/datasets/kitti_dataset.py
 mmdet3d/datasets/lyft_dataset.py
 mmdet3d/datasets/nuscenes_dataset.py
@@ -280,14 +280,15 @@
 mmdet3d/datasets/transforms/formating.py
 mmdet3d/datasets/transforms/loading.py
 mmdet3d/datasets/transforms/test_time_aug.py
 mmdet3d/datasets/transforms/transforms_3d.py
 mmdet3d/engine/__init__.py
 mmdet3d/engine/hooks/__init__.py
 mmdet3d/engine/hooks/benchmark_hook.py
+mmdet3d/engine/hooks/disable_object_sample_hook.py
 mmdet3d/engine/hooks/visualization_hook.py
 mmdet3d/evaluation/__init__.py
 mmdet3d/evaluation/functional/__init__.py
 mmdet3d/evaluation/functional/indoor_eval.py
 mmdet3d/evaluation/functional/instance_seg_eval.py
 mmdet3d/evaluation/functional/lyft_eval.py
 mmdet3d/evaluation/functional/seg_eval.py
@@ -304,15 +305,14 @@
 mmdet3d/evaluation/metrics/instance_seg_metric.py
 mmdet3d/evaluation/metrics/kitti_metric.py
 mmdet3d/evaluation/metrics/lyft_metric.py
 mmdet3d/evaluation/metrics/nuscenes_metric.py
 mmdet3d/evaluation/metrics/seg_metric.py
 mmdet3d/evaluation/metrics/waymo_metric.py
 mmdet3d/models/__init__.py
-mmdet3d/models/builder.py
 mmdet3d/models/backbones/__init__.py
 mmdet3d/models/backbones/base_pointnet.py
 mmdet3d/models/backbones/dgcnn.py
 mmdet3d/models/backbones/dla.py
 mmdet3d/models/backbones/mink_resnet.py
 mmdet3d/models/backbones/multi_backbone.py
 mmdet3d/models/backbones/nostem_regnet.py
@@ -334,14 +334,15 @@
 mmdet3d/models/dense_heads/base_conv_bbox_head.py
 mmdet3d/models/dense_heads/base_mono3d_dense_head.py
 mmdet3d/models/dense_heads/centerpoint_head.py
 mmdet3d/models/dense_heads/fcaf3d_head.py
 mmdet3d/models/dense_heads/fcos_mono3d_head.py
 mmdet3d/models/dense_heads/free_anchor3d_head.py
 mmdet3d/models/dense_heads/groupfree3d_head.py
+mmdet3d/models/dense_heads/imvoxel_head.py
 mmdet3d/models/dense_heads/monoflex_head.py
 mmdet3d/models/dense_heads/parta2_rpn_head.py
 mmdet3d/models/dense_heads/pgd_head.py
 mmdet3d/models/dense_heads/point_rpn_head.py
 mmdet3d/models/dense_heads/shape_aware_head.py
 mmdet3d/models/dense_heads/smoke_mono3d_head.py
 mmdet3d/models/dense_heads/ssd_3d_head.py
@@ -500,15 +501,15 @@
 mmdet3d/testing/model_utils.py
 mmdet3d/utils/__init__.py
 mmdet3d/utils/array_converter.py
 mmdet3d/utils/collect_env.py
 mmdet3d/utils/compat_cfg.py
 mmdet3d/utils/misc.py
 mmdet3d/utils/setup_env.py
-mmdet3d/utils/typing.py
+mmdet3d/utils/typing_utils.py
 mmdet3d/visualization/__init__.py
 mmdet3d/visualization/local_visualizer.py
 mmdet3d/visualization/vis_utils.py
 requirements/build.txt
 requirements/docs.txt
 requirements/mminstall.txt
 requirements/optional.txt
```

### Comparing `mmdet3d-1.1.0rc2/mmdet3d.egg-info/requires.txt` & `mmdet3d-1.1.0rc3/mmdet3d.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 plyfile
 scikit-image
 tensorboard
 trimesh<2.35.40,>=2.35.39
 
 [all]
 black==20.8b1
-typing-extensions==3.7.4
+typing-extensions
 waymo-open-dataset-tf-2-6-0
 lyft_dataset_sdk
 networkx>=2.5
 numba==0.53.0
 numpy
 nuscenes-devkit
 open3d
@@ -41,15 +41,15 @@
 [mim]
 mmcv<2.1.0,>=2.0.0rc0
 mmdet<3.1.0,>=3.0.0rc0
 mmengine<1.0.0,>=0.1.0
 
 [optional]
 black==20.8b1
-typing-extensions==3.7.4
+typing-extensions
 waymo-open-dataset-tf-2-6-0
 
 [tests]
 asynctest
 codecov
 flake8
 interrogate
```

### Comparing `mmdet3d-1.1.0rc2/setup.cfg` & `mmdet3d-1.1.0rc3/setup.cfg`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.0rc2/setup.py` & `mmdet3d-1.1.0rc3/setup.py`

 * *Files identical despite different names*

