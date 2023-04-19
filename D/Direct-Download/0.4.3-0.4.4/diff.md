# Comparing `tmp/Direct-Download-0.4.3.tar.gz` & `tmp/Direct-Download-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Direct-Download-0.4.3.tar", last modified: Wed Apr 19 07:02:27 2023, max compression
+gzip compressed data, was "Direct-Download-0.4.4.tar", last modified: Wed Apr 19 07:11:28 2023, max compression
```

## Comparing `Direct-Download-0.4.3.tar` & `Direct-Download-0.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 07:02:27.515823 Direct-Download-0.4.3/
--rw-rw-rw-   0        0        0     1061 2022-11-14 16:03:35.000000 Direct-Download-0.4.3/LICENSE
--rw-rw-rw-   0        0        0     4147 2023-04-19 07:02:27.481814 Direct-Download-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     3319 2023-04-18 15:39:51.000000 Direct-Download-0.4.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 07:02:27.516824 Direct-Download-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1107 2023-04-18 16:15:29.000000 Direct-Download-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:02:27.407796 Direct-Download-0.4.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 07:02:27.465809 Direct-Download-0.4.3/src/Direct_Download.egg-info/
--rw-rw-rw-   0        0        0     4147 2023-04-19 07:02:26.000000 Direct-Download-0.4.3/src/Direct_Download.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-19 07:02:26.000000 Direct-Download-0.4.3/src/Direct_Download.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 07:02:26.000000 Direct-Download-0.4.3/src/Direct_Download.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-19 07:02:26.000000 Direct-Download-0.4.3/src/Direct_Download.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-19 07:02:26.000000 Direct-Download-0.4.3/src/Direct_Download.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3888 2023-04-18 15:24:17.000000 Direct-Download-0.4.3/src/Direct_Download.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:11:28.465278 Direct-Download-0.4.4/
+-rw-rw-rw-   0        0        0     1061 2022-11-14 16:03:35.000000 Direct-Download-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0     4159 2023-04-19 07:11:28.457277 Direct-Download-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3331 2023-04-19 07:06:43.000000 Direct-Download-0.4.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 07:11:28.466281 Direct-Download-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1107 2023-04-19 07:08:23.000000 Direct-Download-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:11:28.387258 Direct-Download-0.4.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 07:11:28.452274 Direct-Download-0.4.4/src/Direct_Download.egg-info/
+-rw-rw-rw-   0        0        0     4159 2023-04-19 07:11:27.000000 Direct-Download-0.4.4/src/Direct_Download.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-19 07:11:27.000000 Direct-Download-0.4.4/src/Direct_Download.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 07:11:27.000000 Direct-Download-0.4.4/src/Direct_Download.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-19 07:11:27.000000 Direct-Download-0.4.4/src/Direct_Download.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-19 07:11:27.000000 Direct-Download-0.4.4/src/Direct_Download.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3888 2023-04-18 15:24:17.000000 Direct-Download-0.4.4/src/Direct_Download.py
```

### Comparing `Direct-Download-0.4.3/LICENSE` & `Direct-Download-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Direct-Download-0.4.3/PKG-INFO` & `Direct-Download-0.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Direct-Download
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Direct Downloader Module Which Will Get Direct Download Link From Some Popular File Uploading Websites Like Mediafire, Anonfiles
 Home-page: https://github.com/CYCNO/DirectDownload
 Author: CYCNO
 Keywords: direct download,anonfiles,mediafire,mediafire direct download,anonfiles direct download,google drive,google drive direct download link,google drive download link,megaupload,myfile,letsupload,filechan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 <strong><i>A simple yet powerful tool for getting direct download link.</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/Direct-Download/">
