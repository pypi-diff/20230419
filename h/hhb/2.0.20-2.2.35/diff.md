# Comparing `tmp/hhb-2.0.20-py3-none-any.whl.zip` & `tmp/hhb-2.2.35-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,47 +1,91 @@
-Zip file size: 87319 bytes, number of entries: 45
--rw-r--r--  2.0 unx      785 b- defN 22-Aug-22 06:09 hhb/__init__.py
--rw-r--r--  2.0 unx     8230 b- defN 22-Aug-22 06:09 hhb/benchmark.py
--rw-r--r--  2.0 unx     8302 b- defN 22-Aug-22 06:09 hhb/codegen.py
--rw-r--r--  2.0 unx     3136 b- defN 22-Aug-22 06:09 hhb/hhb.py
--rw-r--r--  2.0 unx     2927 b- defN 22-Aug-22 06:09 hhb/importer.py
--rw-r--r--  2.0 unx     5071 b- defN 22-Aug-22 06:09 hhb/profiler.py
--rw-r--r--  2.0 unx     5191 b- defN 22-Aug-22 06:09 hhb/quantizer.py
--rw-r--r--  2.0 unx     4335 b- defN 22-Aug-22 06:09 hhb/simulate.py
--rw-r--r--  2.0 unx     3070 b- defN 22-Aug-22 06:09 hhb/config/anole.tp
--rw-r--r--  2.0 unx     5456 b- defN 22-Aug-22 06:09 hhb/config/anole_multithread.tp
--rw-r--r--  2.0 unx     3243 b- defN 22-Aug-22 06:09 hhb/config/c906.tp
--rw-r--r--  2.0 unx     1194 b- defN 22-Aug-22 06:09 hhb/config/cb_map.tp
--rw-r--r--  2.0 unx     1135 b- defN 22-Aug-22 06:09 hhb/config/cb_reg.tp
--rw-r--r--  2.0 unx     3564 b- defN 22-Aug-22 06:09 hhb/config/light.tp
--rw-r--r--  2.0 unx     3225 b- defN 22-Aug-22 06:09 hhb/config/thead.tp
--rw-r--r--  2.0 unx     1539 b- defN 22-Aug-22 06:09 hhb/config/process/include/io.h
--rw-r--r--  2.0 unx     2040 b- defN 22-Aug-22 06:09 hhb/config/process/include/process.h
--rw-r--r--  2.0 unx     4946 b- defN 22-Aug-22 06:09 hhb/config/process/src/io.c
--rw-r--r--  2.0 unx    20086 b- defN 22-Aug-22 06:09 hhb/config/process/src/process.c
--rw-r--r--  2.0 unx       67 b- defN 22-Aug-22 06:09 hhb/config/template/function_decl.tp
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-22 06:09 hhb/config/template/global_var_decl.tp
--rw-r--r--  2.0 unx      134 b- defN 22-Aug-22 06:09 hhb/config/template/header.tp
--rw-r--r--  2.0 unx      116 b- defN 22-Aug-22 06:09 hhb/config/template/macro_def.tp
--rw-r--r--  2.0 unx      801 b- defN 22-Aug-22 06:09 hhb/config/template/postprocess_def.tp
--rw-r--r--  2.0 unx      792 b- defN 22-Aug-22 06:09 hhb/config/template/preprocess_def.tp
--rw-r--r--  2.0 unx      419 b- defN 22-Aug-22 06:09 hhb/config/template/utils_def.tp
--rw-r--r--  2.0 unx      785 b- defN 22-Aug-22 06:09 hhb/core/__init__.py
--rw-r--r--  2.0 unx    32697 b- defN 22-Aug-22 06:09 hhb/core/arguments_manage.py
--rw-r--r--  2.0 unx    44323 b- defN 22-Aug-22 06:09 hhb/core/codegen_manage.py
--rw-r--r--  2.0 unx    13688 b- defN 22-Aug-22 06:09 hhb/core/common.py
--rw-r--r--  2.0 unx    18616 b- defN 22-Aug-22 06:09 hhb/core/data_process.py
--rw-r--r--  2.0 unx    15010 b- defN 22-Aug-22 06:09 hhb/core/frontend_manage.py
--rw-r--r--  2.0 unx    27076 b- defN 22-Aug-22 06:09 hhb/core/hhbir_manage.py
--rw-r--r--  2.0 unx    13251 b- defN 22-Aug-22 06:09 hhb/core/main_command_manage.py
--rw-r--r--  2.0 unx     9915 b- defN 22-Aug-22 06:09 hhb/core/preprocess_manage.py
--rw-r--r--  2.0 unx     8100 b- defN 22-Aug-22 06:09 hhb/core/profiler_manage.py
--rw-r--r--  2.0 unx    26042 b- defN 22-Aug-22 06:09 hhb/core/quantization_manage.py
--rw-r--r--  2.0 unx     2837 b- defN 22-Aug-22 06:09 hhb/core/simulate_manage.py
--rw-r--r--  2.0 unx       10 b- defN 22-Aug-22 06:13 hhb-2.0.20.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx       38 b- defN 22-Aug-22 06:13 hhb-2.0.20.dist-info/entry_points.txt
--rw-r--r--  2.0 unx      581 b- defN 22-Aug-22 06:13 hhb-2.0.20.dist-info/metadata.json
--rw-r--r--  2.0 unx        4 b- defN 22-Aug-22 06:13 hhb-2.0.20.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-22 06:13 hhb-2.0.20.dist-info/WHEEL
--rw-r--r--  2.0 unx      410 b- defN 22-Aug-22 06:13 hhb-2.0.20.dist-info/METADATA
--rw-r--r--  2.0 unx     3708 b- defN 22-Aug-22 06:13 hhb-2.0.20.dist-info/RECORD
-45 files, 307079 bytes uncompressed, 81547 bytes compressed:  73.4%
+Zip file size: 6640325 bytes, number of entries: 89
+-rw-r--r--  2.0 unx     1221 b- defN 23-Mar-31 10:19 hhb/__init__.py
+-rw-r--r--  2.0 unx      889 b- defN 23-Mar-31 10:19 hhb/__main__.py
+-rw-r--r--  2.0 unx     8078 b- defN 23-Mar-31 10:19 hhb/benchmark.py
+-rw-r--r--  2.0 unx    10839 b- defN 23-Mar-31 10:19 hhb/codegen.py
+-rw-r--r--  2.0 unx     4646 b- defN 23-Mar-31 10:19 hhb/importer.py
+-rw-r--r--  2.0 unx    17814 b- defN 23-Mar-31 10:19 hhb/main.py
+-rw-r--r--  2.0 unx     3834 b- defN 23-Mar-31 10:19 hhb/profiler.py
+-rw-r--r--  2.0 unx     8557 b- defN 23-Mar-31 10:19 hhb/quantizer.py
+-rw-r--r--  2.0 unx     8185 b- defN 23-Mar-31 10:19 hhb/simulate.py
+-rw-r--r--  2.0 unx     3245 b- defN 23-Mar-31 10:19 hhb/config/anole.tp
+-rw-r--r--  2.0 unx     5662 b- defN 23-Mar-31 10:19 hhb/config/anole_multithread.tp
+-rw-r--r--  2.0 unx     3676 b- defN 23-Mar-31 10:19 hhb/config/c906.tp
+-rw-r--r--  2.0 unx     3517 b- defN 23-Mar-31 10:19 hhb/config/c906_cmdline.tp
+-rw-r--r--  2.0 unx     5125 b- defN 23-Mar-31 10:19 hhb/config/c920.tp
+-rw-r--r--  2.0 unx     3772 b- defN 23-Mar-31 10:19 hhb/config/th1520.tp
+-rw-r--r--  2.0 unx     1808 b- defN 23-Mar-31 10:19 hhb/config/th1520_jit.tp
+-rw-r--r--  2.0 unx     3225 b- defN 23-Mar-31 10:19 hhb/config/thead.tp
+-rw-r--r--  2.0 unx     3519 b- defN 23-Mar-31 10:19 hhb/config/x86_ref.tp
+-rw-r--r--  2.0 unx     1539 b- defN 23-Mar-31 10:19 hhb/config/process/include/io.h
+-rw-r--r--  2.0 unx     2040 b- defN 23-Mar-31 10:19 hhb/config/process/include/process.h
+-rw-r--r--  2.0 unx     4946 b- defN 23-Mar-31 10:19 hhb/config/process/src/io.c
+-rw-r--r--  2.0 unx    20086 b- defN 23-Mar-31 10:19 hhb/config/process/src/process.c
+-rw-r--r--  2.0 unx      110 b- defN 23-Mar-31 10:19 hhb/config/template/function_decl.tp
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-31 10:19 hhb/config/template/global_var_decl.tp
+-rw-r--r--  2.0 unx      134 b- defN 23-Mar-31 10:19 hhb/config/template/header.tp
+-rw-r--r--  2.0 unx      116 b- defN 23-Mar-31 10:19 hhb/config/template/macro_def.tp
+-rw-r--r--  2.0 unx     1128 b- defN 23-Mar-31 10:19 hhb/config/template/makefile.tp
+-rw-r--r--  2.0 unx      862 b- defN 23-Mar-31 10:19 hhb/config/template/postprocess_def.tp
+-rw-r--r--  2.0 unx      792 b- defN 23-Mar-31 10:19 hhb/config/template/preprocess_def.tp
+-rw-r--r--  2.0 unx      419 b- defN 23-Mar-31 10:19 hhb/config/template/utils_def.tp
+-rw-r--r--  2.0 unx      785 b- defN 23-Mar-31 10:19 hhb/core/__init__.py
+-rw-r--r--  2.0 unx    53534 b- defN 23-Mar-31 10:19 hhb/core/arguments_manage.py
+-rw-r--r--  2.0 unx    45715 b- defN 23-Mar-31 10:19 hhb/core/codegen_manage.py
+-rw-r--r--  2.0 unx    15217 b- defN 23-Mar-31 10:19 hhb/core/common.py
+-rw-r--r--  2.0 unx    20536 b- defN 23-Mar-31 10:19 hhb/core/data_process.py
+-rw-r--r--  2.0 unx    14277 b- defN 23-Mar-31 10:19 hhb/core/frontend_manage.py
+-rw-r--r--  2.0 unx    41922 b- defN 23-Mar-31 10:19 hhb/core/hhbir_manage.py
+-rw-r--r--  2.0 unx    15817 b- defN 23-Mar-31 10:19 hhb/core/main_command_manage.py
+-rw-r--r--  2.0 unx    11534 b- defN 23-Mar-31 10:19 hhb/core/preprocess_manage.py
+-rw-r--r--  2.0 unx     8104 b- defN 23-Mar-31 10:19 hhb/core/profiler_manage.py
+-rw-r--r--  2.0 unx    28522 b- defN 23-Mar-31 10:19 hhb/core/quantization_manage.py
+-rw-r--r--  2.0 unx     4569 b- defN 23-Mar-31 10:19 hhb/core/simulate_manage.py
+-rw-r--r--  2.0 unx        7 b- defN 23-Mar-31 10:29 hhb/install_nn2/version
+-rw-r--r--  2.0 unx   202441 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/csi_nn.h
+-rw-r--r--  2.0 unx    48693 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/csinn_data_structure.h
+-rw-r--r--  2.0 unx    10205 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/csinn_runtime.h
+-rw-r--r--  2.0 unx     2762 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_asp.h
+-rw-r--r--  2.0 unx      985 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_c860.h
+-rw-r--r--  2.0 unx    29180 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_c906.h
+-rw-r--r--  2.0 unx    26316 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_c908.h
+-rw-r--r--  2.0 unx     4965 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_c920.h
+-rw-r--r--  2.0 unx    16162 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_debug.h
+-rw-r--r--  2.0 unx     3566 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_e804.h
+-rw-r--r--  2.0 unx     3290 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_e907.h
+-rw-r--r--  2.0 unx    64719 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_gref.h
+-rw-r--r--  2.0 unx     6922 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_i805.h
+-rw-r--r--  2.0 unx     1099 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_memory.h
+-rw-r--r--  2.0 unx     1951 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_node.h
+-rw-r--r--  2.0 unx    18655 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_ovx.h
+-rw-r--r--  2.0 unx    12782 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_pnna.h
+-rw-r--r--  2.0 unx    67603 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_ref.h
+-rw-r--r--  2.0 unx     3636 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_ref_i805.h
+-rw-r--r--  2.0 unx     7001 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_thead_rvm.h
+-rw-r--r--  2.0 unx    61404 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_thead_rvv.h
+-rw-r--r--  2.0 unx     1320 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_tvmgen.h
+-rw-r--r--  2.0 unx     3693 b- defN 23-Mar-31 10:29 hhb/install_nn2/include/shl_utils.h
+-rw-r--r--  2.0 unx  4536246 b- defN 23-Mar-31 10:29 hhb/install_nn2/lib/libshl_c906.a
+-rw-r--r--  2.0 unx  4490130 b- defN 23-Mar-31 10:29 hhb/install_nn2/lib/libshl_c908.a
+-rw-r--r--  2.0 unx  3964884 b- defN 23-Mar-31 10:29 hhb/install_nn2/lib/libshl_c920.a
+-rw-r--r--  2.0 unx   263152 b- defN 23-Mar-31 10:29 hhb/install_nn2/lib/libshl_openvx.so
+-rw-r--r--  2.0 unx   671848 b- defN 23-Mar-31 10:29 hhb/install_nn2/lib/libshl_pnna.so
+-rw-r--r--  2.0 unx   852112 b- defN 23-Mar-31 10:29 hhb/install_nn2/lib/libshl_pnna_x86.so
+-rw-r--r--  2.0 unx  1687534 b- defN 23-Mar-31 10:29 hhb/install_nn2/lib/libshl_ref_x86.a
+-rw-r--r--  2.0 unx  3981788 b- defN 23-Mar-31 10:29 hhb/install_nn2/lib/libshl_rvm.a
+-rw-r--r--  2.0 unx  1107632 b- defN 23-Mar-31 10:29 hhb/install_nn2/lib/libshl_th1520.so
+-rw-r--r--  2.0 unx   552460 b- defN 23-Mar-31 10:29 hhb/prebuilt/decode/install/lib/rv/libjpeg.a
+-rw-r--r--  2.0 unx   666746 b- defN 23-Mar-31 10:29 hhb/prebuilt/decode/install/lib/rv/libpng.a
+-rw-r--r--  2.0 unx   277994 b- defN 23-Mar-31 10:29 hhb/prebuilt/decode/install/lib/rv/libz.a
+-rw-r--r--  2.0 unx   336620 b- defN 23-Mar-31 10:29 hhb/prebuilt/decode/install/lib/x86/libjpeg.a
+-rw-r--r--  2.0 unx   335266 b- defN 23-Mar-31 10:29 hhb/prebuilt/decode/install/lib/x86/libpng.a
+-rw-r--r--  2.0 unx   167410 b- defN 23-Mar-31 10:29 hhb/prebuilt/decode/install/lib/x86/libz.a
+-rw-r--r--  2.0 unx      356 b- defN 23-Mar-31 10:29 hhb/prebuilt/runtime/cmd_parse/cmd_parse.h
+-rw-r--r--  2.0 unx  3266478 b- defN 23-Mar-31 10:29 hhb/prebuilt/runtime/riscv_linux/libprebuilt_runtime.a
+-rw-r--r--  2.0 unx   474784 b- defN 23-Mar-31 10:29 hhb/prebuilt/runtime/x86_linux/libprebuilt_runtime.a
+-rw-r--r--  2.0 unx      410 b- defN 23-Mar-31 10:29 hhb-2.2.35.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-31 10:29 hhb-2.2.35.dist-info/WHEEL
+-rw-r--r--  2.0 unx       39 b- defN 23-Mar-31 10:29 hhb-2.2.35.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Mar-31 10:29 hhb-2.2.35.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     7808 b- defN 23-Mar-31 10:29 hhb-2.2.35.dist-info/RECORD
+89 files, 28631558 bytes uncompressed, 6628045 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -1,20 +1,23 @@
 Filename: hhb/__init__.py
 Comment: 
 
+Filename: hhb/__main__.py
+Comment: 
+
 Filename: hhb/benchmark.py
 Comment: 
 
 Filename: hhb/codegen.py
 Comment: 
 
-Filename: hhb/hhb.py
+Filename: hhb/importer.py
 Comment: 
 
-Filename: hhb/importer.py
+Filename: hhb/main.py
 Comment: 
 
 Filename: hhb/profiler.py
 Comment: 
 
 Filename: hhb/quantizer.py
 Comment: 
@@ -27,26 +30,32 @@
 
 Filename: hhb/config/anole_multithread.tp
 Comment: 
 
 Filename: hhb/config/c906.tp
 Comment: 
 
-Filename: hhb/config/cb_map.tp
+Filename: hhb/config/c906_cmdline.tp
+Comment: 
+
+Filename: hhb/config/c920.tp
 Comment: 
 
-Filename: hhb/config/cb_reg.tp
+Filename: hhb/config/th1520.tp
 Comment: 
 
-Filename: hhb/config/light.tp
+Filename: hhb/config/th1520_jit.tp
 Comment: 
 
 Filename: hhb/config/thead.tp
 Comment: 
 
+Filename: hhb/config/x86_ref.tp
+Comment: 
+
 Filename: hhb/config/process/include/io.h
 Comment: 
 
 Filename: hhb/config/process/include/process.h
 Comment: 
 
 Filename: hhb/config/process/src/io.c
@@ -63,14 +72,17 @@
 
 Filename: hhb/config/template/header.tp
 Comment: 
 
 Filename: hhb/config/template/macro_def.tp
 Comment: 
 
+Filename: hhb/config/template/makefile.tp
+Comment: 
+
 Filename: hhb/config/template/postprocess_def.tp
 Comment: 
 
 Filename: hhb/config/template/preprocess_def.tp
 Comment: 
 
 Filename: hhb/config/template/utils_def.tp
@@ -108,29 +120,149 @@
 
 Filename: hhb/core/quantization_manage.py
 Comment: 
 
 Filename: hhb/core/simulate_manage.py
 Comment: 
 
-Filename: hhb-2.0.20.dist-info/DESCRIPTION.rst
+Filename: hhb/install_nn2/version
+Comment: 
+
+Filename: hhb/install_nn2/include/csi_nn.h
+Comment: 
+
+Filename: hhb/install_nn2/include/csinn_data_structure.h
+Comment: 
+
+Filename: hhb/install_nn2/include/csinn_runtime.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_asp.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_c860.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_c906.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_c908.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_c920.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_debug.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_e804.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_e907.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_gref.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_i805.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_memory.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_node.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_ovx.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_pnna.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_ref.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_ref_i805.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_thead_rvm.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_thead_rvv.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_tvmgen.h
+Comment: 
+
+Filename: hhb/install_nn2/include/shl_utils.h
+Comment: 
+
+Filename: hhb/install_nn2/lib/libshl_c906.a
+Comment: 
+
+Filename: hhb/install_nn2/lib/libshl_c908.a
+Comment: 
+
+Filename: hhb/install_nn2/lib/libshl_c920.a
+Comment: 
+
+Filename: hhb/install_nn2/lib/libshl_openvx.so
+Comment: 
+
+Filename: hhb/install_nn2/lib/libshl_pnna.so
+Comment: 
+
+Filename: hhb/install_nn2/lib/libshl_pnna_x86.so
+Comment: 
+
+Filename: hhb/install_nn2/lib/libshl_ref_x86.a
+Comment: 
+
+Filename: hhb/install_nn2/lib/libshl_rvm.a
+Comment: 
+
+Filename: hhb/install_nn2/lib/libshl_th1520.so
+Comment: 
+
+Filename: hhb/prebuilt/decode/install/lib/rv/libjpeg.a
+Comment: 
+
+Filename: hhb/prebuilt/decode/install/lib/rv/libpng.a
+Comment: 
+
+Filename: hhb/prebuilt/decode/install/lib/rv/libz.a
+Comment: 
+
+Filename: hhb/prebuilt/decode/install/lib/x86/libjpeg.a
+Comment: 
+
+Filename: hhb/prebuilt/decode/install/lib/x86/libpng.a
+Comment: 
+
+Filename: hhb/prebuilt/decode/install/lib/x86/libz.a
+Comment: 
+
+Filename: hhb/prebuilt/runtime/cmd_parse/cmd_parse.h
+Comment: 
+
+Filename: hhb/prebuilt/runtime/riscv_linux/libprebuilt_runtime.a
 Comment: 
 
-Filename: hhb-2.0.20.dist-info/entry_points.txt
+Filename: hhb/prebuilt/runtime/x86_linux/libprebuilt_runtime.a
 Comment: 
 
-Filename: hhb-2.0.20.dist-info/metadata.json
+Filename: hhb-2.2.35.dist-info/METADATA
 Comment: 
 
-Filename: hhb-2.0.20.dist-info/top_level.txt
+Filename: hhb-2.2.35.dist-info/WHEEL
 Comment: 
 
-Filename: hhb-2.0.20.dist-info/WHEEL
+Filename: hhb-2.2.35.dist-info/entry_points.txt
 Comment: 
 
-Filename: hhb-2.0.20.dist-info/METADATA
+Filename: hhb-2.2.35.dist-info/top_level.txt
 Comment: 
 
-Filename: hhb-2.0.20.dist-info/RECORD
+Filename: hhb-2.2.35.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hhb/__init__.py

```diff
@@ -10,7 +10,26 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
+
+
+from . import benchmark
+from . import importer
+from . import codegen
+from . import profiler
+from . import quantizer
+from . import simulate
+
+# main
+from .main import Compiler
+from .main import Profiler
+from .core.arguments_manage import Config
+
+# common
+from .core.arguments_manage import generate_hhb_default_config
+from .core.common import convert_invalid_symbol
+from .core.common import print_top5
+from .main import set_debug_level
```

## hhb/benchmark.py

```diff
@@ -27,57 +27,57 @@
 
 import numpy as np
 
 import tvm
 from tvm import runtime
 from tvm.contrib import graph_executor
 
-from core.frontend_manage import import_model
-from core.common import hhb_register_parse, print_top5, HHBException, ensure_dir, AttributeDict
-from core.common import generate_config_file, ALL_ARGUMENTS_DESC, collect_arguments_info
-from core.arguments_manage import (
+from .core.frontend_manage import import_model
+from .core.common import hhb_register_parse, print_top5, HHBException, ensure_dir, AttributeDict
+from .core.common import generate_config_file, ALL_ARGUMENTS_DESC, collect_arguments_info
+from .core.arguments_manage import (
     add_preprocess_argument,
     add_common_argument,
     add_simulate_argument,
     add_postprocess_argument,
     add_import_argument,
     add_optimize_argument,
     add_quantize_argument,
     add_hardware_argument,
     add_codegen_argument,
     ArgumentFilter,
 )
-from core.hhbir_manage import (
+from .core.hhbir_manage import (
     HHBRelayIR,
     HHBQNNIR,
     HHBFloatCodegenIR,
     HHBX86QnnCodegenIR,
     get_input_info_from_relay,
     get_output_info_from_relay,
 )
-from core.quantization_manage import (
+from .core.quantization_manage import (
     collect_quantization_config,
     set_quantize_params_by_board,
     get_config_dict,
 )
-from core.preprocess_manage import (
+from .core.preprocess_manage import (
     collect_preprocess_config,
     set_preprocess_params,
     DatasetLoader,
 )
-from core.codegen_manage import collect_codegen_config
+from .core.codegen_manage import collect_codegen_config
 
 
 # pylint: disable=invalid-name
 logger = logging.getLogger("HHB")
 
 
 @hhb_register_parse
 def add_benchmark_parser(subparsers):
-    """ Include parser for 'benchmark' subcommand """
+    """Include parser for 'benchmark' subcommand"""
 
     parser = subparsers.add_parser("benchmark")
     parser.set_defaults(func=driver_benchmark)
 
     parser.add_argument(
         "--reference-label", metavar="", type=str, help="The true labels of test dataset."
     )
@@ -101,20 +101,14 @@
     add_postprocess_argument(parser)
     add_common_argument(parser)
     add_optimize_argument(parser)
     add_codegen_argument(parser)
 
     parser.add_argument("-v", "--verbose", action="count", default=0, help="Increase verbosity")
     parser.add_argument(
-        "-o",
-        "--output",
-        default="hhb_out",
-        help="The directory that holds the result files.",
-    )
-    parser.add_argument(
         "FILE", nargs="+", help="Path to the input model file, can pass multi files"
     )
 
     ALL_ARGUMENTS_DESC["benchmark"] = collect_arguments_info(parser._actions)
 
 
 def driver_benchmark(args_filter: ArgumentFilter):
@@ -166,15 +160,15 @@
             x86_codegen_ir.convert((mod, params), args.board, args.opt_level)
         else:
             x86_codegen_ir = HHBX86QnnCodegenIR()
             x86_codegen_ir.convert(
                 qnn_ir.get_model(), args.board, args.opt_level, args.output, config_dict
             )
     else:
-        raise HHBException("can not simulate anole, light or c860.")
+        raise HHBException("can not simulate anole, th1520.")
 
     ctx = tvm.cpu(0)
     if args.no_quantize:
         m = graph_executor.GraphModule(x86_codegen_ir.get_model()["default"](ctx))
     else:
         factory = x86_codegen_ir.get_factory()
         lib = x86_codegen_ir.get_lib(args.output)
```

## hhb/codegen.py

```diff
@@ -15,73 +15,159 @@
 # specific language governing permissions and limitations
 # under the License.
 """
 Codegen the imported model.
 """
 import logging
 import os
+import copy
 
-from core.arguments_manage import (
+import tvm
+from tvm import relay
+from tvm.relay.op.contrib import csinn
+
+from .core.arguments_manage import (
     add_optimize_argument,
     add_common_argument,
     add_postprocess_argument,
     add_codegen_argument,
     add_hardware_argument,
     ArgumentFilter,
 )
-from core.common import (
+from .core.common import (
     hhb_register_parse,
     HHBException,
     ensure_dir,
     generate_config_file,
     ALL_ARGUMENTS_DESC,
     collect_arguments_info,
     AttributeDict,
+    get_target,
 )
-from core.hhbir_manage import (
+from .core.hhbir_manage import (
     guess_ir_type,
     HHBIRType,
     HHBRelayIR,
     HHBQNNIR,
     HHBFloatCodegenIR,
     HHBX86QnnCodegenIR,
     HHBBoardQnnCodegenIR,
     get_input_info_from_relay,
     get_output_info_from_relay,
 )
-from core.codegen_manage import collect_codegen_config, set_codegen_config
-from core.preprocess_manage import (
+from .core.codegen_manage import collect_codegen_config, set_codegen_config
+from .core.preprocess_manage import (
     collect_preprocess_config,
     set_preprocess_params,
 )
+from .core.quantization_manage import get_config_dict
 
 # pylint: disable=invalid-name
 logger = logging.getLogger("HHB")
 
 
+def hhb_codegen(hhb_ir, config):
+    """Codegen hhb model.
+
+    Parameters
+    ----------
+    hhb_ir : HHBIRBase
+        HHB ir wrapper that holds module and params
+    config : Config
+        All config for HHB
+
+    Returns
+    -------
+    ret : HHBIRBase or None
+        If the board is x86_ref, ret is HHBFloatCodegenIR/HHBX86QnnCodegenIR;
+        otherwise, ret is None.
+    """
+    mod, params = hhb_ir.get_model()
+    hhb_config = config._cmd_config
+    ret = None
+
+    opt_level = 3
+    target_board_list = (
+        "anole",
+        "th1520",
+        "hth1520",
+        "e907",
+        "c906",
+        "rvm",
+        "c908",
+        "c920",
+    )
+    config_dict = get_config_dict(hhb_config)
+
+    quantized = False
+    if isinstance(hhb_ir, HHBQNNIR):
+        quantized = True
+    if hhb_config.board == "x86_ref":
+        if not quantized:
+            x86_codegen_ir = HHBFloatCodegenIR()
+            x86_codegen_ir.convert((mod, params), hhb_config.board, opt_level)
+        else:
+            ensure_dir(hhb_config.output)
+            x86_codegen_ir = HHBX86QnnCodegenIR()
+            x86_codegen_ir.convert(
+                (mod, params), hhb_config.board, opt_level, hhb_config.output, config_dict
+            )
+        ret = x86_codegen_ir
+    elif hhb_config.board in target_board_list:
+        ensure_dir(hhb_config.output)
+        if not quantized:
+            raise HHBException(
+                "model should be quantized while setting '--board {}'.\n".format(hhb_config.board)
+            )
+        board_codegen_ir = HHBBoardQnnCodegenIR()
+
+        board_codegen_ir.convert(
+            (mod, params),
+            hhb_config.board,
+            opt_level,
+            hhb_config.output,
+            config_dict,
+        )
+
+        _, input_shape_list, _ = get_input_info_from_relay(mod, None)
+        output_shape_list, _ = get_output_info_from_relay(mod, None)
+        board_codegen_ir.save_model(
+            input_shape_list,
+            output_shape_list,
+            hhb_config.board,
+            hhb_config.output,
+            hhb_config.postprocess,
+            hhb_config.codegen_config.model_save,
+            hhb_config.codegen_config.without_preprocess,
+            hhb_config.preprocess_config,
+            hhb_config.codegen_config.multithread,
+            hhb_config.codegen_config.input_memory_type,
+            hhb_config.quantize_config.quantization_scheme,
+            hhb_config.codegen_config,
+        )
+        ret = board_codegen_ir
+    else:
+        raise HHBException("unsupport for board: {}.\n".format(hhb_config.board))
+
+    return ret
+
+
 @hhb_register_parse
 def add_codegen_parser(subparsers):
-    """ Include parser for 'codegen' subcommand """
+    """Include parser for 'codegen' subcommand"""
 
     parser = subparsers.add_parser("codegen", help="Codegen the imported model")
     parser.set_defaults(func=driver_codegen)
 
     add_optimize_argument(parser)
     add_postprocess_argument(parser)
     add_codegen_argument(parser)
     add_hardware_argument(parser)
     add_common_argument(parser)
 
-    parser.add_argument(
-        "-o",
-        "--output",
-        metavar="",
-        default="hhb_out",
-        help="The directory that holds the codegen files.",
-    )
     parser.add_argument("-v", "--verbose", action="count", default=0, help="Increase verbosity")
     parser.add_argument("FILE", help="Directory to the model file")
 
     ALL_ARGUMENTS_DESC["codegen"] = collect_arguments_info(parser._actions)
 
 
 def driver_codegen(args_filter: ArgumentFilter):
@@ -125,21 +211,21 @@
                 input_module, args.board, args.opt_level, args.output, quantize_config
             )
             x86_qnn_codegen_ir.save_model(args.output)
         else:
             raise HHBException("unsupport for IR type: {}".format(HHBIRType.TYPE2NAME[model_type]))
     elif args.board in (
         "anole",
-        "light",
-        "hlight",
-        "asp",
-        "i805",
-        "c860",
+        "th1520",
+        "hth1520",
+        "e907",
         "c906",
+        "rvm",
         "c908",
+        "c920",
     ):
         if model_type != HHBIRType.QNN:
             raise HHBException(
                 "IR type: {} can not be converted to board codegen".format(
                     HHBIRType.TYPE2NAME[model_type]
                 )
             )
@@ -159,43 +245,44 @@
         extra_args.input_shape = input_shape
         extra_args.input_num = len(input_shape)
         extra_args.output_num = len(output_shape)
         extra_args.model_save = args.model_save
         args_filter.filter_argument(all_filters, extra=extra_args)
         args = args_filter.filtered_args
 
-        light_input_fix_size = qnn_ir.info_dict["preprocess"]["light_input_fix_size"]
+        th1520_input_fix_size = args.codegen_config.th1520_input_fix_size
 
         # convert to board qnn codegen ir
         board_qnn_codegen_ir = HHBBoardQnnCodegenIR()
         quantize_config = board_qnn_codegen_ir.get_quant_env(
             os.path.join(args.FILE, qnn_ir.info_file)
         )
+        if args.board == "th1520" and (
+            args.hybrid_computing or quantize_config["auto_hybrid_quantization"]
+        ):
+            args.board = "hth1520"
 
         quantize_config["h_max_out_channel"] = args.hardware_max_out_channel
         quantize_config["h_max_kernel_size"] = args.hardware_max_kernel_size
         quantize_config["h_contain_weight"] = args.hardware_contain_weight
         quantize_config["h_align"] = args.hardware_alignment
         quantize_config["model_save"] = args.model_save
         quantize_config["model_priority"] = args.codegen_config.model_priority
-        quantize_config["structed_sparsity"] = args.structed_sparsity
-        quantize_config["kernel_parallel"] = args.kernel_parallel
+        quantize_config["matrix_extension_mlen"] = args.matrix_extension_mlen
         quantize_config["target"] = args.board
         quantize_config["multi_thread"] = args.codegen_config.multithread
 
-        if len(light_input_fix_size) == 2:
-            quantize_config["light_input_fix_height"] = light_input_fix_size[0]
-            quantize_config["light_input_fix_width"] = light_input_fix_size[1]
-        if args.board == "light" and args.codegen_config.model_save == "save_only":
-            quantize_config["target"] = "light_new"
+        if len(th1520_input_fix_size) == 2:
+            quantize_config["th1520_input_fix_height"] = th1520_input_fix_size[0]
+            quantize_config["th1520_input_fix_width"] = th1520_input_fix_size[1]
         if args.verbose >= 3:
             quantize_config["debug_level"] = "INFO"
         if args.codegen_config.model_save == "save_only":
             quantize_config["h_sram_size"] = (
-                2 ** 20 if not args.hardware_sram_size else args.hardware_sram_size
+                2**20 if not args.hardware_sram_size else args.hardware_sram_size
             )
             quantize_config["h_max_groups"] = (
                 16 if not args.hardware_max_groups else args.hardware_max_groups
             )
         quantize_config["trace_strategy"] = args.codegen_config.trace_strategy
         quantize_config["input_memory_type"] = args.codegen_config.input_memory_type
         quantize_config["output_memory_type"] = args.codegen_config.output_memory_type
```

