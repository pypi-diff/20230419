# Comparing `tmp/gmail_scanner-1.0.0.tar.gz` & `tmp/gmail_scanner-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmail_scanner-1.0.0.tar", last modified: Wed Apr 19 10:53:29 2023, max compression
+gzip compressed data, was "gmail_scanner-1.0.1.tar", last modified: Wed Apr 19 11:19:49 2023, max compression
```

## Comparing `gmail_scanner-1.0.0.tar` & `gmail_scanner-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-19 10:53:29.543896 gmail_scanner-1.0.0/
--rw-r--r--   0 ziji       (501) staff       (20)     1070 2023-04-18 15:24:45.000000 gmail_scanner-1.0.0/LICENSE
--rw-r--r--   0 ziji       (501) staff       (20)     2824 2023-04-19 10:53:29.543723 gmail_scanner-1.0.0/PKG-INFO
--rw-r--r--   0 ziji       (501) staff       (20)     1748 2023-04-19 10:46:13.000000 gmail_scanner-1.0.0/README.md
-drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-19 10:53:29.542444 gmail_scanner-1.0.0/gmail_scanner/
--rw-r--r--   0 ziji       (501) staff       (20)      136 2023-04-19 10:03:30.000000 gmail_scanner-1.0.0/gmail_scanner/__init__.py
--rw-r--r--   0 ziji       (501) staff       (20)     6683 2023-04-19 10:38:29.000000 gmail_scanner-1.0.0/gmail_scanner/gmail_scanner.py
-drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-19 10:53:29.543495 gmail_scanner-1.0.0/gmail_scanner.egg-info/
--rw-r--r--   0 ziji       (501) staff       (20)     2824 2023-04-19 10:53:29.000000 gmail_scanner-1.0.0/gmail_scanner.egg-info/PKG-INFO
--rw-r--r--   0 ziji       (501) staff       (20)      303 2023-04-19 10:53:29.000000 gmail_scanner-1.0.0/gmail_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-19 10:53:29.000000 gmail_scanner-1.0.0/gmail_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-19 10:49:52.000000 gmail_scanner-1.0.0/gmail_scanner.egg-info/not-zip-safe
--rw-r--r--   0 ziji       (501) staff       (20)       51 2023-04-19 10:53:29.000000 gmail_scanner-1.0.0/gmail_scanner.egg-info/requires.txt
--rw-r--r--   0 ziji       (501) staff       (20)       14 2023-04-19 10:53:29.000000 gmail_scanner-1.0.0/gmail_scanner.egg-info/top_level.txt
--rw-r--r--   0 ziji       (501) staff       (20)       38 2023-04-19 10:53:29.543945 gmail_scanner-1.0.0/setup.cfg
--rw-r--r--   0 ziji       (501) staff       (20)     1597 2023-04-19 10:49:19.000000 gmail_scanner-1.0.0/setup.py
+drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-19 11:19:49.329932 gmail_scanner-1.0.1/
+-rw-r--r--   0 ziji       (501) staff       (20)     1070 2023-04-18 15:24:45.000000 gmail_scanner-1.0.1/LICENSE
+-rw-r--r--   0 ziji       (501) staff       (20)     3050 2023-04-19 11:19:49.329736 gmail_scanner-1.0.1/PKG-INFO
+-rw-r--r--   0 ziji       (501) staff       (20)     1974 2023-04-19 11:11:46.000000 gmail_scanner-1.0.1/README.md
+drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-19 11:19:49.328446 gmail_scanner-1.0.1/gmail_scanner/
+-rw-r--r--   0 ziji       (501) staff       (20)      136 2023-04-19 10:03:30.000000 gmail_scanner-1.0.1/gmail_scanner/__init__.py
+-rw-r--r--   0 ziji       (501) staff       (20)     6676 2023-04-19 11:06:41.000000 gmail_scanner-1.0.1/gmail_scanner/gmail_scanner.py
+drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-19 11:19:49.329500 gmail_scanner-1.0.1/gmail_scanner.egg-info/
+-rw-r--r--   0 ziji       (501) staff       (20)     3050 2023-04-19 11:19:49.000000 gmail_scanner-1.0.1/gmail_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 ziji       (501) staff       (20)      303 2023-04-19 11:19:49.000000 gmail_scanner-1.0.1/gmail_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-19 11:19:49.000000 gmail_scanner-1.0.1/gmail_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-19 10:49:52.000000 gmail_scanner-1.0.1/gmail_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 ziji       (501) staff       (20)       51 2023-04-19 11:19:49.000000 gmail_scanner-1.0.1/gmail_scanner.egg-info/requires.txt
+-rw-r--r--   0 ziji       (501) staff       (20)       14 2023-04-19 11:19:49.000000 gmail_scanner-1.0.1/gmail_scanner.egg-info/top_level.txt
+-rw-r--r--   0 ziji       (501) staff       (20)       38 2023-04-19 11:19:49.329982 gmail_scanner-1.0.1/setup.cfg
+-rw-r--r--   0 ziji       (501) staff       (20)     1597 2023-04-19 11:16:51.000000 gmail_scanner-1.0.1/setup.py
```

### Comparing `gmail_scanner-1.0.0/LICENSE` & `gmail_scanner-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gmail_scanner-1.0.0/PKG-INFO` & `gmail_scanner-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmail_scanner
-Version: 1.0.0
+Version: 1.0.1
 Summary: gmail scanner
 Home-page: https://github.com/Annihilater/gmail_scanner
 Author: coo
 Author-email: me@coo.lol
 Maintainer: coo
 Maintainer-email: me@coo.lol
 License: MIT
