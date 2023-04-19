# Comparing `tmp/nvidia_nvml_dev_cu12-12.1.105-py3-none-manylinux1_x86_64.whl.zip` & `tmp/nvidia_nvml_dev_cu12-12.1.55-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 91252 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 01:00 nvidia/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 01:00 nvidia/nvml_dev/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 01:00 nvidia/nvml_dev/include/__init__.py
--rw-r--r--  2.0 unx   502979 b- defN 23-Apr-04 01:00 nvidia/nvml_dev/include/nvml.h
--rw-r--r--  2.0 unx    59262 b- defN 23-Apr-04 01:00 nvidia_nvml_dev_cu12-12.1.105.dist-info/License.txt
--rw-r--r--  2.0 unx     1505 b- defN 23-Apr-04 01:00 nvidia_nvml_dev_cu12-12.1.105.dist-info/METADATA
--rw-r--r--  2.0 unx      106 b- defN 23-Apr-04 01:00 nvidia_nvml_dev_cu12-12.1.105.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-04 01:00 nvidia_nvml_dev_cu12-12.1.105.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      802 b- defN 23-Apr-04 01:00 nvidia_nvml_dev_cu12-12.1.105.dist-info/RECORD
-9 files, 564661 bytes uncompressed, 89840 bytes compressed:  84.1%
+Zip file size: 104859 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 23-Jan-25 04:53 nvidia/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jan-25 04:53 nvidia/nvml_dev/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jan-25 04:53 nvidia/nvml_dev/include/__init__.py
+-rw-r--r--  2.0 unx   502957 b- defN 23-Jan-25 04:53 nvidia/nvml_dev/include/nvml.h
+-rw-r--r--  2.0 unx    83052 b- defN 23-Jan-25 04:53 nvidia/nvml_dev/lib/x64/nvml.lib
+-rw-r--r--  2.0 unx    59262 b- defN 23-Jan-25 04:53 nvidia_nvml_dev_cu12-12.1.55.dist-info/License.txt
+-rw-r--r--  2.0 unx     1504 b- defN 23-Jan-25 04:53 nvidia_nvml_dev_cu12-12.1.55.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 23-Jan-25 04:53 nvidia_nvml_dev_cu12-12.1.55.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jan-25 04:53 nvidia_nvml_dev_cu12-12.1.55.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      886 b- defN 23-Jan-25 04:53 nvidia_nvml_dev_cu12-12.1.55.dist-info/RECORD
+10 files, 647766 bytes uncompressed, 103317 bytes compressed:  84.1%
```

## zipnote {}

```diff
@@ -6,23 +6,26 @@
 
 Filename: nvidia/nvml_dev/include/__init__.py
 Comment: 
 
 Filename: nvidia/nvml_dev/include/nvml.h
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.1.105.dist-info/License.txt
+Filename: nvidia/nvml_dev/lib/x64/nvml.lib
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.1.105.dist-info/METADATA
+Filename: nvidia_nvml_dev_cu12-12.1.55.dist-info/License.txt
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.1.105.dist-info/WHEEL
+Filename: nvidia_nvml_dev_cu12-12.1.55.dist-info/METADATA
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.1.105.dist-info/top_level.txt
+Filename: nvidia_nvml_dev_cu12-12.1.55.dist-info/WHEEL
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.1.105.dist-info/RECORD
+Filename: nvidia_nvml_dev_cu12-12.1.55.dist-info/top_level.txt
+Comment: 
+
+Filename: nvidia_nvml_dev_cu12-12.1.55.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nvidia/nvml_dev/include/nvml.h

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright 1993-2023 NVIDIA Corporation.  All rights reserved.
+ * Copyright 1993-2022 NVIDIA Corporation.  All rights reserved.
  *
  * NOTICE TO USER:
  *
  * This source code is subject to NVIDIA ownership rights under U.S. and
  * international Copyright laws.  Users and possessors of this source code
  * are hereby granted a nonexclusive, royalty-free license to use this code
  * in individual and commercial software.