-<img src="https://img.shields.io/badge/PYPI-V0.4.1-blue?logo=PyPI&style=for-the-badge">
+<img src="https://img.shields.io/badge/PYPI-V0.4-blue?logo=PyPI&style=for-the-badge">
 </a>
 <a href="https://github.com/CYCNO/DirectDownload/graphs/contributors">
 <img src="https://img.shields.io/github/contributors/cycno/DirectDownload?style=for-the-badge&color=green&logo=GitHub">
 </a>
 </div>
 
 ---
@@ -110,13 +110,13 @@
 url = Direct()
 
 #Use download By Enabling download to True for downloading your file 
 url.mediafire('https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', download=True)
 ```
 ## Links
 - [PyPI](https://pypi.org/project/Direct-Download/)
-- [API](https://ddl-api.cycno.repl.co/)
+- [API](https://github.com/CYCNO/Direct-Download-API)
 
 ## Contributors
 ### <a href="https://github.com/CYCNO"><img src="https://avatars.githubusercontent.com/u/90704569?v=4" alt="CYCNO" width="50" height="50" style="border-radius: 50%;"></a>
 
 Contributors are always welcome!
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: Direct-Download Version: 0.4.3 Summary: A Direct
+Metadata-Version: 2.1 Name: Direct-Download Version: 0.4.4 Summary: A Direct
 Downloader Module Which Will Get Direct Download Link From Some Popular File
 Uploading Websites Like Mediafire, Anonfiles Home-page: https://github.com/
 CYCNO/DirectDownload Author: CYCNO Keywords: direct
 download,anonfiles,mediafire,mediafire direct download,anonfiles direct
 download,google drive,google drive direct download link,google drive download
 link,megaupload,myfile,letsupload,filechan Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE
                          ****** Direct Download ******
          A simple yet powerful tool for getting direct download link.
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-badge/PYPI-V0.4.1-blue?logo=PyPI&style=for-the-badge] [https://img.shields.io/
+ badge/PYPI-V0.4-blue?logo=PyPI&style=for-the-badge] [https://img.shields.io/
             github/contributors/cycno/DirectDownload?style=for-the-
                         badge&color=green&logo=GitHub]
 --- ## Feautres - All Information Of File Is Available - No Need To Sign Up Or
 Usage Of Tokens - Data Is In JSON Format - Download the file - Switch Between
 Just Download Link Or ALL Information - Very Easy To Use ## Supported Website -
 [AnonFiles](https://anonfiles.com/) - [Mediafire](https://mediafire.com/) -
 [Google Drive](https://drive.google.com/) - [Myfile](https://myfile.is/) -
@@ -40,10 +40,10 @@
 'picture', # 'size': {'readable': '73.62KB'}}, # 'url': {'directDownload':
 'https://download1482.mediafire.com/h32ugeuxwitg/n2kcs3n9nd88vnr/picture.jpeg',
 # 'original': 'https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/
 file'}}}, # 'status': 'true'} ``` Download the file `download=True` ```py from
 Direct_Download import Direct url = Direct() #Use download By Enabling download
 to True for downloading your file url.mediafire('https://www.mediafire.com/
 file/n2kcs3n9nd88vnr/picture.jpeg/file', download=True) ``` ## Links - [PyPI]
-(https://pypi.org/project/Direct-Download/) - [API](https://ddl-
-api.cycno.repl.co/) ## Contributors ### [CYCNO] Contributors are always
+(https://pypi.org/project/Direct-Download/) - [API](https://github.com/CYCNO/
+Direct-Download-API) ## Contributors ### [CYCNO] Contributors are always
 welcome!
```

### Comparing `Direct-Download-0.4.3/README.md` & `Direct-Download-0.4.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <strong><i>A simple yet powerful tool for getting direct download link.</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/Direct-Download/">
-<img src="https://img.shields.io/badge/PYPI-V0.4.1-blue?logo=PyPI&style=for-the-badge">
+<img src="https://img.shields.io/badge/PYPI-V0.4-blue?logo=PyPI&style=for-the-badge">
 </a>
 <a href="https://github.com/CYCNO/DirectDownload/graphs/contributors">
 <img src="https://img.shields.io/github/contributors/cycno/DirectDownload?style=for-the-badge&color=green&logo=GitHub">
 </a>
 </div>
 
 ---