## hhb/importer.py

```diff
@@ -15,49 +15,106 @@
 # specific language governing permissions and limitations
 # under the License.
 """
 Import networks into relay IR.
 """
 import logging
 import os
+import sys
 
-from core.common import hhb_register_parse
-from core.common import ensure_dir
-from core.common import generate_config_file
-from core.common import ALL_ARGUMENTS_DESC
-from core.common import collect_arguments_info
-from core.arguments_manage import add_import_argument
-from core.arguments_manage import add_optimize_argument
-from core.arguments_manage import add_common_argument
-from core.frontend_manage import import_model
-from core.hhbir_manage import HHBRelayIR
+import tvm
+
+from .core.common import hhb_register_parse
+from .core.common import ensure_dir
+from .core.common import generate_config_file
+from .core.common import ALL_ARGUMENTS_DESC
+from .core.common import collect_arguments_info
+from .core.arguments_manage import add_import_argument
+from .core.arguments_manage import add_optimize_argument
+from .core.arguments_manage import add_common_argument
+from .core.frontend_manage import import_model
+from .core.hhbir_manage import HHBRelayIR
 
 
 # pylint: disable=invalid-name
 logger = logging.getLogger("HHB")
 
 
+def save_imported_model(mod, params, output_dir="."):
+    """Save imported model into file.
+
+    Parameters
+    ----------
+    mod : tvm.IRModule
+        The relay module for compilation
+    params : dict of str to tvm.nd.NDArray
+        The parameter dict to be used by relay
+    output_dir : str
+        The output directory holding file.
+    """
+    mod_path = os.path.join(output_dir, "relay.txt")
+    params_path = os.path.join(output_dir, "relay.params")
+
+    with open(mod_path, "w") as f:
+        f.write(mod.astext())
+
+    with open(params_path, "wb") as f:
+        f.write(tvm.relay.save_param_dict(params))
+
+
+def hhb_import(
+    path, model_format=None, input_name=None, input_shape=None, output_name=None, save_to_dir=None
+) -> HHBRelayIR:
+    """Import a model from a supported framework into relay ir.
+
+    Parameters
+    ----------
+    path : str or list[str]
+        Path to a model file. There may be two files(.caffemodel, .prototxt) for Caffe model
+    model_format : str, optional
+        A string representing input model format
+    input_name : list[str], optional
+        The names of input node in the graph
+    input_shape : list[list[int]], optional
+        The shape of input node in the graph
+    output_name : list[str], optional
+        The name of output node in the graph
+    save_to_dir : str, optional
+        save model into specified directory
+
+    Returns
+    -------
+    relay_ir : HHBRelayIR
+        Relay ir wrapper that holds module and params
+    """
+    if isinstance(path, str):
+        path = [path]
+    mod, params = import_model(path, model_format, input_name, input_shape, output_name)
+
+    if save_to_dir is not None:
+        save_to_dir = ensure_dir(save_to_dir)
+        save_imported_model(mod, params, save_to_dir)
+
+    relay_ir = HHBRelayIR()
+    relay_ir.set_model(mod, params)
+
+    return relay_ir
+
+
 @hhb_register_parse
 def add_import_parser(subparsers):
-    """ Include parser for 'import' subcommand """
+    """Include parser for 'import' subcommand"""
 
     parser = subparsers.add_parser("import", help="Import a model into relay ir")
     parser.set_defaults(func=driver_import)
 
     add_import_argument(parser)
     # add_optimize_argument(parser)
     add_common_argument(parser)
 
-    parser.add_argument(
-        "-o",
-        "--output",
-        metavar="",
-        default="hhb_out",
-        help="The directory that holds the relay ir.",
-    )
     parser.add_argument("-v", "--verbose", action="count", default=0, help="Increase verbosity")
     parser.add_argument(
         "FILE", nargs="+", help="Path to the input model file, can pass multi files"
     )
 
     ALL_ARGUMENTS_DESC["import"] = collect_arguments_info(parser._actions)
```

## hhb/profiler.py

```diff
@@ -25,52 +25,44 @@
 
 import numpy as np
 
 import tvm
 from tvm import relay
 from tvm.relay.quantize.quantize_hhb import _bind_params
 
-from core.frontend_manage import import_model
-from core.common import hhb_register_parse, HHBException, ensure_dir
-from core.common import generate_config_file, ALL_ARGUMENTS_DESC, collect_arguments_info
-from core.arguments_manage import (
+from .core.frontend_manage import import_model
+from .core.common import hhb_register_parse, HHBException, ensure_dir
+from .core.common import generate_config_file, ALL_ARGUMENTS_DESC, collect_arguments_info
+from .core.arguments_manage import (
     add_common_argument,
     add_import_argument,
     add_profiler_argument,
     ArgumentFilter,
 )
-from core.profiler_manage import convert_tvm_trace2python, aitrace_options
-from core.profiler_manage import get_cal_total_info, print_cal_total_info
-from core.profiler_manage import get_mem_total_info, print_mem_total_info
-from core.profiler_manage import profile_light_trace, dump_profile_result
+from .core.profiler_manage import convert_tvm_trace2python, aitrace_options
+from .core.profiler_manage import dump_profile_result
 
 
 # pylint: disable=invalid-name
 logger = logging.getLogger("HHB")
 
 
 @hhb_register_parse
 def add_profiler_parser(subparsers):
-    """ Include parser for 'profiler' subcommand """
+    """Include parser for 'profiler' subcommand"""
 
     parser = subparsers.add_parser("profiler", help="profile model")
     parser.set_defaults(func=driver_profiler)
 
     add_import_argument(parser)
     add_profiler_argument(parser)
     add_common_argument(parser)
 
     parser.add_argument("-v", "--verbose", action="count", default=0, help="Increase verbosity")
     parser.add_argument(
-        "-o",
-        "--output",
-        default="hhb_out",
-        help="The directory that holds the result files.",
-    )
-    parser.add_argument(
         "-f", "--model-file", nargs="+", help="Path to the input model file, can pass multi files"
     )
 
     ALL_ARGUMENTS_DESC["profiler"] = collect_arguments_info(parser._actions)
 
 
 def driver_profiler(args_filter: ArgumentFilter):
@@ -109,28 +101,9 @@
         ]
         mod = transform.Sequential(opt_seq, opt_level=3)(mod)
 
         result = relay.analysis.get_aitrace_data(mod["main"], options)
         result = convert_tvm_trace2python(result)
 
         dump_profile_result(result, args.output_type, args.indicator, args.ir_type, args.output)
-    elif args.ir_type == "light":
-        if "cal" in args.indicator:
-            logger.error("Unsupport 'cal' for indicator while setting --ir-type light.")
-            sys.exit()
-        if "binary" in args.output_type:
-            logger.error("Unsupport 'binary' for --output-type while setting --ir-type light.")
-            sys.exit()
-        if not args.model_file or not os.path.exists(args.model_file[0]):
-            logger.error("File not exits: %s" % args.model_file[0])
-            sys.exit()
-        try:
-            with open(args.model_file[0], "r") as f:
-                trace_data = json.load(f)
-        except:
-            logger.error("Invalid file for light profiling: %s." % args.model_file)
-            sys.exit()
-
-        result = profile_light_trace(trace_data, args.indicator, args.npu_frequency)
-        dump_profile_result(result, args.output_type, args.indicator, args.ir_type, args.output)
     else:
         raise HHBException("Unsupport for profiling type: {}\n".format(args.ir_type))
```

## hhb/quantizer.py

```diff
@@ -16,93 +16,187 @@
 # under the License.
 # pylint: disable=unnecessary-comprehension
 """
 Optimize the imported model.
 """
 import logging
 import os
+from tvm.relay.quantize.quantize_hhb import detect_quantized_model
 
-from core.common import (
+from .core.common import (
     hhb_register_parse,
     HHBException,
     AttributeDict,
     ensure_dir,
     generate_config_file,
     ALL_ARGUMENTS_DESC,
     collect_arguments_info,
 )
-from core.arguments_manage import (
+from .core.frontend_manage import insert_preprocess_node
+from .core.arguments_manage import (
     add_preprocess_argument,
     add_quantize_argument,
     add_hardware_argument,
     add_codegen_argument,
     add_common_argument,
     add_optimize_argument,
     ArgumentFilter,
 )
-from core.hhbir_manage import (
+from .core.hhbir_manage import (
     HHBRelayIR,
     HHBQNNIR,
     get_input_info_from_relay,
     get_output_info_from_relay,
 )
-from core.quantization_manage import (
+from .core.quantization_manage import (
     collect_quantization_config,
     set_quantize_params_by_board,
     get_config_dict,
+    quantize_model,
+    update_hybrid_layer,
+    ignore_layers_from_auto_quant,
 )
-from core.codegen_manage import (
+from .core.codegen_manage import (
     collect_codegen_config,
     set_codegen_config,
 )
-from core.preprocess_manage import collect_preprocess_config, set_preprocess_params, DatasetLoader
+from .core.preprocess_manage import collect_preprocess_config, set_preprocess_params, DatasetLoader
 
 
 # pylint: disable=invalid-name
+LOG = 25
 logger = logging.getLogger("HHB")
 
 
+def save_quantized_model(mod, output_dir="."):
+    """Save quantized model into file.
+
+    Parameters
+    ----------
+    mod : tvm.IRModule
+        The qnn module for compilation
+    output_dir : str
+        The output directory holding file.
+    """
+    mod_path = os.path.join(output_dir, "qnn.txt")
+
+    with open(mod_path, "w") as f:
+        f.write(mod.astext())
+
+
+def hhb_quantize(relay_ir: HHBRelayIR, config, calibrate_data=None, save_to_dir=None) -> HHBQNNIR:
+    """Quantize model and convert relay ir into qnn ir.
+
+    Parameters
+    ----------
+    relay_ir : HHBRelayIR
+        Relay ir wrapper that holds module and params
+    config : Config
+        All config for HHB
+    calibrate_data : List[Dict[str, numpy.ndarray]]
+        The calibration data for quantization. It includes batches of data.
+    save_to_dir : str, optional
+        save model into specified directory
+
+    Returns
+    -------
+    relay_ir : HHBQNNIR
+        Qnn ir wrapper that holds module and params
+    """
+    mod, params = relay_ir.get_model()
+    hhb_config = config._cmd_config
+    inter_hhb_config = get_config_dict(hhb_config)
+    inter_hhb_config["target"] = hhb_config.board
+    inter_hhb_config["params_path"] = os.path.join(inter_hhb_config["params_path"], "qnn.params")
+
+    qnn_ir = HHBQNNIR()
+    qnn_ir._curr_mod = quantize_model(
+        mod, params, inter_hhb_config, calibrate_data, hhb_config.board
+    )
+
+    # update auto-qaunt layers
+    if inter_hhb_config["auto_hybrid_quantization"]:
+        update_hybrid_layer(hhb_config.quantize_config, hhb_config.output)
+
+        limited_layer = ignore_layers_from_auto_quant(qnn_ir._curr_mod, hhb_config.board)
+        logger.info(
+            "These layers will be removed from hybrid quant list: {}".format(
+                set(hhb_config.quantize_config["hybrid_layer_name"]) & set(limited_layer)
+            )
+        )
+        hhb_config.quantize_config["hybrid_layer_name"] = list(
+            set(hhb_config.quantize_config["hybrid_layer_name"]) - set(limited_layer)
+        )
+
+        if hhb_config.quantize_config.ignore_hybrid_layer:
+            hhb_config.quantize_config["hybrid_layer_name"] = list(
+                set(hhb_config.quantize_config["hybrid_layer_name"])
+                - set(hhb_config.quantize_config.ignore_hybrid_layer)
+            )
+
+    if save_to_dir is not None:
+        save_to_dir = ensure_dir(save_to_dir)
+        save_quantized_model(qnn_ir._curr_mod, save_to_dir)
+
+    return qnn_ir
+
+
 @hhb_register_parse
 def add_quantize_parser(subparsers):
-    """ Include parser for 'quantize' subcommand """
+    """Include parser for 'quantize' subcommand"""
 
     parser = subparsers.add_parser("quantize", help="Quantize the imported model")
     parser.set_defaults(func=driver_quantize)
 
     add_preprocess_argument(parser)
     add_quantize_argument(parser)
     add_hardware_argument(parser)
     add_optimize_argument(parser)
     add_codegen_argument(parser)
     add_common_argument(parser)
 
-    parser.add_argument(
-        "-o",
-        "--output",
-        metavar="",
-        default="hhb_out",
-        help="The directory that holds the quantized relay ir.",
-    )
     parser.add_argument("-v", "--verbose", action="count", default=0, help="Increase verbosity")
     parser.add_argument("FILE", help="Directory to the model file")
 
     ALL_ARGUMENTS_DESC["quantize"] = collect_arguments_info(parser._actions)
 
 
 def driver_quantize(args_filter: ArgumentFilter):
     """Driver quantize command"""
     args = args_filter.filtered_args
+    if args.board == "th1520" and (args.hybrid_computing or args.auto_hybrid_quantization):
+        args.board = "hth1520"
     if not os.path.exists(args.FILE) or not os.path.isdir(args.FILE):
         raise HHBException("The directory is not exists: {}".format(args.FILE))
     relay_ir = HHBRelayIR()
     relay_ir.load_model(args.FILE)
     input_mod, input_params = relay_ir.get_model()
     input_name_list, input_shape_list, _ = get_input_info_from_relay(input_mod, input_params)
     output_shape_list, _ = get_output_info_from_relay(input_mod, input_params)
 
+    detected_quant_type = detect_quantized_model(input_mod)
+    if detected_quant_type:
+        if len(detected_quant_type) == 1:
+            detected_quant_type = detected_quant_type.pop()
+            if detected_quant_type == "uint8":
+                args.quantization_scheme = "uint8_asym"
+            elif detected_quant_type == "int8":
+                args.quantization_scheme = "int8_asym"
+            else:
+                raise HHBException("Unsupport quantization type:{}.\n".format(detected_quant_type))
+            logger.log(
+                LOG,
+                "Detect that current model has been quantized with {}, "
+                "--quantization-scheme will be overwritten to {}".format(
+                    detected_quant_type, args.quantization_scheme
+                ),
+            )
+        else:
+            logger.warning("Detect that there are multi quantization types in model.")
+
     # filter arguments and prepare all needed args
     all_filters = [
         collect_preprocess_config,
         set_preprocess_params,
         collect_quantization_config,
         set_quantize_params_by_board,
         collect_codegen_config,
@@ -114,23 +208,20 @@
     extra_args.output_num = len(output_shape_list)
     extra_args.model_save = "save_and_run"  # default value
     args_filter.filter_argument(all_filters, extra=extra_args)
     args = args_filter.filtered_args
 
     # add preprocess node into mod
     if args.preprocess_config.add_preprocess_node:
-        from tvm.relay.quantize.quantize_hhb import _bind_params
-        from tvm.relay import transform
-
-        if input_params:
-            input_mod["main"] = _bind_params(input_mod["main"], input_params)
-            input_params = None
-        input_mod = transform.AddPreprocessNode(
-            args.preprocess_config.data_mean, args.preprocess_config.data_scale
-        )(input_mod)
+        input_mod, input_params = insert_preprocess_node(
+            input_mod,
+            input_params,
+            args.preprocess_config.data_mean,
+            args.preprocess_config.data_scale,
+        )
         logger.debug("Insert preprocess node into model successfully!")
 
     # get calibrate dataset
     dataset_list = []
     if args.calibrate_dataset:
         logger.info("get calibrate dataset from %s", args.calibrate_dataset)
         dl = DatasetLoader(
```

## hhb/simulate.py

```diff
@@ -24,115 +24,219 @@
 import os
 import yaml
 
 import numpy as np
 
 import tvm
 from tvm import runtime
-from tvm.contrib import graph_runtime
+from tvm.contrib import graph_executor
 
-from core.arguments_manage import (
+from .core.arguments_manage import (
     add_simulate_argument,
     add_common_argument,
     add_postprocess_argument,
     add_preprocess_argument,
+    add_codegen_argument,
+    add_optimize_argument,
     ArgumentFilter,
 )
-from core.common import (
+from .core.common import (
     hhb_register_parse,
     HHBException,
     ensure_dir,
     AttributeDict,
     print_top5,
     generate_config_file,
     ALL_ARGUMENTS_DESC,
     collect_arguments_info,
 )
-from core.hhbir_manage import (
+from .core.hhbir_manage import (
     guess_ir_type,
     HHBIRType,
     HHBRelayIR,
     HHBQNNIR,
     HHBFloatCodegenIR,
     HHBX86QnnCodegenIR,
 )
-from core.preprocess_manage import collect_preprocess_config, set_preprocess_params, DatasetLoader
-from core.simulate_manage import inference_model
+from .core.preprocess_manage import collect_preprocess_config, set_preprocess_params, DatasetLoader
+from .core.simulate_manage import inference_model
+from .core.codegen_manage import collect_codegen_config
+from .core.frontend_manage import insert_preprocess_node
 
 # pylint: disable=invalid-name
 logger = logging.getLogger("HHB")
 
 
+def hhb_runner(codegen_ir, config):
+    """Wrapper for hhb runner.
+
+    Parameters
+    ----------
+    codegen_ir : HHBFloatCodegenIR or HHBX86QnnCodegenIR
+        The codegened model.
+    config : Config
+        All config for HHB
+
+    Returns
+    -------
+    ret : GraphModule
+        The object that can be executed for x86_ref
+
+    """
+    hhb_config = config._cmd_config
+    ctx = tvm.cpu(0)
+    if isinstance(codegen_ir, HHBFloatCodegenIR):
+        m = graph_executor.GraphModule(codegen_ir.get_model()["default"](ctx))
+    elif isinstance(codegen_ir, HHBX86QnnCodegenIR):
+        factory = codegen_ir.get_factory()
+        lib = codegen_ir.get_lib(hhb_config.output)
+        m = tvm.contrib.graph_executor.create(factory.get_graph_json(), lib, tvm.cpu(0))
+        m.load_params(tvm.runtime.save_param_dict(factory.get_params()))
+    else:
+        raise HHBException("Can not create runner for {}".format(type(codegen_ir)))
+
+    return m
+
+
+def hhb_inference(graph_module, dataset):
+    """Inference for hhb model.
+
+    Parameters
+    ----------
+    graph_module : GraphModule
+        The object that can be executed for x86_ref
+    dataset : Dict[str, numpy.ndarray]
+        The input data
+
+    Returns
+    -------
+    output : List[numpy.ndarray]
+        The output data.
+    """
+    graph_module.run(**dataset)
+    output = []
+    for i in range(graph_module.get_num_outputs()):
+        out = graph_module.get_output(i).numpy()
+        output.append(out)
+    return output
+
+
 @hhb_register_parse
 def add_simulate_parser(subparsers):
-    """ Include parser for 'simulate' subcommand """
+    """Include parser for 'simulate' subcommand"""
 
     parser = subparsers.add_parser("simulate", help="Simulate the imported model")
     parser.set_defaults(func=driver_simulate)
 
     add_simulate_argument(parser)
     add_preprocess_argument(parser)
     add_postprocess_argument(parser)
+    add_optimize_argument(parser)
+    add_codegen_argument(parser)
     add_common_argument(parser)
 
     parser.add_argument("-v", "--verbose", action="count", default=0, help="Increase verbosity")
-    parser.add_argument(
-        "-o",
-        "--output",
-        default="hhb_out",
-        help="The directory that holds the result files.",
-    )
     parser.add_argument("FILE", help="Directory to the model file")
 
     ALL_ARGUMENTS_DESC["simulate"] = collect_arguments_info(parser._actions)
 
 
 def driver_simulate(args_filter: ArgumentFilter):
     """Driver simulate command"""
     args = args_filter.filtered_args
     if not os.path.exists(args.FILE) or not os.path.isdir(args.FILE):
         raise HHBException("The directory is not exists: {}\n".format(args.FILE))
     model_type = guess_ir_type(args.FILE)
     logger.debug("Infer the ir type: %s in %s" % (HHBIRType.TYPE2NAME[model_type], args.FILE))
 
+    args.output = ensure_dir(args.output)
+
+    x86_codegen_ir = None
+    quantize_config = None
+    if args.board == "x86_ref":
+        if model_type == HHBIRType.RELAY:
+            # get relay ir
+            relay_ir = HHBRelayIR()
+            relay_ir.load_model(args.FILE)
+            input_module = relay_ir.get_model()
+
+            # add preprocess node into mod
+            all_filters = [
+                collect_preprocess_config,
+            ]
+            args_filter.filter_argument(all_filters)
+            args = args_filter.filtered_args
+            if args.preprocess_config.add_preprocess_node:
+                input_mod, input_params = insert_preprocess_node(
+                    input_module[0],
+                    input_module[1],
+                    args.preprocess_config.data_mean,
+                    args.preprocess_config.data_scale,
+                )
+                input_module = (input_mod, input_params)
+                logger.debug("Insert preprocess node into model successfully!")
+
+            # convert to float codegen ir
+            float_codegen_ir = HHBFloatCodegenIR()
+            float_codegen_ir.convert(input_module, args.board, args.opt_level)
+            float_codegen_ir.save_model(args.output)
+            x86_codegen_ir = float_codegen_ir
+        elif model_type == HHBIRType.QNN:
+            # get qnn ir
+            qnn_ir = HHBQNNIR()
+            qnn_ir.load_model(args.FILE)
+            input_module = qnn_ir.get_model()
+            # convert to x86 qnn codegen ir
+            x86_qnn_codegen_ir = HHBX86QnnCodegenIR()
+            quantize_config = x86_qnn_codegen_ir.get_quant_env(
+                os.path.join(args.FILE, qnn_ir.info_file)
+            )
+            x86_qnn_codegen_ir.convert(
+                input_module, args.board, args.opt_level, args.output, quantize_config
+            )
+            x86_qnn_codegen_ir.save_model(args.output)
+            x86_codegen_ir = x86_qnn_codegen_ir
+        else:
+            raise HHBException("unsupport for IR type: {}".format(HHBIRType.TYPE2NAME[model_type]))
+    else:
+        raise HHBException("Only x86_ref support for simulation!")
+
+    if not args.simulate_data:
+        raise HHBException("Please set simulate data by --simulate-data.\n")
+
+    logger.info("get simulate data from %s", args.simulate_data)
+
+    ctx = tvm.cpu(0)
+    if model_type == HHBIRType.RELAY:
+        m = graph_executor.GraphModule(x86_codegen_ir.get_model()["default"](ctx))
+    else:
+        factory = x86_codegen_ir.get_factory()
+        lib = x86_codegen_ir.get_lib(args.output)
+        m = tvm.contrib.graph_executor.create(factory.get_graph_json(), lib, tvm.cpu(0))
+        m.load_params(tvm.runtime.save_param_dict(factory.get_params()))
+
     # filter arguments and prepare all needed args
     all_filters = [
         collect_preprocess_config,
         set_preprocess_params,
+        collect_codegen_config,
     ]
     extra_args = AttributeDict()
-
-    codegen_ir = None
-    curr_module = None
-    if model_type == HHBIRType.FLOAT_CODEGEN:
-        codegen_ir = HHBFloatCodegenIR()
-    elif model_type == HHBIRType.X86_QNN_CODEGEN:
-        codegen_ir = HHBX86QnnCodegenIR()
-    else:
-        raise HHBException(
-            "{} IR don't support for simulation.".format(HHBIRType.TYPE2NAME[model_type])
-        )
-
-    codegen_ir.load_model(args.FILE)
-    curr_module = codegen_ir.get_model()
-    info_dict = codegen_ir.info_dict
-
-    extra_args.input_shape = info_dict["input_shape_list"]
+    extra_args.input_shape = x86_codegen_ir.info_dict["input_shape_list"]
     args_filter.filter_argument(all_filters, extra=extra_args)
     args = args_filter.filtered_args
 
-    if not args.simulate_data:
-        raise HHBException("Please set simulate data by --simulate-data")
-
-    logger.info("get simulate data from %s", args.simulate_data)
+    target_layout = "NCHW"
+    if quantize_config:
+        target_layout = quantize_config["layout"]
     dl = DatasetLoader(
         args.simulate_data,
         args.preprocess_config,
-        info_dict["input_shape_list"],
-        info_dict["input_name_list"],
+        x86_codegen_ir.info_dict["input_shape_list"],
+        x86_codegen_ir.info_dict["input_name_list"],
+        target_layout=target_layout,
     )
-
-    inference_model(curr_module, dl, args.postprocess, args.output)
+    inference_model(m, dl, args.postprocess, args.output)
 
     if args.generate_config:
         args.output = ensure_dir(args.output)
         generate_config_file(os.path.join(args.output, "cmd_simulate_params.yml"))
```

## hhb/config/anole.tp

```diff
@@ -13,15 +13,15 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
-/* auto generate by HHB_VERSION "2.0.20" */
+/* auto generate by HHB_VERSION "2.2.35" */
 
 #_hhb_header_files_#
 
 #_hhb_macro_def_#
 
 #_hhb_function_decl_#
 
@@ -74,33 +74,38 @@
             data_path = argv + 2;
             input_group_num = (argc - 2) / input_num;
         }
     }
 
     void *sess = create_graph(argv[1]);
 
+    struct csinn_tensor* input_tensors[input_num];
+    #_tensor_shape_#
     float *inputf[input_num];
-    uint8_t *input[input_num];
     char filename_prefix[FILE_LENGTH] = {0};
     for (i = 0; i < input_group_num; i++) {
         /* set input */
         for (int j = 0; j < input_num; j++) {
             #_get_input_data_stats_#
-            input[j] = shl_ovx_input_f32_to_u8(j, inputf[j], sess);
+            input_tensors[j]->data = shl_ovx_input_f32_to_u8(j, inputf[j], sess);
         }
 
-        csinn_run(#_anole_value_pass# sess);
+        csinn_update_input_and_run(input_tensors, sess);
 
         snprintf(filename_prefix, FILE_LENGTH, "%s", basename(data_path[i * input_num]));
         postprocess(sess, filename_prefix);
 
         for (int j = 0; j < input_num; j++) {
             shl_mem_free(inputf[j]);
-            shl_mem_free(input[j]);
+            shl_mem_free(input_tensors[j]->data);
         }
     }
 
+    for (int j = 0; j < input_num; j++) {
+        csinn_free_tensor(input_tensors[j]);
+    }
+
     csinn_session_deinit(sess);
     csinn_free_session(sess);
 
     return 0;
 }
```

## hhb/config/anole_multithread.tp

