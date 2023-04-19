# Comparing `tmp/Direct_Download-0.4.2.tar.gz` & `tmp/Direct-Download-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Direct_Download-0.4.2.tar", last modified: Mon Nov 14 13:30:44 2022, max compression
+gzip compressed data, was "Direct-Download-0.4.3.tar", last modified: Wed Apr 19 07:02:27 2023, max compression
```

## Comparing `Direct_Download-0.4.2.tar` & `Direct-Download-0.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-11-14 13:30:44.313454 Direct_Download-0.4.2/
--rw-rw-rw-   0        0        0     1081 2022-10-30 07:06:08.000000 Direct_Download-0.4.2/LICENSE
--rw-rw-rw-   0        0        0     3715 2022-11-14 13:30:44.309454 Direct_Download-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3131 2022-11-14 13:29:53.000000 Direct_Download-0.4.2/README.md
--rw-rw-rw-   0        0        0       42 2022-11-14 13:30:44.314455 Direct_Download-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      982 2022-11-14 13:30:03.000000 Direct_Download-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-14 13:30:44.246438 Direct_Download-0.4.2/src/
-drwxrwxrwx   0        0        0        0 2022-11-14 13:30:44.300451 Direct_Download-0.4.2/src/Direct_Download.egg-info/
--rw-rw-rw-   0        0        0     3715 2022-11-14 13:30:43.000000 Direct_Download-0.4.2/src/Direct_Download.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2022-11-14 13:30:43.000000 Direct_Download-0.4.2/src/Direct_Download.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-14 13:30:43.000000 Direct_Download-0.4.2/src/Direct_Download.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2022-11-14 13:30:43.000000 Direct_Download-0.4.2/src/Direct_Download.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-11-14 13:30:43.000000 Direct_Download-0.4.2/src/Direct_Download.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3833 2022-10-30 07:06:11.000000 Direct_Download-0.4.2/src/Direct_Download.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:02:27.515823 Direct-Download-0.4.3/
+-rw-rw-rw-   0        0        0     1061 2022-11-14 16:03:35.000000 Direct-Download-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0     4147 2023-04-19 07:02:27.481814 Direct-Download-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3319 2023-04-18 15:39:51.000000 Direct-Download-0.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 07:02:27.516824 Direct-Download-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1107 2023-04-18 16:15:29.000000 Direct-Download-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:02:27.407796 Direct-Download-0.4.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 07:02:27.465809 Direct-Download-0.4.3/src/Direct_Download.egg-info/
+-rw-rw-rw-   0        0        0     4147 2023-04-19 07:02:26.000000 Direct-Download-0.4.3/src/Direct_Download.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-19 07:02:26.000000 Direct-Download-0.4.3/src/Direct_Download.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 07:02:26.000000 Direct-Download-0.4.3/src/Direct_Download.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-19 07:02:26.000000 Direct-Download-0.4.3/src/Direct_Download.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-19 07:02:26.000000 Direct-Download-0.4.3/src/Direct_Download.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3888 2023-04-18 15:24:17.000000 Direct-Download-0.4.3/src/Direct_Download.py
```

### Comparing `Direct_Download-0.4.2/PKG-INFO` & `Direct-Download-0.4.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: Direct_Download
-Version: 0.4.2
-Summary: A Direct Downloader Module Which Will Get Direct Download Link From Some Popular File Uploading Websites
+Name: Direct-Download
+Version: 0.4.3
+Summary: A Direct Downloader Module Which Will Get Direct Download Link From Some Popular File Uploading Websites Like Mediafire, Anonfiles
 Home-page: https://github.com/CYCNO/DirectDownload
 Author: CYCNO
-Keywords: direct download,anonfiles,mediafire,mediafire direct download,anonfiles direct download
+Keywords: direct download,anonfiles,mediafire,mediafire direct download,anonfiles direct download,google drive,google drive direct download link,google drive download link,megaupload,myfile,letsupload,filechan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -17,37 +17,41 @@
 <strong><i>A simple yet powerful tool for getting direct download link.</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/Direct-Download/">
-<img src="https://img.shields.io/badge/PYPI-V0.4-blue?logo=PyPI&style=for-the-badge">
+<img src="https://img.shields.io/badge/PYPI-V0.4.1-blue?logo=PyPI&style=for-the-badge">
 </a>
 <a href="https://github.com/CYCNO/DirectDownload/graphs/contributors">
-<img src="https://img.shields.io/github/contributors/cycno/justudy?style=for-the-badge&color=green&logo=GitHub">
+<img src="https://img.shields.io/github/contributors/cycno/DirectDownload?style=for-the-badge&color=green&logo=GitHub">
 </a>
 </div>
 
 ---
 
 ## Feautres
 
  - All Information Of File Is Available
  - No Need To Sign Up Or Usage Of Tokens 
  - Data Is In JSON Format 
- - Redirect link in default browser
+ - Download the file
  - Switch Between Just Download Link Or ALL Information