@@ -96,13 +96,13 @@
 url = Direct()
 
 #Use download By Enabling download to True for downloading your file 
 url.mediafire('https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', download=True)
 ```
 ## Links
 - [PyPI](https://pypi.org/project/Direct-Download/)
-- [API](https://ddl-api.cycno.repl.co/)
+- [API](https://github.com/CYCNO/Direct-Download-API)
 
 ## Contributors
 ### <a href="https://github.com/CYCNO"><img src="https://avatars.githubusercontent.com/u/90704569?v=4" alt="CYCNO" width="50" height="50" style="border-radius: 50%;"></a>
 
 Contributors are always welcome!
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                          ****** Direct Download ******
          A simple yet powerful tool for getting direct download link.
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-badge/PYPI-V0.4.1-blue?logo=PyPI&style=for-the-badge] [https://img.shields.io/
+ badge/PYPI-V0.4-blue?logo=PyPI&style=for-the-badge] [https://img.shields.io/
             github/contributors/cycno/DirectDownload?style=for-the-
                         badge&color=green&logo=GitHub]
 --- ## Feautres - All Information Of File Is Available - No Need To Sign Up Or
 Usage Of Tokens - Data Is In JSON Format - Download the file - Switch Between
 Just Download Link Or ALL Information - Very Easy To Use ## Supported Website -
 [AnonFiles](https://anonfiles.com/) - [Mediafire](https://mediafire.com/) -
 [Google Drive](https://drive.google.com/) - [Myfile](https://myfile.is/) -
@@ -30,10 +30,10 @@
 'picture', # 'size': {'readable': '73.62KB'}}, # 'url': {'directDownload':
 'https://download1482.mediafire.com/h32ugeuxwitg/n2kcs3n9nd88vnr/picture.jpeg',
 # 'original': 'https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/
 file'}}}, # 'status': 'true'} ``` Download the file `download=True` ```py from
 Direct_Download import Direct url = Direct() #Use download By Enabling download
 to True for downloading your file url.mediafire('https://www.mediafire.com/
 file/n2kcs3n9nd88vnr/picture.jpeg/file', download=True) ``` ## Links - [PyPI]
-(https://pypi.org/project/Direct-Download/) - [API](https://ddl-
-api.cycno.repl.co/) ## Contributors ### [CYCNO] Contributors are always
+(https://pypi.org/project/Direct-Download/) - [API](https://github.com/CYCNO/
+Direct-Download-API) ## Contributors ### [CYCNO] Contributors are always
 welcome!
```

### Comparing `Direct-Download-0.4.3/setup.py` & `Direct-Download-0.4.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='Direct-Download',
-    version='0.4.3',
+    version='0.4.4',
     description='A Direct Downloader Module Which Will Get Direct Download Link From Some Popular File Uploading Websites Like Mediafire, Anonfiles',
     author= 'CYCNO',
     url = 'https://github.com/CYCNO/DirectDownload',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages('src'),
     keywords=['direct download', 'anonfiles', 'mediafire','mediafire direct download','anonfiles direct download','google drive','google drive direct download link','google drive download link','megaupload','myfile','letsupload','filechan'],
```

### Comparing `Direct-Download-0.4.3/src/Direct_Download.egg-info/PKG-INFO` & `Direct-Download-0.4.4/src/Direct_Download.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Direct-Download
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Direct Downloader Module Which Will Get Direct Download Link From Some Popular File Uploading Websites Like Mediafire, Anonfiles
 Home-page: https://github.com/CYCNO/DirectDownload
 Author: CYCNO
 Keywords: direct download,anonfiles,mediafire,mediafire direct download,anonfiles direct download,google drive,google drive direct download link,google drive download link,megaupload,myfile,letsupload,filechan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 <strong><i>A simple yet powerful tool for getting direct download link.</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/Direct-Download/">