```diff
@@ -13,15 +13,15 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
-/* auto generate by HHB_VERSION "2.0.20" */
+/* auto generate by HHB_VERSION "2.2.35" */
 
 #_hhb_header_files_#
 #include <pthread.h>
 
 #_hhb_macro_def_#
 
 struct thread_args {
@@ -104,50 +104,56 @@
 
     initNum ++;
     while(1) {
         sleep(1);
         if(initNum == deviceCount) break;
     }
 
+    struct csinn_tensor* input_tensors[input_num];
+    #_tensor_shape_#
     float *inputf[input_num];
     uint8_t *input[input_num];
     char filename_prefix[FILE_LENGTH] = {0};
 
     float thread_total_time = 0;
     uint64_t start_time, end_time;
     loop_time = input_group_num;
     for (i = 0; i < input_group_num; i++) {
         /* set input */
         printf("%d-th thread, %d-th input:\n", device_index, i);
         for (int j = 0; j < input_num; j++) {
             #_get_input_data_stats_#
-            input[j] = shl_ovx_input_f32_to_u8(j, inputf[j], sess);
+            input_tensors[j]->data = shl_ovx_input_f32_to_u8(j, inputf[j], sess);
         }
 
         start_time = shl_get_timespec();
-        csinn_run(#_anole_value_pass# sess);
+        csinn_update_input_and_run(input_tensors, sess);
         end_time = shl_get_timespec();
 
         thread_total_time += (((float)(end_time - start_time)) / 1000000);
         total_time += (((float)(end_time - start_time)) / 1000000);
 
         snprintf(filename_prefix, FILE_LENGTH, "%s", basename(data_path[i * input_num]));
         postprocess(sess, filename_prefix);
 
         for (int j = 0; j < input_num; j++) {
             shl_mem_free(inputf[j]);
-            shl_mem_free(input[j]);
+            shl_mem_free(input_tensors[j]->data);
         }
     }
 
     printf("%d-th thread run graph average execution time: %.5fms, FPS=%.2f\n", device_index, thread_total_time / input_group_num,
                     1000.0/(thread_total_time / input_group_num));
 
     total_fps += 1000.0/(thread_total_time / input_group_num);
 
+    for (int j = 0; j < input_num; j++) {
+        csinn_free_tensor(input_tensors[j]);
+    }
+
     csinn_session_deinit(sess);
     csinn_free_session(sess);
 }
 
 int main(int argc, char **argv) {
     int i=0;
     struct thread_args targs[8];
```

## hhb/config/c906.tp

```diff
@@ -13,15 +13,15 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
-/* auto generate by HHB_VERSION "2.0.20" */
+/* auto generate by HHB_VERSION "2.2.35" */
 
 #_hhb_header_files_#
 
 #_hhb_macro_def_#
 
 #_hhb_function_decl_#
 
@@ -43,15 +43,20 @@
     if (strcmp(suffix, ".params") == 0) {
         // create general graph
         return csinn_(params);
     }
 
     suffix = params_path + (strlen(params_path) - 3);
     if (strcmp(suffix, ".bm") == 0) {
-        return csinn_(params + 8192);
+        struct shl_bm_sections *section = (struct shl_bm_sections *)(params + 4128);
+        if (section->graph_offset) {
+            return csinn_import_binary_model(params);
+        } else {
+            return csinn_(params + section->params_offset * 4096);
+        }
     } else {
         return NULL;
     }
 }
 
 int main(int argc, char **argv) {
     char **data_path = NULL;
@@ -70,41 +75,48 @@
             input_group_num /= input_num;
         } else {
             data_path = argv + 2;
             input_group_num = (argc - 2) / input_num;
         }
     }
 
+    #_hhb_gen_register_#
+
     void *sess = create_graph(argv[1]);
 
-    uint8_t *input[input_num];
+    struct csinn_tensor* input_tensors[input_num];
+    #_tensor_shape_#
     float *inputf[input_num];
     char filename_prefix[FILE_LENGTH] = {0};
     uint64_t start_time, end_time;
     for (i = 0; i < input_group_num; i++) {
         /* set input */
         for (int j = 0; j < input_num; j++) {
             #_get_input_data_stats_#
-            input[j] = shl_ref_f32_to_input_dtype(j, inputf[j], sess);
+            input_tensors[j]->data = shl_ref_f32_to_input_dtype(j, inputf[j], sess);
         }
 
         start_time = shl_get_timespec();
-        csinn_run(#_anole_value_pass# sess);
+        csinn_update_input_and_run(input_tensors, sess);
         end_time = shl_get_timespec();
         printf("Run graph execution time: %.5fms, FPS=%.2f\n", ((float)(end_time-start_time))/1000000,
                     1000000000.0/((float)(end_time-start_time)));
 
         snprintf(filename_prefix, FILE_LENGTH, "%s", basename(data_path[i * input_num]));
         postprocess(sess, filename_prefix);
 
         for (int j = 0; j < input_num; j++) {
             shl_mem_free(inputf[j]);
-            shl_mem_free(input[j]);
+            shl_mem_free(input_tensors[j]->data);
         }
     }
 
+    for (int j = 0; j < input_num; j++) {
+        csinn_free_tensor(input_tensors[j]);
+    }
+
     csinn_session_deinit(sess);
     csinn_free_session(sess);
 
     return 0;
 }
```

## hhb/config/thead.tp

```diff
@@ -13,15 +13,15 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
-/* auto generate by HHB_VERSION "2.0.20" */
+/* auto generate by HHB_VERSION "2.2.35" */
 
 #include <stdlib.h>
 #include <stdio.h>
 #include <string.h>
 #include <stdint.h>
 #include "io.h"
```

## hhb/config/process/include/io.h

```diff
@@ -13,15 +13,15 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
-/* auto generate by HHB_VERSION "2.0.20" */
+/* auto generate by HHB_VERSION "2.2.35" */
 
 #ifndef HHB_IO_H_
 #define HHB_IO_H_
 
 #include <math.h>
 #include <stdint.h>
 #include <stdio.h>
```

## hhb/config/process/include/process.h

```diff
@@ -13,15 +13,15 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
-/* auto generate by HHB_VERSION "2.0.20" */
+/* auto generate by HHB_VERSION "2.2.35" */
 
 #ifndef PROCESS_H_
 #define PROCESS_H_
 
 #include <math.h>
 #include <stdint.h>
 #include <stdio.h>
```

## hhb/config/process/src/io.c

```diff
@@ -13,15 +13,15 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
-/* auto generate by HHB_VERSION "2.0.20" */
+/* auto generate by HHB_VERSION "2.2.35" */
 
 #include "io.h"
 
 /******************************************************************************
  *                                                                            *
  *                      Utils for process data                                *
  *                                                                            *
```

## hhb/config/process/src/process.c

```diff
@@ -13,15 +13,15 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
-/* auto generate by HHB_VERSION "2.0.20" */
+/* auto generate by HHB_VERSION "2.2.35" */
 
 #include "process.h"
 
 #include "io.h"
 #include "jpeglib.h"
 #include "png.h"
 #include "zlib.h"
```

## hhb/config/template/function_decl.tp

```diff
@@ -1,2 +1,2 @@
 void *csinn_(char *params);
-void csinn_run(#_csinn_args# void *td);
+void csinn_update_input_and_run(struct csinn_tensor **input_tensors , void *sess);
```

## hhb/config/template/postprocess_def.tp

```diff
@@ -21,8 +21,10 @@
         print_tensor_info(output);
 
         #_convert_fouput_#
         #_show_top5_stats_#
         #_save_output_stats_#
         #_free_output_data_#
     }
+    csinn_free_tensor(input);
+    csinn_free_tensor(output);
 }
```

## hhb/core/arguments_manage.py