@@ -2055,15 +2055,15 @@
 /***************************************************************************************************/
 
 /**
  * Represents frame buffer capture session type
  */
 typedef enum nvmlFBCSessionType_enum
 {
-    NVML_FBC_SESSION_TYPE_UNKNOWN = 0,     //!< Unknown
+    NVML_FBC_SESSION_TYPE_UNKNOWN = 0,     //!< Unknwon
     NVML_FBC_SESSION_TYPE_TOSYS,           //!< ToSys
     NVML_FBC_SESSION_TYPE_CUDA,            //!< Cuda
     NVML_FBC_SESSION_TYPE_VID,             //!< Vid
     NVML_FBC_SESSION_TYPE_HWENC            //!< HEnc
 } nvmlFBCSessionType_t;
 
 /**
@@ -4707,18 +4707,18 @@
 nvmlReturn_t DECLDIR nvmlDeviceGetEncoderStats (nvmlDevice_t device, unsigned int *sessionCount,
                                                 unsigned int *averageFps, unsigned int *averageLatency);
 
 /**
  * Retrieves information about active encoder sessions on a target device.
  *
  * An array of active encoder sessions is returned in the caller-supplied buffer pointed at by \a sessionInfos. The
- * array element count is passed in \a sessionCount, and \a sessionCount is used to return the number of sessions
+ * array elememt count is passed in \a sessionCount, and \a sessionCount is used to return the number of sessions
  * written to the buffer.
  *
- * If the supplied buffer is not large enough to accommodate the active session array, the function returns
+ * If the supplied buffer is not large enough to accomodate the active session array, the function returns
  * NVML_ERROR_INSUFFICIENT_SIZE, with the element count of nvmlEncoderSessionInfo_t array required in \a sessionCount.
  * To query the number of active encoder sessions, call this function with *sessionCount = 0.  The code will return
  * NVML_SUCCESS with number of active encoder sessions updated in *sessionCount.
  *
  * For Maxwell &tm; or newer fully supported devices.
  *
  * @param device                            The identifier of the target device
@@ -4759,15 +4759,15 @@
 
 /**
 * Retrieves the active frame buffer capture sessions statistics for a given device.
 *
 * For Maxwell &tm; or newer fully supported devices.
 *
 * @param device                            The identifier of the target device
-* @param fbcStats                          Reference to nvmlFBCStats_t structure containing NvFBC stats
+* @param fbcStats                          Reference to nvmlFBCStats_t structure contianing NvFBC stats
 *
 * @return
 *         - \ref NVML_SUCCESS                  if \a fbcStats is fetched
 *         - \ref NVML_ERROR_UNINITIALIZED      if the library has not been successfully initialized
 *         - \ref NVML_ERROR_INVALID_ARGUMENT   if \a fbcStats is NULL
 *         - \ref NVML_ERROR_GPU_IS_LOST        if the target GPU has fallen off the bus or is otherwise inaccessible
 *         - \ref NVML_ERROR_UNKNOWN            on any unexpected error
@@ -4777,15 +4777,15 @@
 /**
 * Retrieves information about active frame buffer capture sessions on a target device.
 *
 * An array of active FBC sessions is returned in the caller-supplied buffer pointed at by \a sessionInfo. The
 * array element count is passed in \a sessionCount, and \a sessionCount is used to return the number of sessions
 * written to the buffer.
 *
-* If the supplied buffer is not large enough to accommodate the active session array, the function returns
+* If the supplied buffer is not large enough to accomodate the active session array, the function returns
 * NVML_ERROR_INSUFFICIENT_SIZE, with the element count of nvmlFBCSessionInfo_t array required in \a sessionCount.
 * To query the number of active FBC sessions, call this function with *sessionCount = 0.  The code will return
 * NVML_SUCCESS with number of active FBC sessions updated in *sessionCount.
 *
 * For Maxwell &tm; or newer fully supported devices.
 *
 * @note hResolution, vResolution, averageFPS and averageLatency data for a FBC session returned in \a sessionInfo may
@@ -5416,15 +5416,15 @@
     unsigned int *pageCount, unsigned long long *addresses);
 
 /**
  * Returns the list of retired pages by source, including pages that are pending retirement
  * The address information provided from this API is the hardware address of the page that was retired.  Note
  * that this does not match the virtual address used in CUDA, but will match the address information in XID 63
  *
- * \note nvmlDeviceGetRetiredPages_v2 adds an additional timestamps parameter to return the time of each page's
+ * \note nvmlDeviceGetRetiredPages_v2 adds an additional timestamps paramter to return the time of each page's
  *       retirement.
  *
  * For Kepler &tm; or newer fully supported devices.
  *
  * @param device                            The identifier of the target device
  * @param cause                             Filter page addresses by cause of retirement
  * @param pageCount                         Reference in which to provide the \a addresses buffer size, and
@@ -5753,15 +5753,15 @@
     NVML_CLOCK_LIMIT_ID_UNLIMITED
 } nvmlClockLimitId_t;
 
 /**
  * Set clocks that device will lock to.
  *
  * Sets the clocks that the device will be running at to the value in the range of minGpuClockMHz to maxGpuClockMHz.
- * Setting this will supersede application clock values and take effect regardless if a cuda app is running.
+ * Setting this will supercede application clock values and take effect regardless if a cuda app is running.
  * See /ref nvmlDeviceSetApplicationsClocks
  *
  * Can be used as a setting to request constant performance.
  *
  * This can be called with a pair of integer clock frequencies in MHz, or a pair of /ref nvmlClockLimitId_t values.
  * See the table below for valid combinations of these values.
  *
@@ -6870,15 +6870,15 @@
 /**
  * Retrieve the supported vGPU types on a physical GPU (device).
  *
  * An array of supported vGPU types for the physical GPU indicated by \a device is returned in the caller-supplied buffer
  * pointed at by \a vgpuTypeIds. The element count of nvmlVgpuTypeId_t array is passed in \a vgpuCount, and \a vgpuCount
  * is used to return the number of vGPU types written to the buffer.
  *
- * If the supplied buffer is not large enough to accommodate the vGPU type array, the function returns
+ * If the supplied buffer is not large enough to accomodate the vGPU type array, the function returns
  * NVML_ERROR_INSUFFICIENT_SIZE, with the element count of nvmlVgpuTypeId_t array required in \a vgpuCount.
  * To query the number of vGPU types supported for the GPU, call this function with *vgpuCount = 0.
  * The code will return NVML_ERROR_INSUFFICIENT_SIZE, or NVML_SUCCESS if no vGPU types are supported.
  *
  * @param device                   The identifier of the target device
  * @param vgpuCount                Pointer to caller-supplied array size, and returns number of vGPU types
  * @param vgpuTypeIds              Pointer to caller-supplied array in which to return list of vGPU types
@@ -6899,17 +6899,17 @@
  * pointed at by \a vgpuTypeIds. The element count of nvmlVgpuTypeId_t array is passed in \a vgpuCount, and \a vgpuCount
  * is used to return the number of vGPU types written to the buffer.
  *
  * The creatable vGPU types for a device may differ over time, as there may be restrictions on what type of vGPU types
  * can concurrently run on a device.  For example, if only one vGPU type is allowed at a time on a device, then the creatable
  * list will be restricted to whatever vGPU type is already running on the device.
  *
- * If the supplied buffer is not large enough to accommodate the vGPU type array, the function returns
+ * If the supplied buffer is not large enough to accomodate the vGPU type array, the function returns
  * NVML_ERROR_INSUFFICIENT_SIZE, with the element count of nvmlVgpuTypeId_t array required in \a vgpuCount.
- * To query the number of vGPU types that can be created for the GPU, call this function with *vgpuCount = 0.
+ * To query the number of vGPU types createable for the GPU, call this function with *vgpuCount = 0.
  * The code will return NVML_ERROR_INSUFFICIENT_SIZE, or NVML_SUCCESS if no vGPU types are creatable.
  *
  * @param device                   The identifier of the target device
  * @param vgpuCount                Pointer to caller-supplied array size, and returns number of vGPU types
  * @param vgpuTypeIds              Pointer to caller-supplied array in which to return list of vGPU types
  *
  * @return
@@ -6981,15 +6981,15 @@
 /**
  * Retrieve the device ID of a vGPU type.
  *
  * For Kepler &tm; or newer fully supported devices.
  *
  * @param vgpuTypeId               Handle to vGPU type
  * @param deviceID                 Device ID and vendor ID of the device contained in single 32 bit value
- * @param subsystemID              Subsystem ID and subsystem vendor ID of the device contained in single 32 bit value
+ * @param subsystemID              Subsytem ID and subsytem vendor ID of the device contained in single 32 bit value
  *
  * @return
  *         - \ref NVML_SUCCESS                 successful completion
  *         - \ref NVML_ERROR_UNINITIALIZED     if the library has not been successfully initialized
  *         - \ref NVML_ERROR_INVALID_ARGUMENT  if \a vgpuTypeId is invalid, or \a deviceId or \a subsystemID are NULL
  *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
  */
