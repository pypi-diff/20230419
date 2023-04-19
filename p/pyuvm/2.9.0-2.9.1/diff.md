# Comparing `tmp/pyuvm-2.9.0.tar.gz` & `tmp/pyuvm-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuvm-2.9.0.tar", last modified: Sat Oct 15 14:19:33 2022, max compression
+gzip compressed data, was "pyuvm-2.9.1.tar", last modified: Wed Apr 19 17:06:25 2023, max compression
```

## Comparing `pyuvm-2.9.0.tar` & `pyuvm-2.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 raysalemi   (501) staff       (20)        0 2022-10-15 14:19:33.399010 pyuvm-2.9.0/
--rw-r--r--   0 raysalemi   (501) staff       (20)      567 2022-10-09 18:34:56.000000 pyuvm-2.9.0/LICENSE
--rw-r--r--   0 raysalemi   (501) staff       (20)       16 2020-12-06 19:42:29.000000 pyuvm-2.9.0/MANIFEST.in
--rw-r--r--   0 raysalemi   (501) staff       (20)    20494 2022-10-15 14:19:33.398825 pyuvm-2.9.0/PKG-INFO
--rw-r--r--   0 raysalemi   (501) staff       (20)    19873 2022-10-10 20:13:39.000000 pyuvm-2.9.0/README.md
--rw-r--r--   0 raysalemi   (501) staff       (20)      104 2021-08-13 21:06:37.000000 pyuvm-2.9.0/pyproject.toml
-drwxr-xr-x   0 raysalemi   (501) staff       (20)        0 2022-10-15 14:19:33.395179 pyuvm-2.9.0/pyuvm/
--rw-r--r--   0 raysalemi   (501) staff       (20)      638 2022-02-12 22:21:28.000000 pyuvm-2.9.0/pyuvm/__init__.py
--rw-r--r--   0 raysalemi   (501) staff       (20)      899 2021-09-28 10:54:51.000000 pyuvm-2.9.0/pyuvm/error_classes.py
--rw-r--r--   0 raysalemi   (501) staff       (20)     1085 2022-10-12 21:06:39.000000 pyuvm-2.9.0/pyuvm/extension_classes.py
--rw-r--r--   0 raysalemi   (501) staff       (20)    12510 2022-01-03 13:27:06.000000 pyuvm-2.9.0/pyuvm/s05_base_classes.py
--rw-r--r--   0 raysalemi   (501) staff       (20)     3233 2021-12-14 11:58:32.000000 pyuvm-2.9.0/pyuvm/s06_reporting_classes.py
--rw-r--r--   0 raysalemi   (501) staff       (20)    19313 2021-12-09 21:54:48.000000 pyuvm-2.9.0/pyuvm/s08_factory_classes.py
--rw-r--r--   0 raysalemi   (501) staff       (20)     4549 2022-01-03 13:27:06.000000 pyuvm-2.9.0/pyuvm/s09_phasing.py
--rw-r--r--   0 raysalemi   (501) staff       (20)    26702 2022-10-09 16:34:56.000000 pyuvm-2.9.0/pyuvm/s12_uvm_tlm_interfaces.py
--rw-r--r--   0 raysalemi   (501) staff       (20)     3442 2021-12-22 15:16:43.000000 pyuvm-2.9.0/pyuvm/s13_predefined_component_classes.py
--rw-r--r--   0 raysalemi   (501) staff       (20)    21777 2022-02-09 13:32:30.000000 pyuvm-2.9.0/pyuvm/s13_uvm_component.py
--rw-r--r--   0 raysalemi   (501) staff       (20)    11424 2022-10-09 16:34:56.000000 pyuvm-2.9.0/pyuvm/s14_15_python_sequences.py
--rw-r--r--   0 raysalemi   (501) staff       (20)     3673 2021-10-22 12:50:53.000000 pyuvm-2.9.0/pyuvm/s18_register_model.py
--rw-r--r--   0 raysalemi   (501) staff       (20)     9374 2022-10-15 13:59:54.000000 pyuvm-2.9.0/pyuvm/utility_classes.py
-drwxr-xr-x   0 raysalemi   (501) staff       (20)        0 2022-10-15 14:19:33.398618 pyuvm-2.9.0/pyuvm.egg-info/
--rw-r--r--   0 raysalemi   (501) staff       (20)    20494 2022-10-15 14:19:33.000000 pyuvm-2.9.0/pyuvm.egg-info/PKG-INFO
--rw-r--r--   0 raysalemi   (501) staff       (20)      559 2022-10-15 14:19:33.000000 pyuvm-2.9.0/pyuvm.egg-info/SOURCES.txt
--rw-r--r--   0 raysalemi   (501) staff       (20)        1 2022-10-15 14:19:33.000000 pyuvm-2.9.0/pyuvm.egg-info/dependency_links.txt
--rw-r--r--   0 raysalemi   (501) staff       (20)       14 2022-10-15 14:19:33.000000 pyuvm-2.9.0/pyuvm.egg-info/requires.txt
--rw-r--r--   0 raysalemi   (501) staff       (20)        6 2022-10-15 14:19:33.000000 pyuvm-2.9.0/pyuvm.egg-info/top_level.txt
--rw-r--r--   0 raysalemi   (501) staff       (20)       38 2022-10-15 14:19:33.399056 pyuvm-2.9.0/setup.cfg
--rwxr-xr-x   0 raysalemi   (501) staff       (20)      931 2022-10-15 14:04:16.000000 pyuvm-2.9.0/setup.py
+drwxr-xr-x   0 raysalemi   (501) staff       (20)        0 2023-04-19 17:06:25.882977 pyuvm-2.9.1/
+-rw-r--r--   0 raysalemi   (501) staff       (20)      567 2022-10-09 18:34:56.000000 pyuvm-2.9.1/LICENSE
+-rw-r--r--   0 raysalemi   (501) staff       (20)       16 2020-12-06 19:42:29.000000 pyuvm-2.9.1/MANIFEST.in
+-rw-r--r--   0 raysalemi   (501) staff       (20)    20550 2023-04-19 17:06:25.882763 pyuvm-2.9.1/PKG-INFO
+-rw-r--r--   0 raysalemi   (501) staff       (20)    19929 2023-04-19 16:03:03.000000 pyuvm-2.9.1/README.md
+-rw-r--r--   0 raysalemi   (501) staff       (20)      104 2021-08-13 21:06:37.000000 pyuvm-2.9.1/pyproject.toml
+drwxr-xr-x   0 raysalemi   (501) staff       (20)        0 2023-04-19 17:06:25.876292 pyuvm-2.9.1/pyuvm/
+-rw-r--r--   0 raysalemi   (501) staff       (20)      638 2022-02-12 22:21:28.000000 pyuvm-2.9.1/pyuvm/__init__.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)      899 2021-09-28 10:54:51.000000 pyuvm-2.9.1/pyuvm/error_classes.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     1286 2023-04-19 17:04:52.000000 pyuvm-2.9.1/pyuvm/extension_classes.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)    12500 2023-04-19 16:03:03.000000 pyuvm-2.9.1/pyuvm/s05_base_classes.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     3535 2023-04-19 16:03:03.000000 pyuvm-2.9.1/pyuvm/s06_reporting_classes.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)    19313 2021-12-09 21:54:48.000000 pyuvm-2.9.1/pyuvm/s08_factory_classes.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     4549 2022-01-03 13:27:06.000000 pyuvm-2.9.1/pyuvm/s09_phasing.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)    26702 2022-10-09 16:34:56.000000 pyuvm-2.9.1/pyuvm/s12_uvm_tlm_interfaces.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     3442 2021-12-22 15:16:43.000000 pyuvm-2.9.1/pyuvm/s13_predefined_component_classes.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)    21777 2022-02-09 13:32:30.000000 pyuvm-2.9.1/pyuvm/s13_uvm_component.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)    11424 2022-10-09 16:34:56.000000 pyuvm-2.9.1/pyuvm/s14_15_python_sequences.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     3673 2021-10-22 12:50:53.000000 pyuvm-2.9.1/pyuvm/s18_register_model.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     9374 2022-10-15 13:59:54.000000 pyuvm-2.9.1/pyuvm/utility_classes.py
+drwxr-xr-x   0 raysalemi   (501) staff       (20)        0 2023-04-19 17:06:25.882533 pyuvm-2.9.1/pyuvm.egg-info/
+-rw-r--r--   0 raysalemi   (501) staff       (20)    20550 2023-04-19 17:06:25.000000 pyuvm-2.9.1/pyuvm.egg-info/PKG-INFO
+-rw-r--r--   0 raysalemi   (501) staff       (20)      559 2023-04-19 17:06:25.000000 pyuvm-2.9.1/pyuvm.egg-info/SOURCES.txt
+-rw-r--r--   0 raysalemi   (501) staff       (20)        1 2023-04-19 17:06:25.000000 pyuvm-2.9.1/pyuvm.egg-info/dependency_links.txt
+-rw-r--r--   0 raysalemi   (501) staff       (20)       14 2023-04-19 17:06:25.000000 pyuvm-2.9.1/pyuvm.egg-info/requires.txt
+-rw-r--r--   0 raysalemi   (501) staff       (20)        6 2023-04-19 17:06:25.000000 pyuvm-2.9.1/pyuvm.egg-info/top_level.txt
+-rw-r--r--   0 raysalemi   (501) staff       (20)       38 2023-04-19 17:06:25.883032 pyuvm-2.9.1/setup.cfg
+-rwxr-xr-x   0 raysalemi   (501) staff       (20)      931 2023-04-19 17:04:52.000000 pyuvm-2.9.1/setup.py
```

### Comparing `pyuvm-2.9.0/LICENSE` & `pyuvm-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.0/PKG-INFO` & `pyuvm-2.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: pyuvm
-Version: 2.9.0
+Version: 2.9.1
 Summary: A Python implementation of the UVM using cocotb
 Home-page: https://github.com/pyuvm/pyuvm
 Author: Ray Salemi
 Author-email: ray@raysalemi.com
 Project-URL: Bug Tracker, https://github.com/pyuvm/pyuvm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Framework :: cocotb
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Description
+# PyUVM
+
+## Description
 
 **pyuvm** is the Universal Verification Methodology implemented in Python instead of SystemVerilog. **pyuvm** uses cocotb to interact with the simulator and schedule simulation events.
 
 **pyuvm** implements the most often-used parts of the UVM while taking advantage of the fact that Python does not have strict typing and does not require parameterized classes. The project refactors pieces of the UVM that were either overly complicated due to typing or legacy code.
 
 The code is based in the IEEE 1800.2 specification and most classes and methods have the specification references in the comments.
 
