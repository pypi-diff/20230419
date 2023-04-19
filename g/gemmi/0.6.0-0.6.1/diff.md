# Comparing `tmp/gemmi-0.6.0.tar.gz` & `tmp/gemmi-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemmi-0.6.0.tar", last modified: Mon Mar  6 12:09:00 2023, max compression
+gzip compressed data, was "gemmi-0.6.1.tar", last modified: Tue Apr 18 20:39:49 2023, max compression
```

## Comparing `gemmi-0.6.0.tar` & `gemmi-0.6.1.tar`

### file list

```diff
@@ -1,345 +1,344 @@
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.820683 gemmi-0.6.0/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16726 2020-07-10 20:35:39.000000 gemmi-0.6.0/LICENSE.txt
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      389 2022-08-01 10:42:25.000000 gemmi-0.6.0/MANIFEST.in
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1399 2023-03-06 12:09:00.820683 gemmi-0.6.0/PKG-INFO
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1390 2022-12-23 19:06:26.000000 gemmi-0.6.0/README.md
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.784683 gemmi-0.6.0/examples/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)        0 2020-07-10 20:35:39.000000 gemmi-0.6.0/examples/__init__.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      396 2020-08-19 11:40:21.000000 gemmi-0.6.0/examples/__main__.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1380 2020-08-19 11:40:21.000000 gemmi-0.6.0/examples/aafreq.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     2378 2023-03-05 13:04:05.000000 gemmi-0.6.0/examples/ccd_gi.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1266 2020-07-10 20:35:39.000000 gemmi-0.6.0/examples/ccd_subgraph.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      529 2020-07-10 20:35:39.000000 gemmi-0.6.0/examples/cif_i_sigi.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1338 2020-08-19 11:40:21.000000 gemmi-0.6.0/examples/col_order.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)      763 2020-07-10 20:35:39.000000 gemmi-0.6.0/examples/from_json.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)      503 2020-07-10 20:35:39.000000 gemmi-0.6.0/examples/hello.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1442 2020-07-10 20:35:39.000000 gemmi-0.6.0/examples/long_geom.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      605 2022-04-23 21:43:35.000000 gemmi-0.6.0/examples/map2mtz.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3590 2022-04-23 21:43:35.000000 gemmi-0.6.0/examples/maskcheck.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      824 2022-04-23 21:43:35.000000 gemmi-0.6.0/examples/maskdiff.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     6855 2020-08-19 11:40:21.000000 gemmi-0.6.0/examples/matthews.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1446 2020-07-10 20:35:39.000000 gemmi-0.6.0/examples/merge_mtz_mmcif.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     5382 2020-08-19 11:40:21.000000 gemmi-0.6.0/examples/monomers.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1101 2020-07-10 20:35:39.000000 gemmi-0.6.0/examples/mtrix_iso.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      575 2020-07-10 20:35:39.000000 gemmi-0.6.0/examples/mtz_i_sigi.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      571 2021-03-08 21:34:35.000000 gemmi-0.6.0/examples/multiproc.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      564 2022-04-23 21:43:35.000000 gemmi-0.6.0/examples/patterson_slice.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1315 2020-07-10 20:35:39.000000 gemmi-0.6.0/examples/rama_gather.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1145 2020-07-10 20:35:39.000000 gemmi-0.6.0/examples/rama_plot.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)      361 2020-08-19 11:40:21.000000 gemmi-0.6.0/examples/simple_search.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      568 2020-07-10 20:35:39.000000 gemmi-0.6.0/examples/sub_ccd.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     4960 2021-02-26 16:20:11.000000 gemmi-0.6.0/examples/weight.py
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.784683 gemmi-0.6.0/gemmi.egg-info/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1399 2023-03-06 12:09:00.000000 gemmi-0.6.0/gemmi.egg-info/PKG-INFO
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11891 2023-03-06 12:09:00.000000 gemmi-0.6.0/gemmi.egg-info/SOURCES.txt
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)        1 2023-03-06 12:09:00.000000 gemmi-0.6.0/gemmi.egg-info/dependency_links.txt
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)        1 2021-05-18 19:29:14.000000 gemmi-0.6.0/gemmi.egg-info/not-zip-safe
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)       21 2023-03-06 12:09:00.000000 gemmi-0.6.0/gemmi.egg-info/top_level.txt
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.780683 gemmi-0.6.0/include/
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.796683 gemmi-0.6.0/include/gemmi/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      844 2020-12-01 20:02:25.000000 gemmi-0.6.0/include/gemmi/addends.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11033 2022-10-12 14:10:08.000000 gemmi-0.6.0/include/gemmi/align.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    15824 2022-08-25 13:33:13.000000 gemmi-0.6.0/include/gemmi/assembly.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7484 2023-02-01 21:08:48.000000 gemmi-0.6.0/include/gemmi/asudata.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11431 2022-08-23 21:05:21.000000 gemmi-0.6.0/include/gemmi/asumask.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1023 2022-08-01 10:43:22.000000 gemmi-0.6.0/include/gemmi/atof.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3791 2021-05-20 19:43:31.000000 gemmi-0.6.0/include/gemmi/atox.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3983 2022-04-23 21:43:35.000000 gemmi-0.6.0/include/gemmi/bessel.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6974 2023-02-01 21:07:05.000000 gemmi-0.6.0/include/gemmi/binner.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4864 2022-06-13 10:43:35.000000 gemmi-0.6.0/include/gemmi/blob.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10368 2022-08-23 21:23:50.000000 gemmi-0.6.0/include/gemmi/c4322.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6018 2023-02-13 09:09:58.000000 gemmi-0.6.0/include/gemmi/calculate.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17280 2022-09-07 12:58:00.000000 gemmi-0.6.0/include/gemmi/ccp4.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13372 2022-05-18 17:02:25.000000 gemmi-0.6.0/include/gemmi/cellred.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    24840 2023-02-24 21:53:47.000000 gemmi-0.6.0/include/gemmi/chemcomp.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4636 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/chemcomp_xyz.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13992 2022-12-28 09:35:27.000000 gemmi-0.6.0/include/gemmi/cif.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14841 2022-12-23 13:09:42.000000 gemmi-0.6.0/include/gemmi/cif2mtz.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    35703 2022-10-14 19:25:51.000000 gemmi-0.6.0/include/gemmi/cifdoc.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5031 2020-08-19 11:40:21.000000 gemmi-0.6.0/include/gemmi/contact.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      590 2023-03-04 21:09:46.000000 gemmi-0.6.0/include/gemmi/crd.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7049 2023-02-07 09:15:44.000000 gemmi-0.6.0/include/gemmi/dencalc.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6965 2021-10-27 09:15:46.000000 gemmi-0.6.0/include/gemmi/dirwalk.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5809 2021-10-23 12:00:35.000000 gemmi-0.6.0/include/gemmi/eig3.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14634 2022-10-14 12:06:03.000000 gemmi-0.6.0/include/gemmi/elem.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4526 2022-10-11 18:19:45.000000 gemmi-0.6.0/include/gemmi/enumstr.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2123 2023-03-04 21:35:09.000000 gemmi-0.6.0/include/gemmi/fail.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5371 2022-04-23 21:43:35.000000 gemmi-0.6.0/include/gemmi/fileutil.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5139 2022-06-09 09:52:00.000000 gemmi-0.6.0/include/gemmi/floodfill.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4468 2023-01-31 21:22:45.000000 gemmi-0.6.0/include/gemmi/formfact.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13191 2022-10-26 13:00:57.000000 gemmi-0.6.0/include/gemmi/fourier.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)   271931 2022-10-31 20:46:06.000000 gemmi-0.6.0/include/gemmi/fprime.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2222 2021-05-24 17:07:41.000000 gemmi-0.6.0/include/gemmi/fstream.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26551 2023-02-01 21:08:11.000000 gemmi-0.6.0/include/gemmi/grid.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5182 2023-03-02 00:39:15.000000 gemmi-0.6.0/include/gemmi/gz.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4512 2021-12-22 18:43:49.000000 gemmi-0.6.0/include/gemmi/input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1846 2022-09-12 17:26:20.000000 gemmi-0.6.0/include/gemmi/interop.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10429 2022-08-23 21:24:04.000000 gemmi-0.6.0/include/gemmi/it92.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9757 2022-04-23 21:43:35.000000 gemmi-0.6.0/include/gemmi/iterator.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4820 2021-12-07 17:42:29.000000 gemmi-0.6.0/include/gemmi/json.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9023 2023-02-23 15:44:49.000000 gemmi-0.6.0/include/gemmi/levmar.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6788 2023-02-16 10:47:29.000000 gemmi-0.6.0/include/gemmi/linkhunt.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14900 2023-02-18 18:10:08.000000 gemmi-0.6.0/include/gemmi/math.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16984 2023-02-01 21:10:16.000000 gemmi-0.6.0/include/gemmi/merge.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13303 2022-08-30 15:23:57.000000 gemmi-0.6.0/include/gemmi/metadata.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      991 2023-03-04 21:10:00.000000 gemmi-0.6.0/include/gemmi/mmcif.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1243 2023-01-20 13:06:29.000000 gemmi-0.6.0/include/gemmi/mmcif_impl.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9848 2023-01-03 20:35:28.000000 gemmi-0.6.0/include/gemmi/mmdb.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3894 2022-10-06 22:31:53.000000 gemmi-0.6.0/include/gemmi/mmread.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      818 2023-03-04 21:07:51.000000 gemmi-0.6.0/include/gemmi/mmread_gz.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    35745 2023-01-20 14:59:53.000000 gemmi-0.6.0/include/gemmi/model.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6285 2022-11-14 14:06:08.000000 gemmi-0.6.0/include/gemmi/modify.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13815 2023-03-04 21:10:55.000000 gemmi-0.6.0/include/gemmi/monlib.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    40814 2023-03-04 21:16:37.000000 gemmi-0.6.0/include/gemmi/mtz.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4464 2023-03-04 21:14:00.000000 gemmi-0.6.0/include/gemmi/mtz2cif.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    15545 2023-02-13 09:09:58.000000 gemmi-0.6.0/include/gemmi/neighbor.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2787 2022-04-23 21:43:35.000000 gemmi-0.6.0/include/gemmi/neutron92.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1479 2022-08-01 10:43:31.000000 gemmi-0.6.0/include/gemmi/numb.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    25860 2022-12-29 21:31:20.000000 gemmi-0.6.0/include/gemmi/pdb.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1287 2020-08-26 14:14:17.000000 gemmi-0.6.0/include/gemmi/pirfasta.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8754 2023-03-04 21:27:37.000000 gemmi-0.6.0/include/gemmi/polyheur.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12909 2021-12-29 23:52:19.000000 gemmi-0.6.0/include/gemmi/qcp.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      954 2023-03-04 21:08:41.000000 gemmi-0.6.0/include/gemmi/read_cif.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1117 2022-09-08 19:52:57.000000 gemmi-0.6.0/include/gemmi/read_map.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5846 2023-01-31 21:22:45.000000 gemmi-0.6.0/include/gemmi/recgrid.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1992 2023-02-04 08:56:39.000000 gemmi-0.6.0/include/gemmi/reciproc.hpp
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.796683 gemmi-0.6.0/include/gemmi/refine/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    56142 2023-03-03 00:50:31.000000 gemmi-0.6.0/include/gemmi/refine/geom.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    22627 2023-03-03 00:50:31.000000 gemmi-0.6.0/include/gemmi/refine/ll.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8857 2023-01-20 13:06:29.000000 gemmi-0.6.0/include/gemmi/refln.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2842 2022-06-06 13:06:39.000000 gemmi-0.6.0/include/gemmi/reindex.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    25545 2022-09-22 17:51:39.000000 gemmi-0.6.0/include/gemmi/remarks.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2849 2023-03-04 21:17:00.000000 gemmi-0.6.0/include/gemmi/resinfo.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1083 2023-03-04 21:17:23.000000 gemmi-0.6.0/include/gemmi/riding_h.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11608 2022-11-23 12:18:21.000000 gemmi-0.6.0/include/gemmi/scaling.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16153 2022-09-14 11:05:13.000000 gemmi-0.6.0/include/gemmi/select.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10437 2021-04-18 11:38:33.000000 gemmi-0.6.0/include/gemmi/seqalign.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5125 2023-03-01 16:42:39.000000 gemmi-0.6.0/include/gemmi/seqid.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5432 2023-01-31 21:22:45.000000 gemmi-0.6.0/include/gemmi/sfcalc.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4034 2021-12-06 18:48:11.000000 gemmi-0.6.0/include/gemmi/small.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6843 2021-12-06 18:46:12.000000 gemmi-0.6.0/include/gemmi/smcif.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17639 2022-08-23 21:05:21.000000 gemmi-0.6.0/include/gemmi/solmask.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4668 2022-08-30 15:08:57.000000 gemmi-0.6.0/include/gemmi/span.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1521 2023-01-27 13:29:28.000000 gemmi-0.6.0/include/gemmi/sprintf.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2761 2023-02-01 21:07:17.000000 gemmi-0.6.0/include/gemmi/stats.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    92527 2023-02-03 17:41:30.000000 gemmi-0.6.0/include/gemmi/symmetry.hpp
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.796683 gemmi-0.6.0/include/gemmi/third_party/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)   114265 2023-01-19 09:46:30.000000 gemmi-0.6.0/include/gemmi/third_party/fast_float.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)   107015 2021-08-26 08:18:28.000000 gemmi-0.6.0/include/gemmi/third_party/pocketfft_hdronly.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    95912 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/sajson.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    58248 2023-03-02 00:36:53.000000 gemmi-0.6.0/include/gemmi/third_party/stb_sprintf.h
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.796683 gemmi-0.6.0/include/gemmi/third_party/tao/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1104 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/LICENSE
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      359 2022-05-19 09:34:03.000000 gemmi-0.6.0/include/gemmi/third_party/tao/NOTES
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.800683 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.800683 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4544 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/analyze_cycles.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      646 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/counted.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      954 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/generic.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      943 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/grammar_info.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1705 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/insert_guard.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1099 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/insert_rules.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      749 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/rule_info.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      990 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/rule_type.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      559 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analyze.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      451 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/apply_mode.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1339 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/argv_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3463 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/ascii.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5021 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/buffer_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      534 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/config.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      872 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/cstream_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1042 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/eol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      440 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/eol_pair.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      961 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/file_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1513 2021-05-24 17:06:09.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/input_error.hpp
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.808683 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1439 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/action.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2869 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/action_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      548 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/alnum.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      538 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/alpha.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1664 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/any.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2750 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/apply.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2521 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/apply0.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1154 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/apply0_single.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1229 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/apply_single.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1626 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/at.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      862 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/bof.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      870 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/bol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1573 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/bump_help.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1373 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/bump_impl.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1076 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/bytes.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1445 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/control.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1049 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/cr_crlf_eol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      975 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/cr_eol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1025 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/crlf_eol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1389 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/cstream_reader.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1178 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/cstring_reader.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      843 2022-08-06 17:18:16.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/demangle.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1045 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/demangle_cxxabi.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      567 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/demangle_nop.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1376 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/demangle_sanitise.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1382 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/disable.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1003 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/discard.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      616 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/dusel_mode.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7228 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/duseltronik.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1377 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/enable.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1557 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/endian.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5410 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/endian_gcc.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2938 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/endian_win.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      884 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/eof.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      920 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/eol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      974 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/eolf.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2518 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/file_mapper.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2011 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/file_opener.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3297 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/file_reader.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      751 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/has_apply.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      756 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/has_apply0.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      772 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/identifier.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3802 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/if_apply.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      580 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/if_must.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      634 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/if_must_else.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1862 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/if_then_else.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      723 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/input_pair.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3323 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/integer_sequence.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1159 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/istream_reader.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2766 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/istring.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1493 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/iterator.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1229 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/lf_crlf_eol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      975 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/lf_eol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      567 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/list.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      610 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/list_must.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      607 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/list_tail.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      697 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/list_tail_pad.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2409 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/marker.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2092 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/minus.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2484 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/must.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1652 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/not_at.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2429 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/one.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1648 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/opt.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      596 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/pad.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      609 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/pad_opt.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      837 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/peek_char.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2245 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/peek_utf16.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1800 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/peek_utf32.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2931 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/peek_utf8.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4180 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/pegtl_string.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1786 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/plus.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1598 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/raise.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1684 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/range.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2994 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/ranges.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2020 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/rep.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      641 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/rep_min.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2880 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/rep_min_max.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1500 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/rep_opt.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1172 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/require.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      568 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/result_on_found.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1910 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/rule_conjunction.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1393 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/rules.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2240 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/seq.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      903 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/skip_control.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2150 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/sor.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1494 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/star.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      594 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/star_must.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2769 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/state.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1736 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/string.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      955 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/trivial.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1972 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/try_catch_type.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2874 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/until.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      876 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/istream_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9778 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/memory_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1913 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/mmap_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3897 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/normal.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      586 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/nothing.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1616 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/parse.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1106 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/parse_error.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1351 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/position.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2198 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/read_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      459 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/rewind_mode.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4942 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/rules.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1936 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/string_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      445 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/tracking_mode.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2832 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/utf16.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2832 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/utf32.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1553 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/utf8.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      602 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/version.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      793 2020-07-10 20:35:39.000000 gemmi-0.6.0/include/gemmi/third_party/tao/pegtl.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    19235 2022-04-23 21:43:35.000000 gemmi-0.6.0/include/gemmi/third_party/tinydir.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2797 2022-11-12 21:59:36.000000 gemmi-0.6.0/include/gemmi/to_chemcomp.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6242 2022-11-08 19:08:56.000000 gemmi-0.6.0/include/gemmi/to_cif.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8862 2021-11-15 18:03:22.000000 gemmi-0.6.0/include/gemmi/to_json.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2231 2023-03-04 21:20:32.000000 gemmi-0.6.0/include/gemmi/to_mmcif.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      862 2023-03-04 21:20:57.000000 gemmi-0.6.0/include/gemmi/to_pdb.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10653 2023-03-04 21:21:39.000000 gemmi-0.6.0/include/gemmi/topo.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10282 2022-10-14 12:11:45.000000 gemmi-0.6.0/include/gemmi/twin.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    21692 2022-10-27 19:50:42.000000 gemmi-0.6.0/include/gemmi/unitcell.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2476 2021-04-17 18:25:34.000000 gemmi-0.6.0/include/gemmi/utf.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8661 2023-02-09 23:24:19.000000 gemmi-0.6.0/include/gemmi/util.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      152 2023-03-01 19:46:14.000000 gemmi-0.6.0/include/gemmi/version.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14766 2023-03-04 21:22:15.000000 gemmi-0.6.0/include/gemmi/xds_ascii.hpp
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.812683 gemmi-0.6.0/python/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4085 2022-09-12 16:59:12.000000 gemmi-0.6.0/python/align.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      327 2022-02-04 16:03:43.000000 gemmi-0.6.0/python/arrvec.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2447 2022-12-21 13:51:11.000000 gemmi-0.6.0/python/ccp4.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8464 2023-02-16 00:04:33.000000 gemmi-0.6.0/python/chemcomp.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17105 2022-12-21 13:17:59.000000 gemmi-0.6.0/python/cif.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3104 2023-01-31 21:22:45.000000 gemmi-0.6.0/python/common.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      195 2022-01-13 20:51:13.000000 gemmi-0.6.0/python/custom.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5307 2022-10-09 18:06:55.000000 gemmi-0.6.0/python/elem.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6093 2023-02-01 21:35:29.000000 gemmi-0.6.0/python/gemmi.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12480 2022-10-26 15:34:30.000000 gemmi-0.6.0/python/grid.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16824 2023-02-04 08:44:54.000000 gemmi-0.6.0/python/hkl.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16699 2023-02-24 21:53:47.000000 gemmi-0.6.0/python/meta.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      745 2023-02-18 19:56:19.000000 gemmi-0.6.0/python/meta.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      571 2021-01-14 17:40:02.000000 gemmi-0.6.0/python/miller_a.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26550 2022-12-29 14:12:44.000000 gemmi-0.6.0/python/mol.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5940 2023-03-05 00:14:47.000000 gemmi-0.6.0/python/monlib.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14980 2023-02-24 21:53:47.000000 gemmi-0.6.0/python/mtz.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7676 2023-01-19 17:21:52.000000 gemmi-0.6.0/python/read.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9555 2022-12-21 20:39:07.000000 gemmi-0.6.0/python/recgrid.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26396 2023-02-15 17:14:45.000000 gemmi-0.6.0/python/refine.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2005 2022-04-23 21:43:35.000000 gemmi-0.6.0/python/scaling.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6440 2022-12-01 12:58:00.000000 gemmi-0.6.0/python/search.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3819 2023-01-31 21:22:45.000000 gemmi-0.6.0/python/sf.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11972 2023-02-03 15:25:52.000000 gemmi-0.6.0/python/sym.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7260 2023-02-13 09:09:58.000000 gemmi-0.6.0/python/topo.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      835 2022-04-23 21:43:35.000000 gemmi-0.6.0/python/tostr.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17384 2023-02-24 21:53:47.000000 gemmi-0.6.0/python/unitcell.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3764 2023-01-03 21:57:58.000000 gemmi-0.6.0/python/write.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      178 2023-03-06 12:09:00.820683 gemmi-0.6.0/setup.cfg
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7729 2023-03-05 23:07:10.000000 gemmi-0.6.0/setup.py
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.812683 gemmi-0.6.0/src/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    23532 2023-02-17 22:05:25.000000 gemmi-0.6.0/src/crd.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    35840 2023-01-20 15:08:21.000000 gemmi-0.6.0/src/mmcif.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      697 2023-01-19 17:16:44.000000 gemmi-0.6.0/src/mmread_gz.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    20569 2023-02-23 13:43:25.000000 gemmi-0.6.0/src/monlib.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6406 2023-01-04 10:20:12.000000 gemmi-0.6.0/src/mtz.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    37163 2023-03-01 19:00:03.000000 gemmi-0.6.0/src/mtz2cif.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8437 2023-01-17 14:03:42.000000 gemmi-0.6.0/src/polyheur.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      899 2023-01-19 17:18:32.000000 gemmi-0.6.0/src/read_cif.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    24535 2022-12-29 18:29:27.000000 gemmi-0.6.0/src/resinfo.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    18536 2023-03-01 16:42:39.000000 gemmi-0.6.0/src/riding_h.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)       99 2023-01-03 20:55:04.000000 gemmi-0.6.0/src/sprintf.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    50897 2023-01-03 22:34:40.000000 gemmi-0.6.0/src/to_mmcif.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26850 2023-01-04 10:12:00.000000 gemmi-0.6.0/src/to_pdb.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    31569 2023-03-04 18:50:52.000000 gemmi-0.6.0/src/topo.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2219 2023-03-01 16:42:39.000000 gemmi-0.6.0/src/xds_ascii.cpp
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.780683 gemmi-0.6.0/third_party/
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-03-06 12:09:00.820683 gemmi-0.6.0/third_party/zlib/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5204 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/adler32.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14053 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/crc32.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    30562 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/crc32.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6819 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/gzguts.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16599 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/gzlib.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    20428 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/gzread.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12978 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/inffast.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      427 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/inffast.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6332 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/inffixed.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    54800 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/inflate.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6618 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/inflate.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12999 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/inftrees.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2928 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/inftrees.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1031 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/license
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16298 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/zconf.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    96239 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/zlib.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7304 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/zutil.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7127 2020-07-10 20:35:39.000000 gemmi-0.6.0/third_party/zlib/zutil.h
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.036314 gemmi-0.6.1/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16726 2020-07-10 20:35:39.000000 gemmi-0.6.1/LICENSE.txt
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      389 2022-08-01 10:42:25.000000 gemmi-0.6.1/MANIFEST.in
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2111 2023-04-18 20:39:49.036314 gemmi-0.6.1/PKG-INFO
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1390 2023-04-15 23:14:09.000000 gemmi-0.6.1/README.md
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.000314 gemmi-0.6.1/examples/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)        0 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/__init__.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      396 2020-08-19 11:40:21.000000 gemmi-0.6.1/examples/__main__.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1380 2020-08-19 11:40:21.000000 gemmi-0.6.1/examples/aafreq.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     2378 2023-03-05 13:04:05.000000 gemmi-0.6.1/examples/ccd_gi.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1266 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/ccd_subgraph.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      529 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/cif_i_sigi.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1338 2020-08-19 11:40:21.000000 gemmi-0.6.1/examples/col_order.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)      763 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/from_json.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)      503 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/hello.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1442 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/long_geom.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      605 2022-04-23 21:43:35.000000 gemmi-0.6.1/examples/map2mtz.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3590 2022-04-23 21:43:35.000000 gemmi-0.6.1/examples/maskcheck.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      824 2022-04-23 21:43:35.000000 gemmi-0.6.1/examples/maskdiff.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     6855 2020-08-19 11:40:21.000000 gemmi-0.6.1/examples/matthews.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1446 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/merge_mtz_mmcif.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     5382 2020-08-19 11:40:21.000000 gemmi-0.6.1/examples/monomers.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1101 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/mtrix_iso.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      575 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/mtz_i_sigi.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      571 2021-03-08 21:34:35.000000 gemmi-0.6.1/examples/multiproc.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      564 2022-04-23 21:43:35.000000 gemmi-0.6.1/examples/patterson_slice.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1315 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/rama_gather.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1145 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/rama_plot.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)      361 2020-08-19 11:40:21.000000 gemmi-0.6.1/examples/simple_search.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      568 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/sub_ccd.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     4960 2021-02-26 16:20:11.000000 gemmi-0.6.1/examples/weight.py
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.000314 gemmi-0.6.1/gemmi.egg-info/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2111 2023-04-18 20:39:48.000000 gemmi-0.6.1/gemmi.egg-info/PKG-INFO
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11864 2023-04-18 20:39:48.000000 gemmi-0.6.1/gemmi.egg-info/SOURCES.txt
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)        1 2023-04-18 20:39:48.000000 gemmi-0.6.1/gemmi.egg-info/dependency_links.txt
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)        1 2021-05-18 19:29:14.000000 gemmi-0.6.1/gemmi.egg-info/not-zip-safe
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)       21 2023-04-18 20:39:48.000000 gemmi-0.6.1/gemmi.egg-info/top_level.txt
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:48.996314 gemmi-0.6.1/include/
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.012314 gemmi-0.6.1/include/gemmi/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      844 2020-12-01 20:02:25.000000 gemmi-0.6.1/include/gemmi/addends.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11033 2022-10-12 14:10:08.000000 gemmi-0.6.1/include/gemmi/align.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4590 2023-04-03 18:48:39.000000 gemmi-0.6.1/include/gemmi/assembly.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7484 2023-02-01 21:08:48.000000 gemmi-0.6.1/include/gemmi/asudata.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11431 2022-08-23 21:05:21.000000 gemmi-0.6.1/include/gemmi/asumask.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1023 2022-08-01 10:43:22.000000 gemmi-0.6.1/include/gemmi/atof.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3791 2021-05-20 19:43:31.000000 gemmi-0.6.1/include/gemmi/atox.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3983 2022-04-23 21:43:35.000000 gemmi-0.6.1/include/gemmi/bessel.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6974 2023-02-01 21:07:05.000000 gemmi-0.6.1/include/gemmi/binner.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4864 2022-06-13 10:43:35.000000 gemmi-0.6.1/include/gemmi/blob.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3045 2023-04-18 20:21:43.000000 gemmi-0.6.1/include/gemmi/bond_idx.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10368 2022-08-23 21:23:50.000000 gemmi-0.6.1/include/gemmi/c4322.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5574 2023-03-21 08:04:35.000000 gemmi-0.6.1/include/gemmi/calculate.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17280 2022-09-07 12:58:00.000000 gemmi-0.6.1/include/gemmi/ccp4.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13372 2022-05-18 17:02:25.000000 gemmi-0.6.1/include/gemmi/cellred.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    23755 2023-04-14 09:25:55.000000 gemmi-0.6.1/include/gemmi/chemcomp.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4657 2023-03-29 11:09:35.000000 gemmi-0.6.1/include/gemmi/chemcomp_xyz.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13992 2022-12-28 09:35:27.000000 gemmi-0.6.1/include/gemmi/cif.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    15241 2023-04-17 21:09:38.000000 gemmi-0.6.1/include/gemmi/cif2mtz.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    35703 2022-10-14 19:25:51.000000 gemmi-0.6.1/include/gemmi/cifdoc.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5036 2023-04-13 00:17:52.000000 gemmi-0.6.1/include/gemmi/contact.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      543 2023-04-15 22:21:44.000000 gemmi-0.6.1/include/gemmi/crd.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7049 2023-02-07 09:15:44.000000 gemmi-0.6.1/include/gemmi/dencalc.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6965 2021-10-27 09:15:46.000000 gemmi-0.6.1/include/gemmi/dirwalk.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      314 2023-03-17 20:22:37.000000 gemmi-0.6.1/include/gemmi/eig3.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14634 2022-10-14 12:06:03.000000 gemmi-0.6.1/include/gemmi/elem.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4526 2022-10-11 18:19:45.000000 gemmi-0.6.1/include/gemmi/enumstr.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2123 2023-03-04 21:35:09.000000 gemmi-0.6.1/include/gemmi/fail.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5371 2022-04-23 21:43:35.000000 gemmi-0.6.1/include/gemmi/fileutil.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5139 2022-06-09 09:52:00.000000 gemmi-0.6.1/include/gemmi/floodfill.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4468 2023-01-31 21:22:45.000000 gemmi-0.6.1/include/gemmi/formfact.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13191 2022-10-26 13:00:57.000000 gemmi-0.6.1/include/gemmi/fourier.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)   271931 2022-10-31 20:46:06.000000 gemmi-0.6.1/include/gemmi/fprime.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2222 2021-05-24 17:07:41.000000 gemmi-0.6.1/include/gemmi/fstream.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26551 2023-02-01 21:08:11.000000 gemmi-0.6.1/include/gemmi/grid.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5182 2023-03-02 00:39:15.000000 gemmi-0.6.1/include/gemmi/gz.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4512 2021-12-22 18:43:49.000000 gemmi-0.6.1/include/gemmi/input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1846 2022-09-12 17:26:20.000000 gemmi-0.6.1/include/gemmi/interop.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10429 2022-08-23 21:24:04.000000 gemmi-0.6.1/include/gemmi/it92.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9757 2022-04-23 21:43:35.000000 gemmi-0.6.1/include/gemmi/iterator.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4820 2021-12-07 17:42:29.000000 gemmi-0.6.1/include/gemmi/json.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9023 2023-02-23 15:44:49.000000 gemmi-0.6.1/include/gemmi/levmar.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6788 2023-04-13 00:17:52.000000 gemmi-0.6.1/include/gemmi/linkhunt.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14300 2023-03-17 19:40:39.000000 gemmi-0.6.1/include/gemmi/math.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16984 2023-02-01 21:10:16.000000 gemmi-0.6.1/include/gemmi/merge.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13592 2023-03-16 21:39:04.000000 gemmi-0.6.1/include/gemmi/metadata.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      991 2023-03-04 21:10:00.000000 gemmi-0.6.1/include/gemmi/mmcif.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1243 2023-01-20 13:06:29.000000 gemmi-0.6.1/include/gemmi/mmcif_impl.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9234 2023-03-17 14:07:43.000000 gemmi-0.6.1/include/gemmi/mmdb.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3894 2022-10-06 22:31:53.000000 gemmi-0.6.1/include/gemmi/mmread.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      818 2023-03-04 21:07:51.000000 gemmi-0.6.1/include/gemmi/mmread_gz.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    35817 2023-03-17 12:43:09.000000 gemmi-0.6.1/include/gemmi/model.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6285 2022-11-14 14:06:08.000000 gemmi-0.6.1/include/gemmi/modify.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11283 2023-03-28 13:58:50.000000 gemmi-0.6.1/include/gemmi/monlib.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    38452 2023-04-18 17:28:58.000000 gemmi-0.6.1/include/gemmi/mtz.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4439 2023-04-15 22:22:09.000000 gemmi-0.6.1/include/gemmi/mtz2cif.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13422 2023-04-13 09:39:56.000000 gemmi-0.6.1/include/gemmi/neighbor.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2787 2022-04-23 21:43:35.000000 gemmi-0.6.1/include/gemmi/neutron92.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1479 2022-08-01 10:43:31.000000 gemmi-0.6.1/include/gemmi/numb.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26254 2023-04-16 18:00:05.000000 gemmi-0.6.1/include/gemmi/pdb.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1287 2020-08-26 14:14:17.000000 gemmi-0.6.1/include/gemmi/pirfasta.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8257 2023-04-15 22:23:44.000000 gemmi-0.6.1/include/gemmi/polyheur.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12909 2021-12-29 23:52:19.000000 gemmi-0.6.1/include/gemmi/qcp.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      954 2023-03-04 21:08:41.000000 gemmi-0.6.1/include/gemmi/read_cif.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1117 2022-09-08 19:52:57.000000 gemmi-0.6.1/include/gemmi/read_map.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5846 2023-01-31 21:22:45.000000 gemmi-0.6.1/include/gemmi/recgrid.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1992 2023-02-04 08:56:39.000000 gemmi-0.6.1/include/gemmi/reciproc.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8857 2023-01-20 13:06:29.000000 gemmi-0.6.1/include/gemmi/refln.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    25493 2023-03-13 12:53:53.000000 gemmi-0.6.1/include/gemmi/remarks.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2849 2023-03-04 21:17:00.000000 gemmi-0.6.1/include/gemmi/resinfo.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1016 2023-03-27 14:36:57.000000 gemmi-0.6.1/include/gemmi/riding_h.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11608 2022-11-23 12:18:21.000000 gemmi-0.6.1/include/gemmi/scaling.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16331 2023-04-05 08:00:20.000000 gemmi-0.6.1/include/gemmi/select.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10437 2021-04-18 11:38:33.000000 gemmi-0.6.1/include/gemmi/seqalign.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5125 2023-03-01 16:42:39.000000 gemmi-0.6.1/include/gemmi/seqid.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5432 2023-01-31 21:22:45.000000 gemmi-0.6.1/include/gemmi/sfcalc.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4034 2021-12-06 18:48:11.000000 gemmi-0.6.1/include/gemmi/small.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6843 2021-12-06 18:46:12.000000 gemmi-0.6.1/include/gemmi/smcif.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17639 2022-08-23 21:05:21.000000 gemmi-0.6.1/include/gemmi/solmask.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4668 2022-08-30 15:08:57.000000 gemmi-0.6.1/include/gemmi/span.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1521 2023-01-27 13:29:28.000000 gemmi-0.6.1/include/gemmi/sprintf.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2761 2023-02-01 21:07:17.000000 gemmi-0.6.1/include/gemmi/stats.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    92527 2023-02-03 17:41:30.000000 gemmi-0.6.1/include/gemmi/symmetry.hpp
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.012314 gemmi-0.6.1/include/gemmi/third_party/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)   114265 2023-01-19 09:46:30.000000 gemmi-0.6.1/include/gemmi/third_party/fast_float.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)   107015 2021-08-26 08:18:28.000000 gemmi-0.6.1/include/gemmi/third_party/pocketfft_hdronly.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    95912 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/sajson.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    58248 2023-03-02 00:36:53.000000 gemmi-0.6.1/include/gemmi/third_party/stb_sprintf.h
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.012314 gemmi-0.6.1/include/gemmi/third_party/tao/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1104 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/LICENSE
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      359 2022-05-19 09:34:03.000000 gemmi-0.6.1/include/gemmi/third_party/tao/NOTES
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.016314 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.016314 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4544 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/analyze_cycles.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      646 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/counted.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      954 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/generic.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      943 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/grammar_info.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1705 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/insert_guard.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1099 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/insert_rules.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      749 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/rule_info.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      990 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/rule_type.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      559 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analyze.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      451 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/apply_mode.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1339 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/argv_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3463 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/ascii.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5021 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/buffer_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      534 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/config.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      872 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/cstream_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1042 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/eol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      440 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/eol_pair.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      961 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/file_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1513 2021-05-24 17:06:09.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/input_error.hpp
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.024314 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1439 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/action.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2869 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/action_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      548 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/alnum.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      538 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/alpha.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1664 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/any.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2750 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2521 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply0.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1154 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply0_single.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1229 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply_single.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1626 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/at.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      862 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bof.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      870 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1573 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bump_help.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1373 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bump_impl.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1076 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bytes.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1445 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/control.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1049 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cr_crlf_eol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      975 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cr_eol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1025 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/crlf_eol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1389 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cstream_reader.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1178 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cstring_reader.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      843 2022-08-06 17:18:16.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1045 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle_cxxabi.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      567 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle_nop.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1376 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle_sanitise.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1382 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/disable.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1003 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/discard.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      616 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/dusel_mode.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7228 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/duseltronik.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1377 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/enable.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1557 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/endian.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5410 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/endian_gcc.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2938 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/endian_win.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      884 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/eof.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      920 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/eol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      974 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/eolf.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2518 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/file_mapper.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2011 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/file_opener.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3297 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/file_reader.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      751 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/has_apply.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      756 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/has_apply0.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      772 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/identifier.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3802 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_apply.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      580 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_must.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      634 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_must_else.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1862 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_then_else.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      723 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/input_pair.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3323 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/integer_sequence.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1159 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/istream_reader.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2766 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/istring.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1493 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/iterator.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1229 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/lf_crlf_eol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      975 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/lf_eol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      567 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      610 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list_must.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      607 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list_tail.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      697 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list_tail_pad.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2409 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/marker.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2092 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/minus.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2484 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/must.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1652 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/not_at.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2429 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/one.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1648 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/opt.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      596 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/pad.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      609 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/pad_opt.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      837 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_char.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2245 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_utf16.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1800 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_utf32.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2931 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_utf8.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4180 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/pegtl_string.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1786 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/plus.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1598 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/raise.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1684 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/range.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2994 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/ranges.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2020 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      641 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep_min.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2880 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep_min_max.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1500 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep_opt.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1172 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/require.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      568 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/result_on_found.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1910 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rule_conjunction.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1393 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rules.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2240 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/seq.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      903 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/skip_control.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2150 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/sor.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1494 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/star.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      594 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/star_must.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2769 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/state.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1736 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/string.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      955 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/trivial.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1972 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/try_catch_type.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2874 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/until.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      876 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/istream_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9778 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/memory_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1913 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/mmap_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3897 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/normal.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      586 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/nothing.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1616 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/parse.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1106 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/parse_error.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1351 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/position.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2198 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/read_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      459 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/rewind_mode.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4942 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/rules.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1936 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/string_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      445 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/tracking_mode.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2832 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/utf16.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2832 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/utf32.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1553 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/utf8.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      602 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/version.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      793 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    19235 2022-04-23 21:43:35.000000 gemmi-0.6.1/include/gemmi/third_party/tinydir.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2797 2022-11-12 21:59:36.000000 gemmi-0.6.1/include/gemmi/to_chemcomp.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6242 2022-11-08 19:08:56.000000 gemmi-0.6.1/include/gemmi/to_cif.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8862 2021-11-15 18:03:22.000000 gemmi-0.6.1/include/gemmi/to_json.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2391 2023-03-21 15:10:08.000000 gemmi-0.6.1/include/gemmi/to_mmcif.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      862 2023-03-04 21:20:57.000000 gemmi-0.6.1/include/gemmi/to_pdb.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10769 2023-04-14 09:26:04.000000 gemmi-0.6.1/include/gemmi/topo.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10282 2022-10-14 12:11:45.000000 gemmi-0.6.1/include/gemmi/twin.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    21692 2022-10-27 19:50:42.000000 gemmi-0.6.1/include/gemmi/unitcell.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2476 2021-04-17 18:25:34.000000 gemmi-0.6.1/include/gemmi/utf.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8661 2023-02-09 23:24:19.000000 gemmi-0.6.1/include/gemmi/util.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      152 2023-04-18 20:19:22.000000 gemmi-0.6.1/include/gemmi/version.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14985 2023-03-22 12:06:35.000000 gemmi-0.6.1/include/gemmi/xds_ascii.hpp
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.028314 gemmi-0.6.1/python/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4085 2022-09-12 16:59:12.000000 gemmi-0.6.1/python/align.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      327 2022-02-04 16:03:43.000000 gemmi-0.6.1/python/arrvec.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2447 2022-12-21 13:51:11.000000 gemmi-0.6.1/python/ccp4.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8464 2023-02-16 00:04:33.000000 gemmi-0.6.1/python/chemcomp.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17105 2022-12-21 13:17:59.000000 gemmi-0.6.1/python/cif.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3052 2023-03-17 18:03:23.000000 gemmi-0.6.1/python/common.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      195 2022-01-13 20:51:13.000000 gemmi-0.6.1/python/custom.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5307 2022-10-09 18:06:55.000000 gemmi-0.6.1/python/elem.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6075 2023-03-17 18:03:23.000000 gemmi-0.6.1/python/gemmi.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12480 2022-10-26 15:34:30.000000 gemmi-0.6.1/python/grid.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16824 2023-02-04 08:44:54.000000 gemmi-0.6.1/python/hkl.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16973 2023-03-17 13:35:13.000000 gemmi-0.6.1/python/meta.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      745 2023-02-18 19:56:19.000000 gemmi-0.6.1/python/meta.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      571 2021-01-14 17:40:02.000000 gemmi-0.6.1/python/miller_a.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26685 2023-04-03 18:53:47.000000 gemmi-0.6.1/python/mol.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5526 2023-03-27 16:12:52.000000 gemmi-0.6.1/python/monlib.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14926 2023-03-14 19:10:45.000000 gemmi-0.6.1/python/mtz.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7676 2023-01-19 17:21:52.000000 gemmi-0.6.1/python/read.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9555 2022-12-21 20:39:07.000000 gemmi-0.6.1/python/recgrid.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2005 2022-04-23 21:43:35.000000 gemmi-0.6.1/python/scaling.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6733 2023-04-13 08:18:16.000000 gemmi-0.6.1/python/search.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3819 2023-01-31 21:22:45.000000 gemmi-0.6.1/python/sf.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12208 2023-03-10 16:44:25.000000 gemmi-0.6.1/python/sym.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7386 2023-04-14 09:26:04.000000 gemmi-0.6.1/python/topo.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      835 2022-04-23 21:43:35.000000 gemmi-0.6.1/python/tostr.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17460 2023-04-13 15:15:53.000000 gemmi-0.6.1/python/unitcell.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3795 2023-03-13 17:58:41.000000 gemmi-0.6.1/python/write.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      178 2023-04-18 20:39:49.036314 gemmi-0.6.1/setup.cfg
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7613 2023-04-16 18:07:18.000000 gemmi-0.6.1/setup.py
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.032314 gemmi-0.6.1/src/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    15603 2023-04-13 00:17:52.000000 gemmi-0.6.1/src/assembly.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      927 2023-03-15 20:18:52.000000 gemmi-0.6.1/src/calculate.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    23793 2023-04-14 09:27:01.000000 gemmi-0.6.1/src/crd.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5709 2023-03-17 20:24:22.000000 gemmi-0.6.1/src/eig3.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    37325 2023-03-17 09:08:42.000000 gemmi-0.6.1/src/mmcif.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      697 2023-01-19 17:16:44.000000 gemmi-0.6.1/src/mmread_gz.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    20572 2023-04-13 00:17:52.000000 gemmi-0.6.1/src/monlib.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11299 2023-03-14 20:24:04.000000 gemmi-0.6.1/src/mtz.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    37188 2023-04-15 22:22:44.000000 gemmi-0.6.1/src/mtz2cif.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9007 2023-04-15 22:41:28.000000 gemmi-0.6.1/src/polyheur.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      899 2023-01-19 17:18:32.000000 gemmi-0.6.1/src/read_cif.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    24654 2023-04-15 12:45:01.000000 gemmi-0.6.1/src/resinfo.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17837 2023-04-15 22:24:51.000000 gemmi-0.6.1/src/riding_h.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)       99 2023-01-03 20:55:04.000000 gemmi-0.6.1/src/sprintf.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    52888 2023-03-21 15:10:08.000000 gemmi-0.6.1/src/to_mmcif.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26456 2023-04-15 22:14:14.000000 gemmi-0.6.1/src/to_pdb.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    39163 2023-04-14 09:26:04.000000 gemmi-0.6.1/src/topo.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2219 2023-03-01 16:42:39.000000 gemmi-0.6.1/src/xds_ascii.cpp
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:48.996314 gemmi-0.6.1/third_party/
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.036314 gemmi-0.6.1/third_party/zlib/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5204 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/adler32.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14053 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/crc32.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    30562 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/crc32.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6819 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/gzguts.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16599 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/gzlib.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    20428 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/gzread.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12978 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/inffast.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      427 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/inffast.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6332 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/inffixed.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    54800 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/inflate.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6618 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/inflate.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12999 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/inftrees.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2928 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/inftrees.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1031 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/license
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16298 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/zconf.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    96239 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/zlib.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7304 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/zutil.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7127 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/zutil.h
```

### Comparing `gemmi-0.6.0/LICENSE.txt` & `gemmi-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/README.md` & `gemmi-0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 GEMMI is an open-source project of [CCP4](https://www.ccp4.ac.uk/)
 and [Global Phasing Ltd](https://www.globalphasing.com/),
 two major providers of software for macromolecular crystallography.
 
 Citing: [JOSS paper](https://doi.org/10.21105/joss.04200).
 
 License: MPLv2, or (at your option) LGPLv3.
-© 2017-2022 Global Phasing Ltd.
+© 2017-2023 Global Phasing Ltd.
```

### Comparing `gemmi-0.6.0/examples/aafreq.py` & `gemmi-0.6.1/examples/aafreq.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/ccd_gi.py` & `gemmi-0.6.1/examples/ccd_gi.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/ccd_subgraph.py` & `gemmi-0.6.1/examples/ccd_subgraph.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/cif_i_sigi.py` & `gemmi-0.6.1/examples/cif_i_sigi.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/col_order.py` & `gemmi-0.6.1/examples/col_order.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/from_json.py` & `gemmi-0.6.1/examples/from_json.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/long_geom.py` & `gemmi-0.6.1/examples/long_geom.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/map2mtz.py` & `gemmi-0.6.1/examples/map2mtz.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/maskcheck.py` & `gemmi-0.6.1/examples/maskcheck.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/maskdiff.py` & `gemmi-0.6.1/examples/maskdiff.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/matthews.py` & `gemmi-0.6.1/examples/matthews.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/merge_mtz_mmcif.py` & `gemmi-0.6.1/examples/merge_mtz_mmcif.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/monomers.py` & `gemmi-0.6.1/examples/monomers.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/mtrix_iso.py` & `gemmi-0.6.1/examples/mtrix_iso.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/mtz_i_sigi.py` & `gemmi-0.6.1/examples/mtz_i_sigi.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/multiproc.py` & `gemmi-0.6.1/examples/multiproc.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/patterson_slice.py` & `gemmi-0.6.1/examples/patterson_slice.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/rama_gather.py` & `gemmi-0.6.1/examples/rama_gather.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/rama_plot.py` & `gemmi-0.6.1/examples/rama_plot.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/sub_ccd.py` & `gemmi-0.6.1/examples/sub_ccd.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/examples/weight.py` & `gemmi-0.6.1/examples/weight.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/gemmi.egg-info/SOURCES.txt` & `gemmi-0.6.1/gemmi.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 include/gemmi/asudata.hpp
 include/gemmi/asumask.hpp
 include/gemmi/atof.hpp
 include/gemmi/atox.hpp
 include/gemmi/bessel.hpp
 include/gemmi/binner.hpp
 include/gemmi/blob.hpp
+include/gemmi/bond_idx.hpp
 include/gemmi/c4322.hpp
 include/gemmi/calculate.hpp
 include/gemmi/ccp4.hpp
 include/gemmi/cellred.hpp
 include/gemmi/chemcomp.hpp
 include/gemmi/chemcomp_xyz.hpp
 include/gemmi/cif.hpp
@@ -96,15 +97,14 @@
 include/gemmi/polyheur.hpp
 include/gemmi/qcp.hpp
 include/gemmi/read_cif.hpp
 include/gemmi/read_map.hpp
 include/gemmi/recgrid.hpp
 include/gemmi/reciproc.hpp
 include/gemmi/refln.hpp
-include/gemmi/reindex.hpp
 include/gemmi/remarks.hpp
 include/gemmi/resinfo.hpp
 include/gemmi/riding_h.hpp
 include/gemmi/scaling.hpp
 include/gemmi/select.hpp
 include/gemmi/seqalign.hpp
 include/gemmi/seqid.hpp
@@ -124,16 +124,14 @@
 include/gemmi/topo.hpp
 include/gemmi/twin.hpp
 include/gemmi/unitcell.hpp
 include/gemmi/utf.hpp
 include/gemmi/util.hpp
 include/gemmi/version.hpp
 include/gemmi/xds_ascii.hpp
-include/gemmi/refine/geom.hpp
-include/gemmi/refine/ll.hpp
 include/gemmi/third_party/fast_float.h
 include/gemmi/third_party/pocketfft_hdronly.h
 include/gemmi/third_party/sajson.h
 include/gemmi/third_party/stb_sprintf.h
 include/gemmi/third_party/tinydir.h
 include/gemmi/third_party/tao/LICENSE
 include/gemmi/third_party/tao/NOTES
@@ -281,24 +279,26 @@
 python/meta.h
 python/miller_a.h
 python/mol.cpp
 python/monlib.cpp
 python/mtz.cpp
 python/read.cpp
 python/recgrid.cpp
-python/refine.cpp
 python/scaling.cpp
 python/search.cpp
 python/sf.cpp
 python/sym.cpp
 python/topo.cpp
 python/tostr.hpp
 python/unitcell.cpp
 python/write.cpp
+src/assembly.cpp
+src/calculate.cpp
 src/crd.cpp
+src/eig3.cpp
 src/mmcif.cpp
 src/mmread_gz.cpp
 src/monlib.cpp
 src/mtz.cpp
 src/mtz2cif.cpp
 src/polyheur.cpp
 src/read_cif.cpp
```

### Comparing `gemmi-0.6.0/include/gemmi/addends.hpp` & `gemmi-0.6.1/include/gemmi/addends.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/align.hpp` & `gemmi-0.6.1/include/gemmi/align.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/assembly.hpp` & `gemmi-0.6.1/src/assembly.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -1,105 +1,20 @@
 // Copyright 2020 Global Phasing Ltd.
-//
-// Generating biological assemblies by applying operations
-// from struct Assembly to a Model.
-// Includes chain (re)naming utilities.
-
-#ifndef GEMMI_ASSEMBLY_HPP_
-#define GEMMI_ASSEMBLY_HPP_
-
-#include <ostream>      // ostream
-#include <memory>       // unique_ptr
-#include "model.hpp"
-#include "modify.hpp"   // transform_pos_and_adp
-#include "neighbor.hpp" // merge_atoms_in_expanded_model
-#include "util.hpp"
 
-namespace gemmi {
-
-enum class HowToNameCopiedChain { Short, AddNumber, Dup };
-
-struct ChainNameGenerator {
-  using How = HowToNameCopiedChain;
-  How how;
-  std::vector<std::string> used_names;
-
-  ChainNameGenerator(How how_) : how(how_) {}
-  ChainNameGenerator(const Model& model, How how_) : how(how_) {
-    if (how != How::Dup)
-      for (const Chain& chain : model.chains)
-        used_names.push_back(chain.name);
-  }
-  bool has(const std::string& name) const {
-    return in_vector(name, used_names);
-  }
-  const std::string& added(const std::string& name) {
-    used_names.push_back(name);
-    return name;
-  }
-
-  std::string make_short_name(const std::string& preferred) {
-    static const char symbols[] = {
-      'A','B','C','D','E','F','G','H','I','J','K','L','M',
-      'N','O','P','Q','R','S','T','U','V','W','X','Y','Z',
-      'a','b','c','d','e','f','g','h','i','j','k','l','m',
-      'n','o','p','q','r','s','t','u','v','w','x','y','z',
-      '0','1','2','3','4','5','6','7','8','9'
-    };
-    if (!has(preferred))
-      return added(preferred);
-    std::string name(1, 'A');
-    for (char symbol : symbols) {
-      name[0] = symbol;
-      if (!has(name))
-        return added(name);
-    }
-    name += 'A';
-    for (char symbol1 : symbols) {
-      name[0] = symbol1;
-      for (char symbol2 : symbols) {
-        name[1] = symbol2;
-        if (!has(name))
-          return added(name);
-      }
-    }
-    fail("run out of 1- and 2-letter chain names");
-  }
+#include "gemmi/assembly.hpp"
 
-  std::string make_name_with_numeric_postfix(const std::string& base, int n) {
-    std::string name = base;
-    name += std::to_string(n);
-    while (has(name)) {
-      name.resize(base.size());
-      name += std::to_string(++n);
-    }
-    return added(name);
-  }
+#include <memory>             // unique_ptr
+#include "gemmi/modify.hpp"   // transform_pos_and_adp
+#include "gemmi/neighbor.hpp" // NeighborSearch
 
-  std::string make_new_name(const std::string& old, int n) {
-    switch (how) {
-      case How::Short: return make_short_name(old);
-      case How::AddNumber: return make_name_with_numeric_postfix(old, n);
-      case How::Dup: return old;
-    }
-    unreachable();
-  }
-};
-
-inline void ensure_unique_chain_name(const Model& model, Chain& chain) {
-  ChainNameGenerator namegen(HowToNameCopiedChain::Short);
-  for (const Chain& ch : model.chains)
-    if (&ch != &chain && !namegen.has(ch.name))
-      namegen.added(ch.name);
-  chain.name = namegen.make_short_name(chain.name);
-}
+namespace gemmi {
 
-namespace impl {
+namespace {
 
-inline bool any_subchain_matches(const Chain& chain, const Assembly::Gen& gen) {
+bool any_subchain_matches(const Chain& chain, const Assembly::Gen& gen) {
   const std::string* prev_subchain = nullptr;
   for (const Residue& res : chain.residues)
     if (prev_subchain == nullptr || res.subchain != *prev_subchain) {
       if (in_vector(res.subchain, gen.subchains))
         return true;
       prev_subchain = &res.subchain;
     }
@@ -107,20 +22,17 @@
 }
 
 struct AssemblyMapping {
   std::vector<std::string> sub;  // records subchain name correspondence
   std::vector<std::map<std::string, std::string>> chain_maps;
 };
 
-} // namespace impl
-
-/// @par mapping is for internal use
-inline Model make_assembly(const Assembly& assembly, const Model& model,
-                           HowToNameCopiedChain how, std::ostream* out,
-                           impl::AssemblyMapping* mapping=nullptr) {
+Model make_assembly_(const Assembly& assembly, const Model& model,
+                     HowToNameCopiedChain how, std::ostream* out,
+                     AssemblyMapping* mapping) {
   Model new_model(model.name);
   ChainNameGenerator namegen(how);
   std::map<std::string, std::string> subs = model.subchain_to_chain();
   for (const Assembly::Gen& gen : assembly.generators)
     for (const Assembly::Operator& oper : gen.operators) {
       if (out) {
         *out << "Applying " << oper.name << " to";
@@ -140,15 +52,15 @@
       std::map<std::string, std::string> new_names;
       bool all_chains = (!gen.chains.empty() && gen.chains[0] == "(all)");
       for (const Chain& chain : model.chains) {
         // PDB files specify bioassemblies in terms of chains,
         // mmCIF files in terms of subchains.
         bool whole_chain = (all_chains || in_vector(chain.name, gen.chains));
         if (whole_chain ||
-            (!gen.subchains.empty() && impl::any_subchain_matches(chain, gen))) {
+            (!gen.subchains.empty() && any_subchain_matches(chain, gen))) {
           // add a new empty chain, but first figure out the name for it
           auto result = new_names.emplace(chain.name, "");
           if (result.second)  // insertion happened - generate a new chain name
             result.first->second = namegen.make_new_name(chain.name, 1);
           new_model.chains.emplace_back(result.first->second);
           Chain& new_chain = new_model.chains.back();
           // add residues to the chain
@@ -178,46 +90,117 @@
       }
       if (mapping)
         mapping->chain_maps.push_back(std::move(new_names));
     }
   return new_model;
 }
 
-inline Assembly expand_to_p1(const UnitCell& cell) {
-  Assembly assembly("unit_cell");
-  std::vector<Assembly::Operator> operators(cell.images.size() + 1);
-  // operators[0] stays as identity
-  for (size_t i = 1; i != operators.size(); ++i) {
-    const FTransform& op = cell.images[i-1];
-    operators[i].transform = cell.orth.combine(op.combine(cell.frac));
+} // anonymous namespace
+
+Model make_assembly(const Assembly& assembly, const Model& model,
+                    HowToNameCopiedChain how, std::ostream* out) {
+  return make_assembly_(assembly, model, how, out, nullptr);
+}
+
+static void remove_cras(Model& model, std::vector<CRA>& vec) {
+  // sort in reverse order, so items can be erased without invalidating pointers
+  std::sort(vec.begin(), vec.end(), [](const CRA& a, const CRA& b) {
+      return std::tie(a.chain, a.residue, a.atom) > std::tie(b.chain, b.residue, b.atom);
+  });
+  const Atom* prev_a = nullptr;
+  for (CRA& cra : vec) {
+    if (cra.atom == prev_a)
+      continue;
+    prev_a = cra.atom;
+    auto atom_idx = cra.atom - cra.residue->atoms.data();
+    cra.residue->atoms.erase(cra.residue->atoms.begin() + atom_idx);
+    if (cra.residue->atoms.empty()) {
+      auto res_idx = cra.residue - cra.chain->residues.data();
+      cra.chain->residues.erase(cra.chain->residues.begin() + res_idx);
+      if (cra.chain->residues.empty()) {
+        auto chain_idx = cra.chain - model.chains.data();
+        model.chains.erase(model.chains.begin() + chain_idx);
+      }
+    }
   }
-  assembly.generators.push_back({{"(all)"}, {}, operators});
-  return assembly;
 }
 
-inline void transform_to_assembly(Structure& st, const std::string& assembly_name,
-                                  HowToNameCopiedChain how, std::ostream* out) {
+void merge_atoms_in_expanded_model(Model& model, const UnitCell& cell, double max_dist) {
+  using Mark = NeighborSearch::Mark;
+  NeighborSearch ns(model, cell, 4.0);
+  ns.populate(true);
+  std::vector<CRA> to_be_deleted;
+  for (int n_ch = 0; n_ch != (int) model.chains.size(); ++n_ch) {
+    Chain& chain = model.chains[n_ch];
+    for (int n_res = 0; n_res != (int) chain.residues.size(); ++n_res) {
+      Residue& res = chain.residues[n_res];
+      for (int n_atom = 0; n_atom != (int) res.atoms.size(); ++n_atom) {
+        Atom& atom = res.atoms[n_atom];
+        std::vector<std::pair<CRA, int>> equiv;
+        ns.for_each_cell(atom.pos, [&](std::vector<Mark>& marks, const Fractional& fr) {
+            for (Mark& m : marks) {
+              // We look for the same atoms, but copied to a different chain.
+              // First quick check that filters out most of non-matching pairs.
+              if (m.altloc != atom.altloc || m.element != atom.element ||
+                  m.chain_idx == n_ch || m.atom_idx != n_atom)
+                continue;
+              // Now check if everything else matches.
+              CRA cra = m.to_cra(model);
+              if (cra.atom &&
+                  cra.atom->serial == atom.serial &&
+                  cra.atom->name == atom.name &&
+                  cra.atom->b_iso == atom.b_iso &&
+                  cra.residue->matches_noseg(res) &&
+                  m.pos.dist_sq(ns.grid.unit_cell.orthogonalize(fr)) < sq(max_dist))
+                equiv.emplace_back(cra, m.image_idx);
+            }
+        });
+        if (!equiv.empty()) {
+          Position pos_sum = atom.pos;
+          for (auto& t : equiv) {
+            CRA& cra = t.first;
+            pos_sum += ns.grid.unit_cell.find_nearest_pbc_position(
+                                          atom.pos, cra.atom->pos, t.second);
+            // The atoms in equiv are to be discarded later.
+            // Deleting now would invalidate indices in NeighborSearch.
+            to_be_deleted.push_back(cra);
+            // Modify the atoms to avoid processing them again.
+            cra.atom->serial = -1;  // this should be enough
+            cra.atom->name.clear(); // this is just in case
+          }
+          size_t n = 1 + equiv.size();
+          atom.pos = pos_sum / double(n);
+          atom.occ = std::min(1.f, n * atom.occ);
+        }
+      }
+    }
+  }
+  remove_cras(model, to_be_deleted);
+}
+
+void transform_to_assembly(Structure& st, const std::string& assembly_name,
+                           HowToNameCopiedChain how, std::ostream* out) {
   const Assembly* assembly = st.find_assembly(assembly_name);
   std::unique_ptr<Assembly> p1_assembly;
   if (!assembly) {
     if (assembly_name == "unit_cell") {
       p1_assembly.reset(new Assembly(expand_to_p1(st.cell)));
       assembly = p1_assembly.get();
     } else if (st.assemblies.empty()) {
       fail("no bioassemblies are listed for this structure");
     } else {
       fail("wrong assembly name, use one of: " +
            join_str(st.assemblies, ' ', [](const Assembly& a) { return a.name; }));
     }
   }
-  impl::AssemblyMapping mapping;
+  AssemblyMapping mapping;
   for (Model& model : st.models) {
     bool set_mapping = (&model == &st.models[0] && how != HowToNameCopiedChain::Dup);
-    model = make_assembly(*assembly, model, how, out,
-                          set_mapping ? &mapping : nullptr);
+    model = make_assembly_(*assembly, model, how, out,
+                           set_mapping ? &mapping : nullptr);
     merge_atoms_in_expanded_model(model, gemmi::UnitCell());
     assign_serial_numbers(model);
   }
   // update Entity::subchains
   if (!mapping.sub.empty())
     for (Entity& ent : st.entities) {
       std::vector<std::string> new_subchains;
@@ -258,17 +241,16 @@
 
   // Should Assembly instructions be kept or removed? Currently - removing.
   st.assemblies.clear();
   // Should st.spacegroup_hm and st.cell be kept? Here we remove only:
   st.cell.images.clear();
 }
 
-// chain is assumed to be from st.models[0]
-inline void rename_chain(Structure& st, Chain& chain,
-                         const std::string& new_name) {
+
+void rename_chain(Structure& st, Chain& chain, const std::string& new_name) {
   auto rename_if_matches = [&](AtomAddress& aa) {
     if (aa.chain_name == chain.name)
       aa.chain_name = new_name;
   };
   for (Connection& con : st.connections) {
     rename_if_matches(con.partner1);
     rename_if_matches(con.partner2);
@@ -291,29 +273,16 @@
           sel.chain = new_name;
   for (auto it = st.models.begin() + 1; it != st.models.end(); ++it)
     if (Chain* ch = it->find_chain(chain.name))
       ch->name = new_name;
   chain.name = new_name;
 }
 
-inline void shorten_chain_names(Structure& st) {
-  ChainNameGenerator namegen(HowToNameCopiedChain::Short);
-  Model& model0 = st.models[0];
-  size_t max_len = model0.chains.size() < 63 ? 1 : 2;
-  for (const Chain& chain : model0.chains)
-    if (chain.name.length() <= max_len)
-      namegen.used_names.push_back(chain.name);
-  for (Chain& chain : model0.chains)
-    if (chain.name.length() > max_len)
-      rename_chain(st, chain,
-                   namegen.make_short_name(chain.name.substr(0, max_len)));
-}
-
 
-inline void expand_ncs(Structure& st, HowToNameCopiedChain how) {
+void expand_ncs(Structure& st, HowToNameCopiedChain how) {
   size_t orig_conn_size = st.connections.size();
   for (Model& model : st.models) {
     if (how == HowToNameCopiedChain::Dup) {
       // change segment of original chains to "0" - is this a good idea?
       for (Chain& chain : model.chains)
         for (Residue& res : chain.residues)
           res.segment = "0";
@@ -374,15 +343,15 @@
     }
   }
   for (NcsOp& op : st.ncs)
     op.given = true;
   st.setup_cell_images();
 }
 
-inline std::vector<Chain> split_chain_by_segments(Chain& orig, ChainNameGenerator& namegen) {
+static std::vector<Chain> split_chain_by_segments(Chain& orig, ChainNameGenerator& namegen) {
   std::vector<Chain> chains;
   std::vector<Residue> orig_res;
   orig_res.swap(orig.residues);
   int n = 0;
   for (auto start = orig_res.begin(); start != orig_res.end(); ) {
     const std::string& seg = start->segment;
     auto ch = std::find_if(chains.begin(), chains.end(), [&](Chain& c) {
@@ -408,18 +377,16 @@
     ch->residues.insert(ch->residues.end(), std::make_move_iterator(start),
                                             std::make_move_iterator(end));
     start = end;
   }
   return chains;
 }
 
-// HowToNameCopiedChain::Dup adds segment name to
-inline void split_chains_by_segments(Model& model, HowToNameCopiedChain how) {
+void split_chains_by_segments(Model& model, HowToNameCopiedChain how) {
   ChainNameGenerator namegen(how);
   std::vector<Chain> new_chains;
   for (Chain& chain : model.chains)
     vector_move_extend(new_chains, split_chain_by_segments(chain, namegen));
   model.chains = std::move(new_chains);
 }
 
 } // namespace gemmi
-#endif
```

### Comparing `gemmi-0.6.0/include/gemmi/asudata.hpp` & `gemmi-0.6.1/include/gemmi/asudata.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/asumask.hpp` & `gemmi-0.6.1/include/gemmi/asumask.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/atof.hpp` & `gemmi-0.6.1/include/gemmi/atof.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/atox.hpp` & `gemmi-0.6.1/include/gemmi/atox.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/bessel.hpp` & `gemmi-0.6.1/include/gemmi/bessel.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/binner.hpp` & `gemmi-0.6.1/include/gemmi/binner.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/blob.hpp` & `gemmi-0.6.1/include/gemmi/blob.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/c4322.hpp` & `gemmi-0.6.1/include/gemmi/c4322.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/calculate.hpp` & `gemmi-0.6.1/include/gemmi/calculate.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -126,14 +126,20 @@
 }
 
 inline double calculate_omega(const Residue& res, const Residue& next) {
   return calculate_dihedral_from_atoms(res.get_ca(), res.get_c(),
                                        next.get_n(), next.get_ca());
 }
 
+inline bool is_peptide_bond_cis(const Atom* ca1, const Atom* c,
+                                const Atom* n, const Atom* ca2) {
+  double omega = calculate_dihedral_from_atoms(ca1, c, n, ca2);
+  return std::fabs(omega) < rad(30.);
+}
+
 inline double calculate_chiral_volume(const Position& actr, const Position& a1,
                                       const Position& a2, const Position& a3) {
   return (a1 - actr).dot((a2 - actr).cross(a3 - actr));
 }
 
 inline std::array<double, 2> calculate_phi_psi(const Residue* prev,
                                                const Residue& res,
@@ -147,39 +153,15 @@
       phi_psi[0] = calculate_dihedral_from_atoms(prev->get_c(), N, CA, C);
     if (next)
       phi_psi[1] = calculate_dihedral_from_atoms(N, CA, C, next->get_n());
   }
   return phi_psi;
 }
 
-inline std::array<double, 4> find_best_plane(const std::vector<Atom*>& atoms) {
-  Vec3 mean;
-  for (const Atom* atom : atoms)
-    mean += atom->pos;
-  mean /= (double) atoms.size();
-  SMat33<double> m{0, 0, 0, 0, 0, 0};
-  for (const Atom* atom : atoms) {
-    Vec3 p = Vec3(atom->pos) - mean;
-    m.u11 += p.x * p.x;
-    m.u22 += p.y * p.y;
-    m.u33 += p.z * p.z;
-    m.u12 += p.x * p.y;
-    m.u13 += p.x * p.z;
-    m.u23 += p.y * p.z;
-  }
-  auto eig = m.calculate_eigenvalues();
-  double smallest = eig[0];
-  for (double d : {eig[1], eig[2]})
-    if (std::fabs(d) < std::fabs(smallest))
-      smallest = d;
-  Vec3 eigvec = m.calculate_eigenvector(smallest);
-  if (eigvec.x < 0)
-    eigvec *= -1;
-  return {{eigvec.x, eigvec.y, eigvec.z, -eigvec.dot(mean)}};
-}
+GEMMI_DLL std::array<double, 4> find_best_plane(const std::vector<Atom*>& atoms);
 
 inline double get_distance_from_plane(const Position& pos,
                                       const std::array<double, 4>& coeff) {
   return coeff[0] * pos.x + coeff[1] * pos.y + coeff[2] * pos.z + coeff[3];
 }
 
 } // namespace gemmi
```

### Comparing `gemmi-0.6.0/include/gemmi/ccp4.hpp` & `gemmi-0.6.1/include/gemmi/ccp4.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/cellred.hpp` & `gemmi-0.6.1/include/gemmi/cellred.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/chemcomp.hpp` & `gemmi-0.6.1/include/gemmi/chemcomp.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -305,33 +305,14 @@
     double cosine = a == 90. ? 0. : std::cos(rad(a));
     x -= cosine * cosine;
     y *= cosine;
   }
   return mult * std::sqrt(x + y);
 }
 
-inline double chiral_abs_volume_sigma(double bond1, double bond2, double bond3,
-                                      double angle1, double angle2, double angle3,
-                                      double sigb1, double sigb2, double sigb3,
-                                      double siga1, double siga2, double siga3) {
-  double mult = bond1 * bond2 * bond3;
-  auto cosine = [](double a) {return a == 90. ? 0. : std::cos(rad(a));};
-  double cosa1 = cosine(angle1);
-  double cosa2 = cosine(angle2);
-  double cosa3 = cosine(angle3);
-  double x_y = 1 + 2 * cosa1 * cosa2 * cosa3 - sq(cosa1) - sq(cosa2) - sq(cosa3);
-  double varv = x_y * (sq(bond2 * bond3) * sq(sigb1) +
-                       sq(bond1 * bond3) * sq(sigb2) +
-                       sq(bond1 * bond2) * sq(sigb3));
-  varv += sq(mult) / x_y * ((1 - sq(cosa1)) * sq(cosa1 - cosa2 * cosa3) * sq(rad(siga1)) +
-                            (1 - sq(cosa2)) * sq(cosa2 - cosa1 * cosa3) * sq(rad(siga2)) +
-                            (1 - sq(cosa3)) * sq(cosa3 - cosa1 * cosa2) * sq(rad(siga3)));
-  return std::sqrt(varv);
-}
-
 inline double Restraints::chiral_abs_volume(const Restraints::Chirality& ch) const {
   return gemmi::chiral_abs_volume(get_bond(ch.id_ctr, ch.id1).value,
                                   get_bond(ch.id_ctr, ch.id2).value,
                                   get_bond(ch.id_ctr, ch.id3).value,
                                   get_angle(ch.id1, ch.id_ctr, ch.id2).value,
                                   get_angle(ch.id2, ch.id_ctr, ch.id3).value,
                                   get_angle(ch.id3, ch.id_ctr, ch.id1).value);
```

### Comparing `gemmi-0.6.0/include/gemmi/chemcomp_xyz.hpp` & `gemmi-0.6.1/include/gemmi/chemcomp_xyz.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     case ChemCompModel::Ideal:
       xyz_tags = {{"pdbx_model_Cartn_x_ideal",
                    "pdbx_model_Cartn_y_ideal",
                    "pdbx_model_Cartn_z_ideal"}};
       break;
   }
   Residue res;
+  res.seqid.num = 1;
   cif::Column col =
     const_cast<cif::Block&>(block).find_values("_chem_comp_atom.comp_id");
   if (col && col.length() > 0)
     res.name = col[0];
   else
     res.name = block.name.substr(starts_with(block.name, "comp_") ? 5 : 0);
   cif::Table table = const_cast<cif::Block&>(block).find("_chem_comp_atom.",
```

### Comparing `gemmi-0.6.0/include/gemmi/cif.hpp` & `gemmi-0.6.1/include/gemmi/cif.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/cif2mtz.hpp` & `gemmi-0.6.1/include/gemmi/cif2mtz.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     std::vector<std::pair<std::string, float>> code_to_number;
 
     Entry(const std::string& line) {
       std::vector<std::string> tokens;
       tokens.reserve(4);
       split_str_into_multi(line, " \t\r\n", tokens);
       if (tokens.size() != 4 && tokens.size() != 5)
-        fail("line should have 4  or 5 words: " + line);
+        fail("line should have 4 or 5 words: " + line);
       if (tokens[2].size() != 1 || tokens[3].size() != 1 ||
           (tokens[3][0] != '0' && tokens[3][0] != '1'))
         fail("incorrect line: " + line);
       refln_tag = tokens[0];
       col_label = tokens[1];
       col_type = tokens[2][0];
       dataset_id = tokens[3][0] - '0';
@@ -401,14 +401,21 @@
           if (std::isnan(mtz.data[k]))
             out << "Value #" << i + indices[j] << " in the loop is not a number: "
                 << v << '\n';
         }
         ++k;
       }
     }
+    if (mtz.is_merged()) {
+      gemmi::DataType type = check_data_type_under_symmetry(gemmi::MtzDataProxy{mtz});
+      if (type == gemmi::DataType::Anomalous)
+        out << "WARNING: CIF block " << rb.block.name << " has old-style anomalous data.\n";
+      else if (type == gemmi::DataType::Unmerged)
+        out << "WARNING: CIF block " << rb.block.name << " has old-style unmerged data.\n";
+    }
     return mtz;
   }
 
 private:
   static float status_to_freeflag(const std::string& str) {
     char c = str[0];
     if (c == '\'' || c == '"')
```

### Comparing `gemmi-0.6.0/include/gemmi/cifdoc.hpp` & `gemmi-0.6.1/include/gemmi/cifdoc.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/contact.hpp` & `gemmi-0.6.1/include/gemmi/contact.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 namespace gemmi {
 
 struct ContactSearch {
   enum class Ignore {
     Nothing=0, SameResidue, AdjacentResidues, SameChain, SameAsu
   };
   // parameters used to configure the search
-  float search_radius;
+  double search_radius;
   Ignore ignore = Ignore::SameResidue;
   bool twice = false;  // report both A-B and B-A
-  float special_pos_cutoff_sq = 0.8f * 0.8f;
   float min_occupancy = 0.f;
+  double special_pos_cutoff_sq = 0.8 * 0.8;
   std::vector<float> radii;
 
-  ContactSearch(float radius) noexcept : search_radius(radius) {}
+  ContactSearch(double radius) noexcept : search_radius(radius) {}
 
   // a helper function that sets per-atom radii basing on covalent_radius()
   void setup_atomic_radii(double multiplier, double tolerance) {
     radii.resize((size_t)El::END);
     for (int i = 0; i != (int) El::END; ++i)
       radii[i] = float(multiplier * Element(i).covalent_r() + tolerance / 2);
   }
@@ -39,20 +39,20 @@
 
   template<typename Func>
   void for_each_contact(NeighborSearch& ns, const Func& func);
 
   struct Result {
     CRA partner1, partner2;
     int image_idx;
-    float dist_sq;
+    double dist_sq;
   };
   std::vector<Result> find_contacts(NeighborSearch& ns) {
     std::vector<Result> out;
     for_each_contact(ns, [&out](const CRA& cra1, const CRA& cra2,
-                                int image_idx, float dist_sq) {
+                                int image_idx, double dist_sq) {
         out.push_back({cra1, cra2, image_idx, dist_sq});
     });
     return out;
   }
 };
 
 template<typename Func>
@@ -70,15 +70,15 @@
       for (int n_atom = 0; n_atom != (int) res.atoms.size(); ++n_atom) {
         Atom& atom = res.atoms[n_atom];
         if (!ns.include_h && is_hydrogen(atom.element))
           continue;
         if (atom.occ < min_occupancy)
           continue;
         ns.for_each(atom.pos, atom.altloc, search_radius,
-                    [&](NeighborSearch::Mark& m, float dist_sq) {
+                    [&](NeighborSearch::Mark& m, double dist_sq) {
             // do not consider connections inside a residue
             if (ignore != Ignore::Nothing && m.image_idx == 0 &&
                 m.chain_idx == n_ch && m.residue_idx == n_res)
               return;
             switch (ignore) {
               case Ignore::Nothing:
                 break;
@@ -101,15 +101,15 @@
               case Ignore::SameAsu:
                 if (m.image_idx == 0)
                   return;
                 break;
             }
             // additionally, we may have per-element distances
             if (!radii.empty()) {
-              float d = radii[atom.element.ordinal()] + radii[m.element.ordinal()];
+              double d = radii[atom.element.ordinal()] + radii[m.element.ordinal()];
               if (d < 0 || dist_sq > d * d)
                 return;
             }
             // avoid reporting connections twice (A-B and B-A)
             if (!twice)
               if (m.chain_idx < n_ch || (m.chain_idx == n_ch &&
                     (m.residue_idx < n_res || (m.residue_idx == n_res &&
```

### Comparing `gemmi-0.6.0/include/gemmi/crd.hpp` & `gemmi-0.6.1/include/gemmi/crd.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 //
 // Generate Refmac intermediate (prepared) files crd and rst
 
 #ifndef GEMMI_CRD_HPP_
 #define GEMMI_CRD_HPP_
 
 #include "topo.hpp"      // for Topo
-#include "riding_h.hpp"  // for HydrogenChange
 
 namespace gemmi {
 
 GEMMI_DLL void setup_for_crd(Structure& st);
 
 GEMMI_DLL void add_automatic_links(Model& model, Structure& st, const MonLib& monlib);
```

### Comparing `gemmi-0.6.0/include/gemmi/dencalc.hpp` & `gemmi-0.6.1/include/gemmi/dencalc.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/dirwalk.hpp` & `gemmi-0.6.1/include/gemmi/dirwalk.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/eig3.hpp` & `gemmi-0.6.1/src/eig3.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,20 @@
-// Eigen decomposition code for symmetric 3x3 matrices.
-
-#ifndef GEMMI_EIG3_HPP_
-#define GEMMI_EIG3_HPP_
-
 // Based on public domain code from Connelly Barnes:
 // http://barnesc.blogspot.com/2007/02/eigenvectors-of-3x3-symmetric-matrix.html
 // which in turn is based on the public domain Java Matrix library JAMA.
 
+#include <gemmi/eig3.hpp>
 #include <cmath>
-#include "math.hpp"
-
-namespace gemmi {
 
 // Symmetric Householder reduction to tridiagonal form.
 //  This is derived from the Algol procedures tred2 by
 //  Bowdler, Martin, Reinsch, and Wilkinson, Handbook for
 //  Auto. Comp., Vol.ii-Linear Algebra, and the corresponding
 //  Fortran subroutine in EISPACK.
-inline void tred2(Mat33& V, double d[3], double e[3]) {
+static void tred2(gemmi::Mat33& V, double d[3], double e[3]) {
   for (int j = 0; j < 3; j++) {
     d[j] = V[3-1][j];
   }
 
   // Householder reduction to tridiagonal form.
   for (int i = 3-1; i > 0; i--) {
     // Scale to avoid under/overflow.
@@ -120,15 +113,15 @@
 }
 
 // Symmetric tridiagonal QL algorithm.
 //  This is derived from the Algol procedures tql2, by
 //  Bowdler, Martin, Reinsch, and Wilkinson, Handbook for
 //  Auto. Comp., Vol.ii-Linear Algebra, and the corresponding
 //  Fortran subroutine in EISPACK.
-inline void tql2(Mat33& V, double d[3], double e[3]) {
+static void tql2(gemmi::Mat33& V, double d[3], double e[3]) {
   for (int i = 1; i < 3; i++) {
     e[i-1] = e[i];
   }
   e[3-1] = 0.0;
 
   double f = 0.0;
   double tst1 = 0.0;
@@ -225,17 +218,18 @@
         V[j][i] = V[j][k];
         V[j][k] = p;
       }
     }
   }
 }
 
-inline Mat33 eigen_decomposition(const SMat33<double>& A, double (&d)[3]) {
+namespace gemmi {
+
+Mat33 eigen_decomposition(const SMat33<double>& A, double (&d)[3]) {
   double e[3];
   Mat33 V = A.as_mat33();
   tred2(V, d, e);
   tql2(V, d, e);
   return V;
 }
 
 } // namespace gemmi
-#endif
```

### Comparing `gemmi-0.6.0/include/gemmi/elem.hpp` & `gemmi-0.6.1/include/gemmi/elem.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/enumstr.hpp` & `gemmi-0.6.1/include/gemmi/enumstr.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/fail.hpp` & `gemmi-0.6.1/include/gemmi/fail.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/fileutil.hpp` & `gemmi-0.6.1/include/gemmi/fileutil.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/floodfill.hpp` & `gemmi-0.6.1/include/gemmi/floodfill.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/formfact.hpp` & `gemmi-0.6.1/include/gemmi/formfact.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/fourier.hpp` & `gemmi-0.6.1/include/gemmi/fourier.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/fprime.hpp` & `gemmi-0.6.1/include/gemmi/fprime.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/fstream.hpp` & `gemmi-0.6.1/include/gemmi/fstream.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/grid.hpp` & `gemmi-0.6.1/include/gemmi/grid.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/gz.hpp` & `gemmi-0.6.1/include/gemmi/gz.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/input.hpp` & `gemmi-0.6.1/include/gemmi/input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/interop.hpp` & `gemmi-0.6.1/include/gemmi/interop.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/it92.hpp` & `gemmi-0.6.1/include/gemmi/it92.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/iterator.hpp` & `gemmi-0.6.1/include/gemmi/iterator.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/json.hpp` & `gemmi-0.6.1/include/gemmi/json.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/levmar.hpp` & `gemmi-0.6.1/include/gemmi/levmar.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/linkhunt.hpp` & `gemmi-0.6.1/include/gemmi/linkhunt.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   struct Match {
     const ChemLink* chem_link = nullptr;
     int chem_link_count = 0;
     int score = -1000;
     CRA cra1;
     CRA cra2;
     bool same_image;
-    float bond_length = 0.f;
+    double bond_length = 0;
     Connection* conn = nullptr;
   };
 
   double global_max_dist = 2.34; // ZN-CYS
   const MonLib* monlib_ptr = nullptr;
   std::multimap<std::string, const ChemLink*> links;
 
@@ -100,15 +100,15 @@
                                     /*max r1+r2 ~=*/3.0 * radius_margin);
     NeighborSearch ns(model, st.cell, std::max(5.0, search_radius));
     ns.populate();
 
     ContactSearch contacts((float) search_radius);
     contacts.ignore = ignore;
     contacts.for_each_contact(ns, [&](const CRA& cra1, const CRA& cra2,
-                                      int image_idx, float dist_sq) {
+                                      int image_idx, double dist_sq) {
         Match match;
 
         // search for a match in chem_links
         if (bond_margin > 0) {
           auto range = links.equal_range(Restraints::lexicographic_str(
                                             cra1.atom->name, cra2.atom->name));
           // similar to MonLib::match_link()
```

### Comparing `gemmi-0.6.0/include/gemmi/math.hpp` & `gemmi-0.6.1/include/gemmi/math.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -310,15 +310,16 @@
     inv.u33 = inv_det * (u11 * u22 - u12 * u12);
     inv.u12 = inv_det * (u13 * u23 - u12 * u33);
     inv.u13 = inv_det * (u12 * u23 - u13 * u22);
     inv.u23 = inv_det * (u12 * u13 - u11 * u23);
     return inv;
   }
 
-  // Based on https://en.wikipedia.org/wiki/Eigenvalue_algorithm
+  /// Based on https://en.wikipedia.org/wiki/Eigenvalue_algorithm
+  /// To calculate both eigenvalues and eigenvectors use eig3.hpp
   std::array<double, 3> calculate_eigenvalues() const {
     double p1 = u12*u12 + u13*u13 + u23*u23;
     if (p1 == 0)
       return {{u11, u22, u33}};
     double q = (1./3.) * trace();
     SMat33<double> b{u11 - q, u22 - q, u33 - q, u12, u13, u23};
     double p2 = sq(b.u11) + sq(b.u22) + sq(b.u33) + 2 * p1;
@@ -329,35 +330,14 @@
       phi = (1./3.) * pi();
     else if (r < 1)
       phi = (1./3.) * std::acos(r);
     double eig1 = q + 2 * p * std::cos(phi);
     double eig3 = q + 2 * p * std::cos(phi + 2./3.*pi());
     return {{eig1, 3 * q - eig1 - eig3, eig3}};
   }
-
-  // Assumes one of the eigenvalue calculate above.
-  // May not work if eigenvalues are not distinct.
-  Vec3 calculate_eigenvector(double eigenvalue) const {
-    Vec3 r0(u11 - eigenvalue, u12, u13);
-    Vec3 r1(u12, u22 - eigenvalue, u23);
-    Vec3 r2(u13, u23, u33 - eigenvalue);
-    Vec3 cr[3] = {r0.cross(r1), r0.cross(r2), r1.cross(r2)};
-    int idx = 0;
-    double lensq = 0;
-    for (int i = 0; i < 3; ++i) {
-      double tmp = cr[i].length_sq();
-      if (tmp > lensq) {
-        idx = i;
-        lensq = tmp;
-      }
-    }
-    if (lensq == 0)
-      return Vec3(0, 0, 1); // an arbitrary choice for the special case
-    return cr[idx] / std::sqrt(lensq);
-  }
 };
 
 struct Transform {
   Mat33 mat;
   Vec3 vec;
 
   Transform inverse() const {
```

### Comparing `gemmi-0.6.0/include/gemmi/merge.hpp` & `gemmi-0.6.1/include/gemmi/merge.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/metadata.hpp` & `gemmi-0.6.1/include/gemmi/metadata.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     DataCollection, DataExtraction, DataProcessing, DataReduction,
     DataScaling, ModelBuilding, Phasing, Refinement, Unspecified
   };
   std::string name;
   std::string version;
   std::string date;
   Classification classification = Unspecified;
-  int pdbx_ordinal = -1;
 };
 
 // Information from REMARK 200/230 is significantly expanded in PDBx/mmCIF.
 // These remarks corresponds to data across 12 mmCIF categories
 // including categories _exptl, _reflns, _exptl_crystal, _diffrn and others.
 // _exptl and _reflns seem to be 1:1. Usually we have one experiment (_exptl),
 // except for a joint refinement (e.g. X-ray + neutron data).
@@ -262,14 +261,23 @@
   std::string link_id;  // _struct_conn.ccp4_link_id (== _chem_link.id)
   Type type = Unknown;
   Asu asu = Asu::Any;
   AtomAddress partner1, partner2;
   double reported_distance = 0.0;
 };
 
+// Corresponds to CISPEP or _struct_mon_prot_cis
+struct CisPep {
+  AtomAddress partner_c, partner_n;
+  std::string model_str;
+  // mmCIF has (unused by the PDB) tag _struct_mon_prot_cis.label_alt_id
+  // that enables defining CIS link per conformation.
+  char only_altloc = '\0';
+  double reported_angle = NAN;
+};
 
 // Secondary structure. PDBx/mmCIF stores helices and sheets separately.
 
 // mmCIF spec defines 32 possible values for _struct_conf.conf_type_id -
 // "the type of the conformation of the backbone of the polymer (whether
 // protein or nucleic acid)". But as of 2019 only HELX_P is used (not counting
 // TURN_P that occurs in only 6 entries). The actual helix type is given
```

### Comparing `gemmi-0.6.0/include/gemmi/mmcif.hpp` & `gemmi-0.6.1/include/gemmi/mmcif.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/mmcif_impl.hpp` & `gemmi-0.6.1/include/gemmi/mmcif_impl.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/mmdb.hpp` & `gemmi-0.6.1/include/gemmi/mmdb.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -50,28 +50,14 @@
       mmdb::PChain chain2 = model2->CreateChain(chain.name.c_str());
       for (const Residue& res : chain.residues) {
         const char icode[2] = {res.seqid.icode, '\0'};
         mmdb::PResidue res2 = chain2->GetResidueCreate(res.name.c_str(),
                                                        *res.seqid.num,
                                                        icode,
                                                        true);
-        if (res.is_cis) {
-          if (const Residue* next = chain.next_residue(res)) {
-            mmdb::CisPep* cispep = new mmdb::CisPep();
-            cispep->serNum = model2->GetCisPeps()->Length() + 1;
-            strcpy_to_mmdb(cispep->chainID1, chain.name);
-            strcpy_to_mmdb(cispep->pep1, res.name);
-            set_seqid_in_mmdb(&cispep->seqNum1, cispep->icode1, res.seqid);
-            strcpy_to_mmdb(cispep->chainID2, chain.name);
-            strcpy_to_mmdb(cispep->pep2, next->name);
-            set_seqid_in_mmdb(&cispep->seqNum2, cispep->icode2, next->seqid);
-            cispep->modNum = imodel;
-            model2->AddCisPep(cispep);
-          }
-        }
         for (const Atom& atom : res.atoms) {
           mmdb::PAtom atom2 = mmdb::newAtom();
           const char altloc[2] = {atom.altloc, '\0'};
           atom2->SetAtomName(0, atom.serial, atom.padded_name().c_str(),
                              altloc, res.segment.c_str(), atom.element.uname());
           atom2->Het = res.het_flag == 'H';
           atom2->SetCharge(atom.charge);
@@ -96,14 +82,15 @@
           atom2->MakeTer();
           atom2->serNum = res.atoms.back().serial + 1;
           res2->AddAtom(atom2);
         }
       }
     }
     int n_model = manager->AddModel(model2);
+    // currently we don't setup CisPeps, so this doesn't do anything
     manager->GetModel(n_model)->CopyCisPeps(model2);
     manager->PutCell(st.cell.a, st.cell.b, st.cell.c,
                      st.cell.alpha, st.cell.beta, st.cell.gamma, 1);
     manager->SetSpaceGroup(st.spacegroup_hm.c_str());
     mmdb::Cryst* cryst = manager->GetCrystData();
     auto z = st.info.find("_cell.Z_PDB");
     if (z != st.info.end() && !z->second.empty()) {
```

### Comparing `gemmi-0.6.0/include/gemmi/mmread.hpp` & `gemmi-0.6.1/include/gemmi/mmread.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/mmread_gz.hpp` & `gemmi-0.6.1/include/gemmi/mmread_gz.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/model.hpp` & `gemmi-0.6.1/include/gemmi/model.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,14 @@
   static const char* what() { return "Residue"; }
 
   std::string subchain;   // mmCIF _atom_site.label_asym_id
   std::string entity_id;  // mmCIF _atom_site.label_entity_id
   OptionalNum label_seq;  // mmCIF _atom_site.label_seq_id
   EntityType entity_type = EntityType::Unknown;
   char het_flag = '\0';   // 'A' = ATOM, 'H' = HETATM, 0 = unspecified
-  bool is_cis = false;    // bond to the next residue marked as cis
   char flag = '\0';       // custom flag
   SiftsUnpResidue sifts_unp;  // UniProt reference from SIFTS
   short group_idx = 0;        // ignore - internal variable
   std::vector<Atom> atoms;
 
   Residue() = default;
   explicit Residue(const ResidueId& rid) noexcept : ResidueId(rid) {}
@@ -184,15 +183,14 @@
   // copy all but atoms (children) - for use in templates
   Residue empty_copy() const {
     Residue res((ResidueId&)*this);
     res.subchain = subchain;
     res.label_seq = label_seq;
     res.entity_type = entity_type;
     res.het_flag = het_flag;
-    res.is_cis = is_cis;
     res.flag = flag;
     return res;
   }
   using child_type = Atom;
   std::vector<Atom>& children() { return atoms; }
   const std::vector<Atom>& children() const { return atoms; }
 
@@ -851,14 +849,15 @@
   std::string name;
   UnitCell cell;
   std::string spacegroup_hm;  // usually pdb symbol, cf. SpaceGroup::pdb_name()
   std::vector<Model> models;
   std::vector<NcsOp> ncs;
   std::vector<Entity> entities;
   std::vector<Connection> connections;
+  std::vector<CisPep> cispeps;
   std::vector<Helix> helices;
   std::vector<Sheet> sheets;
   std::vector<Assembly> assemblies;
   Metadata meta;
 
   CoorFormat input_format = CoorFormat::Unknown;
   bool has_d_fraction = false;  // uses Refmac's ccp4_deuterium_fraction
@@ -892,14 +891,17 @@
   const Model& first_model() const {
     return const_cast<Structure*>(this)->first_model();
   }
 
   Model* find_model(const std::string& model_name) {
     return impl::find_or_null(models, model_name);
   }
+  const Model* find_model(const std::string& model_name) const {
+    return const_cast<Structure*>(this)->find_model(model_name);
+  }
   Model& find_or_add_model(const std::string& model_name) {
     return impl::find_or_add(models, model_name);
   }
 
   void remove_model(const std::string& model_name) {
     models.erase(impl::find_iter(models, model_name));
   }
```

### Comparing `gemmi-0.6.0/include/gemmi/modify.hpp` & `gemmi-0.6.1/include/gemmi/modify.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/monlib.hpp` & `gemmi-0.6.1/include/gemmi/monlib.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -316,84 +316,9 @@
   std::string error;
   bool ok = monlib.read_monomer_lib(monomer_dir, resnames, read_cif, &error);
   if (!ignore_missing && !ok)
     fail(error + "Please create definitions for missing monomers.");
   return monlib;
 }
 
-
-struct BondIndex {
-  const Model& model;
-
-  struct AtomImage {
-    int atom_serial;
-    bool same_image;
-    bool operator==(const AtomImage& o) const {
-      return atom_serial == o.atom_serial && same_image == o.same_image;
-    }
-  };
-  std::map<int, std::vector<AtomImage>> index;
-
-  BondIndex(const Model& model_) : model(model_) {
-    for (const_CRA cra : model.all())
-      if (!index.emplace(cra.atom->serial, std::vector<AtomImage>()).second)
-        fail("duplicated serial numbers");
-  }
-
-  void add_oneway_link(const Atom& a, const Atom& b, bool same_image) {
-    std::vector<AtomImage>& list_a = index.at(a.serial);
-    AtomImage ai{b.serial, same_image};
-    if (!in_vector(ai, list_a))
-      list_a.push_back(ai);
-  }
-
-  void add_link(const Atom& a, const Atom& b, bool same_image) {
-    add_oneway_link(a, b, same_image);
-    add_oneway_link(b, a, same_image);
-  }
-
-  void add_monomer_bonds(MonLib& monlib) {
-    for (const Chain& chain : model.chains)
-      for (const Residue& res : chain.residues) {
-        std::string altlocs;
-        add_distinct_altlocs(res, altlocs);
-        if (altlocs.empty())
-          altlocs += '*';
-        auto monomer = monlib.monomers.find(res.name);
-        if (monomer == monlib.monomers.end())
-          fail("Monomer description not found: " + res.name);
-        for (const Restraints::Bond& bond : monomer->second.rt.bonds)
-          for (char alt : altlocs)
-            if (const Atom* at1 = res.find_atom(bond.id1.atom, alt))
-              if (const Atom* at2 = res.find_atom(bond.id2.atom, alt)) {
-                add_link(*at1, *at2, true);
-                if (!at1->altloc && !at2->altloc)
-                  break;
-              }
-      }
-  }
-
-  bool are_linked(const Atom& a, const Atom& b, bool same_image) const {
-    return in_vector({b.serial, same_image}, index.at(a.serial));
-  }
-
-  int graph_distance(const Atom& a, const Atom& b, bool same_image,
-                     int max_distance=4) const {
-    std::vector<AtomImage> neighbors(1, {a.serial, true});
-    for (int distance = 1; distance <= max_distance; ++distance) {
-      for (size_t n = neighbors.size(); n--; ) {
-        for (AtomImage ai : index.at(neighbors[n].atom_serial)) {
-          if (!neighbors[n].same_image)
-            ai.same_image = !ai.same_image;
-          if (ai.atom_serial == b.serial && ai.same_image == same_image)
-            return distance;
-          if (!in_vector(ai, neighbors))
-            neighbors.push_back(ai);
-        }
-      }
-    }
-    return max_distance + 1;
-  }
-};
-
 } // namespace gemmi
 #endif
```

### Comparing `gemmi-0.6.0/include/gemmi/mtz.hpp` & `gemmi-0.6.1/include/gemmi/mtz.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 // MTZ reflection file format.
 
 #ifndef GEMMI_MTZ_HPP_
 #define GEMMI_MTZ_HPP_
 
 #include <cassert>
 #include <cstdint>       // for int32_t
-#include <cstdio>        // for FILE, fprintf
 #include <cstring>       // for memcpy
 #include <cmath>         // for isnan
 #include <algorithm>     // for sort, any_of
 #include <array>
 #include <initializer_list>
+#include <ostream>
 #include <string>
 #include <vector>
 #include "atox.hpp"      // for simple_atoi, read_word
 #include "atof.hpp"      // for fast_atof
 #include "input.hpp"     // for FileStream, CharArray
 #include "iterator.hpp"  // for StrideIter
 #include "fail.hpp"      // for fail
@@ -177,15 +177,16 @@
   std::vector<Dataset> datasets;
   std::vector<Column> columns;
   std::vector<Batch> batches;
   std::vector<std::string> history;
   std::string appended_text;
   std::vector<float> data;
 
-  FILE* warnings = nullptr;
+  // stream used for warnings when reading mtz file (and also in mtz2cif)
+  std::ostream* warnings = nullptr;
 
   explicit Mtz(bool with_base=false) {
     if (with_base)
       add_base();
   }
   Mtz(Mtz&& o) noexcept { *this = std::move(o); }
   Mtz& operator=(Mtz&& o) noexcept {
@@ -515,17 +516,17 @@
     double c = fast_atof(line, &line);
     double alpha = fast_atof(line, &line);
     double beta = fast_atof(line, &line);
     double gamma = fast_atof(line, &line);
     return UnitCell(a, b, c, alpha, beta, gamma);
   }
 
-  void warn(const std::string& text) const {
+  template<typename T> void warn(const T& text) const {
     if (warnings)
-      std::fprintf(warnings, "%s\n", text.c_str());
+      *warnings << text << std::endl;
   }
 
   template<typename Stream>
   void seek_headers(Stream& stream) {
     std::ptrdiff_t pos = 4 * std::ptrdiff_t(header_offset - 1);
     if (!stream.seek(pos))
       fail("Cannot rewind to the MTZ header at byte " + std::to_string(pos));
@@ -816,74 +817,19 @@
     return {{(int)data[offset], (int)data[offset+1], (int)data[offset+2]}};
   }
   void set_hkl(size_t offset, const Miller& hkl) {
     for (int i = 0; i != 3; ++i)
       data[offset + i] = static_cast<float>(hkl[i]);
   }
 
-  // (for merged MTZ only) change HKL to ASU equivalent, adjust phases
-  void ensure_asu(bool tnt_asu=false) {
-    if (!is_merged())
-      fail("Mtz::ensure_asu() is for merged MTZ only");
-    if (!spacegroup)
-      return;
-    GroupOps gops = spacegroup->operations();
-    ReciprocalAsu asu(spacegroup, tnt_asu);
-    std::vector<int> phase_columns = positions_of_columns_with_type('P');
-    std::vector<int> abcd_columns = positions_of_columns_with_type('A');
-    std::vector<int> dano_columns = positions_of_columns_with_type('D');
-    std::vector<std::pair<int,int>> plus_minus_columns = positions_of_plus_minus_columns();
-    bool no_special_columns = phase_columns.empty() && abcd_columns.empty() &&
-                              plus_minus_columns.empty() && dano_columns.empty();
-    bool centric = no_special_columns || gops.is_centrosymmetric();
-    for (size_t n = 0; n < data.size(); n += columns.size()) {
-      Miller hkl = get_hkl(n);
-      if (asu.is_in(hkl))
-        continue;
-      auto result = asu.to_asu(hkl, gops);
-      // cf. impl::move_to_asu() in asudata.hpp
-      set_hkl(n, result.first);
-      if (no_special_columns)
-        continue;
-      int isym = result.second;
-      if (!phase_columns.empty() || !abcd_columns.empty()) {
-        const Op& op = gops.sym_ops[(isym - 1) / 2];
-        double shift = op.phase_shift(hkl);
-        if (shift != 0) {
-          if (isym % 2 == 0)
-            shift = -shift;
-          double shift_deg = deg(shift);
-          for (int col : phase_columns)
-            data[n + col] = float(data[n + col] + shift_deg);
-          for (auto i = abcd_columns.begin(); i+3 < abcd_columns.end(); i += 4) {
-            double sinx = std::sin(shift);
-            double cosx = std::cos(shift);
-            double sin2x = 2 * sinx * cosx;
-            double cos2x = sq(cosx)- sq(sinx);
-            double a = data[n + *(i+0)];
-            double b = data[n + *(i+1)];
-            double c = data[n + *(i+2)];
-            double d = data[n + *(i+3)];
-            // a sin(x+y) + b cos(x+y) = a sin(x) cos(y) - b sin(x) sin(y)
-            //                         + a cos(x) sin(y) + b cos(x) cos(y)
-            data[n + *(i+0)] = float(a * cosx - b * sinx);
-            data[n + *(i+1)] = float(a * sinx + b * cosx);
-            data[n + *(i+2)] = float(c * cos2x - d * sin2x);
-            data[n + *(i+3)] = float(c * sin2x + d * cos2x);
-          }
-        }
-      }
-      if (isym % 2 == 0 && !centric) {
-        for (std::pair<int,int> cols : plus_minus_columns)
-          std::swap(data[n + cols.first], data[n + cols.second]);
-        for (int col : dano_columns)
-          data[n + col] = -data[n + col];
-      }
-    }
-  }
+  /// (for merged MTZ only) change HKL to ASU equivalent, adjust phases, etc
+  void ensure_asu(bool tnt_asu=false);
+
+  /// reindex data, usually followed by ensure_asu()
+  void reindex(const Op& op, std::ostream* out);
 
   // (for unmerged MTZ only) change HKL according to M/ISYM
   bool switch_to_original_hkl() {
     if (indices_switched_to_original)
       return false;
     if (!has_data())
       fail("switch_to_original_hkl(): data not read yet");
@@ -988,16 +934,15 @@
       Column& dst = columns[dest_idx + i];
       const Column& src = src_mtz->columns[src_col.idx + i];
       dst.type = src.type;
       dst.label = src.label;
       dst.min_value = src.min_value;
       dst.max_value = src.max_value;
       dst.source = src.source;
-      if (src_mtz == this)
-        dst.dataset_id = src.dataset_id;
+      dst.dataset_id = src.dataset_id;
     }
     if (src_mtz == this) {
       // internal copying
       for (size_t n = 0; n < data.size(); n += columns.size())
         for (size_t i = 0; i <= trailing_cols.size(); ++i)
           data[n + dest_idx + i] = data[n + src_col.idx + i];
     } else {
@@ -1056,14 +1001,15 @@
         col_idx += 1 + (int)trailing_cols.size();
     }
     for (int i = 0; i <= (int) trailing_cols.size(); ++i)
       add_column("", ' ', -1, dest_idx + i, false);
     expand_data_rows(1 + trailing_cols.size(), dest_idx);
     // copy the data
     const Column& src_col_now = col_idx < 0 ? src_col : columns[col_idx];
+    // most of the work (hkl-based row matching and data copying) is done here:
     do_replace_column(dest_idx, src_col_now, trailing_cols);
     return columns[dest_idx];
   }
 
   void remove_column(size_t idx) {
     check_column(idx, "remove_column()");
     columns.erase(columns.begin() + idx);
```

### Comparing `gemmi-0.6.0/include/gemmi/mtz2cif.hpp` & `gemmi-0.6.1/include/gemmi/mtz2cif.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 //  - check that the FP column is not from Refmac
 //  - should we allow for repeated column names in MTZ?
 
 #ifndef GEMMI_MTZ2CIF_HPP_
 #define GEMMI_MTZ2CIF_HPP_
 
 #include <ostream>
-#include <unordered_map>
 #include "mtz.hpp"       // for Mtz
 #include "xds_ascii.hpp" // for XdsAscii
 #include "merge.hpp"     // for Intensities
 
 namespace gemmi {
 
 class GEMMI_DLL MtzToCif {
```

### Comparing `gemmi-0.6.0/include/gemmi/neighbor.hpp` & `gemmi-0.6.1/include/gemmi/neighbor.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 #include "small.hpp"
 
 namespace gemmi {
 
 struct NeighborSearch {
 
   struct Mark {
-    float x, y, z;
+    Position pos;
     char altloc;
     Element element;
-    int image_idx;
+    short image_idx;
     int chain_idx;
     int residue_idx;
     int atom_idx;
 
-    Mark(const Position& p, char alt, El el, int im, int ch, int res, int atom)
-    : x(float(p.x)), y(float(p.y)), z(float(p.z)), altloc(alt), element(el),
+    Mark(const Position& p, char alt, El el, short im, int ch, int res, int atom)
+    : pos(p), altloc(alt), element(el),
       image_idx(im), chain_idx(ch), residue_idx(res), atom_idx(atom) {}
 
-    Position pos() const { return {x, y, z}; }
-
     CRA to_cra(Model& mdl) const {
       Chain& c = mdl.chains.at(chain_idx);
       Residue& r = c.residues.at(residue_idx);
       Atom& a = r.atoms.at(atom_idx);
       return {&c, &r, &a};
     }
     const_CRA to_cra(const Model& mdl) const {
@@ -47,134 +45,168 @@
     }
     SmallStructure::Site& to_site(SmallStructure& small) const {
       return small.sites.at(atom_idx);
     }
     const SmallStructure::Site& to_site(const SmallStructure& small) const {
       return small.sites.at(atom_idx);
     }
-    // Here the point p must not be across PBC boundary,
-    // typically p is orthogonalized Fractional in for_each_cell.
-    float dist_sq_(const Position& p) const {
-      return sq((float)p.x - x) + sq((float)p.y - y) + sq((float)p.z - z);
-    }
   };
 
   Grid<std::vector<Mark>> grid;
   double radius_specified = 0.;
   Model* model = nullptr;
   SmallStructure* small_structure = nullptr;
+  bool use_pbc = true;
   bool include_h = true;
 
   NeighborSearch() = default;
   // Model is not const so it can be modified in for_each_contact()
-  NeighborSearch(Model& model_, const UnitCell& cell, double max_radius) {
+  NeighborSearch(Model& model_, const UnitCell& cell, double radius) {
     model = &model_;
-    radius_specified = max_radius;
+    radius_specified = radius;
     set_bounding_cell(cell);
     set_grid_size();
   }
-  NeighborSearch(SmallStructure& small, double max_radius) {
+  NeighborSearch(SmallStructure& small, double radius) {
     small_structure = &small;
-    radius_specified = max_radius;
+    radius_specified = radius;
     grid.unit_cell = small.cell;
     set_grid_size();
   }
 
   NeighborSearch& populate(bool include_h_=true);
   void add_chain(const Chain& chain, bool include_h_=true);
   void add_chain_n(const Chain& chain, int n_ch);
   void add_atom(const Atom& atom, int n_ch, int n_res, int n_atom);
   void add_site(const SmallStructure::Site& site, int n);
 
-  // assumes data in [0, 1), but uses index_n to handle numeric deviations
+  // assumes data in [0, 1), but uses index_n to account for numerical errors
   std::vector<Mark>& get_subcell(const Fractional& fr) {
     return grid.data[grid.index_n(int(fr.x * grid.nu),
                                   int(fr.y * grid.nv),
                                   int(fr.z * grid.nw))];
   }
 
   template<typename Func>
-  void for_each_cell(const Position& pos, const Func& func);
+  void for_each_cell(const Position& pos, const Func& func, int k=1);
+
   template<typename Func>
-  void for_each(const Position& pos, char alt, float radius, const Func& func);
+  void for_each(const Position& pos, char alt, double radius, const Func& func, int k=1) {
+    if (radius <= 0)
+      return;
+    for_each_cell(pos, [&](std::vector<Mark>& marks, const Fractional& fr) {
+        Position p = use_pbc ? grid.unit_cell.orthogonalize(fr) : pos;
+        for (Mark& m : marks) {
+          double dist_sq = m.pos.dist_sq(p);
+          if (dist_sq < sq(radius) && is_same_conformer(alt, m.altloc))
+            func(m, dist_sq);
+        }
+    }, k);
+  }
 
-  // with radius==0 it uses radius_specified
-  std::vector<Mark*> find_atoms(const Position& pos, char alt, float radius) {
-    if (radius == 0.f)
-      radius = (float) radius_specified;
-    std::vector<Mark*> out;
-    for_each(pos, alt, radius, [&out](Mark& a, float) { out.push_back(&a); });
-    return out;
+  int sufficient_k(double r) const {
+    // .00001 is added to account for possible numeric error in r
+    return r <= radius_specified ? 1 : int(r / radius_specified + 1.00001);
   }
 
-  // with max_dist==0 it uses radius_specified
-  std::vector<Mark*> find_neighbors_(const Position& pos, char altloc,
-                                     float min_dist, float max_dist) {
+  // with radius==0 it uses radius_specified
+  std::vector<Mark*> find_atoms(const Position& pos, char alt,
+                                double min_dist, double radius) {
+    int k = sufficient_k(radius);
+    if (radius == 0)
+      radius = radius_specified;
     std::vector<Mark*> out;
-    if (max_dist == 0.f)
-      max_dist = (float) radius_specified;
-    for_each(pos, altloc, max_dist, [&](Mark& a, float dist_sq) {
+    for_each(pos, alt, radius, [&](Mark& a, double dist_sq) {
         if (dist_sq >= sq(min_dist))
           out.push_back(&a);
-    });
+    }, k);
     return out;
   }
-  std::vector<Mark*> find_neighbors(const Atom& atom,
-                                    float min_dist, float max_dist) {
-    return find_neighbors_(atom.pos, atom.altloc, min_dist, max_dist);
+
+  std::vector<Mark*> find_neighbors(const Atom& atom, double min_dist, double max_dist) {
+    return find_atoms(atom.pos, atom.altloc, min_dist, max_dist);
   }
   std::vector<Mark*> find_site_neighbors(const SmallStructure::Site& site,
-                                         float min_dist, float max_dist) {
+                                         double min_dist, double max_dist) {
     Position pos = grid.unit_cell.orthogonalize(site.fract);
-    return find_neighbors_(pos, '\0', min_dist, max_dist);
+    return find_atoms(pos, '\0', min_dist, max_dist);
   }
 
-  Mark* find_nearest_atom(const Position& pos) {
+  std::pair<Mark*, double>
+  find_nearest_atom_within_k(const Position& pos, int k, double radius) {
     Mark* mark = nullptr;
-    float nearest_dist_sq = float(radius_specified * radius_specified);
+    double nearest_dist_sq = radius * radius;
     for_each_cell(pos, [&](std::vector<Mark>& marks, const Fractional& fr) {
-        Position p = grid.unit_cell.orthogonalize(fr);
+        Position p = use_pbc ? grid.unit_cell.orthogonalize(fr) : pos;
         for (Mark& m : marks) {
-          float dist_sq = m.dist_sq_(p);
+          double dist_sq = m.pos.dist_sq(p);
           if (dist_sq < nearest_dist_sq) {
             mark = &m;
             nearest_dist_sq = dist_sq;
           }
         }
-    });
-    return mark;
+    }, k);
+    return {mark, nearest_dist_sq};
+  }
+
+  // it would be good to return also NearestImage
+  Mark* find_nearest_atom(const Position& pos, double radius=INFINITY) {
+    double r_spec = radius_specified;
+    if (radius == 0.f)
+      radius = r_spec;
+    int max_k = std::max(std::max(std::max(grid.nu, grid.nv), grid.nw), 2);
+    for (int k = 1; k < max_k; k *= 2) {
+      auto result = find_nearest_atom_within_k(pos, k, radius);
+      // if Mark was not found, result.second is set to radius^2.
+      if (result.second < sq(k * r_spec))
+        return result.first;
+      if (result.first != nullptr) {
+        // We found an atom, but because it was further away than k*r_spec,
+        // so now it's sufficient to find the nearest atom in dist:
+        double dist = std::sqrt(result.second);
+        return find_nearest_atom_within_k(pos, sufficient_k(dist), radius).first;
+      }
+    }
+    if (!use_pbc)
+      // pos can be outside of bounding box. In such case, although it's slow,
+      // search in all cells. Using large number that will be clipped.
+      return find_nearest_atom_within_k(pos, INT_MAX/4, radius).first;
+    return nullptr;
   }
 
-  float dist_sq(const Position& pos1, const Position& pos2) const {
-    return (float) grid.unit_cell.distance_sq(pos1, pos2);
+  double dist_sq(const Position& pos1, const Position& pos2) const {
+    return grid.unit_cell.distance_sq(pos1, pos2);
   }
-  float dist(const Position& pos1, const Position& pos2) const {
+  double dist(const Position& pos1, const Position& pos2) const {
     return std::sqrt(dist_sq(pos1, pos2));
   }
 
   FTransform get_image_transformation(int image_idx) const {
     // 0 is for identity, other indices are shifted by one.
     if (image_idx == 0)
       return Transform{};
     if ((size_t)image_idx <= grid.unit_cell.images.size())
       return grid.unit_cell.images[image_idx-1];
     fail("No such image index: " + std::to_string(image_idx));
   }
 
 private:
   void set_grid_size() {
-    grid.set_size_from_spacing(radius_specified, GridSizeRounding::Down);
-    if (grid.nu < 3 || grid.nv < 3 || grid.nw < 3)
-      grid.set_size_without_checking(std::max(grid.nu, 3),
-                                     std::max(grid.nv, 3),
-                                     std::max(grid.nw, 3));
+    // We don't use set_size_from_spacing() etc because we don't need
+    // FFT-friendly size nor symmetry.
+    double inv_radius = 1 / radius_specified;
+    const UnitCell& uc = grid.unit_cell;
+    grid.set_size_without_checking(std::max(int(inv_radius / uc.ar), 1),
+                                   std::max(int(inv_radius / uc.br), 1),
+                                   std::max(int(inv_radius / uc.cr), 1));
   }
 
   void set_bounding_cell(const UnitCell& cell) {
-    if (cell.is_crystal()) {
+    use_pbc = cell.is_crystal();
+    if (use_pbc) {
       grid.unit_cell = cell;
     } else {
       // cf. calculate_box()
       Box<Position> box;
       for (CRA cra : model->all())
         box.extend(cra.atom->pos);
       // The box needs to include all NCS images (strict NCS from MTRIXn).
@@ -184,17 +216,19 @@
       if (!ncs.empty()) {
         for (CRA cra : model->all())
           // images store fractional transforms, but for non-crystal
           // it should be the same as Cartesian transform.
           for (const Transform& tr : ncs)
             box.extend(Position(tr.apply(cra.atom->pos)));
       }
-      box.add_margin(1.5 * radius_specified);  // much more than needed
+      box.add_margin(0.01);
       Position size = box.get_size();
       grid.unit_cell.set(size.x, size.y, size.z, 90, 90, 90);
+      grid.unit_cell.frac.vec -= grid.unit_cell.fractionalize(box.minimum);
+      grid.unit_cell.orth.vec += box.minimum;
       for (const Transform& tr : ncs) {
         UnitCell& c = grid.unit_cell;
         // cf. add_ncs_images_to_cs_images()
         c.images.push_back(c.frac.combine(tr.combine(c.orth)));
       }
     }
   }
@@ -243,23 +277,24 @@
 
 inline void NeighborSearch::add_atom(const Atom& atom,
                                      int n_ch, int n_res, int n_atom) {
   const UnitCell& gcell = grid.unit_cell;
   Fractional frac0 = gcell.fractionalize(atom.pos);
   {
     Fractional frac = frac0.wrap_to_unit();
-    Position pos = gcell.orthogonalize(frac);
+    // for non-crystals, frac==frac0 => pos = atom.pos
+    Position pos = use_pbc ? gcell.orthogonalize(frac) : atom.pos;
     get_subcell(frac).emplace_back(pos, atom.altloc, atom.element.elem,
                                    0, n_ch, n_res, n_atom);
   }
   for (int n_im = 0; n_im != (int) gcell.images.size(); ++n_im) {
     Fractional frac = gcell.images[n_im].apply(frac0).wrap_to_unit();
     Position pos = gcell.orthogonalize(frac);
     get_subcell(frac).emplace_back(pos, atom.altloc, atom.element.elem,
-                                   n_im + 1, n_ch, n_res, n_atom);
+                                   short(n_im + 1), n_ch, n_res, n_atom);
   }
 }
 
 // We exclude special position images of atoms here, but not in add_atom.
 // This choice is somewhat arbitrary, but it also reflects the fact that
 // in MX files occupances of atoms on special positions are (almost always)
 // fractional and all images are to be taken into account.
@@ -278,133 +313,61 @@
     if (gcell.distance_sq(frac, frac0) < sq(SPECIAL_POS_TOL) ||
         std::any_of(others.begin(), others.end(), [&](const Fractional& f) {
           return gcell.distance_sq(frac, f) < sq(SPECIAL_POS_TOL);
         }))
       continue;
     Position pos = gcell.orthogonalize(frac);
     get_subcell(frac).emplace_back(pos, '\0', site.element.elem,
-                                   n_im + 1, -1, -1, n);
+                                   short(n_im + 1), -1, -1, n);
     others.push_back(frac);
   }
 }
 
 template<typename Func>
-void NeighborSearch::for_each_cell(const Position& pos, const Func& func) {
-  Fractional fr = grid.unit_cell.fractionalize(pos).wrap_to_unit();
-  const int u0 = int(fr.x * grid.nu);
-  const int v0 = int(fr.y * grid.nv);
-  const int w0 = int(fr.z * grid.nw);
-  const int uend = u0 + std::min(3, grid.nu) - 1;
-  const int vend = v0 + std::min(3, grid.nv) - 1;
-  const int wend = w0 + std::min(3, grid.nw) - 1;
-  for (int w = w0 - 1; w < wend; ++w) {
-    int dw = w >= grid.nw ? -1 : w < 0 ? 1 : 0;
-    for (int v = v0 - 1; v < vend; ++v) {
-      int dv = v >= grid.nv ? -1 : v < 0 ? 1 : 0;
-      for (int u = u0 - 1; u < uend; ++u) {
-        int du = u >= grid.nu ? -1 : u < 0 ? 1 : 0;
-        size_t idx = grid.index_q(u + du * grid.nu,
-                                  v + dv * grid.nv,
-                                  w + dw * grid.nw);
-        func(grid.data[idx], Fractional(fr.x + du, fr.y + dv, fr.z + dw));
-      }
-    }
-  }
-}
-
-template<typename Func>
-void NeighborSearch::for_each(const Position& pos, char alt, float radius,
-                              const Func& func) {
-  if (radius <= 0.f)
-    return;
-  for_each_cell(pos, [&](std::vector<Mark>& marks, const Fractional& fr) {
-      Position p = grid.unit_cell.orthogonalize(fr);
-      for (Mark& m : marks) {
-        float dist_sq = m.dist_sq_(p);
-        if (dist_sq < sq(radius) && is_same_conformer(alt, m.altloc))
-          func(m, dist_sq);
-      }
-  });
-}
-
-
-inline void remove_cras(Model& model, std::vector<CRA>& vec) {
-  // sort in reverse order, so items can be erased without invalidating pointers
-  std::sort(vec.begin(), vec.end(), [](const CRA& a, const CRA& b) {
-      return std::tie(a.chain, a.residue, a.atom) > std::tie(b.chain, b.residue, b.atom);
-  });
-  const Atom* prev_a = nullptr;
-  for (CRA& cra : vec) {
-    if (cra.atom == prev_a)
-      continue;
-    prev_a = cra.atom;
-    auto atom_idx = cra.atom - cra.residue->atoms.data();
-    cra.residue->atoms.erase(cra.residue->atoms.begin() + atom_idx);
-    if (cra.residue->atoms.empty()) {
-      auto res_idx = cra.residue - cra.chain->residues.data();
-      cra.chain->residues.erase(cra.chain->residues.begin() + res_idx);
-      if (cra.chain->residues.empty()) {
-        auto chain_idx = cra.chain - model.chains.data();
-        model.chains.erase(model.chains.begin() + chain_idx);
-      }
-    }
-  }
-}
-
-// To be used after expand_ncs() and make_assembly().
-// Searches and merges overlapping equivalent atoms from different chains.
-inline void merge_atoms_in_expanded_model(Model& model, const UnitCell& cell,
-                                          double max_dist=0.2) {
-  using Mark = NeighborSearch::Mark;
-  NeighborSearch ns(model, cell, 4.0);
-  ns.populate(true);
-  std::vector<CRA> to_be_deleted;
-  for (int n_ch = 0; n_ch != (int) model.chains.size(); ++n_ch) {
-    Chain& chain = model.chains[n_ch];
-    for (int n_res = 0; n_res != (int) chain.residues.size(); ++n_res) {
-      Residue& res = chain.residues[n_res];
-      for (int n_atom = 0; n_atom != (int) res.atoms.size(); ++n_atom) {
-        Atom& atom = res.atoms[n_atom];
-        std::vector<std::pair<CRA, int>> equiv;
-        ns.for_each_cell(atom.pos, [&](std::vector<Mark>& marks, const Fractional& fr) {
-            for (Mark& m : marks) {
-              // We look for the same atoms, but copied to a different chain.
-              // First quick check that filters out most of non-matching pairs.
-              if (m.altloc != atom.altloc || m.element != atom.element ||
-                  m.chain_idx == n_ch || m.atom_idx != n_atom)
-                continue;
-              // Now check if everything else matches.
-              CRA cra = m.to_cra(model);
-              if (cra.atom &&
-                  cra.atom->serial == atom.serial &&
-                  cra.atom->name == atom.name &&
-                  cra.atom->b_iso == atom.b_iso &&
-                  cra.residue->matches_noseg(res) &&
-                  m.dist_sq_(ns.grid.unit_cell.orthogonalize(fr)) < sq(max_dist))
-                equiv.emplace_back(cra, m.image_idx);
-            }
-        });
-        if (!equiv.empty()) {
-          Position pos_sum = atom.pos;
-          for (auto& t : equiv) {
-            CRA& cra = t.first;
-            pos_sum += ns.grid.unit_cell.find_nearest_pbc_position(
-                                          atom.pos, cra.atom->pos, t.second);
-            // The atoms in equiv are to be discarded later.
-            // Deleting now would invalidate indices in NeighborSearch.
-            to_be_deleted.push_back(cra);
-            // Modify the atoms to avoid processing them again.
-            cra.atom->serial = -1;  // this should be enough
-            cra.atom->name.clear(); // this is just in case
-          }
-          size_t n = 1 + equiv.size();
-          atom.pos = pos_sum / double(n);
-          atom.occ = std::min(1.f, n * atom.occ);
+void NeighborSearch::for_each_cell(const Position& pos, const Func& func, int k) {
+  Fractional fr = grid.unit_cell.fractionalize(pos);
+  if (use_pbc)
+    fr = fr.wrap_to_unit();
+  int u0 = int(fr.x * grid.nu) - k;
+  int v0 = int(fr.y * grid.nv) - k;
+  int w0 = int(fr.z * grid.nw) - k;
+  int uend = u0 + 2 * k + 1;
+  int vend = v0 + 2 * k + 1;
+  int wend = w0 + 2 * k + 1;
+  if (use_pbc) {
+    auto shift = [](int j, int n) {
+      if (j < 0)
+        return (j + 1) / n - 1;
+      if (j >= n)
+        return j / n;
+      return 0;
+    };
+    for (int w = w0; w < wend; ++w) {
+      int dw = shift(w, grid.nw);
+      for (int v = v0; v < vend; ++v) {
+        int dv = shift(v, grid.nv);
+        size_t idx0 = grid.index_q(0, v - dv * grid.nv, w - dw * grid.nw);
+        for (int u = u0; u < uend; ++u) {
+          int du = shift(u, grid.nu);
+          size_t idx = idx0 + (u - du * grid.nu);
+          func(grid.data[idx], Fractional(fr.x - du, fr.y - dv, fr.z - dw));
         }
       }
     }
+  } else {
+    u0 = std::max(0, u0);
+    v0 = std::max(0, v0);
+    w0 = std::max(0, w0);
+    uend = std::min(uend, grid.nu);
+    vend = std::min(vend, grid.nv);
+    wend = std::min(wend, grid.nw);
+    for (int w = w0; w < wend; ++w)
+      for (int v = v0; v < vend; ++v)
+        for (int u = u0; u < uend; ++u) {
+          size_t idx = grid.index_q(u, v, w);
+          func(grid.data[idx], fr);
+        }
   }
-  remove_cras(model, to_be_deleted);
 }
 
 } // namespace gemmi
 #endif
```

### Comparing `gemmi-0.6.0/include/gemmi/neutron92.hpp` & `gemmi-0.6.1/include/gemmi/neutron92.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/numb.hpp` & `gemmi-0.6.1/include/gemmi/numb.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/pdb.hpp` & `gemmi-0.6.1/include/gemmi/pdb.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -195,19 +195,25 @@
           c.reported_distance = read_double(&record[73], 5);
       }
       st.connections.emplace_back(c);
     } else if (record[0] == 'C' || record[0] == 'c') { // CISPEP
       if (record.length() < 22)
         continue;
       const char* r = record.c_str();
-      std::string cname = read_string(r + 14, 2);
-      ResidueId rid = read_res_id(r + 17, r + 11);
-      for (Model& model : st.models)
-        if (Residue* res = model.find_residue(cname, rid))
-          res->is_cis = true;
+      CisPep cispep;
+      cispep.partner_c.chain_name = read_string(r + 14, 2);
+      cispep.partner_c.res_id = read_res_id(r + 17, r + 11);
+      cispep.partner_n.chain_name = read_string(r + 28, 2);
+      cispep.partner_n.res_id = read_res_id(r + 31, r + 25);
+      // In files with a single model in the PDB CISPEP modNum is 0,
+      // but _struct_mon_prot_cis.pdbx_PDB_model_num is 1.
+      cispep.model_str = st.models.size() == 1 ? st.models[0].name
+                                               : read_string(r + 43, 3);
+      cispep.reported_angle = read_double(r + 53, 6);
+      st.cispeps.push_back(cispep);
     }
   }
 }
 
 template<typename Stream>
 Structure read_pdb_from_stream(Stream&& stream, const std::string& source,
                                const PdbReadOptions& options) {
```

### Comparing `gemmi-0.6.0/include/gemmi/pirfasta.hpp` & `gemmi-0.6.1/include/gemmi/pirfasta.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/polyheur.hpp` & `gemmi-0.6.1/include/gemmi/polyheur.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 #ifndef GEMMI_POLYHEUR_HPP_
 #define GEMMI_POLYHEUR_HPP_
 
 #include <vector>
 #include "model.hpp"
 #include "resinfo.hpp"   // for find_tabulated_residue
-#include "calculate.hpp" // for calculate_omega
 #include "util.hpp"      // for vector_remove_if
 
 namespace gemmi {
 
 // A simplistic classification. It may change in the future.
 // It returns PolymerType which corresponds to _entity_poly.type,
 // but here we use only PeptideL, Rna, Dna, DnaRnaHybrid and Unknown.
@@ -83,25 +82,29 @@
   if (is_polynucleotide(ptype))
     return have_nucleotide_bond(r1, r2);
   return false;
 }
 
 /// are_connected2() is less exact, but requires only CA (or P) atoms.
 inline bool are_connected2(const Residue& r1, const Residue& r2, PolymerType ptype) {
-  auto this_or_first = [](const Atom* a, const Residue& r) -> const Atom* {
-    return a || r.atoms.empty() ? a : &r.atoms.front();
+  auto this_or_first = [](const Atom* a, const Residue& r, El el) -> const Atom* {
+    if (a || r.atoms.empty())
+      return a;
+    if (const Atom* b = r.find_by_element(el))
+      return b;
+    return &r.atoms.front();
   };
   if (is_polypeptide(ptype)) {
-    const Atom* a1 = this_or_first(r1.get_ca(), r1);
-    const Atom* a2 = this_or_first(r2.get_ca(), r2);
+    const Atom* a1 = this_or_first(r1.get_ca(), r1, El::C);
+    const Atom* a2 = this_or_first(r2.get_ca(), r2, El::C);
     return a1 && a2 && a1->pos.dist_sq(a2->pos) < sq(5.0);
   }
   if (is_polynucleotide(ptype)) {
-    const Atom* a1 = this_or_first(r1.get_p(), r1);
-    const Atom* a2 = this_or_first(r2.get_p(), r2);
+    const Atom* a1 = this_or_first(r1.get_p(), r1, El::P);
+    const Atom* a2 = this_or_first(r2.get_p(), r2, El::P);
     return a1 && a2 && a1->pos.dist_sq(a2->pos) < sq(7.5);
   }
   return false;
 }
 
 /// are_connected3() = are_connected() + fallback to are_connected2()
 inline bool are_connected3(const Residue& r1, const Residue& r2, PolymerType ptype) {
@@ -167,31 +170,14 @@
 inline void setup_entities(Structure& st) {
   add_entity_types(st, /*overwrite=*/false);
   assign_subchains(st, /*force=*/false);
   ensure_entities(st);
   deduplicate_entities(st);
 }
 
-/// Assign Residue::is_cis based on the omega angle of the first conformer
-template<class T> void assign_cis_flags(T& obj) {
-  for (auto& child : obj.children())
-    assign_cis_flags(child);
-}
-inline void assign_cis_flags(Chain& chain) {
-  for (Residue& res : chain.residues) {
-    bool cis = false;
-    if (res.entity_type == EntityType::Polymer)
-      if (const Residue* next = chain.next_residue(res))
-        if (have_peptide_bond(res, *next))
-          if (std::fabs(calculate_omega(res, *next)) < rad(30.))
-            cis = true;
-    res.is_cis = cis;
-  }
-}
-
 // Remove waters. It may leave empty chains.
 template<class T> void remove_waters(T& obj) {
   for (auto& child : obj.children())
     remove_waters(child);
 }
 template<> inline void remove_waters(Chain& ch) {
   vector_remove_if(ch.residues,
```

### Comparing `gemmi-0.6.0/include/gemmi/qcp.hpp` & `gemmi-0.6.1/include/gemmi/qcp.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/read_cif.hpp` & `gemmi-0.6.1/include/gemmi/read_cif.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/read_map.hpp` & `gemmi-0.6.1/include/gemmi/read_map.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/recgrid.hpp` & `gemmi-0.6.1/include/gemmi/recgrid.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/reciproc.hpp` & `gemmi-0.6.1/include/gemmi/reciproc.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/refln.hpp` & `gemmi-0.6.1/include/gemmi/refln.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/remarks.hpp` & `gemmi-0.6.1/include/gemmi/remarks.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,14 @@
           }
         }
       }
       if (istarts_with(item.version, "version "))
         item.version.erase(0, 8);
     }
     item.classification = type;
-    item.pdbx_ordinal = (int) meta.software.size();
   }
 }
 
 // REMARK   3   TERM                          COUNT    WEIGHT   FUNCTION.
 // REMARK   3    BOND LENGTHS              : 5760   ; 2.000  ; HARMONIC
 inline void add_restraint_count_weight(RefinementInfo& ref_info,
                                        const char* key, const char* value) {
```

### Comparing `gemmi-0.6.0/include/gemmi/resinfo.hpp` & `gemmi-0.6.1/include/gemmi/resinfo.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/riding_h.hpp` & `gemmi-0.6.1/include/gemmi/riding_h.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 #define GEMMI_RIDING_H_HPP_
 
 #include <cmath>         // for isnan
 #include "topo.hpp"      // for Topo
 
 namespace gemmi {
 
-GEMMI_DLL void add_hydrogens_without_positions(Topo::ResInfo& ri);
 GEMMI_DLL void place_hydrogens_on_all_atoms(Topo& topo);
 
 inline void adjust_hydrogen_distances(Topo& topo, Restraints::DistanceOf of,
                                       double default_scale=1.) {
   for (const Topo::Bond& t : topo.bonds) {
     assert(t.atoms[0] != nullptr && t.atoms[1] != nullptr);
     if (t.atoms[0]->is_hydrogen() || t.atoms[1]->is_hydrogen()) {
```

### Comparing `gemmi-0.6.0/include/gemmi/scaling.hpp` & `gemmi-0.6.1/include/gemmi/scaling.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/select.hpp` & `gemmi-0.6.1/include/gemmi/select.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,16 @@
     cid += '/';
     cid += from_seqid.str();
     if (!residue_names.all) {
       cid += '(';
       cid += residue_names.str();
       cid += ')';
     }
-    if (!from_seqid.empty() || !to_seqid.empty()) {
+    if ((!from_seqid.empty() || !to_seqid.empty()) &&
+        (from_seqid.seqnum != to_seqid.seqnum || from_seqid.icode != to_seqid.icode)) {
       cid += '-';
       cid += to_seqid.str();
     }
     cid += '/';
     if (!atom_names.all)
       cid += atom_names.str();
     if (!elements.empty()) {
@@ -463,14 +464,16 @@
     if (cid[pos] == '.')
       ++pos;
     if (cid[pos] == '*')
       ++pos;
     if (cid[pos] == '-') {
       ++pos;
       sel.to_seqid = parse_cid_seqid(cid, pos, INT_MAX);
+    } else if (sel.from_seqid.seqnum != INT_MIN) {
+      sel.to_seqid = sel.from_seqid;
     }
     sep = pos;
     if (cid[sep] != '/' && cid[sep] != ';' && cid[sep] != '\0')
       wrong_syntax(cid, 0);
   }
 
   // atom;  at[el]:aloc
```

### Comparing `gemmi-0.6.0/include/gemmi/seqalign.hpp` & `gemmi-0.6.1/include/gemmi/seqalign.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/seqid.hpp` & `gemmi-0.6.1/include/gemmi/seqid.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/sfcalc.hpp` & `gemmi-0.6.1/include/gemmi/sfcalc.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/small.hpp` & `gemmi-0.6.1/include/gemmi/small.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/smcif.hpp` & `gemmi-0.6.1/include/gemmi/smcif.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/solmask.hpp` & `gemmi-0.6.1/include/gemmi/solmask.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/span.hpp` & `gemmi-0.6.1/include/gemmi/span.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/sprintf.hpp` & `gemmi-0.6.1/include/gemmi/sprintf.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/stats.hpp` & `gemmi-0.6.1/include/gemmi/stats.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/symmetry.hpp` & `gemmi-0.6.1/include/gemmi/symmetry.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/fast_float.h` & `gemmi-0.6.1/include/gemmi/third_party/fast_float.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/pocketfft_hdronly.h` & `gemmi-0.6.1/include/gemmi/third_party/pocketfft_hdronly.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/sajson.h` & `gemmi-0.6.1/include/gemmi/third_party/sajson.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/stb_sprintf.h` & `gemmi-0.6.1/include/gemmi/third_party/stb_sprintf.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/LICENSE` & `gemmi-0.6.1/include/gemmi/third_party/tao/LICENSE`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/analyze_cycles.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/analyze_cycles.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/counted.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/counted.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/generic.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/generic.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/grammar_info.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/grammar_info.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/insert_guard.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/insert_guard.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/insert_rules.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/insert_rules.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/rule_info.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/rule_info.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analysis/rule_type.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/rule_type.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/analyze.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analyze.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/argv_input.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/argv_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/ascii.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/ascii.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/buffer_input.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/buffer_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/config.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/config.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/cstream_input.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/cstream_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/eol.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/eol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/file_input.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/file_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/input_error.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/input_error.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/action.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/action.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/action_input.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/action_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/alnum.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/alnum.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/alpha.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/alpha.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/any.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/any.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/apply.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/apply0.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply0.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/apply0_single.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply0_single.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/apply_single.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply_single.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/at.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/at.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/bof.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bof.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/bol.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/bump_help.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bump_help.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/bump_impl.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bump_impl.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/bytes.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bytes.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/control.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/control.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/cr_crlf_eol.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cr_crlf_eol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/cr_eol.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cr_eol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/crlf_eol.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/crlf_eol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/cstream_reader.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cstream_reader.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/cstring_reader.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cstring_reader.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/demangle.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/demangle_cxxabi.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle_cxxabi.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/demangle_nop.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle_nop.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/demangle_sanitise.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle_sanitise.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/disable.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/disable.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/discard.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/discard.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/dusel_mode.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/dusel_mode.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/duseltronik.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/duseltronik.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/enable.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/enable.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/endian.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/endian.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/endian_gcc.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/endian_gcc.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/endian_win.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/endian_win.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/eof.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/eof.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/eol.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/eol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/eolf.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/eolf.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/file_mapper.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/file_mapper.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/file_opener.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/file_opener.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/file_reader.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/file_reader.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/has_apply.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/has_apply.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/has_apply0.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/has_apply0.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/identifier.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/identifier.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/if_apply.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_apply.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/if_must.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_must.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/if_must_else.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_must_else.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/if_then_else.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_then_else.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/input_pair.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/input_pair.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/integer_sequence.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/integer_sequence.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/istream_reader.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/istream_reader.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/istring.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/istring.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/iterator.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/iterator.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/lf_crlf_eol.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/lf_crlf_eol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/lf_eol.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/lf_eol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/list.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/list_must.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list_must.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/list_tail.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list_tail.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/list_tail_pad.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list_tail_pad.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/marker.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/marker.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/minus.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/minus.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/must.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/must.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/not_at.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/not_at.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/one.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/one.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/opt.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/opt.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/pad.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/pad.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/pad_opt.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/pad_opt.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/peek_char.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_char.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/peek_utf16.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_utf16.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/peek_utf32.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_utf32.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/peek_utf8.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_utf8.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/pegtl_string.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/pegtl_string.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/plus.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/plus.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/raise.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/raise.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/range.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/range.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/ranges.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/ranges.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/rep.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/rep_min.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep_min.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/rep_min_max.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep_min_max.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/rep_opt.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep_opt.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/require.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/require.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/result_on_found.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/result_on_found.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/rule_conjunction.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rule_conjunction.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/rules.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rules.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/seq.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/seq.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/skip_control.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/skip_control.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/sor.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/sor.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/star.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/star.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/star_must.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/star_must.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/state.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/state.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/string.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/string.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/trivial.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/trivial.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/try_catch_type.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/try_catch_type.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/internal/until.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/until.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/istream_input.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/istream_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/memory_input.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/memory_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/mmap_input.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/mmap_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/normal.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/normal.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/nothing.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/nothing.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/parse.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/parse.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/parse_error.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/parse_error.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/position.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/position.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/read_input.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/read_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/rules.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/rules.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/string_input.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/string_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/utf16.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/utf16.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/utf32.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/utf32.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/utf8.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/utf8.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl/version.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/version.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tao/pegtl.hpp` & `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/third_party/tinydir.h` & `gemmi-0.6.1/include/gemmi/third_party/tinydir.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/to_chemcomp.hpp` & `gemmi-0.6.1/include/gemmi/to_chemcomp.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/to_cif.hpp` & `gemmi-0.6.1/include/gemmi/to_cif.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/to_json.hpp` & `gemmi-0.6.1/include/gemmi/to_json.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/to_mmcif.hpp` & `gemmi-0.6.1/include/gemmi/to_mmcif.hpp`

 * *Files 25% similar despite different names*

```diff
@@ -38,35 +38,37 @@
   bool cis:1;
   bool scale:1;
   bool atom_type:1;
   bool entity_poly_seq:1;
   bool tls:1;
   bool software:1;
   bool group_pdb:1;  // include _atom_site.group_PDB
+  bool auth_all:1;   // include _atom_site.auth_atom_id and auth_comp_id
 
   explicit MmcifOutputGroups(bool all)
     : atoms(all), block_name(all), entry(all), database_status(all),
       author(all), cell(all), symmetry(all), entity(all),
       entity_poly(false),  // see the comment under "if (groups.entity_poly)"
       struct_ref(all), chem_comp(all), exptl(all), diffrn(all),
       reflns(all), refine(all), title_keywords(all), ncs(all),
       struct_asym(all), origx(all), struct_conf(all), struct_sheet(all),
       struct_biol(all), assembly(all), conn(all), cis(all),
       scale(all), atom_type(all), entity_poly_seq(all), tls(all),
-      software(all), group_pdb(all) {}
+      software(all), group_pdb(all), auth_all(false) {}
 };
 
 GEMMI_DLL void update_mmcif_block(const Structure& st, cif::Block& block,
                                   MmcifOutputGroups groups=MmcifOutputGroups(true));
 GEMMI_DLL cif::Document make_mmcif_document(const Structure& st,
                                             MmcifOutputGroups groups=MmcifOutputGroups(true));
 GEMMI_DLL cif::Block make_mmcif_block(const Structure& st,
                                       MmcifOutputGroups groups=MmcifOutputGroups(true));
 GEMMI_DLL cif::Block make_mmcif_headers(const Structure& st);
 GEMMI_DLL void add_minimal_mmcif_data(const Structure& st, cif::Block& block);
 
 // temporarily we use it in crd.cpp
 GEMMI_DLL void write_struct_conn(const Structure& st, cif::Block& block);
+GEMMI_DLL void write_cispeps(const Structure& st, cif::Block& block);
 
 } // namespace gemmi
 
 #endif
```

### Comparing `gemmi-0.6.0/include/gemmi/to_pdb.hpp` & `gemmi-0.6.1/include/gemmi/to_pdb.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/topo.hpp` & `gemmi-0.6.1/include/gemmi/topo.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -84,18 +84,19 @@
   };
 
   struct Link {
     std::string link_id;
     Residue* res1 = nullptr;
     Residue* res2 = nullptr;
     std::vector<Rule> link_rules;
-    // altloc and asu are used only for ChainInfo::extras, not for ResInfo::prev
     char alt1 = '\0';
     char alt2 = '\0';
-    Asu asu = Asu::Any;
+    Asu asu = Asu::Any;  // used only in Links in ChainInfo::extras
+    bool is_cis = false;  // helper field for CISPEP record generation
+
     // aliasing1/2 points to vector element in ChemComp::aliases.
     // The pointers should stay valid even if a ChemComp is moved.
     const ChemComp::Aliasing* aliasing1 = nullptr;
     const ChemComp::Aliasing* aliasing2 = nullptr;
 
     // only for polymer links, res1 and res2 must be in the same vector (Chain)
     std::ptrdiff_t res_distance() const { return res1 - res2; }
@@ -172,14 +173,15 @@
     for (int i = 0; (size_t) i != t.atoms.size(); ++i)
       if (t.atoms[i] == a)
         return i;
     return -1;
   }
 
   std::ostream* warnings = nullptr;
+  bool only_bonds = false;  // an internal flag for apply_restraints()
   std::vector<ChainInfo> chain_infos;
   std::vector<Link> extras;
 
   // Restraints applied to Model
   std::vector<Bond> bonds;
   std::vector<Angle> angles;
   std::vector<Torsion> torsions;
@@ -233,16 +235,15 @@
   const Chirality* get_chirality(const Atom* ctr) const {
     for (const Chirality& chir : chirs)
       if (chir.atoms[0] == ctr)
         return &chir;
     return nullptr;
   }
 
-  std::pair<double,double>
-  ideal_chiral_abs_volume_sigma(const Chirality &ch) const;
+  double ideal_chiral_abs_volume(const Chirality &ch) const;
 
   std::vector<Rule> apply_restraints(const Restraints& rt,
                                      Residue& res, Residue* res2,
                                      char altloc1, char altloc2, bool require_alt);
   void apply_restraints_from_link(Link& link, const MonLib& monlib);
 
   // Structure is non-const b/c connections may have link_id assigned.
@@ -251,15 +252,18 @@
   // Monlib may get modified by addition of extra links from the model.
   void initialize_refmac_topology(Structure& st, Model& model0,
                                   MonLib& monlib, bool ignore_unknown_links=false);
 
   // This step stores pointers to gemmi::Atom's from model0,
   // so after this step don't add or remove atoms.
   // monlib is needed only for links.
-  void finalize_refmac_topology(const MonLib& monlib);
+  void apply_all_restraints(const MonLib& monlib);
+
+  // prepare bond_index, angle_index, torsion_index, plane_index
+  void create_indices();
 
   Link* find_polymer_link(const AtomAddress& a1, const AtomAddress& a2) {
     for (ChainInfo& ci : chain_infos)
       if (a1.chain_name == ci.chain_ref.name && a2.chain_name == ci.chain_ref.name) {
         for (ResInfo& ri : ci.res_infos)
           for (Link& link : ri.prev) {
             assert(link.res1 && link.res2);
@@ -271,37 +275,38 @@
                  a1.altloc == link.alt2 && a2.altloc == link.alt1))
               return &link;
           }
       }
     return nullptr;
   }
 
+  void set_cispeps_in_structure(Structure& st);
+
   GEMMI_COLD void err(const std::string& msg) const {
     if (warnings == nullptr)
       fail(msg);
     *warnings << "Warning: " << msg << std::endl;
   }
 
 private:
   // storage for link restraints modified by aliases
   std::vector<std::unique_ptr<Restraints>> rt_storage;
   // cache for ChemComps after applying modifications
   std::unordered_map<std::string, std::unique_ptr<ChemComp>> cc_cache;
   // storage for ad-hoc ChemComps (placeholders for those missing in MonLib)
   std::vector<std::unique_ptr<ChemComp>> cc_storage;
 
-  static void add_polymer_links(PolymerType polymer_type,
-                                const ResInfo& ri1, ResInfo& ri2, MonLib* monlib);
   void setup_connection(Connection& conn, Model& model0, MonLib& monlib,
                         bool ignore_unknown_links);
 };
 
 GEMMI_DLL std::unique_ptr<Topo>
 prepare_topology(Structure& st, MonLib& monlib, size_t model_index,
                  HydrogenChange h_change, bool reorder,
-                 std::ostream* warnings=nullptr, bool ignore_unknown_links=false);
+                 std::ostream* warnings=nullptr, bool ignore_unknown_links=false,
+                 bool use_cispeps=false);
 
 
 GEMMI_DLL std::unique_ptr<ChemComp> make_chemcomp_with_restraints(const Residue& res);
 
 } // namespace gemmi
 #endif
```

### Comparing `gemmi-0.6.0/include/gemmi/twin.hpp` & `gemmi-0.6.1/include/gemmi/twin.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/unitcell.hpp` & `gemmi-0.6.1/include/gemmi/unitcell.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/utf.hpp` & `gemmi-0.6.1/include/gemmi/utf.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/util.hpp` & `gemmi-0.6.1/include/gemmi/util.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/include/gemmi/xds_ascii.hpp` & `gemmi-0.6.1/include/gemmi/xds_ascii.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     double zd;
     double rlp;
     double peak;
     double corr;  // is it always integer?
     double maxc;
     int iset = 1;
 
-    // I think ZD can't be negative
-    int frame() const { return int(zd + 1); }
+    // ZD can be negative for a few reflections
+    int frame() const { return (int) std::floor(zd + 1); }
   };
   struct Iset {
     int id;
     std::string input_file;
     double wavelength = 0.;
     double cell_constants[6] = {0., 0., 0., 0., 0., 0.};
     //statistics set by gather_iset_statistics()
@@ -181,14 +181,20 @@
   /// \par p is degree of polarization from range (0,1), as used in XDS.
   void apply_polarization_correction(double p, Vec3 normal);
 
   /// \par overload is maximally allowed pixel value in a peak (MAXC).
   void eliminate_overloads(double overload) {
     vector_remove_if(data, [&](Refl& r) { return r.maxc > overload; });
   }
+
+  /// \par batchmin lowest allowed batch number.
+  void eliminate_batchmin(int batchmin) {
+    double minz = batchmin - 1;
+    vector_remove_if(data, [&](Refl& r) { return r.zd < minz; });
+  }
 };
 
 template<size_t N>
 bool starts_with_ptr(const char* a, const char (&b)[N], const char** endptr) {
   if (std::strncmp(a, b, N-1) != 0)
     return false;
   *endptr = a + N - 1;
```

### Comparing `gemmi-0.6.0/python/align.cpp` & `gemmi-0.6.1/python/align.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/python/ccp4.cpp` & `gemmi-0.6.1/python/ccp4.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/python/chemcomp.cpp` & `gemmi-0.6.1/python/chemcomp.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/python/cif.cpp` & `gemmi-0.6.1/python/cif.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/python/common.h` & `gemmi-0.6.1/python/common.h`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 void add_cif(pybind11::module& cif); // cif.cpp
 void add_cif_read(pybind11::module& cif); // read.cpp
 void add_read_structure(pybind11::module& m); // read.cpp
 void add_small(pybind11::module& m); // read.cpp
 void add_chemcomp(pybind11::module& m); // chemcomp.cpp
 void add_monlib(pybind11::module& m); // monlib.cpp
 void add_topo(pybind11::module& m); // topo.cpp
-void add_refine(pybind11::module& m); // refine.cpp
 void add_alignment(pybind11::module& m); // align.cpp
 void add_scaling(pybind11::module& m); // scaling.cpp
 void add_search(pybind11::module& m); // search.cpp
 void add_sf(pybind11::module& m); // sf.cpp
 void add_custom(pybind11::module& m); // custom.cpp
 
 // defined in write.cpp
```

### Comparing `gemmi-0.6.0/python/elem.cpp` & `gemmi-0.6.1/python/elem.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/python/gemmi.cpp` & `gemmi-0.6.1/python/gemmi.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,13 @@
   add_sf(mg);
   add_cif_read(cif);
   add_mtz(mg);
   add_hkl(mg);
   add_chemcomp(mg);
   add_monlib(mg);
   add_topo(mg);
-  add_refine(mg);
   add_alignment(mg);
   add_search(mg);
   add_read_structure(mg);
   add_scaling(mg);
   add_custom(mg);
 }
```

### Comparing `gemmi-0.6.0/python/grid.cpp` & `gemmi-0.6.1/python/grid.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/python/hkl.cpp` & `gemmi-0.6.1/python/hkl.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/python/meta.cpp` & `gemmi-0.6.1/python/meta.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -176,14 +176,23 @@
     .def_readwrite("reported_distance", &Connection::reported_distance)
     .def("__repr__", [](const Connection& self) {
         return tostr("<gemmi.Connection ", self.name, "  ",
                      self.partner1.str(), " - ", self.partner2.str(), '>');
     });
   py::bind_vector<std::vector<Connection>>(m, "ConnectionList");
 
+  py::class_<CisPep>(m, "CisPep")
+    .def(py::init<>())
+    .def_readwrite("partner_c", &CisPep::partner_c)
+    .def_readwrite("partner_n", &CisPep::partner_n)
+    .def_readwrite("model_str", &CisPep::model_str)
+    .def_readwrite("only_altloc", &CisPep::only_altloc)
+    .def_readwrite("reported_angle", &CisPep::reported_angle)
+    ;
+
   py::class_<Helix> helix(m, "Helix");
   py::enum_<Helix::HelixClass>(helix, "HelixClass")
     .value("UnknownHelix", Helix::HelixClass::UnknownHelix)
     .value("RAlpha", Helix::HelixClass::RAlpha)
     .value("ROmega", Helix::HelixClass::ROmega)
     .value("RPi", Helix::HelixClass::RPi)
     .value("RGamma", Helix::HelixClass::RGamma)
@@ -265,15 +274,14 @@
     ;
   softitem
     .def(py::init<>())
     .def_readwrite("name", &SoftwareItem::name)
     .def_readwrite("version", &SoftwareItem::version)
     .def_readwrite("date", &SoftwareItem::date)
     .def_readwrite("classification", &SoftwareItem::classification)
-    .def_readwrite("pdbx_ordinal", &SoftwareItem::pdbx_ordinal)
     ;
   py::class_<ReflectionsInfo>(m, "ReflectionsInfo")
     .def(py::init<>())
     .def_readwrite("resolution_high", &ReflectionsInfo::resolution_high)
     .def_readwrite("resolution_low", &ReflectionsInfo::resolution_low)
     .def_readwrite("completeness", &ReflectionsInfo::completeness)
     .def_readwrite("redundancy", &ReflectionsInfo::redundancy)
```

### Comparing `gemmi-0.6.0/python/meta.h` & `gemmi-0.6.1/python/meta.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/python/miller_a.h` & `gemmi-0.6.1/python/miller_a.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/python/mol.cpp` & `gemmi-0.6.1/python/mol.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     .def_readwrite("cell", &Structure::cell)
     .def_readwrite("spacegroup_hm", &Structure::spacegroup_hm)
     .def_readwrite("ncs", &Structure::ncs)
     .def_readwrite("resolution", &Structure::resolution)
     .def_readwrite("input_format", &Structure::input_format)
     .def_readwrite("entities", &Structure::entities)
     .def_readwrite("connections", &Structure::connections)
+    .def_readwrite("cispeps", &Structure::cispeps)
     .def_readwrite("helices", &Structure::helices)
     .def_readwrite("sheets", &Structure::sheets)
     .def_readwrite("assemblies", &Structure::assemblies)
     .def_readwrite("meta", &Structure::meta)
     .def_readwrite("has_d_fraction", &Structure::has_d_fraction)
     .def_readwrite("info", &Structure::info)
     .def_readwrite("raw_remarks", &Structure::raw_remarks)
@@ -157,15 +158,14 @@
     .def("add_entity_types", (void (*)(Structure&, bool)) &add_entity_types,
          py::arg("overwrite")=false)
     .def("assign_subchains", &assign_subchains,
          py::arg("force")=false, py::arg("fail_if_unknown")=true)
     .def("ensure_entities", &ensure_entities)
     .def("deduplicate_entities", &deduplicate_entities)
     .def("setup_entities", &setup_entities)
-    .def("assign_cis_flags", assign_cis_flags<Structure>)
     .def("remove_alternative_conformations",
          remove_alternative_conformations<Structure>)
     .def("remove_hydrogens", remove_hydrogens<Structure>)
     .def("remove_waters", remove_waters<Structure>)
     .def("remove_ligands_and_waters", remove_ligands_and_waters<Structure>)
     .def("expand_hd_mixture", &expand_hd_mixture)
     .def("collapse_hd_mixture", &collapse_hd_mixture)
@@ -517,14 +517,16 @@
         py::arg("residue"), py::arg("next_residue"));
   m.def("calculate_sequence_weight", &calculate_sequence_weight,
         py::arg("sequence"), py::arg("unknown")=0.);
   m.def("make_assembly", [](const Assembly& assembly, const Model& model,
                             HowToNameCopiedChain how) {
         return make_assembly(assembly, model, how, nullptr);
   });
+  m.def("merge_atoms_in_expanded_model", &merge_atoms_in_expanded_model,
+        py::arg("model"), py::arg("cell"), py::arg("max_dist")=0.2);
 
   // select.hpp
   py::class_<FilterProxy<Selection, Model>> pySelectionModelsProxy(m, "SelectionModelsProxy");
   py::class_<FilterProxy<Selection, Chain>> pySelectionChainsProxy(m, "SelectionChainsProxy");
   py::class_<FilterProxy<Selection, Residue>> pySelectionResiduesProxy(m, "SelectionResiduesProxy");
   py::class_<FilterProxy<Selection, Atom>> pySelectionAtomsProxy(m, "SelectionAtomsProxy");
```

### Comparing `gemmi-0.6.0/python/monlib.cpp` & `gemmi-0.6.1/python/monlib.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -32,20 +32,20 @@
     .def_readwrite("group", &ChemLink::Side::group)
     .def("__repr__", [](const ChemLink::Side& self) {
         return "<gemmi.ChemLink.Side " + self.comp + "/" +
                ChemComp::group_str(self.group) + ">";
     });
 
   py::class_<ChemMod::AtomMod>(chemmod, "AtomMod")
-    .def_readwrite("func", &ChemMod::AtomMod::func) 
-    .def_readwrite("old_id", &ChemMod::AtomMod::old_id) 
-    .def_readwrite("new_id", &ChemMod::AtomMod::new_id) 
-    .def_readwrite("el", &ChemMod::AtomMod::el) 
-    .def_readwrite("charge", &ChemMod::AtomMod::charge) 
-    .def_readwrite("chem_type", &ChemMod::AtomMod::chem_type) 
+    .def_readwrite("func", &ChemMod::AtomMod::func)
+    .def_readwrite("old_id", &ChemMod::AtomMod::old_id)
+    .def_readwrite("new_id", &ChemMod::AtomMod::new_id)
+    .def_readwrite("el", &ChemMod::AtomMod::el)
+    .def_readwrite("charge", &ChemMod::AtomMod::charge)
+    .def_readwrite("chem_type", &ChemMod::AtomMod::chem_type)
   ;
   chemlink
     .def(py::init<>())
     .def_readwrite("id", &ChemLink::id)
     .def_readwrite("name", &ChemLink::name)
     .def_readwrite("side1", &ChemLink::side1)
     .def_readwrite("side2", &ChemLink::side2)
@@ -118,18 +118,8 @@
   m.def("read_monomer_lib", [](const std::string& monomer_dir,
                                const std::vector<std::string>& resnames,
                                const std::string& libin,
                                bool ignore_missing) {
     return read_monomer_lib(monomer_dir, resnames, gemmi::read_cif_gz, libin, ignore_missing);
   }, py::arg("monomer_dir"), py::arg("resnames"), py::arg("libin")=std::string(),
      py::arg("ignore_missing")=false);
-
-  py::class_<BondIndex>(m, "BondIndex")
-    .def(py::init<const Model&>(), py::keep_alive<1, 2>())
-    .def("add_link", &BondIndex::add_link)
-    .def("add_monomer_bonds", &BondIndex::add_monomer_bonds)
-    .def("are_linked", &BondIndex::are_linked)
-    .def("graph_distance", &BondIndex::graph_distance,
-         py::arg("a"), py::arg("b"), py::arg("same_index"),
-         py::arg("max_distance")=4)
-    ;
 }
```

### Comparing `gemmi-0.6.0/python/mtz.cpp` & `gemmi-0.6.1/python/mtz.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 // Copyright 2019 Global Phasing Ltd.
 
 #include "gemmi/mtz.hpp"
-#include "gemmi/reindex.hpp"  // for reindex_mtz
 #include "gemmi/fourier.hpp"
 #include "gemmi/gz.hpp"
 #include "tostr.hpp"
 
 #include "common.h"
 #include <pybind11/stl.h>
 #include <pybind11/stl_bind.h>
@@ -247,15 +246,15 @@
     .def("sort", &Mtz::sort, py::arg("use_first")=3)
     .def("ensure_asu", &Mtz::ensure_asu, py::arg("tnt_asu")=false)
     .def("switch_to_original_hkl", &Mtz::switch_to_original_hkl)
     .def("switch_to_asu_hkl", &Mtz::switch_to_asu_hkl)
     .def("write_to_file", &Mtz::write_to_file, py::arg("path"))
     .def("reindex", [](Mtz& self, const Op& op) {
         std::ostringstream out;
-        reindex_mtz(self, op, &out);
+        self.reindex(op, &out);
         return out.str();
     }, py::arg("op"))
     .def("__repr__", [](const Mtz& self) {
         return tostr("<gemmi.Mtz with ", self.columns.size(), " columns, ",
                      self.nreflections, " reflections>");
     });
```

### Comparing `gemmi-0.6.0/python/read.cpp` & `gemmi-0.6.1/python/read.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/python/recgrid.cpp` & `gemmi-0.6.1/python/recgrid.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/python/scaling.cpp` & `gemmi-0.6.1/python/scaling.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/python/search.cpp` & `gemmi-0.6.1/python/search.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 // Copyright 2018 Global Phasing Ltd.
 
 #include "gemmi/neighbor.hpp"
 #include "gemmi/linkhunt.hpp"
+#include "gemmi/bond_idx.hpp"
 #include "common.h"
 #include <pybind11/stl.h>
 #include <pybind11/stl_bind.h>
 
 namespace py = pybind11;
 using namespace gemmi;
 
 PYBIND11_MAKE_OPAQUE(std::vector<NeighborSearch::Mark*>)
 
 void add_search(py::module& m) {
   py::class_<NeighborSearch> neighbor_search(m, "NeighborSearch");
   py::class_<NeighborSearch::Mark>(neighbor_search, "Mark")
-    .def_readonly("x", &NeighborSearch::Mark::x)
-    .def_readonly("y", &NeighborSearch::Mark::y)
-    .def_readonly("z", &NeighborSearch::Mark::z)
+    .def_readonly("pos", &NeighborSearch::Mark::pos)
     .def_readonly("altloc", &NeighborSearch::Mark::altloc)
     .def_readonly("element", &NeighborSearch::Mark::element)
     .def_readonly("image_idx", &NeighborSearch::Mark::image_idx)
     .def_readonly("chain_idx", &NeighborSearch::Mark::chain_idx)
     .def_readonly("residue_idx", &NeighborSearch::Mark::residue_idx)
     .def_readonly("atom_idx", &NeighborSearch::Mark::atom_idx)
-    .def("pos", &NeighborSearch::Mark::pos)
     .def("to_cra", (CRA (NeighborSearch::Mark::*)(Model&) const)
                    &NeighborSearch::Mark::to_cra)
     .def("to_site", (SmallStructure::Site& (NeighborSearch::Mark::*)(SmallStructure&) const)
                     &NeighborSearch::Mark::to_site)
     .def("__repr__", [](const NeighborSearch::Mark& self) {
-        return cat("<gemmi.NeighborSearch.Mark ", self.element.name(),
-                   " of atom ", self.chain_idx, '/', self.residue_idx, '/',
-                   self.atom_idx, '>');
+        return cat("<gemmi.NeighborSearch.Mark ", int(self.image_idx), " of atom ",
+                   self.chain_idx, '/', self.residue_idx, '/', self.atom_idx,
+                   " element ", self.element.name(), ">");
     });
   py::bind_vector<std::vector<NeighborSearch::Mark*>>(m, "VectorMarkPtr");
   neighbor_search
     .def_readonly("radius_specified", &NeighborSearch::radius_specified)
     .def(py::init<Model&, const UnitCell&, double>(),
          py::arg("model"), py::arg("cell"), py::arg("max_radius")/*,
          py::keep_alive<1, 2>()*/)
@@ -50,41 +48,41 @@
          "Usually run after constructing NeighborSearch.")
     .def("add_chain", &NeighborSearch::add_chain,
          py::arg("chain"), py::arg("include_h")=true)
     .def("add_atom", &NeighborSearch::add_atom,
          py::arg("atom"), py::arg("n_ch"), py::arg("n_res"), py::arg("n_atom"),
          "Lower-level alternative to populate()")
     .def("find_atoms", &NeighborSearch::find_atoms,
-         py::arg("pos"), py::arg("alt")='\0', py::arg("radius")=0,
+         py::arg("pos"), py::arg("alt")='\0',
+         py::kw_only(), py::arg("min_dist")=0, py::arg("radius")=0,
          py::return_value_policy::move, py::keep_alive<0, 1>())
     .def("find_neighbors", &NeighborSearch::find_neighbors,
          py::arg("atom"), py::arg("min_dist")=0, py::arg("max_dist")=0,
          py::return_value_policy::move, py::keep_alive<0, 1>())
     .def("find_nearest_atom", &NeighborSearch::find_nearest_atom,
+         py::arg("pos"), py::arg("radius")=INFINITY,
          py::return_value_policy::reference_internal)
     .def("find_site_neighbors", &NeighborSearch::find_site_neighbors,
          py::arg("atom"), py::arg("min_dist")=0, py::arg("max_dist")=0,
          py::return_value_policy::move, py::keep_alive<0, 1>())
     .def("dist", &NeighborSearch::dist)
     .def("get_image_transformation", &NeighborSearch::get_image_transformation)
     .def_property_readonly("grid_cell",
         [](const NeighborSearch& self) { return self.grid.unit_cell; })
     .def("__repr__", [](const NeighborSearch& self) {
         return cat("<gemmi.NeighborSearch with grid ",
                    self.grid.nu, ", ", self.grid.nv, ", ", self.grid.nw, '>');
     });
-  m.def("merge_atoms_in_expanded_model", &merge_atoms_in_expanded_model,
-        py::arg("model"), py::arg("cell"), py::arg("max_dist")=0.2);
 
   py::class_<ContactSearch> contactsearch(m, "ContactSearch");
   py::enum_<ContactSearch::Ignore> csignore(contactsearch, "Ignore");
   py::class_<ContactSearch::Result> csresult(contactsearch, "Result");
 
   contactsearch
-    .def(py::init<float>())
+    .def(py::init<double>())
     .def_readwrite("search_radius", &ContactSearch::search_radius)
     .def_readwrite("ignore", &ContactSearch::ignore)
     .def_readwrite("twice", &ContactSearch::twice)
     .def_readwrite("special_pos_cutoff_sq", &ContactSearch::special_pos_cutoff_sq)
     .def_readwrite("min_occupancy", &ContactSearch::min_occupancy)
     .def("setup_atomic_radii", &ContactSearch::setup_atomic_radii)
     .def("get_radius", [](const ContactSearch& self, Element el) {
@@ -128,8 +126,18 @@
     .def_readonly("chem_link_count", &LinkHunt::Match::chem_link_count)
     .def_readonly("cra1", &LinkHunt::Match::cra1)
     .def_readonly("cra2", &LinkHunt::Match::cra2)
     .def_readonly("same_image", &LinkHunt::Match::same_image)
     .def_readonly("bond_length", &LinkHunt::Match::bond_length)
     .def_readonly("conn", &LinkHunt::Match::conn)
     ;
+
+  py::class_<BondIndex>(m, "BondIndex")
+    .def(py::init<const Model&>(), py::keep_alive<1, 2>())
+    .def("add_link", &BondIndex::add_link)
+    .def("add_monomer_bonds", &BondIndex::add_monomer_bonds)
+    .def("are_linked", &BondIndex::are_linked)
+    .def("graph_distance", &BondIndex::graph_distance,
+         py::arg("a"), py::arg("b"), py::arg("same_index"),
+         py::arg("max_distance")=4)
+    ;
 }
```

### Comparing `gemmi-0.6.0/python/sf.cpp` & `gemmi-0.6.1/python/sf.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/python/sym.cpp` & `gemmi-0.6.1/python/sym.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,18 @@
         ReciprocalAsu asu(&sg);
         for (py::ssize_t i = 0; i < h.shape(0); ++i) {
           Op::Miller hkl = asu.to_asu({{h(i, 0), h(i, 1), h(i, 2)}}, gops).first;
           for (int j = 0; j != 3; ++j)
             h(i, j) = hkl[j];
         }
     }, py::arg("miller_array").noconvert())
+    // In Python SpaceGroup class can't be created, we only use references to
+    // elements in spacegroup_tables::main.
+    .def("__eq__", [](const SpaceGroup& a, const SpaceGroup& b) { return &a == &b; },
+         py::is_operator())
     .def("__repr__", [](const SpaceGroup &self) {
         return "<gemmi.SpaceGroup(\"" + self.xhm() + "\")>";
     })
     .def(py::pickle(
         [](const SpaceGroup &self) {
           return self.xhm();
         },
```

### Comparing `gemmi-0.6.0/python/topo.cpp` & `gemmi-0.6.1/python/topo.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -135,40 +135,42 @@
     .def_readonly("bonds", &Topo::bonds)
     .def_readonly("angles", &Topo::angles)
     .def_readonly("torsions", &Topo::torsions)
     .def_readonly("chirs", &Topo::chirs)
     .def_readonly("planes", &Topo::planes)
     .def_readonly("extras", &Topo::extras)
     .def_readonly("chain_infos", &Topo::chain_infos)
-    .def("ideal_chiral_abs_volume_sigma", &Topo::ideal_chiral_abs_volume_sigma)
+    .def("ideal_chiral_abs_volume", &Topo::ideal_chiral_abs_volume)
     .def("links_to_previous", [](Topo& self, Residue* res) {
         if (Topo::ResInfo* ri = self.find_resinfo(res))
           return ri->prev;
         fail("links_to_previous(): Residue not found");
     }, py::return_value_policy::reference_internal)
     .def("first_bond_in_link", &Topo::first_bond_in_link,
          py::return_value_policy::reference_internal)
+    .def("set_cispeps_in_structure", &Topo::set_cispeps_in_structure)
     ;
 
   m.def("prepare_topology",
     [](Structure& st, MonLib& monlib, size_t model_index,
        HydrogenChange h_change, bool reorder,
-       const py::object& pywarnings, bool ignore_unknown_links) {
+       const py::object& pywarnings, bool ignore_unknown_links, bool use_cispeps) {
       std::ostream* warnings = nullptr;
       std::ostream os(nullptr);
       std::unique_ptr<py::detail::pythonbuf> buffer;
       if (!pywarnings.is_none()) {
         buffer.reset(new py::detail::pythonbuf(pywarnings));
         os.rdbuf(buffer.get());
         warnings = &os;
       }
       return prepare_topology(st, monlib, model_index, h_change, reorder,
-                              warnings, ignore_unknown_links);
+                              warnings, ignore_unknown_links, use_cispeps);
     }, py::arg("st"), py::arg("monlib"), py::arg("model_index")=0,
        py::arg("h_change")=HydrogenChange::NoChange, py::arg("reorder")=false,
-       py::arg("warnings")=py::none(), py::arg("ignore_unknown_links")=false);
+       py::arg("warnings")=py::none(), py::arg("ignore_unknown_links")=false,
+       py::arg("use_cispeps")=false);
 
   // crd.hpp
   m.def("setup_for_crd", &setup_for_crd);
   m.def("prepare_refmac_crd", &prepare_refmac_crd);
   m.def("add_automatic_links", &add_automatic_links);
 }
```

### Comparing `gemmi-0.6.0/python/tostr.hpp` & `gemmi-0.6.1/python/tostr.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/python/unitcell.cpp` & `gemmi-0.6.1/python/unitcell.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 namespace py = pybind11;
 using namespace gemmi;
 
 static std::string triple(double x, double y, double z) {
   using namespace std;  // VS2015/17 doesn't like std::snprintf
   char buf[128];
-  snprintf(buf, 128, "%g, %g, %g", x, y, z);
+  auto r = [](double d) { return std::fabs(d) >= 1e-15 ? d : 0; };
+  snprintf(buf, 128, "%g, %g, %g", r(x), r(y), r(z));
   return std::string(buf);
 }
 
 static void mat33_from_list(Mat33& self, std::array<std::array<double,3>,3>& m) {
   for (int i = 0; i < 3; ++i)
     for (int j = 0; j < 3; ++j)
       self.a[i][j] = m[i][j];
```

### Comparing `gemmi-0.6.0/python/write.cpp` & `gemmi-0.6.1/python/write.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     DEF_BIT_PROPERTY(cis)
     DEF_BIT_PROPERTY(scale)
     DEF_BIT_PROPERTY(atom_type)
     DEF_BIT_PROPERTY(entity_poly_seq)
     DEF_BIT_PROPERTY(tls)
     DEF_BIT_PROPERTY(software)
     DEF_BIT_PROPERTY(group_pdb)
+    DEF_BIT_PROPERTY(auth_all)
     ;
 
   structure
     .def("make_pdb_headers", &make_pdb_headers)
     .def("write_pdb", [](const Structure& st, const std::string& path,
                          bool seqres_records, bool ssbond_records,
                          bool link_records, bool cispep_records,
```

### Comparing `gemmi-0.6.0/setup.py` & `gemmi-0.6.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 USE_SYSTEM_ZLIB = False
 MIN_PYBIND_VER = '2.6.2'
 
 def read_version_from_header():
     with open('include/gemmi/version.hpp') as f:
         for line in f:
             if line.startswith('#define GEMMI_VERSION '):
-                return line.split()[2].strip('"dev')
+                return line.split()[2].strip('"')
 
 __version__ = read_version_from_header()
 
 class get_pybind_include(object):
     """Helper class to determine the pybind11 include path
     The purpose of this class is to postpone importing pybind11
     until it is actually installed, so that the ``get_include()``
@@ -47,20 +47,20 @@
 
 ext_modules = [
     Extension('gemmi',
               ['python/%s.cpp' % name for name in
                   ['gemmi', 'align', 'ccp4', 'chemcomp', 'cif', 'custom',
                    'elem', 'hkl', 'grid', 'meta', 'mol', 'monlib', 'mtz',
                    'read', 'recgrid', 'scaling', 'search', 'sf', 'sym',
-                   'refine', 'topo', 'unitcell', 'write']]
+                   'topo', 'unitcell', 'write']]
               + ['src/%s.cpp' % name for name in
                   ['sprintf', 'mtz', 'to_pdb', 'to_mmcif', 'mtz2cif',
-                   'read_cif', 'mmcif', 'mmread_gz',
+                   'read_cif', 'mmcif', 'mmread_gz', 'calculate', 'eig3',
                    'resinfo', 'polyheur', 'monlib', 'topo', 'riding_h', 'crd',
-                   'xds_ascii']],
+                   'xds_ascii', 'assembly']],
               include_dirs=zlib_include_dirs + [
                   'include',
                   'third_party',
                   # Path to pybind11 headers
                   get_pybind_include(),
               ],
               libraries=[zlib_library],
@@ -164,33 +164,32 @@
         for ext in self.extensions:
             ext.define_macros = [('VERSION_INFO',
                                   '"%s"' % self.distribution.get_version())]
             ext.extra_compile_args = opts
             ext.extra_link_args = link_opts
         build_ext.build_extensions(self)
 
+def long_description():
+    readme_path = os.path.join(os.path.dirname(__file__), "README.md")
+    with open(readme_path) as f:
+        lines = f.readlines()
+    # replace badges from README with this info:
+    lines[:2] = ['Note: command-line program gemmi is in PyPI\n',
+                 '[gemmi-program](https://pypi.org/project/gemmi-program/).\n']
+    return ''.join(lines)
+
 setup(
     name='gemmi',
     version=__version__,
     author='Marcin Wojdyr',
     author_email='wojdyr@gmail.com',
     url='https://project-gemmi.github.io/',
     description='library for structural biology',
-    long_description='''\
-    Library for macromolecular crystallography and structural bioinformatics.
-    For working with coordinate files (mmCIF, PDB, mmJSON),
-    refinement restraints (monomer library), electron density maps (CCP4),
-    and crystallographic reflection data (MTZ, SF-mmCIF). It understands
-    crystallographic symmetries, it knows how to switch between the real
-    and reciprocal space and it can do a few other things.
-
-    The setup.py script builds only Python extension.
-    Use cmake to build also a command-line program.
-    ''',
-    long_description_content_type='text/plain',
+    long_description=long_description(),
+    long_description_content_type='text/markdown',
     libraries=build_libs,
     ext_modules=ext_modules,
     packages=['gemmi-examples'],
     package_dir={'gemmi-examples': 'examples'},
     install_requires=[],
     setup_requires=['pybind11>=' + MIN_PYBIND_VER],
     cmdclass={'build_ext': BuildExt},
```

### Comparing `gemmi-0.6.0/src/crd.cpp` & `gemmi-0.6.1/src/crd.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
   };
   NeighborSearch ns(model, st.cell, 5.0);
   ns.populate();
   ContactSearch contacts(3.1f);  // 3.1 > 130% of ZN-CYS bond (2.34)
   contacts.ignore = ContactSearch::Ignore::AdjacentResidues;
   int counter = 0;
   contacts.for_each_contact(ns, [&](const CRA& cra1, const CRA& cra2,
-                                    int image_idx, float dist_sq) {
+                                    int image_idx, double dist_sq) {
     if (st.find_connection_by_cra(cra1, cra2))
       return;
     auto m = monlib.match_link(*cra1.residue, cra1.atom->name, cra1.atom->altloc,
                                *cra2.residue, cra2.atom->name, cra2.atom->altloc,
                                sq(1 / 1.4) * dist_sq);
     const ChemLink* link = std::get<0>(m);
     bool invert = std::get<1>(m);
@@ -221,14 +221,21 @@
     auto it = block.items.end() - 2;
     assert(it->type == cif::ItemType::Loop && it->has_prefix("_struct_conn."));
     for (std::string& tag : it->loop.tags)
       if (ends_with(tag, "_auth_asym_id"))
         tag += "-disabled";
   }
 
+  if (!st.cispeps.empty()) {
+    items.emplace_back(cif::CommentArg{"#########################\n"
+                                       "## STRUCT_MON_PROT_CIS ##\n"
+                                       "#########################"});
+    write_cispeps(st, block);
+  }
+
   items.emplace_back(cif::CommentArg{"###############\n"
                                      "## ATOM_SITE ##\n"
                                      "###############"});
   cif::Loop& atom_loop = block.init_mmcif_loop("_atom_site.", {
       "group_PDB",
       "id",
       "label_atom_id",
@@ -387,15 +394,15 @@
                       t.restr->value, t.restr->esd, NAN, NAN,
                       deg(t.calculate()));
   } else if (rule.rkind == Topo::RKind::Chirality) {
     const Topo::Chirality& t = topo.chirs[rule.index];
     add_restraint_row(restr_loop, "CHIR", ++counters[3],
                       chirality_to_string(t.restr->sign), ".",
                       {t.atoms[0], t.atoms[1], t.atoms[2], t.atoms[3]},
-                      topo.ideal_chiral_abs_volume_sigma(t).first, 0.2, NAN, NAN,
+                      topo.ideal_chiral_abs_volume(t), 0.2, NAN, NAN,
                       t.calculate());
   } else if (rule.rkind == Topo::RKind::Plane) {
     const Topo::Plane& t = topo.planes[rule.index];
     ++counters[4];
     auto coeff = find_best_plane(t.atoms);
     for (const Atom* atom : t.atoms)
       add_restraint_row(restr_loop, "PLAN", counters[4], t.restr->label, ".",
```

### Comparing `gemmi-0.6.0/src/mmcif.cpp` & `gemmi-0.6.1/src/mmcif.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -224,14 +224,58 @@
       if (row.has2(kLabelAltId+i))
         a.altloc = cif::as_char(row[kLabelAltId+i], '\0');
     }
     st.connections.emplace_back(c);
   }
 }
 
+// CISPEP equivalent
+void read_prot_cis(cif::Block& block, Structure& st) {
+  enum {
+    kModelNum=0,
+    kAuthAsymId=1, kAuthSeqId=2, kInsCode=3, kLabelCompId=4, kAuthCompId=5,
+    kAuthAsymId2=6, kAuthSeqId2=7, kInsCode2=8, kLabelCompId2=9, kAuthCompId2=10,
+    kAltId=11, kOmegaAngle=12
+  };
+  // We could use label_seq_id etc and call set_part_of_address_from_label(),
+  // but for now let's assume that auth_seq_id etc are there.
+  for (auto row : block.find("_struct_mon_prot_cis.",
+                             {"pdbx_PDB_model_num",                  // 0
+                              "auth_asym_id",                        // 1
+                              "auth_seq_id", "?pdbx_PDB_ins_code",   // 2-3
+                              "?label_comp_id", "?auth_comp_id",     // 4-5
+                              "?pdbx_auth_asym_id_2",                // 6
+                              "?pdbx_auth_seq_id_2", "?pdbx_PDB_ins_code_2",   // 7-8
+                              "?pdbx_label_comp_id_2", "?pdbx_auth_comp_id_2", // 9-10
+                              "?label_alt_id", "?pdbx_omega_angle"})) {        // 11-12
+    CisPep cispep;
+    cispep.model_str = row.str(kModelNum);
+    cispep.partner_c.chain_name = row.str(kAuthAsymId);
+    cispep.partner_c.res_id.seqid = make_seqid(row.str(kAuthSeqId), row.ptr_at(kInsCode));
+    cispep.partner_c.res_id.name = row.str(row.has2(kLabelCompId2) ? 4 : 5);
+    if (row.has(kLabelCompId))
+      cispep.partner_c.res_id.name = row.str(kLabelCompId);
+    else if (row.has(kAuthCompId))
+      cispep.partner_c.res_id.name = row.str(kAuthCompId);
+    if (row.has(kAuthAsymId2))
+      cispep.partner_n.chain_name = row.str(kAuthAsymId2);
+    if (row.has(kAuthSeqId2))
+      cispep.partner_n.res_id.seqid = make_seqid(row.str(kAuthSeqId2), row.ptr_at(kInsCode2));
+    if (row.has(kLabelCompId2))
+      cispep.partner_n.res_id.name = row.str(kLabelCompId2);
+    else if (row.has(kAuthCompId2))
+      cispep.partner_n.res_id.name = row.str(kAuthCompId2);
+    if (row.has(kAltId))
+      cispep.only_altloc = cif::as_char(row[kAltId], '\0');
+    if (row.has(kOmegaAngle))
+      cispep.reported_angle = cif::as_number(row[kOmegaAngle]);
+    st.cispeps.push_back(cispep);
+  }
+}
+
 // Operation expression is an item type used for *.oper_expression.
 // Here, to keep it simple, we ignore products such as "(2)(3)".
 // We parse "3", "1,3,5", "one,two", "(3)", "(a)", "(1-60)", "(2,3-8,XY)", etc
 std::vector<std::string> parse_operation_expr(const std::string& expr) {
   std::vector<std::string> result;
   std::size_t start = 0;
   std::size_t close_br = std::string::npos;
@@ -565,24 +609,22 @@
     copy_double(row, 7, exper.reflections.r_sym);
     copy_double(row, 8, exper.reflections.mean_I_over_sigma);
   }
 
   for (auto row : block.find("_software.", {"name",
                                             "?classification",
                                             "?version",
-                                            "?date",
-                                            "?pdbx_ordinal"})) {
+                                            "?date"})) {
     st.meta.software.emplace_back();
     SoftwareItem& item = st.meta.software.back();
     item.name = row.str(0);
     if (row.has2(1))
       item.classification = software_classification_from_string(row.str(1));
     copy_string(row, 2, item.version);
     copy_string(row, 3, item.date);
-    copy_int(row, 4, item.pdbx_ordinal);
   }
 
   std::vector<std::string> ncs_oper_tags = transform_tags("matrix", "vector");
   ncs_oper_tags.emplace_back("id");  // 12
   ncs_oper_tags.emplace_back("?code");  // 13
   cif::Table ncs_oper = block.find("_struct_ncs_oper.", ncs_oper_tags);
   for (auto op : ncs_oper) {
@@ -826,32 +868,19 @@
       }
   }
 
   fill_residue_entity_type(st);
 
   st.setup_cell_images();
 
-  // CISPEP
-  for (auto row : block.find("_struct_mon_prot_cis.",
-                             {"pdbx_PDB_model_num", "auth_asym_id",  // 0-1
-                              "auth_seq_id", "?pdbx_PDB_ins_code",   // 2-3
-                              "?label_comp_id", "?auth_comp_id"})) { // 4-5
-    if (row.has2(0) && row.has2(1) && row.has2(2) &&
-        (row.has2(4) || row.has2(5)))
-      if (Model* mdl = st.find_model(row[0])) {
-        std::string comp = row.str(row.has2(4) ? 4 : 5);
-        ResidueId rid = make_resid(comp, row.str(2), row.ptr_at(3));
-        if (Residue* res = mdl->find_residue(row[1], rid))
-          res->is_cis = true;
-      }
-  }
 
   st.helices = read_helices(block);
   st.sheets = read_sheets(block);
   read_connectivity(block, st);
+  read_prot_cis(block, st);
   st.assemblies = read_assemblies(block);
   read_sifts_unp(block, st);
 
   return st;
 }
 
 } // namespace gemmi
```

### Comparing `gemmi-0.6.0/src/mmread_gz.cpp` & `gemmi-0.6.1/src/mmread_gz.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/src/monlib.cpp` & `gemmi-0.6.1/src/monlib.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
                                "atom_id_2", "atom_id_3", "atom_id_4",
                                "new_value_angle", "new_value_angle_esd",
                                "?new_period"}))
     rt.torsions.push_back({row.has(1) ? row.str(1) : "",
                            {chem_mod_type(row[0]), row.str(2)},
                            {1, row.str(3)}, {1, row.str(4)}, {1, row.str(5)},
                            cif::as_number(row[6]), cif::as_number(row[7]),
-                           row.has(8) ? cif::as_int(row[8]) : -1});
+                           row.has(8) ? cif::as_int(row[8], 0) : -1});
   for (auto row : block.find("_chem_mod_chir.",
                              {"function", "atom_id_centre", "atom_id_1",
                               "atom_id_2", "atom_id_3",
                               "new_volume_sign"}))
     rt.chirs.push_back({{1, row.str(1)}, {chem_mod_type(row[0]), row.str(2)},
                         {1, row.str(3)}, {1, row.str(4)},
                         chirality_from_string(row[5])});
```

### Comparing `gemmi-0.6.0/src/mtz2cif.cpp` & `gemmi-0.6.1/src/mtz2cif.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 // Copyright 2020-2022 Global Phasing Ltd.
 
 #include <gemmi/mtz2cif.hpp>
 
 #include <climits>       // for INT_MIN
-#include <set>
 #include <algorithm>     // for all_of
+#include <set>
+#include <unordered_map>
 
 #include <gemmi/asudata.hpp>   // for calculate_hkl_value_correlation
 #include <gemmi/eig3.hpp>      // for eigen_decomposition
 #include <gemmi/sprintf.hpp>   // for gstb_snprintf, to_str
 #include <gemmi/atox.hpp>      // for read_word
 #include <gemmi/version.hpp>   // for GEMMI_VERSION
```

### Comparing `gemmi-0.6.0/src/polyheur.cpp` & `gemmi-0.6.1/src/polyheur.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         // buffer molecules w/o hydrogens are mostly ions
         if (info.kind == ResidueInfo::BUF && info.hydrogen_count == 0)
           continue;
         if (info.is_peptide_linking())
           ++aa;
         if (info.is_na_linking())
           ++na;
+        counts[info.kind]++;
       } else if (r.get_ca()) {
         ++aa;
       } else if (r.get_p()) {
         ++na;
       }
       ++total;
     }
@@ -61,14 +62,18 @@
 
 static std::vector<Residue>::iterator infer_polymer_end(Chain& chain, PolymerType ptype) {
   auto b = chain.residues.begin();
   auto e = chain.residues.end();
   for (auto it = b; it != e; ++it) {
     ResidueInfo info = find_tabulated_residue(it->name);
     if (info.found()) {
+      if (info.is_water()) {
+        e = it;
+        break;
+      }
       bool maybe_linking = (is_polypeptide(ptype) && info.is_peptide_linking())
                         || (is_polynucleotide(ptype) && info.is_na_linking());
       // The first residue could be non-polymer.
       if (!maybe_linking && b != chain.residues.begin()) {
         e = it;
         break;
       }
@@ -85,15 +90,24 @@
     return e;
   // Ligands are often separated by a significant gap in the sequence ID numeration.
   // But such gap can also mean that part of the chain is not modelled.
   auto last = std::min(e, chain.residues.end() - 1);
   for (auto it = b; it < last; ++it) {
     int gap = *(it+1)->seqid.num - *it->seqid.num;
     // The gap should be non-negative, but you can find exceptions in the PDB.
-    if (gap < -1 || gap > 10 || !are_connected2(*it, *(it+1), ptype))
+    if (gap < -1 || gap > 10)
+      return it+1;
+    // Usually polymers are longer than 1-2 residues, although there are
+    // exceptions (example: 1-residue polymers in 5N22), so we can't be sure.
+    // OTOH a protein can be capped with monomers different from amino-acid
+    // and are_connected2() may return false negative. So if there is no gap
+    // in numbering, it seems better to assume the polymer didn't end yet.
+    if (gap == 1 && it - chain.residues.begin() < 2)
+      continue;
+    if (!are_connected2(*it, *(it+1), ptype))
       return it+1;
   }
   return e;
 }
 
 void add_entity_types(Chain& chain, bool overwrite) {
   if (!overwrite &&
```

### Comparing `gemmi-0.6.0/src/read_cif.cpp` & `gemmi-0.6.1/src/read_cif.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/src/resinfo.cpp` & `gemmi-0.6.1/src/resinfo.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
       case ID("CIR"): return { RI::AA,  1, 'r',  13, 175.186f };
       case ID("BMT"): return { RI::AA,  1, 't',  19, 201.263f };
       case ID("DIL"): return { RI::AAD, 1, 'i',  13, 131.173f };
       case ID("FGA"): return { RI::AA,  1, 'e',   9, 147.129f };
       case ID("PHI"): return { RI::AA,  1, 'f',  10, 291.086f };
       case ID("CRQ"): return { RI::AA,  1, 'q',  16, 344.322f };
       case ID("SME"): return { RI::AA,  1, 'm',  11, 165.211f };
-      case ID("GHP"): return { RI::AAD, 1, 'g',   9, 167.162f };
+      case ID("GHP"): return { RI::AA,  1, 'g',   9, 167.162f };  // d-peptide in CCD
       case ID("MHO"): return { RI::AA,  1, 'm',  11, 165.211f };
       case ID("NEP"): return { RI::AA,  1, 'h',  10, 235.134f };
       case ID("TRQ"): return { RI::AA,  1, 'w',  10, 234.208f };
       case ID("TOX"): return { RI::AA,  1, 'w',  12, 236.224f };
       case ID("ALC"): return { RI::AA,  1, 'a',  17, 171.237f };
       case ID("3FG"): return { RI::AA,  1, ' ',   9, 183.161f };
       case ID("SCH"): return { RI::AA,  1, 'c',   9, 167.250f };
@@ -131,15 +131,15 @@
       case ID("MEA"): return { RI::AA,  1, 'f',  13, 179.216f };
       case ID("MED"): return { RI::AAD, 1, 'm',  11, 149.211f };
       case ID("OAS"): return { RI::AA,  1, 's',   9, 147.129f };
       case ID("GL3"): return { RI::AA,  1, 'g',   5, 91.1322f };
       case ID("FVA"): return { RI::AA,  1, 'v',  11, 145.156f };
       case ID("PHL"): return { RI::AA,  1, 'f',  13, 151.206f };
       case ID("CRF"): return { RI::AA,  1, 't',  18, 342.349f };
-      case ID("OMZ"): return { RI::AAD, 1, ' ',  10, 231.633f };
+      case ID("OMZ"): return { RI::AA,  1, ' ',  10, 231.633f };  // d-peptide in CCD
       case ID("BFD"): return { RI::AA,  1, 'd',   6, 198.102f };
       case ID("MEQ"): return { RI::AA,  1, 'q',  12, 160.171f };
       case ID("DAB"): return { RI::AA,  1, 'a',  10, 118.134f };
       case ID("AGM"): return { RI::AA,  1, 'r',  17, 189.235f };
 
       case ID("PSU"): return { RI::RNA, 2, 'u',  13, 324.181f };
       case ID("5MU"): return { RI::RNA, 2, 'u',  15, 338.208f };
@@ -359,14 +359,15 @@
       switch (name[1]) {
         case 'A': return { RI::DNA, 2, 'A',  14, 331.222f };
         case 'C': return { RI::DNA, 2, 'C',  14, 307.197f };
         case 'G': return { RI::DNA, 2, 'G',  14, 347.221f };
         case 'I': return { RI::DNA, 2, 'I',  13, 332.207f };
         case 'T': return { RI::DNA, 2, 'T',  15, 322.208f };
         case 'U': return { RI::DNA, 2, 'U',  13, 308.182f };
+        case 'N': return { RI::DNA, 2, 'N',  14, 198.111f };  // unknown DNA
       }
     else
 #define ID(s) (s[0] << 8 | s[1])
       switch (ID(name.c_str())) {
         case ID("AG"): return { RI::BUF, 0, ' ',   0, 107.868f };
         case ID("AL"): return { RI::BUF, 0, ' ',   0, 26.9815f };
         case ID("BA"): return { RI::BUF, 0, ' ',   0, 137.327f };
```

### Comparing `gemmi-0.6.0/src/riding_h.cpp` & `gemmi-0.6.1/src/riding_h.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,100 +1,63 @@
 // Copyright 2018-2022 Global Phasing Ltd.
 
 #include <gemmi/riding_h.hpp>
-#include <gemmi/calculate.hpp> // for calculate_angle
 
 namespace gemmi {
 
-// Assumes no hydrogens in the residue.
-// Position and serial number are not assigned for new atoms.
-void add_hydrogens_without_positions(Topo::ResInfo& ri) {
-  Residue& res = *ri.res;
-  // Add H atom for each conformation (altloc) of the parent atom.
-  for (size_t i = 0, size = res.atoms.size(); i != size; ++i) {
-    const ChemComp& cc = ri.get_final_chemcomp(res.atoms[i].altloc);
-    for (const Restraints::Bond& bond : cc.rt.bonds) {
-      // res.atoms may get re-allocated, so we can't set parent earlier
-      const Atom& parent = res.atoms[i];
-      assert(!parent.is_hydrogen());
-      const Restraints::AtomId* atom_id;
-      if (bond.id1 == parent.name)
-        atom_id = &bond.id2;
-      else if (bond.id2 == parent.name)
-        atom_id = &bond.id1;
-      else
-        continue;
-      auto it = cc.find_atom(atom_id->atom);
-      if (it == cc.atoms.end())
-        fail("inconsistent _chem_comp " + cc.name);
-      if (it->is_hydrogen()) {
-        gemmi::Atom atom;
-        atom.name = it->id;
-        atom.altloc = parent.altloc;
-        atom.element = it->el;
-        // calc_flag will be changed to Calculated when the position is set
-        atom.calc_flag = CalcFlag::Dummy;
-        atom.occ = parent.occ;
-        atom.b_iso = parent.b_iso;
-        res.atoms.push_back(atom);
-      }
-    }
-  }
-}
-
+namespace {
 
 // Calculate position using one angle (theta) and one dihedral angle (tau).
 // Returns position of x4 in x1-x2-x3-x4, where dist=|x3-x4| and
 // theta is angle(x2, x3, x4).
 // Based on section 3.3 of Paciorek et al, Acta Cryst. A52, 349 (1996).
-static Position position_from_angle_and_torsion(const Position& x1,
-                                                const Position& x2,
-                                                const Position& x3,
-                                                double dist,  // |x3-x4|
-                                                double theta, // angle x2-x3-x4
-                                                double tau) { // dihedral angle
+Position position_from_angle_and_torsion(const Position& x1,
+                                         const Position& x2,
+                                         const Position& x3,
+                                         double dist,  // |x3-x4|
+                                         double theta, // angle x2-x3-x4
+                                         double tau) { // dihedral angle
   Vec3 u = x2 - x1;
   Vec3 v = x3 - x2;
   Vec3 e1 = v.normalized();
   Vec3 e2 = -(u - u.dot(e1) * e1).normalized();
   Vec3 e3 = e1.cross(e2);
   Vec3 e23 = std::cos(tau) * e2 + std::sin(tau) * e3;
   return x3 + Position(dist * (-std::cos(theta) * e1 + std::sin(theta) * e23));
 }
 
 // Similar to position_from_angle_and_torsion(), but x1 and tau are not given.
-static Position arbitrary_position_from_angle(const Position& x2,
-                                              const Position& x3,
-                                              double dist,     // |x3-x4|
-                                              double theta) {  // angle x2-x3-x4
+Position arbitrary_position_from_angle(const Position& x2,
+                                       const Position& x3,
+                                       double dist,     // |x3-x4|
+                                       double theta) {  // angle x2-x3-x4
   Vec3 u(1, 0, 0);
   Vec3 v = x3 - x2;
   Vec3 e1 = v.normalized();
   Vec3 e2_ = -(u - u.dot(e1) * e1);
   if (e2_.length_sq() < 1e-6) {
     // u || v, let's take any non-parallel u
     u = Vec3(0, 1, 0);
     e2_ = -(u - u.dot(e1) * e1);
   }
   Vec3 e2 = e2_.normalized();
   return x3 + Position(dist * (-std::cos(theta) * e1 + std::sin(theta) * e2));
 }
 
 
-static Vec3 get_vector_to_line(const Position& point,
-                               const Position& point_on_the_line,
-                               const Vec3& unit_vector) {
+Vec3 get_vector_to_line(const Position& point,
+                        const Position& point_on_the_line,
+                        const Vec3& unit_vector) {
   // en.wikipedia.org/wiki/Distance_from_a_point_to_a_line#Vector_formulation
   // the component of a - p perpendicular to the line is: (a-p) - ((a-p).n)n
   Vec3 ap = point_on_the_line - point;
   return ap - ap.dot(unit_vector) * unit_vector;
 }
 
 // If no points satisfy the distances returns a pair of NaNs
-static
 std::pair<Position, Position> trilaterate(const Position& p1, double r1sq,
                                           const Position& p2, double r2sq,
                                           const Position& p3, double r3sq) {
   // It was based on https://en.wikipedia.org/wiki/Trilateration
   // but apparently that page has changed in the meantime.
   Vec3 ex = (p2 - p1).normalized();
   double i = ex.dot(p3-p1);
@@ -108,15 +71,15 @@
   double z = std::sqrt(z2);  // may result in NaN
   return std::make_pair(p1 + Position(x*ex + y*ey + z*ez),
                         p1 + Position(x*ex + y*ey - z*ez));
 }
 
 // Calculate position using two angles.
 // Returns p4. Topology: p1 is bonded to p2, p3 and p4.
-static std::pair<Position, Position>
+std::pair<Position, Position>
 position_from_two_angles(const Position& p1,
                          const Position& p2,
                          const Position& p3,
                          double dist14,     // |p4-p1|
                          double theta214,   // angle p2-p1-p4
                          double theta314) { // angle p3-p1-p4
   double d12sq = p1.dist_sq(p2);
@@ -126,88 +89,57 @@
   double d24sq = d14sq + d12sq - 2 * std::sqrt(d14sq * d12sq) * cos(theta214);
   double d34sq = d14sq + d13sq - 2 * std::sqrt(d14sq * d13sq) * cos(theta314);
   return trilaterate(p1, d14sq, p2, d24sq, p3, d34sq);
 }
 
 // Returns angle between hydrogen and the plane of heavy atoms
 // in 2H tetrahedral configuration. theta0 is the angle between heavy atoms.
-static double calculate_tetrahedral_delta(double theta0, double theta1, double theta2) {
+double calculate_tetrahedral_delta(double theta0, double theta1, double theta2) {
   // simplified trilateration:
   //   auto r = trilaterate(Position(0, 0, 0), 1,
   //                        Position(1, 0, 0), 2 - 2 * std::cos(theta1),
   //                        Position(std::cos(theta0), std::sin(theta0), 0),
   //                        2 - 2 * std::cos(theta2));
   //   return std::asin(std::fabs(r.first.z));
   double x = std::cos(theta1);
   double y = (std::cos(theta2) - x * std::cos(theta0)) / std::sin(theta0);
   double z2 = 1 - x*x - y*y;
   double z = std::sqrt(z2);  // may result in NaN
   return std::asin(z);
 }
 
-static void place_hydrogens(const Topo& topo, const Atom& atom) {
+struct BondedAtom {
+  Atom* ptr;
+  Position& pos; // == ptr->pos;
+  double dist;
+};
+
+// known and hs are lists of heavy atoms and hydrogens bonded to atom.
+// hs is const, but nevertheless atoms it points to are modified.
+void place_hydrogens(const Topo& topo, const Atom& atom,
+                     const std::vector<BondedAtom>& known,
+                     const std::vector<BondedAtom>& hs) {
   using Angle = Restraints::Angle;
-  struct BondedAtom {
-    Atom* ptr;
-    Position& pos; // == ptr->pos;
-    double dist;
-  };
-
-  // put atoms bonded to atom into two lists
-  std::vector<BondedAtom> known; // heavy atoms with known positions
-  std::vector<BondedAtom> hs;    // H atoms (unknown)
-  known.reserve(3);
-  hs.reserve(4);
-
-  auto range = topo.bond_index.equal_range(&atom);
-  char limit_altoc = '\0';
-  for (auto i = range.first; i != range.second; ++i) {
-    const Topo::Bond* t = i->second;
-    Atom* other = t->atoms[t->atoms[0] == &atom ? 1 : 0];
-    if (other->altloc) {
-      if (atom.altloc) {
-        // We support links between different altlocs in Topo (e.g. link A-B),
-        // although these are rare, special cases.
-        // But if we had bonds between atom 1 (A/B) and atom 2 (A/B/C),
-        // and we had bonds B-B and B-C, we'd want to use only one of them (B-B).
-        // Checking atom's name is not robust, but should suffice here.
-        if (atom.altloc != other->altloc &&
-            in_vector_f([&](const BondedAtom& a) { return a.ptr->name == other->name; },
-                           known))
-          continue;
-      } else {  // atom.altoc == '\0', other->altloc != 0
-        // We can't rely on atom names: in microheterogeneities different
-        // conformations can have different atom names.
-        if (limit_altoc && other->altloc != limit_altoc)
-          continue;
-        limit_altoc = other->altloc;
-      }
-    }
-    auto& atom_list = other->is_hydrogen() ? hs : known;
-    atom_list.push_back({other, other->pos, t->restr->value});
-  }
-
-  if (hs.size() == 0)
-    return;
+  assert(!hs.empty());
 
   auto giveup = [&](const std::string& message) {
-    for (BondedAtom& bonded_h : hs) {
+    for (const BondedAtom& bonded_h : hs) {
       bonded_h.ptr->occ = 0;
       bonded_h.ptr->calc_flag = CalcFlag::Dummy;
     }
     fail(message);
   };
 
-  for (BondedAtom& bonded_h : hs)
+  for (const BondedAtom& bonded_h : hs)
     bonded_h.ptr->calc_flag = CalcFlag::Calculated;
 
   // ==== only hydrogens ====
   if (known.size() == 0) {
     // we can only arbitrarily pick directions of atoms
-    for (BondedAtom& bonded_h : hs)
+    for (const BondedAtom& bonded_h : hs)
       bonded_h.ptr->occ = 0;
     hs[0].pos = atom.pos + Position(hs[0].dist, 0, 0);
     if (hs.size() > 1) {
       double theta = pi();
       if (const Angle* ang = topo.take_angle(hs[1].ptr, &atom, hs[0].ptr))
         theta = ang->radians();
       hs[1].pos = atom.pos + Position(hs[1].dist * cos(theta),
@@ -322,15 +254,15 @@
       Vec3 v3 = rotate_about_axis(v1, axis, rad(-120));
       hs[(idx+1) % 3].pos = atom.pos + Position(v2);
       hs[(idx+2) % 3].pos = atom.pos + Position(v3);
     } else if (hs.size() >= 4) {
       giveup("Unusual: atom bonded to one heavy atoms and 4+ hydrogens.");
     }
     if (!tau_end || period > (int)hs.size())
-      for (BondedAtom& bonded_h : hs)
+      for (const BondedAtom& bonded_h : hs)
         bonded_h.ptr->occ = 0;
   // ==== two heavy atoms and hydrogens ====
   } else if (known.size() == 2) {
     if (hs.size() >= 3)
       giveup("Unusual: atom bonded to 2+ heavy atoms and 3+ hydrogens.");
     const Angle* ang1 = topo.take_angle(hs[0].ptr, &atom, known[0].ptr);
     const Angle* ang2 = topo.take_angle(hs[0].ptr, &atom, known[1].ptr);
@@ -429,28 +361,75 @@
     Vec3 h_dir = abc.x * u10 + abc.y * u20 + abc.z * u30;
     if (std::isnan(h_dir.x))
       giveup("bonded atoms are exactly overlapping.");
     hs[0].pos = atom.pos + Position(h_dir.changed_magnitude(hs[0].dist));
   }
 }
 
+} // anonymous namespace
+
 void place_hydrogens_on_all_atoms(Topo& topo) {
+  std::vector<BondedAtom> known;
+  std::vector<BondedAtom> hs;
+  auto filter = [](char alt, const std::vector<BondedAtom>& v) {
+    std::vector<BondedAtom> out;
+    out.reserve(v.size());
+    for (const BondedAtom& ba : v)
+      if (ba.ptr->altloc_matches(alt))
+        out.push_back(ba);
+    return out;
+  };
   for (Topo::ChainInfo& chain_info : topo.chain_infos)
     for (Topo::ResInfo& ri : chain_info.res_infos) {
       // If we don't have monomer description from a cif file,
       // only ad-hoc restraints, don't try to place hydrogens.
       if (ri.orig_chemcomp == nullptr)
         continue;
-      for (Atom& atom : ri.res->atoms)
-        if (!atom.is_hydrogen()) {
-          try {
-            place_hydrogens(topo, atom);
-          } catch (const std::runtime_error& e) {
-            topo.err("Placing of hydrogen bonded to "
-                     + atom_str(chain_info.chain_ref, *ri.res, atom)
-                     + " failed:\n  " + e.what());
+      for (Atom& atom : ri.res->atoms) {
+        if (atom.is_hydrogen())
+          continue;
+        try {
+          // gather bonded atoms
+          known.clear();
+          hs.clear();
+          auto range = topo.bond_index.equal_range(&atom);
+          for (auto i = range.first; i != range.second; ++i) {
+            const Topo::Bond* t = i->second;
+            Atom* other = t->atoms[t->atoms[0] == &atom ? 1 : 0];
+            if (other->altloc && atom.altloc) {
+              // We support links between different altlocs in Topo (e.g. link A-B),
+              // although these are rare, special cases.
+              // But if we had bonds between atom 1 (A/B) and atom 2 (A/B/C),
+              // and we had bonds B-B and B-C, we'd want to use only one of them (B-B).
+              // Checking atom's name is not robust, but should suffice here.
+              if (atom.altloc != other->altloc &&
+                  in_vector_f([&](const BondedAtom& a) { return a.ptr->name == other->name; },
+                              known))
+                continue;
+            }
+            auto& atom_list = other->is_hydrogen() ? hs : known;
+            atom_list.push_back({other, other->pos, t->restr->value});
           }
+          if (hs.size() == 0)
+            continue;
+          if (atom.altloc == '\0') {
+            std::string altlocs;  // cf. add_distinct_altlocs
+            for (const auto& h : hs)
+              if (h.ptr->altloc && altlocs.find(h.ptr->altloc) == std::string::npos)
+                altlocs += h.ptr->altloc;
+            if (altlocs.size() > 1) {
+              for (char alt : altlocs)
+                place_hydrogens(topo, atom, filter(alt, known), filter(alt, hs));
+              continue;
+            }
+          }
+          place_hydrogens(topo, atom, known, hs);
+        } catch (const std::runtime_error& e) {
+          topo.err("Placing of hydrogen bonded to "
+                   + atom_str(chain_info.chain_ref, *ri.res, atom)
+                   + " failed:\n  " + e.what());
         }
+      }
     }
 }
 
 }
```

### Comparing `gemmi-0.6.0/src/to_mmcif.cpp` & `gemmi-0.6.1/src/to_mmcif.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,16 @@
 // only if the chain name is missing, which was OK in the past.
 // Here we use '' rather than . or ?.
 inline std::string qchain(const std::string& s) {
   return cif::quote(s);
 }
 
 
-void add_cif_atoms(const Structure& st, cif::Block& block, bool use_group_pdb) {
+void add_cif_atoms(const Structure& st, cif::Block& block,
+                   bool use_group_pdb, bool auth_all) {
   // atom list
   cif::Loop& atom_loop = block.init_mmcif_loop("_atom_site.", {
       "id",
       "type_symbol",
       "label_atom_id",
       "label_alt_id",
       "label_comp_id",
@@ -71,17 +72,21 @@
       "pdbx_PDB_ins_code",
       "Cartn_x",
       "Cartn_y",
       "Cartn_z",
       "occupancy",
       "B_iso_or_equiv",
       "pdbx_formal_charge",
+      "auth_atom_id",  // optional (tags[15] is removed if !auth_all)
+      "auth_comp_id",  // optional (tags[16] is removed if !auth_all)
       "auth_seq_id",
       "auth_asym_id",
       "pdbx_PDB_model_num"});
+  if (!auth_all)
+    atom_loop.tags.erase(atom_loop.tags.begin() + 15, atom_loop.tags.begin() + 17);
   if (use_group_pdb)
     atom_loop.tags.emplace(atom_loop.tags.begin(), "_atom_site.group_PDB");
   bool has_calc_flag = false;
   bool has_tls_group_id = false;
   size_t atom_site_count = 0;
   for (const Model& model : st.models)
     for (const Chain& chain : model.chains)
@@ -128,14 +133,19 @@
           vv.emplace_back(pdbx_icode(res));
           vv.emplace_back(to_str(atom.pos.x));
           vv.emplace_back(to_str(atom.pos.y));
           vv.emplace_back(to_str(atom.pos.z));
           vv.emplace_back(to_str(atom.occ));
           vv.emplace_back(to_str(atom.b_iso));
           vv.emplace_back(atom.charge == 0 ? "?" : std::to_string(atom.charge));
+          if (auth_all) {
+            size_t atom_name_idx = vv.size() - 13;
+            vv.emplace_back(vv[atom_name_idx]);  // auth_atom_id = label_atom_id
+            vv.emplace_back(vv[atom_name_idx + 2]);  // auth_comp_id = label_comp_id
+          }
           vv.emplace_back(auth_seq_id);
           vv.emplace_back(qchain(chain.name));
           vv.emplace_back(string_or_qmark(model.name));
           if (has_calc_flag)
             vv.emplace_back(&".\0d\0c\0dum"[2 * (int) atom.calc_flag]);
           if (has_tls_group_id)
             vv.emplace_back(int_or_qmark(atom.tls_group_id));
@@ -378,14 +388,54 @@
 
   cif::Loop& type_loop = block.init_mmcif_loop("_struct_conn_type.", {"id"});
   for (int i = 0; i < (int)type_ids.size() - 1; ++i)
     if (type_ids[i])
       type_loop.add_row({connection_type_to_string((Connection::Type)i)});
 }
 
+void write_cispeps(const Structure& st, cif::Block& block) {
+  cif::Loop& prot_cis_loop = block.init_mmcif_loop("_struct_mon_prot_cis.",
+      {"pdbx_id", "pdbx_PDB_model_num",
+       "label_asym_id", "label_seq_id", "label_comp_id",
+       "auth_asym_id", "auth_seq_id", "pdbx_PDB_ins_code",
+       "pdbx_label_asym_id_2", "pdbx_label_seq_id_2", "pdbx_label_comp_id_2",
+       "pdbx_auth_asym_id_2", "pdbx_auth_seq_id_2", "pdbx_PDB_ins_code_2",
+       "label_alt_id", "pdbx_omega_angle"});
+  auto& v = prot_cis_loop.values;
+  int pdbx_id = 0;
+  for (const CisPep& cispep : st.cispeps) {
+    const Model* model = &st.models[0];
+    if (st.models.size() > 1) {
+      model = st.find_model(cispep.model_str);
+      if (!model)
+        continue;
+    }
+    const_CRA cra1 = model->find_cra(cispep.partner_c, true);
+    const_CRA cra2 = model->find_cra(cispep.partner_n, true);
+    if (!cra1.residue || !cra2.residue)
+      continue;
+    v.emplace_back(std::to_string(++pdbx_id));            // pdbx_id
+    v.emplace_back(cispep.model_str);                     // pdbx_PDB_model_num
+    v.emplace_back(subchain_or_dot(*cra1.residue));       // label_asym_id
+    v.emplace_back(cra1.residue->label_seq.str('.'));     // label_seq_id
+    v.emplace_back(cra1.residue->name);                   // label_comp_id
+    v.emplace_back(qchain(cispep.partner_c.chain_name));  // auth_asym_id
+    v.emplace_back(cispep.partner_c.res_id.seqid.num.str()); // auth_seq_id
+    v.emplace_back(pdbx_icode(cispep.partner_c.res_id));  // pdbx_PDB_ins_code
+    v.emplace_back(subchain_or_dot(*cra2.residue));       // pdbx_label_asym_id_2
+    v.emplace_back(cra2.residue->label_seq.str('.'));     // pdbx_label_seq_id_2
+    v.emplace_back(cra2.residue->name);                   // pdbx_label_comp_id_2
+    v.emplace_back(qchain(cispep.partner_n.chain_name));  // pdbx_auth_asym_id_2
+    v.emplace_back(cispep.partner_n.res_id.seqid.num.str()); // pdbx_auth_seq_id_2
+    v.emplace_back(pdbx_icode(cispep.partner_n.res_id));  // pdbx_PDB_ins_code_2
+    v.emplace_back(1, cispep.only_altloc ? cispep.only_altloc : '.');
+    v.emplace_back(number_or_qmark(cispep.reported_angle));
+  }
+}
+
 void update_mmcif_block(const Structure& st, cif::Block& block, MmcifOutputGroups groups) {
   if (st.models.empty())
     return;
 
   if (groups.block_name)
     block.name = is_valid_block_name(st.name) ? st.name : "model";
 
@@ -961,29 +1011,16 @@
   }
   if (groups.assembly && !st.assemblies.empty())
     write_assemblies(st, block);
 
   if (groups.conn)
     write_struct_conn(st, block);
 
-  if (groups.cis) {  // _struct_mon_prot_cis
-    cif::Loop& prot_cis_loop = block.init_mmcif_loop("_struct_mon_prot_cis.",
-        {"pdbx_id", "pdbx_PDB_model_num", "label_asym_id", "label_seq_id",
-         "auth_asym_id", "auth_seq_id", "pdbx_PDB_ins_code",
-         "label_comp_id", "label_alt_id"});
-    for (const Model& model : st.models)
-      for (const Chain& chain : model.chains)
-        for (const Residue& res : chain.residues)
-          if (res.is_cis)
-            prot_cis_loop.add_row({std::to_string(prot_cis_loop.length()+1),
-                                   model.name, subchain_or_dot(res),
-                                   res.label_seq.str('.'), qchain(chain.name),
-                                   res.seqid.num.str(), pdbx_icode(res),
-                                   res.name, "."});
-  }
+  if (groups.cis)  // _struct_mon_prot_cis
+    write_cispeps(st, block);
 
   // _atom_sites (SCALE)
   if (groups.scale && (st.has_origx || st.cell.explicit_matrices)) {
     cif::ItemSpan span(block.items, "_atom_sites.");
     span.set_pair("_atom_sites.entry_id", id);
     std::string prefix = "_atom_sites.fract_transf_";
     for (int i = 0; i < 3; ++i) {
@@ -1029,15 +1066,15 @@
             start = end + 1;
           }
           poly_loop.add_row({qchain(ent.name), num, mon_ids.substr(start)});
         }
   }
 
   if (groups.atoms)
-    add_cif_atoms(st, block, groups.group_pdb);
+    add_cif_atoms(st, block, groups.group_pdb, groups.auth_all);
 
   if (groups.tls && st.meta.has_tls()) {
     cif::Loop& loop = block.init_mmcif_loop("_pdbx_refine_tls.", {
         "pdbx_refine_id", "id",
         "T[1][1]", "T[2][2]", "T[3][3]", "T[1][2]", "T[1][3]", "T[2][3]",
         "L[1][1]", "L[2][2]", "L[3][3]", "L[1][2]", "L[1][3]", "L[2][3]",
         "S[1][1]", "S[1][2]", "S[1][3]",
@@ -1075,17 +1112,18 @@
                               sel.res_end.num ? sel.res_end.str() : "?",
                               string_or_qmark(sel.details)});
   }
 
   if (groups.software && !st.meta.software.empty()) {
     cif::Loop& loop = block.init_mmcif_loop("_software.",
                  {"pdbx_ordinal", "classification", "name", "version", "date"});
+    int ordinal = 0;
     for (const SoftwareItem& item : st.meta.software)
       loop.add_row({
-          std::to_string(item.pdbx_ordinal),
+          std::to_string(++ordinal),
           cif::quote(software_classification_to_string(item.classification)),
           cif::quote(item.name),
           string_or_dot(item.version),
           string_or_qmark(item.date)});
   }
 }
 
@@ -1109,11 +1147,11 @@
 }
 
 void add_minimal_mmcif_data(const Structure& st, cif::Block& block) {
   cif::ItemSpan cell_span(block.items, "_cell.");
   write_cell_parameters(st.cell, cell_span);
   block.set_pair("_symmetry.space_group_name_H-M", cif::quote(st.spacegroup_hm));
   write_ncs_oper(st, block);
-  add_cif_atoms(st, block, /*use_group_pdb=*/false);
+  add_cif_atoms(st, block, /*use_group_pdb=*/false, /*auth_all=*/false);
 }
 
 } // namespace gemmi
```

### Comparing `gemmi-0.6.0/src/to_pdb.cpp` & `gemmi-0.6.1/src/to_pdb.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 #include <cstring>        // for memset, memcpy
 #include <algorithm>
 #include <array>
 #include <sstream>       // for ostringstream
 
 #include <gemmi/fail.hpp>       // for fail
 #include <gemmi/sprintf.hpp>
-#include <gemmi/calculate.hpp>  // for calculate_omega
-#include <gemmi/polyheur.hpp>   // for are_connected
 #include <gemmi/resinfo.hpp>
 #include <gemmi/util.hpp>
 
 namespace gemmi {
 
 #define WRITE(...) do { \
     gstb_snprintf(buf, 82, __VA_ARGS__); \
@@ -544,15 +542,15 @@
              cra2.residue->name.c_str(), cra2.chain->name.c_str(),
              write_seq_id(cra2.residue->seqid).data(),
              "1555", im.symmetry_code(false).c_str(), im.dist());
         }
     }
 
     // LINK  (note: uses only the first model and primary conformation)
-    if (!st.models.empty() && opt.link_records) {
+    if (opt.link_records) {
       for (const Connection& con : st.connections)
         if (con.type == Connection::Covale || con.type == Connection::MetalC ||
             con.type == Connection::Unknown) {
           const_CRA cra1 = st.models[0].find_cra(con.partner1, true);
           const_CRA cra2 = st.models[0].find_cra(con.partner2, true);
           // In special cases (LINKR gap) atoms are not there.
           if (!cra1.residue || !cra2.residue)
@@ -590,43 +588,38 @@
               std::memset(buf+58, ' ', 14); // erase symmetry
             // overwrite distance with link_id
             gstb_snprintf(buf+72, 82-72, "%-8s\n", con.link_id.c_str());
           }
           buf[80] = '\n';
           os.write(buf, 81);
         }
-
     }
 
-    // CISPEP (note: uses only the first conformation)
-    if (!st.models.empty() && opt.cispep_records) {
+    // CISPEP
+    if (opt.cispep_records) {
       int counter = 0;
-      for (const Model& model : st.models)
-        for (const Chain& chain : model.chains)
-          for (const Residue& res : chain.residues)
-            if (res.is_cis) {
-              const Residue* next = chain.next_residue(res);
-              if (next && are_connected(res, *next, PolymerType::PeptideL)) {
-                if (++counter == 10000)
-                  counter = 0;
-                WRITE("CISPEP%4d %3s%2s %5s   %3s%2s %5s %9s %12.2f %20s",
-                      counter,
-                      res.name.c_str(), chain.name.c_str(),
-                      write_seq_id(res.seqid).data(),
-                      next->name.c_str(), chain.name.c_str(),
-                      write_seq_id(next->seqid).data(),
-                      st.models.size() > 1 ? model.name.c_str() : "0",
-                      deg(calculate_omega(res, *next)),
-                      "");
-              }
-            }
+      for (const CisPep& cispep : st.cispeps) {
+        WRITE("CISPEP%4d %3s%2s %5s   %3s%2s %5s %9s %12.2f %20s",
+              ++counter,
+              cispep.partner_c.res_id.name.c_str(),
+              cispep.partner_c.chain_name.c_str(),
+              write_seq_id(cispep.partner_c.res_id.seqid).data(),
+              cispep.partner_n.res_id.name.c_str(),
+              cispep.partner_n.chain_name.c_str(),
+              write_seq_id(cispep.partner_n.res_id.seqid).data(),
+              st.models.size() > 1 ? cispep.model_str.c_str() : "0",
+              std::isnan(cispep.reported_angle) ? 0. : cispep.reported_angle,
+              "");
+        if (counter == 9999)
+          counter = 0;
+      }
     }
   }
 
-  if(opt.cryst1_record)
+  if (opt.cryst1_record)
     write_cryst1(st, os);
   if (st.has_origx && !st.origx.is_identity()) {
     for (int i = 0; i < 3; ++i)
       WRITE("ORIGX%d %13.6f%10.6f%10.6f %14.5f %24s", i+1,
             st.origx.mat[i][0], st.origx.mat[i][1], st.origx.mat[i][2],
             st.origx.vec.at(i), "");
   }
```

### Comparing `gemmi-0.6.0/src/topo.cpp` & `gemmi-0.6.1/src/topo.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 // Copyright 2018-2022 Global Phasing Ltd.
 
 #include <gemmi/topo.hpp>
 #include <cmath>               // for sqrt, round
+#include <map>                 // for multimap
+#include <unordered_map>       // for unordered_multimap
 #include <gemmi/polyheur.hpp>  // for get_or_check_polymer_type, ...
 #include <gemmi/riding_h.hpp>  // for place_hydrogens_on_all_atoms, ...
 #include <gemmi/modify.hpp>    // for remove_hydrogens
 
 namespace gemmi {
 
 std::unique_ptr<ChemComp> make_chemcomp_with_restraints(const Residue& res) {
@@ -150,68 +152,81 @@
   for (int n = 0; monlib.get_link(cl.id) != nullptr; ++n)
     cl.id.replace(orig_len, cl.id.size(), std::to_string(n));
 
   auto it = monlib.links.emplace(cl.id, cl);
   return it.first->first;
 }
 
-void Topo::add_polymer_links(PolymerType polymer_type,
-                             const Topo::ResInfo& ri1,
-                             Topo::ResInfo& ri2,
-                             MonLib* monlib) {
-  Link link;
+static void add_polymer_links(PolymerType polymer_type,
+                              const Topo::ResInfo& ri1,
+                              Topo::ResInfo& ri2,
+                              MonLib* monlib) {
+  Topo::Link link;
   link.res1 = ri1.res;
   link.res2 = ri2.res;
   assert(&ri1 - &ri2 == link.res_distance());
   bool groups_ok = (ri1.orig_chemcomp != nullptr && ri2.orig_chemcomp != nullptr);
 
   if (is_polypeptide(polymer_type)) {
     std::string c = "C";
+    std::string ca1 = "CA";
     std::string n = "N";
+    std::string ca2 = "CA";
     if (ri1.orig_chemcomp && !ChemComp::is_peptide_group(ri1.orig_chemcomp->group)) {
       for (const ChemComp::Aliasing& aliasing : ri1.orig_chemcomp->aliases)
         if (ChemComp::is_peptide_group(aliasing.group)) {
           link.aliasing1 = &aliasing;
-          if (const std::string* c_ptr = aliasing.name_from_alias(c))
-            c = *c_ptr;
+          if (const std::string* ptr = aliasing.name_from_alias(c))
+            c = *ptr;
+          if (const std::string* ptr = aliasing.name_from_alias(ca1))
+            ca1 = *ptr;
           break;
         }
       if (!link.aliasing1)
         groups_ok = false;
     }
     ChemComp::Group n_terminus_group = ri2.orig_chemcomp ? ri2.orig_chemcomp->group
                                                          : ChemComp::Group::Null;
     if (ri2.orig_chemcomp && !ChemComp::is_peptide_group(ri2.orig_chemcomp->group)) {
       for (const ChemComp::Aliasing& aliasing : ri2.orig_chemcomp->aliases)
         if (ChemComp::is_peptide_group(aliasing.group)) {
           link.aliasing2 = &aliasing;
           n_terminus_group = aliasing.group;
-          if (const std::string* n_ptr = aliasing.name_from_alias(n))
-            n = *n_ptr;
+          if (const std::string* ptr = aliasing.name_from_alias(n))
+            n = *ptr;
+          if (const std::string* ptr = aliasing.name_from_alias(ca2))
+            ca2 = *ptr;
           break;
         }
       if (!link.aliasing2)
         groups_ok = false;
     }
     for (const Atom& a1 : ri1.res->atoms)
       if (a1.name == c && a1.element == El::C) {
         for (const Atom& a2 : ri2.res->atoms)
           if (a2.name == n && a2.element == El::N &&
               (a2.altloc == a1.altloc || a2.altloc == '\0' || a1.altloc == '\0') &&
               in_peptide_bond_distance(&a1, &a2)) {
+            // One C-N pair of atoms can create here only one link.
+            // Ignoring artificial configuration of no-altloc C and N atoms,
+            // and CA atoms in 2+ conformations making both CIS and TRANS links.
             link.alt1 = a1.altloc;
             link.alt2 = a2.altloc;
             if (groups_ok) {
-              bool is_cis = ri1.res->is_cis;
+              // Deciding CIS/TRANS based on omega angle.
+              char alt = a1.altloc_or(a2.altloc_or('*'));
+              const Atom* ca1_atom = ri1.res->find_atom(ca1, alt, El::C);
+              const Atom* ca2_atom = ri2.res->find_atom(ca2, alt, El::C);
+              link.is_cis = is_peptide_bond_cis(ca1_atom, &a1, &a2, ca2_atom);
               if (n_terminus_group == ChemComp::Group::PPeptide)
-                link.link_id = is_cis ? "PCIS" : "PTRANS";
+                link.link_id = link.is_cis ? "PCIS" : "PTRANS";
               else if (n_terminus_group == ChemComp::Group::MPeptide)
-                link.link_id = is_cis ? "NMCIS" : "NMTRANS";
+                link.link_id = link.is_cis ? "NMCIS" : "NMTRANS";
               else
-                link.link_id = is_cis ? "CIS" : "TRANS";
+                link.link_id = link.is_cis ? "CIS" : "TRANS";
             } else if (monlib) {
               link.link_id = add_auto_chemlink(*monlib,
                                                ri1.res->name, c,
                                                ri2.res->name, n,
                                                1.34, 0.04);
             }
             ri2.prev.push_back(link);
@@ -265,30 +280,25 @@
 
   if (ri2.prev.empty()) {
     link.link_id = "gap";
     ri2.prev.push_back(link);
   }
 }
 
-std::pair<double,double>
-Topo::ideal_chiral_abs_volume_sigma(const Chirality &ch) const {
+double Topo::ideal_chiral_abs_volume(const Chirality &ch) const {
   const Restraints::Bond* bond_c1 = take_bond(ch.atoms[0], ch.atoms[1]);
   const Restraints::Bond* bond_c2 = take_bond(ch.atoms[0], ch.atoms[2]);
   const Restraints::Bond* bond_c3 = take_bond(ch.atoms[0], ch.atoms[3]);
   const Restraints::Angle* angle_1c2 = take_angle(ch.atoms[1], ch.atoms[0], ch.atoms[2]);
   const Restraints::Angle* angle_2c3 = take_angle(ch.atoms[2], ch.atoms[0], ch.atoms[3]);
   const Restraints::Angle* angle_3c1 = take_angle(ch.atoms[3], ch.atoms[0], ch.atoms[1]);
   if (bond_c1 && bond_c2 && bond_c3 && angle_1c2 && angle_2c3 && angle_3c1)
-    return std::make_pair(chiral_abs_volume(bond_c1->value, bond_c2->value, bond_c3->value,
-                                            angle_1c2->value, angle_2c3->value, angle_3c1->value),
-                          chiral_abs_volume_sigma(bond_c1->value, bond_c2->value, bond_c3->value,
-                                            angle_1c2->value, angle_2c3->value, angle_3c1->value,
-                                            bond_c1->esd, bond_c2->esd, bond_c3->esd,
-                                            angle_1c2->esd, angle_2c3->esd, angle_3c1->esd));
-  return std::make_pair(std::numeric_limits<double>::quiet_NaN(), 0);
+    return chiral_abs_volume(bond_c1->value, bond_c2->value, bond_c3->value,
+                             angle_1c2->value, angle_2c3->value, angle_3c1->value);
+  return std::numeric_limits<double>::quiet_NaN();
 }
 
 std::vector<Topo::Rule> Topo::apply_restraints(const Restraints& rt,
                                                Residue& res, Residue* res2,
                                                char altloc1, char altloc2,
                                                bool require_alt) {
   std::string altlocs;
@@ -309,14 +319,18 @@
           if (with_alt || !require_alt) {
             rules.push_back({RKind::Bond, bonds.size()});
             bonds.push_back({&bond, {{at1, at2}}});
           }
           if (!with_alt)
             break;
         }
+
+  if (only_bonds)
+    return rules;
+
   for (const Restraints::Angle& angle : rt.angles)
     for (char alt : altlocs)
       if (Atom* at1 = angle.id1.get_from(res, res2, alt, altloc2))
         if (Atom* at2 = angle.id2.get_from(res, res2, alt, altloc2))
           if (Atom* at3 = angle.id3.get_from(res, res2, alt, altloc2)) {
             bool with_alt = at1->altloc || at2->altloc || at3->altloc;
             if (with_alt || !require_alt) {
@@ -393,16 +407,15 @@
         rt_copy->rename_atom(Restraints::AtomId{1, p.second}, p.first);
     if (link.aliasing2)
       for (const auto& p : link.aliasing2->related)
         rt_copy->rename_atom(Restraints::AtomId{2, p.second}, p.first);
     rt = rt_copy.get();
     rt_storage.push_back(std::move(rt_copy));
   }
-  auto rules = apply_restraints(*rt, *link.res1, link.res2, link.alt1, link.alt2, false);
-  vector_move_extend(link.link_rules, std::move(rules));
+  link.link_rules = apply_restraints(*rt, *link.res1, link.res2, link.alt1, link.alt2, false);
 }
 
 // see comments above the declaration
 void Topo::initialize_refmac_topology(Structure& st, Model& model0,
                                       MonLib& monlib, bool ignore_unknown_links) {
   // initialize chains and residues
   for (Chain& chain : model0.chains)
@@ -433,15 +446,15 @@
       auto prev_end = ci.group_end(prev_begin);
       while (prev_end != ci.res_infos.end()) {
         auto group_begin = prev_end;
         auto group_end = ci.group_end(group_begin);
         for (auto ri = group_begin; ri != group_end; ++ri)
           for (auto prev_ri = prev_begin; prev_ri != prev_end; ++prev_ri) {
             MonLib* monlib_ptr = ignore_unknown_links ? nullptr : &monlib;
-            Topo::add_polymer_links(ci.polymer_type, *prev_ri, *ri, monlib_ptr);
+            add_polymer_links(ci.polymer_type, *prev_ri, *ri, monlib_ptr);
           }
         prev_begin = group_begin;
         prev_end = group_end;
       }
     }
   }
 
@@ -522,34 +535,35 @@
         // no cache - ad-hoc restraints are separate for each residue
         cc_storage.emplace_back(make_chemcomp_with_restraints(*ri.res));
         ri.chemcomps.push_back({'\0', cc_storage.back().get()});
       }
     }
 }
 
-void Topo::finalize_refmac_topology(const MonLib& monlib) {
-  // apply restraints
+void Topo::apply_all_restraints(const MonLib& monlib) {
   for (ChainInfo& chain_info : chain_infos)
     for (ResInfo& ri : chain_info.res_infos) {
       // link restraints
       for (Link& link : ri.prev)
         apply_restraints_from_link(link, monlib);
       // monomer restraints
-      bool require_alt = false;
-      for (const auto& it : ri.chemcomps) {
-        auto rules = apply_restraints(it.cc->rt, *ri.res, nullptr,
-                                      it.altloc, '\0', require_alt);
+      auto it = ri.chemcomps.cbegin();
+      ri.monomer_rules = apply_restraints(it->cc->rt, *ri.res, nullptr,
+                                          it->altloc, '\0', /*require_alt=*/false);
+      while (++it != ri.chemcomps.end()) {
+        auto rules = apply_restraints(it->cc->rt, *ri.res, nullptr,
+                                      it->altloc, '\0', /*require_alt=*/true);
         vector_move_extend(ri.monomer_rules, std::move(rules));
-        require_alt = true;
       }
     }
   for (Link& link : extras)
     apply_restraints_from_link(link, monlib);
+}
 
-  // create indices
+void Topo::create_indices() {
   for (Bond& bond : bonds) {
     bond_index.emplace(bond.atoms[0], &bond);
     if (bond.atoms[1] != bond.atoms[0])
       bond_index.emplace(bond.atoms[1], &bond);
   }
   for (Angle& ang : angles)
     angle_index.emplace(ang.atoms[1], &ang);
@@ -646,60 +660,215 @@
                                       extra.res1->name, conn.partner1.atom_name,
                                       extra.res2->name, conn.partner2.atom_name,
                                       ideal_dist, 0.02);
   }
   extras.push_back(extra);
 }
 
-static void remove_hydrogens_from_atom(Topo::ResInfo* ri,
+void Topo::set_cispeps_in_structure(Structure& st) {
+  st.cispeps.clear();
+  if (chain_infos.empty())
+    return;
+  // model is not stored in Topo, let's determine it from chain_infos[0]
+  std::string model_str;
+  for (const Model& model : st.models)
+    if (!model.chains.empty() &&
+        &model.chains[0] == &chain_infos[0].chain_ref)
+      model_str = model.name;
+  for (ChainInfo& chain_info : chain_infos)
+    for (ResInfo& res_info : chain_info.res_infos)
+      for (Link& link : res_info.prev)
+        if (link.is_cis) {
+          CisPep cp;
+          cp.model_str = model_str;
+          cp.partner_c = AtomAddress(chain_info.chain_ref.name, *link.res1, "", link.alt1);
+          cp.partner_n = AtomAddress(chain_info.chain_ref.name, *link.res2, "", link.alt2);
+          cp.only_altloc = link.alt1 ? link.alt1 : link.alt2;
+          for (const Rule& rule : link.link_rules)
+            if (rule.rkind == RKind::Torsion) {
+              const Torsion& tor = torsions[rule.index];
+              if (tor.restr->label == "omega") {
+                cp.reported_angle = tor.calculate();
+                break;
+              }
+            }
+          st.cispeps.push_back(cp);
+        }
+}
+
+namespace {
+
+void remove_hydrogens_from_atom(Topo::ResInfo* ri,
                                        const std::string& atom_name, char alt) {
   if (!ri)
     return;
   std::vector<Atom>& atoms = ri->res->atoms;
   const Restraints& rt = ri->get_final_chemcomp(alt).rt;
   for (auto it = atoms.end(); it-- != atoms.begin(); ) {
     if (it->is_hydrogen() && is_same_conformer(it->altloc, alt)) {
       const Restraints::AtomId* heavy = rt.first_bonded_atom(it->name);
       if (heavy && heavy->atom == atom_name)
         atoms.erase(it);
     }
   }
 }
 
+void set_cis_in_link(Topo::Link& link, bool is_cis) {
+  if (is_cis) {
+    if (ends_with(link.link_id, "TRANS"))
+      link.link_id.replace(link.link_id.size() - 5, 5, "CIS");
+  } else {
+    if (ends_with(link.link_id, "CIS"))
+      link.link_id.replace(link.link_id.size() - 3, 3, "TRANS");
+  }
+  link.is_cis = is_cis;
+}
+
+void force_cispeps(Topo& topo, bool single_model, const Model& model,
+                          const std::vector<CisPep>& cispeps,
+                          std::ostream* warnings) {
+  std::multimap<const Residue*, const CisPep*> cispep_index;
+  for (const CisPep& cp : cispeps) {
+    if (single_model || model.name == cp.model_str)
+      if (const Residue* res_n = model.find_cra(cp.partner_n).residue)
+        cispep_index.emplace(res_n, &cp);
+  }
+  for (Topo::ChainInfo& chain_info : topo.chain_infos)
+    for (Topo::ResInfo& res_info : chain_info.res_infos) {
+      auto range = cispep_index.equal_range(res_info.res);
+      for (Topo::Link& link : res_info.prev) {
+        bool is_cis = false;
+        for (auto i = range.first; i != range.second; ++i) {
+          const CisPep& cp = *i->second;
+          if (cp.partner_c.res_id.matches_noseg(*link.res1) &&
+              (cp.only_altloc == '\0' || cp.only_altloc == link.alt1
+                                      || cp.only_altloc == link.alt2))
+            is_cis = true;
+        }
+        if (is_cis != link.is_cis) {
+          set_cis_in_link(link, is_cis);
+          if (warnings)
+            *warnings << "Link between "
+                      << atom_str(chain_info.chain_ref.name, *link.res1, "", link.alt1)
+                      << " and "
+                      << atom_str(chain_info.chain_ref.name, *link.res2, "", link.alt2)
+                      << " forced to " << link.link_id << std::endl;
+        }
+      }
+    }
+}
+
+struct Neigh {
+  char alt;
+  float occ;
+};
+using NeighMap = std::unordered_multimap<int, Neigh>;
+
+// Assumes no hydrogens in the residue.
+// Position and serial number are not assigned for new atoms.
+void add_hydrogens_without_positions(Topo::ResInfo& ri, const NeighMap& neighbors) {
+  Residue& res = *ri.res;
+  // Add H atom for each conformation (altloc) of the parent atom and its
+  // first neighbors.
+  for (size_t i = 0, size = res.atoms.size(); i != size; ++i) {
+    char parent_alt = res.atoms[i].altloc;
+    float parent_occ = res.atoms[i].occ;
+    std::map<char, float> altlocs; // altloc + occupancy
+    if (parent_alt == '\0') {
+      float max_occ = 1.001f;
+      auto range = neighbors.equal_range(res.atoms[i].serial);
+      for (auto it = range.first; it != range.second; ++it) {
+        const Neigh& neigh = it->second;
+        if (neigh.alt && altlocs.count(neigh.alt) == 0 && neigh.occ < max_occ) {
+          altlocs.emplace(neigh.alt, neigh.occ * parent_occ);
+          max_occ -= neigh.occ;
+        }
+      }
+    }
+    if (altlocs.empty())
+      altlocs.emplace(parent_alt, parent_occ);
+    const ChemComp& cc = ri.get_final_chemcomp(parent_alt);
+    for (const Restraints::Bond& bond : cc.rt.bonds) {
+      // res.atoms may get re-allocated, so we can't set parent earlier
+      const Atom& parent = res.atoms[i];
+      assert(!parent.is_hydrogen());
+      const Restraints::AtomId* atom_id = bond.other(parent.name);
+      if (!atom_id)
+        continue;
+      auto it = cc.find_atom(atom_id->atom);
+      if (it == cc.atoms.end())
+        fail("inconsistent _chem_comp " + cc.name);
+      if (it->is_hydrogen()) {
+        gemmi::Atom atom;
+        atom.name = it->id;
+        atom.element = it->el;
+        // calc_flag will be changed to Calculated when the position is set
+        atom.calc_flag = CalcFlag::Dummy;
+        atom.b_iso = parent.b_iso;
+        for (auto alt_occ : altlocs) {
+          atom.altloc = alt_occ.first;
+          atom.occ = alt_occ.second;
+          res.atoms.push_back(atom);
+        }
+      }
+    }
+  }
+}
+
+NeighMap prepare_neighbor_data(Topo& topo, const MonLib& monlib) {
+  // disable warnings here, so they are not printed twice
+  std::streambuf *warnings_orig = nullptr;
+  if (topo.warnings)
+    warnings_orig = topo.warnings->rdbuf(nullptr);
+  // Prepare bonds. It fills topo.bonds - cleared later in this function,
+  // and monomer_rules/link_rules - overwritten if apply_all_restraints()
+  // is called again.
+  topo.only_bonds = true;
+  topo.apply_all_restraints(monlib);
+  topo.only_bonds = false;
+  // re-enable warnings
+  if (warnings_orig)
+    topo.warnings->rdbuf(warnings_orig);
+  NeighMap neighbors;
+  for (const Topo::Bond& bond : topo.bonds) {
+    const Atom* a1 = bond.atoms[0];
+    const Atom* a2 = bond.atoms[1];
+    neighbors.emplace(a1->serial, Neigh{a2->altloc, a2->occ});
+    if (a1 != a2)
+      neighbors.emplace(a2->serial, Neigh{a1->altloc, a1->occ});
+  }
+  topo.bonds.clear();
+  return neighbors;
+}
+
+}  // anonymous namespace
+
 std::unique_ptr<Topo>
 prepare_topology(Structure& st, MonLib& monlib, size_t model_index,
                  HydrogenChange h_change, bool reorder,
-                 std::ostream* warnings, bool ignore_unknown_links) {
+                 std::ostream* warnings, bool ignore_unknown_links, bool use_cispeps) {
   std::unique_ptr<Topo> topo(new Topo);
   topo->warnings = warnings;
   if (model_index >= st.models.size())
     fail("no such model index: " + std::to_string(model_index));
   topo->initialize_refmac_topology(st, st.models[model_index], monlib, ignore_unknown_links);
 
+  if (use_cispeps)
+    force_cispeps(*topo, st.models.size() == 1, st.models[model_index], st.cispeps, warnings);
 
-  for (Topo::ChainInfo& chain_info : topo->chain_infos) {
+  // remove hydrogens, or change deuterium to fraction, or nothing
+  // and then check atom names
+  for (Topo::ChainInfo& chain_info : topo->chain_infos)
     for (Topo::ResInfo& ri : chain_info.res_infos) {
       Residue& res = *ri.res;
       if (h_change != HydrogenChange::NoChange && h_change != HydrogenChange::Shift
           // don't re-add H's if we don't have chemical component description
           && (ri.orig_chemcomp != nullptr || h_change == HydrogenChange::Remove)) {
         // remove/add hydrogens
         remove_hydrogens(res);
-        if (h_change == HydrogenChange::ReAdd ||
-            (h_change == HydrogenChange::ReAddButWater && !res.is_water())) {
-          add_hydrogens_without_positions(ri);
-          if (h_change == HydrogenChange::ReAddButWater) {
-            // a special handling of HIS for compatibility with Refmac
-            if (res.name == "HIS") {
-              for (gemmi::Atom& atom : ri.res->atoms)
-                if (atom.name == "HD1" || atom.name == "HE2")
-                  atom.occ = 0;
-            }
-          }
-        }
       } else {
         // Special handling of Deuterium - mostly for Refmac.
         // Note: if the model has deuterium, it gets modified.
         if (replace_deuterium_with_fraction(res)) {
           // deuterium names usually differ from the names in dictionary
           for (Atom& atom : res.atoms)
             if (atom.name[0] == 'D' && atom.fraction != 0) {
@@ -717,30 +886,57 @@
           std::string msg = "definition not found for "
                           + atom_str(chain_info.chain_ref, *ri.res, atom);
           if (ri.orig_chemcomp && ri.orig_chemcomp->has_atom(atom.name))
             msg += " (linkage should remove this atom)";
           topo->err(msg);
         }
       }
-      // sort atoms in residues
+    }
+
+  // add hydrogens
+  if (h_change == HydrogenChange::ReAdd || h_change == HydrogenChange::ReAddButWater) {
+    NeighMap neighbors = prepare_neighbor_data(*topo, monlib);
+    for (Topo::ChainInfo& chain_info : topo->chain_infos)
+      for (Topo::ResInfo& ri : chain_info.res_infos) {
+        Residue& res = *ri.res;
+        if (ri.orig_chemcomp != nullptr &&
+            (h_change == HydrogenChange::ReAdd || !res.is_water())) {
+          add_hydrogens_without_positions(ri, neighbors);
+
+          // a special handling of HIS for compatibility with Refmac
+          if (res.name == "HIS") {
+            for (gemmi::Atom& atom : ri.res->atoms)
+              if (atom.name == "HD1" || atom.name == "HE2")
+                atom.occ = 0;
+          }
+        }
+      }
+  }
+
+  // sort atoms in residues
+  for (Topo::ChainInfo& chain_info : topo->chain_infos)
+    for (Topo::ResInfo& ri : chain_info.res_infos)
       if (reorder && ri.orig_chemcomp) {
+        Residue& res = *ri.res;
         const ChemComp& cc = *ri.orig_chemcomp;
         for (Atom& atom : res.atoms) {
           auto it = cc.find_atom(atom.name);
           // If atom.name is not found (b/c it was added in a modification),
           // the atom will be put after original atoms.
           atom.serial = int(it - cc.atoms.begin()); // temporary, for sorting only
         }
         std::sort(res.atoms.begin(), res.atoms.end(), [](const Atom& a, const Atom& b) {
                     return a.serial != b.serial ? a.serial < b.serial
                                                 : a.altloc < b.altloc;
         });
+        // check for missing altloc
+        for (auto atom = res.atoms.begin(); atom + 1 < res.atoms.end(); ++atom)
+          if (atom->name == (atom + 1)->name && atom->altloc == '\0')
+            topo->err("missing altloc in " + atom_str(chain_info.chain_ref, *ri.res, *atom));
       }
-    }
-  }
 
   // for atoms with ad-hoc links, for now we don't want hydrogens
   if (!ignore_unknown_links && h_change != HydrogenChange::NoChange) {
     auto remove_h_from_auto_links = [&](const Topo::Link& link) {
       const ChemLink* cl = monlib.get_link(link.link_id);
       if (cl && starts_with(cl->name, "auto-")) {
         const Restraints::Bond& bond = cl->rt.bonds.at(0);
@@ -753,18 +949,20 @@
         for (const Topo::Link& link : res_info.prev)
           remove_h_from_auto_links(link);
     for (const Topo::Link& link : topo->extras)
       remove_h_from_auto_links(link);
   }
 
   assign_serial_numbers(st.models[model_index]);
-  topo->finalize_refmac_topology(monlib);
+  // fill Topo::bonds, angles, ... and ResInfo::monomer_rules, Links::link_rules
+  topo->apply_all_restraints(monlib);
+  // fill bond_index, angle_index, etc
+  topo->create_indices();
 
   // the hydrogens added previously have positions not set
   if (h_change != HydrogenChange::NoChange)
     place_hydrogens_on_all_atoms(*topo);
 
   return topo;
 }
 
-
 }
```

### Comparing `gemmi-0.6.0/src/xds_ascii.cpp` & `gemmi-0.6.1/src/xds_ascii.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/adler32.c` & `gemmi-0.6.1/third_party/zlib/adler32.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/crc32.c` & `gemmi-0.6.1/third_party/zlib/crc32.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/crc32.h` & `gemmi-0.6.1/third_party/zlib/crc32.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/gzguts.h` & `gemmi-0.6.1/third_party/zlib/gzguts.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/gzlib.c` & `gemmi-0.6.1/third_party/zlib/gzlib.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/gzread.c` & `gemmi-0.6.1/third_party/zlib/gzread.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/inffast.c` & `gemmi-0.6.1/third_party/zlib/inffast.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/inffixed.h` & `gemmi-0.6.1/third_party/zlib/inffixed.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/inflate.c` & `gemmi-0.6.1/third_party/zlib/inflate.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/inflate.h` & `gemmi-0.6.1/third_party/zlib/inflate.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/inftrees.c` & `gemmi-0.6.1/third_party/zlib/inftrees.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/inftrees.h` & `gemmi-0.6.1/third_party/zlib/inftrees.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/license` & `gemmi-0.6.1/third_party/zlib/license`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/zconf.h` & `gemmi-0.6.1/third_party/zlib/zconf.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/zlib.h` & `gemmi-0.6.1/third_party/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/zutil.c` & `gemmi-0.6.1/third_party/zlib/zutil.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.0/third_party/zlib/zutil.h` & `gemmi-0.6.1/third_party/zlib/zutil.h`

 * *Files identical despite different names*