@@ -34,24 +34,30 @@
 # @Author: doi
 # @email : me@coo.lol
 # @File  : README.md
 -->
 
 # Gmail Scanner
 
-Gmail Scanner
+Gmail Scanner is a Gmail mailbox scanner.
 
 ## Description
 
+Gmail Scanner has a multi-process mode that is very fast, and how fast it is depends on the performance of your machine.
+
 The program will return only one results:
 
 - `Unregistered`: It means that the Gmail is not registered or is **blocked**.
 
 ## Update
 
+### 1.0.1
+
+- Fixed some bug
+
 ### 1.0.0
 
 - Record results to a csv file.
 
 ## Usage
 
 **You need to install `gmail_scanner` before.**
@@ -61,38 +67,38 @@
 ```
 
 ### Lite Mode
 
 1. Create a new `.py` file with the following codes.
 
 ```python
-from gmail_scanner import check_one_gmail
+from gmail_scanner.gmail_scanner import check_one_gmail
 
 # Only Print Unregistered Result
 # admin is email prefix
-check_one_gmail(f"admin")
+check_one_gmail(f"admin001")
 ```
 
 2. If you want to scan a lots of Gmail, you can use the following codes.
 
 ```python
-from gmail_scanner import scan_int, scan_int_multi
+from gmail_scanner.gmail_scanner import scan_int_single, scan_int_multi
 
 # single process mode(slow) to scan 6-digit gmail mailboxes
 start_num = 0
 end_num = 999999
 email_length = 6
-output_file = 'results.csv'
-scan_int(start_num, end_num, email_length, output_file)
+output_file = f'results.csv'
+scan_int_single(start_num, end_num, email_length, output_file)
 
 # multi process mode(fast) to scan 6-digit gmail mailboxes
 start_num = 0
 end_num = 999999
 email_length = 6
-output_file = 'results.csv'
+output_file = f'results.csv'
 batch_num = 1000
 process_num = 20
 scan_int_multi(start_num, end_num, email_length, output_file, batch_num, process_num)
 
 ```
 
 ## PyPi
```

#### html2text {}