@@ -31,49 +33,48 @@
 |6|Reporting Classes|Leverages logging, controlled using UVM hierarchy|
 |8|Factory Classes|All uvm_void classes automatically registered|
 |9|Phasing|Simplified to only common phases. Supports objection system|
 |12|UVM TLM Interfaces|Fully implemented|
 |13|Predefined Component Classes|Implements uvm_component with hierarchy, uvm_root singleton,run_test(), simplified ConfigDB, uvm_driver, etc|
 |14 & 15|Sequences, sequencer, sequence_item|Refactored sequencer functionality leveraging Python language capabilities. Simpler and more direct implementation|
 
-
-## Installation
+### Installation
 
 You can install **pyuvm** using `pip`. This will also install **cocotb** as a requirement for **pyuvm**.
 
 ```bash
 % pip install pyuvm
 ```
 
 Then you can run a simple test:
 
-```
+```bash
 % python
 >>> from pyuvm import *
 >>> my_object = uvm_object("my_object")
 >>> type(my_object)
 <class 's05_base_classes.uvm_object'>
 >>> print("object name:", my_object.get_name())
 object name: my_object
 ```
 
-## Running from the repository
+### Running from the repository
 
 You can run pyuvm from a cloned repository by installing the cloned repository using pip.
 
 ```bash
 % cd <pyuvm repo directory>
 % pip install -e .
 ```
 
-# Usage
+## Usage
 
 This section demonstrates running an example simulation and then shows how the example has been put together demonstrating what the UVM looks like in Python.
 
-## Running the simulation
+### Running the simulation
 
 The TinyALU is, as its name implies, a tiny ALU. It has four operations: ADD, AND, NOT, and MUL. This example shows us running the Verilog version of the design, but there is also a VHDL version.
 
 **cocotb** uses a Makefile to run its simulation. We see it in `examples/TinyALU`:
 
 ```makefile
 CWD=$(shell pwd)
@@ -107,41 +108,44 @@
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0x71 XOR 0x01 = 0x0070
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xb8 MUL 0x47 = 0x3308
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xff ADD 0xff = 0x01fe
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xff AND 0xff = 0x00ff
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xff XOR 0xff = 0x0000
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xff MUL 0xff = 0xfe01
 ```
-# The `TinyAluBfm` in `tinyalu_utils.py`
+
+## The `TinyAluBfm` in `tinyalu_utils.py`
 
 The `TinyAluBfm` is a singleton that uses **cocotb** to communicate with the TinyALU.  The BFM exposes three coroutines to the user: `send_op()`, `get_cmd()`, and `get_result()`.
 
 The singleton uses the `cocotb.top` variable to get the handle to the DUT.  This is the handle that we normally pass to a `cocotb.test()` coroutine.
 
 The `TinyAluBfm` is defined in `tinyalu_utils.py` and imported into our testbench.
-# The `pyuvm` testbench
+
+## The `pyuvm` testbench
 
 The `testbench.py` contains the entire UVM testbench and connects to the TinyALU through a `TinyAluBfm` object defined in `tinyalu_utils.py`.  We'll examine the `testbench.py` file and enough of the **cocotb** test too run the simlation
 
-## Importing `pyuvm`
+### Importing `pyuvm`
 
 Testbenches written in the SystemVerilog UVM usually import the package like this:
 
 ```systemverilog
 import uvm_pkg::*;
 ```
 
 This gives you access to the class names without needing a package path.  To get
 similar behavior with `pyuvm` us the `from` import syntax. We import `pyuvm` to distinguish the `@pyuvm.test()` decorator from the `@cocotb.test()` decorator:
 
 ```python
 import pyuvm
 from pyuvm import *
 ```
-## The AluTest classes
+
+### The AluTest classes
 
 We're going to examine the UVM classes from the top, the test, to the bottom, the sequences.
 
 **pyuvm** names the UVM classes as they are named in the specification. Therefore **pyvu use underscore naming as is done in SystemVerilog and not camel-casing.
 
 We extend `uvm_test` to create the `AluTest`, using camel-casing in our code even if **pyuvm** does not use it:
 
@@ -175,16 +179,18 @@
         self.test_all = TestAllSeq.create("test_all")
 
     async def run_phase(self):
         self.raise_objection()
         await self.test_all.start()
         self.drop_objection()
 ```
