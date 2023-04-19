# Comparing `tmp/ioddcombase-1.6.4-cp39-cp39-win_amd64.whl.zip` & `tmp/ioddcombase-1.6.6-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,15 @@
-Zip file size: 1485239 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      732 b- defN 23-Mar-18 02:24 siogeen/LICENSE.txt
--rw-rw-rw-  2.0 fat   604672 b- defN 23-Mar-18 02:24 siogeen/base/IoddUtility.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat  3043840 b- defN 23-Mar-18 02:26 siogeen/base/_IoddDrv.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      394 b- defN 23-Mar-18 02:24 siogeen/base/__init__.py
--rw-rw-rw-  2.0 fat      732 b- defN 23-Mar-18 02:26 IoddComBase-1.6.4.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     5128 b- defN 23-Mar-18 02:26 IoddComBase-1.6.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Mar-18 02:26 IoddComBase-1.6.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-18 02:26 IoddComBase-1.6.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      766 b- defN 23-Mar-18 02:26 IoddComBase-1.6.4.dist-info/RECORD
-9 files, 3656372 bytes uncompressed, 1483915 bytes compressed:  59.4%
+Zip file size: 2457295 bytes, number of entries: 13
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 19:52 ioddcombase.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 19:52 IoddComBase-1.6.6.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 19:52 siogeen/
+-rw-rw-r--  2.0 unx      796 b- defN 23-Apr-18 19:52 IoddComBase-1.6.6.dist-info/RECORD
+-rw-rw-r--  2.0 unx      732 b- defN 23-Apr-18 19:52 IoddComBase-1.6.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      209 b- defN 23-Apr-18 19:52 IoddComBase-1.6.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx     4998 b- defN 23-Apr-18 19:52 IoddComBase-1.6.6.dist-info/METADATA
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-18 19:52 IoddComBase-1.6.6.dist-info/top_level.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 19:52 siogeen/base/
+-rw-rw-r--  2.0 unx      732 b- defN 23-Apr-18 19:52 siogeen/LICENSE.txt
+-rwxr-xr-x  2.0 unx  6141340 b- defN 23-Apr-18 19:52 siogeen/base/_IoddDrv.cpython-39-i386-linux-gnu.so
+-rw-r--r--  2.0 unx      416 b- defN 23-Apr-18 19:52 siogeen/base/__init__.py
+-rwxr-xr-x  2.0 unx  1019332 b- defN 23-Apr-18 19:52 siogeen/base/IoddUtility.cpython-39-i386-linux-gnu.so
+13 files, 7168563 bytes uncompressed, 2455495 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -1,28 +1,40 @@
-Filename: siogeen/LICENSE.txt
+Filename: ioddcombase.libs/
 Comment: 
 
-Filename: siogeen/base/IoddUtility.cp39-win_amd64.pyd
+Filename: IoddComBase-1.6.6.dist-info/
 Comment: 
 
-Filename: siogeen/base/_IoddDrv.cp39-win_amd64.pyd
+Filename: siogeen/
 Comment: 
 
-Filename: siogeen/base/__init__.py
+Filename: IoddComBase-1.6.6.dist-info/RECORD
+Comment: 
+
+Filename: IoddComBase-1.6.6.dist-info/LICENSE.txt
+Comment: 
+
+Filename: IoddComBase-1.6.6.dist-info/WHEEL
 Comment: 
 
-Filename: IoddComBase-1.6.4.dist-info/LICENSE.txt
+Filename: IoddComBase-1.6.6.dist-info/METADATA
 Comment: 
 
-Filename: IoddComBase-1.6.4.dist-info/METADATA
+Filename: IoddComBase-1.6.6.dist-info/top_level.txt
 Comment: 
 
-Filename: IoddComBase-1.6.4.dist-info/WHEEL
+Filename: siogeen/base/
 Comment: 
 
-Filename: IoddComBase-1.6.4.dist-info/top_level.txt
+Filename: siogeen/LICENSE.txt
+Comment: 
+
+Filename: siogeen/base/_IoddDrv.cpython-39-i386-linux-gnu.so
+Comment: 
+
+Filename: siogeen/base/__init__.py
 Comment: 
 
-Filename: IoddComBase-1.6.4.dist-info/RECORD
+Filename: siogeen/base/IoddUtility.cpython-39-i386-linux-gnu.so
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## siogeen/base/__init__.py