```diff
@@ -1,34 +1,37 @@
-Metadata-Version: 2.1 Name: gmail_scanner Version: 1.0.0 Summary: gmail scanner
+Metadata-Version: 2.1 Name: gmail_scanner Version: 1.0.1 Summary: gmail scanner
 Home-page: https://github.com/Annihilater/gmail_scanner Author: coo Author-
 email: me@coo.lol Maintainer: coo Maintainer-email: me@coo.lol License: MIT
 Platform: all Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier:
 Programming Language :: Python :: 3.4 Classifier: Programming Language ::
 Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Internet :: WWW/
 HTTP :: Dynamic Content Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Description-Content-Type: text/markdown License-File: LICENSE
-# Gmail Scanner Gmail Scanner ## Description The program will return only one
-results: - `Unregistered`: It means that the Gmail is not registered or is
-**blocked**. ## Update ### 1.0.0 - Record results to a csv file. ## Usage **You
-need to install `gmail_scanner` before.** ```bash pip install gmail_scanner ```
-### Lite Mode 1. Create a new `.py` file with the following codes. ```python
-from gmail_scanner import check_one_gmail # Only Print Unregistered Result #
-admin is email prefix check_one_gmail(f"admin") ``` 2. If you want to scan a
-lots of Gmail, you can use the following codes. ```python from gmail_scanner
-import scan_int, scan_int_multi # single process mode(slow) to scan 6-digit
-gmail mailboxes start_num = 0 end_num = 999999 email_length = 6 output_file =
-'results.csv' scan_int(start_num, end_num, email_length, output_file) # multi
-process mode(fast) to scan 6-digit gmail mailboxes start_num = 0 end_num =
-999999 email_length = 6 output_file = 'results.csv' batch_num = 1000
-process_num = 20 scan_int_multi(start_num, end_num, email_length, output_file,
-batch_num, process_num) ``` ## PyPi [https://img.shields.io/badge/Pypi-
-000000?style=for-the-badge&logo=pypi&logoColor=red] ## Docker ```bash git clone
-https://github.com/Annihilater/gmail_scanner cd gmail_scanner cp .env.example
-.env # edit the .env file docker pull klause/gmail_scanner:latest docker-
-compose up -d ``` ## Author **GmailScanner** Â© [coo](https://github.com/
-Annihilater), Released under the [MIT](./LICENSE) License.
+# Gmail Scanner Gmail Scanner is a Gmail mailbox scanner. ## Description Gmail
+Scanner has a multi-process mode that is very fast, and how fast it is depends
+on the performance of your machine. The program will return only one results: -
+`Unregistered`: It means that the Gmail is not registered or is **blocked**. ##
+Update ### 1.0.1 - Fixed some bug ### 1.0.0 - Record results to a csv file. ##
+Usage **You need to install `gmail_scanner` before.** ```bash pip install
+gmail_scanner ``` ### Lite Mode 1. Create a new `.py` file with the following
+codes. ```python from gmail_scanner.gmail_scanner import check_one_gmail # Only
+Print Unregistered Result # admin is email prefix check_one_gmail(f"admin001")
+``` 2. If you want to scan a lots of Gmail, you can use the following codes.
+```python from gmail_scanner.gmail_scanner import scan_int_single,
+scan_int_multi # single process mode(slow) to scan 6-digit gmail mailboxes
+start_num = 0 end_num = 999999 email_length = 6 output_file = f'results.csv'
+scan_int_single(start_num, end_num, email_length, output_file) # multi process
+mode(fast) to scan 6-digit gmail mailboxes start_num = 0 end_num = 999999
+email_length = 6 output_file = f'results.csv' batch_num = 1000 process_num = 20
+scan_int_multi(start_num, end_num, email_length, output_file, batch_num,
+process_num) ``` ## PyPi [https://img.shields.io/badge/Pypi-000000?style=for-
+the-badge&logo=pypi&logoColor=red] ## Docker ```bash git clone https://
+github.com/Annihilater/gmail_scanner cd gmail_scanner cp .env.example .env #
+edit the .env file docker pull klause/gmail_scanner:latest docker-compose up -
+d ``` ## Author **GmailScanner** Â© [coo](https://github.com/Annihilater),
+Released under the [MIT](./LICENSE) License.
```

### Comparing `gmail_scanner-1.0.0/README.md` & `gmail_scanner-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,24 +5,30 @@
 # @Author: doi
 # @email : me@coo.lol
 # @File  : README.md
 -->
 
 # Gmail Scanner
 
-Gmail Scanner
+Gmail Scanner is a Gmail mailbox scanner.
 
 ## Description
 
+Gmail Scanner has a multi-process mode that is very fast, and how fast it is depends on the performance of your machine.
+
 The program will return only one results:
 
 - `Unregistered`: It means that the Gmail is not registered or is **blocked**.
 
 ## Update
 
+### 1.0.1
+
+- Fixed some bug
+
 ### 1.0.0
 
 - Record results to a csv file.
 
 ## Usage
 
 **You need to install `gmail_scanner` before.**
@@ -32,38 +38,38 @@
 ```
 
 ### Lite Mode
 
 1. Create a new `.py` file with the following codes.
 
 ```python
-from gmail_scanner import check_one_gmail
+from gmail_scanner.gmail_scanner import check_one_gmail
 
 # Only Print Unregistered Result
 # admin is email prefix
