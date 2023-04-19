# Comparing `tmp/llama_rs_python-0.0.1.tar.gz` & `tmp/llama_rs_python-0.0.2.tar.gz`

## Comparing `llama_rs_python-0.0.1.tar` & `llama_rs_python-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      376 1970-01-01 00:00:00.000000 llama_rs_python-0.0.1/Cargo.toml
--rw-r--r--   0     1001      123     2810 2023-04-18 19:06:52.000000 llama_rs_python-0.0.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     3424 2023-04-18 19:06:52.000000 llama_rs_python-0.0.1/.gitignore
--rw-r--r--   0     1001      123     1071 2023-04-18 19:06:52.000000 llama_rs_python-0.0.1/LICENSE
--rw-r--r--   0     1001      123     1513 2023-04-18 19:06:52.000000 llama_rs_python-0.0.1/README.md
--rw-r--r--   0     1001      123     1367 2023-04-18 19:06:52.000000 llama_rs_python-0.0.1/llama_rs_python.pyi
--rw-r--r--   0     1001      123      377 2023-04-18 19:06:52.000000 llama_rs_python-0.0.1/pyproject.toml
--rw-r--r--   0     1001      123     1383 2023-04-18 19:06:52.000000 llama_rs_python-0.0.1/src/configs.rs
--rw-r--r--   0     1001      123     5408 2023-04-18 19:06:52.000000 llama_rs_python-0.0.1/src/lib.rs
--rw-r--r--   0     1001      123     1541 2023-04-18 19:06:52.000000 llama_rs_python-0.0.1/src/logging_utils.rs
--rw-r--r--   0     1001      123      342 2023-04-18 19:06:52.000000 llama_rs_python-0.0.1/src/results.rs
--rw-r--r--   0     1001      123      541 2023-04-18 19:06:52.000000 llama_rs_python-0.0.1/test.py
--rw-r--r--   0     1001      123    11938 2023-04-18 19:07:35.000000 llama_rs_python-0.0.1/Cargo.lock
--rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 llama_rs_python-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      376 1970-01-01 00:00:00.000000 llama_rs_python-0.0.2/Cargo.toml
+-rw-r--r--   0     1001      123     2810 2023-04-19 10:26:55.000000 llama_rs_python-0.0.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     3424 2023-04-19 10:26:55.000000 llama_rs_python-0.0.2/.gitignore
+-rw-r--r--   0     1001      123     1071 2023-04-19 10:26:55.000000 llama_rs_python-0.0.2/LICENSE
+-rw-r--r--   0     1001      123     1864 2023-04-19 10:26:55.000000 llama_rs_python-0.0.2/README.md
+-rw-r--r--   0     1001      123      653 2023-04-19 10:26:55.000000 llama_rs_python-0.0.2/example.py
+-rw-r--r--   0     1001      123     2151 2023-04-19 10:26:55.000000 llama_rs_python-0.0.2/llama_rs_python.pyi
+-rw-r--r--   0     1001      123      724 2023-04-19 10:26:55.000000 llama_rs_python-0.0.2/pyproject.toml
+-rw-r--r--   0     1001      123     3860 2023-04-19 10:26:55.000000 llama_rs_python-0.0.2/src/configs.rs
+-rw-r--r--   0     1001      123      527 2023-04-19 10:26:55.000000 llama_rs_python-0.0.2/src/lib.rs
+-rw-r--r--   0     1001      123     1541 2023-04-19 10:26:55.000000 llama_rs_python-0.0.2/src/logging_utils.rs
+-rw-r--r--   0     1001      123     5186 2023-04-19 10:26:55.000000 llama_rs_python-0.0.2/src/model.rs
+-rw-r--r--   0     1001      123     1263 2023-04-19 10:26:55.000000 llama_rs_python-0.0.2/src/results.rs
+-rw-r--r--   0     1001      123    11938 2023-04-19 10:27:45.000000 llama_rs_python-0.0.2/Cargo.lock
+-rw-r--r--   0        0        0     2551 1970-01-01 00:00:00.000000 llama_rs_python-0.0.2/PKG-INFO
```

### Comparing `llama_rs_python-0.0.1/.github/workflows/CI.yml` & `llama_rs_python-0.0.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `llama_rs_python-0.0.1/.gitignore` & `llama_rs_python-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `llama_rs_python-0.0.1/LICENSE` & `llama_rs_python-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_rs_python-0.0.1/README.md` & `llama_rs_python-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -18,23 +18,24 @@
 ```python 
 from llama_rs_python import Model
 
 #load the model
 model = Model("path/to/model.bin")
 
 #generate
-print(model.generate("The meaning of life is").text)
+print(model.generate("The meaning of life is"))
 ```
 
 The package also supports callbacks to get each token as it is generated.
 The callback-function also supports canceling the generation by returning a `True` value from the pytohn side.
 
 ```python 
-import sys
 from llama_rs_python import Model
+import sys
+from typing import Optional
 
 #load the model
 model = Model("path/to/model.bin")
 
 #define the callback
 def callback(token:str)->Optional[bool]:
     print(token,end="")
@@ -50,13 +51,24 @@
 ```python 
 from llama_rs_python import Model, GenerationConfig
 
 #load the model
 model = Model("path/to/model.bin")
 
 #create a config
