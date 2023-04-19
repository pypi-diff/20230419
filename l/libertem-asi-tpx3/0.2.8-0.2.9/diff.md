# Comparing `tmp/libertem_asi_tpx3-0.2.8.tar.gz` & `tmp/libertem_asi_tpx3-0.2.9.tar.gz`

## Comparing `libertem_asi_tpx3-0.2.8.tar` & `libertem_asi_tpx3-0.2.9.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0      189 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.8/local_dependencies/stats/Cargo.toml
--rw-r--r--   0     1001      123     2581 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/stats/src/lib.rs
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/Cargo.toml
--rw-r--r--   0     1001      123      247 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/README.md
--rw-r--r--   0     1001      123     2815 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/examples/consumer/main.rs
--rw-r--r--   0     1001      123     3772 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/examples/producer/main.rs
--rwxr-xr-x   0     1001      123      121 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/run-consumer.sh
--rwxr-xr-x   0     1001      123      121 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/run-producer.sh
--rw-r--r--   0     1001      123       31 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/rust-toolchain.toml
--rw-r--r--   0     1001      123     6872 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/backend_memfd.rs
--rw-r--r--   0     1001      123     2823 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/backend_shm.rs
--rw-r--r--   0     1001      123     3741 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/freestack.rs
--rw-r--r--   0     1001      123     1029 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/lib.rs
--rw-r--r--   0     1001      123    19891 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/slab.rs
--rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.8/Cargo.toml
--rw-r--r--   0     1001      123      332 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/README.md
--rw-r--r--   0     1001      123    14832 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/acquisition.py
--rw-r--r--   0     1001      123     3363 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/compare.py
--rw-r--r--   0     1001      123     1443 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/crash.py
--rw-r--r--   0     1001      123     1096 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/live_client.py
--rw-r--r--   0     1001      123    12763 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/live_server.py
--rw-r--r--   0     1001      123     1361 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/run_udf.py
--rw-r--r--   0     1001      123     2540 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/sim.py
--rw-r--r--   0     1001      123     2274 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/simple.py
--rw-r--r--   0     1001      123      450 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/pyproject.toml
--rw-r--r--   0     1001      123       31 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/rust-toolchain.toml
--rw-r--r--   0     1001      123     6609 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/cam_client.rs
--rw-r--r--   0     1001      123    25695 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/chunk_stack.rs
--rw-r--r--   0     1001      123      343 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/common.rs
--rw-r--r--   0     1001      123     4293 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/csr_view.rs
--rw-r--r--   0     1001      123     3384 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/csr_view_raw.rs
--rw-r--r--   0     1001      123      987 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/deserialize.rs
--rw-r--r--   0     1001      123      291 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/exceptions.rs
--rw-r--r--   0     1001      123     7487 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/headers.rs
--rw-r--r--   0     1001      123      649 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/headers_py.rs
--rw-r--r--   0     1001      123      280 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/lib.rs
--rw-r--r--   0     1001      123    11265 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/main_py.rs
--rw-r--r--   0     1001      123    22613 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/receiver.rs
--rw-r--r--   0     1001      123      872 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/serialize.rs
--rw-r--r--   0     1001      123    18935 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/sparse_csr.rs
--rw-r--r--   0     1001      123      746 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/stats.rs
--rw-r--r--   0     1001      123     2672 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/stream.rs
--rw-r--r--   0     1001      123    95572 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/Cargo.lock
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/Cargo.toml
+-rw-r--r--   0     1001      123      247 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/README.md
+-rw-r--r--   0     1001      123     2815 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/examples/consumer/main.rs
+-rw-r--r--   0     1001      123     3772 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/examples/producer/main.rs
+-rwxr-xr-x   0     1001      123      121 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/run-consumer.sh
+-rwxr-xr-x   0     1001      123      121 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/run-producer.sh
+-rw-r--r--   0     1001      123       31 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/rust-toolchain.toml
+-rw-r--r--   0     1001      123     6872 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/src/backend_memfd.rs
+-rw-r--r--   0     1001      123     2823 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/src/backend_shm.rs
+-rw-r--r--   0     1001      123     3741 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/src/freestack.rs
+-rw-r--r--   0     1001      123     1029 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/src/lib.rs
+-rw-r--r--   0     1001      123    19891 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/src/slab.rs
+-rw-r--r--   0        0        0      189 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.9/local_dependencies/stats/Cargo.toml
+-rw-r--r--   0     1001      123     2581 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/local_dependencies/stats/src/lib.rs
+-rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.9/Cargo.toml
+-rw-r--r--   0     1001      123      332 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/README.md
+-rw-r--r--   0     1001      123     3363 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/examples/compare.py
+-rw-r--r--   0     1001      123     1443 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/examples/crash.py
+-rw-r--r--   0     1001      123     1096 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/examples/live_client.py
+-rw-r--r--   0     1001      123    12702 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/examples/live_server.py
+-rw-r--r--   0     1001      123     1361 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/examples/run_udf.py
+-rw-r--r--   0     1001      123     2540 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/examples/sim.py
+-rw-r--r--   0     1001      123     2274 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/examples/simple.py
+-rw-r--r--   0     1001      123      450 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/pyproject.toml
+-rw-r--r--   0     1001      123       31 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/rust-toolchain.toml
+-rw-r--r--   0     1001      123     6609 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/cam_client.rs
+-rw-r--r--   0     1001      123    25695 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/chunk_stack.rs
+-rw-r--r--   0     1001      123      343 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/common.rs
+-rw-r--r--   0     1001      123     4293 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/csr_view.rs
+-rw-r--r--   0     1001      123     3384 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/csr_view_raw.rs
+-rw-r--r--   0     1001      123      987 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/deserialize.rs
+-rw-r--r--   0     1001      123      291 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/exceptions.rs
+-rw-r--r--   0     1001      123     7487 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/headers.rs
+-rw-r--r--   0     1001      123      649 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/headers_py.rs
+-rw-r--r--   0     1001      123      280 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/lib.rs
+-rw-r--r--   0     1001      123    11265 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/main_py.rs
+-rw-r--r--   0     1001      123    22613 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/receiver.rs
+-rw-r--r--   0     1001      123      872 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/serialize.rs
+-rw-r--r--   0     1001      123    18935 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/sparse_csr.rs
+-rw-r--r--   0     1001      123      746 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/stats.rs
+-rw-r--r--   0     1001      123     2672 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/src/stream.rs
+-rw-r--r--   0     1001      123    95572 2023-04-19 15:17:41.000000 libertem_asi_tpx3-0.2.9/Cargo.lock
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.9/PKG-INFO
```

### Comparing `libertem_asi_tpx3-0.2.8/local_dependencies/stats/src/lib.rs` & `libertem_asi_tpx3-0.2.9/local_dependencies/stats/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/Cargo.toml` & `libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/Cargo.toml`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/examples/consumer/main.rs` & `libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/examples/consumer/main.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/examples/producer/main.rs` & `libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/examples/producer/main.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/backend_memfd.rs` & `libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/src/backend_memfd.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/backend_shm.rs` & `libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/src/backend_shm.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/freestack.rs` & `libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/src/freestack.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/lib.rs` & `libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/slab.rs` & `libertem_asi_tpx3-0.2.9/local_dependencies/ipc-test/src/slab.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/Cargo.toml` & `libertem_asi_tpx3-0.2.9/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 name = "libertem-asi-tpx3"
 authors = ["Alexander Clausen <a.clausen@fz-juelich.de>"]
 license = "MIT"
-version = "0.2.8"
+version = "0.2.9"
 edition = "2021"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "libertem_asi_tpx3"
 crate-type = ["cdylib"]
```

