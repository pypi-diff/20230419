# Comparing `tmp/nvidia_cuda_profiler_api_cu12-12.1.105-py3-none-manylinux1_x86_64.whl.zip` & `tmp/nvidia_cuda_profiler_api_cu12-12.1.55-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 21386 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 04:15 nvidia/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 04:15 nvidia/cuda_profiler_api/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 04:15 nvidia/cuda_profiler_api/include/__init__.py
--rw-r--r--  2.0 unx     7019 b- defN 23-Apr-04 04:15 nvidia/cuda_profiler_api/include/cudaProfiler.h
--rw-r--r--  2.0 unx     4566 b- defN 23-Apr-04 04:15 nvidia/cuda_profiler_api/include/cuda_profiler_api.h
--rw-r--r--  2.0 unx    59262 b- defN 23-Apr-04 04:15 nvidia_cuda_profiler_api_cu12-12.1.105.dist-info/License.txt
--rw-r--r--  2.0 unx     1552 b- defN 23-Apr-04 04:15 nvidia_cuda_profiler_api_cu12-12.1.105.dist-info/METADATA
--rw-r--r--  2.0 unx      106 b- defN 23-Apr-04 04:15 nvidia_cuda_profiler_api_cu12-12.1.105.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-04 04:15 nvidia_cuda_profiler_api_cu12-12.1.105.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      989 b- defN 23-Apr-04 04:15 nvidia_cuda_profiler_api_cu12-12.1.105.dist-info/RECORD
-10 files, 73501 bytes uncompressed, 19634 bytes compressed:  73.3%
+Zip file size: 21401 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 23-Jan-25 04:50 nvidia/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jan-25 04:50 nvidia/cuda_profiler_api/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jan-25 04:50 nvidia/cuda_profiler_api/include/__init__.py
+-rw-r--r--  2.0 unx     7235 b- defN 23-Jan-25 04:50 nvidia/cuda_profiler_api/include/cudaProfiler.h
+-rw-r--r--  2.0 unx     4700 b- defN 23-Jan-25 04:50 nvidia/cuda_profiler_api/include/cuda_profiler_api.h
+-rw-r--r--  2.0 unx    59262 b- defN 23-Jan-25 04:50 nvidia_cuda_profiler_api_cu12-12.1.55.dist-info/License.txt
+-rw-r--r--  2.0 unx     1551 b- defN 23-Jan-25 04:50 nvidia_cuda_profiler_api_cu12-12.1.55.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 23-Jan-25 04:50 nvidia_cuda_profiler_api_cu12-12.1.55.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jan-25 04:50 nvidia_cuda_profiler_api_cu12-12.1.55.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      983 b- defN 23-Jan-25 04:50 nvidia_cuda_profiler_api_cu12-12.1.55.dist-info/RECORD
+10 files, 73836 bytes uncompressed, 19659 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: nvidia/cuda_profiler_api/include/cudaProfiler.h
 Comment: 
 
 Filename: nvidia/cuda_profiler_api/include/cuda_profiler_api.h
 Comment: 
 
-Filename: nvidia_cuda_profiler_api_cu12-12.1.105.dist-info/License.txt
+Filename: nvidia_cuda_profiler_api_cu12-12.1.55.dist-info/License.txt
 Comment: 
 
-Filename: nvidia_cuda_profiler_api_cu12-12.1.105.dist-info/METADATA
+Filename: nvidia_cuda_profiler_api_cu12-12.1.55.dist-info/METADATA
 Comment: 
 
-Filename: nvidia_cuda_profiler_api_cu12-12.1.105.dist-info/WHEEL
+Filename: nvidia_cuda_profiler_api_cu12-12.1.55.dist-info/WHEEL
 Comment: 
 
-Filename: nvidia_cuda_profiler_api_cu12-12.1.105.dist-info/top_level.txt
+Filename: nvidia_cuda_profiler_api_cu12-12.1.55.dist-info/top_level.txt
 Comment: 
 
-Filename: nvidia_cuda_profiler_api_cu12-12.1.105.dist-info/RECORD
+Filename: nvidia_cuda_profiler_api_cu12-12.1.55.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nvidia/cuda_profiler_api/include/cudaProfiler.h

 * *Ordering differences only*