+
 We extend the `AluTest` class to create a parallel version of the test and a Fibonacci program. You can find these sequences in `testbench.py`
-```
+
+```python
 @pyuvm.test()
 class ParallelTest(AluTest):
     def build_phase(self):
         uvm_factory().set_type_override_by_type(TestAllSeq, TestAllForkSeq)
         super().build_phase()
 
 @pyuvm.test()
@@ -192,19 +198,21 @@
     def build_phase(self):
         ConfigDB().set(None, "*", "DISABLE_COVERAGE_ERRORS", True)
         uvm_factory().set_type_override_by_type(TestAllSeq, FibonacciSeq)
         return super().build_phase()
 
 
 ```
+
 All the familiar pieces of a UVM testbench are in **pyuvm**.
 
-## The ALUEnv Class
+### The ALUEnv Class
 
 The `uvm_env` class is a container for the components that make up the testbench.  There are four component classes instantiated:
+
 * `Monitor`—There are actually two monitors instantiated, one to monitor commands (`self.cmd_mod`) and the other to monitor results (`self.result_mon`).  The `Monitor` code is the same for both. We pass them the name of the proxy function that gets the data they monitor.
 * `Scoreboard`—The scoreboard gathers all the commands and results and compares predicted results to actual results.
 * `Coverage`—The coverage class checks that we've covered all the kinds of operations and issues an error if we did not.
 * `Driver`—This `uvm_driver` processes sequences items.
 * `uvm_sequencer`—The `uvm_sequencer` queues sequence items and passes them to the `Driver`
 * We store `self.seqr` in the `ConfigDB()` so test can get it as we see above.
 
@@ -223,20 +231,23 @@
 
     def connect_phase(self):
         self.driver.seq_item_port.connect(self.seqr.seq_item_export)
         self.cmd_mon.ap.connect(self.scoreboard.cmd_export)
         self.cmd_mon.ap.connect(self.coverage.analysis_export)
         self.driver.ap.connect(self.scoreboard.result_export)
 ```
-## The Monitor
+
+### The Monitor
+
 The `Monitor` extends `uvm_component`. Takes the name of a `CocotProxy` method name as an argument.  It uses the name to find the method in the proxy and then calls the method. You cannot do this in SystemVerilog as there is no introspection.
 
 The `Monitor` creates an analysis port and writes the data it gets into the analysis port.
 
 Notice in the `run_phase()` we use the `await` keyword to wait for the `get_cmd` coroutine.  Unlike SystemVerilog, Python makes it clear when you are calling a time-consuming task vs a function. Also notice that the `run_phase()` has the `async` keyword to designate that it is a coroutine. (A task in SystemVerilog.)
+
 ```python
 class Monitor(uvm_component):
     def __init__(self, name, parent, method_name):
         super().__init__(name, parent)
         self.method_name = method_name
 
     def build_phase(self):
@@ -246,22 +257,25 @@
 
     async def run_phase(self):
         while True:
             datum = await self.get_method()
             self.logger.debug(f"MONITORED {datum}")
             self.ap.write(datum)
 ```
-## The Scoreboard
+
+### The Scoreboard
+
 The scoreboard receives commands from the command monitor and results from the results monitor in the same order.  It uses the commands to predict the results and compares them.
 
 * The `build_phase` uses `uvm_tlm_analysis_fifos` to receive data from the monitors and store it.
 * The scoreboard exposes the FIFO exports by copying them into class data members.  As we see in the environment above, this allows us to connect the exports without reaching into the `Scoreboard's` inner workings.
 * We connect the exports in the `connect_phase()`
-* The `check_phase() runs after the `run_phase()`.  At this point the scoreboard has all operations and results. It loops through the operations and predicts the result, then it compares the predicted and actual result.
+* The `check_phase()` runs after the `run_phase()`.  At this point the scoreboard has all operations and results. It loops through the operations and predicts the result, then it compares the predicted and actual result.
 * Notice that we do not use UVM reporting. Instead we us the Python `logging` module. Every `uvm_report_object` and its children has its own logger stored in `self.logger.`
+
 ```python
 class Scoreboard(uvm_component):
 
     def build_phase(self):
         self.cmd_fifo = uvm_tlm_analysis_fifo("cmd_fifo", self)
         self.result_fifo = uvm_tlm_analysis_fifo("result_fifo", self)
         self.cmd_get_port = uvm_get_port("cmd_get_port", self)
@@ -288,15 +302,16 @@
                                      f" 0x{actual_result:04x}")
                 else:
                     self.logger.error(f"FAILED: 0x{A:02x} {op.name} 0x{B:02x} "
                                       f"= 0x{actual_result:04x} "
                                       f"expected 0x{predicted_result:04x}")
 
 ```
-## Coverage
+
+### Coverage
 
 The `Coverage` Class extends `uvm_subscriber` which extends `uvm_analysis_export`.  As we see in the `AluEnv` above, this allows us to pass the object directly to the `connect()` method to connect it to an analysis port.
 
 The `Coverage` Class overrides the `write()` method expected of a `uvm_subscriber`. If it didn't you'd get a runtime error.  The `Coverage` class uses a set to store all the operations seen. Then it subtracts that from the set of all operations. If the result has a length longer than `0` it issues an error.
 
 Since this tesbench loops through all the operations you will not see this error.
 
@@ -322,15 +337,15 @@
                     f"Functional coverage error. Missed: {set(Ops)-self.cvg}")
                 assert False
             else:
                 self.logger.info("Covered all operations")
                 assert True
 ```
 
-## Driver
+### Driver
 
 The `Driver` extends `uvm_driver` and so it works with sequences and sequence items.
 
 The `connect_phase()` gets the proxy from the `ConfigDB()` and the `run_phase()` uses it to get items and process them by calling `send_op`.  We use `while True` because we do this forever. **cocotb** will shut down the `run_phase` coroutine at the end of simulation.
 
 ```python
 class Driver(uvm_driver):
@@ -351,15 +366,17 @@
             await self.bfm.send_op(cmd.A, cmd.B, cmd.op)
             result = await self.bfm.get_result()
             self.ap.write(result)
             cmd.result = result
             self.seq_item_port.item_done()
 
 ```
-## The ALU Sequence
+
+### The ALU Sequence
+
 The ALU Sequence creates sequence items, randomizes them and sends them to the `Driver`. It inherits `start_item` and `finish_item` from `uvm_sequence`.
 
 It is clear that `start_item` and `finish_item` block because we call them using the `await` keyword.  `start_item` waits for it's turn to use the sequencer, and `finish_item` sends the sequence_item to the driver and returns when the driver calls `item_done()`
 
 ```python
 class TestAllSeq(uvm_sequence):
 
@@ -367,35 +384,40 @@
         seqr = ConfigDB().get(None, "", "SEQR")
         random = RandomSeq("random")
         max = MaxSeq("max")
         await random.start(seqr)
         await max.start(seqr)
 
 ```
+
 This virtual sequence launches two other sequences: `RandomSeq` and `MaxSeq`. `RandomSeq` randomizes the operands.
+
 ```python
 class RandomSeq(uvm_sequence):
     async def body(self):
         for op in list(Ops):
             cmd_tr = AluSeqItem("cmd_tr", None, None, op)
             await self.start_item(cmd_tr)
             cmd_tr.randomize_operands()
             await self.finish_item(cmd_tr)
 ```