### Comparing `libertem_asi_tpx3-0.2.8/examples/compare.py` & `libertem_asi_tpx3-0.2.9/examples/compare.py`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/examples/crash.py` & `libertem_asi_tpx3-0.2.9/examples/crash.py`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/examples/live_client.py` & `libertem_asi_tpx3-0.2.9/examples/live_client.py`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/examples/live_server.py` & `libertem_asi_tpx3-0.2.9/examples/live_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from libertem.udf.sumsigudf import SumSigUDF
 from libertem.udf.masks import ApplyMasksUDF
 from libertem.executor.pipelined import PipelinedExecutor
 from libertem_live.api import LiveContext
 from libertem_live.udf.monitor import (
     SignalMonitorUDF, PartitionMonitorUDF
 )
-from acquisition import AsiAcquisition, AsiDetectorConnection
 
 from libertem.udf.base import UDFResults, UDF
 from libertem.common.async_utils import sync_to_async
 
 if typing.TYPE_CHECKING:
     from libertem.common.executor import JobExecutor
 
@@ -258,15 +257,15 @@
             "event": "ACQUISITION_ENDED",
             "id": acq_id,
         }))
 
     async def handle_partial_result(
         self,
         partial_results: UDFResults,
-        pending_acq,
+        pending_aq,
         acq_id: str,
         previous_results: typing.Optional[UDFResults]
     ):
         deltas = await self.make_deltas(partial_results, previous_results)
 
         delta_results: typing.List[EncodedResult] = []
         for delta in deltas:
@@ -295,74 +294,74 @@
         }))
         for result in delta_results:
             await self.broadcast(result.compressed_data)
 
     async def acquisition_loop(self):
         min_delta = 0.05
         while True:
-            pending_acq = await sync_to_async(self.conn.wait_for_acquisition, timeout=10)
-            if pending_acq is None:
+            pending_aq = await sync_to_async(self.conn.wait_for_acquisition, timeout=10)
+            if pending_aq is None:
                 continue
             try:
-                acq_id = await self.handle_pending_acquisition(pending_acq)
+                acq_id = await self.handle_pending_acquisition(pending_aq)
                 print(f"acquisition starting with id={acq_id}")
                 t0 = time.perf_counter()
                 previous_results = None
                 partial_results = None