```diff
@@ -1,216 +1,216 @@
-/*
- * Copyright 1993-2018 NVIDIA Corporation.  All rights reserved.
- *
- * NOTICE TO LICENSEE:
- *
- * This source code and/or documentation ("Licensed Deliverables") are
- * subject to NVIDIA intellectual property rights under U.S. and
- * international Copyright laws.
- *
- * These Licensed Deliverables contained herein is PROPRIETARY and
- * CONFIDENTIAL to NVIDIA and is being provided under the terms and
- * conditions of a form of NVIDIA software license agreement by and
- * between NVIDIA and Licensee ("License Agreement") or electronically
- * accepted by Licensee.  Notwithstanding any terms or conditions to
- * the contrary in the License Agreement, reproduction or disclosure
- * of the Licensed Deliverables to any third party without the express
- * written consent of NVIDIA is prohibited.
- *
- * NOTWITHSTANDING ANY TERMS OR CONDITIONS TO THE CONTRARY IN THE
- * LICENSE AGREEMENT, NVIDIA MAKES NO REPRESENTATION ABOUT THE
- * SUITABILITY OF THESE LICENSED DELIVERABLES FOR ANY PURPOSE.  IT IS
- * PROVIDED "AS IS" WITHOUT EXPRESS OR IMPLIED WARRANTY OF ANY KIND.
- * NVIDIA DISCLAIMS ALL WARRANTIES WITH REGARD TO THESE LICENSED
- * DELIVERABLES, INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY,
- * NONINFRINGEMENT, AND FITNESS FOR A PARTICULAR PURPOSE.
- * NOTWITHSTANDING ANY TERMS OR CONDITIONS TO THE CONTRARY IN THE
- * LICENSE AGREEMENT, IN NO EVENT SHALL NVIDIA BE LIABLE FOR ANY
- * SPECIAL, INDIRECT, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, OR ANY
- * DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS,
- * WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
- * ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE
- * OF THESE LICENSED DELIVERABLES.
- *
- * U.S. Government End Users.  These Licensed Deliverables are a
- * "commercial item" as that term is defined at 48 C.F.R. 2.101 (OCT
- * 1995), consisting of "commercial computer software" and "commercial
- * computer software documentation" as such terms are used in 48
- * C.F.R. 12.212 (SEPT 1995) and is provided to the U.S. Government
- * only as a commercial end item.  Consistent with 48 C.F.R.12.212 and
- * 48 C.F.R. 227.7202-1 through 227.7202-4 (JUNE 1995), all
- * U.S. Government End Users acquire the Licensed Deliverables with
- * only those rights set forth herein.
- *
- * Any use of the Licensed Deliverables in individual and commercial
- * software must include, in the user documentation and internal
- * comments to the code, the above Disclaimer and U.S. Government End
- * Users Notice.
- */
-
-#ifndef cuda_profiler_H
-#define cuda_profiler_H
-
-#include <cuda.h>
-
-#if defined(__CUDA_API_VERSION_INTERNAL) || defined(__DOXYGEN_ONLY__) || defined(CUDA_ENABLE_DEPRECATED)
-#define __CUDA_DEPRECATED
-#elif defined(_MSC_VER)
-#define __CUDA_DEPRECATED __declspec(deprecated)
-#elif defined(__GNUC__)
-#define __CUDA_DEPRECATED __attribute__((deprecated))
-#else
-#define __CUDA_DEPRECATED
-#endif
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-/**
- * Profiler Output Modes
- */
-/*DEVICE_BUILTIN*/
-typedef enum CUoutput_mode_enum
-{
-    CU_OUT_KEY_VALUE_PAIR  = 0x00, /**< Output mode Key-Value pair format. */
-    CU_OUT_CSV             = 0x01  /**< Output mode Comma separated values format. */
-}CUoutput_mode;
-
-
-/**
- * \ingroup CUDA_DRIVER
- * \defgroup CUDA_PROFILER_DEPRECATED Profiler Control [DEPRECATED]
- *
- * ___MANBRIEF___ profiler control functions of the low-level CUDA driver API
- * (___CURRENT_FILE___) ___ENDMANBRIEF___
- *
- * This section describes the profiler control functions of the low-level CUDA
- * driver application programming interface.
- *
- * @{
- */
-
-/**
- * \brief Initialize the profiling.
- *
- * \deprecated
- *
- * Note that this function is deprecated and should not be used.
- * Starting with CUDA 12.0, it always returns error code ::CUDA_ERROR_NOT_SUPPORTED.
- * 
- * Using this API user can initialize the CUDA profiler by specifying
- * the configuration file, output file and output file format. This
- * API is generally used to profile different set of counters by
- * looping the kernel launch. The \p configFile parameter can be used
- * to select profiling options including profiler counters. Refer to
- * the "Compute Command Line Profiler User Guide" for supported
- * profiler options and counters.
- *
- * Limitation: The CUDA profiler cannot be initialized with this API
- * if another profiling tool is already active, as indicated by the
- * ::CUDA_ERROR_PROFILER_DISABLED return code.
- *
- * Typical usage of the profiling APIs is as follows: 
- *
- * for each set of counters/options\n
- * {\n
- *     cuProfilerInitialize(); //Initialize profiling, set the counters or options in the config file \n
- *     ...\n
- *     cuProfilerStart(); \n
- *     // code to be profiled \n
- *     cuProfilerStop(); \n
- *     ...\n
- *     cuProfilerStart(); \n
- *     // code to be profiled \n
- *     cuProfilerStop(); \n
- *     ...\n
- * }\n
- *
- * \param configFile - Name of the config file that lists the counters/options
- * for profiling.
- * \param outputFile - Name of the outputFile where the profiling results will
- * be stored.
- * \param outputMode - outputMode, can be ::CU_OUT_KEY_VALUE_PAIR or ::CU_OUT_CSV.
- *
- * \return
- * ::CUDA_ERROR_NOT_SUPPORTED
- * \notefnerr
- *
- * \sa
- * ::cuProfilerStart,
- * ::cuProfilerStop,
- */
-__CUDA_DEPRECATED CUresult CUDAAPI cuProfilerInitialize(const char *configFile, const char *outputFile, CUoutput_mode outputMode);
- 
-/** @} */ /* END CUDA_PROFILER_DEPRECATED */
-
-/**
- * \ingroup CUDA_DRIVER
- * \defgroup CUDA_PROFILER Profiler Control 
- *
- * ___MANBRIEF___ profiler control functions of the low-level CUDA driver API
- * (___CURRENT_FILE___) ___ENDMANBRIEF___
- *
- * This section describes the profiler control functions of the low-level CUDA
- * driver application programming interface.
- *
- * @{
- */
-
-/**
- * \brief Enable profiling.
- *
- * Enables profile collection by the active profiling tool for the
- * current context. If profiling is already enabled, then
- * cuProfilerStart() has no effect.
- *
- * cuProfilerStart and cuProfilerStop APIs are used to
- * programmatically control the profiling granularity by allowing
- * profiling to be done only on selective pieces of code.
- * 
- *
- * \return
- * ::CUDA_SUCCESS,
- * ::CUDA_ERROR_INVALID_CONTEXT
- * \notefnerr
- *
- * \sa
- * ::cuProfilerInitialize,
- * ::cuProfilerStop,
- * ::cudaProfilerStart
- */
-CUresult CUDAAPI cuProfilerStart(void);
-
-/**
- * \brief Disable profiling.
- *
- * Disables profile collection by the active profiling tool for the
- * current context. If profiling is already disabled, then
- * cuProfilerStop() has no effect.
- *
- * cuProfilerStart and cuProfilerStop APIs are used to
- * programmatically control the profiling granularity by allowing
- * profiling to be done only on selective pieces of code.
- *
- * \return
- * ::CUDA_SUCCESS,
- * ::CUDA_ERROR_INVALID_CONTEXT
- * \notefnerr
- *
- * \sa
- * ::cuProfilerInitialize,
- * ::cuProfilerStart,
- * ::cudaProfilerStop
- */
-CUresult CUDAAPI cuProfilerStop(void);
-
-/** @} */ /* END CUDA_PROFILER */
-
-#ifdef __cplusplus
-};
-#endif
-
-#undef __CUDA_DEPRECATED
-
-#endif
-
+/*
+ * Copyright 1993-2018 NVIDIA Corporation.  All rights reserved.
+ *
+ * NOTICE TO LICENSEE:
+ *
+ * This source code and/or documentation ("Licensed Deliverables") are
+ * subject to NVIDIA intellectual property rights under U.S. and
+ * international Copyright laws.
+ *
+ * These Licensed Deliverables contained herein is PROPRIETARY and
+ * CONFIDENTIAL to NVIDIA and is being provided under the terms and
+ * conditions of a form of NVIDIA software license agreement by and
+ * between NVIDIA and Licensee ("License Agreement") or electronically
+ * accepted by Licensee.  Notwithstanding any terms or conditions to
+ * the contrary in the License Agreement, reproduction or disclosure
+ * of the Licensed Deliverables to any third party without the express
+ * written consent of NVIDIA is prohibited.
+ *
+ * NOTWITHSTANDING ANY TERMS OR CONDITIONS TO THE CONTRARY IN THE
+ * LICENSE AGREEMENT, NVIDIA MAKES NO REPRESENTATION ABOUT THE
+ * SUITABILITY OF THESE LICENSED DELIVERABLES FOR ANY PURPOSE.  IT IS
+ * PROVIDED "AS IS" WITHOUT EXPRESS OR IMPLIED WARRANTY OF ANY KIND.
+ * NVIDIA DISCLAIMS ALL WARRANTIES WITH REGARD TO THESE LICENSED
+ * DELIVERABLES, INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY,
+ * NONINFRINGEMENT, AND FITNESS FOR A PARTICULAR PURPOSE.
+ * NOTWITHSTANDING ANY TERMS OR CONDITIONS TO THE CONTRARY IN THE
+ * LICENSE AGREEMENT, IN NO EVENT SHALL NVIDIA BE LIABLE FOR ANY
+ * SPECIAL, INDIRECT, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, OR ANY
+ * DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS,
+ * WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+ * ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE
+ * OF THESE LICENSED DELIVERABLES.
+ *
+ * U.S. Government End Users.  These Licensed Deliverables are a
+ * "commercial item" as that term is defined at 48 C.F.R. 2.101 (OCT
+ * 1995), consisting of "commercial computer software" and "commercial
+ * computer software documentation" as such terms are used in 48
+ * C.F.R. 12.212 (SEPT 1995) and is provided to the U.S. Government
+ * only as a commercial end item.  Consistent with 48 C.F.R.12.212 and
+ * 48 C.F.R. 227.7202-1 through 227.7202-4 (JUNE 1995), all
+ * U.S. Government End Users acquire the Licensed Deliverables with
+ * only those rights set forth herein.
+ *
+ * Any use of the Licensed Deliverables in individual and commercial
+ * software must include, in the user documentation and internal
+ * comments to the code, the above Disclaimer and U.S. Government End
+ * Users Notice.
+ */
+
+#ifndef cuda_profiler_H
+#define cuda_profiler_H
+
+#include <cuda.h>
+
+#if defined(__CUDA_API_VERSION_INTERNAL) || defined(__DOXYGEN_ONLY__) || defined(CUDA_ENABLE_DEPRECATED)
+#define __CUDA_DEPRECATED
+#elif defined(_MSC_VER)
+#define __CUDA_DEPRECATED __declspec(deprecated)
+#elif defined(__GNUC__)
+#define __CUDA_DEPRECATED __attribute__((deprecated))
+#else
+#define __CUDA_DEPRECATED
+#endif
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+/**
+ * Profiler Output Modes
+ */
+/*DEVICE_BUILTIN*/
+typedef enum CUoutput_mode_enum
+{
+    CU_OUT_KEY_VALUE_PAIR  = 0x00, /**< Output mode Key-Value pair format. */
+    CU_OUT_CSV             = 0x01  /**< Output mode Comma separated values format. */
+}CUoutput_mode;
+
+
+/**
+ * \ingroup CUDA_DRIVER
+ * \defgroup CUDA_PROFILER_DEPRECATED Profiler Control [DEPRECATED]
+ *
+ * ___MANBRIEF___ profiler control functions of the low-level CUDA driver API
+ * (___CURRENT_FILE___) ___ENDMANBRIEF___
+ *
+ * This section describes the profiler control functions of the low-level CUDA
+ * driver application programming interface.
+ *
+ * @{
+ */
+
+/**
+ * \brief Initialize the profiling.
+ *
+ * \deprecated
+ *
+ * Note that this function is deprecated and should not be used.
+ * Starting with CUDA 12.0, it always returns error code ::CUDA_ERROR_NOT_SUPPORTED.
+ * 
+ * Using this API user can initialize the CUDA profiler by specifying
+ * the configuration file, output file and output file format. This
+ * API is generally used to profile different set of counters by
+ * looping the kernel launch. The \p configFile parameter can be used
+ * to select profiling options including profiler counters. Refer to
+ * the "Compute Command Line Profiler User Guide" for supported
+ * profiler options and counters.
+ *
+ * Limitation: The CUDA profiler cannot be initialized with this API
+ * if another profiling tool is already active, as indicated by the
+ * ::CUDA_ERROR_PROFILER_DISABLED return code.
+ *
+ * Typical usage of the profiling APIs is as follows: 
+ *
+ * for each set of counters/options\n
+ * {\n
+ *     cuProfilerInitialize(); //Initialize profiling, set the counters or options in the config file \n
+ *     ...\n
+ *     cuProfilerStart(); \n
+ *     // code to be profiled \n
+ *     cuProfilerStop(); \n
+ *     ...\n
+ *     cuProfilerStart(); \n
+ *     // code to be profiled \n
+ *     cuProfilerStop(); \n
+ *     ...\n
+ * }\n
+ *
+ * \param configFile - Name of the config file that lists the counters/options
+ * for profiling.
+ * \param outputFile - Name of the outputFile where the profiling results will
+ * be stored.
+ * \param outputMode - outputMode, can be ::CU_OUT_KEY_VALUE_PAIR or ::CU_OUT_CSV.
+ *
+ * \return
+ * ::CUDA_ERROR_NOT_SUPPORTED
+ * \notefnerr
+ *
+ * \sa
+ * ::cuProfilerStart,
+ * ::cuProfilerStop,
+ */
+__CUDA_DEPRECATED CUresult CUDAAPI cuProfilerInitialize(const char *configFile, const char *outputFile, CUoutput_mode outputMode);
+ 
+/** @} */ /* END CUDA_PROFILER_DEPRECATED */
+
+/**
+ * \ingroup CUDA_DRIVER
+ * \defgroup CUDA_PROFILER Profiler Control 
+ *
+ * ___MANBRIEF___ profiler control functions of the low-level CUDA driver API
+ * (___CURRENT_FILE___) ___ENDMANBRIEF___
+ *
+ * This section describes the profiler control functions of the low-level CUDA
+ * driver application programming interface.
+ *
+ * @{
+ */
+
+/**
+ * \brief Enable profiling.
+ *
+ * Enables profile collection by the active profiling tool for the
+ * current context. If profiling is already enabled, then
+ * cuProfilerStart() has no effect.
+ *
+ * cuProfilerStart and cuProfilerStop APIs are used to
+ * programmatically control the profiling granularity by allowing
+ * profiling to be done only on selective pieces of code.
+ * 
+ *
+ * \return
+ * ::CUDA_SUCCESS,
+ * ::CUDA_ERROR_INVALID_CONTEXT
+ * \notefnerr
+ *
+ * \sa
+ * ::cuProfilerInitialize,
+ * ::cuProfilerStop,
+ * ::cudaProfilerStart
+ */
+CUresult CUDAAPI cuProfilerStart(void);
+
+/**
+ * \brief Disable profiling.
+ *
+ * Disables profile collection by the active profiling tool for the
+ * current context. If profiling is already disabled, then
+ * cuProfilerStop() has no effect.
+ *
+ * cuProfilerStart and cuProfilerStop APIs are used to
+ * programmatically control the profiling granularity by allowing
+ * profiling to be done only on selective pieces of code.
+ *
+ * \return
+ * ::CUDA_SUCCESS,
+ * ::CUDA_ERROR_INVALID_CONTEXT
+ * \notefnerr
+ *
+ * \sa
+ * ::cuProfilerInitialize,
+ * ::cuProfilerStart,
+ * ::cudaProfilerStop
+ */
+CUresult CUDAAPI cuProfilerStop(void);
+
+/** @} */ /* END CUDA_PROFILER */
+
+#ifdef __cplusplus
+};
+#endif
+
+#undef __CUDA_DEPRECATED
+
+#endif
+
```

