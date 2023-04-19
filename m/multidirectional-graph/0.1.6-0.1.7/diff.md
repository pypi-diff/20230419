# Comparing `tmp/multidirectional_graph-0.1.6.tar.gz` & `tmp/multidirectional_graph-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidirectional_graph-0.1.6.tar", last modified: Tue Apr  4 15:44:17 2023, max compression
+gzip compressed data, was "multidirectional_graph-0.1.7.tar", last modified: Wed Apr 19 01:24:37 2023, max compression
```

## Comparing `multidirectional_graph-0.1.6.tar` & `multidirectional_graph-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-04 15:44:17.883863 multidirectional_graph-0.1.6/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      142 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/MANIFEST.in
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1940 2023-04-04 15:44:17.883863 multidirectional_graph-0.1.6/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1709 2023-04-04 15:43:43.000000 multidirectional_graph-0.1.6/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-04 15:44:17.855859 multidirectional_graph-0.1.6/multidirectional_graph/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      107 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    20320 2023-04-04 15:42:10.000000 multidirectional_graph-0.1.6/multidirectional_graph/_graph.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-04 15:44:17.855859 multidirectional_graph-0.1.6/multidirectional_graph/fonts/
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-04 15:44:17.859860 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    64184 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/Oswald-Bold.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    63872 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/Oswald-ExtraLight.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    64004 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/Oswald-Light.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    64184 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/Oswald-Medium.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    63900 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/Oswald-Regular.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    64220 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/Oswald-SemiBold.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   126336 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/Oswald-VariableFont_wght.ttf
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-04 15:44:17.871861 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11560 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/LICENSE.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   168060 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-Black.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   174108 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   167336 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-Bold.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   171508 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   170504 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-Italic.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   167000 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-Light.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   173172 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-LightItalic.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   168644 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-Medium.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   173416 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   168260 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-Regular.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   168488 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-Thin.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   172860 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-ThinItalic.ttf
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-04 15:44:17.883863 multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   228736 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Black.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   169668 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-BlackItalic.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   229816 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Bold.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   172748 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-BoldItalic.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   223796 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-ExtraLight.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   168132 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-ExtraLightItalic.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   169568 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Italic.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   227844 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Light.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   171544 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-LightItalic.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   226888 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Regular.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   229672 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-SemiBold.ttf
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   172816 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-SemiBoldItalic.ttf
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-04 15:44:17.855859 multidirectional_graph-0.1.6/multidirectional_graph.egg-info/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1940 2023-04-04 15:44:17.000000 multidirectional_graph-0.1.6/multidirectional_graph.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2274 2023-04-04 15:44:17.000000 multidirectional_graph-0.1.6/multidirectional_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-04 15:44:17.000000 multidirectional_graph-0.1.6/multidirectional_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       11 2023-04-04 15:44:17.000000 multidirectional_graph-0.1.6/multidirectional_graph.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       23 2023-04-04 15:44:17.000000 multidirectional_graph-0.1.6/multidirectional_graph.egg-info/top_level.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-04 15:44:17.883863 multidirectional_graph-0.1.6/setup.cfg
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1007 2023-04-04 15:44:06.000000 multidirectional_graph-0.1.6/setup.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-19 01:24:37.934926 multidirectional_graph-0.1.7/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      142 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/MANIFEST.in
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1940 2023-04-19 01:24:37.934926 multidirectional_graph-0.1.7/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1709 2023-04-04 15:43:43.000000 multidirectional_graph-0.1.7/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-19 01:24:37.922926 multidirectional_graph-0.1.7/multidirectional_graph/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      107 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    20288 2023-04-19 01:21:58.000000 multidirectional_graph-0.1.7/multidirectional_graph/_graph.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-19 01:24:37.922926 multidirectional_graph-0.1.7/multidirectional_graph/fonts/
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-19 01:24:37.922926 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    64184 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/Oswald-Bold.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    63872 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/Oswald-ExtraLight.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    64004 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/Oswald-Light.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    64184 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/Oswald-Medium.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    63900 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/Oswald-Regular.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    64220 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/Oswald-SemiBold.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   126336 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/Oswald-VariableFont_wght.ttf
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-19 01:24:37.930926 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11560 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/LICENSE.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   168060 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-Black.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   174108 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   167336 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-Bold.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   171508 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   170504 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-Italic.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   167000 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-Light.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   173172 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   168644 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-Medium.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   173416 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   168260 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-Regular.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   168488 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-Thin.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   172860 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-ThinItalic.ttf
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-19 01:24:37.934926 multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   228736 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Black.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   169668 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-BlackItalic.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   229816 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Bold.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   172748 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-BoldItalic.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   223796 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-ExtraLight.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   168132 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-ExtraLightItalic.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   169568 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Italic.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   227844 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Light.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   171544 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-LightItalic.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   226888 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Regular.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   229672 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-SemiBold.ttf
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)   172816 2023-04-03 23:57:24.000000 multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-SemiBoldItalic.ttf
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-19 01:24:37.922926 multidirectional_graph-0.1.7/multidirectional_graph.egg-info/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1940 2023-04-19 01:24:37.000000 multidirectional_graph-0.1.7/multidirectional_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2274 2023-04-19 01:24:37.000000 multidirectional_graph-0.1.7/multidirectional_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-19 01:24:37.000000 multidirectional_graph-0.1.7/multidirectional_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       11 2023-04-19 01:24:37.000000 multidirectional_graph-0.1.7/multidirectional_graph.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       23 2023-04-19 01:24:37.000000 multidirectional_graph-0.1.7/multidirectional_graph.egg-info/top_level.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-19 01:24:37.934926 multidirectional_graph-0.1.7/setup.cfg
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1007 2023-04-19 01:20:52.000000 multidirectional_graph-0.1.7/setup.py
```

### Comparing `multidirectional_graph-0.1.6/PKG-INFO` & `multidirectional_graph-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidirectional_graph
-Version: 0.1.6
+Version: 0.1.7
 Summary: Package for plotting multidirectional graphs
 Author: Eduardo Messias de Morais
 Author-email: emdemor415@gmail.com
 Description-Content-Type: text/markdown
 
 # Multidirectional Graph