-check_one_gmail(f"admin")
+check_one_gmail(f"admin001")
 ```
 
 2. If you want to scan a lots of Gmail, you can use the following codes.
 
 ```python
-from gmail_scanner import scan_int, scan_int_multi
+from gmail_scanner.gmail_scanner import scan_int_single, scan_int_multi
 
 # single process mode(slow) to scan 6-digit gmail mailboxes
 start_num = 0
 end_num = 999999
 email_length = 6
-output_file = 'results.csv'
-scan_int(start_num, end_num, email_length, output_file)
+output_file = f'results.csv'
+scan_int_single(start_num, end_num, email_length, output_file)
 
 # multi process mode(fast) to scan 6-digit gmail mailboxes
 start_num = 0
 end_num = 999999
 email_length = 6
-output_file = 'results.csv'
+output_file = f'results.csv'
 batch_num = 1000
 process_num = 20
 scan_int_multi(start_num, end_num, email_length, output_file, batch_num, process_num)
 
 ```
 
 ## PyPi
```

### Comparing `gmail_scanner-1.0.0/gmail_scanner/gmail_scanner.py` & `gmail_scanner-1.0.1/gmail_scanner/gmail_scanner.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         # 1/True: unregistered，2/False: registered
         status = True if data[0][0][1] == 1 else False
     else:
         status, text = response.status_code, response.text
 
     if status:
         spent = round(time.time() - start_time, 4)