-<img src="https://img.shields.io/badge/PYPI-V0.4.1-blue?logo=PyPI&style=for-the-badge">
+<img src="https://img.shields.io/badge/PYPI-V0.4-blue?logo=PyPI&style=for-the-badge">
 </a>
 <a href="https://github.com/CYCNO/DirectDownload/graphs/contributors">
 <img src="https://img.shields.io/github/contributors/cycno/DirectDownload?style=for-the-badge&color=green&logo=GitHub">
 </a>
 </div>
 
 ---
@@ -110,13 +110,13 @@
 url = Direct()
 
 #Use download By Enabling download to True for downloading your file 
 url.mediafire('https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', download=True)
 ```
 ## Links
 - [PyPI](https://pypi.org/project/Direct-Download/)
-- [API](https://ddl-api.cycno.repl.co/)
+- [API](https://github.com/CYCNO/Direct-Download-API)
 
 ## Contributors
 ### <a href="https://github.com/CYCNO"><img src="https://avatars.githubusercontent.com/u/90704569?v=4" alt="CYCNO" width="50" height="50" style="border-radius: 50%;"></a>
 
 Contributors are always welcome!
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: Direct-Download Version: 0.4.3 Summary: A Direct
+Metadata-Version: 2.1 Name: Direct-Download Version: 0.4.4 Summary: A Direct
 Downloader Module Which Will Get Direct Download Link From Some Popular File
 Uploading Websites Like Mediafire, Anonfiles Home-page: https://github.com/
 CYCNO/DirectDownload Author: CYCNO Keywords: direct
 download,anonfiles,mediafire,mediafire direct download,anonfiles direct
 download,google drive,google drive direct download link,google drive download
 link,megaupload,myfile,letsupload,filechan Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE
                          ****** Direct Download ******
          A simple yet powerful tool for getting direct download link.
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-badge/PYPI-V0.4.1-blue?logo=PyPI&style=for-the-badge] [https://img.shields.io/
+ badge/PYPI-V0.4-blue?logo=PyPI&style=for-the-badge] [https://img.shields.io/
             github/contributors/cycno/DirectDownload?style=for-the-
                         badge&color=green&logo=GitHub]
 --- ## Feautres - All Information Of File Is Available - No Need To Sign Up Or
 Usage Of Tokens - Data Is In JSON Format - Download the file - Switch Between
 Just Download Link Or ALL Information - Very Easy To Use ## Supported Website -
 [AnonFiles](https://anonfiles.com/) - [Mediafire](https://mediafire.com/) -
 [Google Drive](https://drive.google.com/) - [Myfile](https://myfile.is/) -
@@ -40,10 +40,10 @@
 'picture', # 'size': {'readable': '73.62KB'}}, # 'url': {'directDownload':
 'https://download1482.mediafire.com/h32ugeuxwitg/n2kcs3n9nd88vnr/picture.jpeg',
 # 'original': 'https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/
 file'}}}, # 'status': 'true'} ``` Download the file `download=True` ```py from
 Direct_Download import Direct url = Direct() #Use download By Enabling download
 to True for downloading your file url.mediafire('https://www.mediafire.com/
 file/n2kcs3n9nd88vnr/picture.jpeg/file', download=True) ``` ## Links - [PyPI]
-(https://pypi.org/project/Direct-Download/) - [API](https://ddl-
-api.cycno.repl.co/) ## Contributors ### [CYCNO] Contributors are always
+(https://pypi.org/project/Direct-Download/) - [API](https://github.com/CYCNO/
+Direct-Download-API) ## Contributors ### [CYCNO] Contributors are always
 welcome!
```

### Comparing `Direct-Download-0.4.3/src/Direct_Download.py` & `Direct-Download-0.4.4/src/Direct_Download.py`

 * *Files identical despite different names*

