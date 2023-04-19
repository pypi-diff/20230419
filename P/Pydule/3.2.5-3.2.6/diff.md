# Comparing `tmp/Pydule-3.2.5.tar.gz` & `tmp/Pydule-3.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pydule-3.2.5.tar", last modified: Mon Apr 10 14:42:46 2023, max compression
+gzip compressed data, was "Pydule-3.2.6.tar", last modified: Wed Apr 19 15:44:11 2023, max compression
```

## Comparing `Pydule-3.2.5.tar` & `Pydule-3.2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:46.017458 Pydule-3.2.5/
--rw-rw-rw-   0        0        0     2013 2023-04-10 14:42:46.017458 Pydule-3.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1235 2023-04-10 14:40:07.000000 Pydule-3.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 14:42:46.017458 Pydule-3.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1280 2023-04-10 14:39:29.000000 Pydule-3.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:45.688574 Pydule-3.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:46.008915 Pydule-3.2.5/src/Pydule.egg-info/
--rw-rw-rw-   0        0        0     2013 2023-04-10 14:42:45.000000 Pydule-3.2.5/src/Pydule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-04-10 14:42:45.000000 Pydule-3.2.5/src/Pydule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 14:42:45.000000 Pydule-3.2.5/src/Pydule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-04-10 14:42:45.000000 Pydule-3.2.5/src/Pydule.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-10 14:42:45.000000 Pydule-3.2.5/src/Pydule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7606 2023-04-10 01:54:45.000000 Pydule-3.2.5/src/Pydule.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:44:11.014132 Pydule-3.2.6/
+-rw-rw-rw-   0        0        0     2082 2023-04-19 15:44:11.003513 Pydule-3.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1294 2023-04-19 15:42:06.000000 Pydule-3.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 15:44:11.014132 Pydule-3.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-04-19 15:40:36.000000 Pydule-3.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:44:10.733695 Pydule-3.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 15:44:10.994959 Pydule-3.2.6/src/Pydule.egg-info/
+-rw-rw-rw-   0        0        0     2082 2023-04-19 15:44:09.000000 Pydule-3.2.6/src/Pydule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-04-19 15:44:09.000000 Pydule-3.2.6/src/Pydule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 15:44:09.000000 Pydule-3.2.6/src/Pydule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-04-19 15:44:09.000000 Pydule-3.2.6/src/Pydule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 15:44:09.000000 Pydule-3.2.6/src/Pydule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7999 2023-04-19 15:35:42.000000 Pydule-3.2.6/src/Pydule.py
```

### Comparing `Pydule-3.2.5/PKG-INFO` & `Pydule-3.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.2.5
-Summary: Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Translate a Sentence to Other Language and more..
+Version: 3.2.6
+Summary: Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,15 @@
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
 - Download Mp3 or Mp4 From Youtube
 - Insert Elements in Tuple & String
 - Generate Qrcode
+- Copy Text
 - Text Translation
 - Edit JSON Files
 - Replace Letters in String
 - Replace Elements in List and Tuple
 - Check Weather of any City
 - Open any File
 - Play Songs
@@ -56,13 +57,16 @@
 
 # to Get all Available Functions
 py.functions() 
 
 # to Open Calculator
 py.openapp('calculator')
 
+# to Copy Text
+py.copytext('Hello World')
+
 # to Download Youtube Audio
 py.ytmp3('YOUR LINK HERE')
 
 # to Download Youtube Video with Audio
 py.ytmp4('YOUR LINK HERE')
   ```
```

### Comparing `Pydule-3.2.5/README.md` & `Pydule-3.2.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
 - Download Mp3 or Mp4 From Youtube
 - Insert Elements in Tuple & String
 - Generate Qrcode
+- Copy Text
 - Text Translation
 - Edit JSON Files
 - Replace Letters in String
 - Replace Elements in List and Tuple
 - Check Weather of any City
 - Open any File
 - Play Songs
@@ -42,13 +43,16 @@
 
 # to Get all Available Functions
 py.functions() 
 
 # to Open Calculator
 py.openapp('calculator')
 
+# to Copy Text
+py.copytext('Hello World')
+
 # to Download Youtube Audio
 py.ytmp3('YOUR LINK HERE')
 
 # to Download Youtube Video with Audio
 py.ytmp4('YOUR LINK HERE')
   ```
```

### Comparing `Pydule-3.2.5/setup.py` & `Pydule-3.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import setuptools
 
 with open('README.md','r') as fh:
 	long_description = fh.read()
 
 setup(
 	name='Pydule',
-	version='3.2.5',
-	description="Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Translate a Sentence to Other Language and more..",
+	version='3.2.6',
+	description="Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..",
 	author='D.Tamil Mutharasan',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	packages=setuptools.find_packages(),
 	keywords=['python','PyDule','Module','Pydule','pydule','matrix','qrcode','youtube','weather','list','tuple','set','dictionary','clear','color','pick_color','open','app','search','play','mp3','song','restart','system','shutdown','date','time','text_to_speech','text','speech'],
 	classifiers=[
 		"Programming Language :: Python :: 3",
@@ -30,11 +30,12 @@
 		'playsound',
 		'datetime',
 		'requests',
 		'AppOpener',
 		'deep_translator',
 		'qrcode',
 		'pytube',
-		'numpy'
+		'numpy',
+		'pyperclip'
 	]
 
 )
```

### Comparing `Pydule-3.2.5/src/Pydule.egg-info/PKG-INFO` & `Pydule-3.2.6/src/Pydule.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.2.5
-Summary: Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Translate a Sentence to Other Language and more..
+Version: 3.2.6
+Summary: Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,15 @@
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
 - Download Mp3 or Mp4 From Youtube
 - Insert Elements in Tuple & String
 - Generate Qrcode