```diff
@@ -11,20 +11,22 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Manage command line arguments."""
-from collections import OrderedDict
-from email.policy import default
+from collections import OrderedDict, namedtuple
+from email.mime import base
+from inspect import ArgSpec
 import os
-from random import choices
 import sys
 import argparse
+import copy
+import json
 
 import yaml
 
 from .common import (
     HHBException,
     HHB_REGISTERED_PARSER,
     hhb_version,
@@ -33,696 +35,1141 @@
     argument_filter_helper,
     ALL_ARGUMENTS_DESC,
     generate_readme_file,
     find_index,
     hhb_exit,
     ARGS_DEST_TO_OPTIONS_STRING,
     ALL_ARGUMENTS_INFO,
+    collect_arguments_info,
 )
 
+from .preprocess_manage import collect_preprocess_config, set_preprocess_params
+from .quantization_manage import (
+    collect_quantization_config,
+    get_config_dict,
+    set_quantize_params_by_board,
+)
+from .codegen_manage import collect_codegen_config, set_codegen_config
+from .hhbir_manage import get_input_info_from_relay, get_output_info_from_relay
+
 
 ALL_SUBCOMMAND = ["import", "quantize", "codegen", "simulate", "benchmark", "profiler"]
 HIDDEN_SUBCOMMAND = ["benchmark"]
 
 
 def boolean_string(s):
     if s not in {"False", "True"}:
         raise ValueError("Not a valid boolean string")
     return s == "True"
 
 
-@get_parameters_info("common")
-def add_common_argument(parser):
-    parser.add_argument(
-        "--config-file",
-        type=str,
+ArgSpec = namedtuple(
+    "ArgSpec",
+    [
+        "name",
+        "abbr_name",
+        "type",
+        "default",
+        "choices",
+        "action",
+        "nargs",
+        "help",
+        "hidden",
+        "version",
+    ],
+)
+
+
+class ArgSpecHelper(object):
+    def __init__(
+        self,
+        name,
+        abbr_name=None,
+        type=None,
         default=None,
-        metavar="",
-        help="Configue more complex parameters for executing the model.",
-    )
-    parser.add_argument("--generate-config", action="store_true", help="Generate  config file")
+        choices=None,
+        action=None,
+        nargs=None,
+        help=None,
+        hidden=False,
+        version=None,
+    ) -> None:
+        self.spec = ArgSpec(
+            name=name,
+            abbr_name=abbr_name,
+            type=type,
+            default=default,
+            choices=choices,
+            action=action,
+            nargs=nargs,
+            help=help,
+            hidden=hidden,
+            version=version,
+        )
+        if action == "store_true" and default is None:
+            self.value = False
+        else:
+            self.value = default
 
+    def show_help(self):
+        """Show help string."""
+        return self.spec.help
+
+
+class ArgumentsBase(object):
+    def __init__(self) -> None:
+        self._exclusive_group = []
+
+    @property
+    def name(self):
+        return "argument_base"
+
+    def add_exclusive_group(self, *args):
+        self._exclusive_group.append(args)
+
+    def _get_actual_args(self, arg_spec: ArgSpec):
+        position_args = []
+        if arg_spec.abbr_name is not None:
+            position_args.append(arg_spec.abbr_name)
+        position_args.append(arg_spec.name)
+
+        keyword_args = {}
+        if arg_spec.type is not None:
+            keyword_args["type"] = arg_spec.type
+        if arg_spec.default is not None:
+            keyword_args["default"] = arg_spec.default
+        if arg_spec.choices is not None:
+            keyword_args["choices"] = arg_spec.choices
+        if arg_spec.action is not None:
+            keyword_args["action"] = arg_spec.action
+        if arg_spec.nargs is not None:
+            keyword_args["nargs"] = arg_spec.nargs
+        if not arg_spec.hidden:
+            if arg_spec.help is not None:
+                keyword_args["help"] = arg_spec.help
+        else:
+            keyword_args["help"] = argparse.SUPPRESS
+        if arg_spec.version is not None:
+            keyword_args["version"] = arg_spec.version
+
+        return position_args, keyword_args
+
+    def set_parser(self, parser: argparse.ArgumentParser):
+        # set exclusive group args
+        for group in self._exclusive_group:
+            group_arg = parser.add_mutually_exclusive_group()
+
+            for g in group:
+                if not isinstance(g, ArgSpecHelper):
+                    raise HHBException("Only ArgSpecHelpr obj can be put into exclusive group.")
+                p_args, k_args = self._get_actual_args(g.spec)
+                group_arg.add_argument(*p_args, **k_args)
+
+        # set other normal args
+        unroll_group = []
+        for group in self._exclusive_group:
+            unroll_group.extend(group)
+        for arg in self.__dict__.values():
+            if not isinstance(arg, ArgSpecHelper):
+                continue
+            if arg in unroll_group:
+                continue
+
+            p_args, k_args = self._get_actual_args(arg.spec)
+            parser.add_argument(*p_args, **k_args)
+
+    def get_option_string_to_argument(self):
+        """Get {(abbr_name, name): argument} dict."""
+        res = {}
+        for arg in self.__dict__.values():
+            if not isinstance(arg, ArgSpecHelper):
+                continue
+            if arg.spec.abbr_name:
+                res[(arg.spec.abbr_name, arg.spec.name)] = arg
+            else:
+                res[(arg.spec.name,)] = arg
+        return res
 
-@get_parameters_info("preprocess")
+    def __str__(self) -> str:
+        res = {}
+        for key, arg in self.__dict__.items():
+            if not isinstance(arg, ArgSpecHelper):
+                continue
+
+            res[key] = arg.value
+
+        return str(res)
+
+
+class CommonArguments(ArgumentsBase):
+    def __init__(self) -> None:
+        super(CommonArguments, self).__init__()
+
+        self.config_file = ArgSpecHelper(
+            name="--config-file",
+            type=str,
+            default=None,
+            help="Configue more complex parameters for executing the model.",
+        )
+        self.generate_config = ArgSpecHelper(
+            name="--generate-config", action="store_true", help="Generate  config file"
+        )
+        self.output = ArgSpecHelper(
+            name="--output",
+            abbr_name="-o",
+            default="hhb_out",
+            help="The directory that holds the outputs.",
+        )
+
+    @property
+    def name(self):
+        return "common"
+
+
+class ImportArguments(ArgumentsBase):
+    def __init__(self) -> None:
+        super(ImportArguments, self).__init__()
+        self.input_name = ArgSpecHelper(
+            name="--input-name",
+            abbr_name="-in",
+            type=str,
+            default=None,
+            help="Set the name of input node. If '--input-name'is None, "
+            "default value is 'Placeholder'. Multiple values "
+            "are separated by semicolon(;).",
+        )
+        self.input_shape = ArgSpecHelper(
+            name="--input-shape",
+            abbr_name="-is",
+            type=str,
+            default=None,
+            help="Set the shape of input nodes. Multiple shapes are separated "
+            "by semicolon(;) and the dims between shape are separated "
+            "by space.",
+        )
+        self.output_name = ArgSpecHelper(
+            name="--output-name",
+            abbr_name="-on",
+            type=str,
+            help="Set the name of output nodes. Multiple shapes are " "separated by semicolon(;).",
+        )
+
+        from .frontend_manage import get_frontend_names
+
+        self.model_format = ArgSpecHelper(
+            name="--model-format",
+            choices=get_frontend_names(),
+            help="Specify input model format:{}".format(get_frontend_names()),
+        )
+        self.reorder_pixel_format = ArgSpecHelper(
+            name="--reorder-pixel-format",
+            action="store_true",
+            help="If original model's input data pixel format is rgb, then covert it to bgr;"
+            "otherwise, then convert it to rgb.",
+        )
+
+    @property
+    def name(self):
+        return "import"
+
+
+class OptimizeArguments(ArgumentsBase):
+    def __init__(self) -> None:
+        super(OptimizeArguments, self).__init__()
+        self.board = ArgSpecHelper(
+            name="--board",
+            default="unset",
+            choices=[
+                "anole",
+                "th1520",
+                "e907",
+                "c906",
+                "c908",
+                "c920",
+                "rvm",
+                "x86_ref",
+                "unset",
+            ],
+            help="Set target device, default is anole.",
+        )
+        self.opt_level = ArgSpecHelper(
+            name="--opt-level",
+            choices=[-1, 0, 1, 2, 3],
+            default=3,
+            type=int,
+            help="Specify the optimization level, default is 3.",
+            hidden=True,
+        )
+        self.hybrid_computing = ArgSpecHelper(
+            name="--hybrid-computing",
+            action="store_true",
+            help="Supports hybrid computing on multiple devices. Currently supports "
+            "CPU and NPU for th1520.",
+        )
+        self.link_lib = ArgSpecHelper(
+            name="--link-lib",
+            default="unset",
+            choices=[
+                "shl_pnna",
+                "shl_th1520",
+                "shl_c906",
+                "shl_c908",
+                "shl_c920",
+                "shl_rvm",
+                "unset",
+            ],
+            help="Set link library for -D. default is unset",
+        )
+
+    @property
+    def name(self):
+        return "optimize"
+
+
+class QuantizeArguments(ArgumentsBase):
+    def __init__(self) -> None:
+        super(QuantizeArguments, self).__init__()
+
+        self.calibrate_dataset = ArgSpecHelper(
+            name="--calibrate-dataset",
+            abbr_name="-cd",
+            type=str,
+            help="Provide with dataset for the input of model in reference step. "
+            "Support dir or .npz .jpg .png .JPEG or .txt in which there are path "
+            "of images. Note: only one image path in one line if .txt.",
+        )
+        self.quantization_scheme = ArgSpecHelper(
+            name="--quantization-scheme",
+            choices=[
+                "int4_asym_w_sym",
+                "uint8_asym",
+                "int8_asym",
+                "int8_sym",
+                "int8_original",
+                "int8_asym_w_sym",
+                "int16_sym",
+                "float16",
+                "float16_w_int8",
+                "bfloat16",
+                "float32",
+                "unset",
+            ],
+            default="unset",
+            help="Scheme of quantization. default is unset, and select scheme by --board.",
+        )
+        self.auto_hybrid_quantization = ArgSpecHelper(
+            name="--auto-hybrid-quantization",
+            action="store_true",
+            help="If set, quantize model automatically.",
+        )
+        self.quantization_loss_algorithm = ArgSpecHelper(
+            name="--quantization-loss-algorithm",
+            type=str,
+            choices=["cos_similarity", "mse", "kl_divergence", "cross_entropy", "gini"],
+            default="cos_similarity",
+            help="How to calculate accuracy loss for every layer.",
+        )
+        self.quantization_loss_threshold = ArgSpecHelper(
+            name="--quantization-loss-threshold",
+            type=float,
+            default=0.99,
+            help="The threshold that will determin thich layer will be quantized with hybrid way."
+            "If it is None, we will select threshold automatically.",
+        )
+        self.dump_quantization_loss = ArgSpecHelper(
+            name="--dump-quantization-loss",
+            action="store_true",
+            help="If set, dump quantizaiton loss into file.",
+        )
+        self.loss_threshold_type = ArgSpecHelper(
+            name="--loss-threshold-type",
+            type=str,
+            choices=["min", "max", "avg"],
+            default="avg",
+            help="The threshold type for quantizaiton loss, default is avg.",
+            hidden=True,
+        )
+        self.from_quant_file = ArgSpecHelper(
+            name="--from-quant-file",
+            action="store_true",
+            help="If set, get hybrid quantization infomation from model.quant.json",
+            hidden=True,
+        )
+        self.ignore_hybrid_layer = ArgSpecHelper(
+            name="--ignore-hybrid-layer",
+            type=str,
+            nargs="+",
+            help="Ignore layers to be hybrid layers.",
+            hidden=True,
+        )
+        self.hybrid_quantization_scheme = ArgSpecHelper(
+            name="--hybrid-quantization-scheme",
+            choices=[
+                "int4_asym_w_sym",
+                "uint8_asym",
+                "int8_asym",
+                "int8_sym",
+                "int8_original",
+                "int8_asym_w_sym",
+                "int16_sym",
+                "float16",
+                "bfloat16",
+                "float32",
+                "unset",
+            ],
+            default="unset",
+            help="Scheme of hybrid quantization. default is unset.",
+        )
+        self.hybrid_layer_name = ArgSpecHelper(
+            name="--hybrid-layer-name",
+            type=str,
+            nargs="+",
+            help="Layer buffer name to use hybrid quantization.",
+        )
+        self.num_bit_activation = ArgSpecHelper(
+            name="--num-bit-activation",
+            type=int,
+            choices=[0, 16, 32],
+            default=0,
+            help="The bit number that quantizes activation layer. default is 0, means unset.",
+            hidden=True,
+        )
+        self.num_bit_input = ArgSpecHelper(
+            name="--num-bit-input",
+            type=int,
+            choices=[0, 8, 16, 32],
+            default=0,
+            help="The bit number that quantizes input layer. default is 0, means unset.",
+            hidden=True,
+        )
+        self.num_bit_weight = ArgSpecHelper(
+            name="--num-bit-weight",
+            type=int,
+            choices=[0, 8, 16, 32],
+            default=0,
+            help="The bit number that quantizes weight layer. default is 0, means unset.",
+            hidden=True,
+        )
+        self.dtype_input = ArgSpecHelper(
+            name="--dtype-input",
+            choices=["float", "int", "uint", "unset"],
+            default="unset",
+            help="The dtype of quantized input layer, default is uint.",
+            hidden=True,
+        )
+        self.dtype_weight = ArgSpecHelper(
+            name="--dtype-weight",
+            choices=["float", "int", "uint", "unset"],
+            default="unset",
+            help="The dtype of quantized constant parameters, default is uint.",
+            hidden=True,
+        )
+        self.dtype_activation = ArgSpecHelper(
+            name="--dtype-activation",
+            choices=["float", "int", "uint", "unset"],
+            default="unset",
+            help="The dtype of quantized activation layer, default is uint.",
+            hidden=True,
+        )
+        self.calibrate_mode = ArgSpecHelper(
+            name="--calibrate-mode",
+            choices=["maxmin", "pow2", "kl_divergence", "kl_divergence_tsing", "scale"],
+            default="maxmin",
+            help="How to calibrate while doing quantization, default is maxmin.",
+            hidden=True,
+        )
+        self.activate_quantized_type = ArgSpecHelper(
+            name="--activate-quantized-type",
+            choices=["asym", "sym", "unset"],
+            default="unset",
+            help="Select the algorithm of quantization, default is asym.",
+            hidden=True,
+        )
+        self.weight_quantized_type = ArgSpecHelper(
+            name="--weight-quantized-type",
+            choices=["asym", "sym", "unset"],
+            default="unset",
+            help="Select the algorithm of quantization, default is asym.",
+            hidden=True,
+        )
+        self.weight_scale = ArgSpecHelper(
+            name="--weight-scale",
+            choices=["max", "power2"],
+            default="max",
+            help="Select the mothod that quantizes weight value, default is max.",
+            hidden=True,
+        )
+        self.fuse_conv_relu = ArgSpecHelper(
+            name="--fuse-conv-relu",
+            action="store_true",
+            help="Fuse the convolution and relu layer.",
+        )
+        self.fuse_reshape_dense = ArgSpecHelper(
+            name="--fuse-reshape-dense",
+            action="store_true",
+            help="Fuse the reshape and dense layer.",
+        )
+        self.channel_quantization = ArgSpecHelper(
+            name="--channel-quantization",
+            action="store_true",
+            help="Do quantizetion across channel.",
+        )
+        self.broadcast_quantization = ArgSpecHelper(
+            name="--broadcast-quantization",
+            action="store_true",
+            help="Broadcast quantization parameters for special ops.",
+        )
+        self.channel_quantization_ratio_threshold = ArgSpecHelper(
+            name="--channel-quantization-ratio-threshold",
+            type=float,
+            default=0.0,
+            help="Set optimize quantitative parameters threshold for channel quantization."
+            + "The value can be selected in range [0, 1). 0 means this pass is not be used."
+            + "0.3 is a recommended threshold if this pass is turned on.",
+            hidden=True,
+        )
+        self.fuse_clip = ArgSpecHelper(
+            name="--fuse-clip",
+            action="store_true",
+            help="Fuse clip's attr into pre layer's quantitative information. "
+            + "This flag is only valid when quantization is used.",
+        )
+        self.fuse_mul_before_conv = ArgSpecHelper(
+            name="--fuse-mul-before-conv",
+            default=True,
+            choices=[False, True],
+            type=boolean_string,
+            help="This parameter is used to merge mul before conv2d to conv2d.",
+            hidden=True,
+        )
+        self.fuse_mul_after_conv = ArgSpecHelper(
+            name="--fuse-mul-after-conv",
+            default=True,
+            choices=[False, True],
+            type=boolean_string,
+            help="This parameter is used to merge mul after conv2d to conv2d.",
+            hidden=True,
+        )
+        self.fuse_add_before_conv = ArgSpecHelper(
+            name="--fuse-add-before-conv",
+            default=True,
+            choices=[False, True],
+            type=boolean_string,
+            help="This parameter is used to merge add before conv2d to conv2d.",
+            hidden=True,
+        )
+        self.fuse_add_after_conv = ArgSpecHelper(
+            name="--fuse-add-after-conv",
+            default=True,
+            choices=[False, True],
+            type=boolean_string,
+            help="This parameter is used to merge add after conv2d to conv2d.",
+            hidden=True,
+        )
+        self.fuse_zp2bias = ArgSpecHelper(
+            name="--fuse-zp2bias",
+            action="store_true",
+            help="Merge conv2d/dense zp to bias.",
+        )
+        self.target_layout = ArgSpecHelper(
+            name="--target-layout",
+            default="NCHW",
+            choices=["NCHW", "NHWC"],
+            help="Set target layout.",
+        )
+        self.use_custom_fusion = ArgSpecHelper(
+            name="--use-custom-fusion",
+            action="store_true",
+            help="This parameter is used to use custom fusion like fuse cache_matmul and layer norm.",
+            hidden=True,
+        )
+        self.convert_to_relay = ArgSpecHelper(
+            name="--convert-to-relay",
+            action="store_true",
+            help="This parameter is used to convert quanted qnn model to relay.",
+            hidden=True,
+        )
+
+    @property
+    def name(self):
+        return "quantize"
+
+
+class HardwareArguments(ArgumentsBase):
+    def __init__(self) -> None:
+        super(HardwareArguments, self).__init__()
+
+        self.hardware_sram_size = ArgSpecHelper(
+            name="--hardware-sram-size",
+            type=str,
+            default=None,
+            help="Set the size of sram. The unit must in [m, M, KB, kb].",
+            hidden=True,
+        )
+        self.hardware_max_groups = ArgSpecHelper(
+            name="--hardware-max-groups",
+            type=int,
+            default=0,
+            help="This parameter is used to describe the maximum number of groups supported by hardware.",
+            hidden=True,
+        )
+        self.hardware_max_out_channel = ArgSpecHelper(
+            name="--hardware-max-out-channel",
+            type=int,
+            default=0,
+            help="This parameter is used to describe the maximum number of output channel supported by hardware.",
+            hidden=True,
+        )
+        self.hardware_max_kernel_size = ArgSpecHelper(
+            name="--hardware-max-kernel-size",
+            type=int,
+            default=0,
+            help="This parameter is used to describe the size of sram.",
+            hidden=True,
+        )
+        self.hardware_contain_weight = ArgSpecHelper(
+            name="--hardware-contain-weight",
+            action="store_true",
+            help="This parameter is used to describe whether the weight size should be contained when split ops.",
+            hidden=True,
+        )
+        self.hardware_alignment = ArgSpecHelper(
+            name="--hardware-alignment",
+            type=int,
+            choices=[1, 8, 16, 32],
+            default=1,
+            help="This parameter describes whether the hardware requires data alignment.",
+            hidden=True,
+        )
+        self.matrix_extension_mlen = ArgSpecHelper(
+            name="--matrix-extension-mlen",
+            default=0,
+            type=int,
+            help="Specify T-head Matrix extension's MLEN bit, default is 0, unuse matrix extension.",
+        )
+
+    @property
+    def name(self):
+        return "hardware"
+
+
+class SimulateArguments(ArgumentsBase):
+    def __init__(self) -> None:
+        super(SimulateArguments, self).__init__()
+
+        self.simulate_data = ArgSpecHelper(
+            name="--simulate-data",
+            abbr_name="-sd",
+            type=str,
+            default=None,
+            help="Provide with dataset for the input of model in reference step. "
+            "Support dir or .npz .jpg .png .JPEG or .txt in which there are path "
+            "of images. Note: only one image path in one line if .txt.",
+        )
+
+    @property
+    def name(self):
+        return "simulate"
+
+
+class PostprocessArguments(ArgumentsBase):
+    def __init__(self) -> None:
+        super(PostprocessArguments, self).__init__()
+
+        self.postprocess = ArgSpecHelper(
+            name="--postprocess",
+            type=str,
+            default="top5",
+            choices=["top5", "save", "save_and_top5"],
+            help="Set the mode of postprocess: "
+            "'top5' show top5 of output; "
+            "'save' save output to file;"
+            "'save_and_top5' show top5 and save output to file."
+            " Default is top5",
+        )
+
+    @property
+    def name(self):
+        return "postprocess"
+
+
+class PreprocessArguments(ArgumentsBase):
+    def __init__(self) -> None:
+        super(PreprocessArguments, self).__init__()
+
+        self.data_mean = ArgSpecHelper(
+            name="--data-mean",
+            abbr_name="-m",
+            type=str,
+            default="0",
+            help="Set the mean value of input, multiple values are separated by space, "
+            "default is 0.",
+        )
+        self.data_scale = ArgSpecHelper(
+            name="--data-scale",
+            abbr_name="-s",
+            type=float,
+            default=1,
+            help="Scale number(mul) for inputs normalization(data=img*scale), default is 1.",
+        )
+        self.data_scale_div = ArgSpecHelper(
+            name="--data-scale-div",
+            abbr_name="-sv",
+            type=float,
+            default=1,
+            help="Scale number(div) for inputs normalization(data=img/scale), default is 1.",
+        )
+        self.add_exclusive_group(self.data_scale, self.data_scale_div)
+        self.data_resize = ArgSpecHelper(
+            name="--data-resize",
+            abbr_name="-r",
+            type=int,
+            default=None,
+            help="Resize base size for input image to resize.",
+        )
+        self.pixel_format = ArgSpecHelper(
+            name="--pixel-format",
+            choices=["RGB", "BGR"],
+            default="RGB",
+            help="The pixel format of image data, defalut is RGB",
+        )
+        self.data_layout = ArgSpecHelper(
+            name="--data-layout",
+            choices=["NCHW", "NHWC", "CHW", "HWC", "Any"],
+            default="NCHW",
+            help='The input data layout, defalut is "NCHW"',
+            hidden=True,
+        )
+        self.add_preprocess_node = ArgSpecHelper(
+            name="--add-preprocess-node", action="store_true", help="Add preprocess node for model."
+        )
+
+    @property
+    def name(self):
+        return "preprocess"
+
+
+class CodegenArguments(ArgumentsBase):
+    def __init__(self) -> None:
+        super(CodegenArguments, self).__init__()
+
+        self.model_save = ArgSpecHelper(
+            name="--model-save",
+            choices=["run_only", "save_only", "save_and_run"],
+            default="run_only",
+            help="Whether save binary graph or run only.\n"
+            "run_only: execute model only, not save binary graph.\n"
+            "save_only: save binary graph only.\n"
+            "save_and_run: execute and save model.",
+        )
+        self.model_priority = ArgSpecHelper(
+            name="--model-priority",
+            default=0,
+            type=int,
+            help="Set model priority, only for th1520 now.\n"
+            "0 is lowest, 1 is medium, 2 is highest.",
+        )
+        self.without_preprocess = ArgSpecHelper(
+            name="--without-preprocess",
+            action="store_true",
+            help="Do not generate preprocess codes.",
+        )
+        self.multithread = ArgSpecHelper(
+            name="--multithread",
+            action="store_true",
+            help="Create multithread codes.",
+            hidden=True,
+        )
+        self.trace_strategy = ArgSpecHelper(
+            name="--trace-strategy",
+            choices=["normal", "advanced"],
+            default="normal",
+            help="Strategy to generate trace data.",
+            hidden=True,
+        )
+        self.input_memory_type = ArgSpecHelper(
+            name="--input-memory-type",
+            choices=[0, 1, 2],
+            type=int,
+            nargs="+",
+            help="Set the memory type for input tensor, support for multi-values.\n"
+            "0: allocated by CPU and not aligned;\n"
+            "1: allocated by CPU and aligned;\n"
+            "2: dma buffer.",
+        )
+        self.output_memory_type = ArgSpecHelper(
+            name="--output-memory-type",
+            choices=[0, 1, 2],
+            type=int,
+            nargs="+",
+            help="Set the memory type for output tensor, support for multi-values.\n"
+            "0: allocated by CPU and not aligned;\n"
+            "1: allocated by CPU and aligned;\n"
+            "2: dma buffer.",
+        )
+        self.memory_type = ArgSpecHelper(
+            name="--memory-type",
+            choices=[0, 1, 2],
+            type=int,
+            help="Set the memory type for input and output tensors.\n"
+            "0: allocated by CPU and not aligned;\n"
+            "1: allocated by CPU and aligned;\n"
+            "2: dma buffer.",
+        )
+        self.dynamic_cb_reg = ArgSpecHelper(
+            name="--dynamic-cb-reg",
+            action="store_true",
+            help="Emit cb_map file to reduce elf size on RTOS.",
+        )
+        self.conv2d_algorithm = ArgSpecHelper(
+            name="--conv2d-algorithm",
+            choices=["direct", "winograd", "gemm", "unset"],
+            default="unset",
+            help="The recommend algorithm for conv2d implementation, default is unset.",
+            hidden=True,
+        )
+        self.th1520_input_fix_size = ArgSpecHelper(
+            name="--th1520-input-fix-size",
+            type=str,
+            default="0",
+            help="Set input stride.",
+            hidden=True,
+        )
+        self.ahead_of_time = ArgSpecHelper(
+            name="--ahead-of-time",
+            choices=["intrinsic", "unset"],
+            default="unset",
+            help="AOT to generate intrinsic.",
+        )
+        self.dynamic_shape = ArgSpecHelper(
+            name="--dynamic-shape", action="store_true", help="If set, don't quantize the model."
+        )
+        self.with_makefile = ArgSpecHelper(
+            name="--with-makefile",
+            action="store_true",
+            help="Generate corresponding makefile.",
+            hidden=True,
+        )
+
+    @property
+    def name(self):
+        return "codegen"
+
+
+class ProfilerArguments(ArgumentsBase):
+    def __init__(self) -> None:
+        super(ProfilerArguments, self).__init__()
+
+        self.ir_type = ArgSpecHelper(
+            name="--ir-type",
+            choices=[
+                "relay",
+            ],
+            default="relay",
+            help="The ir type that will be profiled, default is relay",
+        )
+        self.indicator = ArgSpecHelper(
+            name="--indicator",
+            choices=["cal", "mem", "all"],
+            default="cal",
+            nargs="+",
+            help="Select indicator to profile, default is cal(calculation).\n"
+            "cal: calculation, how many operations to be executed for current op.\n"
+            "mem: memory, how many memory to be used for current op.\n"
+            "all: include all indicators above.",
+        )
+        self.output_type = ArgSpecHelper(
+            name="--output-type",
+            choices=["json", "binary", "print", "total", "all"],
+            default="total",
+            nargs="+",
+            help="How to show results, default is show summary result.",
+        )
+
+    @property
+    def name(self):
+        return "profiler"
+
+
+class MainArguments(ArgumentsBase):
+    def __init__(self) -> None:
+        super(MainArguments, self).__init__()
+
+        self.verbose = ArgSpecHelper(
+            name="--verbose",
+            abbr_name="-v",
+            action="count",
+            default=0,
+            help="Increase verbosity",
+        )
+        self.help = ArgSpecHelper(
+            name="--help",
+            abbr_name="-h",
+            action="store_true",
+            help="Show this help information",
+        )
+        self.version = ArgSpecHelper(
+            name="--version",
+            action="version",
+            version="{}\n".format(hhb_version()),
+            help="Print the version and exit",
+        )
+        self.E = ArgSpecHelper(name="-E", action="store_true", help="Convert model into relay ir.")
+        self.Q = ArgSpecHelper(name="-Q", action="store_true", help="Quantize the relay ir.")
+        self.C = ArgSpecHelper(name="-C", action="store_true", help="codegen the model.")
+        self.D = ArgSpecHelper(name="-D", action="store_true", help="deploy on platform.")
+        self.S = ArgSpecHelper(name="-S", action="store_true", help="run elf to simulate.")
+        self.simulate = ArgSpecHelper(
+            name="--simulate", action="store_true", help="Simulate model on x86 device."
+        )
+        self.add_exclusive_group(self.E, self.Q, self.C, self.D, self.S, self.simulate)
+
+        self.no_quantize = ArgSpecHelper(
+            name="--no-quantize", action="store_true", help="If set, don't quantize the model."
+        )
+        self.model_file = ArgSpecHelper(
+            name="--model-file",
+            abbr_name="-f",
+            nargs="+",
+            help="Path to the input model file, can pass multi files",
+        )
+        self.save_temps = ArgSpecHelper(
+            name="--save-temps", action="store_true", help="Save temp files."
+        )
+        self.generate_dataset = ArgSpecHelper(
+            name="--generate-dataset",
+            action="store_true",
+            help="Generate dataset according to provided preprocess parameters.",
+        )
+        self.generate_readme = ArgSpecHelper(
+            name="--generate-readme",
+            action="store_true",
+            help="Automatically generate README.md.",
+            hidden=True,
+        )
+
+    @property
+    def name(self):
+        return "main"
+
+
+class Config(object):
+    def __init__(self, board="unset") -> None:
+        self.common = CommonArguments()
+        self.import_config = ImportArguments()
+        self.optimize = OptimizeArguments()
+        self.quantize = QuantizeArguments()
+        self.hardware = HardwareArguments()
+        self.simulate = SimulateArguments()
+        self.postprocess = PostprocessArguments()
+        self.preprocess = PreprocessArguments()
+        self.codegen = CodegenArguments()
+        self.profile = ProfilerArguments()
+        self.main = MainArguments()
+
+        self.set_config_by_board(board)
+
+        self._cmd_config = None
+
+    def update_config_from_module(self, hhb_ir):
+        mod, params = hhb_ir.get_model()
+        input_name_list, input_shape_list, _ = get_input_info_from_relay(mod, params)
+        output_shape_list, _ = get_output_info_from_relay(mod, params)
+
+        # if self.import_config.input_name.value is None:
+        self.import_config.input_name.value = input_name_list
+        self.import_config.input_shape.value = input_shape_list
+        if self.import_config.output_name.value is None:
+            self.import_config.output_name.value = []
+            for i in range(len(output_shape_list)):
+                self.import_config.output_name.value.append("output" + str(i))
+
+    def update_config_from_file(self, path: str):
+        """Update arguments values in config.
+
+        The specified json file can be generated by generate_hhb_default_config().
+        """
+        # init ARGS_DEST_TO_OPTIONS_STRING
+        get_default_config()
+
+        # config from specified file
+        file_config = {}
+        if path and os.path.isfile(path):
+            with open(path, "r") as f:
+                file_config = json.load(f)
+        if not file_config:
+            return
+
+        for item in file_config.values():
+            for dest, value in item.items():
+                optstr = tuple(ARGS_DEST_TO_OPTIONS_STRING[dest])
+
+                for arg in self.__dict__.values():
+                    if not isinstance(arg, ArgumentsBase):
+                        continue
+                    optstr_to_arg = arg.get_option_string_to_argument()
+                    if optstr in optstr_to_arg:
+                        optstr_to_arg[optstr].value = value
+
+    def get_all_arguments_info(self):
+        if not ARGS_DEST_TO_OPTIONS_STRING:
+            raise HHBException(
+                "Please generate command line arguments by generate_cmd_config() first."
+            )
+
+        optinon_string_to_dest = {}
+        for k, v in ARGS_DEST_TO_OPTIONS_STRING.items():
+            optinon_string_to_dest[tuple(v)] = k
+
+        res = {}
+        for arg in self.__dict__.values():
+            if not isinstance(arg, ArgumentsBase):
+                continue
+            res[arg.name] = {}
+            opt_str_to_arg = arg.get_option_string_to_argument()
+            for k, v in opt_str_to_arg.items():
+                if k in optinon_string_to_dest:
+                    dest_name = optinon_string_to_dest[k]
+                    res[arg.name][dest_name] = v.value
+
+        return res
+
+    def set_config_by_board(self, board: str):
+        if board not in self.optimize.board.spec.choices:
+            raise HHBException(
+                "Specified board: {} is not in {}".format(board, self.optimize.board.spec.choices)
+            )
+        self.optimize.board.value = board
+
+        if board in ("anole",):
+            self.quantize.quantization_scheme.value = "uint8_asym"
+        elif board in ("x86_ref", "th1520"):
+            self.quantize.quantization_scheme.value = "int8_asym"
+        elif board in ("c906", "c920"):
+            self.quantize.quantization_scheme.value = "float16"
+        elif board in ("e907", "c908", "rvm"):
+            self.quantize.quantization_scheme.value = "int8_asym_w_sym"
+        else:
+            self.quantize.quantization_scheme.value = "uint8_asym"
+
+    def generate_cmd_config(self, with_io_info=True):
+        """Genrate command line arguments."""
+
+        def _update_config(orig_config, new_config):
+            for sec, value in new_config.items():
+                if sec in orig_config:
+                    orig_config[sec].update(value)
+
+        # This is the base config for cmd backend.
+        base_config, _ = get_default_config()
+
+        # The arguments that are set by user with Config obj
+        # It should overwrite the base config first.
+        obj_config = self.get_all_arguments_info()
+        _update_config(base_config, obj_config)
+
+        # unroll arguments
+        unroll_config = AttributeDict()
+        for value in base_config.values():
+            unroll_config.update(value)
+
+        extra_args = AttributeDict()
+        all_filters = []
+        if with_io_info:
+            all_filters = [
+                collect_preprocess_config,
+                set_preprocess_params,
+                collect_quantization_config,
+                set_quantize_params_by_board,
+                collect_codegen_config,
+                set_codegen_config,
+            ]
+            if (
+                self.import_config.input_shape.value is None
+                or self.import_config.output_name.value is None
+            ):
+                raise HHBException(
+                    "There is no input/output info, please set them directly or execute "
+                    "update_config_from_module() firstly."
+                )
+
+            extra_args.input_shape = self.import_config.input_shape.value
+            extra_args.input_num = len(extra_args.input_shape)
+            extra_args.output_num = len(self.import_config.output_name.value)
+        args_filter = ArgumentFilter(unroll_config)
+        args_filter.filtered_args = unroll_config
+        args_filter.filter_argument(all_filters, extra=extra_args)
+
+        self._cmd_config = args_filter.filtered_args
+
+
+@get_parameters_info(CommonArguments().name)
+def add_common_argument(parser):
+    """All common parameters"""
+    CommonArguments().set_parser(parser)
+
+
+@get_parameters_info(PreprocessArguments().name)
 def add_preprocess_argument(parser):
-    """ All preprocess parameters"""
-    parser.add_argument(
-        "-m",
-        "--data-mean",
-        type=str,
-        default="0",
-        metavar="",
-        help="Set the mean value of input, multiple values are separated by space, "
-        "default is 0.",
-    )
-
-    group = parser.add_mutually_exclusive_group()
-    group.add_argument(
-        "-s",
-        "--data-scale",
-        type=float,
-        default="1",
-        metavar="",
-        help="Scale number(mul) for inputs normalization(data=img*scale), default is 1.",
-    )
-    group.add_argument(
-        "-sv",
-        "--data-scale-div",
-        type=float,
-        default="1",
-        metavar="",
-        help="Scale number(div) for inputs normalization(data=img/scale), default is 1.",
-    )
-
-    parser.add_argument(
-        "-r",
-        "--data-resize",
-        type=int,
-        default=None,
-        metavar="",
-        help="Resize base size for input image to resize.",
-    )
-    parser.add_argument(
-        "--pixel-format",
-        choices=["RGB", "BGR"],
-        default="RGB",
-        help="The pixel format of image data, defalut is RGB",
-    )
-    parser.add_argument(
-        "--data-layout",
-        choices=["NCHW", "NHWC", "CHW", "HWC", "Any"],
-        default="NCHW",
-        # help='The input data layout, defalut is "NCHW"',
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--add-preprocess-node", action="store_true", help="Add preprocess node for model."
-    )
-    parser.add_argument(
-        "--light-input-fix-size",
-        type=str,
-        default="0",
-        metavar="",
-        help=argparse.SUPPRESS,
-    )
+    """All preprocess parameters"""
+    PreprocessArguments().set_parser(parser)
 
 
-@get_parameters_info("import")
+@get_parameters_info(ImportArguments().name)
 def add_import_argument(parser):
     """All parameters needed by 'import' subcommand"""
-    # import frontends
-    parser.add_argument(
-        "-in",
-        "--input-name",
-        type=str,
-        default=None,
-        metavar="",
-        help="Set the name of input node. If '--input-name'is None, "
-        "default value is 'Placeholder'. Multiple values "
-        "are separated by semicolon(;).",
-    )
-    parser.add_argument(
-        "-is",
-        "--input-shape",
-        type=str,
-        default=None,
-        metavar="",
-        help="Set the shape of input nodes. Multiple shapes are separated "
-        "by semicolon(;) and the dims between shape are separated "
-        "by space.",
-    )
-    parser.add_argument(
-        "-on",
-        "--output-name",
-        type=str,
-        metavar="",
-        help="Set the name of output nodes. Multiple shapes are " "separated by semicolon(;).",
-    )
-    from .frontend_manage import get_frontend_names
-
-    parser.add_argument(
-        "--model-format",
-        choices=get_frontend_names(),
-        help="Specify input model format:{}".format(get_frontend_names()),
-    )
-    parser.add_argument(
-        "--reorder-pixel-format",
-        action="store_true",
-        help="If original model's input data pixel format is rgb, then covert it to bgr;"
-        "otherwise, then convert it to rgb.",
-    )
+    ImportArguments().set_parser(parser)
 
 
-@get_parameters_info("optimize")
+@get_parameters_info(OptimizeArguments().name)
 def add_optimize_argument(parser):
     """All parameters needed by optimization"""
-    parser.add_argument(
-        "--board",
-        default="unset",
-        choices=[
-            "anole",
-            "light",
-            "hlight",
-            "asp",
-            "i805",
-            "c860",
-            "c906",
-            "c908",
-            "x86_ref",
-            "unset",
-        ],
-        help="Set target device, default is anole.",
-    )
-    parser.add_argument(
-        "--opt-level",
-        choices=[-1, 0, 1, 2, 3],
-        default=3,
-        type=int,
-        # help="Specify the optimization level, default is 3.",
-        help=argparse.SUPPRESS,
-    )
+    OptimizeArguments().set_parser(parser)
 
 
-@get_parameters_info("quantize")
+@get_parameters_info(QuantizeArguments().name)
 def add_quantize_argument(parser):
     """All parameters needed by 'quantize' subcommand"""
-    parser.add_argument(
-        "-cd",
-        "--calibrate-dataset",
-        type=str,
-        default=None,
-        metavar="",
-        help="Provide with dataset for the input of model in reference step. "
-        "Support dir or .npz .jpg .png .JPEG or .txt in which there are path "
-        "of images. Note: only one image path in one line if .txt.",
-    )
-    parser.add_argument(
-        "--quantization-scheme",
-        choices=[
-            "int4_asym_w_sym",
-            "uint8_asym",
-            "int8_asym",
-            "int8_sym",
-            "int8_original",
-            "int8_asym_w_sym",
-            "int16_sym",
-            "float16",
-            "bfloat16",
-            "float32",
-            "unset",
-        ],
-        default="unset",
-        help="Scheme of quantization. default is unset, and select scheme by --board.",
-    )
-    parser.add_argument(
-        "--auto-hybrid-quantization",
-        action="store_true",
-        help="If set, quantize model automatically.",
-    )
-    parser.add_argument(
-        "--quantization-loss-algorithm",
-        type=str,
-        choices=["cos_similarity", "mse", "kl_divergence", "cross_entropy", "gini"],
-        default="cos_similarity",
-        help="How to calculate accuracy loss for every layer.",
-    )
-    parser.add_argument(
-        "--quantization-loss-threshold",
-        type=float,
-        default=0.99,
-        help="The threshold that will determin thich layer will be quantized with hybrid way."
-        "If it is None, we will select threshold automatically.",
-    )
-    parser.add_argument(
-        "--dump-quantization-loss",
-        action="store_true",
-        help="If set, dump quantizaiton loss into file.",
-    )
-    parser.add_argument(
-        "--loss-threshold-type",
-        type=str,
-        choices=["min", "max", "avg"],
-        default="avg",
-        # help="The threshold type for quantizaiton loss, default is avg.",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--from-quant-file",
-        action="store_true",
-        # help="If set, get hybrid quantization infomation from model.quant.json",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--ignore-hybrid-layer",
-        type=str,
-        nargs="+",
-        # help="Ignore layers to be hybrid layers.",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--hybrid-quantization-scheme",
-        choices=[
-            "int4_asym_w_sym",
-            "uint8_asym",
-            "int8_asym",
-            "int8_sym",
-            "int8_original",
-            "int8_asym_w_sym",
-            "int16_sym",
-            "float16",
-            "bfloat16",
-            "unset",
-        ],
-        default="unset",
-        help="Scheme of hybrid quantization. default is unset.",
-    )
-    parser.add_argument(
-        "--hybrid-layer-name",
-        type=str,
-        nargs="+",
-        help="Layer buffer name to use hybrid quantization.",
-    )
-    parser.add_argument(
-        "--num-bit-activation",
-        type=int,
-        choices=[0, 16, 32],
-        default=0,
-        # help="The bit number that quantizes activation layer. default is 0, means unset.",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--num-bit-input",
-        type=int,
-        choices=[0, 8, 16, 32],
-        default=0,
-        # help="The bit number that quantizes input layer. default is 0, means unset.",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--num-bit-weight",
-        type=int,
-        choices=[0, 8, 16, 32],
-        default=0,
-        # help="The bit number that quantizes weight layer. default is 0, means unset.",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--dtype-input",
-        choices=["float", "int", "uint", "unset"],
-        default="unset",
-        # help="The dtype of quantized input layer, default is uint.",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--dtype-weight",
-        choices=["float", "int", "uint", "unset"],
-        default="unset",
-        # help="The dtype of quantized constant parameters, default is uint.",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--dtype-activation",
-        choices=["float", "int", "uint", "unset"],
-        default="unset",
-        # help="The dtype of quantized activation layer, default is uint.",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--calibrate-mode",
-        choices=["maxmin", "pow2", "kl_divergence", "kl_divergence_tsing"],
-        default="maxmin",
-        # help="How to calibrate while doing quantization, default is maxmin.",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--activate-quantized-type",
-        choices=["asym", "sym", "unset"],
-        default="unset",
-        # help="Select the algorithm of quantization, default is asym.",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--weight-quantized-type",
-        choices=["asym", "sym", "unset"],
-        default="unset",
-        # help="Select the algorithm of quantization, default is asym.",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--weight-scale",
-        choices=["max", "power2"],
-        default="max",
-        # help="Select the mothod that quantizes weight value, default is max.",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--fuse-conv-relu",
-        action="store_true",
-        help="Fuse the convolution and relu layer.",
-    )
-    parser.add_argument(
-        "--fuse-reshape-dense",
-        action="store_true",
-        help="Fuse the reshape and dense layer.",
-    )
-    parser.add_argument(
-        "--channel-quantization",
-        action="store_true",
-        help="Do quantizetion across channel.",
-    )
-    parser.add_argument(
-        "--broadcast-quantization",
-        action="store_true",
-        help="Broadcast quantization parameters for special ops.",
-    )
-    parser.add_argument(
-        "--channel-quantization-ratio-threshold",
-        type=float,
-        default=0.0,
-        help=argparse.SUPPRESS,
-        # help="Set optimize quantitative parameters threshold for channel quantization."
-        # + "The value can be selected in range [0, 1). 0 means this pass is not be used."
-        # + "0.3 is a recommended threshold if this pass is turned on.",
-    )
-    parser.add_argument(
-        "--fuse-clip",
-        action="store_true",
-        help="Fuse clip's attr into pre layer's quantitative information. "
-        + "This flag is only valid when quantization is used.",
-    )
-    parser.add_argument(
-        "--fuse-mul-before-conv",
-        default=True,
-        choices=[False, True],
-        type=boolean_string,
-        help=argparse.SUPPRESS,
-        # help="This parameter is used to merge mul before conv2d to conv2d.",
-    )
-    parser.add_argument(
-        "--fuse-mul-after-conv",
-        default=True,
-        choices=[False, True],
-        type=boolean_string,
-        help=argparse.SUPPRESS,
-        # help="This parameter is used to merge mul after conv2d to conv2d.",
-    )
-    parser.add_argument(
-        "--fuse-add-before-conv",
-        default=True,
-        choices=[False, True],
-        type=boolean_string,
-        help=argparse.SUPPRESS,
-        # help="This parameter is used to merge add before conv2d to conv2d.",
-    )
-    parser.add_argument(
-        "--fuse-add-after-conv",
-        default=True,
-        choices=[False, True],
-        type=boolean_string,
-        help=argparse.SUPPRESS,
-        # help="This parameter is used to merge add after conv2d to conv2d.",
-    )
-    parser.add_argument(
-        "--fuse-zp2bias",
-        action="store_true",
-        help="Merge conv2d/dense zp to bias.",
-    )
-    parser.add_argument(
-        "--target-layout",
-        default="NCHW",
-        choices=["NCHW", "NHWC"],
-        help="Set target layout.",
-    )
-    parser.add_argument(
-        "--use-custom-fusion",
-        action="store_true",
-        help=argparse.SUPPRESS,
-        # help="This parameter is used to use custom fusion like fuse cache_matmul and layer norm.",
-    )
-    parser.add_argument(
-        "--convert-to-relay",
-        action="store_true",
-        help=argparse.SUPPRESS,
-        # help="This parameter is used to convert quanted qnn model to relay.",
-    )
+    QuantizeArguments().set_parser(parser)
 
 
-@get_parameters_info("hardware")
+@get_parameters_info(HardwareArguments().name)
 def add_hardware_argument(parser):
-    parser.add_argument(
-        "--hardware-sram-size",
-        type=str,
-        default=None,
-        metavar="",
-        help=argparse.SUPPRESS,
-        # help="Set the size of sram. The unit must in [m, M, KB, kb].",
-    )
-    parser.add_argument(
-        "--hardware-max-groups",
-        type=int,
-        default=0,
-        help=argparse.SUPPRESS,
-        # help="This parameter is used to describe the maximum number of groups supported by hardware.",
-    )
-    parser.add_argument(
-        "--hardware-max-out-channel",
-        type=int,
-        default=0,
-        help=argparse.SUPPRESS,
-        # help="This parameter is used to describe the maximum number of output channel supported by hardware.",
-    )
-    parser.add_argument(
-        "--hardware-max-kernel-size",
-        type=int,
-        default=0,
-        help=argparse.SUPPRESS,
-        # help="This parameter is used to describe the size of sram.",
-    )
-    parser.add_argument(
-        "--hardware-contain-weight",
-        action="store_true",
-        help=argparse.SUPPRESS,
-        # help="This parameter is used to describe whether the weight size should be contained when split ops.",
-    )
-    parser.add_argument(
-        "--hardware-alignment",
-        type=int,
-        choices=[1, 8, 16, 32],
-        default=1,
-        help=argparse.SUPPRESS,
-        # help="This parameter describes whether the hardware requires data alignment.",
-    )
-    parser.add_argument(
-        "--structed-sparsity",
-        default="unset",
-        choices=[
-            "asp4:2",
-            "asp4:1",
-            "unset",
-        ],
-        help="Specify the structed sparsity scheme, default is unset.",
-    )
-    parser.add_argument(
-        "--kernel-parallel",
-        default="0",
-        type=int,
-        help="Specify every layer's kernel parallel, default is 0, auto choose best parallel.",
-    )
+    """All hardware parameters"""
+    HardwareArguments().set_parser(parser)
 
 
-@get_parameters_info("simulate")
+@get_parameters_info(SimulateArguments().name)
 def add_simulate_argument(parser):
     """All parameters needed by 'simulate' subcommand"""
-    parser.add_argument(
-        "-sd",
-        "--simulate-data",
-        type=str,
-        default=None,
-        metavar="",
-        help="Provide with dataset for the input of model in reference step. "
-        "Support dir or .npz .jpg .png .JPEG or .txt in which there are path "
-        "of images. Note: only one image path in one line if .txt.",
-    )
+    SimulateArguments().set_parser(parser)
 
 
-@get_parameters_info("postprocess")
+@get_parameters_info(PostprocessArguments().name)
 def add_postprocess_argument(parser):
     """All postprocess parameters"""
-    parser.add_argument(
-        "--postprocess",
-        type=str,
-        default="top5",
-        choices=["top5", "save", "save_and_top5"],
-        help="Set the mode of postprocess: "
-        "'top5' show top5 of output; "
-        "'save' save output to file;"
-        "'save_and_top5' show top5 and save output to file."
-        " Default is top5",
-    )
+    PostprocessArguments().set_parser(parser)
 
 
-@get_parameters_info("main")
+@get_parameters_info(MainArguments().name)
 def add_main_argument(parser):
     """All commands that are compatible with previous version."""
-    parser.add_argument("-v", "--verbose", action="count", default=0, help="Increase verbosity")
-    parser.add_argument("-h", "--help", action="store_true", help="Show this help information")
-    parser.add_argument(
-        "--version",
-        action="version",
-        version="{}\n".format(hhb_version()),
-        help="Print the version and exit",
-    )
-
-    group = parser.add_mutually_exclusive_group()
-    group.add_argument("-E", action="store_true", help="Convert model into relay ir.")
-    group.add_argument("-Q", action="store_true", help="Quantize the relay ir.")
-    group.add_argument("-C", action="store_true", help="codegen the model.")
-    group.add_argument("--simulate", action="store_true", help="Simulate model on x86 device.")
-    # group.add_argument(
-    #     "--generate-config", action="store_true", help="Generate config file for HHB"
-    # )
-    parser.add_argument(
-        "--no-quantize", action="store_true", help="If set, don't quantize the model."
-    )
-    parser.add_argument(
-        "-f",
-        "--model-file",
-        nargs="+",
-        metavar="",
-        help="Path to the input model file, can pass multi files",
-    )
-    parser.add_argument("--save-temps", action="store_true", help="Save temp files.")
-    parser.add_argument(
-        "--generate-dataset",
-        action="store_true",
-        help="Generate dataset according to provided preprocess parameters.",
-    )
-    parser.add_argument(
-        "-o",
-        "--output",
-        metavar="",
-        default="hhb_out",
-        help="The directory that holds the outputs.",
-    )
-    parser.add_argument(
-        "--generate-readme",
-        action="store_true",
-        help=argparse.SUPPRESS,
-        # help="Automatically generate README.md."
-    )
+    MainArguments().set_parser(parser)
 
 
-@get_parameters_info("codegen")
+@get_parameters_info(CodegenArguments().name)
 def add_codegen_argument(parser):
-    parser.add_argument(
-        "--model-save",
-        choices=["run_only", "save_only", "save_and_run"],
-        default="run_only",
-        help="Whether save binary graph or run only.\n"
-        "run_only: execute model only, not save binary graph.\n"
-        "save_only: save binary graph only.\n"
-        "save_and_run: execute and save model.",
-    )
-    parser.add_argument(
-        "--model-priority",
-        default=0,
-        type=int,
-        help="Set model priority, only for light now.\n" "0 is lowest, 1 is medium, 2 is highest.",
-    )
-    parser.add_argument(
-        "--without-preprocess",
-        action="store_true",
-        help="Do not generate preprocess codes.",
-    )
-    parser.add_argument(
-        "--multithread",
-        action="store_true",
-        # help="Create multithread codes."
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--trace-strategy",
-        choices=["normal", "advanced"],
-        default="normal",
-        # help="Strategy to generate trace data.",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "--input-memory-type",
-        choices=[0, 1, 2],
-        type=int,
-        nargs="+",
-        help="Set the memory type for input tensor, support for multi-values.\n"
-        "0: allocated by CPU and not aligned;\n"
-        "1: allocated by CPU and aligned;\n"
-        "2: dma buffer.",
-    )
-    parser.add_argument(
-        "--output-memory-type",
-        choices=[0, 1, 2],
-        type=int,
-        nargs="+",
-        help="Set the memory type for output tensor, support for multi-values.\n"
-        "0: allocated by CPU and not aligned;\n"
-        "1: allocated by CPU and aligned;\n"
-        "2: dma buffer.",
-    )
-    parser.add_argument(
-        "--memory-type",
-        choices=[0, 1, 2],
-        type=int,
-        help="Set the memory type for input and output tensors.\n"
-        "0: allocated by CPU and not aligned;\n"
-        "1: allocated by CPU and aligned;\n"
-        "2: dma buffer.",
-    )
-    parser.add_argument(
-        "--dynamic-cb-reg", action="store_true", help="Emit cb_map file to reduce elf size on RTOS."
-    )
-    parser.add_argument(
-        "--conv2d-algorithm",
-        choices=["direct", "winograd", "gemm", "unset"],
-        default="unset",
-        # help="The recommend algorithm for conv2d implementation, default is unset.",
-        help=argparse.SUPPRESS,
-    )
+    """All codegen parameters"""
+    CodegenArguments().set_parser(parser)
 
 
-@get_parameters_info("profiler")
+@get_parameters_info(ProfilerArguments().name)
 def add_profiler_argument(parser):
-    parser.add_argument(
-        "--ir-type",
-        choices=["relay", "light"],
-        default="relay",
-        help="The ir type that will be profiled, default is relay",
-    )
-    parser.add_argument(
-        "--indicator",
-        choices=["cal", "mem", "cycle", "all"],
-        default="cal",
-        nargs="+",
-        help="Select indicator to profile, default is cal(calculation).\n"
-        "cal: calculation, how many operations to be executed for current op.\n"
-        "mem: memory, how many memory to be used for current op.\n"
-        "cycle: how many cycles to execute op.\n"
-        "all: include all indicators above.",
-    )
-    parser.add_argument(
-        "--output-type",
-        choices=["json", "binary", "print", "total", "all"],
-        default="total",
-        nargs="+",
-        help="How to show results, default is show summary result.",
-    )
-    parser.add_argument(
-        "--npu-frequency",
-        default=1000000000,
-        type=int,
-        help="NPU frequency(HZ).",
-    )
+    """All profiler parameters"""
+    ProfilerArguments().set_parser(parser)
 
 
 @argument_filter_helper
 def parse_node_name(filtered_args, extra=None):
     """
     Convert "input1;input2;input3..." into ["input1", "input2", "input3", ...]
 
@@ -734,14 +1181,16 @@
     filtered_args : AttributeDict
         filtered args
     """
 
     def convert_str2list(name):
         if not name:
             return list()
+        if isinstance(name, (list, tuple)):
+            return list(name)
         name_list = name.strip().split(";")
         name_list = list([n for n in name_list if n])
         name_list = [n.strip() for n in name_list]
         return list(name_list)
 
     if hasattr(filtered_args, "input_name"):
         filtered_args["input_name"] = convert_str2list(filtered_args["input_name"])
@@ -762,14 +1211,16 @@
     filtered_args : AttributeDict
         filtered args
     """
 
     def convert_str2list(shape):
         if not shape:
             return list()
+        if isinstance(shape, (list, tuple)):
+            return list(shape)
         if "," in shape:
             shape = shape.replace(",", " ")
         shape_list = []
         shape_str_list = shape.strip().split(";")
         shape_str_list = list([n for n in shape_str_list if n])
         for shape_str in shape_str_list:
             tmp_list = shape_str.strip().split(" ")
@@ -791,19 +1242,21 @@
 
     Parameters
     ----------
     filtered_args : AttributeDict
         filtered args
     """
     size_map = {
-        "kb": 2 ** 10,
-        "m": 2 ** 20,
+        "kb": 2**10,
+        "m": 2**20,
     }
 
     def convert_str2int(txt_size):
+        if isinstance(txt_size, int):
+            return txt_size
         if txt_size:
             txt_size = txt_size.lower()
             if "kb" in txt_size:
                 num = txt_size[: txt_size.find("kb")]
                 sram_size = float(num) * size_map["kb"]
             elif "m" in txt_size:
                 num = txt_size[: txt_size.find("m")]
@@ -845,15 +1298,18 @@
 
             ALL_ARGUMENTS_INFO[name][arg_name] = arg_value
 
 
 class ArgumentFilter(object):
     def __init__(self, args):
         self.origin_args = args  # parsed by argparse
-        self.filtered_args = AttributeDict(**(self.origin_args.__dict__))
+        if isinstance(self.origin_args, argparse.Namespace):
+            self.filtered_args = AttributeDict(**(self.origin_args.__dict__))
+        else:
+            self.filtered_args = AttributeDict(**self.origin_args)
 
         self._built_in_filter()
 
     def _built_in_filter(self):
         # do some basic filtering
         _func_handle_seq = [parse_node_name, parse_node_shape, parse_sram_size]
 
@@ -1006,7 +1462,92 @@
             args_filter.filtered_args.func = driver_main_command
 
         try:
             return args_filter.filtered_args.func(args_filter)
         except HHBException as err:
             sys.stderr.write("Error: {}".format(err))
             return 4
+
+
+def get_default_config():
+    arg_manage = ArgumentManage([])
+    parser = argparse.ArgumentParser(add_help=False)
+    # add command line parameters
+    arg_manage.set_main_command(parser)
+    add_profiler_argument(parser)
+    desc = collect_arguments_info(parser._actions)
+    res = copy.deepcopy(ALL_ARGUMENTS_INFO)
+
+    return res, desc
+
+
+def generate_hhb_default_config(
+    path="hhb_config_default.json", specified_groups=None, with_hidden=False
+):
+    """Generate defualt config.
+
+    Parameters
+    ----------
+    path : str
+        The path of file that holds default config.
+    specified_groups : list or tuple
+        Arguments in sepcified_groups are generated. Group name can be selected from
+        ["common", "preprocess", "import", "optimize", "quantize", "hardware",
+            "simulate", "postprocess", "main", "codegen", "profiler"]
+    with_hidden : bool
+        If it is true, more arguments will be generated in the config file.
+    """
+    res, desc = get_default_config()
+
+    exclude_sections = [
+        # "main",
+        # "import",
+        # "preprocess",
+        # "common",
+        # "postprocess",
+        # "simulate",
+    ]
+    all_sections = ALL_ARGUMENTS_INFO.keys()
+    if not specified_groups:
+        specified_groups = list(all_sections)
+    if not isinstance(specified_groups, (str, list, tuple)):
+        raise HHBException("Unsupport for type: {}".format(type(specified_groups)))
+    if isinstance(specified_groups, str):
+        specified_groups = [
+            specified_groups,
+        ]
+    inter_exclude = set(all_sections) - set(specified_groups)
+    exclude_sections += list(inter_exclude)
+
+    exclude_arguments = [
+        # "opt_level",
+        # "calibrate_dataset",
+        # "config_file",
+        # "generate_config"
+    ]
+
+    # ignore hidden arguments
+    non_hidden_argument = []
+    for item in desc:
+        modify_item = item.name.strip().split(",")[-1].strip()
+        if "--" not in modify_item:
+            modify_item = modify_item.replace("-", "")
+        else:
+            modify_item = modify_item.replace("--", "")
+            modify_item = modify_item.replace("-", "_")
+        non_hidden_argument.append(modify_item)
+
+    # delete some unused arguments
+    for ses, value in ALL_ARGUMENTS_INFO.items():
+        if ses in exclude_sections:
+            res.pop(ses)
+            continue
+        for arg in value.keys():
+            if arg in exclude_arguments:
+                res[ses].pop(arg)
+                continue
+            if not with_hidden and arg not in non_hidden_argument:
+                res[ses].pop(arg)
+                continue
+
+    with open(path, "w") as f:
+        json.dump(res, f, indent=2)
```