+
 `MaxSeq` sets the operands to `0xff`:
+
 ```python
 class MaxSeq(uvm_sequence):
     async def body(self):
         for op in list(Ops):
             cmd_tr = AluSeqItem("cmd_tr", 0xff, 0xff, op)
             await self.start_item(cmd_tr)
             await self.finish_item(cmd_tr)
 ```
 
-## ALU Sequence Item
+### ALU Sequence Item
+
 The `AluSeqItem` contains the TinyALU commands.  It has two operands and an operation.
 
 The SystemVerilog `uvm_sequence_item` class uses `convert2string()` to convert the item to a string and `do_compare()` to compare the item to another item.  We do not use these in **pyuvm** because Python has magic methods that do these functions.
 
 `__eq__()`—This does the same thing as `do_compare()` It returns `True` if the items are equal.  This method works with the `==` operator.
 
 `__str__()`—This does the same thing as `convert2string()`.  It returns a string version of the item. The `print` function calls this method automatically.
@@ -424,49 +446,46 @@
     def __str__(self):
         return f"{self.get_name()} : A: 0x{self.A:02x} \
         OP: {self.op.name} ({self.op.value}) B: 0x{self.B:02x}"
 
 ```
 
 Now that we've got the UVM testbench we can call it from a **cocotb** test.
-# The Cocotb Tests
+
+## The Cocotb Tests
 
 **cocotb** finds `uvm_test` classes identified with the `@pyuvm.test()` decorator and launches them as coroutines.  Our test does the following:
 
-# Contributing
+## Contributing
 
 You can contribute to `pyuvm` by forking this repository and submitting pull requests.
 
 The repository runs all needed tests using `tox`.  The test runs
 `flake8` and fails if that linter finds any issues.  Visual Studio Code
 can be set up to automatically check `flake8` issues.  The repository
 ignores F403 and F405 issues from `flake8`.
 
 There are three sets of `pytest` tests that test features that
 don't use coroutines.  The rest of the tests are in `tests/cocotb_tests`
 and need a simulator to run.
 
-
 Credits:
 
 * Ray Salemi—Original author, created as an employee of Siemens.
 * IEEE 1800.2 Specification
 * Siemens for supporting me in this effort.
 
-# License
+## License
 
 Copyright 2020 Siemens EDA
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 [http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
-
-
-
```

### Comparing `pyuvm-2.9.0/README.md` & `pyuvm-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# Description
+# PyUVM
+
+## Description
 
 **pyuvm** is the Universal Verification Methodology implemented in Python instead of SystemVerilog. **pyuvm** uses cocotb to interact with the simulator and schedule simulation events.
 
 **pyuvm** implements the most often-used parts of the UVM while taking advantage of the fact that Python does not have strict typing and does not require parameterized classes. The project refactors pieces of the UVM that were either overly complicated due to typing or legacy code.
 
 The code is based in the IEEE 1800.2 specification and most classes and methods have the specification references in the comments.
 
@@ -14,49 +16,48 @@
 |6|Reporting Classes|Leverages logging, controlled using UVM hierarchy|
 |8|Factory Classes|All uvm_void classes automatically registered|
 |9|Phasing|Simplified to only common phases. Supports objection system|
 |12|UVM TLM Interfaces|Fully implemented|
 |13|Predefined Component Classes|Implements uvm_component with hierarchy, uvm_root singleton,run_test(), simplified ConfigDB, uvm_driver, etc|
 |14 & 15|Sequences, sequencer, sequence_item|Refactored sequencer functionality leveraging Python language capabilities. Simpler and more direct implementation|
 
-
-## Installation
+### Installation
 
 You can install **pyuvm** using `pip`. This will also install **cocotb** as a requirement for **pyuvm**.
 
 ```bash
 % pip install pyuvm
 ```
 
 Then you can run a simple test:
 
-```
+```bash
 % python
 >>> from pyuvm import *
 >>> my_object = uvm_object("my_object")
 >>> type(my_object)
 <class 's05_base_classes.uvm_object'>
 >>> print("object name:", my_object.get_name())
 object name: my_object
 ```
 
-## Running from the repository
+### Running from the repository
 
 You can run pyuvm from a cloned repository by installing the cloned repository using pip.
 
 ```bash
 % cd <pyuvm repo directory>
 % pip install -e .
 ```
 
-# Usage
+## Usage
 
 This section demonstrates running an example simulation and then shows how the example has been put together demonstrating what the UVM looks like in Python.
 
-## Running the simulation
+### Running the simulation
 
 The TinyALU is, as its name implies, a tiny ALU. It has four operations: ADD, AND, NOT, and MUL. This example shows us running the Verilog version of the design, but there is also a VHDL version.
 
 **cocotb** uses a Makefile to run its simulation. We see it in `examples/TinyALU`:
 
 ```makefile
 CWD=$(shell pwd)
@@ -90,41 +91,44 @@
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0x71 XOR 0x01 = 0x0070
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xb8 MUL 0x47 = 0x3308
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xff ADD 0xff = 0x01fe
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xff AND 0xff = 0x00ff
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xff XOR 0xff = 0x0000
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xff MUL 0xff = 0xfe01
 ```
-# The `TinyAluBfm` in `tinyalu_utils.py`
+
+## The `TinyAluBfm` in `tinyalu_utils.py`
 
 The `TinyAluBfm` is a singleton that uses **cocotb** to communicate with the TinyALU.  The BFM exposes three coroutines to the user: `send_op()`, `get_cmd()`, and `get_result()`.
 
 The singleton uses the `cocotb.top` variable to get the handle to the DUT.  This is the handle that we normally pass to a `cocotb.test()` coroutine.
 
 The `TinyAluBfm` is defined in `tinyalu_utils.py` and imported into our testbench.
-# The `pyuvm` testbench
+
+## The `pyuvm` testbench
 
 The `testbench.py` contains the entire UVM testbench and connects to the TinyALU through a `TinyAluBfm` object defined in `tinyalu_utils.py`.  We'll examine the `testbench.py` file and enough of the **cocotb** test too run the simlation
 
-## Importing `pyuvm`
+### Importing `pyuvm`
 
 Testbenches written in the SystemVerilog UVM usually import the package like this:
 
 ```systemverilog
 import uvm_pkg::*;
 ```
 
 This gives you access to the class names without needing a package path.  To get
 similar behavior with `pyuvm` us the `from` import syntax. We import `pyuvm` to distinguish the `@pyuvm.test()` decorator from the `@cocotb.test()` decorator:
 
 ```python
 import pyuvm
 from pyuvm import *
 ```
-## The AluTest classes
+
+### The AluTest classes
 
 We're going to examine the UVM classes from the top, the test, to the bottom, the sequences.
 
 **pyuvm** names the UVM classes as they are named in the specification. Therefore **pyvu use underscore naming as is done in SystemVerilog and not camel-casing.
 
 We extend `uvm_test` to create the `AluTest`, using camel-casing in our code even if **pyuvm** does not use it:
 
@@ -158,16 +162,18 @@
         self.test_all = TestAllSeq.create("test_all")
 
     async def run_phase(self):
         self.raise_objection()
         await self.test_all.start()
         self.drop_objection()
 ```
+
 We extend the `AluTest` class to create a parallel version of the test and a Fibonacci program. You can find these sequences in `testbench.py`
