# Comparing `tmp/rasa_gen-0.0.1.tar.gz` & `tmp/rasa_gen-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasa_gen-0.0.1.tar", last modified: Mon Apr 17 05:31:20 2023, max compression
+gzip compressed data, was "rasa_gen-0.0.2.tar", last modified: Wed Apr 19 03:47:44 2023, max compression
```

## Comparing `rasa_gen-0.0.1.tar` & `rasa_gen-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 05:31:20.811778 rasa_gen-0.0.1/
--rw-rw-rw-   0        0        0      310 2023-04-17 05:31:20.811778 rasa_gen-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-15 04:54:39.000000 rasa_gen-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 05:31:20.805273 rasa_gen-0.0.1/rasa_gen/
--rw-rw-rw-   0        0        0       26 2023-04-16 08:24:11.000000 rasa_gen-0.0.1/rasa_gen/__init__.py
--rw-rw-rw-   0        0        0     5678 2023-04-17 05:15:29.000000 rasa_gen-0.0.1/rasa_gen/generator.py
-drwxrwxrwx   0        0        0        0 2023-04-17 05:31:20.811778 rasa_gen-0.0.1/rasa_gen.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-17 05:31:20.000000 rasa_gen-0.0.1/rasa_gen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-04-17 05:31:20.000000 rasa_gen-0.0.1/rasa_gen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 05:31:20.000000 rasa_gen-0.0.1/rasa_gen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 05:31:20.000000 rasa_gen-0.0.1/rasa_gen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 05:31:20.811778 rasa_gen-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      492 2023-04-17 05:30:43.000000 rasa_gen-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 03:47:44.075417 rasa_gen-0.0.2/
+-rw-rw-rw-   0        0        0    11555 2023-04-17 09:11:03.000000 rasa_gen-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2531 2023-04-19 03:47:44.075001 rasa_gen-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-19 03:47:43.998123 rasa_gen-0.0.2/rasa_gen/
+-rw-rw-rw-   0        0        0       26 2023-04-16 08:24:11.000000 rasa_gen-0.0.2/rasa_gen/__init__.py
+-rw-rw-rw-   0        0        0    11297 2023-04-19 02:18:41.000000 rasa_gen-0.0.2/rasa_gen/generator.py
+drwxrwxrwx   0        0        0        0 2023-04-19 03:47:44.073522 rasa_gen-0.0.2/rasa_gen.egg-info/
+-rw-rw-rw-   0        0        0     2531 2023-04-19 03:47:43.000000 rasa_gen-0.0.2/rasa_gen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-04-19 03:47:43.000000 rasa_gen-0.0.2/rasa_gen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 03:47:43.000000 rasa_gen-0.0.2/rasa_gen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-19 03:47:43.000000 rasa_gen-0.0.2/rasa_gen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 03:47:43.000000 rasa_gen-0.0.2/rasa_gen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 03:47:44.075417 rasa_gen-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      673 2023-04-19 03:47:35.000000 rasa_gen-0.0.2/setup.py
```