@@ -7120,18 +7120,18 @@
  */
 nvmlReturn_t DECLDIR nvmlVgpuTypeGetMaxInstancesPerVm(nvmlVgpuTypeId_t vgpuTypeId, unsigned int *vgpuInstanceCountPerVm);
 
 /**
  * Retrieve the active vGPU instances on a device.
  *
  * An array of active vGPU instances is returned in the caller-supplied buffer pointed at by \a vgpuInstances. The
- * array element count is passed in \a vgpuCount, and \a vgpuCount is used to return the number of vGPU instances
+ * array elememt count is passed in \a vgpuCount, and \a vgpuCount is used to return the number of vGPU instances
  * written to the buffer.
  *
- * If the supplied buffer is not large enough to accommodate the vGPU instance array, the function returns
+ * If the supplied buffer is not large enough to accomodate the vGPU instance array, the function returns
  * NVML_ERROR_INSUFFICIENT_SIZE, with the element count of nvmlVgpuInstance_t array required in \a vgpuCount.
  * To query the number of active vGPU instances, call this function with *vgpuCount = 0.  The code will return
  * NVML_ERROR_INSUFFICIENT_SIZE, or NVML_SUCCESS if no vGPU Types are supported.
  *
  * For Kepler &tm; or newer fully supported devices.
  *
  * @param device                   The identifier of the target device
@@ -7324,15 +7324,15 @@
  *
  * For Maxwell &tm; or newer fully supported devices.
  *
  * @param vgpuInstance             Identifier of the target vGPU instance
  * @param encoderCapacity          Reference to an unsigned int for the encoder capacity
  *
  * @return
- *         - \ref NVML_SUCCESS                 if \a encoderCapacity has been retrieved
+ *         - \ref NVML_SUCCESS                 if \a encoderCapacity has been retrived
  *         - \ref NVML_ERROR_UNINITIALIZED     if the library has not been successfully initialized
  *         - \ref NVML_ERROR_INVALID_ARGUMENT  if \a vgpuInstance is 0, or \a encoderQueryType is invalid
  *         - \ref NVML_ERROR_NOT_FOUND         if \a vgpuInstance does not match a valid active vGPU instance on the system
  *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
  */
 nvmlReturn_t DECLDIR nvmlVgpuInstanceGetEncoderCapacity(nvmlVgpuInstance_t vgpuInstance, unsigned int *encoderCapacity);
 