-```
+
+```python
 @pyuvm.test()
 class ParallelTest(AluTest):
     def build_phase(self):
         uvm_factory().set_type_override_by_type(TestAllSeq, TestAllForkSeq)
         super().build_phase()
 
 @pyuvm.test()
@@ -175,19 +181,21 @@
     def build_phase(self):
         ConfigDB().set(None, "*", "DISABLE_COVERAGE_ERRORS", True)
         uvm_factory().set_type_override_by_type(TestAllSeq, FibonacciSeq)
         return super().build_phase()
 
 
 ```
+
 All the familiar pieces of a UVM testbench are in **pyuvm**.
 
-## The ALUEnv Class
+### The ALUEnv Class
 
 The `uvm_env` class is a container for the components that make up the testbench.  There are four component classes instantiated:
+
 * `Monitor`—There are actually two monitors instantiated, one to monitor commands (`self.cmd_mod`) and the other to monitor results (`self.result_mon`).  The `Monitor` code is the same for both. We pass them the name of the proxy function that gets the data they monitor.
 * `Scoreboard`—The scoreboard gathers all the commands and results and compares predicted results to actual results.
 * `Coverage`—The coverage class checks that we've covered all the kinds of operations and issues an error if we did not.
 * `Driver`—This `uvm_driver` processes sequences items.
 * `uvm_sequencer`—The `uvm_sequencer` queues sequence items and passes them to the `Driver`
 * We store `self.seqr` in the `ConfigDB()` so test can get it as we see above.
 
@@ -206,20 +214,23 @@
 
     def connect_phase(self):
         self.driver.seq_item_port.connect(self.seqr.seq_item_export)
         self.cmd_mon.ap.connect(self.scoreboard.cmd_export)
         self.cmd_mon.ap.connect(self.coverage.analysis_export)
         self.driver.ap.connect(self.scoreboard.result_export)
 ```
-## The Monitor
+
+### The Monitor
+
 The `Monitor` extends `uvm_component`. Takes the name of a `CocotProxy` method name as an argument.  It uses the name to find the method in the proxy and then calls the method. You cannot do this in SystemVerilog as there is no introspection.
 
 The `Monitor` creates an analysis port and writes the data it gets into the analysis port.
 
 Notice in the `run_phase()` we use the `await` keyword to wait for the `get_cmd` coroutine.  Unlike SystemVerilog, Python makes it clear when you are calling a time-consuming task vs a function. Also notice that the `run_phase()` has the `async` keyword to designate that it is a coroutine. (A task in SystemVerilog.)
+
 ```python
 class Monitor(uvm_component):
     def __init__(self, name, parent, method_name):
         super().__init__(name, parent)
         self.method_name = method_name
 
     def build_phase(self):
@@ -229,22 +240,25 @@
 
     async def run_phase(self):
         while True:
             datum = await self.get_method()
             self.logger.debug(f"MONITORED {datum}")
             self.ap.write(datum)
 ```
-## The Scoreboard
+
+### The Scoreboard
+
 The scoreboard receives commands from the command monitor and results from the results monitor in the same order.  It uses the commands to predict the results and compares them.
 
 * The `build_phase` uses `uvm_tlm_analysis_fifos` to receive data from the monitors and store it.
 * The scoreboard exposes the FIFO exports by copying them into class data members.  As we see in the environment above, this allows us to connect the exports without reaching into the `Scoreboard's` inner workings.
 * We connect the exports in the `connect_phase()`
-* The `check_phase() runs after the `run_phase()`.  At this point the scoreboard has all operations and results. It loops through the operations and predicts the result, then it compares the predicted and actual result.
+* The `check_phase()` runs after the `run_phase()`.  At this point the scoreboard has all operations and results. It loops through the operations and predicts the result, then it compares the predicted and actual result.
 * Notice that we do not use UVM reporting. Instead we us the Python `logging` module. Every `uvm_report_object` and its children has its own logger stored in `self.logger.`
+
 ```python
 class Scoreboard(uvm_component):
 
     def build_phase(self):
         self.cmd_fifo = uvm_tlm_analysis_fifo("cmd_fifo", self)
         self.result_fifo = uvm_tlm_analysis_fifo("result_fifo", self)
         self.cmd_get_port = uvm_get_port("cmd_get_port", self)
@@ -271,15 +285,16 @@
                                      f" 0x{actual_result:04x}")
                 else:
                     self.logger.error(f"FAILED: 0x{A:02x} {op.name} 0x{B:02x} "
                                       f"= 0x{actual_result:04x} "
                                       f"expected 0x{predicted_result:04x}")
 
 ```
-## Coverage
+
+### Coverage
 
 The `Coverage` Class extends `uvm_subscriber` which extends `uvm_analysis_export`.  As we see in the `AluEnv` above, this allows us to pass the object directly to the `connect()` method to connect it to an analysis port.
 
 The `Coverage` Class overrides the `write()` method expected of a `uvm_subscriber`. If it didn't you'd get a runtime error.  The `Coverage` class uses a set to store all the operations seen. Then it subtracts that from the set of all operations. If the result has a length longer than `0` it issues an error.
 
 Since this tesbench loops through all the operations you will not see this error.
 
@@ -305,15 +320,15 @@
                     f"Functional coverage error. Missed: {set(Ops)-self.cvg}")
                 assert False
             else:
                 self.logger.info("Covered all operations")
                 assert True
 ```
 
-## Driver
+### Driver
 
 The `Driver` extends `uvm_driver` and so it works with sequences and sequence items.
 
 The `connect_phase()` gets the proxy from the `ConfigDB()` and the `run_phase()` uses it to get items and process them by calling `send_op`.  We use `while True` because we do this forever. **cocotb** will shut down the `run_phase` coroutine at the end of simulation.
 
 ```python
 class Driver(uvm_driver):
@@ -334,15 +349,17 @@
             await self.bfm.send_op(cmd.A, cmd.B, cmd.op)
             result = await self.bfm.get_result()
             self.ap.write(result)
             cmd.result = result
             self.seq_item_port.item_done()
 
 ```
-## The ALU Sequence
+
+### The ALU Sequence
+
 The ALU Sequence creates sequence items, randomizes them and sends them to the `Driver`. It inherits `start_item` and `finish_item` from `uvm_sequence`.
 
 It is clear that `start_item` and `finish_item` block because we call them using the `await` keyword.  `start_item` waits for it's turn to use the sequencer, and `finish_item` sends the sequence_item to the driver and returns when the driver calls `item_done()`
 
 ```python
 class TestAllSeq(uvm_sequence):
 
@@ -350,35 +367,40 @@
         seqr = ConfigDB().get(None, "", "SEQR")
         random = RandomSeq("random")
         max = MaxSeq("max")
         await random.start(seqr)
         await max.start(seqr)
 
 ```
+
 This virtual sequence launches two other sequences: `RandomSeq` and `MaxSeq`. `RandomSeq` randomizes the operands.
+
 ```python
 class RandomSeq(uvm_sequence):
     async def body(self):
         for op in list(Ops):
             cmd_tr = AluSeqItem("cmd_tr", None, None, op)
             await self.start_item(cmd_tr)
             cmd_tr.randomize_operands()
             await self.finish_item(cmd_tr)
 ```
+
 `MaxSeq` sets the operands to `0xff`:
+
 ```python
 class MaxSeq(uvm_sequence):
     async def body(self):
         for op in list(Ops):
             cmd_tr = AluSeqItem("cmd_tr", 0xff, 0xff, op)
             await self.start_item(cmd_tr)
             await self.finish_item(cmd_tr)
 ```
 