-                aq = self.ctx.prepare_from_pending(
-                    pending_acq,
+                aq = self.ctx.make_acquisition(
                     conn=self.conn,
-                    pending_aq=pending_acq,
+                    pending_aq=pending_aq,
                     frames_per_partition=4*8192,
                 )
                 last_update = 0
                 try:
                     udfs_only = list(self.udfs.values())
                     async for partial_results in self.ctx.run_udf_iter(dataset=aq, udf=udfs_only, sync=False):
                         if time.time() - last_update > min_delta:
-                            await self.handle_partial_result(partial_results, pending_acq, acq_id, previous_results)
+                            await self.handle_partial_result(partial_results, pending_aq, acq_id, previous_results)
                             previous_results = copy.deepcopy(partial_results)
                             last_update = time.time()
-                    await self.handle_partial_result(partial_results, pending_acq, acq_id, previous_results)
+                    await self.handle_partial_result(partial_results, pending_aq, acq_id, previous_results)
                 except Exception as e:
                     import traceback
                     traceback.print_exc()
                     self.ctx.close()
                     self.conn.close()
                     self.connect()
                 previous_results = copy.deepcopy(partial_results)
             finally:
-                await self.handle_acquisition_end(pending_acq, acq_id)
+                await self.handle_acquisition_end(pending_aq, acq_id)
             previous_results = None
             t1 = time.perf_counter()
             print(f"acquisition done with id={acq_id}; took {t1-t0:.3f}s")
 
     async def serve(self):
         async with websockets.serve(self, "localhost", 8444):
             try:
                 await self.acquisition_loop()
             finally:
                 self.conn.close()
                 self.ctx.close()
 
     def connect(self):
-        conn = AsiDetectorConnection(
-            uri="localhost:8283",
-            chunks_per_stack=16,
-            bytes_per_chunk=1500000,
-            num_slots=1000,
-        )
         executor = PipelinedExecutor(
             spec=PipelinedExecutor.make_spec(
                 cpus=range(20), cudas=[]
             ),
             pin_workers=False,
             # delayed_gc=False,
         )
         ctx = LiveContext(executor=executor)
+        conn = ctx.make_connection('asi_tpx3').open(
+            data_host="localhost",
+            data_port=8283,
+            chunks_per_stack=16,
+            bytes_per_chunk=1500000,
+            buffer_size=2048,
+        )
 
         self.conn = conn
         self.executor = executor
         self.ctx = ctx
 
 async def main():
     server = WSServer()
```

### Comparing `libertem_asi_tpx3-0.2.8/examples/run_udf.py` & `libertem_asi_tpx3-0.2.9/examples/run_udf.py`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/examples/sim.py` & `libertem_asi_tpx3-0.2.9/examples/sim.py`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/examples/simple.py` & `libertem_asi_tpx3-0.2.9/examples/simple.py`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/src/cam_client.rs` & `libertem_asi_tpx3-0.2.9/src/cam_client.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/src/chunk_stack.rs` & `libertem_asi_tpx3-0.2.9/src/chunk_stack.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/src/csr_view.rs` & `libertem_asi_tpx3-0.2.9/src/csr_view.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/src/csr_view_raw.rs` & `libertem_asi_tpx3-0.2.9/src/csr_view_raw.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/src/deserialize.rs` & `libertem_asi_tpx3-0.2.9/src/deserialize.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/src/headers.rs` & `libertem_asi_tpx3-0.2.9/src/headers.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/src/headers_py.rs` & `libertem_asi_tpx3-0.2.9/src/headers_py.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/src/main_py.rs` & `libertem_asi_tpx3-0.2.9/src/main_py.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/src/receiver.rs` & `libertem_asi_tpx3-0.2.9/src/receiver.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/src/serialize.rs` & `libertem_asi_tpx3-0.2.9/src/serialize.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/src/sparse_csr.rs` & `libertem_asi_tpx3-0.2.9/src/sparse_csr.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/src/stats.rs` & `libertem_asi_tpx3-0.2.9/src/stats.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/src/stream.rs` & `libertem_asi_tpx3-0.2.9/src/stream.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.8/Cargo.lock` & `libertem_asi_tpx3-0.2.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1654,15 +1654,15 @@
 name = "libc"
 version = "0.2.140"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
 
 [[package]]
 name = "libertem-asi-tpx3"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "bincode",
  "crossbeam",
  "crossbeam-channel",
  "env_logger",
  "ipc-test",
  "log",
@@ -1673,15 +1673,15 @@
  "tempfile",
  "uuid",
  "zerocopy",
 ]
 
 [[package]]
 name = "libertem-dectris"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "bincode",
  "bs_sys",
  "clap 3.2.23",
  "crossbeam",
  "crossbeam-channel",
  "env_logger",
```

### Comparing `libertem_asi_tpx3-0.2.8/PKG-INFO` & `libertem_asi_tpx3-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libertem-asi-tpx3
-Version: 0.2.8
+Version: 0.2.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Author: Alexander Clausen <a.clausen@fz-juelich.de>
 Author-email: Alexander Clausen <a.clausen@fz-juelich.de>
 License: MIT
 Requires-Python: >=3.7
```