```diff
@@ -8,7 +8,8 @@
 Created on 04.03.2017
 '''
 
 __author__ = "Reimund Renner"
 __email__ = "reimund@siogeen.com"
 __contact__ = "contact@siogeen.com"
 __license__ = "proprietary and confidential"
+__version__ = "1.6.6"
```

## Comparing `IoddComBase-1.6.4.dist-info/LICENSE.txt` & `IoddComBase-1.6.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `IoddComBase-1.6.4.dist-info/METADATA` & `IoddComBase-1.6.6.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,121 +1,118 @@
-Metadata-Version: 2.1
-Name: IoddComBase
-Version: 1.6.4
-Summary: IoddCom base
-Home-page: https://siogeen.com
-Author: Reimund Renner
-Author-email: reimund@siogeen.com
-License: proprietary and confidential
-Project-URL: Documentation, https://siogeen.com/doc/
-Project-URL: Help Desk, https://siogeen.com/helpdesk/
-Project-URL: Knowledge Base, https://siogeen.com/helpdesk/knowledgebase
-Project-URL: News, https://news.siogeen.com/
-Keywords: IO-Link,IODD,development,test,production
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Manufacturing
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Customer Service
-Classifier: Topic :: Software Development :: Embedded Systems
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-Requires-Dist: bitstring
-Requires-Dist: urllib3
-Requires-Dist: pyserial
-Requires-Dist: prettytable
-Requires-Dist: getmac
-
-IoddComBase - base IoddCom package
-==================================
-
-This is the base package for Siogeen IoddCom.
-
-.. _IoddComChecker: /project/IoddComChecker
-.. _IoddComCheckerGui: /project/IoddComCheckerGui
-
-For checking your IO-Link masters working with Siogeen IoddCom, please see IoddComChecker_ or IoddComCheckerGui_
-
-For full package, requests and support go to https://siogeen.com
-
-**Copyright 2017-2023 Siogeen UG** (limited liability)
-
-.. _request: https://siogeen.com/#contact
-
-Supported Platforms
-~~~~~~~~~~~~~~~~~~~
-
-============= ===================== ===================
-**OS**         Python 2.7, 3.4-3.5   Python 3.6 - 3.11
-============= ===================== ===================
-**Windows**     [1]_                   x
-**Linux**       [1]_                   x
-**Raspberry**   [1]_                  3.7, 3.9
-**macOS**       [1]_                  3.8-3.11 [2]_
-============= ===================== ===================
-
-.. [1] IoddCom for Python 2.7, 3.4 - 3.5 on request_.
-.. [2] IoddCom for macOS: Intel chip only, yet
-
-Support for other platforms on request_.
-
-Supported operating systems and IO-Link masters
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Table of supported IO-Link masters for specific operating systems (OS):
-
-+---------------------------------+---------------------------------------------------+
-| Master                          | supported OS                                      |
-|                                 +---------+----------+--------------+---------------+
-|                                 | Windows |  Linux   | Raspberry Pi | macOS 64 [3]_ |
-+=================================+=========+==========+==============+===============+
-| TMG-USB based masters [4]_ [5]_ |   x     |    x     |    x         |    x          |
-+---------------------------------+---------+----------+--------------+---------------+
-| TMG ethernet based masters [6]_ |   x     |    x     |    x         |    x          |
-+---------------------------------+---------+----------+--------------+---------------+
-| ifm ethernet based masters [7]_ |   x     |    x     |    x         |    x          |
-+---------------------------------+---------+----------+--------------+---------------+
-| ifm USB based masters [8]_      |   x     |    x     |    x         |    x          |
-+---------------------------------+---------+----------+--------------+---------------+
-
-For Windows, Linux and Raspberry Pi both, 32-bit and 64-bit versions are available.
-
-.. [3] For macOS 10.15+ Python 3.8-3.11 with Intel chip (others on request)
-
-.. [4] Driver not included. Need driver from manufacturer or install DTM driver
-       for the device.
-
-.. [5] For example: Baumer, Leuze, Pepperl+Fuchs, SICK AG, Turck
-
-.. [6] For Example: Balluff, Belden, Murrelektronik, Pepperl+Fuchs, Wenglor
-
-.. [7] All ifm IO-Link masters AL1xxx should be supported. Functionality depends on
-       master type.
-       The following functions are missing yet: PD streaming, master data storage read/write,
-       master commands, PD valid status
-
-.. [8] Experimental ifm USB IO-Link master AL1060 support. Special functions missing
-       like for [7]_
-
-Not supported masters:
-
-* RevolutionPi RevPi masters
-* Pepperl & Fuchs comtrol masters
-* Baumer USB-C and senscontrol masters
-* Germbedded masters
-* TEConcept masters
-* iO-Fly masters
-* iq masters
-
-Support for them or other masters on request_.
+Metadata-Version: 2.1
+Name: IoddComBase
+Version: 1.6.6
+Summary: IoddCom base
+Home-page: https://siogeen.com
+Author: Reimund Renner
+Author-email: reimund@siogeen.com
+License: proprietary and confidential
+Project-URL: Documentation, https://siogeen.com/doc/
+Project-URL: Help Desk, https://siogeen.com/helpdesk/
+Project-URL: Knowledge Base, https://siogeen.com/helpdesk/knowledgebase
+Project-URL: News, https://news.siogeen.com/
+Keywords: IO-Link,IODD,development,test,production
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Manufacturing
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Customer Service
+Classifier: Topic :: Software Development :: Embedded Systems
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: bitstring
+Requires-Dist: urllib3
+Requires-Dist: pyserial
+Requires-Dist: prettytable
+Requires-Dist: getmac
+
+IoddComBase - base IoddCom package
+==================================
+
+This is the base package for Siogeen IoddCom.
+
+.. _IoddComChecker: /project/IoddComChecker
+.. _IoddComCheckerGui: /project/IoddComCheckerGui
+
+For checking your IO-Link masters working with Siogeen IoddCom, please see IoddComChecker_ or IoddComCheckerGui_
+
+For full package, requests and support go to https://siogeen.com
+
+**Copyright 2017-2023 Siogeen UG** (limited liability)
+
+.. _request: https://siogeen.com/#contact
+
+Supported Platforms
+~~~~~~~~~~~~~~~~~~~
+
+========================= ===================== ===================
+**OS**                    Python 2.7, 3.4-3.5   Python 3.6 - 3.11
+========================= ===================== ===================
+**Windows**                 [1]_                   x
+**Linux x86/x64**           [1]_                   x
+**Linux Arm (Raspberry)**   [1]_                  3.7-3.10
+**macOS**                   [1]_                  3.8-3.11 [2]_
+========================= ===================== ===================
+
+.. [1] IoddCom for Python 2.7, 3.4 - 3.5 on request_.
+.. [2] IoddCom for macOS: Intel chip only, yet
+
+Support for other platforms on request_.
+
+Supported operating systems and IO-Link masters
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Table of supported IO-Link masters for specific operating systems (OS):
+
++---------------------------------+---------------------------------------------------+
+| Master                          | supported OS                                      |
+|                                 +---------+----------+--------------+---------------+
+|                                 | Windows |  Linux   | Raspberry Pi | macOS 64 [3]_ |
++=================================+=========+==========+==============+===============+
+| TMG-USB based masters [4]_      |   x     |    x     |    x         |    x          |
++---------------------------------+---------+----------+--------------+---------------+
+| TMG ethernet based masters [5]_ |   x     |    x     |    x         |    x          |
++---------------------------------+---------+----------+--------------+---------------+
+| ifm ethernet based masters [6]_ |   x     |    x     |    x         |    x          |
++---------------------------------+---------+----------+--------------+---------------+
+| ifm USB based masters [7]_      |   x     |    x     |    x         |    x          |
++---------------------------------+---------+----------+--------------+---------------+
+
+For Windows, Linux and Raspberry Pi both, 32-bit and 64-bit versions are available.
+
+.. [3] For macOS 10.15+ Python 3.8-3.11 with Intel chip (others on request)
+
+.. [4] For example: Baumer, Leuze, Pepperl+Fuchs, SICK AG, Turck
+
+.. [5] For Example: Balluff, Belden, Murrelektronik, Pepperl+Fuchs, Wenglor
+
+.. [6] All ifm IO-Link masters AL1xxx should be supported. Functionality depends on
+       master type.
+       The following functions are missing yet: PD streaming, master data storage read/write,
+       master commands, PD valid status
+
+.. [7] Experimental ifm USB IO-Link master AL1060 support. Special functions missing
+       like for [6]_
+
+Not supported masters:
+
+* RevolutionPi RevPi masters
+* Pepperl & Fuchs comtrol masters
+* Baumer USB-C and senscontrol masters
+* Germbedded masters
+* TEConcept masters
+* iO-Fly masters
+* iq masters
+
+Support for them or other masters on request_.
```