-        text = f"{current_time()},{spent},{email_prefix},{status},{text}\n"
+        text = f"{current_time()},{spent},{email_prefix},{status}\n"
         print(text)
         if output_file is not None:
             with open(output_file, mode='a') as f:
                 f.write(text)
 
     result = {
         "domain": email_prefix,
```

### Comparing `gmail_scanner-1.0.0/gmail_scanner.egg-info/PKG-INFO` & `gmail_scanner-1.0.1/gmail_scanner.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmail-scanner
-Version: 1.0.0
+Version: 1.0.1
 Summary: gmail scanner
 Home-page: https://github.com/Annihilater/gmail_scanner
 Author: coo
 Author-email: me@coo.lol
 Maintainer: coo
 Maintainer-email: me@coo.lol
 License: MIT
@@ -34,24 +34,30 @@
 # @Author: doi
 # @email : me@coo.lol
 # @File  : README.md
 -->
 
 # Gmail Scanner
 
-Gmail Scanner
+Gmail Scanner is a Gmail mailbox scanner.
 
 ## Description
 
+Gmail Scanner has a multi-process mode that is very fast, and how fast it is depends on the performance of your machine.
+
 The program will return only one results:
 
 - `Unregistered`: It means that the Gmail is not registered or is **blocked**.
 
 ## Update
 
+### 1.0.1
+
+- Fixed some bug
+
 ### 1.0.0
 
 - Record results to a csv file.
 
 ## Usage
 
 **You need to install `gmail_scanner` before.**
@@ -61,38 +67,38 @@
 ```
 
 ### Lite Mode
 
 1. Create a new `.py` file with the following codes.
 
 ```python
-from gmail_scanner import check_one_gmail
+from gmail_scanner.gmail_scanner import check_one_gmail
 
 # Only Print Unregistered Result
 # admin is email prefix
-check_one_gmail(f"admin")
+check_one_gmail(f"admin001")
 ```
 
 2. If you want to scan a lots of Gmail, you can use the following codes.
 
 ```python
-from gmail_scanner import scan_int, scan_int_multi
+from gmail_scanner.gmail_scanner import scan_int_single, scan_int_multi
 
 # single process mode(slow) to scan 6-digit gmail mailboxes
 start_num = 0
 end_num = 999999
 email_length = 6
-output_file = 'results.csv'
-scan_int(start_num, end_num, email_length, output_file)
+output_file = f'results.csv'
+scan_int_single(start_num, end_num, email_length, output_file)
 
 # multi process mode(fast) to scan 6-digit gmail mailboxes
 start_num = 0
 end_num = 999999
 email_length = 6
-output_file = 'results.csv'
+output_file = f'results.csv'
 batch_num = 1000
 process_num = 20
 scan_int_multi(start_num, end_num, email_length, output_file, batch_num, process_num)
 
 ```
 
 ## PyPi
```

#### html2text {}

```diff
@@ -1,34 +1,37 @@
-Metadata-Version: 2.1 Name: gmail-scanner Version: 1.0.0 Summary: gmail scanner
+Metadata-Version: 2.1 Name: gmail-scanner Version: 1.0.1 Summary: gmail scanner
 Home-page: https://github.com/Annihilater/gmail_scanner Author: coo Author-
 email: me@coo.lol Maintainer: coo Maintainer-email: me@coo.lol License: MIT
 Platform: all Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier:
 Programming Language :: Python :: 3.4 Classifier: Programming Language ::
 Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Internet :: WWW/
 HTTP :: Dynamic Content Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Description-Content-Type: text/markdown License-File: LICENSE
-# Gmail Scanner Gmail Scanner ## Description The program will return only one
-results: - `Unregistered`: It means that the Gmail is not registered or is
-**blocked**. ## Update ### 1.0.0 - Record results to a csv file. ## Usage **You
-need to install `gmail_scanner` before.** ```bash pip install gmail_scanner ```
-### Lite Mode 1. Create a new `.py` file with the following codes. ```python
-from gmail_scanner import check_one_gmail # Only Print Unregistered Result #
-admin is email prefix check_one_gmail(f"admin") ``` 2. If you want to scan a
-lots of Gmail, you can use the following codes. ```python from gmail_scanner
-import scan_int, scan_int_multi # single process mode(slow) to scan 6-digit
-gmail mailboxes start_num = 0 end_num = 999999 email_length = 6 output_file =
-'results.csv' scan_int(start_num, end_num, email_length, output_file) # multi
-process mode(fast) to scan 6-digit gmail mailboxes start_num = 0 end_num =
-999999 email_length = 6 output_file = 'results.csv' batch_num = 1000
-process_num = 20 scan_int_multi(start_num, end_num, email_length, output_file,
-batch_num, process_num) ``` ## PyPi [https://img.shields.io/badge/Pypi-
-000000?style=for-the-badge&logo=pypi&logoColor=red] ## Docker ```bash git clone
-https://github.com/Annihilater/gmail_scanner cd gmail_scanner cp .env.example
-.env # edit the .env file docker pull klause/gmail_scanner:latest docker-
-compose up -d ``` ## Author **GmailScanner** Â© [coo](https://github.com/
-Annihilater), Released under the [MIT](./LICENSE) License.
+# Gmail Scanner Gmail Scanner is a Gmail mailbox scanner. ## Description Gmail
+Scanner has a multi-process mode that is very fast, and how fast it is depends
+on the performance of your machine. The program will return only one results: -
+`Unregistered`: It means that the Gmail is not registered or is **blocked**. ##
+Update ### 1.0.1 - Fixed some bug ### 1.0.0 - Record results to a csv file. ##
+Usage **You need to install `gmail_scanner` before.** ```bash pip install
+gmail_scanner ``` ### Lite Mode 1. Create a new `.py` file with the following
+codes. ```python from gmail_scanner.gmail_scanner import check_one_gmail # Only
+Print Unregistered Result # admin is email prefix check_one_gmail(f"admin001")
+``` 2. If you want to scan a lots of Gmail, you can use the following codes.
+```python from gmail_scanner.gmail_scanner import scan_int_single,
+scan_int_multi # single process mode(slow) to scan 6-digit gmail mailboxes
+start_num = 0 end_num = 999999 email_length = 6 output_file = f'results.csv'
+scan_int_single(start_num, end_num, email_length, output_file) # multi process
+mode(fast) to scan 6-digit gmail mailboxes start_num = 0 end_num = 999999
+email_length = 6 output_file = f'results.csv' batch_num = 1000 process_num = 20
+scan_int_multi(start_num, end_num, email_length, output_file, batch_num,
+process_num) ``` ## PyPi [https://img.shields.io/badge/Pypi-000000?style=for-
+the-badge&logo=pypi&logoColor=red] ## Docker ```bash git clone https://
+github.com/Annihilater/gmail_scanner cd gmail_scanner cp .env.example .env #
+edit the .env file docker pull klause/gmail_scanner:latest docker-compose up -
+d ``` ## Author **GmailScanner** Â© [coo](https://github.com/Annihilater),
+Released under the [MIT](./LICENSE) License.
```

### Comparing `gmail_scanner-1.0.0/setup.py` & `gmail_scanner-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="gmail_scanner",
-    version="1.0.0",
+    version="1.0.1",
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="coo",
     author_email="me@coo.lol",
     maintainer="coo",
     maintainer_email="me@coo.lol",
```