-## ALU Sequence Item
+### ALU Sequence Item
+
 The `AluSeqItem` contains the TinyALU commands.  It has two operands and an operation.
 
 The SystemVerilog `uvm_sequence_item` class uses `convert2string()` to convert the item to a string and `do_compare()` to compare the item to another item.  We do not use these in **pyuvm** because Python has magic methods that do these functions.
 
 `__eq__()`—This does the same thing as `do_compare()` It returns `True` if the items are equal.  This method works with the `==` operator.
 
 `__str__()`—This does the same thing as `convert2string()`.  It returns a string version of the item. The `print` function calls this method automatically.
@@ -407,49 +429,46 @@
     def __str__(self):
         return f"{self.get_name()} : A: 0x{self.A:02x} \
         OP: {self.op.name} ({self.op.value}) B: 0x{self.B:02x}"
 
 ```
 
 Now that we've got the UVM testbench we can call it from a **cocotb** test.
-# The Cocotb Tests
+
+## The Cocotb Tests
 
 **cocotb** finds `uvm_test` classes identified with the `@pyuvm.test()` decorator and launches them as coroutines.  Our test does the following:
 
-# Contributing
+## Contributing
 
 You can contribute to `pyuvm` by forking this repository and submitting pull requests.
 
 The repository runs all needed tests using `tox`.  The test runs
 `flake8` and fails if that linter finds any issues.  Visual Studio Code
 can be set up to automatically check `flake8` issues.  The repository
 ignores F403 and F405 issues from `flake8`.
 
 There are three sets of `pytest` tests that test features that
 don't use coroutines.  The rest of the tests are in `tests/cocotb_tests`
 and need a simulator to run.
 
-
 Credits:
 
 * Ray Salemi—Original author, created as an employee of Siemens.
 * IEEE 1800.2 Specification
 * Siemens for supporting me in this effort.
 
-# License
+## License
 
 Copyright 2020 Siemens EDA
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 [http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
-
-
-
```

### Comparing `pyuvm-2.9.0/pyuvm/__init__.py` & `pyuvm-2.9.1/pyuvm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.0/pyuvm/error_classes.py` & `pyuvm-2.9.1/pyuvm/error_classes.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.0/pyuvm/s05_base_classes.py` & `pyuvm-2.9.1/pyuvm/s05_base_classes.py`

 * *Files 11% similar despite different names*

```diff
@@ -73,25 +73,25 @@
 
     # 5.3.4.5
     def get_type(self):
         """
         Not implemented because Python can implement the factory without
         these shenanigans.
         """
-        raise error_classes.UVMNotImplemented(
+        raise error_classes.UsePythonMethod(
             'Python provides better ways to do this '
             'so the uvm_object_wrapper is unimplemented')
 
     # 5.3.4.6
     def get_object_type(self):
         """
         Not implemented because Python can implement the factory without
         these shenanigans.
         """
-        raise error_classes.UVMNotImplemented(
+        raise error_classes.UsePythonMethod(
             'Python provides better ways to do this '
             'so the uvm_object_wrapper is unimplemented')
 
     # 5.3.4.7
     def get_type_name(self):
         """
         Returns types  __name__ magic variable
@@ -119,28 +119,28 @@
         return new
 
     # 5.3.6.1
     def print(self):
         """
         Not implemented. Use __str__() and print()
         """
-        raise error_classes.UVMNotImplemented(
+        raise error_classes.UsePythonMethod(
             'There are better ways to do printing in Python using'
             'print() or str()')
 
     # 5.3.6.2
     def sprint(self):
         """ Not implemented. use __str__() and print()"""
-        raise error_classes.UVMNotImplemented(
+        raise error_classes.UsePythonMethod(
             'There are better ways to do printing in Python')
 
     # 5.3.6.3
     def do_print(self):
         """ not implemented. Use __str__() and print()"""
-        raise error_classes.UVMNotImplemented(
+        raise error_classes.UsePythonMethod(
             'There are better ways to do printing in Python')
 
     # 5.3.6.4
     def convert2string(self):
         """
         Returns the result of self.__str__().
         Perhaps better to just use __str__() directly?
```

### Comparing `pyuvm-2.9.0/pyuvm/s06_reporting_classes.py` & `pyuvm-2.9.1/pyuvm/s06_reporting_classes.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,28 +5,36 @@
 # There may be a need to implement uvm_info, uvm_error,
 # uvm_warning, and uvm_fatal, but it would be best to
 # first see how the native Python logging system does the job.
 
 from pyuvm.s05_base_classes import uvm_object
 import logging
 import sys
-from cocotb.log import SimColourLogFormatter, SimTimeContextFilter
+from cocotb.log import SimTimeContextFilter
+from cocotb.log import SimLogFormatter, SimColourLogFormatter
+from cocotb.utils import want_color_output
 from logging import DEBUG, CRITICAL, ERROR, WARNING, INFO, NOTSET, NullHandler   # noqa: F401, E501
 
 
 class PyuvmFormatter(SimColourLogFormatter):
     def __init__(self, full_name):
         self.full_name = full_name
         super().__init__()
 
     def format(self, record):
-        new_msg = f"{record.filename}({record.lineno})"
-        new_msg += f"[{self.full_name}]: " + record.msg
+        new_msg = f"[{self.full_name}]: " + record.msg
         record.msg = new_msg
-        return super().format(record)
+        name_temp = record.name
+        record.name = f"{record.pathname}({record.lineno})"
+        if want_color_output():
+            formatted_msg = super().format(record)
+        else:
+            formatted_msg = SimLogFormatter.format(self, record)
+        record.name = name_temp
+        return formatted_msg
 
 
 # 6.2.1
 class uvm_report_object(uvm_object):
     __default_logging_level = logging.INFO
     """ The basis of all classes that can report """
     def __init__(self, name):
```

### Comparing `pyuvm-2.9.0/pyuvm/s08_factory_classes.py` & `pyuvm-2.9.1/pyuvm/s08_factory_classes.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.0/pyuvm/s09_phasing.py` & `pyuvm-2.9.1/pyuvm/s09_phasing.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.0/pyuvm/s12_uvm_tlm_interfaces.py` & `pyuvm-2.9.1/pyuvm/s12_uvm_tlm_interfaces.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.0/pyuvm/s13_predefined_component_classes.py` & `pyuvm-2.9.1/pyuvm/s13_predefined_component_classes.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.0/pyuvm/s13_uvm_component.py` & `pyuvm-2.9.1/pyuvm/s13_uvm_component.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.0/pyuvm/s14_15_python_sequences.py` & `pyuvm-2.9.1/pyuvm/s14_15_python_sequences.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.0/pyuvm/s18_register_model.py` & `pyuvm-2.9.1/pyuvm/s18_register_model.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.0/pyuvm/utility_classes.py` & `pyuvm-2.9.1/pyuvm/utility_classes.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.0/pyuvm.egg-info/PKG-INFO` & `pyuvm-2.9.1/pyuvm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: pyuvm
-Version: 2.9.0
+Version: 2.9.1
 Summary: A Python implementation of the UVM using cocotb
 Home-page: https://github.com/pyuvm/pyuvm
 Author: Ray Salemi
 Author-email: ray@raysalemi.com
 Project-URL: Bug Tracker, https://github.com/pyuvm/pyuvm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Framework :: cocotb
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Description
+# PyUVM
+
+## Description
 
 **pyuvm** is the Universal Verification Methodology implemented in Python instead of SystemVerilog. **pyuvm** uses cocotb to interact with the simulator and schedule simulation events.
 
 **pyuvm** implements the most often-used parts of the UVM while taking advantage of the fact that Python does not have strict typing and does not require parameterized classes. The project refactors pieces of the UVM that were either overly complicated due to typing or legacy code.
 
 The code is based in the IEEE 1800.2 specification and most classes and methods have the specification references in the comments.
 