## nvidia/cuda_profiler_api/include/cuda_profiler_api.h

 * *Ordering differences only*

```diff
@@ -1,134 +1,134 @@
-/*
- * Copyright 1993-2012 NVIDIA Corporation.  All rights reserved.
- *
- * NOTICE TO LICENSEE:
- *
- * This source code and/or documentation ("Licensed Deliverables") are
- * subject to NVIDIA intellectual property rights under U.S. and
- * international Copyright laws.
- *
- * These Licensed Deliverables contained herein is PROPRIETARY and
- * CONFIDENTIAL to NVIDIA and is being provided under the terms and
- * conditions of a form of NVIDIA software license agreement by and
- * between NVIDIA and Licensee ("License Agreement") or electronically
- * accepted by Licensee.  Notwithstanding any terms or conditions to
- * the contrary in the License Agreement, reproduction or disclosure
- * of the Licensed Deliverables to any third party without the express
- * written consent of NVIDIA is prohibited.
- *
- * NOTWITHSTANDING ANY TERMS OR CONDITIONS TO THE CONTRARY IN THE
- * LICENSE AGREEMENT, NVIDIA MAKES NO REPRESENTATION ABOUT THE
- * SUITABILITY OF THESE LICENSED DELIVERABLES FOR ANY PURPOSE.  IT IS
- * PROVIDED "AS IS" WITHOUT EXPRESS OR IMPLIED WARRANTY OF ANY KIND.
- * NVIDIA DISCLAIMS ALL WARRANTIES WITH REGARD TO THESE LICENSED
- * DELIVERABLES, INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY,
- * NONINFRINGEMENT, AND FITNESS FOR A PARTICULAR PURPOSE.
- * NOTWITHSTANDING ANY TERMS OR CONDITIONS TO THE CONTRARY IN THE
- * LICENSE AGREEMENT, IN NO EVENT SHALL NVIDIA BE LIABLE FOR ANY
- * SPECIAL, INDIRECT, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, OR ANY
- * DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS,
- * WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
- * ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE
- * OF THESE LICENSED DELIVERABLES.
- *
- * U.S. Government End Users.  These Licensed Deliverables are a
- * "commercial item" as that term is defined at 48 C.F.R. 2.101 (OCT
- * 1995), consisting of "commercial computer software" and "commercial
- * computer software documentation" as such terms are used in 48
- * C.F.R. 12.212 (SEPT 1995) and is provided to the U.S. Government
- * only as a commercial end item.  Consistent with 48 C.F.R.12.212 and
- * 48 C.F.R. 227.7202-1 through 227.7202-4 (JUNE 1995), all
- * U.S. Government End Users acquire the Licensed Deliverables with
- * only those rights set forth herein.
- *
- * Any use of the Licensed Deliverables in individual and commercial
- * software must include, in the user documentation and internal
- * comments to the code, the above Disclaimer and U.S. Government End
- * Users Notice.
- */
-
-#if !defined(__CUDA_PROFILER_API_H__)
-#define __CUDA_PROFILER_API_H__
-
-#include "driver_types.h"
-
-#if defined(__CUDA_API_VERSION_INTERNAL) || defined(__DOXYGEN_ONLY__) || defined(CUDA_ENABLE_DEPRECATED)
-#define __CUDA_DEPRECATED
-#elif defined(_MSC_VER)
-#define __CUDA_DEPRECATED __declspec(deprecated)
-#elif defined(__GNUC__)
-#define __CUDA_DEPRECATED __attribute__((deprecated))
-#else
-#define __CUDA_DEPRECATED
-#endif
-
-#if defined(__cplusplus)
-extern "C" {
-#endif /* __cplusplus */
-
-/**
- * \ingroup CUDART
- * \defgroup CUDART_PROFILER Profiler Control
- *
- * ___MANBRIEF___ profiler control functions of the CUDA runtime API
- * (___CURRENT_FILE___) ___ENDMANBRIEF___
- *
- * This section describes the profiler control functions of the CUDA runtime
- * application programming interface.
- *
- * @{
- */
-
-/**
- * \brief Enable profiling.
- *
- * Enables profile collection by the active profiling tool for the
- * current context. If profiling is already enabled, then
- * cudaProfilerStart() has no effect.
- *
- * cudaProfilerStart and cudaProfilerStop APIs are used to
- * programmatically control the profiling granularity by allowing
- * profiling to be done only on selective pieces of code.
- * 
- *
- * \return
- * ::cudaSuccess
- * \notefnerr
- *
- * \sa
- * ::cudaProfilerStop,
- * ::cuProfilerStart
- */
-extern __host__ cudaError_t CUDARTAPI cudaProfilerStart(void);
-
-/**
- * \brief Disable profiling.
- *
- * Disables profile collection by the active profiling tool for the
- * current context. If profiling is already disabled, then
- * cudaProfilerStop() has no effect.
- *
- * cudaProfilerStart and cudaProfilerStop APIs are used to
- * programmatically control the profiling granularity by allowing
- * profiling to be done only on selective pieces of code.
- *
- * \return
- * ::cudaSuccess
- * \notefnerr
- *
- * \sa
- * ::cudaProfilerStart,
- * ::cuProfilerStop
- */
-extern __host__ cudaError_t CUDARTAPI cudaProfilerStop(void);
-
-/** @} */ /* END CUDART_PROFILER */
-
-#undef __CUDA_DEPRECATED
-
-#if defined(__cplusplus)
-}
-#endif /* __cplusplus */
-
-#endif /* !__CUDA_PROFILER_API_H__ */
-
+/*
+ * Copyright 1993-2012 NVIDIA Corporation.  All rights reserved.
+ *
+ * NOTICE TO LICENSEE:
+ *
+ * This source code and/or documentation ("Licensed Deliverables") are
+ * subject to NVIDIA intellectual property rights under U.S. and
+ * international Copyright laws.
+ *
+ * These Licensed Deliverables contained herein is PROPRIETARY and
+ * CONFIDENTIAL to NVIDIA and is being provided under the terms and
+ * conditions of a form of NVIDIA software license agreement by and
+ * between NVIDIA and Licensee ("License Agreement") or electronically
+ * accepted by Licensee.  Notwithstanding any terms or conditions to
+ * the contrary in the License Agreement, reproduction or disclosure
+ * of the Licensed Deliverables to any third party without the express
+ * written consent of NVIDIA is prohibited.
+ *
+ * NOTWITHSTANDING ANY TERMS OR CONDITIONS TO THE CONTRARY IN THE
+ * LICENSE AGREEMENT, NVIDIA MAKES NO REPRESENTATION ABOUT THE
+ * SUITABILITY OF THESE LICENSED DELIVERABLES FOR ANY PURPOSE.  IT IS
+ * PROVIDED "AS IS" WITHOUT EXPRESS OR IMPLIED WARRANTY OF ANY KIND.
+ * NVIDIA DISCLAIMS ALL WARRANTIES WITH REGARD TO THESE LICENSED
+ * DELIVERABLES, INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY,
+ * NONINFRINGEMENT, AND FITNESS FOR A PARTICULAR PURPOSE.
+ * NOTWITHSTANDING ANY TERMS OR CONDITIONS TO THE CONTRARY IN THE
+ * LICENSE AGREEMENT, IN NO EVENT SHALL NVIDIA BE LIABLE FOR ANY
+ * SPECIAL, INDIRECT, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, OR ANY
+ * DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS,
+ * WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+ * ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE
+ * OF THESE LICENSED DELIVERABLES.
+ *
+ * U.S. Government End Users.  These Licensed Deliverables are a
+ * "commercial item" as that term is defined at 48 C.F.R. 2.101 (OCT
+ * 1995), consisting of "commercial computer software" and "commercial
+ * computer software documentation" as such terms are used in 48
+ * C.F.R. 12.212 (SEPT 1995) and is provided to the U.S. Government
+ * only as a commercial end item.  Consistent with 48 C.F.R.12.212 and
+ * 48 C.F.R. 227.7202-1 through 227.7202-4 (JUNE 1995), all
+ * U.S. Government End Users acquire the Licensed Deliverables with
+ * only those rights set forth herein.
+ *
+ * Any use of the Licensed Deliverables in individual and commercial
+ * software must include, in the user documentation and internal
+ * comments to the code, the above Disclaimer and U.S. Government End
+ * Users Notice.
+ */
+
+#if !defined(__CUDA_PROFILER_API_H__)
+#define __CUDA_PROFILER_API_H__
+
+#include "driver_types.h"
+
+#if defined(__CUDA_API_VERSION_INTERNAL) || defined(__DOXYGEN_ONLY__) || defined(CUDA_ENABLE_DEPRECATED)
+#define __CUDA_DEPRECATED
+#elif defined(_MSC_VER)
+#define __CUDA_DEPRECATED __declspec(deprecated)
+#elif defined(__GNUC__)
+#define __CUDA_DEPRECATED __attribute__((deprecated))
+#else
+#define __CUDA_DEPRECATED
+#endif
+
+#if defined(__cplusplus)
+extern "C" {
+#endif /* __cplusplus */
+
+/**
+ * \ingroup CUDART
+ * \defgroup CUDART_PROFILER Profiler Control
+ *
+ * ___MANBRIEF___ profiler control functions of the CUDA runtime API
+ * (___CURRENT_FILE___) ___ENDMANBRIEF___
+ *
+ * This section describes the profiler control functions of the CUDA runtime
+ * application programming interface.
+ *
+ * @{
+ */
+
+/**
+ * \brief Enable profiling.
+ *
+ * Enables profile collection by the active profiling tool for the
+ * current context. If profiling is already enabled, then
+ * cudaProfilerStart() has no effect.
+ *
+ * cudaProfilerStart and cudaProfilerStop APIs are used to
+ * programmatically control the profiling granularity by allowing
+ * profiling to be done only on selective pieces of code.
+ * 
+ *
+ * \return
+ * ::cudaSuccess
+ * \notefnerr
+ *
+ * \sa
+ * ::cudaProfilerStop,
+ * ::cuProfilerStart
+ */
+extern __host__ cudaError_t CUDARTAPI cudaProfilerStart(void);
+
+/**
+ * \brief Disable profiling.
+ *
+ * Disables profile collection by the active profiling tool for the
+ * current context. If profiling is already disabled, then
+ * cudaProfilerStop() has no effect.
+ *
+ * cudaProfilerStart and cudaProfilerStop APIs are used to
+ * programmatically control the profiling granularity by allowing
+ * profiling to be done only on selective pieces of code.
+ *
+ * \return
+ * ::cudaSuccess
+ * \notefnerr
+ *
+ * \sa
+ * ::cudaProfilerStart,
+ * ::cuProfilerStop
+ */
+extern __host__ cudaError_t CUDARTAPI cudaProfilerStop(void);
+
+/** @} */ /* END CUDART_PROFILER */
+
+#undef __CUDA_DEPRECATED
+
+#if defined(__cplusplus)
+}
+#endif /* __cplusplus */
+
+#endif /* !__CUDA_PROFILER_API_H__ */
+
```

## Comparing `nvidia_cuda_profiler_api_cu12-12.1.105.dist-info/License.txt` & `nvidia_cuda_profiler_api_cu12-12.1.55.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `nvidia_cuda_profiler_api_cu12-12.1.105.dist-info/METADATA` & `nvidia_cuda_profiler_api_cu12-12.1.55.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-cuda-profiler-api-cu12
-Version: 12.1.105
+Version: 12.1.55
 Summary: CUDA Profiler API
 Home-page: https://developer.nvidia.com/cuda-zone
 Author: Nvidia CUDA Installer Team
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Keywords: cuda,nvidia,runtime,machine learning,deep learning
 Classifier: Development Status :: 4 - Beta
```