+- Copy Text
 - Text Translation
 - Edit JSON Files
 - Replace Letters in String
 - Replace Elements in List and Tuple
 - Check Weather of any City
 - Open any File
 - Play Songs
@@ -56,13 +57,16 @@
 
 # to Get all Available Functions
 py.functions() 
 
 # to Open Calculator
 py.openapp('calculator')
 
+# to Copy Text
+py.copytext('Hello World')
+
 # to Download Youtube Audio
 py.ytmp3('YOUR LINK HERE')
 
 # to Download Youtube Video with Audio
 py.ytmp4('YOUR LINK HERE')
   ```
```

### Comparing `Pydule-3.2.5/src/Pydule.py` & `Pydule-3.2.6/src/Pydule.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import datetime
 import os
+import tkinter as tk
 import pyttsx3 
 import playsound as ps
 from playsound import playsound
 from tkinter import *
 from tkinter import colorchooser
 
 engine = pyttsx3.init() 
 
 err='\n \U0000274C Something Went Wrong \U0000274C\n'
 
 def openapp(appname):
 	from AppOpener import open
 	open(appname)
 
+def wjson(data,path):
+	import json
+	with open(path,'w') as json_file:
+		json.dump(data,json_file)
+
 def deljsonele(path):
 	import json
 	jsonfile=json.load(open(path))
 	copy=jsonfile.copy()
 	k=eval(input('Enter the Key : '))
 	del copy[k]
 	with open(path,'w') as json_file:
 		json.dump(copy,json_file)	
 
-def rejson(path):
+def upjson(path):
 	import json
 	jsonfile=json.load(open(path))
 	copy=jsonfile.copy()
 	k=eval(input('Enter the Key : '))
 	v=eval(input('Enter the Value : '))
 	copy[k]=v
 	with open(path,'w') as json_file:
@@ -73,18 +79,18 @@
 				else:
 					new+=j
 		return new
 	else:
 		print(err)			
 
 def functions():
-	l=['deljsonele(<path>)','rejson(<path>)','translate(<sentence>,<language>)','ytmp4(<youtube_link>)','ytmp3(<youtube_link>)','cqrcode(<link>)','summatrix(<matrix a>,<matrix b>)','submatrix(<matrix a>,<matrix b>)','intuple(<tuple>,<index>,<new_element>)','instr(<str>,<index>,<new_element>)','reSet(<old_set>,<new_element>,<old_element>)','reStr(<old_str>,<index>,<new_str>)','reDict(<old_dict>,<old_key>,<new_key>)','reList(<old_list>,<index>,<new_element>)','reTuple(<old_tuple>,<index>,<new_element>)','clist(<length_of_the_list>)','ctuple(<length_of_the_tuple>)','cdict(<length_of_the_dict>)','cset(<length_of_the_set>)','pickcolor()','search(<content>)','playsong(<path>)','restart_system()','shutdown_system()','datetoday()','timenow()','say(<content>)','openfile(<path>)','weathernow(<city_name>)','setvoice(<number_between 0 to 2>)','voicerate(<any_number>)']
-	print('Available Functions : ')
+	l=['wjson(<dict>,<path>)','deljsonele(<path>)','upjson(<path>)','copytext(<text_to_copy>)','translate(<sentence>,<language>)','ytmp4(<youtube_link>)','ytmp3(<youtube_link>)','cqrcode(<link>)','summatrix(<matrix a>,<matrix b>)','submatrix(<matrix a>,<matrix b>)','intuple(<tuple>,<index>,<new_element>)','instr(<str>,<index>,<new_element>)','reSet(<old_set>,<new_element>,<old_element>)','reStr(<old_str>,<index>,<new_str>)','reDict(<old_dict>,<old_key>,<new_key>)','reList(<old_list>,<index>,<new_element>)','reTuple(<old_tuple>,<index>,<new_element>)','clist(<length_of_the_list>)','ctuple(<length_of_the_tuple>)','cdict(<length_of_the_dict>)','cset(<length_of_the_set>)','pickcolor()','search(<content>)','playsong(<path>)','restart_system()','shutdown_system()','datetoday()','timenow()','say(<content>)','openfile(<path>)','weathernow(<city_name>)','setvoice(<number_between 0 to 2>)','voicerate(<any_number>)']
+	print('Available Functions : \n')
 	for i in l:
-		print(i)
+		print(f'\t{i}')
 
 def summatrix(x,y):
 	import numpy as np
 	result = np.array(x) + np.array(y)
 	return result
 
 def submatrix(x,y):
@@ -217,22 +223,28 @@
 	print('Enter Values One by One \U0001F447\n')
 	for i in range(mx):
 		s=eval(input(f'Enter {num(i+1)} Values : '))
 		Set.add(s)
 	print('\nSet Created Successfully \U00002714')	
 	return Set
 
+def copytext(string):
+	import pyperclip
+	pyperclip.copy(string)
+	spam=pyperclip.paste()
+
 def pickcolor():
-	root=Tk()
+	root=tk.Tk()
 	root.geometry('250x100')
 	root.title('Color Picker')
 	def n():
-		c=colorchooser.askcolor(title='CP')
-		print(c)
-	b=Button(root,text='Pick Color',command=n).pack()
+		c=colorchooser.askcolor(title='Pydule Color Picker \U00002714')
+		copytext('\''+str(c[-1])+'\'')
+		print(f'Choosen Color ({c[-1]}) is Copied \U00002714')
+	b=tk.Button(root,text='Pick Color',command=n).pack()
 	root.mainloop()				
 	
 def search(content):
 	import pywhatkit as kt
 	kt.search(content)	
 	print('\nSearching \U0001F50E...\n')
```