## hhb/core/codegen_manage.py

```diff
@@ -24,28 +24,35 @@
 from tvm import relay
 from math import ceil
 
 from .common import argument_filter_helper, hhb_exit
 from .common import ALL_ARGUMENTS_INFO
 from .common import AttributeDict
 from .common import HHBException
+from .common import parse_mean
 from .hhbir_manage import HHBBoardQnnCodegenIR
 from tvm.relay.backend.contrib.csinn_backend import emit_binary_model
 
 
 logger = logging.getLogger("HHB")
 
 
 @argument_filter_helper
 def collect_codegen_config(filtered_args, extra=None):
     """collect codegen arguments"""
     filtered_args.codegen_config = AttributeDict()
     for k in ALL_ARGUMENTS_INFO["codegen"]:
         filtered_args.codegen_config[k] = filtered_args[k]
 
+    filtered_args.codegen_config.th1520_input_fix_size = parse_mean(
+        filtered_args.codegen_config.th1520_input_fix_size
+    )
+    if filtered_args.codegen_config.model_save == "save_only":
+        raise HHBException("Unsupport --model-save = save_only.\n")
+
 
 @argument_filter_helper
 def set_codegen_config(filtered_args, extra=None):
     """set codegen arguments"""
 
     def _set_memory_type(io_memory_type, io_num, unify_type=None):
         res = io_memory_type
@@ -91,69 +98,58 @@
         execute_path = os.path.dirname(os.path.realpath(sys.executable))
     else:
         execute_path, _ = os.path.split(os.path.abspath(__file__))
         execute_path = os.path.join(execute_path, "..")
     return execute_path
 
 
-def main_c_codegen(
+def entry_c_codegen(
     codegen_obj: HHBBoardQnnCodegenIR,
     input_shape,
     output_shape,
     board,
     output_path,
+    main_file,
     postprocess="top5",
     model_save="run_only",
     without_preprocess=False,
     preprocess_params=None,
     multithread=False,
     input_memory_type=None,
     q_scheme=None,
+    dynamic_shape=None,
+    hhb_gen=False,
 ):
-    """ Generate the main.c file """
+    """Generate the main.c file"""
 
     execute_path = get_execute_path()
-    if board == "anole":
-        if multithread:
-            main_file = os.path.join(execute_path, "config", "anole_multithread.tp")
-        else:
-            main_file = os.path.join(execute_path, "config", "anole.tp")
-    elif board in ("light", "hlight"):
-        main_file = os.path.join(execute_path, "config", "light.tp")
-    elif board == "c906" or board == "c908":
-        main_file = os.path.join(execute_path, "config", "c906.tp")
-    else:
-        main_file = os.path.join(execute_path, "config", "thead.tp")
 
     with open(main_file, "r") as f:
         code_str = f.read()
 
     template_dir = os.path.join(execute_path, "config", "template")
 
     # check options setting
     if preprocess_params.calibrate_data_format == "npz":
         without_preprocess = True
-    if board in ("asp"):
-        without_preprocess = True
-    if board != "anole" and board != "light":
+
+    if board != "anole" and board != "th1520":
         # disable_nbg = True
         model_save = "run_only"
 
     #######################################################################
     #
     # Header Codegen
     #
     with open(os.path.join(template_dir, "header.tp"), "r") as f:
         header_str = f.read()
     if board == "anole":
         header_str += '\n#include "shl_ovx.h"'
-    elif board in ("light", "hlight", "asp", "c906", "c908"):
-        header_str += '\n#include "shl_ref.h"'
     else:
-        header_str += '\n#include "csi_nn.h"'
+        header_str += '\n#include "shl_ref.h"'
 
     if not without_preprocess:
         header_str += '\n#include "process.h"'
         process_c_path = os.path.join(execute_path, "config", "process", "src", "process.c")
         process_c = os.path.join(output_path, codegen_obj.preprocess_source_name)
         process_h_path = os.path.join(execute_path, "config", "process", "include", "process.h")
         process_h = os.path.join(output_path, codegen_obj.preprocess_header_name)
@@ -198,26 +194,20 @@
     for i in range(len(input_shape)):
         csinn_args += "void *data" + str(i) + ", "
     function_str = function_str.replace("#_csinn_args#", csinn_args)
     if multithread and board == "anole":
         function_str = function_str.replace(
             "void *csinn_(char *params);", "void *csinn_(char *params, int deviceIndex);"
         )
-    if board == "light" and model_save == "save_only":
+    if board == "th1520" and model_save == "save_only":
         function_str = function_str.replace(
             "void *csinn_(char *params);", "#define csinn_(...) NULL"
         )
     code_str = code_str.replace("#_hhb_function_decl_#", function_str)
 
-    if board == "c860":
-        csinn_args = ""
-        for i in range(len(input_shape) + len(output_shape)):
-            csinn_args += "void *data" + str(i) + ", "
-        code_str = code_str.replace("#_thead_csinn_args#", csinn_args)
-
     #######################################################################
     #
     # Global Variable Codegen
     #
     with open(os.path.join(template_dir, "global_var_decl.tp"), "r") as f:
         global_var_str = f.read()
 
@@ -259,37 +249,37 @@
     #
     # Postprocess Codegen
     #
     with open(os.path.join(template_dir, "postprocess_def.tp"), "r") as f:
         postprocess_str = f.read()
 
     convert_fouput = ""
-    if board in ("light", "hlight", "asp", "c906", "c908"):
+    if board != "anole":
         convert_fouput = "struct csinn_tensor *foutput = shl_ref_tensor_transform_f32(output);"
 
     postprocess_str = postprocess_str.replace("#_convert_fouput_#", convert_fouput)
 
     show_top5 = ""
     if "top5" in postprocess:
-        if board in ("light", "hlight", "asp", "c906", "c908"):
-            show_top5 = "shl_show_top5(foutput, sess);"
-        else:
+        if board == "anole":
             show_top5 = "shl_ovx_show_top5(i, sess);"
+        else:
+            show_top5 = "shl_show_top5(foutput, sess);"
     postprocess_str = postprocess_str.replace("#_show_top5_stats_#", show_top5)
 
     free_anole_input_data = ""
     free_output_data = ""
     if board == "anole":
         free_anole_input_data = "free(input->data);"
         free_output_data = "free(output->data);"
-    if board in ("light", "hlight", "asp", "c906", "c908"):
+    if board in ("th1520", "hth1520", "c906", "rvm", "c908", "c920"):
         free_output_data = "shl_ref_tensor_transform_free_f32(foutput);\n"
-        if board in ("c906", "c908"):
+        if board in ("c906", "rvm", "c908", "c920"):
             free_output_data += " " * 8 + "if (!output->is_const) {\n"
-            free_output_data += " " * 12 + "free(output->data);\n"
+            free_output_data += " " * 12 + "shl_mem_free(output->data);\n"
             free_output_data += " " * 8 + "}"
     postprocess_str = postprocess_str.replace("#_free_anole_input_data_#", free_anole_input_data)
     postprocess_str = postprocess_str.replace("#_free_output_data_#", free_output_data)
 
     save_output = ""
     if "save" in postprocess:
         save_output = "char filename[FILE_LENGTH] = {0};\n"
@@ -297,31 +287,42 @@
         save_output += (
             " " * 8 + "shape2string(output->dim, output->dim_count, shape, SHAPE_LENGHT);\n"
         )
         save_output += (
             " " * 8
             + 'snprintf(filename, FILE_LENGTH, "%s_output%u_%s.txt", filename_prefix, i, shape);\n'
         )
-        if board in ("light", "hlight", "asp", "c906", "c908"):
+        if board == "anole":
+            save_output += " " * 8 + "shl_ovx_save_output(i, filename, sess);\n"
+        else:
             save_output += " " * 8 + "int output_size = csinn_tensor_size(foutput);\n"
             save_output += (
                 " " * 8 + "save_data_to_file(filename, (float*)foutput->data, output_size);\n"
             )
-        else:
-            save_output += " " * 8 + "shl_ovx_save_output(i, filename, sess);\n"
     postprocess_str = postprocess_str.replace("#_save_output_stats_#", save_output)
     code_str = code_str.replace("#_hhb_postprocess_def_#", postprocess_str)
 
+    if board == "c920":
+        if "save" in postprocess:
+            code_str = code_str.replace("#_hhb_c920_postprocess_#", "1")
+        else:
+            code_str = code_str.replace("#_hhb_c920_postprocess_#", "0")
+
     #######################################################################
     #
     # Main Codegen
     #
     code_str = code_str.replace("#_input_num#", str(len(input_shape)))
     code_str = code_str.replace("#_output_num#", str(len(output_shape)))
 
+    hhb_gen_register = ""
+    if hhb_gen:
+        hhb_gen_register = "void hhb_gen_register(); hhb_gen_register();"
+    code_str = code_str.replace("#_hhb_gen_register_#", hhb_gen_register)
+
     aligned_buffer_stats = ""
     if input_memory_type and (1 in input_memory_type):
         aligned_buffer_stats += "void *input_aligned[input_num];\n"
         aligned_buffer_stats += " " * 4 + "for (i = 0; i < input_num; i++) {\n"
         aligned_buffer_stats += (
             " " * 8
             + "input_size[i] = csinn_tensor_byte_size(((struct csinn_session *)sess)->input[i]);\n"
@@ -329,29 +330,42 @@
         aligned_buffer_stats += (
             " " * 8 + "input_aligned[i] = shl_mem_alloc_aligned(input_size[i], 0);\n"
         )
         aligned_buffer_stats += " " * 4 + "}\n"
     code_str = code_str.replace("#_aligned_buffer_stats_#", aligned_buffer_stats)
 
     aligned_buffer_copy = ""
+    aligned_buffer_free = ""
     if input_memory_type:
         for i in range(len(input_shape)):
             if input_memory_type[i] == 1:  # cpu aligned
                 if i != 0:
                     aligned_buffer_copy += " " * 8
                 aligned_buffer_copy += (
                     "memcpy(input_aligned["
                     + str(i)
                     + "], input["
                     + str(i)
                     + "], input_size["
                     + str(i)
                     + "]);\n"
                 )
+                aligned_buffer_copy += " " * 8
+                aligned_buffer_copy += (
+                    "input_tensors[" + str(i) + "]->data = input_aligned[" + str(i) + "];\n"
+                )
+                aligned_buffer_free += "shl_mem_free(input_aligned[j]);"
+            else:
+                if i != 0:
+                    aligned_buffer_copy += " " * 8
+                aligned_buffer_copy += (
+                    "input_tensors[" + str(i) + "]->data = input[" + str(i) + "];\n"
+                )
     code_str = code_str.replace("#_aligned_buffer_copy_#", aligned_buffer_copy)
+    code_str = code_str.replace("#_aligned_buffer_free_#", aligned_buffer_free)
 
     get_input_data_stats = ""
     if without_preprocess:
         get_input_data_stats += "if (get_file_type(data_path[i * input_num + j]) != FILE_BIN) {\n"
         get_input_data_stats += (
             " " * 16
             + 'printf("Please input binary files, since you compiled the model without preprocess.\\n");\n'
@@ -388,32 +402,143 @@
         get_input_data_stats += " " * 12 + "}\n"
         get_input_data_stats += " " * 12 + "inputf[j] = img->data;\n"
         get_input_data_stats += " " * 12 + "free_image_data(img);\n"
     code_str = code_str.replace("#_get_input_data_stats_#", get_input_data_stats)
 
     run_csinn_stats_anole = ""
     run_csinn_stats_thead = ""
-    for i in range(len(input_shape)):
-        if input_memory_type and input_memory_type[i] == 1:
-            run_csinn_stats_anole += "input_aligned[" + str(i) + "], "
+    if dynamic_shape:
+        run_csinn_stats_anole += """
+    if (option->input_number) {
+        for (int i = 0; i < option->input_number; i++) {
+            input_tensors[i] = csinn_alloc_tensor(NULL);
+            input_tensors[i]->dim_count = option->input_shape[i].dim_count;
+            for (int j = 0; j < input_tensors[i]->dim_count; j++) {
+                input_tensors[i]->dim[j] = option->input_shape[i].dims[j];
+            }
+            csinn_update_input(i, input_tensors[i], sess);
+        }
+    } else {
+        printf("Use --input-shape to set input shape\\n");
+        return 0;
+    }
+        """
+    else:
+        for i in range(len(input_shape)):
+            if i > 0:
+                run_csinn_stats_anole += "    "
+            run_csinn_stats_anole += f"input_tensors[{i}] = csinn_alloc_tensor(NULL);\n"
+            run_csinn_stats_anole += f"    input_tensors[{i}]->dim_count = {len(input_shape[i])};\n"
+            for j, s in enumerate(input_shape[i]):
+                run_csinn_stats_anole += f"    input_tensors[{i}]->dim[{j}] = {s};\n"
+
+            run_csinn_stats_thead += "input[" + str(i) + "], "
+    code_str = code_str.replace("#_tensor_shape_#", run_csinn_stats_anole)
+
+    return code_str
+
+
+def main_c_codegen(
+    codegen_obj: HHBBoardQnnCodegenIR,
+    input_shape,
+    output_shape,
+    board,
+    output_path,
+    postprocess="top5",
+    model_save="run_only",
+    without_preprocess=False,
+    preprocess_params=None,
+    multithread=False,
+    input_memory_type=None,
+    q_scheme=None,
+    dynamic_shape=None,
+    hhb_gen=False,
+):
+    """Generate the main.c file"""
+
+    execute_path = get_execute_path()
+    if board == "anole":
+        if multithread:
+            main_file = os.path.join(execute_path, "config", "anole_multithread.tp")
+        else:
+            main_file = os.path.join(execute_path, "config", "anole.tp")
+    elif board in ("th1520", "hth1520"):
+        main_file = os.path.join(execute_path, "config", "th1520.tp")
+    elif board in ("c906", "rvm", "c908"):
+        if dynamic_shape:
+            main_file = os.path.join(execute_path, "config", "c906_cmdline.tp")
         else:
-            run_csinn_stats_anole += "input[" + str(i) + "], "
-        run_csinn_stats_thead += "input[" + str(i) + "], "
-    code_str = code_str.replace("#_anole_value_pass#", run_csinn_stats_anole)
-
-    if board == "c860":
-        for i in range(len(output_shape)):
-            run_csinn_stats_thead += "output[" + str(i) + "], "
-        code_str = code_str.replace("#_thead_value_pass#", run_csinn_stats_thead)
+            main_file = os.path.join(execute_path, "config", "c906.tp")
+    elif board == "c920":
+        main_file = os.path.join(execute_path, "config", "c920.tp")
+    else:
+        without_preprocess = True
+        main_file = os.path.join(execute_path, "config", "x86_ref.tp")
+
+    code_str = entry_c_codegen(
+        codegen_obj,
+        input_shape,
+        output_shape,
+        board,
+        output_path,
+        main_file,
+        postprocess,
+        model_save,
+        without_preprocess,
+        preprocess_params,
+        multithread,
+        input_memory_type,
+        q_scheme,
+        dynamic_shape,
+        hhb_gen,
+    )
 
     logger.info("save main souce to %s", os.path.join(output_path, codegen_obj.main_source_name))
     with open(os.path.join(output_path, codegen_obj.main_source_name), "w") as f:
         f.write(code_str)
 
 
+def jit_c_codegen(
+    codegen_obj: HHBBoardQnnCodegenIR,
+    input_shape,
+    output_shape,
+    board,
+    output_path,
+    preprocess_params=None,
+    q_scheme=None,
+):
+    """Generate the main.c file"""
+
+    execute_path = get_execute_path()
+    if board in ("th1520", "hth1520", "c920"):
+        main_file = os.path.join(execute_path, "config", "th1520_jit.tp")
+
+    code_str = entry_c_codegen(
+        codegen_obj,
+        input_shape,
+        output_shape,
+        board,
+        output_path,
+        main_file,
+        "top5",
+        "run_only",
+        True,
+        preprocess_params,
+        False,
+        None,
+        q_scheme,
+        None,
+        False,
+    )
+
+    logger.info("save jit souce to %s", os.path.join(output_path, "jit.c"))
+    with open(os.path.join(output_path, "jit.c"), "w") as f:
+        f.write(code_str)
+
+
 def _preprocess_macro_define(preprocess_params, preprocess_str):
     if len(preprocess_params["data_mean"]) not in (1, 3):
         raise HHBException(
             "do not know how to deal with mean values:{}".format(preprocess_params["data_mean"])
         )
     if preprocess_params["add_preprocess_node"]:
         preprocess_params["data_mean"] = [0, 0, 0]
@@ -458,71 +583,24 @@
 
         op_name = call.op.name
         if op_name == "qnn.csi.conv2d":
             in_shape = list(call.type_args[0].concrete_shape)
             kernel_shape = list(call.type_args[1].concrete_shape)
             if call.attrs.groups > 1:
                 op_name = "group_conv2d"
-                if call.attrs.out_layout == "NHWC":
-                    # for i805 NHWC layout
-                    if call.attrs.groups == in_shape[3] and kernel_shape[0] == 1:
-                        op_name = "depthwise_conv2d"
-                elif call.attrs.out_layout == "NCHW":
+                if call.attrs.out_layout == "NCHW":
                     if call.attrs.groups == in_shape[0] and kernel_shape[1] == 1:
                         op_name = "depthwise_conv2d"
         if op_name not in self.layer_kinds:
             self.layer_kinds.append(op_name)
 
     def get_op_kinds(self):
         return self.layer_kinds
 
 
-def generate_func_map(model, board, dump_file_path):
-    def get_register_func(i805h_path):
-        import re
-
-        register_func = {}
-        with open(i805h_path, "r") as f:
-            for line in f:
-                match_obj = re.match(r"int shl_i805_(.*)_u8", line)
-                if match_obj:
-                    func_name = match_obj.group(1)
-                    if "init" in func_name:
-                        func_name = func_name[:-5]
-                    if func_name not in register_func:
-                        register_func[func_name] = func_name
-        return register_func
-
-    op_kinds = VisitLayers(model["main"]).get_op_kinds()
-    execute_path = get_execute_path()
-    i805h_path = os.path.join(execute_path, "../../install_nn2/include/shl_i805.h")
-    register_funcs = get_register_func(i805h_path)
-    func_file = os.path.join(execute_path, "config", "cb_map.tp")
-    with open(func_file, "r") as f:
-        code_str = f.read()
-    repleased_str = ""
-    optimized_stwich_str = "\t\tcase CSINN_OP_{}:\n\t\t\treturn shl_#TARGET_{}_u8;\n\t\t\tbreak;\n"
-    ref_stwich_str = "\t\tcase CSINN_OP_{}:\n\t\t\treturn shl_ref_{}_quant;\n\t\t\tbreak;\n"
-    mem_ops = ["transpose", "resahpe", "squeeze"]
-    for op in op_kinds:
-        kind = op.split(".")[-1]
-        if kind in register_funcs:
-            repleased_str += optimized_stwich_str.format(kind.upper(), register_funcs[kind])
-        else:
-            tmp_str = ref_stwich_str.format(kind.upper(), kind.lower())
-            if kind in mem_ops:
-                tmp_str = tmp_str.replace("_quant", "")
-            repleased_str += tmp_str
-
-    code_str = code_str.replace("#OP_CASE", repleased_str)
-    code_str = code_str.replace("#TARGET", board)
-    with open(dump_file_path, "w+") as f:
-        f.write(code_str)
-
-
 def generate_c906_cb_reg(model, board, dump_file_path, q_scheme):
 
     c906_cb_reg_map = {
         "abs": {
             "CSINN_DTYPE_FLOAT16": ["CSINN_OP_ABS", "NULL", "shl_c906_abs_fp16", "shl_gref_abs"],
             "CSINN_DTYPE_FLOAT32": ["CSINN_OP_ABS", "NULL", "shl_c906_abs_f32", "shl_gref_abs"],
         },
@@ -830,15 +908,15 @@
         },
     }
 
     op_kinds = VisitLayers(model["main"]).get_op_kinds()
     if "qnn.csi.conv2d" in op_kinds:
         op_kinds.append("depthwise_conv2d")
     execute_path = get_execute_path()
-    func_file = os.path.join(execute_path, "config", "cb_reg.tp")
+    func_file = os.path.join(execute_path, "config", "reg_rewrite", "c906.tp")
     with open(func_file, "r") as f:
         code_str = f.read()
     cb_op_str = ""
     cb_op_est_str = ""
     reg_906 = "\tshl_c906_reg_op({}, {}, {}, {});\n"
     est_906 = "\tshl_c906_reg_op_est({}, {}, {});\n"
     if q_scheme == "unset":
@@ -1218,18 +1296,18 @@
     binary_graph_section = False
     graph_info = False
 
     if model_save == "save_only":
         model_params_section = False
         binary_graph_section = True
 
-    if board == "light":
+    if board == "th1520":
         graph_info = True
 
-    if board not in ["light", "light_new"]:
+    if board not in ["th1520"]:
         model_params_section = True
         binary_graph_section = False
 
     bm_list = []
 
     if binary_graph_section:
         bm_list.append(["0", "graph", os.path.join(output_path, "csi.mbs.bin")])
```

## hhb/core/common.py

```diff
@@ -20,14 +20,15 @@
 import functools
 import argparse
 import re
 import yaml
 import logging
 import collections
 import sys
+import subprocess
 
 import numpy as np
 
 
 ArgInfo = collections.namedtuple("_ArgInfo", ["name", "choices", "default_value", "help"])
 
 HHB_REGISTERED_PARSER = []
@@ -36,24 +37,48 @@
 ALL_ARGUMENTS_DESC = {}
 ARGS_DEST_TO_OPTIONS_STRING = {}
 logger = logging.getLogger("HHB")
 
 
 def hhb_version():
     """Version information"""
-    __version__ = "2.0.20"
-    __build_time__ = "20220822"
+    __version__ = "2.2.35"
+    __build_time__ = "20230330"
     return "HHB version: " + __version__ + ", build " + __build_time__
 
 
 def hhb_exit(message):
     logger.error(message)
     sys.exit()
 
 
+def parse_mean(mean):
+    """Parse the mean value .
+
+    Parameters
+    ----------
+    mean : str or list
+        The provided mean value
+
+    Returns
+    -------
+    mean_list : list[int]
+        The mean list
+    """
+    if isinstance(mean, list):
+        return mean
+    if "," in mean:
+        mean = mean.replace(",", " ")
+    mean_list = mean.strip().split(" ")
+    mean_list = list([float(n) for n in mean_list if n])
+    # if len(mean_list) == 1:
+    #     mean_list = mean_list * 3
+    return mean_list
+
+
 class HHBException(Exception):
     """HHB Exception"""
 
 
 class AttributeDict(dict):
     def __init__(self, **kwargs):
         super(AttributeDict, self).__init__()
@@ -161,39 +186,71 @@
     if directory is None:
         directory = "hhb_out"
     if not os.path.exists(directory):
         os.makedirs(directory)
     return directory
 
 
+def ensure_compiler(command):
+    """Call compiler command, and return version
+
+    Parameters
+    ----------
+
+    command : str
+        command to call
+    """
+    cmd_line = [command, "-v"]
+    cmd_output = subprocess.check_output(cmd_line, stderr=subprocess.STDOUT)
+    output_str = cmd_output.decode()
+    if "command not found" in output_str:
+        raise HHBException("Cannot find compiler.\n{}".format(output_str))
+    # only for gcc
+    version_index = output_str.find("gcc Toolchain") + 15
+    version_str = output_str[version_index : version_index + 3]
+    if version_str:
+        return float(version_str)
+    return 0
+
+
 def get_target(board):
     """Get the target info accorrding to the board type."""
     if board == "anole":
         target = "c -device=anole"
-    elif board == "light":
-        target = "c -device=light"
-    elif board == "hlight":
-        target = "c -device=hlight"
-    elif board == "asp":
-        target = "c -device=asp"
-    elif board == "i805":
-        target = "c -device=i805"
-    elif board == "c860":
-        target = "c -device=c860"
+    elif board == "th1520":
+        target = "c -device=th1520"
+    elif board == "hth1520":
+        target = "c -device=hth1520"
+    elif board == "e907":
+        target = "c -device=e907"
     elif board == "c906":
         target = "c -device=c906"
+    elif board == "rvm":
+        target = "c -device=rvm"
     elif board == "c908":
         target = "c -device=c908"
+    elif board == "c920":
+        target = "c -device=c920"
     elif board == "x86_ref":
         target = "c"
     return target
 
 
-def print_top5(value, output_name, shape):
-    """Print the top5 infomation"""
+def print_top5(value, output_name=None, shape=None):
+    """Print the top5 infomation
+
+    Parameters
+    ----------
+    value : numpy.ndarray
+        The data need to be print.
+    output_name : str
+        The name of value.
+    shape : List[int]
+        The original shape of value.
+    """
     if not isinstance(value, np.ndarray):
         raise HHBException("Unsupport for {}, please input ndarray".format(type(value)))
     len_t = np.prod(value.size)
     pre = np.reshape(value, [len_t])
     ind = np.argsort(pre)
     if len_t > 5:
         ind = ind[len_t - 5 :]
@@ -208,15 +265,27 @@
     print(f"The var_value of output: {pre.var():.6f}")
     print(f"====== index:{output_name}, shape:{shape}, top5: ======")
     for (i, v) in zip(ind, value):
         print("{}:{}".format(i, v))
 
 
 def convert_invalid_symbol(input_str):
-    """Convert invalid symbols in string into '_' """
+    """Convert invalid symbols in string into '_'
+
+    Parameters
+    ----------
+    input_str : str
+        Input string
+
+    Returns
+    -------
+    new_str : str
+        Modified string.
+
+    """
     invalid_symbol = r"[/:\s\.]"
     new_str = re.sub(invalid_symbol, "_", input_str)
     return new_str
 
 
 def find_index(data, item):
     """Find item index in data
```

