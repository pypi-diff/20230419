# Comparing `tmp/finometerdl-0.1.1.tar.gz` & `tmp/finometerdl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finometerdl-0.1.1.tar", max compression
+gzip compressed data, was "finometerdl-0.1.2.tar", max compression
```

## Comparing `finometerdl-0.1.1.tar` & `finometerdl-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1018 2023-04-19 11:10:23.346852 finometerdl-0.1.1/README.md
--rw-r--r--   0        0        0       38 2023-04-19 11:42:04.226885 finometerdl-0.1.1/finometerdl/__init__.py
--rw-r--r--   0        0        0      888 2023-04-19 11:25:06.220201 finometerdl-0.1.1/finometerdl/logger.py
--rw-r--r--   0        0        0      427 2023-04-19 11:43:10.870220 finometerdl-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1692 1970-01-01 00:00:00.000000 finometerdl-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1026 2023-04-19 12:13:49.420252 finometerdl-0.1.2/README.md
+-rw-r--r--   0        0        0       38 2023-04-19 11:42:04.226885 finometerdl-0.1.2/finometerdl/__init__.py
+-rw-r--r--   0        0        0     1467 2023-04-19 12:17:05.773589 finometerdl-0.1.2/finometerdl/logger.py
+-rw-r--r--   0        0        0      427 2023-04-19 12:17:12.813589 finometerdl-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 finometerdl-0.1.2/PKG-INFO
```

### Comparing `finometerdl-0.1.1/README.md` & `finometerdl-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 The project consists of two parts: `finometer_logger.ino` and `logger.py`.
 
 ## finometer_logger.ino
 
 `finometer_logger.ino` is a C++ script designed to be loaded on to an Arduino board to interact with the analogue (BNC) outputs of the Finometer.
 The pins should be set up as follows:
 
-Finometer Analogue Output 1 -> Arudion Pin A1 (Finger cuff pressure)
-Finometer Analogue Output 2 -> Arudion Pin A2 (Hydrostatic finger height)
-Finometer Analogue Output 3 -> Arudion Pin A3 (Arm cuff pressure)
-Finometer Analogue Output 4 -> Arudion Pin A4 (Finger plethysmogram)
+- Finometer Analogue Output 1 -> Arduino Pin A1 (Finger cuff pressure)
+- Finometer Analogue Output 2 -> Arduino Pin A2 (Hydrostatic finger height)
+- Finometer Analogue Output 3 -> Arduino Pin A3 (Arm cuff pressure)
+- Finometer Analogue Output 4 -> Arduino Pin A4 (Finger plethysmogram)
 
 These output values are sent via a serial connection along with the elapsed time since the Arduino started.
 
 ## logger.py
 
 The `logger.py` script is a simple python script that logs the values read from a serial port to an output csv file.
 If no name is provided the output file is named `output-` followed by the current date an time.
```

### Comparing `finometerdl-0.1.1/finometerdl/logger.py` & `finometerdl-0.1.2/finometerdl/logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 # Python imports
 import serial
 from datetime import datetime
 
 def logger(source="/dev/ttyACM0", dest=None, encoding='utf-8'):
+    """Logs serial readings
+
+    Args:
+        source (string, optional) : Source port of the serial device.
+            Defaults to "/dev/ttyACM0".
+        dest (string, optional) : Destination file to write serial output to.
+            If None, will use the format 'output-DATETIME.csv' where DATETIME
+            is the current date and time.
+            Defaults to None.
+        encoding (string, optional) : Encoding of serial device. 
+            Defaults to 'utf-8'.
+
+    Returns:
+        return val (bool) : True if successful. False otherwise.
+    """
 
     # Connects to source
     with serial.Serial(source, timeout=10) as ser:
         print(f"Connected to:\n{ser}")
 
         # Creates file
         if dest is None:
@@ -22,10 +37,11 @@
                     print(line)
                     f.write(line)
                 except UnicodeDecodeError:
                     pass
                 except KeyboardInterrupt:
                     break
     print("Finished reading data.")
+    return True
 
 if __name__ == "__main__":
     logger()
```

### Comparing `finometerdl-0.1.1/PKG-INFO` & `finometerdl-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finometerdl
-Version: 0.1.1
+Version: 0.1.2
 Summary: A data logger for the Finometer Medical Device
 Home-page: https://github.com/abdrysdale/finometer-data-logger
 License: GPL-3.0-or-later
 Author: Alex
 Author-email: adrysdale@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -21,18 +21,18 @@
 The project consists of two parts: `finometer_logger.ino` and `logger.py`.
 
 ## finometer_logger.ino
 
 `finometer_logger.ino` is a C++ script designed to be loaded on to an Arduino board to interact with the analogue (BNC) outputs of the Finometer.
 The pins should be set up as follows:
 
-Finometer Analogue Output 1 -> Arudion Pin A1 (Finger cuff pressure)
-Finometer Analogue Output 2 -> Arudion Pin A2 (Hydrostatic finger height)
-Finometer Analogue Output 3 -> Arudion Pin A3 (Arm cuff pressure)
-Finometer Analogue Output 4 -> Arudion Pin A4 (Finger plethysmogram)
+- Finometer Analogue Output 1 -> Arduino Pin A1 (Finger cuff pressure)
+- Finometer Analogue Output 2 -> Arduino Pin A2 (Hydrostatic finger height)
+- Finometer Analogue Output 3 -> Arduino Pin A3 (Arm cuff pressure)
+- Finometer Analogue Output 4 -> Arduino Pin A4 (Finger plethysmogram)
 
 These output values are sent via a serial connection along with the elapsed time since the Arduino started.
 
 ## logger.py
 
 The `logger.py` script is a simple python script that logs the values read from a serial port to an output csv file.
 If no name is provided the output file is named `output-` followed by the current date an time.
```