-config = GenerationConfig(top_p=0.9)
+config = GenerationConfig(top_p=0.9,seed=1441,max_new_tokens=1024)
 
 #generate
-print(model.generate("The meaning of life is",generation_config=config).text)
+print(model.generate("The meaning of life is",generation_config=config))
 ```
 
+To configure model specific settings the `SessionConfig` class can be used.
+
+```python
+from llama_rs_python import Model, SessionConfig
+
+#define the session
+session_config = SessionConfig(threads=8,context_length=512)
+
+#load the model
+model = Model("path/to/model.bin",session_config=session_config)
+```
```

### Comparing `llama_rs_python-0.0.1/src/lib.rs` & `llama_rs_python-0.0.2/src/model.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,78 @@
 use pyo3::prelude::*;
 
-use llama_rs::{InferenceError, InferenceSessionParameters, TokenUtf8Buffer};
+use llama_rs::{InferenceError, TokenUtf8Buffer};
 use pyo3::exceptions::PyException;
 use pyo3::types::{PyTuple};
 
 use rand::prelude::*;
 use rand_chacha::ChaCha8Rng;
 
-mod logging_utils;
-mod configs;
-mod results;
+use crate::configs;
+use crate::results;
+use crate::logging_utils;
 
 #[pyclass]
-pub struct GenerationResult {}
-
-#[pyclass]
-#[pyo3(text_signature = "(path, context_length=2048, threads=8, batch_size=8, verbose=False,/)")]
 pub struct Model {
     model: llama_rs::Model,
     #[pyo3(get, set)]
-    batch_size: usize,
-    #[pyo3(get, set)]
-    threads: usize,
+    config: configs::SessionConfig,
     #[pyo3(get, set)]
     verbose: bool,
+    #[pyo3(get)]
+    path: String,
 }
 
 //Ok im not even pretending to know what this does
 unsafe impl Send for Model {}
 
 #[pymethods]
 impl Model {
     
     #[new]
-    fn new(path: String, context_length: Option<usize>,threads:Option<usize>,batch_size:Option<usize>,verbose:Option<bool>) -> Self {
+    fn new(path: String, session_config:Option<configs::SessionConfig>,verbose:Option<bool>) -> Self {
         let should_log = verbose.unwrap_or(false);
+        
+        //Build the correct session parameters
+        let default_config = configs::SessionConfig::default();
+        let config_to_use = session_config.unwrap_or(default_config);
+
+        //Load the model
         let model = llama_rs::Model::load(
             &path,
-            context_length.unwrap_or(2048),
+            config_to_use.context_length,
             |load_progress| {
             if should_log{
                 logging_utils::log_load_progress(load_progress)
             }
         }).unwrap();
-        Model { model: model, batch_size: batch_size.unwrap_or(8), threads: threads.unwrap_or(8), verbose: should_log }
+        Model { model: model, config:config_to_use, verbose: should_log, path:path }
     } 
 
-    #[pyo3(text_signature = "(prompt, seed=42, maximum_token_count=256, callback=None, /)")]
     fn generate(
         &self,
         _py: Python,
         prompt: String,
         generation_config: Option<&configs::GenerationConfig>,
-        seed: Option<u64>,
-        maximum_token_count: Option<usize>,
         callback: Option<PyObject>,
     ) -> PyResult<results::GenerationResult> {
 
-        let session_params = InferenceSessionParameters::default();
+        let session_params = self.config.to_llama_rs_params();
         
         //Build the correct generation parameters
         let default_config = configs::GenerationConfig::default();
         let config_to_use = generation_config.unwrap_or(&default_config);
 
-        let generation_params = config_to_use.to_llama_rs_params(self.threads, self.batch_size);
-
-        let mut session = self.model.start_session(session_params);
+        let generation_params = config_to_use.to_llama_rs_params(self.config.threads,  self.config.batch_size);
 
-        let mut rng = ChaCha8Rng::seed_from_u64(seed.unwrap_or(42));
+        let mut rng = ChaCha8Rng::seed_from_u64(config_to_use.seed);
         let prompt = prompt.as_str();
 
+        let mut session = self.model.start_session(session_params);
+
         //Extract the callback function from the python object
         let mut callback_function: Option<&PyAny> = None;
         let pytohn_object: Py<PyAny>;
 
         if let Some(unwrapped) = callback {
             pytohn_object = unwrapped;
             let python_function = pytohn_object.as_ref(_py);
@@ -90,19 +89,21 @@
 
 
         //Start the inference loop
         let mut tokens_processed = 0;
         let mut token_utf8_buf = TokenUtf8Buffer::new();
 
         let mut total_generated_text = String::new();
+        let mut stop_reason = results::StopReason::EndToken;
 
         let generation_start_at = std::time::SystemTime::now();
         loop {
             //Check if we have reached the maximum token count
-            if maximum_token_count.is_some() && tokens_processed >= maximum_token_count.unwrap() {
+            if config_to_use.max_new_tokens.is_some() && tokens_processed >= config_to_use.max_new_tokens.unwrap() {
+                stop_reason=results::StopReason::MaxLength;
                 break;
             }
 
             //Infere the next token and break if the END_OF_TEXT token is reached
             let token = match session.infer_next_token(&self.model, &generation_params, &mut rng) {
                 Ok(token) => token,
                 Err(InferenceError::EndOfText) => break,
@@ -117,39 +118,30 @@
                 if let Some(function) = callback_function {
                     let args = PyTuple::new(_py, &[tokens]);
                     let result = function.call1(args)?;
                     //Check if the callback function returned true
                     if !result.is_none() {
                         if result.is_true()? {
                             //If the callback function returned true, stop the generation
+                            stop_reason=results::StopReason::UserCancelled;
                             break;
                         }
                     }
                 }
-                
             }
 
             tokens_processed += 1;
         }
         let generation_duration = generation_start_at.elapsed().unwrap();
 
         let result = results::GenerationResult{
             text:total_generated_text,
             times: results::GenerationTimes{
                 total:generation_duration.as_millis()+feed_prompt_duration.as_millis(),
                 generation:generation_duration.as_millis(),
-                prompt_feeding:feed_prompt_duration.as_millis()}
+                prompt_feeding:feed_prompt_duration.as_millis()},
+            stop_reason:stop_reason
             };
 
-        Ok((result))
+        Ok(result)
     }
-}
-
-/// A Python module implemented in Rust.
-#[pymodule]
-fn llama_rs_python(_py: Python, m: &PyModule) -> PyResult<()> {
-    m.add_class::<Model>()?;
-    m.add_class::<configs::GenerationConfig>()?;
-    m.add_class::<results::GenerationTimes>()?;
-    m.add_class::<results::GenerationResult>()?;
-    Ok(())
-}
+}
```

### Comparing `llama_rs_python-0.0.1/src/logging_utils.rs` & `llama_rs_python-0.0.2/src/logging_utils.rs`

 * *Files identical despite different names*

### Comparing `llama_rs_python-0.0.1/test.py` & `llama_rs_python-0.0.2/example.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from llama_rs_python import Model,GenerationConfig
+from llama_rs_python import Model,SessionConfig,Precision,GenerationConfig
 from typing import Optional
 import sys 
 
 prompt="The meaning of life is"
 
 print("Loading Model...")
-model = Model("../llama-rs/ggml-alpaca-7b-q4.bin",context_length=512,threads=8,batch_size=8,verbose=True)
+session_config = SessionConfig(threads=8,context_length=512)
+model = Model("../llama-rs/ggml-alpaca-7b-q4.bin",session_config=session_config,verbose=True)
 
 print("Loaded model!")
 
 print("Begining Generation:")
 print(prompt,end="")
 
 def callback(token:str)->Optional[bool]:
     print(token,end="")
     sys.stdout.flush()
     
-config=GenerationConfig()
+config=GenerationConfig(top_p=0.9,seed=1441,max_new_tokens=1024)
 result = model.generate(prompt,generation_config=config,callback=callback)
 print(result)
```

### Comparing `llama_rs_python-0.0.1/Cargo.lock` & `llama_rs_python-0.0.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
  "serde",
  "serde_bytes",
  "thiserror",
 ]
 
 [[package]]
 name = "llama-rs-python"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
  "llama-rs",
  "log",
  "pyo3",
  "rand",
  "rand_chacha",
 ]