## hhb/core/data_process.py

```diff
@@ -17,14 +17,15 @@
 # pylint: disable=invalid-name, unused-argument, too-many-lines, import-outside-toplevel
 # pylint: disable=no-else-return, inconsistent-return-statements, no-else-raise
 """ Preprocess data helper """
 import os
 import glob
 import functools
 import logging
+from pathlib import Path
 
 import cv2
 import numpy as np
 
 
 # pylint: disable=invalid-name
 logger = logging.getLogger("HHB")
@@ -63,23 +64,23 @@
         data = np.transpose(data, (2, 0, 1))
         data = np.expand_dims(data, axis=0)
 
     return data
 
 
 class PathType(object):
-    """Denote the kind of path. """
+    """Denote the kind of path."""
 
     NOTEXISTS = 0
     FILE = 1
     DIR = 2
 
 
 def check_data(func):
-    """The wrapper for checking whether the data field is empty. """
+    """The wrapper for checking whether the data field is empty."""
 
     @functools.wraps(func)
     def wrapper_inner(*args, **kwargs):
         self = args[0]
         if len(self.data) == 0:
             raise ValueError("Please load images first.")
         value = func(*args, **kwargs)
@@ -99,43 +100,43 @@
     @classmethod
     def get_channel_idx(cls, layout_type):
         channel_index = {cls.CHW: 0, cls.HWC: 2, cls.NCHW: 1, cls.NHWC: 3}
         return channel_index[layout_type]
 
     @classmethod
     def get_type2str(cls, layout_type):
-        """ Convert layout type into str """
+        """Convert layout type into str"""
         if layout_type == cls.NCHW:
             return "NCHW"
         elif layout_type == cls.NHWC:
             return "NHWC"
         elif layout_type == cls.HWC:
             return "HWC"
         elif layout_type == cls.CHW:
             return "CHW"
         else:
             raise ValueError("Unsupport for the layout of data.")
 
     @classmethod
     def get_str2type(cls, layout_str):
-        """ Convert str into layout type """
+        """Convert str into layout type"""
         if layout_str == "NCHW":
             return cls.NCHW
         elif layout_str == "NHWC":
             return cls.NHWC
         elif layout_str == "HWC":
             return cls.HWC
         elif layout_str == "CHW":
             return cls.CHW
         else:
             raise ValueError("Unsupport for the layout str of data.")
 
     @classmethod
     def get_data_layout(cls, shape):
-        """ Get the data layout"""
+        """Get the data layout"""
         assert shape
         assert len(shape) == 4, "The dim of data should be 4."
         curr_shape = shape[1:]
         if 1 in curr_shape:
             index = curr_shape.index(1)
         elif 3 in curr_shape:
             index = curr_shape.index(3)
@@ -222,14 +223,16 @@
         # support for directory .txt or .npz
         path_type = self._check_path(path)
         img_path_list = list()
         if path_type == PathType.DIR:
             img_path_list += glob.glob(os.path.join(path, "*.jpg"))
             img_path_list += glob.glob(os.path.join(path, "*.png"))
             img_path_list += glob.glob(os.path.join(path, "*.JPEG"))
+
+            img_path_list += glob.glob(os.path.join(path, "*.npz"))
         elif path_type == PathType.FILE:
             suffix = path.strip().split(".")[-1].lower()
             if suffix == "txt":
                 with open(path, "r") as f:
                     for line in f.readlines():
                         line_s = line.strip()
                         if line_s and self._check_path(line_s) == PathType.FILE:
@@ -241,14 +244,21 @@
             else:
                 raise NotImplementedError(
                     "Unsupport for {}, "
                     "please pass valid files(.txt .npz .jpg .png .JPEG).".format(path)
                 )
         else:
             raise FileNotFoundError(f"{path} is invalid. Please pass valid path.")
+
+        for p in img_path_list:
+            suffix = p.strip().split(".")[-1].lower()
+            if suffix not in ("png", "jpg", "jpeg", "npz"):
+                raise ValueError("Only support for files(.png .jpg .jpeg adn .npz)")
+        if not img_path_list:
+            raise ValueError("There is empty dataset.")
         return img_path_list
 
     def load_dataset(self, path, gray=False):
         """load multi-images. Only support for directory and .txt
 
         Parameters
         ----------
@@ -262,14 +272,50 @@
         # support for directory .txt or .npz
         img_path_list = self.get_file_list(path)
         if not img_path_list:
             raise ValueError("there is no data...")
         for img_path in img_path_list:
             self.load_image(img_path, gray)
 
+    def load(self, path, gray=False):
+        """load images.
+
+        Parameters
+        ----------
+        path : str
+            The path of images: support for .jpg, .png, .jpeg, .txt, dir.
+        gray : bool
+            If gray is False, load image with rgb mode;
+            If gray is True, load image with gray mode while it is gray image.
+        """
+        if isinstance(path, (list, tuple)):
+            for p in path:
+                self.load(p, gray=gray)
+        elif isinstance(path, str):
+            path_type = self._check_path(path)
+            if path_type == PathType.DIR or (
+                path_type == PathType.FILE and path.strip().split(".")[-1].lower() == "txt"
+            ):
+                self.load_dataset(path, gray=gray)
+            elif path_type == PathType.FILE:
+                suffix = path.strip().split(".")[-1].lower()
+                if suffix == "txt":
+                    self.load_dataset(path, gray=gray)
+                elif suffix in ("png", "jpg", "jpeg"):
+                    self.load_image(path, gray=gray)
+                else:
+                    raise NotImplementedError(
+                        "Unsupport for {}, "
+                        "please pass valid files(.txt .jpg .png .JPEG or dir).".format(path)
+                    )
+            else:
+                raise FileNotFoundError("Path does not exist: {}".format(path))
+        else:
+            raise ValueError("Error data type: {}".format(type(path)))
+
     @check_data
     def sub_mean(self, mean_val=None):
         """Sub mean value for loaded dataset.
 
         Parameters
         ----------
         mean_val: int or float or list or tuple or numpy.ndarray
@@ -509,7 +555,8 @@
         for idx, d in enumerate(self.data):
             self.data[idx] = np.expand_dims(d, axis=0)
 
     @check_data
     def data_clear(self):
         self.data.clear()
         self.layout = DataLayout.HWC
+        self.origin_filenames.clear()
```

## hhb/core/frontend_manage.py

```diff
@@ -26,14 +26,16 @@
 import logging
 import sys
 from pathlib import Path
 
 import tvm
 from tvm import relay
 from tvm.relay import expr as _expr
+from tvm.relay.quantize.quantize_hhb import _bind_params
+from tvm.relay import transform
 from tvm.driver.tvmc.frontends import Frontend
 from tvm.driver.tvmc.frontends import KerasFrontend
 from tvm.driver.tvmc.frontends import OnnxFrontend
 from tvm.driver.tvmc.frontends import TensorflowFrontend
 from tvm.driver.tvmc.frontends import TFLiteFrontend
 from tvm.driver.tvmc.frontends import PyTorchFrontend
 
@@ -61,23 +63,23 @@
         new_k = convert_invalid_symbol(k)
         params[new_k] = params.pop(k)
 
     return mod, params
 
 
 class HHBKerasFrontend(KerasFrontend):
-    """ Keras frontend for HHB. """
+    """Keras frontend for HHB."""
 
     def load(self, path, input_name=None, input_shape=None, output_name=None):
         keras_path = path[0]
         return super().load(keras_path)
 
 
 class HHBOnnxFrontend(OnnxFrontend):
-    """ ONNX frontend for HHB. """
+    """ONNX frontend for HHB."""
 
     def load(self, path, input_name=None, input_shape=None, output_name=None):
         onnx_path = path[0]
         if (not input_name) and (not input_shape) and (not output_name):
             return super().load(onnx_path)
         import onnx
 
@@ -89,15 +91,15 @@
         for idx, name in enumerate(input_name):
             input_dict[name] = input_shape[idx]
         logger.info("Parse Onnx model and convert into Relay IR.")
         return relay.frontend.from_onnx(onnx_model, input_dict)
 
 
 class HHBTensorflowFrontend(TensorflowFrontend):
-    """ Tensorflow frontend for HHB. """
+    """Tensorflow frontend for HHB."""
 
     def load(self, path, input_name=None, input_shape=None, output_name=None):
         pb_path = path[0]
         if (not input_name) and (not input_shape) and (not output_name):
             return super().load(pb_path)
         import tensorflow as tf
 
@@ -129,15 +131,15 @@
         logger.info("Parse Tensorflow model and convert into Relay IR.")
         return relay.frontend.from_tensorflow(
             graph_def, layout="NCHW", shape=input_dict, outputs=output_name, input_layout="NCHW"
         )
 
 
 class HHBTFLiteFrontend(TFLiteFrontend):
-    """ TFLite frontend for HHB. """
+    """TFLite frontend for HHB."""
 
     def load(self, path, input_name=None, input_shape=None, output_name=None):
         tflite_path = path[0]
         # pylint: disable=C0415
         import tflite.Model as model
 
         with open(tflite_path, "rb") as tf_graph:
@@ -149,55 +151,60 @@
         except AttributeError:
             tflite_model = model.GetRootAsModel(content, 0)
 
         try:
             version = tflite_model.Version()
             logger.debug("tflite version %s", version)
         except Exception:
-            raise TVMCException("input file not tflite")
+            raise HHBException("input file not tflite")
 
         if version != 3:
-            raise TVMCException("input file not tflite version 3")
+            raise HHBException("input file not tflite version 3")
 
         logger.debug("tflite_input_type")
         if input_shape is None:
             shape_dict, dtype_dict = TFLiteFrontend._input_type(tflite_model)
         else:
             shape_dict = {name: shape for name, shape in zip(input_name, input_shape)}
             dtype_dict = {name: "float32" for name in input_name}
 
+        for k, v in shape_dict.items():
+            if len(v) == 4:
+                # convert to NCHW
+                shape_dict[k][1], shape_dict[k][3] = shape_dict[k][3], shape_dict[k][1]
+
         logger.debug("parse TFLite model and convert into Relay computation graph")
         target_layout = "NCHW"
         mod, params = relay.frontend.from_tflite_to_hhb(
             tflite_model, shape_dict, dtype_dict, target_layout, output_name
         )
         return mod, params
 
 
 class HHBPyTorchFrontend(PyTorchFrontend):
-    """ PyTorch frontend for HHB. """
+    """PyTorch frontend for HHB."""
 
     def load(self, path, input_name=None, input_shape=None, output_name=None):
         pytorch_path = path[0]
         return super().load(pytorch_path)
 
 
 class HHBCaffeFrontend(Frontend):
-    """ Caffe frontend for HHB. """
+    """Caffe frontend for HHB."""
 
     @staticmethod
     def name():
         return "caffe"
 
     @staticmethod
     def suffixes():
         return ["prototxt", "caffemodel"]
 
     def _check_and_get_caffemodel(self, path):
-        """ Check the imported model file whether satisfy the Caffe framework. """
+        """Check the imported model file whether satisfy the Caffe framework."""
         if isinstance(path, (list, tuple)) and len(path) == 2:
             from google.protobuf import text_format
             import tvm.relay.frontend.caffe_pb2 as pb
 
             prototxt_net = pb.NetParameter()
             caffemodel_net = pb.NetParameter()
 
@@ -250,68 +257,21 @@
         logger.info("Parse Caffe model and convert into Relay IR.")
         mod, params, _ = relay.frontend.from_caffe(
             caffemodel_net, prototxt_net, shape_dict, dtype_dict
         )
         return mod, params
 
 
-class HHBKaldiFrontend(Frontend):
-    """ Kaldi frontend for HHB. """
-
-    @staticmethod
-    def name():
-        return "kaldi"
-
-    @staticmethod
-    def suffixes():
-        return ["txt"]
-
-    def _check_and_get_kaldimodel(self, path):
-        """ Check the imported model file whether satisfy the kaldi framework. """
-        if isinstance(path, (list, tuple)) and len(path) == 1:
-            from tvm.relay.frontend.kaldi_parse import KaldiLoader
-
-            try:
-                return relay.frontend.KaldiLoader(path[0]).load()
-            except Exception:
-                sys.stderr.write("Please input valid kaldi file: .txt\n")
-                sys.exit(-1)
-        raise HHBException("Please input valid kaldi file: .txt\n")
-
-    def load(self, path, input_name=None, input_shape=None, output_name=None):
-        kaldi_net = self._check_and_get_kaldimodel(path)
-
-        shape_dict = {}
-        dtype_dict = {}
-        if input_name and input_shape:
-            assert len(input_name) == 1, f"only need single input name, but get {input_name}"
-            assert len(input_shape) == 1, f"only need single input shape, but get {input_shape}"
-            shape_dict[input_name[0]] = input_shape[0]
-            dtype_dict[input_name[0]] = "float32"
-        else:
-            layer = kaldi_net[0]
-            if layer["token"] == "AffineTransform":
-                iname = "input"
-                shape_dict[iname] = list([1, layer["size_settings"][1]])
-                dtype_dict[iname] = "float32"
-            else:
-                raise HHBException("Please input 'input_name' and 'input_shape'.")
-        logger.debug("Parse Kaldi model and convert into Relay IR.")
-        mod, params = relay.frontend.from_kaldi(kaldi_net, shape_dict, dtype_dict)
-        return mod, params
-
-
 ALL_HHB_FRONTENDS = [
     HHBKerasFrontend,
     HHBOnnxFrontend,
     HHBTensorflowFrontend,
     HHBTFLiteFrontend,
     HHBPyTorchFrontend,
     HHBCaffeFrontend,
-    HHBKaldiFrontend,
 ]
 
 
 def get_frontend_names():
     """Return the names of all supported frontends
 
     Returns
@@ -395,15 +355,15 @@
 
 
 def import_model(path, model_format=None, input_name=None, input_shape=None, output_name=None):
     """Import a model from a supported framework into relay ir.
 
     Parameters
     ----------
-    path : list[str]
+    path : list[str] or str
         Path to a model file. There may be two files(.caffemodel, .prototxt) for Caffe model
     model_format : str, optional
         A string representing input model format
     input_name : list[str], optional
         The names of input node in the graph
     input_shape : list[list[int]], optional
         The shape of input node in the graph
@@ -413,21 +373,52 @@
     Returns
     -------
     mod : tvm.IRModule
         The relay module for compilation
     params : dict of str to tvm.nd.NDArray
         The parameter dict to be used by relay
     """
+    if isinstance(path, str):
+        path = [path]
     if model_format is not None:
         frontend = get_frontend_by_name(model_format)
     else:
         frontend = guess_frontend(path)
     if input_name and input_shape:
         assert len(input_name) == len(
             input_shape
         ), "The length of \
                 input_name must be equal to that of input_shape."
     mod, params = frontend.load(path, input_name, input_shape, output_name)
     mod = relay.transform.InferType()(mod)
     mod, params = remove_invalid_symbol(mod, params)
 
     return mod, params
+
+
+def insert_preprocess_node(mod, params, data_mean, data_scale):
+    """Insert preprocess nodes into the head of model.
+
+    Parameters
+    ----------
+    mod : tvm.IRModule
+        The relay module for compilation
+    params : dict of str to tvm.nd.NDArray
+        The parameter dict to be used by relay
+    data_mean : List or Tuple
+        The mean values
+    data_scale : float
+        The scale values
+
+    Returns
+    -------
+    mod : tvm.IRModule
+        The modified module
+    params : dict of str to tvm.nd.NDArray
+        The modified parameter dict.
+    """
+    if params:
+        mod["main"] = _bind_params(mod["main"], params)
+        params = None
+    mod = transform.AddPreprocessNode(data_mean, data_scale)(mod)
+
+    return mod, params
```

## hhb/core/hhbir_manage.py

```diff
@@ -12,19 +12,21 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Manage HHB IR"""
 import os
+import sys
 import logging
 from abc import ABC
 from abc import abstractmethod
 import yaml
 import shutil
+import glob
 
 import tvm
 from tvm import relay
 from tvm import runtime
 from tvm.relay import quantize as qtz
 from tvm.relay.backend import executor_factory
 from tvm.contrib import graph_runtime
@@ -34,23 +36,24 @@
 
 from .common import (
     HHBException,
     get_target,
     hhb_ir_helper,
     HHB_IR,
     AttributeDict,
+    ensure_compiler,
 )
 
 
 # pylint: disable=invalid-name
 logger = logging.getLogger("HHB")
 
 
 def match_mod_params(mod, params):
-    """ The params of module's main function match the params dict."""
+    """The params of module's main function match the params dict."""
     if not params:
         return mod, params
     var_name_list = []
     for arg in mod["main"].params:
         if arg.name_hint not in var_name_list:
             var_name_list.append(arg.name_hint)
     params_new = {}
@@ -119,14 +122,28 @@
         if not os.path.exists(os.path.join(model_path, k)):
             raise HHBException("There is no {} in {}".format(k, model_path))
 
 
 def reorder_pixel_format(mod, params):
     """If original model's input data pixel format is rgb, then covert it to bgr,
     otherwise, then convert it to rgb.
+
+    Parameters
+    ----------
+    mod : tvm.IRModule
+        The relay module for compilation
+    params : dict of str to tvm.nd.NDArray
+        The parameter dict to be used by relay
+
+    Returns
+    -------
+    mod : tvm.IRModule
+        The modified relay module
+    params : dict of str to tvm.nd.NDArray
+        The modified parameter dict to be used by relay
     """
 
     class InnerVisitor(relay.ExprVisitor):
         """Counting the number of call"""
 
         def __init__(self):
             super(InnerVisitor, self).__init__()
@@ -189,33 +206,33 @@
     @abstractmethod
     def name():
         """IR name"""
 
     @staticmethod
     @abstractmethod
     def model_type():
-        """ IR type"""
+        """IR type"""
 
     @abstractmethod
     def load_model(self, model_path):
         """Load a model from a given path.
 
         Parameters
         ----------
         model_path : str
             Path to a tar file
         """
 
     @abstractmethod
     def convert(self):
-        """ Convert input module into current stage. """
+        """Convert input module into current stage."""
 
     @abstractmethod
     def save_model(self, model_path):
-        """Save current module into files. """
+        """Save current module into files."""
 
     def check_ir_type(self, model_path):
         files = os.listdir(model_path)
         res = True
         for f in self.all_included_filenames:
             if f not in files:
                 res = False
@@ -260,15 +277,15 @@
             params = tvm.relay.load_param_dict(f.read())
         self._mod, self._params = match_mod_params(mod, params)
 
     def convert(self):
         pass
 
     def save_model(self, model_path):
-        """Save current module into files. """
+        """Save current module into files."""
         assert self._mod, "Error: empty module."
         if not os.path.exists(model_path):
             raise HHBException("Directory {} is not exists".format(model_path))
         mod_path = os.path.join(model_path, self.mod_name)
         params_path = os.path.join(model_path, self.params_name)
 
         with open(mod_path, "w") as f:
@@ -302,14 +319,18 @@
     @staticmethod
     def model_type():
         return HHBIRType.QNN
 
     def get_model(self):
         return self._curr_mod, self._curr_params
 
+    def set_model(self, mod, params=None):
+        self._curr_mod = mod
+        self._curr_params = params
+
     def load_model(self, model_path):
         mod_path = os.path.join(model_path, self.mod_name)
         params_path = os.path.join(model_path, self.params_name)
         # ensure all needed files existing
         check_included_filename(model_path, self)
         with open(mod_path, "r") as f:
             self._curr_mod = tvm.parser.fromtext(f.read())
@@ -420,17 +441,18 @@
             not isinstance(input_module, (list, tuple))
             and not isinstance(input_module[0], tvm.ir.module.IRModule)
             and not isinstance(input_module[1], dict)
         ):
             raise HHBException("input_module should be [IRModule, dict]")
 
         target = "llvm"
+        model = relay.transform.DynamicToStatic()(input_module[0])
         with tvm.transform.PassContext(opt_level=opt_level):
             logger.info("building relay graph without quantization")
-            self._curr_module = relay.build(input_module[0], target=target, params=input_module[1])
+            self._curr_module = relay.build(model, target=target, params=input_module[1])
 
         (
             input_name_list,
             input_shape_list,
             input_dtype_list,
         ) = get_input_info_from_relay(input_module[0], input_module[1])
         output_shape_list, output_dtype_list = get_output_info_from_relay(
@@ -498,28 +520,25 @@
     def get_model(self):
         return self._curr_module
 
     def get_factory(self):
         return self._curr_factory
 
     def get_lib(self, output_dir):
-        contrib_dir = os.path.dirname(os.path.realpath(os.path.expanduser(__file__)))
-        contrib_dir = os.path.realpath(os.path.join(contrib_dir, ".."))
-        source_dir = os.path.join(contrib_dir, "..", "..")
-        include_path = os.path.join(source_dir, "install_nn2", "include")
-        ref_x86_dir0 = os.path.join(source_dir, "install_nn2", "lib")  # for source
-        ref_x86_dir1 = os.path.join(contrib_dir, "install_nn2", "lib")  # for package binary
+        _, shl_dir, _, _, _ = find_base_path()
+        include_path = os.path.join(shl_dir, "include")
+        ref_x86_dir = os.path.join(shl_dir, "lib")
+
         lib_path = os.path.join(output_dir, "quant.so")
         kwargs = {}
         kwargs["options"] = [
             "-O2",
             "-g",
             "-I" + include_path,
-            "-L" + ref_x86_dir0,
-            "-L" + ref_x86_dir1,
+            "-L" + ref_x86_dir,
             "-lshl_ref_x86",
         ]
         kwargs["cc"] = "gcc"
         lib = self.get_factory().get_lib()
         lib.export_library(lib_path, fcompile=False, workspace_dir=output_dir, **kwargs)
         lib = tvm.runtime.load_module(lib_path)
         return lib
@@ -591,21 +610,17 @@
             "input_dtype_list": input_dtype_list,
             "output_shape_list": output_shape_list,
             "output_dtype_list": output_dtype_list,
         }
 
     def save_model(self, model_path):
         """Save current module into files."""
-        contrib_dir = os.path.dirname(os.path.realpath(os.path.expanduser(__file__)))
-        source_dir = os.path.join(contrib_dir, "..", "..", "..")
-        include_path = os.path.join(source_dir, "install_nn2", "include")
-
         lib_path = os.path.join(model_path, self.lib_name)
         kwargs = {}
-        kwargs["options"] = ["-O0", "-g3", "-I" + include_path]
+        kwargs["options"] = ["-O0", "-g3"]
         logger.info("write lib to %s" % lib_path)
         self._curr_module.export_hhb_library(
             lib_path, fcompile=False, output_dir=model_path, **kwargs
         )
 
         info_path = os.path.join(model_path, self.info_file)
         logger.info("write extra info to %s" % info_path)
@@ -621,14 +636,15 @@
 class HHBBoardQnnCodegenIR(HHBIRBase):
     def __init__(self, without_preprocess=False):
         super().__init__()
         self.mod = None
         self.params_name = "model.params"
         self.graph_info_name = "graph_info.bin"
         self.lib_source_name = "model.c"
+        self.intrinsic_source_name = "intrinsic.c"
         self.main_source_name = "main.c"
         self.preprocess_source_name = "process.c"
         self.preprocess_header_name = "process.h"
         self.preio_source_name = "io.c"
         self.preio_header_name = "io.h"
 
         self.all_included_filenames.extend(
@@ -704,19 +720,34 @@
         )
         logger.debug(
             "Set the memory type of output tenosr as: {}".format(
                 device_config["output_memory_type"]
             )
         )
 
+        if device_config["ahead_of_time"] == "intrinsic":
+            with tvm.transform.PassContext(
+                opt_level=opt_level, config={"relay.ext.csinn.options": device_config}
+            ):
+                csinn_mod = csinn.partition_for_csinn(mod, params)
+                factory = relay.build(csinn_mod, target=target, params=params)
+
+            lib = factory.get_lib()
+            self._curr_module = lib
+            lib_path = os.path.join(output_path, self.intrinsic_source_name)
+
+            logger.info("write lib source code to %s", lib_path)
+            factory.export_library(lib_path, fcompile=fcompile)
+            device_config["ahead_of_time"] = "unset"
+
         with tvm.transform.PassContext(
             opt_level=opt_level, config={"relay.ext.csinn.options": device_config}
         ):
-            mod = csinn.partition_for_csinn(mod, params)
-            factory = relay.build(mod, target=target, params=params)
+            csinn_mod = csinn.partition_for_csinn(mod, params)
+            factory = relay.build(csinn_mod, target=target, params=params)
 
         lib = factory.get_lib()
         self._curr_module = lib
         lib_path = os.path.join(output_path, self.lib_source_name)
         logger.info("write lib source code to %s", lib_path)
         factory.export_library(lib_path, fcompile=fcompile)
 
@@ -730,55 +761,419 @@
         model_save="run_only",
         without_preprocess=False,
         preprocess_params=None,
         multithread=False,
         input_memory_type=None,
         q_scheme=None,
         codegen_config=None,
+        hhb_gen=False,
     ):
         from .codegen_manage import (
             main_c_codegen,
-            generate_func_map,
+            jit_c_codegen,
             generate_c906_cb_reg,
             generate_rvv_cb_reg,
         )
 
-        if board == "i805":
-            dump_file_path = os.path.join(output_path, "cb_map.c")
-            logger.info("write bc map code to %s", dump_file_path)
-            generate_func_map(self.mod, board, dump_file_path)
-            return
-        elif board == "c906" and codegen_config.dynamic_cb_reg:
+        if board == "c906" and codegen_config.dynamic_cb_reg:
             dump_file_path = os.path.join(output_path, "cb_reg.c")
             logger.info("write bc reg to %s", dump_file_path)
             opks = generate_c906_cb_reg(self.mod, board, dump_file_path, q_scheme)
             dump_file_path = os.path.join(output_path, "cb_rvv.c")
             logger.info("write bc rvv to %s", dump_file_path)
             opks = generate_rvv_cb_reg(False, dump_file_path, q_scheme, opks)
+        elif board in ("th1520", "hth1520", "c920"):
+            jit_c_codegen(
+                self, input_shape, output_shape, board, output_path, preprocess_params, q_scheme
+            )
 
         main_c_codegen(
             self,
             input_shape,
             output_shape,
             board,
             output_path,
             postprocess,
             model_save,
             without_preprocess,
             preprocess_params,
             multithread,
             input_memory_type,
             q_scheme,
+            codegen_config.dynamic_shape,
+            hhb_gen,
         )
 
         from .codegen_manage import package_sections
 
         package_sections(board, output_path, model_save)
 
 
+def base_dir_exists(dir):
+    found_dir = os.path.abspath(dir)
+    found_dir = os.path.join(found_dir, "install_nn2/include")
+    if os.path.exists(found_dir) and os.path.isdir(found_dir):
+        return found_dir
+    else:
+        return None
+
+
+def find_base_path():
+    if getattr(sys, "frozen", False) and hasattr(sys, "_MEIPASS"):
+        # for pyinstaller
+        exe_dir = os.path.dirname(os.path.realpath(sys.executable))
+    else:
+        # for source file
+        exe_dir = os.path.dirname(os.path.realpath(__file__))
+
+    source_dir = os.path.join(exe_dir, "..", "..", "..")
+    wheel_dir = os.path.join(exe_dir, "..")
+
+    if base_dir_exists(exe_dir):
+        # pyintaller
+        base_found = exe_dir
+        tvm_inc_dir = exe_dir + "/tvm/include/"
+        dlpack_inc_dir = exe_dir + "/tvm/include/dlpack/"
+        shl_dir = exe_dir + "/install_nn2/"
+        prebuilt_dir = exe_dir + "/prebuilt/"
+    elif base_dir_exists(source_dir):
+        # source code
+        base_found = source_dir
+        tvm_inc_dir = source_dir + "/include/"
+        dlpack_inc_dir = source_dir + "/3rdparty/dlpack/include/"
+        shl_dir = source_dir + "/install_nn2/"
+        prebuilt_dir = source_dir + "/thead/prebuilt/"
+    elif base_dir_exists(wheel_dir):
+        # wheel/pip
+        base_found = wheel_dir
+        tvm_inc_dir = wheel_dir + "/../tvm/include/"
+        dlpack_inc_dir = wheel_dir + "/../tvm/dlpack/include/"
+        shl_dir = wheel_dir + "/install_nn2/"
+        prebuilt_dir = wheel_dir + "/prebuilt/"
+    else:
+        raise HHBException("Cannot find the executable base dir.\n")
+
+    base_found = os.path.join(os.path.abspath(base_found), "")
+    shl_dir = os.path.join(os.path.abspath(shl_dir), "")
+    prebuilt_dir = os.path.join(os.path.abspath(prebuilt_dir), "")
+    tvm_inc_dir = os.path.join(os.path.abspath(tvm_inc_dir), "")
+    dlpack_inc_dir = os.path.join(os.path.abspath(dlpack_inc_dir), "")
+    return base_found, shl_dir, prebuilt_dir, tvm_inc_dir, dlpack_inc_dir
+
+
+@hhb_ir_helper
+class HHBBoardBuildRuntime:
+    def __init__(self, board, work_dir, intrinsic=False, link_lib="unset", android=False):
+        self.board = board
+        self.work_dir = work_dir
+        self.intrinsic = intrinsic
+        self.jit = False
+
+        self.source_name = []
+        self.runtime_name = ""
+        self.jit_name = ""
+
+        if board in ("th1520", "hth1520", "th1520_x86", "c920"):
+            self.jit = True
+
+        self.cflag = " -O2 -g "
+
+        if board in ("c906", "c908", "c920", "rvm", "th1520", "hth1520"):
+            self.compiler = "riscv64-unknown-linux-gnu-gcc"
+            # check compiler version
+            compiler_version = ensure_compiler(self.compiler)
+            if compiler_version < 2.6:
+                raise HHBException("Please upgrade compiler version.\n")
+
+            self.cflag += "-mabi=lp64d "
+        elif board in ("x86_ref", "th1520_x86"):
+            self.compiler = "gcc"
+        else:
+            raise HHBException("Unsupport platform build: {}.\n".format(board))
+
+        hhb_base_dir, shl_dir, prebuilt_dir, tvm_inc_dir, dlpack_dir = find_base_path()
+
+        logger.info("HHB base dir: %s", hhb_base_dir)
+
+        self.include_dir = " -I" + shl_dir + "include " + " -I" + dlpack_dir
+
+        self.include_dir += " -I" + tvm_inc_dir + " "
+
+        self.link_flag = " -Wl,--gc-sections -L " + shl_dir + "lib/ "
+        # reuse cflag in link, but no -march
+        self.link_flag += self.cflag
+
+        if board == "th1520":
+            self.link_flag += " -Wl,-unresolved-symbols=ignore-in-shared-libs "
+            if link_lib in ("unset", "shl_th1520"):
+                self.link_flag += " -lshl_th1520 "
+            elif link_lib == "shl_pnna":
+                self.link_flag += " -lshl_pnna "
+            else:
+                raise HHBException("Unsupport link {} for th1520.\n".format(link_lib))
+        elif board == "hth1520":
+            self.link_flag += " -Wl,-unresolved-symbols=ignore-in-shared-libs "
+            if link_lib in ("unset", "shl_th1520"):
+                self.link_flag += " -lshl_th1520 "
+            elif link_lib == "shl_pnna":
+                self.link_flag += " -lshl_pnna "
+            else:
+                raise HHBException("Unsupport link {} for th1520.\n".format(link_lib))
+        elif board == "th1520_x86":
+            self.link_flag += " -Wl,-unresolved-symbols=ignore-in-shared-libs "
+            self.link_flag += " -lshl_pnna_x86 "
+        elif board == "rvm":
+            self.link_flag += " -lshl_rvm -static "
+        elif board == "c906":
+            self.link_flag += " -lshl_c906 -static "
+            self.cflag += " -march=rv64gcv0p7_zfh_xtheadc "
+        elif board == "c908":
+            self.link_flag += " -lshl_c908 -static "
+        elif board == "c920":
+            if link_lib in ("unset", "shl_c920"):
+                self.link_flag += " -lshl_c920 -static "
+            elif link_lib == "shl_th1520":
+                self.link_flag += " -Wl,-unresolved-symbols=ignore-in-shared-libs "
+                self.link_flag += " -lshl_th1520 "
+            else:
+                raise HHBException("Unsupport link {} for c920.\n".format(link_lib))
+            self.cflag += " -march=rv64gcv0p7_zfh_xtheadc "
+        elif board == "x86_ref":
+            self.link_flag += " -lshl_ref_x86 "
+        else:
+            self.link_flag += " -lshl_rvv -static "
+
+        self.include_dir += " -I " + prebuilt_dir + "runtime/cmd_parse"
+        if android:
+            runtime_dir = " -L " + prebuilt_dir + "runtime/riscv_android"
+        else:
+            if board in ("c906", "c908", "c920", "rvm", "th1520", "hth1520"):
+                decode_dir = " -L " + prebuilt_dir + "decode/install/lib/rv"
+                runtime_dir = " -L " + prebuilt_dir + "runtime/riscv_linux"
+            else:
+                decode_dir = " -L " + prebuilt_dir + "decode/install/lib/x86"
+                runtime_dir = " -L " + prebuilt_dir + "runtime/x86_linux"
+
+        if board in ("c906", "c908", "c920", "rvm", "th1520", "hth1520", "th1520_x86"):
+            self.link_flag += (
+                decode_dir + runtime_dir + " -lprebuilt_runtime -ljpeg -lpng -lz -lstdc++ -lm "
+            )
+        else:
+            self.link_flag += decode_dir + runtime_dir + " -lprebuilt_runtime -fopenmp -lm -lstdc++"
+
+    def prefix_path(self, filename):
+        return " " + self.work_dir + "/" + filename + " "
+
+    def csource_command_line(self, source_name):
+        cmd_line = (
+            self.compiler
+            + self.cflag
+            + self.include_dir
+            + " -I"
+            + self.work_dir
+            + self.prefix_path(source_name + ".c")
+            + " -c -o "
+            + self.prefix_path(source_name + ".o")
+        )
+        self.source_name.append(source_name)
+        return cmd_line
+
+    def build_c(self):
+        cmd = self.csource_command_line("main")
+        logger.info(cmd)
+        os.system(cmd)
+        cmd = self.csource_command_line("model")
+        logger.info(cmd)
+        os.system(cmd)
+
+        if self.jit:
+            cmd = self.csource_command_line("jit")
+            logger.info(cmd)
+            os.system(cmd)
+
+        if self.intrinsic:
+            cmd = self.csource_command_line("intrinsic")
+            logger.info(cmd)
+            os.system(cmd)
+
+    def link_elf(self, runtime_name="hhb_runtime", jit_name="hhb_jit"):
+        self.runtime_name = runtime_name
+        self.jit_name = jit_name
+        cmd_line = (
+            self.compiler
+            + self.prefix_path("model.o")
+            + self.prefix_path("main.o")
+            + " -o "
+            + self.prefix_path(runtime_name)
+        )
+        if self.intrinsic:
+            cmd_line += self.prefix_path("intrinsic.o")
+
+        cmd_line += self.link_flag
+        logger.info(cmd_line)
+        os.system(cmd_line)
+
+        if self.jit:
+            cmd_line = (
+                self.compiler
+                + self.prefix_path("model.o")
+                + self.prefix_path("jit.o")
+                + " -o "
+                + self.prefix_path(jit_name)
+            )
+            cmd_line += self.link_flag
+            logger.info(cmd_line)
+            os.system(cmd_line)
+
+    def generate_makefile(self):
+        """Generate corresponding makefile."""
+        from .codegen_manage import get_execute_path
+
+        exec_dir = get_execute_path()
+        tp_path = os.path.join(exec_dir, "config", "template", "makefile.tp")
+
+        #######################################################################
+        #
+        # Generate compiler
+        #
+        with open(tp_path, "r") as f:
+            makefile_data = f.read()
+        makefile_data = makefile_data.replace("#_hhb_makefile_compiler_#", self.compiler)
+
+        #######################################################################
+        #
+        # Generate include
+        #
+        self.include_dir += " -I."
+        include_data = ""
+        if self.include_dir:
+            include_data = self.include_dir.strip().split(" ")
+            include_data = [i for i in include_data if i]
+            include_data = " \\\n\t".join(include_data)
+        makefile_data = makefile_data.replace("#_hhb_makefile_include_#", include_data)
+
+        #######################################################################
+        #
+        # Generate cflags
+        #
+        makefile_data = makefile_data.replace("#_hhb_makefile_cflag_#", self.cflag + "${INCLUDE}")
+
+        #######################################################################
+        #
+        # Generate ldflags
+        #
+        ld_data = self.link_flag.strip().split(" ")
+        ld_data = list(filter(lambda x: x, ld_data))
+        ld_data_p1 = []
+        ld_data_p2 = []
+        idx = 0
+        while idx < len(ld_data):
+            if ld_data[idx] == "-L":
+                ld_data_p1.extend([ld_data[idx], ld_data[idx + 1]])
+                idx += 2
+            else:
+                ld_data_p2.append(ld_data[idx])
+                idx += 1
+        p1_str = ""
+        for i in range(len(ld_data_p1) // 2):
+            p1_str += ld_data_p1[2 * i] + ld_data_p1[2 * i + 1] + " \\\n\t"
+        makefile_data = makefile_data.replace("#_hhb_makefile_ldflag1_#", p1_str)
+        p2_str = " ".join(ld_data_p2)
+        makefile_data = makefile_data.replace("#_hhb_makefile_ldflag2_#", p2_str)
+
+        #######################################################################
+        #
+        # Generate objects
+        #
+        obj_data = ""
+        if self.source_name:
+            for sf in self.source_name:
+                curr_obj = f"{sf}.o: {sf}.c\n"
+                curr_obj += "\t$(CC) $(CFLAGS) -c -o $@  $^\n"
+
+                obj_data += curr_obj + "\n"
+        obj_data = obj_data.rstrip()
+        makefile_data = makefile_data.replace("#_hhb_makefile_compile_obj_#", obj_data)
+
+        #######################################################################
+        #
+        # Generate elf
+        #
+        elf_data = f"{self.runtime_name}: main.o model.o"
+        if self.intrinsic:
+            elf_data += " intrinsic.o"
+        elf_data += "\n"
+        elf_data += "\t$(CC) $(CFLAGS) -o $@  $^ $(LDFLAGS)\n"
+
+        if self.jit:
+            elf_data += "\n"
+            elf_data += f"{self.jit_name}: jit.o model.o\n"
+            elf_data += "\t$(CC) $(CFLAGS) -o $@  $^ $(LDFLAGS)\n"
+        elf_data = elf_data.rstrip()
+        makefile_data = makefile_data.replace("#_hhb_makefile_elf_#", elf_data)
+
+        #######################################################################
+        #
+        # Generate clean
+        #
+        clean_data = f"-rm *.o {self.runtime_name}"
+        if self.jit:
+            clean_data += f" {self.jit_name}"
+        makefile_data = makefile_data.replace("#_hhb_makefile_clean_#", clean_data)
+
+        #######################################################################
+        #
+        # Generate target
+        #
+        target_data = self.runtime_name
+        if self.jit:
+            target_data += " " + self.jit_name
+        makefile_data = makefile_data.replace("#_hhb_makefile_default_target_#", target_data)
+
+        #######################################################################
+        #
+        # Generate simulation exectution
+        #
+        sim_exec_data = ""
+        if self.board in ("x86_ref", "c906", "c908", "c920", "th1520_x86"):
+            if self.board == "th1520_x86":
+                _, shl_dir, _, _, _ = find_base_path()
+                sim_exec_data += "export NNA_DDK_DIR=\n"
+                sim_exec_data += (
+                    f"export LD_LIBRARY_PATH=$NNA_DDK_DIR/x86:{os.path.join(shl_dir, 'lib')}\n"
+                )
+                sim_exec_data += "export LD_LIBRARY_PATH=$NNA_DDK_DIR/x86/sim_nna.so\n"
+            sim_exec_data += f"run_sim: {self.runtime_name}\n"
+            input_data = glob.glob(os.path.join(self.work_dir, "*.bin"))
+            input_data = list(map(lambda x: os.path.basename(x), input_data))
+            if "graph_info.bin" in input_data:
+                input_data.remove("graph_info.bin")
+            if not input_data:
+                input_data = ["data.0.bin"]
+            input_data = sorted(input_data)
+
+            exec_prefix = ""
+            if self.board == "c906":
+                exec_prefix += "qemu-riscv64 -cpu c906fdv "
+            elif self.board == "c908":
+                exec_prefix += "qemu-riscv64 -cpu c908v "
+            elif self.board == "c920":
+                exec_prefix += "qemu-riscv64 -cpu c920 "
+            sim_exec_data += f"\t{exec_prefix}./{self.runtime_name} hhb.bm {' '.join(input_data)}\n"
+
+            if self.board == "th1520_x86" and self.jit:
+                sim_exec_data += f"\nrun_jit: {self.jit_name}\n"
+                sim_exec_data += f"\t./{self.jit_name} hhb.bm\n"
+        makefile_data = makefile_data.replace("#_hhb_makefile_run_sim_#", sim_exec_data)
+
+        target_path = os.path.join(self.work_dir, f"makefile.{self.board}")
+        with open(target_path, "w") as f:
+            f.write(makefile_data)
+
+
 def guess_ir_type(file_path):
     """
     Get IR type according to the files in file_path
 
     Parameters
     ----------
     file_path : str
@@ -787,14 +1182,16 @@
     Returns
     -------
     res : HHBIRType
         Inferred IR type
     """
     hhb_ir_type = []
     for h in HHB_IR:
+        if h == HHBBoardBuildRuntime:
+            continue
         hhb_ir_obj = h()
         hhb_ir_type.append(int(hhb_ir_obj.check_ir_type(file_path)))
 
     if sum(hhb_ir_type) == 0:
         return HHBIRType.UNKNOWN
     elif sum(hhb_ir_type) == 1:
         idx = hhb_ir_type.index(1)
```