@@ -31,49 +33,48 @@
 |6|Reporting Classes|Leverages logging, controlled using UVM hierarchy|
 |8|Factory Classes|All uvm_void classes automatically registered|
 |9|Phasing|Simplified to only common phases. Supports objection system|
 |12|UVM TLM Interfaces|Fully implemented|
 |13|Predefined Component Classes|Implements uvm_component with hierarchy, uvm_root singleton,run_test(), simplified ConfigDB, uvm_driver, etc|
 |14 & 15|Sequences, sequencer, sequence_item|Refactored sequencer functionality leveraging Python language capabilities. Simpler and more direct implementation|
 
-
-## Installation
+### Installation
 
 You can install **pyuvm** using `pip`. This will also install **cocotb** as a requirement for **pyuvm**.
 
 ```bash
 % pip install pyuvm
 ```
 
 Then you can run a simple test:
 
-```
+```bash
 % python
 >>> from pyuvm import *
 >>> my_object = uvm_object("my_object")
 >>> type(my_object)
 <class 's05_base_classes.uvm_object'>
 >>> print("object name:", my_object.get_name())
 object name: my_object
 ```
 
-## Running from the repository
+### Running from the repository
 
 You can run pyuvm from a cloned repository by installing the cloned repository using pip.
 
 ```bash
 % cd <pyuvm repo directory>
 % pip install -e .
 ```
 
-# Usage
+## Usage
 
 This section demonstrates running an example simulation and then shows how the example has been put together demonstrating what the UVM looks like in Python.
 
-## Running the simulation
+### Running the simulation
 
 The TinyALU is, as its name implies, a tiny ALU. It has four operations: ADD, AND, NOT, and MUL. This example shows us running the Verilog version of the design, but there is also a VHDL version.
 
 **cocotb** uses a Makefile to run its simulation. We see it in `examples/TinyALU`:
 
 ```makefile
 CWD=$(shell pwd)
@@ -107,41 +108,44 @@
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0x71 XOR 0x01 = 0x0070
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xb8 MUL 0x47 = 0x3308
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xff ADD 0xff = 0x01fe
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xff AND 0xff = 0x00ff
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xff XOR 0xff = 0x0000
 250000.00ns INFO     testbench.py(209)[uvm_test_top.env.scoreboard]: PASSED: 0xff MUL 0xff = 0xfe01
 ```
-# The `TinyAluBfm` in `tinyalu_utils.py`
+
+## The `TinyAluBfm` in `tinyalu_utils.py`
 
 The `TinyAluBfm` is a singleton that uses **cocotb** to communicate with the TinyALU.  The BFM exposes three coroutines to the user: `send_op()`, `get_cmd()`, and `get_result()`.
 
 The singleton uses the `cocotb.top` variable to get the handle to the DUT.  This is the handle that we normally pass to a `cocotb.test()` coroutine.
 
 The `TinyAluBfm` is defined in `tinyalu_utils.py` and imported into our testbench.
-# The `pyuvm` testbench
+
+## The `pyuvm` testbench
 
 The `testbench.py` contains the entire UVM testbench and connects to the TinyALU through a `TinyAluBfm` object defined in `tinyalu_utils.py`.  We'll examine the `testbench.py` file and enough of the **cocotb** test too run the simlation
 
-## Importing `pyuvm`
+### Importing `pyuvm`
 
 Testbenches written in the SystemVerilog UVM usually import the package like this:
 
 ```systemverilog
 import uvm_pkg::*;
 ```
 
 This gives you access to the class names without needing a package path.  To get
 similar behavior with `pyuvm` us the `from` import syntax. We import `pyuvm` to distinguish the `@pyuvm.test()` decorator from the `@cocotb.test()` decorator:
 
 ```python
 import pyuvm
 from pyuvm import *
 ```
-## The AluTest classes
+
+### The AluTest classes
 
 We're going to examine the UVM classes from the top, the test, to the bottom, the sequences.
 
 **pyuvm** names the UVM classes as they are named in the specification. Therefore **pyvu use underscore naming as is done in SystemVerilog and not camel-casing.
 
 We extend `uvm_test` to create the `AluTest`, using camel-casing in our code even if **pyuvm** does not use it:
 
@@ -175,16 +179,18 @@
         self.test_all = TestAllSeq.create("test_all")
 
     async def run_phase(self):
         self.raise_objection()
         await self.test_all.start()
         self.drop_objection()
 ```
+
 We extend the `AluTest` class to create a parallel version of the test and a Fibonacci program. You can find these sequences in `testbench.py`
-```
+
+```python
 @pyuvm.test()
 class ParallelTest(AluTest):
     def build_phase(self):
         uvm_factory().set_type_override_by_type(TestAllSeq, TestAllForkSeq)
         super().build_phase()
 
 @pyuvm.test()
@@ -192,19 +198,21 @@
     def build_phase(self):
         ConfigDB().set(None, "*", "DISABLE_COVERAGE_ERRORS", True)
         uvm_factory().set_type_override_by_type(TestAllSeq, FibonacciSeq)
         return super().build_phase()
 
 
 ```
+
 All the familiar pieces of a UVM testbench are in **pyuvm**.
 
-## The ALUEnv Class
+### The ALUEnv Class
 
 The `uvm_env` class is a container for the components that make up the testbench.  There are four component classes instantiated:
+
 * `Monitor`—There are actually two monitors instantiated, one to monitor commands (`self.cmd_mod`) and the other to monitor results (`self.result_mon`).  The `Monitor` code is the same for both. We pass them the name of the proxy function that gets the data they monitor.
 * `Scoreboard`—The scoreboard gathers all the commands and results and compares predicted results to actual results.
 * `Coverage`—The coverage class checks that we've covered all the kinds of operations and issues an error if we did not.
 * `Driver`—This `uvm_driver` processes sequences items.
 * `uvm_sequencer`—The `uvm_sequencer` queues sequence items and passes them to the `Driver`
 * We store `self.seqr` in the `ConfigDB()` so test can get it as we see above.
 
@@ -223,20 +231,23 @@
 
     def connect_phase(self):
         self.driver.seq_item_port.connect(self.seqr.seq_item_export)
         self.cmd_mon.ap.connect(self.scoreboard.cmd_export)
         self.cmd_mon.ap.connect(self.coverage.analysis_export)
         self.driver.ap.connect(self.scoreboard.result_export)
 ```
-## The Monitor
+
+### The Monitor
+
 The `Monitor` extends `uvm_component`. Takes the name of a `CocotProxy` method name as an argument.  It uses the name to find the method in the proxy and then calls the method. You cannot do this in SystemVerilog as there is no introspection.
 
 The `Monitor` creates an analysis port and writes the data it gets into the analysis port.
 
 Notice in the `run_phase()` we use the `await` keyword to wait for the `get_cmd` coroutine.  Unlike SystemVerilog, Python makes it clear when you are calling a time-consuming task vs a function. Also notice that the `run_phase()` has the `async` keyword to designate that it is a coroutine. (A task in SystemVerilog.)