```

### Comparing `llama_rs_python-0.0.1/PKG-INFO` & `llama_rs_python-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: llama-rs-python
-Version: 0.0.1
+Version: 0.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
+Summary: Unofficial python bindings for llama-rs. 🐍❤️🦀
+Author: Lukas Kreussel
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Bug Tracker, https://github.com/LLukas22/llama-rs-python/issues
+Project-URL: Homepage, https://github.com/LLukas22/llama-rs-python
 
 # llama-rs-python
 Unofficial python bindings for [llama-rs](https://github.com/rustformers/llama-rs) created with [PyO3](https://github.com/PyO3/pyo3). 🐍❤️🦀
 
 This package gives access to the basic functionality of the llama-rs project.
 
 GGML converted models can be loaded and executed.
@@ -28,23 +34,24 @@
 ```python 
 from llama_rs_python import Model
 
 #load the model
 model = Model("path/to/model.bin")
 
 #generate
-print(model.generate("The meaning of life is").text)
+print(model.generate("The meaning of life is"))
 ```
 
 The package also supports callbacks to get each token as it is generated.
 The callback-function also supports canceling the generation by returning a `True` value from the pytohn side.
 
 ```python 
-import sys
 from llama_rs_python import Model
+import sys
+from typing import Optional
 
 #load the model
 model = Model("path/to/model.bin")
 
 #define the callback
 def callback(token:str)->Optional[bool]:
     print(token,end="")
@@ -60,14 +67,24 @@
 ```python 
 from llama_rs_python import Model, GenerationConfig
 
 #load the model
 model = Model("path/to/model.bin")
 
 #create a config
-config = GenerationConfig(top_p=0.9)
+config = GenerationConfig(top_p=0.9,seed=1441,max_new_tokens=1024)
 
 #generate
-print(model.generate("The meaning of life is",generation_config=config).text)
+print(model.generate("The meaning of life is",generation_config=config))
 ```
 
+To configure model specific settings the `SessionConfig` class can be used.
+
+```python
+from llama_rs_python import Model, SessionConfig
 
+#define the session
+session_config = SessionConfig(threads=8,context_length=512)
+
+#load the model
+model = Model("path/to/model.bin",session_config=session_config)
+```
```