## hhb/core/main_command_manage.py

```diff
@@ -16,24 +16,26 @@
 # under the License.
 """Manage main command."""
 import logging
 import os
 import numpy as np
 import tvm
 from tvm.contrib import graph_executor
+from tvm.relay.quantize.quantize_hhb import detect_quantized_model
 
 from .arguments_manage import ArgumentFilter
-from .frontend_manage import import_model
+from .frontend_manage import import_model, insert_preprocess_node
 from .common import ensure_dir, AttributeDict, HHBException, generate_config_file
 from .hhbir_manage import (
     HHBRelayIR,
     HHBQNNIR,
     HHBFloatCodegenIR,
     HHBX86QnnCodegenIR,
     HHBBoardQnnCodegenIR,
+    HHBBoardBuildRuntime,
     get_input_info_from_relay,
     get_output_info_from_relay,
     reorder_pixel_format,
 )
 from .quantization_manage import (
     collect_quantization_config,
     set_quantize_params_by_board,
@@ -43,15 +45,15 @@
 )
 from .preprocess_manage import (
     collect_preprocess_config,
     set_preprocess_params,
     DatasetLoader,
 )
 from .codegen_manage import collect_codegen_config, set_codegen_config
-from .simulate_manage import inference_model
+from .simulate_manage import inference_model, inference_elf
 
 
 LOG = 25
 logger = logging.getLogger("HHB")
 
 
 def generate_dataset(args_filter: ArgumentFilter):
@@ -103,15 +105,15 @@
         if not (args.E or args.Q or args.C or args.simulate):
             return 0
 
     if args.generate_dataset:
         generate_dataset(args_filter)
         return 0
 
-    if not (args.E or args.Q or args.C or args.simulate):
+    if not (args.E or args.Q or args.C or args.D or args.S or args.simulate):
         raise HHBException("No subcommand select.\n")
 
     #######################################################################
     #
     # Execute '-E' command
     #
     logger.log(LOG, "Start import model.")
@@ -138,20 +140,46 @@
 
     if args.E or args.save_temps:
         relay_ir.save_model(args.output)
 
     if args.E:
         return 0
 
+    if args.board == "th1520" and (args.hybrid_computing or args.auto_hybrid_quantization):
+        args.board = "hth1520"
+
     #######################################################################
     #
     # Execute '-Q' command
     #
     input_name_list, input_shape_list, _ = get_input_info_from_relay(mod, params)
     output_shape_list, _ = get_output_info_from_relay(mod, params)
+
+    if not args.no_quantize:
+        detected_quant_type = detect_quantized_model(mod)
+        if detected_quant_type:
+            if len(detected_quant_type) == 1:
+                detected_quant_type = detected_quant_type.pop()
+                if detected_quant_type == "uint8":
+                    args.quantization_scheme = "uint8_asym"
+                elif detected_quant_type == "int8":
+                    args.quantization_scheme = "int8_asym"
+                else:
+                    raise HHBException(
+                        "Unsupport quantization type:{}.\n".format(detected_quant_type)
+                    )
+                logger.log(
+                    LOG,
+                    "Detect that current model has been quantized with {}, "
+                    "--quantization-scheme will be overwritten to {}".format(
+                        detected_quant_type, args.quantization_scheme
+                    ),
+                )
+            else:
+                logger.warning("Detect that there are multi quantization types in model.")
     # filter arguments and prepare all needed args
     all_filters = [
         collect_preprocess_config,
         set_preprocess_params,
         collect_quantization_config,
         set_quantize_params_by_board,
         collect_codegen_config,
@@ -163,23 +191,17 @@
     extra_args.output_num = len(output_shape_list)
     extra_args.model_save = args.model_save
     args_filter.filter_argument(all_filters, extra=extra_args)
     args = args_filter.filtered_args
 
     # add preprocess node into mod
     if args.preprocess_config.add_preprocess_node:
-        from tvm.relay.quantize.quantize_hhb import _bind_params
-        from tvm.relay import transform
-
-        if params:
-            mod["main"] = _bind_params(mod["main"], params)
-            params = None
-        mod = transform.AddPreprocessNode(
-            args.preprocess_config.data_mean, args.preprocess_config.data_scale
-        )(mod)
+        mod, params = insert_preprocess_node(
+            mod, params, args.preprocess_config.data_mean, args.preprocess_config.data_scale
+        )
         logger.debug("Insert preprocess node into model successfully!")
 
     config_dict = get_config_dict(args)
 
     if not args.no_quantize:
         logger.log(LOG, "Start quantization.")
         dataset_list = []
@@ -205,21 +227,22 @@
 
     #######################################################################
     #
     # Execute '-C' command
     #
     target_board_list = (
         "anole",
-        "light",
-        "hlight",
-        "asp",
-        "i805",
-        "c860",
+        "th1520",
+        "hth1520",
+        "e907",
         "c906",
+        "rvm",
         "c908",
+        "c920",
+        "x86_ref",
     )
     config_dict = get_config_dict(args)
     if config_dict["auto_hybrid_quantization"]:
         update_hybrid_layer(config_dict, args.output)
 
         limited_layer = ignore_layers_from_auto_quant(qnn_ir.get_model()[0], config_dict["target"])
         logger.info(
@@ -232,144 +255,196 @@
         )
 
         if args.quantize_config.ignore_hybrid_layer:
             config_dict["hybrid_layer_name"] = list(
                 set(config_dict["hybrid_layer_name"])
                 - set(args.quantize_config.ignore_hybrid_layer)
             )
+    th1520_input_fix_size = args.codegen_config.th1520_input_fix_size
 
-    light_input_fix_size = args.preprocess_config.light_input_fix_size
-    is_x86 = True
     if args.board == "x86_ref":
         if args.no_quantize:
             x86_codegen_ir = HHBFloatCodegenIR()
             x86_codegen_ir.convert((mod, params), args.board, args.opt_level)
+            x86_codegen_ir.save_model(args.output)
         else:
             x86_codegen_ir = HHBX86QnnCodegenIR()
             x86_codegen_ir.convert(
                 qnn_ir.get_model(), args.board, args.opt_level, args.output, config_dict
             )
-    elif args.board in target_board_list:
-        is_x86 = False
-        if args.no_quantize:
+
+    if args.no_quantize:
+        if args.board == "x86_ref":
+            pass
+        else:
             raise HHBException(
                 "can not set '--no-quantize' with '--board {}'.\n".format(args.board)
             )
-        board_codegen_ir = HHBBoardQnnCodegenIR()
-
-        board_codegen_ir.convert(
-            qnn_ir.get_model(),
-            args.board,
-            args.opt_level,
-            args.output,
-            config_dict,
-        )
     else:
-        raise HHBException("unsupport for board: {}.\n".format(args.board))
+        if args.board in target_board_list:
+            board_codegen_ir = HHBBoardQnnCodegenIR()
 
-    if args.C or args.save_temps:
-        if args.board == "x86_ref":
-            x86_codegen_ir.save_model(args.output)
-        elif args.board in target_board_list:
+            board_codegen_ir.convert(
+                qnn_ir.get_model(),
+                args.board,
+                args.opt_level,
+                args.output,
+                config_dict,
+            )
+        else:
+            raise HHBException("unsupport for board: {}.\n".format(args.board))
+
+    if args.C or args.D or args.S or args.save_temps:
+        if args.board in target_board_list and not args.no_quantize:
             input_name_list, input_shape_list, _ = get_input_info_from_relay(
                 qnn_ir.get_model()[0], None
             )
+            hhb_gen = False
+            if args.ahead_of_time == "intrinsic":
+                hhb_gen = True
             board_codegen_ir.save_model(
                 input_shape_list,
                 output_shape_list,
                 args.board,
                 args.output,
                 args.postprocess,
                 args.codegen_config.model_save,
                 args.codegen_config.without_preprocess,
                 args.preprocess_config,
                 args.codegen_config.multithread,
                 args.codegen_config.input_memory_type,
                 args.quantize_config.quantization_scheme,
                 args.codegen_config,
+                hhb_gen,
             )
 
             # save part data in calibrate dataset into tensor file
             data_count = 0
             for k in input_name_list:
                 if not dataset_list:
                     break
                 safe_k = k.replace("/", "_")
                 v = dataset_list[0][k]
                 v = v.astype("float32")
                 if args.target_layout == "NHWC":
                     v = v.transpose([0, 2, 3, 1])
                 v.tofile(os.path.join(args.output, safe_k + ".{}.tensor".format(data_count)), "\n")
                 v.tofile(os.path.join(args.output, safe_k + ".{}.bin".format(data_count)))
-                if len(light_input_fix_size) == 2:
+                if len(th1520_input_fix_size) == 2:
                     v = np.pad(
                         v,
                         (
                             (0, 0),
                             (0, 0),
-                            (0, int(light_input_fix_size[0]) - v.shape[2]),
-                            (0, int(light_input_fix_size[1]) - v.shape[3]),
+                            (0, int(th1520_input_fix_size[0]) - v.shape[2]),
+                            (0, int(th1520_input_fix_size[1]) - v.shape[3]),
                         ),
                         "constant",
                     )
                     v.tofile(
                         os.path.join(args.output, safe_k + ".{}.pad.tensor".format(data_count)),
                         "\n",
                     )
                     v.tofile(os.path.join(args.output, safe_k + ".{}.pad.bin".format(data_count)))
                 data_count += 1
-        elif args.board in ("i805"):
-            # generate function map
-            board_codegen_ir.save_model(
-                input_shape_list,
-                output_shape_list,
-                args.board,
-                args.output,
-            )
-            # save part data in calibrate dataset into tensor file
-            data_count = 0
-            input_name_list, _, _ = get_input_info_from_relay(qnn_ir.get_model()[0], None)
-            for k in input_name_list:
-                safe_k = k.replace("/", "_")
-                v = dataset_list[0][k]
-                v = v.astype("float32")
-                scale = (v.max() - v.min()) / 255
-                zp = int(0.0 - v.min() / scale)
-                v = v / scale + zp
-                v = v.astype("uint8")
-                if args.target_layout == "NHWC":
-                    v = v.transpose([0, 2, 3, 1])
-                v.tofile(os.path.join(args.output, safe_k + ".{}.tensor".format(data_count)), "\n")
-                v.tofile(os.path.join(args.output, safe_k + ".{}.bin".format(data_count)))
-                data_count += 1
 
     if args.C:
         return 0
 
     #######################################################################
     #
+    # Execute '-D' command, build all source files into one elf
+    #
+
+    if args.D or args.S:
+        intrinsic = False
+        if args.ahead_of_time == "intrinsic":
+            intrinsic = True
+        platform_deploy = HHBBoardBuildRuntime(args.board, args.output, intrinsic, args.link_lib)
+
+        # build all c source files to .o
+        platform_deploy.build_c()
+        # link_elf for linux platform
+        platform_deploy.link_elf()
+        # generate makefile
+        if args.with_makefile:
+            platform_deploy.generate_makefile()
+
+        if args.board in ("th1520", "hth1520"):
+            # for x86 simulate
+            platform_deploy = HHBBoardBuildRuntime("th1520_x86", args.output)
+
+            # build all c source files to .o
+            platform_deploy.build_c()
+            # link_elf for linux platform
+            platform_deploy.link_elf("hhb_th1520_x86_runtime", "hhb_th1520_x86_jit")
+            # generate makefile
+            if args.with_makefile:
+                platform_deploy.generate_makefile()
+
+    if args.D:
+        return 0
+
+    #######################################################################
+    #
+    # Execute '-S' command
+    #
+    dl = DatasetLoader(
+        args.simulate_data,
+        args.preprocess_config,
+        input_shape_list,
+        input_name_list,
+        target_layout=args.target_layout,
+    )
+    if args.S:
+        dataset = dl.get_data()
+        all_file_path = dl.all_file_path
+        if args.board == "x86_ref":
+            inference_elf("./hhb_runtime", dataset, input_name_list, all_file_path, args.output)
+        elif args.board == "c906":
+            inference_elf(
+                "qemu-riscv64 -cpu c906fdv hhb_runtime",
+                dataset,
+                input_name_list,
+                all_file_path,
+                args.output,
+            )
+        elif args.board == "c908":
+            inference_elf(
+                "qemu-riscv64 -cpu c908v hhb_runtime",
+                dataset,
+                input_name_list,
+                all_file_path,
+                args.output,
+            )
+        elif args.board == "c920":
+            inference_elf(
+                "qemu-riscv64 -cpu c920 hhb_runtime",
+                dataset,
+                input_name_list,
+                all_file_path,
+                args.output,
+            )
+        else:
+            raise HHBException("Unsupport to simulate for %s.\n", args.board)
+        return 0
+
+    #######################################################################
+    #
     # Execute '--simulate' command
     #
-    if not is_x86:
-        raise HHBException("{} don't support for simulation.\n".format(args.board))
     if not args.simulate_data:
         raise HHBException("Please set simulate data by --simulate-data.\n")
 
     logger.info("get simulate data from %s", args.simulate_data)
 
     ctx = tvm.cpu(0)
     if args.no_quantize:
         m = graph_executor.GraphModule(x86_codegen_ir.get_model()["default"](ctx))
     else:
+        x86_codegen_ir.save_model(args.output)
         factory = x86_codegen_ir.get_factory()
         lib = x86_codegen_ir.get_lib(args.output)
         m = tvm.contrib.graph_executor.create(factory.get_graph_json(), lib, tvm.cpu(0))
         m.load_params(tvm.runtime.save_param_dict(factory.get_params()))
 
-    dl = DatasetLoader(
-        args.simulate_data,
-        args.preprocess_config,
-        input_shape_list,
-        input_name_list,
-        target_layout=args.target_layout,
-    )
     inference_model(m, dl, args.postprocess, args.output)
```

## hhb/core/preprocess_manage.py