- - very Easy To Use
+ - Very Easy To Use
  
  ## Supported Website
 
 - [AnonFiles](https://anonfiles.com/)
 - [Mediafire](https://mediafire.com/)
-- More Added Soon...
+- [Google Drive](https://drive.google.com/)
+- [Myfile](https://myfile.is/)
+- [Letsupload](https://letsupload.cc/)
+- [Filechan](https://filechan.org/)
+- [MegaUpload](https://megaupload.nz/)
 
 ## Installation
 You Can Install Direct Download Using PIP
 
 ```bash
 pip install Direct-Download
 ```
@@ -62,30 +66,29 @@
 url = Direct()
 
 #For mediafire
 link = url.mediafire('https://www.mediafire.com/view/n2kcs3n9nd88vnr/picture.jpeg/file')
 print(link)
 
 #Output
-#{'directDownload': 'https://download1482.mediafire.com/4f1knkpxhq6g/n2kcs3n9nd88vnr/picture.jpeg'}
+#'https://download1482.mediafire.com/4f1knkpxhq6g/n2kcs3n9nd88vnr/picture.jpeg'
 
 #For Anonfiles
 link = url.anonfiles('https://anonfiles.com/n4pdf5Fdy1/night-mountains-minimalist-8k-wo_1_jpeg')
 print(link)
 
 #Output
-#{'directDownload': 'https://cdn-126.anonfiles.com/n4pdf5Fdy1/889ab081-1667110179/night-mountains-minimalist-8k-wo (1).jpeg'}
+#'https://cdn-126.anonfiles.com/n4pdf5Fdy1/889ab081-1667110179/night-mountains-minimalist-8k-wo (1).jpeg'
 ```
 
 ## Usage/Examples
 Get All Information About File `metadata=True`
 
 ```py
 from Direct_Download import Direct
-from pprint import pprint
 
 url = Direct()
 
 #Use Metadata By Enabling Metadata to True
 link = url.mediafire('https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', metadata=True)
 print(link)
 
@@ -96,23 +99,24 @@
 #                                'name': 'picture',
 #                                'size': {'readable': '73.62KB'}},
 #                  'url': {'directDownload': 'https://download1482.mediafire.com/h32ugeuxwitg/n2kcs3n9nd88vnr/picture.jpeg',
 #                           'original': 'https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file'}}},
 # 'status': 'true'}
 ```
 
-Open Link In Your Browser `redirect=True`
+Download the file `download=True`
 ```py
 from Direct_Download import Direct
 
 url = Direct()
 
-#Use Redirect By Enabling Redirect to True
-url.mediafire('https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', redirect=True)
+#Use download By Enabling download to True for downloading your file 
+url.mediafire('https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', download=True)
 ```
 ## Links
 - [PyPI](https://pypi.org/project/Direct-Download/)
+- [API](https://ddl-api.cycno.repl.co/)
 
 ## Contributors
-- [@CYCNO](https://github.com/CYCNO)
+### <a href="https://github.com/CYCNO"><img src="https://avatars.githubusercontent.com/u/90704569?v=4" alt="CYCNO" width="50" height="50" style="border-radius: 50%;"></a>
 
-Contributorsare always welcome!
+Contributors are always welcome!
```

#### html2text {}

```diff
@@ -1,44 +1,49 @@
-Metadata-Version: 2.1 Name: Direct_Download Version: 0.4.2 Summary: A Direct
+Metadata-Version: 2.1 Name: Direct-Download Version: 0.4.3 Summary: A Direct
 Downloader Module Which Will Get Direct Download Link From Some Popular File
-Uploading Websites Home-page: https://github.com/CYCNO/DirectDownload Author:
-CYCNO Keywords: direct download,anonfiles,mediafire,mediafire direct
-download,anonfiles direct download Classifier: Programming Language :: Python
-:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE
+Uploading Websites Like Mediafire, Anonfiles Home-page: https://github.com/
+CYCNO/DirectDownload Author: CYCNO Keywords: direct
+download,anonfiles,mediafire,mediafire direct download,anonfiles direct
+download,google drive,google drive direct download link,google drive download
+link,megaupload,myfile,letsupload,filechan Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
+Type: text/markdown License-File: LICENSE
                          ****** Direct Download ******
          A simple yet powerful tool for getting direct download link.
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
- badge/PYPI-V0.4-blue?logo=PyPI&style=for-the-badge] [https://img.shields.io/
-github/contributors/cycno/justudy?style=for-the-badge&color=green&logo=GitHub]
+badge/PYPI-V0.4.1-blue?logo=PyPI&style=for-the-badge] [https://img.shields.io/
+            github/contributors/cycno/DirectDownload?style=for-the-
+                        badge&color=green&logo=GitHub]
 --- ## Feautres - All Information Of File Is Available - No Need To Sign Up Or
-Usage Of Tokens - Data Is In JSON Format - Redirect link in default browser -
-Switch Between Just Download Link Or ALL Information - very Easy To Use ##
-Supported Website - [AnonFiles](https://anonfiles.com/) - [Mediafire](https://
-mediafire.com/) - More Added Soon... ## Installation You Can Install Direct
+Usage Of Tokens - Data Is In JSON Format - Download the file - Switch Between
+Just Download Link Or ALL Information - Very Easy To Use ## Supported Website -
+[AnonFiles](https://anonfiles.com/) - [Mediafire](https://mediafire.com/) -
+[Google Drive](https://drive.google.com/) - [Myfile](https://myfile.is/) -
+[Letsupload](https://letsupload.cc/) - [Filechan](https://filechan.org/) -
+[MegaUpload](https://megaupload.nz/) ## Installation You Can Install Direct
 Download Using PIP ```bash pip install Direct-Download ``` ## Quick Start ```py
 #First Import Direct From Module from Direct_Download import Direct #Declaring
 Variable As a Class url = Direct() #For mediafire link = url.mediafire('https:/
 /www.mediafire.com/view/n2kcs3n9nd88vnr/picture.jpeg/file') print(link) #Output
-#{'directDownload': 'https://download1482.mediafire.com/4f1knkpxhq6g/
-n2kcs3n9nd88vnr/picture.jpeg'} #For Anonfiles link = url.anonfiles('https://
-anonfiles.com/n4pdf5Fdy1/night-mountains-minimalist-8k-wo_1_jpeg') print(link)
-#Output #{'directDownload': 'https://cdn-126.anonfiles.com/n4pdf5Fdy1/889ab081-
-1667110179/night-mountains-minimalist-8k-wo (1).jpeg'} ``` ## Usage/Examples
-Get All Information About File `metadata=True` ```py from Direct_Download
-import Direct from pprint import pprint url = Direct() #Use Metadata By
-Enabling Metadata to True link = url.mediafire('https://www.mediafire.com/file/
-n2kcs3n9nd88vnr/picture.jpeg/file', metadata=True) print(link) # Output #
-{'data': {'file': {'metadata': {'DateAndTime': {'date': '2022-10-20', # 'time':
-'11:00:27'}, # 'id': 'www.mediafire.com', # 'name': 'picture', # 'size':
-{'readable': '73.62KB'}}, # 'url': {'directDownload': 'https://
-download1482.mediafire.com/h32ugeuxwitg/n2kcs3n9nd88vnr/picture.jpeg', #
-'original': 'https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/
-file'}}}, # 'status': 'true'} ``` Open Link In Your Browser `redirect=True`
-```py from Direct_Download import Direct url = Direct() #Use Redirect By
-Enabling Redirect to True url.mediafire('https://www.mediafire.com/file/
-n2kcs3n9nd88vnr/picture.jpeg/file', redirect=True) ``` ## Links - [PyPI](https:
-//pypi.org/project/Direct-Download/) ## Contributors - [@CYCNO](https://
-github.com/CYCNO) Contributorsare always welcome!
+#'https://download1482.mediafire.com/4f1knkpxhq6g/n2kcs3n9nd88vnr/picture.jpeg'
+#For Anonfiles link = url.anonfiles('https://anonfiles.com/n4pdf5Fdy1/night-
+mountains-minimalist-8k-wo_1_jpeg') print(link) #Output #'https://cdn-
+126.anonfiles.com/n4pdf5Fdy1/889ab081-1667110179/night-mountains-minimalist-8k-
+wo (1).jpeg' ``` ## Usage/Examples Get All Information About File
+`metadata=True` ```py from Direct_Download import Direct url = Direct() #Use
+Metadata By Enabling Metadata to True link = url.mediafire('https://
+www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', metadata=True) print
+(link) # Output #{'data': {'file': {'metadata': {'DateAndTime': {'date': '2022-
+10-20', # 'time': '11:00:27'}, # 'id': 'www.mediafire.com', # 'name':
+'picture', # 'size': {'readable': '73.62KB'}}, # 'url': {'directDownload':
+'https://download1482.mediafire.com/h32ugeuxwitg/n2kcs3n9nd88vnr/picture.jpeg',
+# 'original': 'https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/
+file'}}}, # 'status': 'true'} ``` Download the file `download=True` ```py from
+Direct_Download import Direct url = Direct() #Use download By Enabling download
+to True for downloading your file url.mediafire('https://www.mediafire.com/
+file/n2kcs3n9nd88vnr/picture.jpeg/file', download=True) ``` ## Links - [PyPI]
+(https://pypi.org/project/Direct-Download/) - [API](https://ddl-
+api.cycno.repl.co/) ## Contributors ### [CYCNO] Contributors are always
+welcome!
```

### Comparing `Direct_Download-0.4.2/README.md` & `Direct-Download-0.4.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,104 +1,108 @@
-<div align="center">
-<h1 align="center">Direct Download</h1>
-<strong><i>A simple yet powerful tool for getting direct download link.</i></strong>
-<br>
-<br>
-<a href="https://www.python.org/">
-<img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
-</a>
-<a href="https://pypi.org/project/Direct-Download/">
-<img src="https://img.shields.io/badge/PYPI-V0.4-blue?logo=PyPI&style=for-the-badge">
-</a>
-<a href="https://github.com/CYCNO/DirectDownload/graphs/contributors">
-<img src="https://img.shields.io/github/contributors/cycno/justudy?style=for-the-badge&color=green&logo=GitHub">
-</a>
-</div>
-
----
-
-## Feautres
-
- - All Information Of File Is Available
- - No Need To Sign Up Or Usage Of Tokens 
- - Data Is In JSON Format 
- - Redirect link in default browser
- - Switch Between Just Download Link Or ALL Information
- - very Easy To Use
- 
- ## Supported Website
-
-- [AnonFiles](https://anonfiles.com/)
-- [Mediafire](https://mediafire.com/)
-- More Added Soon...
-
-## Installation
-You Can Install Direct Download Using PIP
-
-```bash
-pip install Direct-Download
-```
-
-## Quick Start
-
-```py
-#First Import Direct From Module
-from Direct_Download import Direct
-
-#Declaring Variable As a Class
-url = Direct()
-
-#For mediafire
-link = url.mediafire('https://www.mediafire.com/view/n2kcs3n9nd88vnr/picture.jpeg/file')
-print(link)
-
-#Output
-#{'directDownload': 'https://download1482.mediafire.com/4f1knkpxhq6g/n2kcs3n9nd88vnr/picture.jpeg'}
-
-#For Anonfiles
-link = url.anonfiles('https://anonfiles.com/n4pdf5Fdy1/night-mountains-minimalist-8k-wo_1_jpeg')
-print(link)
-
-#Output
-#{'directDownload': 'https://cdn-126.anonfiles.com/n4pdf5Fdy1/889ab081-1667110179/night-mountains-minimalist-8k-wo (1).jpeg'}
-```
-
-## Usage/Examples
-Get All Information About File `metadata=True`
-
-```py
-from Direct_Download import Direct
-from pprint import pprint
-
-url = Direct()
-
-#Use Metadata By Enabling Metadata to True
-link = url.mediafire('https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', metadata=True)
-print(link)
-
-# Output
-#{'data': {'file': {'metadata': {'DateAndTime': {'date': '2022-10-20',
-#                                                'time': '11:00:27'},
-#                                'id': 'www.mediafire.com',
-#                                'name': 'picture',
-#                                'size': {'readable': '73.62KB'}},
-#                  'url': {'directDownload': 'https://download1482.mediafire.com/h32ugeuxwitg/n2kcs3n9nd88vnr/picture.jpeg',
-#                           'original': 'https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file'}}},
-# 'status': 'true'}
-```
-
-Open Link In Your Browser `redirect=True`
-```py
-from Direct_Download import Direct
-
-url = Direct()
-
-#Use Redirect By Enabling Redirect to True
-url.mediafire('https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', redirect=True)
-```
-## Links
-- [PyPI](https://pypi.org/project/Direct-Download/)
-
-## Contributors
-- [@CYCNO](https://github.com/CYCNO)
-
-Contributorsare always welcome!
+<div align="center">
+<h1 align="center">Direct Download</h1>
+<strong><i>A simple yet powerful tool for getting direct download link.</i></strong>
+<br>
+<br>
+<a href="https://www.python.org/">
+<img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
+</a>
+<a href="https://pypi.org/project/Direct-Download/">
+<img src="https://img.shields.io/badge/PYPI-V0.4.1-blue?logo=PyPI&style=for-the-badge">
+</a>
+<a href="https://github.com/CYCNO/DirectDownload/graphs/contributors">
+<img src="https://img.shields.io/github/contributors/cycno/DirectDownload?style=for-the-badge&color=green&logo=GitHub">
+</a>
+</div>
+
+---
+
+## Feautres
+
+ - All Information Of File Is Available
+ - No Need To Sign Up Or Usage Of Tokens 
+ - Data Is In JSON Format 
+ - Download the file
+ - Switch Between Just Download Link Or ALL Information
+ - Very Easy To Use
+ 
+ ## Supported Website
+
+- [AnonFiles](https://anonfiles.com/)
+- [Mediafire](https://mediafire.com/)
+- [Google Drive](https://drive.google.com/)
+- [Myfile](https://myfile.is/)
+- [Letsupload](https://letsupload.cc/)
+- [Filechan](https://filechan.org/)
+- [MegaUpload](https://megaupload.nz/)
+
+## Installation
+You Can Install Direct Download Using PIP
+
+```bash
+pip install Direct-Download
+```
+
+## Quick Start
+
+```py
+#First Import Direct From Module
+from Direct_Download import Direct
+
+#Declaring Variable As a Class
+url = Direct()
+
+#For mediafire
+link = url.mediafire('https://www.mediafire.com/view/n2kcs3n9nd88vnr/picture.jpeg/file')
+print(link)
+
+#Output
+#'https://download1482.mediafire.com/4f1knkpxhq6g/n2kcs3n9nd88vnr/picture.jpeg'
+
+#For Anonfiles
+link = url.anonfiles('https://anonfiles.com/n4pdf5Fdy1/night-mountains-minimalist-8k-wo_1_jpeg')
+print(link)
+
+#Output
+#'https://cdn-126.anonfiles.com/n4pdf5Fdy1/889ab081-1667110179/night-mountains-minimalist-8k-wo (1).jpeg'
+```
+
+## Usage/Examples
+Get All Information About File `metadata=True`
+
+```py
+from Direct_Download import Direct
+
+url = Direct()
+
+#Use Metadata By Enabling Metadata to True
+link = url.mediafire('https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', metadata=True)
+print(link)
+
+# Output
+#{'data': {'file': {'metadata': {'DateAndTime': {'date': '2022-10-20',
+#                                                'time': '11:00:27'},
+#                                'id': 'www.mediafire.com',
+#                                'name': 'picture',
+#                                'size': {'readable': '73.62KB'}},
+#                  'url': {'directDownload': 'https://download1482.mediafire.com/h32ugeuxwitg/n2kcs3n9nd88vnr/picture.jpeg',
+#                           'original': 'https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file'}}},
+# 'status': 'true'}
+```
+
+Download the file `download=True`
+```py
+from Direct_Download import Direct
+
+url = Direct()
+
+#Use download By Enabling download to True for downloading your file 
+url.mediafire('https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', download=True)
+```
+## Links
+- [PyPI](https://pypi.org/project/Direct-Download/)
+- [API](https://ddl-api.cycno.repl.co/)
+
+## Contributors
+### <a href="https://github.com/CYCNO"><img src="https://avatars.githubusercontent.com/u/90704569?v=4" alt="CYCNO" width="50" height="50" style="border-radius: 50%;"></a>
+
+Contributors are always welcome!
```

#### html2text {}

```diff
@@ -1,36 +1,39 @@
                          ****** Direct Download ******
          A simple yet powerful tool for getting direct download link.
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
- badge/PYPI-V0.4-blue?logo=PyPI&style=for-the-badge] [https://img.shields.io/
-github/contributors/cycno/justudy?style=for-the-badge&color=green&logo=GitHub]
+badge/PYPI-V0.4.1-blue?logo=PyPI&style=for-the-badge] [https://img.shields.io/
+            github/contributors/cycno/DirectDownload?style=for-the-
+                        badge&color=green&logo=GitHub]
 --- ## Feautres - All Information Of File Is Available - No Need To Sign Up Or
-Usage Of Tokens - Data Is In JSON Format - Redirect link in default browser -
-Switch Between Just Download Link Or ALL Information - very Easy To Use ##
-Supported Website - [AnonFiles](https://anonfiles.com/) - [Mediafire](https://
-mediafire.com/) - More Added Soon... ## Installation You Can Install Direct
+Usage Of Tokens - Data Is In JSON Format - Download the file - Switch Between
+Just Download Link Or ALL Information - Very Easy To Use ## Supported Website -
+[AnonFiles](https://anonfiles.com/) - [Mediafire](https://mediafire.com/) -
+[Google Drive](https://drive.google.com/) - [Myfile](https://myfile.is/) -
+[Letsupload](https://letsupload.cc/) - [Filechan](https://filechan.org/) -
+[MegaUpload](https://megaupload.nz/) ## Installation You Can Install Direct
 Download Using PIP ```bash pip install Direct-Download ``` ## Quick Start ```py
 #First Import Direct From Module from Direct_Download import Direct #Declaring
 Variable As a Class url = Direct() #For mediafire link = url.mediafire('https:/
 /www.mediafire.com/view/n2kcs3n9nd88vnr/picture.jpeg/file') print(link) #Output
-#{'directDownload': 'https://download1482.mediafire.com/4f1knkpxhq6g/
-n2kcs3n9nd88vnr/picture.jpeg'} #For Anonfiles link = url.anonfiles('https://
-anonfiles.com/n4pdf5Fdy1/night-mountains-minimalist-8k-wo_1_jpeg') print(link)
-#Output #{'directDownload': 'https://cdn-126.anonfiles.com/n4pdf5Fdy1/889ab081-
-1667110179/night-mountains-minimalist-8k-wo (1).jpeg'} ``` ## Usage/Examples
-Get All Information About File `metadata=True` ```py from Direct_Download
-import Direct from pprint import pprint url = Direct() #Use Metadata By
-Enabling Metadata to True link = url.mediafire('https://www.mediafire.com/file/
-n2kcs3n9nd88vnr/picture.jpeg/file', metadata=True) print(link) # Output #
-{'data': {'file': {'metadata': {'DateAndTime': {'date': '2022-10-20', # 'time':
-'11:00:27'}, # 'id': 'www.mediafire.com', # 'name': 'picture', # 'size':
-{'readable': '73.62KB'}}, # 'url': {'directDownload': 'https://
-download1482.mediafire.com/h32ugeuxwitg/n2kcs3n9nd88vnr/picture.jpeg', #
-'original': 'https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/
-file'}}}, # 'status': 'true'} ``` Open Link In Your Browser `redirect=True`
-```py from Direct_Download import Direct url = Direct() #Use Redirect By
-Enabling Redirect to True url.mediafire('https://www.mediafire.com/file/
-n2kcs3n9nd88vnr/picture.jpeg/file', redirect=True) ``` ## Links - [PyPI](https:
-//pypi.org/project/Direct-Download/) ## Contributors - [@CYCNO](https://
-github.com/CYCNO) Contributorsare always welcome!
+#'https://download1482.mediafire.com/4f1knkpxhq6g/n2kcs3n9nd88vnr/picture.jpeg'
+#For Anonfiles link = url.anonfiles('https://anonfiles.com/n4pdf5Fdy1/night-
+mountains-minimalist-8k-wo_1_jpeg') print(link) #Output #'https://cdn-
+126.anonfiles.com/n4pdf5Fdy1/889ab081-1667110179/night-mountains-minimalist-8k-
+wo (1).jpeg' ``` ## Usage/Examples Get All Information About File
+`metadata=True` ```py from Direct_Download import Direct url = Direct() #Use
+Metadata By Enabling Metadata to True link = url.mediafire('https://
+www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', metadata=True) print
+(link) # Output #{'data': {'file': {'metadata': {'DateAndTime': {'date': '2022-
+10-20', # 'time': '11:00:27'}, # 'id': 'www.mediafire.com', # 'name':
+'picture', # 'size': {'readable': '73.62KB'}}, # 'url': {'directDownload':
+'https://download1482.mediafire.com/h32ugeuxwitg/n2kcs3n9nd88vnr/picture.jpeg',
+# 'original': 'https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/
+file'}}}, # 'status': 'true'} ``` Download the file `download=True` ```py from
+Direct_Download import Direct url = Direct() #Use download By Enabling download
+to True for downloading your file url.mediafire('https://www.mediafire.com/
+file/n2kcs3n9nd88vnr/picture.jpeg/file', download=True) ``` ## Links - [PyPI]
+(https://pypi.org/project/Direct-Download/) - [API](https://ddl-
+api.cycno.repl.co/) ## Contributors ### [CYCNO] Contributors are always
+welcome!
```

### Comparing `Direct_Download-0.4.2/setup.py` & `Direct-Download-0.4.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-import setuptools
-from setuptools import setup
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setup(
-    name='Direct_Download',
-    version='0.4.2',
-    description='A Direct Downloader Module Which Will Get Direct Download Link From Some Popular File Uploading Websites',
-    author= 'CYCNO',
-    url = 'https://github.com/CYCNO/DirectDownload',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),
-    keywords=['direct download', 'anonfiles', 'mediafire','mediafire direct download','anonfiles direct download'],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.6',
-    py_modules=['Direct_Download'],
-    package_dir={'':'src'},
-    install_requires = [
-        'beautifulsoup4',
-        'requests'
-    ]
+from setuptools import setup, find_packages
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setup(
+    name='Direct-Download',
+    version='0.4.3',
+    description='A Direct Downloader Module Which Will Get Direct Download Link From Some Popular File Uploading Websites Like Mediafire, Anonfiles',
+    author= 'CYCNO',
+    url = 'https://github.com/CYCNO/DirectDownload',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    packages=find_packages('src'),
+    keywords=['direct download', 'anonfiles', 'mediafire','mediafire direct download','anonfiles direct download','google drive','google drive direct download link','google drive download link','megaupload','myfile','letsupload','filechan'],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.6',
+    py_modules=['Direct_Download'],
+    package_dir={'':'src'},
+    install_requires = [
+        'wget',
+        'requests'
+    ]
 )
```

### Comparing `Direct_Download-0.4.2/src/Direct_Download.egg-info/PKG-INFO` & `Direct-Download-0.4.3/src/Direct_Download.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: Direct-Download
-Version: 0.4.2
-Summary: A Direct Downloader Module Which Will Get Direct Download Link From Some Popular File Uploading Websites
+Version: 0.4.3
+Summary: A Direct Downloader Module Which Will Get Direct Download Link From Some Popular File Uploading Websites Like Mediafire, Anonfiles
 Home-page: https://github.com/CYCNO/DirectDownload
 Author: CYCNO
-Keywords: direct download,anonfiles,mediafire,mediafire direct download,anonfiles direct download
+Keywords: direct download,anonfiles,mediafire,mediafire direct download,anonfiles direct download,google drive,google drive direct download link,google drive download link,megaupload,myfile,letsupload,filechan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -17,37 +17,41 @@
 <strong><i>A simple yet powerful tool for getting direct download link.</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/Direct-Download/">
-<img src="https://img.shields.io/badge/PYPI-V0.4-blue?logo=PyPI&style=for-the-badge">
+<img src="https://img.shields.io/badge/PYPI-V0.4.1-blue?logo=PyPI&style=for-the-badge">
 </a>
 <a href="https://github.com/CYCNO/DirectDownload/graphs/contributors">
-<img src="https://img.shields.io/github/contributors/cycno/justudy?style=for-the-badge&color=green&logo=GitHub">
+<img src="https://img.shields.io/github/contributors/cycno/DirectDownload?style=for-the-badge&color=green&logo=GitHub">
 </a>
 </div>
 
 ---
 
 ## Feautres
 
  - All Information Of File Is Available
  - No Need To Sign Up Or Usage Of Tokens 
  - Data Is In JSON Format 
- - Redirect link in default browser
+ - Download the file
  - Switch Between Just Download Link Or ALL Information
- - very Easy To Use
+ - Very Easy To Use
  
  ## Supported Website
 
 - [AnonFiles](https://anonfiles.com/)
 - [Mediafire](https://mediafire.com/)
-- More Added Soon...
+- [Google Drive](https://drive.google.com/)
+- [Myfile](https://myfile.is/)
+- [Letsupload](https://letsupload.cc/)
+- [Filechan](https://filechan.org/)
+- [MegaUpload](https://megaupload.nz/)
 
 ## Installation
 You Can Install Direct Download Using PIP
 
 ```bash
 pip install Direct-Download
 ```
@@ -62,30 +66,29 @@
 url = Direct()
 
 #For mediafire
 link = url.mediafire('https://www.mediafire.com/view/n2kcs3n9nd88vnr/picture.jpeg/file')
 print(link)
 
 #Output
-#{'directDownload': 'https://download1482.mediafire.com/4f1knkpxhq6g/n2kcs3n9nd88vnr/picture.jpeg'}
+#'https://download1482.mediafire.com/4f1knkpxhq6g/n2kcs3n9nd88vnr/picture.jpeg'
 
 #For Anonfiles
 link = url.anonfiles('https://anonfiles.com/n4pdf5Fdy1/night-mountains-minimalist-8k-wo_1_jpeg')
 print(link)
 
 #Output
-#{'directDownload': 'https://cdn-126.anonfiles.com/n4pdf5Fdy1/889ab081-1667110179/night-mountains-minimalist-8k-wo (1).jpeg'}
+#'https://cdn-126.anonfiles.com/n4pdf5Fdy1/889ab081-1667110179/night-mountains-minimalist-8k-wo (1).jpeg'
 ```
 
 ## Usage/Examples
 Get All Information About File `metadata=True`
 
 ```py
 from Direct_Download import Direct
-from pprint import pprint
 
 url = Direct()
 
 #Use Metadata By Enabling Metadata to True
 link = url.mediafire('https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', metadata=True)
 print(link)
 
@@ -96,23 +99,24 @@
 #                                'name': 'picture',
 #                                'size': {'readable': '73.62KB'}},
 #                  'url': {'directDownload': 'https://download1482.mediafire.com/h32ugeuxwitg/n2kcs3n9nd88vnr/picture.jpeg',
 #                           'original': 'https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file'}}},
 # 'status': 'true'}
 ```
 
-Open Link In Your Browser `redirect=True`
+Download the file `download=True`
 ```py
 from Direct_Download import Direct
 
 url = Direct()
 
-#Use Redirect By Enabling Redirect to True
-url.mediafire('https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', redirect=True)
+#Use download By Enabling download to True for downloading your file 
+url.mediafire('https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', download=True)
 ```
 ## Links
 - [PyPI](https://pypi.org/project/Direct-Download/)
+- [API](https://ddl-api.cycno.repl.co/)
 
 ## Contributors
-- [@CYCNO](https://github.com/CYCNO)
+### <a href="https://github.com/CYCNO"><img src="https://avatars.githubusercontent.com/u/90704569?v=4" alt="CYCNO" width="50" height="50" style="border-radius: 50%;"></a>
 
-Contributorsare always welcome!
+Contributors are always welcome!
```

#### html2text {}

```diff
@@ -1,44 +1,49 @@
-Metadata-Version: 2.1 Name: Direct-Download Version: 0.4.2 Summary: A Direct
+Metadata-Version: 2.1 Name: Direct-Download Version: 0.4.3 Summary: A Direct
 Downloader Module Which Will Get Direct Download Link From Some Popular File
-Uploading Websites Home-page: https://github.com/CYCNO/DirectDownload Author:
-CYCNO Keywords: direct download,anonfiles,mediafire,mediafire direct
-download,anonfiles direct download Classifier: Programming Language :: Python
-:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE
+Uploading Websites Like Mediafire, Anonfiles Home-page: https://github.com/
+CYCNO/DirectDownload Author: CYCNO Keywords: direct
+download,anonfiles,mediafire,mediafire direct download,anonfiles direct
+download,google drive,google drive direct download link,google drive download
+link,megaupload,myfile,letsupload,filechan Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
+Type: text/markdown License-File: LICENSE
                          ****** Direct Download ******
          A simple yet powerful tool for getting direct download link.
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
- badge/PYPI-V0.4-blue?logo=PyPI&style=for-the-badge] [https://img.shields.io/
-github/contributors/cycno/justudy?style=for-the-badge&color=green&logo=GitHub]
+badge/PYPI-V0.4.1-blue?logo=PyPI&style=for-the-badge] [https://img.shields.io/
+            github/contributors/cycno/DirectDownload?style=for-the-
+                        badge&color=green&logo=GitHub]
 --- ## Feautres - All Information Of File Is Available - No Need To Sign Up Or
-Usage Of Tokens - Data Is In JSON Format - Redirect link in default browser -
-Switch Between Just Download Link Or ALL Information - very Easy To Use ##
-Supported Website - [AnonFiles](https://anonfiles.com/) - [Mediafire](https://
-mediafire.com/) - More Added Soon... ## Installation You Can Install Direct
+Usage Of Tokens - Data Is In JSON Format - Download the file - Switch Between
+Just Download Link Or ALL Information - Very Easy To Use ## Supported Website -
+[AnonFiles](https://anonfiles.com/) - [Mediafire](https://mediafire.com/) -
+[Google Drive](https://drive.google.com/) - [Myfile](https://myfile.is/) -
+[Letsupload](https://letsupload.cc/) - [Filechan](https://filechan.org/) -
+[MegaUpload](https://megaupload.nz/) ## Installation You Can Install Direct
 Download Using PIP ```bash pip install Direct-Download ``` ## Quick Start ```py
 #First Import Direct From Module from Direct_Download import Direct #Declaring
 Variable As a Class url = Direct() #For mediafire link = url.mediafire('https:/
 /www.mediafire.com/view/n2kcs3n9nd88vnr/picture.jpeg/file') print(link) #Output
-#{'directDownload': 'https://download1482.mediafire.com/4f1knkpxhq6g/
-n2kcs3n9nd88vnr/picture.jpeg'} #For Anonfiles link = url.anonfiles('https://
-anonfiles.com/n4pdf5Fdy1/night-mountains-minimalist-8k-wo_1_jpeg') print(link)
-#Output #{'directDownload': 'https://cdn-126.anonfiles.com/n4pdf5Fdy1/889ab081-
-1667110179/night-mountains-minimalist-8k-wo (1).jpeg'} ``` ## Usage/Examples
-Get All Information About File `metadata=True` ```py from Direct_Download
-import Direct from pprint import pprint url = Direct() #Use Metadata By
-Enabling Metadata to True link = url.mediafire('https://www.mediafire.com/file/
-n2kcs3n9nd88vnr/picture.jpeg/file', metadata=True) print(link) # Output #
-{'data': {'file': {'metadata': {'DateAndTime': {'date': '2022-10-20', # 'time':
-'11:00:27'}, # 'id': 'www.mediafire.com', # 'name': 'picture', # 'size':
-{'readable': '73.62KB'}}, # 'url': {'directDownload': 'https://
-download1482.mediafire.com/h32ugeuxwitg/n2kcs3n9nd88vnr/picture.jpeg', #
-'original': 'https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/
-file'}}}, # 'status': 'true'} ``` Open Link In Your Browser `redirect=True`
-```py from Direct_Download import Direct url = Direct() #Use Redirect By
-Enabling Redirect to True url.mediafire('https://www.mediafire.com/file/
-n2kcs3n9nd88vnr/picture.jpeg/file', redirect=True) ``` ## Links - [PyPI](https:
-//pypi.org/project/Direct-Download/) ## Contributors - [@CYCNO](https://
-github.com/CYCNO) Contributorsare always welcome!
+#'https://download1482.mediafire.com/4f1knkpxhq6g/n2kcs3n9nd88vnr/picture.jpeg'
+#For Anonfiles link = url.anonfiles('https://anonfiles.com/n4pdf5Fdy1/night-
+mountains-minimalist-8k-wo_1_jpeg') print(link) #Output #'https://cdn-
+126.anonfiles.com/n4pdf5Fdy1/889ab081-1667110179/night-mountains-minimalist-8k-
+wo (1).jpeg' ``` ## Usage/Examples Get All Information About File
+`metadata=True` ```py from Direct_Download import Direct url = Direct() #Use
+Metadata By Enabling Metadata to True link = url.mediafire('https://
+www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/file', metadata=True) print
+(link) # Output #{'data': {'file': {'metadata': {'DateAndTime': {'date': '2022-
+10-20', # 'time': '11:00:27'}, # 'id': 'www.mediafire.com', # 'name':
+'picture', # 'size': {'readable': '73.62KB'}}, # 'url': {'directDownload':
+'https://download1482.mediafire.com/h32ugeuxwitg/n2kcs3n9nd88vnr/picture.jpeg',
+# 'original': 'https://www.mediafire.com/file/n2kcs3n9nd88vnr/picture.jpeg/
+file'}}}, # 'status': 'true'} ``` Download the file `download=True` ```py from
+Direct_Download import Direct url = Direct() #Use download By Enabling download
+to True for downloading your file url.mediafire('https://www.mediafire.com/
+file/n2kcs3n9nd88vnr/picture.jpeg/file', download=True) ``` ## Links - [PyPI]
+(https://pypi.org/project/Direct-Download/) - [API](https://ddl-
+api.cycno.repl.co/) ## Contributors ### [CYCNO] Contributors are always
+welcome!
```

