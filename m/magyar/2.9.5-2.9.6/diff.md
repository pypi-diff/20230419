# Comparing `tmp/magyar-2.9.5.tar.gz` & `tmp/magyar-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-2.9.5.tar", last modified: Mon Apr 17 21:35:19 2023, max compression
+gzip compressed data, was "magyar-2.9.6.tar", last modified: Wed Apr 19 15:07:36 2023, max compression
```

## Comparing `magyar-2.9.5.tar` & `magyar-2.9.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-17 21:35:19.640199 magyar-2.9.5/
--rw-rw-r--   0 bela      (1000) bela      (1000)     3884 2023-04-17 21:35:19.640199 magyar-2.9.5/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     3513 2023-04-17 21:33:22.000000 magyar-2.9.5/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-17 21:35:19.640199 magyar-2.9.5/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     3884 2023-04-17 21:35:19.000000 magyar-2.9.5/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-17 21:35:19.000000 magyar-2.9.5/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-17 21:35:19.000000 magyar-2.9.5/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-17 21:35:19.000000 magyar-2.9.5/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    31836 2023-04-17 21:33:22.000000 magyar-2.9.5/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-17 21:35:19.640199 magyar-2.9.5/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-17 21:33:22.000000 magyar-2.9.5/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-19 15:07:36.954181 magyar-2.9.6/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     3912 2023-04-19 15:07:36.954181 magyar-2.9.6/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     3541 2023-04-19 15:02:33.000000 magyar-2.9.6/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-19 15:07:36.954181 magyar-2.9.6/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     3912 2023-04-19 15:07:36.000000 magyar-2.9.6/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-19 15:07:36.000000 magyar-2.9.6/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-19 15:07:36.000000 magyar-2.9.6/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-19 15:07:36.000000 magyar-2.9.6/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    31836 2023-04-19 15:02:33.000000 magyar-2.9.6/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-19 15:07:36.954181 magyar-2.9.6/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-19 15:05:49.000000 magyar-2.9.6/setup.py
```

### Comparing `magyar-2.9.5/PKG-INFO` & `magyar-2.9.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.9.5
+Version: 2.9.6
 Summary: Hungarian names...
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -86,18 +86,18 @@
     magyar.villamos:    kulcs  {'viszonylat', indulas, erkezes, menetido, varos}
     magyar.orszag:             {'orszag': 'főváros'}
 
 ## Metódus
    A  szótárakból választhatsz véletlenszerű KULCSOT. (szótár neve, elemek száma)
                     
     szotarbol_veletlen_kulcs(szotar, n)
-Pl:
-    import magyar
-    print(magyar.szotarbol_veletlen_kulcs(magyar.jaras,15))
-Eredmény:
+Pl: </br>
+    import magyar</br>
+    print(magyar.szotarbol_veletlen_kulcs(magyar.jaras,15)) </br></br>
+Eredmény: </br>
     ['Szekszárdi járás', 'Gönci járás', 'Szigetvári járás', 'Mezőkovácsházi járás', 'Bátonyterenyei járás',
     'Körmendi járás', 'Váci járás', 'Edelényi járás', 'Pilisvörösvári járás', 'Kaposvári járás', 'Hódmezővásárhelyi járás',
     'Hatvani járás', 'Törökszentmiklósi járás', 'Putnoki járás', 'Mezőkövesdi járás']
 
 
 ## Szerző
```

### Comparing `magyar-2.9.5/README.md` & `magyar-2.9.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,18 +74,18 @@
     magyar.villamos:    kulcs  {'viszonylat', indulas, erkezes, menetido, varos}
     magyar.orszag:             {'orszag': 'főváros'}
 
 ## Metódus
    A  szótárakból választhatsz véletlenszerű KULCSOT. (szótár neve, elemek száma)
                     
     szotarbol_veletlen_kulcs(szotar, n)
-Pl:
-    import magyar
-    print(magyar.szotarbol_veletlen_kulcs(magyar.jaras,15))
-Eredmény:
+Pl: </br>
+    import magyar</br>
+    print(magyar.szotarbol_veletlen_kulcs(magyar.jaras,15)) </br></br>
+Eredmény: </br>
     ['Szekszárdi járás', 'Gönci járás', 'Szigetvári járás', 'Mezőkovácsházi járás', 'Bátonyterenyei járás',
     'Körmendi járás', 'Váci járás', 'Edelényi járás', 'Pilisvörösvári járás', 'Kaposvári járás', 'Hódmezővásárhelyi járás',
     'Hatvani járás', 'Törökszentmiklósi járás', 'Putnoki járás', 'Mezőkövesdi járás']
 
 
 ## Szerző
```

### Comparing `magyar-2.9.5/magyar.egg-info/PKG-INFO` & `magyar-2.9.6/magyar.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.9.5
+Version: 2.9.6
 Summary: Hungarian names...
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -86,18 +86,18 @@
     magyar.villamos:    kulcs  {'viszonylat', indulas, erkezes, menetido, varos}
     magyar.orszag:             {'orszag': 'főváros'}
 
 ## Metódus
    A  szótárakból választhatsz véletlenszerű KULCSOT. (szótár neve, elemek száma)
                     
     szotarbol_veletlen_kulcs(szotar, n)
-Pl:
-    import magyar
-    print(magyar.szotarbol_veletlen_kulcs(magyar.jaras,15))
-Eredmény:
+Pl: </br>
+    import magyar</br>
+    print(magyar.szotarbol_veletlen_kulcs(magyar.jaras,15)) </br></br>
+Eredmény: </br>
     ['Szekszárdi járás', 'Gönci járás', 'Szigetvári járás', 'Mezőkovácsházi járás', 'Bátonyterenyei járás',
     'Körmendi járás', 'Váci járás', 'Edelényi járás', 'Pilisvörösvári járás', 'Kaposvári járás', 'Hódmezővásárhelyi járás',
     'Hatvani járás', 'Törökszentmiklósi járás', 'Putnoki járás', 'Mezőkövesdi járás']
 
 
 ## Szerző
```

### Comparing `magyar-2.9.5/magyar.py` & `magyar-2.9.6/magyar.py`

 * *Files identical despite different names*

### Comparing `magyar-2.9.5/setup.py` & `magyar-2.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="2.9.5",
+    version="2.9.6",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian names...",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