```diff
@@ -22,14 +22,15 @@
 from .common import argument_filter_helper
 from .common import AttributeDict
 from .common import ALL_ARGUMENTS_INFO
 from .common import HHBException
 from .common import AttributeDict
 from .common import convert_invalid_symbol
 from .common import find_index
+from .common import parse_mean
 from .data_process import DataLayout, convert_data_layout
 from .data_process import DataPreprocess
 
 
 # pylint: disable=invalid-name
 logger = logging.getLogger("HHB")
 
@@ -54,37 +55,66 @@
     mean_list = mean.strip().split(" ")
     mean_list = list([float(n) for n in mean_list if n])
     # if len(mean_list) == 1:
     #     mean_list = mean_list * 3
     return mean_list
 
 
+def get_dataset_format(data_path):
+    """Obtain dataset format
+
+    Parameters
+    ----------
+    data_path : str
+        Dataset path
+
+    Returns
+    -------
+    data_format : str
+        Dataset format, "jpg", "npz" or "mixed"
+    """
+    data_format = None
+    dp = DataPreprocess()
+    all_file_path = dp.get_file_list(data_path)
+
+    all_suffix = []
+    for input_file in all_file_path:
+        suffix = input_file.split(".")[-1]
+        all_suffix.append(suffix)
+    all_suffix = set(all_suffix)
+    if "npz" not in all_suffix:
+        data_format = "jpg"
+    else:
+        if all_suffix - set(["npz"]):
+            data_format = "mixed"
+        else:
+            data_format = "npz"
+    return data_format
+
+
 @argument_filter_helper
 def collect_preprocess_config(filtered_args, extra=None):
     """add quantize_config item for hold quantization info"""
     filtered_args.preprocess_config = AttributeDict()
     for k in ALL_ARGUMENTS_INFO["preprocess"]:
         filtered_args.preprocess_config[k] = filtered_args[k]
 
     filtered_args.preprocess_config.data_mean = parse_mean(
         filtered_args.preprocess_config.data_mean
     )
     filtered_args.preprocess_config.simulate_data_format = (
-        filtered_args.simulate_data.strip().split(".")[-1].lower()
+        get_dataset_format(filtered_args.simulate_data)
         if hasattr(filtered_args, "simulate_data") and filtered_args.simulate_data
         else None
     )
     filtered_args.preprocess_config.calibrate_data_format = (
-        filtered_args.calibrate_dataset.strip().split(".")[-1].lower()
+        get_dataset_format(filtered_args.calibrate_dataset)
         if hasattr(filtered_args, "calibrate_dataset") and filtered_args.calibrate_dataset
         else None
     )
-    filtered_args.preprocess_config.light_input_fix_size = parse_mean(
-        filtered_args.preprocess_config.light_input_fix_size
-    )
     filtered_args.preprocess_config.data_scale = filtered_args["data_scale"] * (
         1 / filtered_args["data_scale_div"]
     )
 
 
 @argument_filter_helper
 def set_preprocess_params(filtered_args, extra=None):
@@ -163,69 +193,77 @@
         self.target_layout = target_layout
 
         self._dp = DataPreprocess()
         self.all_file_path = self._dp.get_file_list(self.data_path)
 
     def get_data(self):
         assert self.batch == 1, "Only support for batch_size=1 while loading npz data."
-        suffix = self.data_path.split(".")[-1]
-        if suffix == "npz":
-            self.pre_params.with_preprocess = False
-            npz_data = np.load(self.data_path)
-            for i_name in self.input_name:
-                valid_keys = []
-                for k in npz_data.keys():
-                    valid_keys.append(convert_invalid_symbol(k))
-                if i_name not in valid_keys:
-                    logger.warning("The input data {} is not in the passed .npz file.")
-                    continue
-            split_npz_data = {}
-            epoch = list(npz_data.values())[0].shape[0]
-            npz_origin_names = [name for name in npz_data]
-            npz_valid_names = [convert_invalid_symbol(name) for name in npz_data]
-            npz_data_list = [npz_data[name] for name in npz_data]
-            for idx, name in enumerate(self.input_name):
-                if name not in npz_valid_names:
-                    logger.warning(
-                        f"model need input name '{npz_origin_names[find_index(npz_valid_names, name)]}',"
-                        "but not find in input data."
-                    )
-                    continue
-                value = npz_data_list[find_index(npz_valid_names, name)]
-                if list(value.shape) == list(self.input_shape[idx]):
-                    split_dataset = [value]
-                    epoch = 1
-                else:
-                    split_dataset = np.split(value, epoch, axis=0)
-                split_npz_data[name] = split_dataset
-            for index in range(epoch):
-                tmp_d = {}
-                for k, v in split_npz_data.items():
-                    data_rank = len(v[index].shape)
-                    if data_rank == 4:
-                        v[index] = convert_data_layout(
-                            v[index], self.pre_params.data_layout, self.target_layout
+        # check file type
+        if get_dataset_format(self.data_path) == "mixed":
+            raise ValueError("Detect mixed .npz file and jpg file, only one of them can be used.")
+
+        for input_file in self.all_file_path:
+            suffix = input_file.split(".")[-1]
+            if suffix == "npz":
+                # self.pre_params.with_preprocess = False
+                npz_data = np.load(input_file)
+                for i_name in self.input_name:
+                    valid_keys = []
+                    for k in npz_data.keys():
+                        valid_keys.append(convert_invalid_symbol(k))
+                    if i_name not in valid_keys:
+                        logger.warning(
+                            "The input name: {} is not in the passed .npz file input name: {}.".format(
+                                i_name, valid_keys
+                            )
                         )
-                    tmp_d[k] = v[index]
-                    idx = find_index(self.input_name, k)
-                    if idx != -1 and list(self.input_shape[idx]) != list(v[index].shape):
-                        if len(list(self.input_shape[idx])) != 0:
-                            raise ValueError(
-                                "Input data shape doesn't match required shape: {} vs {}".format(
-                                    list(v[index].shape), list(self.input_shape[idx])
-                                )
+                        continue
+                split_npz_data = {}
+                epoch = list(npz_data.values())[0].shape[0]
+                npz_origin_names = [name for name in npz_data]
+                npz_valid_names = [convert_invalid_symbol(name) for name in npz_data]
+                npz_data_list = [npz_data[name] for name in npz_data]
+                for idx, name in enumerate(self.input_name):
+                    if name not in npz_valid_names:
+                        logger.warning(
+                            f"model need input name '{npz_origin_names[find_index(npz_valid_names, name)]}',"
+                            "but not find in input data."
+                        )
+                        continue
+                    value = npz_data_list[find_index(npz_valid_names, name)]
+                    if list(value.shape) == list(self.input_shape[idx]):
+                        split_dataset = [value]
+                        epoch = 1
+                    else:
+                        split_dataset = np.split(value, epoch, axis=0)
+                    split_npz_data[name] = split_dataset
+                for index in range(epoch):
+                    tmp_d = {}
+                    for k, v in split_npz_data.items():
+                        data_rank = len(v[index].shape)
+                        if data_rank == 4:
+                            v[index] = convert_data_layout(
+                                v[index], self.pre_params.data_layout, self.target_layout
                             )
-                yield tmp_d
-        else:
-            if len(self.input_name) > 1:
-                raise ValueError(
-                    "The number of model input is more than 1, please " "use .npz file instead."
-                )
-            for img_file in self.all_file_path:
-                self._dp.load_image(img_file, gray=self.pre_params.gray)
+                        tmp_d[k] = v[index]
+                        idx = find_index(self.input_name, k)
+                        if idx != -1 and list(self.input_shape[idx]) != list(v[index].shape):
+                            if len(list(self.input_shape[idx])) != 0:
+                                raise ValueError(
+                                    "Input data shape doesn't match required shape: {} vs {}".format(
+                                        list(v[index].shape), list(self.input_shape[idx])
+                                    )
+                                )
+                    yield tmp_d
+            else:
+                if len(self.input_name) > 1:
+                    raise ValueError(
+                        "The number of model input is more than 1, please " "use .npz file instead."
+                    )
+                self._dp.load_image(input_file, gray=self.pre_params.gray)
                 if len(self._dp.get_data()) != self.batch:
                     continue
                 self._dp.img_resize(resize_shape=self.pre_params.data_resize)
                 self._dp.img_crop(crop_shape=self.pre_params.target_shape)
                 self._dp.channel_swap(self.pre_params.channel_swap)
                 if not self.pre_params.add_preprocess_node:
                     self._dp.sub_mean(mean_val=self.pre_params.data_mean)
@@ -235,7 +273,24 @@
                 dataset = self._dp.get_data()
                 dataset = np.concatenate(dataset, axis=0)
                 dataset = convert_data_layout(
                     dataset, self.pre_params.data_layout, self.target_layout
                 )
                 yield {self.input_name[0]: dataset}
                 self._dp.data_clear()
+
+
+def hhb_preprocess(data_path: str, config, is_generator=False):
+    """Convert data provided by data_path into target input data."""
+    dl = DatasetLoader(
+        data_path,
+        config._cmd_config.preprocess_config,
+        config._cmd_config.input_shape,
+        config._cmd_config.input_name,
+    )
+    res = dl
+    if not is_generator:
+        dataset_list = []
+        for d in dl.get_data():
+            dataset_list.append(d)
+        res = dataset_list
+    return res
```

## hhb/core/profiler_manage.py

```diff
@@ -153,21 +153,21 @@
     print(
         f"Total memory(float): params={info['params'] * 4} bytes, output={info['output'] * 4} bytes.\n"
         f"Total ddr: accum_ddr={info['accum_ddr']} bytes, coeff_ddr={info['coeff_ddr']} bytes,\n"
         f"           input_ddr={info['input_ddr']} bytes, output_ddr={info['output_ddr']} bytes."
     )
 
 
-def profile_light_trace(trace_data, indicator, frequency):
-    """Profile trace data for light.
+def profile_th1520_trace(trace_data, indicator, frequency):
+    """Profile trace data for th1520.
 
     Parameters
     ----------
     trace_data : dict
-        Original trace data in light.
+        Original trace data in th1520.
 
     indicator : list
         Indicator type to profile.
 
     frequency : int
         NPU frequency
 
@@ -279,15 +279,15 @@
             if "cal" in indicator or "all" in indicator:
                 total_info = get_cal_total_info(result)
                 print_cal_total_info(total_info)
 
             if "mem" in indicator or "all" in indicator:
                 total_info = get_mem_total_info(result)
                 print_mem_total_info(total_info)
-        elif ir_type == "light":
+        elif ir_type == "th1520":
             if "mem" in indicator or "all" in indicator:
                 total_info = get_mem_total_info(result)
                 print_mem_total_info(total_info)
 
             if "cycle" in indicator or "all" in indicator:
                 total_info = get_cycle_total_info(result)
                 print_cycle_total_info(total_info)
```

## hhb/core/quantization_manage.py

```diff
@@ -63,18 +63,18 @@
         )
         logger.log(LOG, "\t{}".format(config_dict["hybrid_layer_name"]))
     else:
         logger.log(LOG, "There is no layer to do hybrid quantization.")
 
 
 def ignore_layers_from_auto_quant(module, board):
-    """disable some ops hybrid quant: op before concat. """
+    """disable some ops hybrid quant: op before concat."""
 
     class GetLimitedLayers(tvm.relay.ExprVisitor):
-        """Get the limited layers """
+        """Get the limited layers"""
 
         def __init__(self, board):
             super(GetLimitedLayers, self).__init__()
             self.op_lists = []
             self.board = board
 
         def visit_call(self, call):
@@ -104,17 +104,14 @@
                             if (
                                 ppp_call
                                 and isinstance(ppp_call, Call)
                                 and ppp_call.op.name == "qnn.csi.conv2d"
                             ):
                                 curr_name = str(ppp_call.attrs.layer_name)
                                 self.op_lists.append(curr_name)
-            # elif call.op.name == "qnn.csi.relu" and self.board == "light":
-            #     curr_name = str(call.attrs.layer_name)
-            #     self.op_lists.append(curr_name)
             else:
                 for pre_call in call.args:
                     if isinstance(pre_call, Call):
                         if pre_call.op.name == "qnn.csi.concatenate":
                             # the op after concat should be ignore
                             curr_name = str(call.attrs.layer_name)
                             self.op_lists.append(curr_name)
@@ -164,40 +161,35 @@
         "dump_quantization_loss": args.quantize_config.dump_quantization_loss,
         "params_path": args.output,
         "model_save": args.model_save,
         "trace_strategy": args.codegen_config.trace_strategy,
         "input_memory_type": args.codegen_config.input_memory_type,
         "output_memory_type": args.codegen_config.output_memory_type,
         "model_priority": args.codegen_config.model_priority,
-        "structed_sparsity": args.structed_sparsity,
-        "kernel_parallel": args.kernel_parallel,
+        "matrix_extension_mlen": args.matrix_extension_mlen,
         "target": args.board,
         "multi_thread": args.codegen_config.multithread,
         "loss_threshold_type": args.quantize_config.loss_threshold_type,
         "from_quant_file": args.quantize_config.from_quant_file,
         "conv2d_algorithm": args.codegen_config.conv2d_algorithm,
+        "ahead_of_time": args.codegen_config.ahead_of_time,
+        "dynamic_shape": args.codegen_config.dynamic_shape,
     }
-    light_input_fix_size = args.preprocess_config.light_input_fix_size
-    if len(light_input_fix_size) == 2:
-        config_dict["light_input_fix_height"] = light_input_fix_size[0]
-        config_dict["light_input_fix_width"] = light_input_fix_size[1]
-
-    if args.board == "light" and args.codegen_config.model_save == "save_only":
-        config_dict["target"] = "light_new"
+    th1520_input_fix_size = args.codegen_config.th1520_input_fix_size
+    if len(th1520_input_fix_size) == 2:
+        config_dict["th1520_input_fix_height"] = th1520_input_fix_size[0]
+        config_dict["th1520_input_fix_width"] = th1520_input_fix_size[1]
 
     if args.verbose >= 3:
         config_dict["debug_level"] = "INFO"
 
-    if args.codegen_config.model_save == "save_only":
-        config_dict["h_sram_size"] = (
-            2 ** 20 if not args.hardware_sram_size else args.hardware_sram_size
-        )
-        config_dict["h_max_groups"] = (
-            16 if not args.hardware_max_groups else args.hardware_max_groups
-        )
+    if args.codegen_config.ahead_of_time == "intrinsic":
+        if args.quantize_config.quantization_scheme not in ["float32", "float16"]:
+            raise HHBException("--ahead-of-time intrinsic only support float32 or float16.\n")
+
     return config_dict
 
 
 @argument_filter_helper
 def collect_quantization_config(filtered_args, extra=None):
     """add quantize_config item for hold quantization info"""
     unexpected_params = ["calibrate_dataset"]
@@ -234,46 +226,47 @@
             "fuse_reshape_dense": True,
             "fuse_mul_add_to_conv": True,
             "channel_quantization": False,
             "broadcast_quantization": True,
         }
         if not filtered_args.quantize_config.quantization_scheme in ("unset", "uint8_asym"):
             raise HHBException("Anole only support uint8_asym\n")
+        if filtered_args.quantize_config.quantization_scheme == "unset":
+            new_values["quantization_scheme"] = "uint8_asym"
         if filtered_args.quantize_config.channel_quantization:
             hhb_exit("Anole unsupport channel quantization.")
-    elif filtered_args.board == "light":
+    elif filtered_args.board == "th1520":
         new_values = {
             "num_bit_input": 8,
             "num_bit_weight": 8,
             "num_bit_activation": 32,
-            "dtype_input": "float32",
-            "dtype_weight": "float32",
-            "dtype_activation": "float32",
+            "dtype_input": "int8",
+            "dtype_weight": "int8",
+            "dtype_activation": "int32",
             "calibrate_mode": "maxmin",
-            "weight_quantized_type": "sym",
-            "activate_quantized_type": "sym",
+            "weight_quantized_type": "asym",
+            "activate_quantized_type": "asym",
             "weight_scale": "maxmin",
             "fuse_conv_relu": False,
             "fuse_relu": False,
             # "fuse_reshape": False,
             "fuse_mul_add_to_conv": True,
             # "channel_quantization": False,
             "broadcast_quantization": True,
         }
         if filtered_args.quantize_config.channel_quantization:
             if filtered_args.quantize_config.quantization_scheme != "int8_asym_w_sym":
                 hhb_exit(
-                    "Light channel quantization only support with int8_asym_w_sym quantization scheme."
+                    "th1520 channel quantization only support with int8_asym_w_sym quantization scheme."
                 )
         if filtered_args.quantize_config.channel_quantization:
             new_values["calibrate_mode"] = "maxmin"
             new_values["weight_scale"] = "maxmin"
         if filtered_args.quantize_config.quantization_scheme == "unset":
-            new_values["quantization_scheme"] = "int8_sym"
-            filtered_args.quantize_config.quantization_scheme = "unset"
+            new_values["quantization_scheme"] = "int8_asym"
         elif filtered_args.quantize_config.quantization_scheme == "int8_sym":
             new_values["quantization_scheme"] = "int8_sym"
             filtered_args.quantize_config.quantization_scheme = "unset"
         elif filtered_args.quantize_config.quantization_scheme == "int8_asym_w_sym":
             new_values["quantization_scheme"] = "int8_asym_w_sym"
         elif filtered_args.quantize_config.quantization_scheme == "int8_original":
             new_values["quantization_scheme"] = "int8_original"
@@ -286,139 +279,188 @@
         elif filtered_args.quantize_config.quantization_scheme == "int16_sym":
             new_values["quantization_scheme"] = "int16_sym"
             new_values["num_bit_input"] = 16
             new_values["num_bit_weight"] = 16
             filtered_args.quantize_config.quantization_scheme = "unset"
         else:
             raise HHBException(
-                f"Unsupport quantization scheme '{filtered_args.quantize_config.quantization_scheme}' on light\n"
+                f"Unsupport quantization scheme '{filtered_args.quantize_config.quantization_scheme}' on th1520\n"
             )
         if filtered_args.quantize_config.quantization_scheme in ("float16", "bfloat16"):
-            raise HHBException("Light unsupport float16 or bfloat16\n")
+            raise HHBException("th1520 unsupport float16 or bfloat16\n")
 
-    elif filtered_args.board == "hlight":
+    elif filtered_args.board == "hth1520":
         new_values = {
             "num_bit_input": 8,
             "num_bit_weight": 8,
             "num_bit_activation": 32,
-            "dtype_input": "float32",
-            "dtype_weight": "float32",
-            "dtype_activation": "float32",
+            "dtype_input": "int8",
+            "dtype_weight": "int8",
+            "dtype_activation": "int32",
             "calibrate_mode": "maxmin",
-            "weight_quantized_type": "sym",
-            "activate_quantized_type": "sym",
+            "weight_quantized_type": "asym",
+            "activate_quantized_type": "asym",
             "weight_scale": "maxmin",
             "fuse_relu": False,
             # "fuse_reshape": False,
             "fuse_mul_add_to_conv": True,
             # "channel_quantization": False,
             "broadcast_quantization": True,
         }
-
+        if filtered_args.quantize_config.quantization_scheme == "unset":
+            new_values["quantization_scheme"] = "int8_asym"
         if filtered_args.quantize_config.channel_quantization:
-            hhb_exit("HLight unsupport channel quantization.")
-    elif filtered_args.board == "asp":
+            hhb_exit("hth1520 unsupport channel quantization.")
+    elif filtered_args.board == "e907":
         new_values = {
             "num_bit_input": 8,
             "num_bit_weight": 8,
             # "num_bit_activation": 32,
             "dtype_input": "int8",
             "dtype_weight": "int8",
             "dtype_activation": "int32",
             "calibrate_mode": "maxmin",
-            "weight_quantized_type": "sym",
+            "weight_quantized_type": "asym",
             "activate_quantized_type": "asym",
             "weight_scale": "maxmin",
+            # "fuse_conv_relu": False,
+            "fuse_relu": False,
+            # "fuse_reshape": False,
+            "fuse_mul_add_to_conv": True,
+            # "channel_quantization": False,
+            # "broadcast_quantization": False,
+        }
+        if filtered_args.quantize_config.quantization_scheme == "unset":
+            new_values["quantization_scheme"] = "int8_asym_w_sym"
+    elif filtered_args.board == "c906":
+        new_values = {
+            "num_bit_input": 16,
+            "num_bit_weight": 16,
+            # "num_bit_activation": 32,
+            "dtype_input": "float16",
+            "dtype_weight": "float16",
+            "dtype_activation": "float16",
+            # "calibrate_mode": "maxmin",
+            "weight_quantized_type": "sym",
+            "activate_quantized_type": "sym",
+            "weight_scale": "maxmin",
             "fuse_conv_relu": False,
-            "fuse_relu": True,
+            "fuse_relu": False,
             # "fuse_reshape": False,
             "fuse_mul_add_to_conv": True,
             # "channel_quantization": False,
-            "broadcast_quantization": True,
+            # "broadcast_quantization": False,
         }
-        # ASP only support NHWC
-        filtered_args.quantize_config.target_layout = "NHWC"
-    elif filtered_args.board == "i805":
+        if filtered_args.quantize_config.quantization_scheme == "unset":
+            new_values["quantization_scheme"] = "float16"
+    elif filtered_args.board == "rvm":
+        new_values = {
+            "num_bit_input": 16,
+            "num_bit_weight": 16,
+            # "num_bit_activation": 32,
+            "dtype_input": "float16",
+            "dtype_weight": "float16",
+            "dtype_activation": "float16",
+            # "calibrate_mode": "maxmin",
+            "weight_quantized_type": "sym",
+            "activate_quantized_type": "sym",
+            "weight_scale": "maxmin",
+            # "fuse_conv_relu": False,
+            "fuse_relu": False,
+            # "fuse_reshape": False,
+            "fuse_mul_add_to_conv": True,
+            # "channel_quantization": False,
+            # "broadcast_quantization": False,
+        }
+        if filtered_args.quantize_config.quantization_scheme == "unset":
+            new_values["quantization_scheme"] = "int8_asym_w_sym"
+    elif filtered_args.board == "c908":
         new_values = {
             "num_bit_input": 8,
             "num_bit_weight": 8,
-            # "num_bit_activation": 32,
-            "dtype_input": "uint8",
-            "dtype_weight": "uint8",
+            "num_bit_activation": 32,
+            "dtype_input": "int8",
+            "dtype_weight": "int8",
             "dtype_activation": "int32",
-            "calibrate_mode": "maxmin",
+            # "calibrate_mode": "maxmin",
             "weight_quantized_type": "asym",
             "activate_quantized_type": "asym",
             "weight_scale": "maxmin",
-            "fuse_conv_relu": False,
+            # "fuse_conv_relu": False,
             "fuse_relu": False,
             # "fuse_reshape": False,
             "fuse_mul_add_to_conv": True,
             # "channel_quantization": False,
             # "broadcast_quantization": False,
         }
-        if filtered_args.quantize_config.channel_quantization:
-            hhb_exit("i805 unsupport channel quantization.")
-    elif filtered_args.board == "c906":
+        if filtered_args.quantize_config.quantization_scheme == "unset":
+            new_values["quantization_scheme"] = "int8_asym_w_sym"
+    elif filtered_args.board == "c920":
         new_values = {
             "num_bit_input": 16,
             "num_bit_weight": 16,
             # "num_bit_activation": 32,
             "dtype_input": "float16",
             "dtype_weight": "float16",
             "dtype_activation": "float16",
-            "calibrate_mode": "maxmin",
+            # "calibrate_mode": "maxmin",
             "weight_quantized_type": "sym",
             "activate_quantized_type": "sym",
             "weight_scale": "maxmin",
             "fuse_conv_relu": False,
             "fuse_relu": False,
             # "fuse_reshape": False,
             "fuse_mul_add_to_conv": True,
             # "channel_quantization": False,
             # "broadcast_quantization": False,
         }
-    elif filtered_args.board == "c908":
+        if filtered_args.quantize_config.quantization_scheme == "unset":
+            new_values["quantization_scheme"] = "float16"
+    elif filtered_args.board == "x86_ref":
         new_values = {
             "num_bit_input": 8,
             "num_bit_weight": 8,
-            # "num_bit_activation": 32,
-            "dtype_input": "float32",
-            "dtype_weight": "float32",
-            "dtype_activation": "float32",
-            "calibrate_mode": "maxmin",
-            "weight_quantized_type": "sym",
-            "activate_quantized_type": "sym",
+            "num_bit_activation": 32,
+            "dtype_input": "int8",
+            "dtype_weight": "int8",
+            "dtype_activation": "int32",
+            # "calibrate_mode": "maxmin",
+            "weight_quantized_type": "asym",
+            "activate_quantized_type": "asym",
             "weight_scale": "maxmin",
             # "fuse_conv_relu": False,
             "fuse_relu": False,
             # "fuse_reshape": False,
             "fuse_mul_add_to_conv": True,
             # "channel_quantization": False,
             # "broadcast_quantization": False,
         }
+        if filtered_args.quantize_config.quantization_scheme == "unset":
+            new_values["quantization_scheme"] = "int8_asym"
     else:
         new_values = {
             "num_bit_input": 8,
             "num_bit_weight": 8,
             "num_bit_activation": 32,
-            "dtype_input": "uint8",
-            "dtype_weight": "uint8",
+            "dtype_input": "int8",
+            "dtype_weight": "int8",
             "dtype_activation": "int32",
             # "calibrate_mode": "maxmin",
             "weight_quantized_type": "asym",
             "activate_quantized_type": "asym",
             "weight_scale": "maxmin",
             "fuse_conv_relu": False,
             "fuse_relu": False,
             # "fuse_reshape": False,
             "fuse_mul_add_to_conv": True,
             # "channel_quantization": False,
             # "broadcast_quantization": False,
         }
+        if filtered_args.quantize_config.quantization_scheme == "unset":
+            new_values["quantization_scheme"] = "int8_asym_w_sym"
 
     # if filtered_args.board != "x86_ref":
     #     if (
     #         filtered_args.quantize_config.hybrid_quantization_scheme != "unset"
     #         or filtered_args.quantize_config.hybrid_layer_name is not None
     #     ):
     #         raise HHBException("Only 'x86_ref' target support for hybrid-quantization.\n")
@@ -496,14 +538,24 @@
         new_values["num_bit_weight"] = 16
         new_values["num_bit_activation"] = 16
         new_values["dtype_input"] = "float16"
         new_values["dtype_weight"] = "float16"
         new_values["dtype_activation"] = "float16"
         new_values["activate_quantized_type"] = "sym"
         new_values["weight_quantized_type"] = "sym"
+    elif filtered_args.quantize_config.quantization_scheme == "float16_w_int8":
+        new_values["num_bit_input"] = 16
+        new_values["num_bit_weight"] = 16
+        new_values["num_bit_activation"] = 16
+        new_values["dtype_input"] = "float16"
+        # w_int8 only for matmul now
+        new_values["dtype_weight"] = "float16"
+        new_values["dtype_activation"] = "float16"
+        new_values["activate_quantized_type"] = "sym"
+        new_values["weight_quantized_type"] = "sym"
     elif filtered_args.quantize_config.quantization_scheme == "bfloat16":
         new_values["num_bit_input"] = 16
         new_values["num_bit_weight"] = 16
         new_values["num_bit_activation"] = 16
         new_values["dtype_input"] = "bfloat16"
         new_values["dtype_weight"] = "bfloat16"
         new_values["dtype_activation"] = "bfloat16"
@@ -554,18 +606,17 @@
         ] = filtered_args.quantize_config.activate_quantized_type
 
     filtered_args.quantize_config.update(new_values)
 
     if (
         filtered_args.quantize_config.broadcast_quantization
         and filtered_args.quantize_config.fuse_relu
-        and filtered_args.board != "asp"
     ):
         raise HHBException(
-            "--broadcast-quantization and --fuse_relu can only be used simultaneously when the board is ASP.\n"
+            "--broadcast-quantization and --fuse_relu can only be used simultaneously.\n"
         )
 
 
 def quantize_model(mod, params, qconfig, dataset=None, target="x86_ref"):
     """Quantize the imported relay module.
 
     Parameters
```

## hhb/core/simulate_manage.py

```diff
@@ -13,20 +13,25 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 # pylint: disable=unnecessary-comprehension
 """Manage simulate"""
 import os
+import logging
 
 import numpy as np
 
 from .preprocess_manage import DatasetLoader
 from .common import print_top5, ensure_dir
 
+# pylint: disable=invalid-name
+LOG = 25
+logger = logging.getLogger("HHB")
+
 
 def inference_model(graph_module, data_loader: DatasetLoader, postprocess="top5", output_dir="."):
     """Inference GraphModule by specified data loader
 
     Parameters
     ----------
     graph_module: GraphModule
@@ -57,16 +62,70 @@
             )
             output_prefix = os.path.basename(out_basename) + "_output_" + str(i) + ".tensor"
             if postprocess == "top5":
                 print_top5(out, str(i), out_shape)
             elif postprocess == "save":
                 output_dir = ensure_dir(output_dir)
                 np.savetxt(
-                    os.path.join(output_dir, output_prefix), out, delimiter="\n", newline="\n"
+                    os.path.join(output_dir, output_prefix),
+                    out,
+                    fmt="%f",
+                    delimiter="\n",
+                    newline="\n",
                 )
             else:
                 print_top5(out, str(i), out_shape)
                 output_dir = ensure_dir(output_dir)
                 np.savetxt(
-                    os.path.join(output_dir, output_prefix), out, delimiter="\n", newline="\n"
+                    os.path.join(output_dir, output_prefix),
+                    out,
+                    fmt="%f",
+                    delimiter="\n",
+                    newline="\n",
                 )
         index += 1
+
+
+def inference_elf(elf_file, dataset, input_name_list, all_file_path, output_dir="."):
+    """Inference elf on x86 by specified data loader
+
+    Parameters
+    ----------
+    elf: str
+        elf file that build to execute the graph.
+
+    data_loader: DatasetLoader
+        Data loader machine that can load specified data.
+
+    postprocess: Optional[str]
+        How to deal with output data:
+        "top5": print the top5 values of outputs;
+        "save": save the output values into file;
+        "save_and_top5": print the top5 values and save the values into file.
+
+    """
+    command_line_base = "cd " + output_dir + "; " + elf_file + " ./hhb.bm "
+
+    index = 0
+    for data in dataset:
+        command_line = command_line_base
+        data_count = 0
+        for k in input_name_list:
+            if len(all_file_path) == 1:
+                if index == 0:
+                    input_name = all_file_path[0]
+                else:
+                    input_name = all_file_path[0] + "_" + str(index)
+            else:
+                input_name = all_file_path[index]
+            v = data[k]
+            v = v.astype("float32")
+            file = os.path.basename(input_name) + ".{}.bin".format(data_count)
+            file_path = os.path.join(output_dir, file)
+            v.tofile(file_path)
+            command_line += file + " "
+            data_count += 1
+
+        logger.log(LOG, command_line)
+        os.system(command_line)
+
+        index += 1
```

## Comparing `hhb/config/cb_map.tp` & `hhb/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,24 @@
-/*
- * Licensed to the Apache Software Foundation (ASF) under one
- * or more contributor license agreements.  See the NOTICE file
- * distributed with this work for additional information
- * regarding copyright ownership.  The ASF licenses this file
- * to you under the Apache License, Version 2.0 (the
- * "License"); you may not use this file except in compliance
- * with the License.  You may obtain a copy of the License at
- *
- *   http://www.apache.org/licenses/LICENSE-2.0
- *
- * Unless required by applicable law or agreed to in writing,
- * software distributed under the License is distributed on an
- * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
- * KIND, either express or implied.  See the License for the
- * specific language governing permissions and limitations
- * under the License.
- */
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+"""
+HHB - HHB command-line interface
+"""
 
-/* auto generate by HHB_VERSION "2.0.20" */
+from .main import main
 
-#include <shl_i805.h>
-
-void *shl_cb_map_#TARGET(int op, int dtype)
-{
-    switch (dtype)
-    {
-    case CSINN_DTYPE_UINT8:
-        switch (op)
-        {
-#OP_CASE
-        default:
-            return CSINN_FALSE;
-        }
-    case CSINN_DTYPE_INT16:
-        return CSINN_FALSE;
-        break;
-    default:
-        return CSINN_FALSE;
-    }
-}
+if __name__ == "__main__":
+    main()
```

## Comparing `hhb/config/light.tp` & `hhb/config/th1520.tp`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
-/* auto generate by HHB_VERSION "2.0.20" */
+/* auto generate by HHB_VERSION "2.2.35" */
 
 #_hhb_header_files_#
 
 #_hhb_macro_def_#
 
 #_hhb_function_decl_#
 
@@ -78,40 +78,46 @@
             data_path = argv + 2;
             input_group_num = (argc - 2) / input_num;
         }
     }
 
     void *sess = create_graph(argv[1]);
 
-    uint8_t *input[input_num];
+    struct csinn_tensor* input_tensors[input_num];
+    #_tensor_shape_#
     float *inputf[input_num];
+    int8_t *input[input_num];
     char filename_prefix[FILE_LENGTH] = {0};
     #_aligned_buffer_stats_#
     uint64_t start_time, end_time;
     for (i = 0; i < input_group_num; i++) {
         /* set input */
         for (int j = 0; j < input_num; j++) {
             #_get_input_data_stats_#
             input[j] = shl_ref_f32_to_input_dtype(j, inputf[j], sess);
         }
         #_aligned_buffer_copy_#
         start_time = shl_get_timespec();
-        csinn_run(#_anole_value_pass# sess);
+        csinn_update_input_and_run(input_tensors, sess);
         end_time = shl_get_timespec();
         printf("Run graph execution time: %.5fms, FPS=%.2f\n", ((float)(end_time-start_time))/1000000,
                     1000000000.0/((float)(end_time-start_time)));
 
         snprintf(filename_prefix, FILE_LENGTH, "%s", basename(data_path[i * input_num]));
         postprocess(sess, filename_prefix);
 
         for (int j = 0; j < input_num; j++) {
             shl_mem_free(inputf[j]);
             shl_mem_free(input[j]);
         }
     }
+    for (int j = 0; j < input_num; j++) {
+        csinn_free_tensor(input_tensors[j]);
+        #_aligned_buffer_free_#
+    }
 
     csinn_session_deinit(sess);
     csinn_free_session(sess);
 
     return 0;
 }
```