@@ -7377,15 +7377,15 @@
 /**
  * Retrieves information about all active encoder sessions on a vGPU Instance.
  *
  * An array of active encoder sessions is returned in the caller-supplied buffer pointed at by \a sessionInfo. The
  * array element count is passed in \a sessionCount, and \a sessionCount is used to return the number of sessions
  * written to the buffer.
  *
- * If the supplied buffer is not large enough to accommodate the active session array, the function returns
+ * If the supplied buffer is not large enough to accomodate the active session array, the function returns
  * NVML_ERROR_INSUFFICIENT_SIZE, with the element count of nvmlEncoderSessionInfo_t array required in \a sessionCount.
  * To query the number of active encoder sessions, call this function with *sessionCount = 0. The code will return
  * NVML_SUCCESS with number of active encoder sessions updated in *sessionCount.
  *
  * For Maxwell &tm; or newer fully supported devices.
  *
  * @param vgpuInstance                      Identifier of the target vGPU instance
@@ -7407,15 +7407,15 @@
 
 /**
 * Retrieves the active frame buffer capture sessions statistics of a vGPU Instance
 *
 * For Maxwell &tm; or newer fully supported devices.
 *
 * @param vgpuInstance                      Identifier of the target vGPU instance
-* @param fbcStats                          Reference to nvmlFBCStats_t structure containing NvFBC stats
+* @param fbcStats                          Reference to nvmlFBCStats_t structure contianing NvFBC stats
 *
 * @return
 *         - \ref NVML_SUCCESS                  if \a fbcStats is fetched
 *         - \ref NVML_ERROR_UNINITIALIZED      if the library has not been successfully initialized
 *         - \ref NVML_ERROR_INVALID_ARGUMENT   if \a vgpuInstance is 0, or \a fbcStats is NULL
 *         - \ref NVML_ERROR_NOT_FOUND          if \a vgpuInstance does not match a valid active vGPU instance on the system
 *         - \ref NVML_ERROR_UNKNOWN            on any unexpected error
@@ -7425,15 +7425,15 @@
 /**
 * Retrieves information about active frame buffer capture sessions on a vGPU Instance.
 *
 * An array of active FBC sessions is returned in the caller-supplied buffer pointed at by \a sessionInfo. The
 * array element count is passed in \a sessionCount, and \a sessionCount is used to return the number of sessions
 * written to the buffer.
 *
-* If the supplied buffer is not large enough to accommodate the active session array, the function returns
+* If the supplied buffer is not large enough to accomodate the active session array, the function returns
 * NVML_ERROR_INSUFFICIENT_SIZE, with the element count of nvmlFBCSessionInfo_t array required in \a sessionCount.
 * To query the number of active FBC sessions, call this function with *sessionCount = 0.  The code will return
 * NVML_SUCCESS with number of active FBC sessions updated in *sessionCount.
 *
 * For Maxwell &tm; or newer fully supported devices.
 *
 * @note hResolution, vResolution, averageFPS and averageLatency data for a FBC session returned in \a sessionInfo may
@@ -7535,29 +7535,29 @@
 {
     unsigned int             version;                                                    //!< Current version of the structure
     unsigned int             revision;                                                   //!< Current revision of the structure
     nvmlVgpuGuestInfoState_t guestInfoState;                                             //!< Current state of Guest-dependent fields
     char                     guestDriverVersion[NVML_SYSTEM_DRIVER_VERSION_BUFFER_SIZE]; //!< Version of driver installed in guest
     char                     hostDriverVersion[NVML_SYSTEM_DRIVER_VERSION_BUFFER_SIZE];  //!< Version of driver installed in host
     unsigned int             reserved[6];                                                //!< Reserved for internal use
-    unsigned int             vgpuVirtualizationCaps;                                     //!< vGPU virtualization capabilities bitfield
+    unsigned int             vgpuVirtualizationCaps;                                     //!< vGPU virtualizaion capabilities bitfileld
     unsigned int             guestVgpuVersion;                                           //!< vGPU version of guest driver
     unsigned int             opaqueDataSize;                                             //!< Size of opaque data field in bytes
     char                     opaqueData[4];                                              //!< Opaque data
 } nvmlVgpuMetadata_t;
 
 /**
  * Physical GPU metadata structure
  */
 typedef struct nvmlVgpuPgpuMetadata_st
 {
     unsigned int            version;                                                    //!< Current version of the structure
     unsigned int            revision;                                                   //!< Current revision of the structure
     char                    hostDriverVersion[NVML_SYSTEM_DRIVER_VERSION_BUFFER_SIZE];  //!< Host driver version
-    unsigned int            pgpuVirtualizationCaps;                                     //!< Pgpu virtualization capabilities bitfield
+    unsigned int            pgpuVirtualizationCaps;                                     //!< Pgpu virtualizaion capabilities bitfileld
     unsigned int            reserved[5];                                                //!< Reserved for internal use
     nvmlVgpuVersion_t       hostSupportedVgpuRange;                                     //!< vGPU version range supported by host driver
     unsigned int            opaqueDataSize;                                             //!< Size of opaque data field in bytes
     char                    opaqueData[4];                                              //!< Opaque data
 } nvmlVgpuPgpuMetadata_t;
 
 /**
@@ -7647,15 +7647,15 @@
 /**
  * Takes a vGPU instance metadata structure read from \ref nvmlVgpuInstanceGetMetadata(), and a vGPU metadata structure for a
  * physical GPU read from \ref nvmlDeviceGetVgpuMetadata(), and returns compatibility information of the vGPU instance and the
  * physical GPU.
  *
  * The caller passes in a buffer via \a compatibilityInfo, into which a compatibility information structure is written. The
  * structure defines the states in which the vGPU / VM may be booted on the physical GPU. If the vGPU / VM compatibility
- * with the physical GPU is limited, a limit code indicates the factor limiting compatability.
+ * with the physical GPU is limited, a limit code indicates the factor limiting compability.
  * (see \ref nvmlVgpuPgpuCompatibilityLimitCode_t for details).
  *
  * Note: vGPU compatibility does not take into account dynamic capacity conditions that may limit a system's ability to
  *       boot a given vGPU or associated VM.
  *
  * @param vgpuMetadata          Pointer to caller-supplied vGPU metadata structure
  * @param pgpuMetadata          Pointer to caller-supplied GPU metadata structure
```

## Comparing `nvidia_nvml_dev_cu12-12.1.105.dist-info/License.txt` & `nvidia_nvml_dev_cu12-12.1.55.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `nvidia_nvml_dev_cu12-12.1.105.dist-info/METADATA` & `nvidia_nvml_dev_cu12-12.1.55.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-nvml-dev-cu12
-Version: 12.1.105
+Version: 12.1.55
 Summary: NVML native dev links, headers
 Home-page: https://developer.nvidia.com/cuda-zone
 Author: Nvidia CUDA Installer Team
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Keywords: cuda,nvidia,runtime,machine learning,deep learning
 Classifier: Development Status :: 4 - Beta
```

## Comparing `nvidia_nvml_dev_cu12-12.1.105.dist-info/RECORD` & `nvidia_nvml_dev_cu12-12.1.55.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 nvidia/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nvidia/nvml_dev/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nvidia/nvml_dev/include/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-nvidia/nvml_dev/include/nvml.h,sha256=nH0kuD2kAOD20eQe3tG40o0Dzg7yDvudTKmySnbR5UY,502979
-nvidia_nvml_dev_cu12-12.1.105.dist-info/License.txt,sha256=rW9YU_ugyg0VnQ9Y1JrkmDDC-Mk_epJki5zpCttMbM0,59262
-nvidia_nvml_dev_cu12-12.1.105.dist-info/METADATA,sha256=sZItUCMnbZMF8Yv5smFUNiuNiqh0e8g6N7I5qIG5Ozs,1505
-nvidia_nvml_dev_cu12-12.1.105.dist-info/WHEEL,sha256=-kQi_VMfvRQozZJT7HUPMfY-5vLo0LVTmAylNJ3Ft98,106
-nvidia_nvml_dev_cu12-12.1.105.dist-info/top_level.txt,sha256=fTkAtiFuL16nUrB9ytDDtpytz2t0B4NvYTnRzwAhO14,7
-nvidia_nvml_dev_cu12-12.1.105.dist-info/RECORD,,
+nvidia/nvml_dev/include/nvml.h,sha256=jSXkLSn787yiiv-jZ6itvKiMm2JeAPO6Pbu4B8ioNqA,502957
+nvidia/nvml_dev/lib/x64/nvml.lib,sha256=WHxWYQfTiuxn-LE8ErAuiAKp_UnxgV2_EQuOzCQo6bE,83052
+nvidia_nvml_dev_cu12-12.1.55.dist-info/License.txt,sha256=rW9YU_ugyg0VnQ9Y1JrkmDDC-Mk_epJki5zpCttMbM0,59262
+nvidia_nvml_dev_cu12-12.1.55.dist-info/METADATA,sha256=n1cerROPL_DlSKlw-PgAPHnqA_YvfnfnKd-qyjlJWRs,1504
+nvidia_nvml_dev_cu12-12.1.55.dist-info/WHEEL,sha256=i9qQj8KaD8_YEW0Vc2oS56fKju23RkQ-FVz-QmzVakQ,98
+nvidia_nvml_dev_cu12-12.1.55.dist-info/top_level.txt,sha256=fTkAtiFuL16nUrB9ytDDtpytz2t0B4NvYTnRzwAhO14,7
+nvidia_nvml_dev_cu12-12.1.55.dist-info/RECORD,,
```