+
 ```python
 class Monitor(uvm_component):
     def __init__(self, name, parent, method_name):
         super().__init__(name, parent)
         self.method_name = method_name
 
     def build_phase(self):
@@ -246,22 +257,25 @@
 
     async def run_phase(self):
         while True:
             datum = await self.get_method()
             self.logger.debug(f"MONITORED {datum}")
             self.ap.write(datum)
 ```
-## The Scoreboard
+
+### The Scoreboard
+
 The scoreboard receives commands from the command monitor and results from the results monitor in the same order.  It uses the commands to predict the results and compares them.
 
 * The `build_phase` uses `uvm_tlm_analysis_fifos` to receive data from the monitors and store it.
 * The scoreboard exposes the FIFO exports by copying them into class data members.  As we see in the environment above, this allows us to connect the exports without reaching into the `Scoreboard's` inner workings.
 * We connect the exports in the `connect_phase()`
-* The `check_phase() runs after the `run_phase()`.  At this point the scoreboard has all operations and results. It loops through the operations and predicts the result, then it compares the predicted and actual result.
+* The `check_phase()` runs after the `run_phase()`.  At this point the scoreboard has all operations and results. It loops through the operations and predicts the result, then it compares the predicted and actual result.
 * Notice that we do not use UVM reporting. Instead we us the Python `logging` module. Every `uvm_report_object` and its children has its own logger stored in `self.logger.`
+
 ```python
 class Scoreboard(uvm_component):
 
     def build_phase(self):
         self.cmd_fifo = uvm_tlm_analysis_fifo("cmd_fifo", self)
         self.result_fifo = uvm_tlm_analysis_fifo("result_fifo", self)
         self.cmd_get_port = uvm_get_port("cmd_get_port", self)
@@ -288,15 +302,16 @@
                                      f" 0x{actual_result:04x}")
                 else:
                     self.logger.error(f"FAILED: 0x{A:02x} {op.name} 0x{B:02x} "
                                       f"= 0x{actual_result:04x} "
                                       f"expected 0x{predicted_result:04x}")
 
 ```
-## Coverage
+
+### Coverage
 
 The `Coverage` Class extends `uvm_subscriber` which extends `uvm_analysis_export`.  As we see in the `AluEnv` above, this allows us to pass the object directly to the `connect()` method to connect it to an analysis port.
 
 The `Coverage` Class overrides the `write()` method expected of a `uvm_subscriber`. If it didn't you'd get a runtime error.  The `Coverage` class uses a set to store all the operations seen. Then it subtracts that from the set of all operations. If the result has a length longer than `0` it issues an error.
 
 Since this tesbench loops through all the operations you will not see this error.
 
@@ -322,15 +337,15 @@
                     f"Functional coverage error. Missed: {set(Ops)-self.cvg}")
                 assert False
             else:
                 self.logger.info("Covered all operations")
                 assert True
 ```
 
-## Driver
+### Driver
 
 The `Driver` extends `uvm_driver` and so it works with sequences and sequence items.
 
 The `connect_phase()` gets the proxy from the `ConfigDB()` and the `run_phase()` uses it to get items and process them by calling `send_op`.  We use `while True` because we do this forever. **cocotb** will shut down the `run_phase` coroutine at the end of simulation.
 
 ```python
 class Driver(uvm_driver):
@@ -351,15 +366,17 @@
             await self.bfm.send_op(cmd.A, cmd.B, cmd.op)
             result = await self.bfm.get_result()
             self.ap.write(result)
             cmd.result = result
             self.seq_item_port.item_done()
 
 ```
-## The ALU Sequence
+
+### The ALU Sequence
+
 The ALU Sequence creates sequence items, randomizes them and sends them to the `Driver`. It inherits `start_item` and `finish_item` from `uvm_sequence`.
 
 It is clear that `start_item` and `finish_item` block because we call them using the `await` keyword.  `start_item` waits for it's turn to use the sequencer, and `finish_item` sends the sequence_item to the driver and returns when the driver calls `item_done()`
 
 ```python
 class TestAllSeq(uvm_sequence):
 
@@ -367,35 +384,40 @@
         seqr = ConfigDB().get(None, "", "SEQR")
         random = RandomSeq("random")
         max = MaxSeq("max")
         await random.start(seqr)
         await max.start(seqr)
 
 ```
+
 This virtual sequence launches two other sequences: `RandomSeq` and `MaxSeq`. `RandomSeq` randomizes the operands.
+
 ```python
 class RandomSeq(uvm_sequence):
     async def body(self):
         for op in list(Ops):
             cmd_tr = AluSeqItem("cmd_tr", None, None, op)
             await self.start_item(cmd_tr)
             cmd_tr.randomize_operands()
             await self.finish_item(cmd_tr)
 ```
+
 `MaxSeq` sets the operands to `0xff`:
+
 ```python
 class MaxSeq(uvm_sequence):
     async def body(self):
         for op in list(Ops):
             cmd_tr = AluSeqItem("cmd_tr", 0xff, 0xff, op)
             await self.start_item(cmd_tr)
             await self.finish_item(cmd_tr)
 ```
 
-## ALU Sequence Item
+### ALU Sequence Item
+
 The `AluSeqItem` contains the TinyALU commands.  It has two operands and an operation.
 
 The SystemVerilog `uvm_sequence_item` class uses `convert2string()` to convert the item to a string and `do_compare()` to compare the item to another item.  We do not use these in **pyuvm** because Python has magic methods that do these functions.
 
 `__eq__()`—This does the same thing as `do_compare()` It returns `True` if the items are equal.  This method works with the `==` operator.
 
 `__str__()`—This does the same thing as `convert2string()`.  It returns a string version of the item. The `print` function calls this method automatically.
@@ -424,49 +446,46 @@
     def __str__(self):
         return f"{self.get_name()} : A: 0x{self.A:02x} \
         OP: {self.op.name} ({self.op.value}) B: 0x{self.B:02x}"
 
 ```
 
 Now that we've got the UVM testbench we can call it from a **cocotb** test.
-# The Cocotb Tests
+
+## The Cocotb Tests
 
 **cocotb** finds `uvm_test` classes identified with the `@pyuvm.test()` decorator and launches them as coroutines.  Our test does the following:
 
-# Contributing
+## Contributing
 
 You can contribute to `pyuvm` by forking this repository and submitting pull requests.
 
 The repository runs all needed tests using `tox`.  The test runs
 `flake8` and fails if that linter finds any issues.  Visual Studio Code
 can be set up to automatically check `flake8` issues.  The repository
 ignores F403 and F405 issues from `flake8`.
 
 There are three sets of `pytest` tests that test features that
 don't use coroutines.  The rest of the tests are in `tests/cocotb_tests`
 and need a simulator to run.
 
-
 Credits:
 
 * Ray Salemi—Original author, created as an employee of Siemens.
 * IEEE 1800.2 Specification
 * Siemens for supporting me in this effort.
 
-# License
+## License
 
 Copyright 2020 Siemens EDA
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 [http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
-
-
-
```

### Comparing `pyuvm-2.9.0/pyuvm.egg-info/SOURCES.txt` & `pyuvm-2.9.1/pyuvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.0/setup.py` & `pyuvm-2.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyuvm",
-    version="2.9.0",
+    version="2.9.1",
     author="Ray Salemi",
     author_email="ray@raysalemi.com",
     description="A Python implementation of the UVM using cocotb",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pyuvm/pyuvm",
     project_urls={
```