```

### Comparing `multidirectional_graph-0.1.6/README.md` & `multidirectional_graph-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/_graph.py` & `multidirectional_graph-0.1.7/multidirectional_graph/_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
             lambda x, y: x + y, [list(self.data[d].values()) for d in self.data]
         )
 
     def _get_group_sizes(self):
         return {d: len(self.data[d]) for d in self.data}
 
     def _set_title(self):
-        self.title = f"AVALIAÇÃO MULTIDIRECIONAL DE\n{self.tipo_avaliacao}".upper()
+        self.title = f"{self.tipo_avaliacao}".upper()
 
     def _add_title(self, ax):
         self._set_title()
 
         skills_width = self.category_width + self.group_width
         left_plot = self.min_x-skills_width
```

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/Oswald-Bold.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/Oswald-Bold.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/Oswald-ExtraLight.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/Oswald-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/Oswald-Light.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/Oswald-Light.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/Oswald-Medium.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/Oswald-Medium.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/Oswald-Regular.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/Oswald-Regular.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/Oswald-SemiBold.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/Oswald-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Oswald/Oswald-VariableFont_wght.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Oswald/Oswald-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/LICENSE.txt` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-Black.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-BlackItalic.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-Bold.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-BoldItalic.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-Italic.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-Light.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-LightItalic.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-Medium.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-MediumItalic.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-Regular.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-Thin.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/Roboto/Roboto-ThinItalic.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Black.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Black.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-BlackItalic.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Bold.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-BoldItalic.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-ExtraLight.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-ExtraLightItalic.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Italic.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Light.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Light.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-LightItalic.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Regular.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-SemiBold.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-SemiBoldItalic.ttf` & `multidirectional_graph-0.1.7/multidirectional_graph/fonts/SourceSerif/SourceSerifPro-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph.egg-info/PKG-INFO` & `multidirectional_graph-0.1.7/multidirectional_graph.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidirectional-graph
-Version: 0.1.6
+Version: 0.1.7
 Summary: Package for plotting multidirectional graphs
 Author: Eduardo Messias de Morais
 Author-email: emdemor415@gmail.com
 Description-Content-Type: text/markdown
 
 # Multidirectional Graph
```

### Comparing `multidirectional_graph-0.1.6/multidirectional_graph.egg-info/SOURCES.txt` & `multidirectional_graph-0.1.7/multidirectional_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multidirectional_graph-0.1.6/setup.py` & `multidirectional_graph-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 
 setup(
     name="multidirectional_graph",
-    version="0.1.6",
+    version="0.1.7",
     description="Package for plotting multidirectional graphs",
     author="Eduardo Messias de Morais",
     author_email="emdemor415@gmail.com",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=["multidirectional_graph"],
     package_data={
```

