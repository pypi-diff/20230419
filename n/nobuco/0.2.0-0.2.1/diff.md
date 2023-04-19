# Comparing `tmp/nobuco-0.2.0.tar.gz` & `tmp/nobuco-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.2.0.tar", last modified: Tue Apr 18 18:55:19 2023, max compression
+gzip compressed data, was "nobuco-0.2.1.tar", last modified: Wed Apr 19 08:39:45 2023, max compression
```

## Comparing `nobuco-0.2.0.tar` & `nobuco-0.2.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.569498 nobuco-0.2.0/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.2.0/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)       14 2023-04-15 10:44:29.000000 nobuco-0.2.0/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)    18006 2023-04-18 18:55:19.569498 nobuco-0.2.0/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    16172 2023-04-18 12:28:26.000000 nobuco-0.2.0/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.565498 nobuco-0.2.0/docs/
--rw-rw-r--   0 alex      (1000) alex      (1000)    64876 2023-03-25 20:16:55.000000 nobuco-0.2.0/docs/channel_ordering.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    63145 2023-03-25 20:46:53.000000 nobuco-0.2.0/docs/channel_ordering_forced.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    67966 2023-04-18 11:28:12.000000 nobuco-0.2.0/docs/control_if.png
--rw-rw-r--   0 alex      (1000) alex      (1000)     2110 2023-04-05 14:55:45.000000 nobuco-0.2.0/docs/converter_inside_converter1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    26497 2023-04-05 19:25:33.000000 nobuco-0.2.0/docs/converter_inside_converter1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2319 2023-04-05 14:56:10.000000 nobuco-0.2.0/docs/converter_inside_converter2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    30325 2023-04-05 19:25:54.000000 nobuco-0.2.0/docs/converter_inside_converter2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     3070 2023-04-06 09:06:34.000000 nobuco-0.2.0/docs/essentials1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    35615 2023-04-06 09:06:58.000000 nobuco-0.2.0/docs/essentials1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2811 2023-04-05 14:47:00.000000 nobuco-0.2.0/docs/essentials2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    32971 2023-04-05 19:22:33.000000 nobuco-0.2.0/docs/essentials2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2281 2023-04-05 14:48:33.000000 nobuco-0.2.0/docs/essentials3.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    28090 2023-04-05 19:22:46.000000 nobuco-0.2.0/docs/essentials3.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1559 2023-04-05 14:51:28.000000 nobuco-0.2.0/docs/inplace1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    18606 2023-04-05 19:23:57.000000 nobuco-0.2.0/docs/inplace1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1050 2023-04-05 14:52:17.000000 nobuco-0.2.0/docs/inplace2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    11981 2023-04-05 19:24:22.000000 nobuco-0.2.0/docs/inplace2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-04-05 14:52:18.000000 nobuco-0.2.0/docs/inplace3.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    14409 2023-04-05 19:25:18.000000 nobuco-0.2.0/docs/inplace3.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     6859 2023-03-24 11:40:17.000000 nobuco-0.2.0/docs/inplace_empty.png
--rw-rw-r--   0 alex      (1000) alex      (1000)   926558 2023-04-16 10:49:50.000000 nobuco-0.2.0/docs/nobuco.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    82036 2023-03-03 12:08:40.000000 nobuco-0.2.0/docs/tutorial.png
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.565498 nobuco-0.2.0/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      461 2023-04-18 17:44:04.000000 nobuco-0.2.0/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      798 2023-03-07 13:07:06.000000 nobuco-0.2.0/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13121 2023-04-18 17:45:07.000000 nobuco-0.2.0/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.565498 nobuco-0.2.0/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.2.0/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-18 11:13:00.000000 nobuco-0.2.0/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2455 2023-04-18 11:52:51.000000 nobuco-0.2.0/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-18 18:43:24.000000 nobuco-0.2.0/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.2.0/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3497 2023-03-07 10:32:51.000000 nobuco-0.2.0/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.565498 nobuco-0.2.0/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.2.0/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3106 2023-04-18 10:12:58.000000 nobuco-0.2.0/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13309 2023-04-18 18:06:08.000000 nobuco-0.2.0/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1275 2023-04-18 18:43:04.000000 nobuco-0.2.0/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.569498 nobuco-0.2.0/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.2.0/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.2.0/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4886 2023-04-18 10:06:25.000000 nobuco-0.2.0/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.2.0/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-18 10:06:25.000000 nobuco-0.2.0/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.569498 nobuco-0.2.0/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-18 09:00:20.000000 nobuco-0.2.0/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4398 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4675 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9840 2023-04-18 17:59:47.000000 nobuco-0.2.0/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6822 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2863 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2568 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10232 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/tensor_manipulation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.569498 nobuco-0.2.0/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.2.0/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.2.0/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9670 2023-04-18 11:49:04.000000 nobuco-0.2.0/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-18 18:22:15.000000 nobuco-0.2.0/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.569498 nobuco-0.2.0/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.2.0/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1943 2023-04-18 10:12:57.000000 nobuco-0.2.0/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3167 2023-04-18 10:12:58.000000 nobuco-0.2.0/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.565498 nobuco-0.2.0/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    18006 2023-04-18 18:55:19.000000 nobuco-0.2.0/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     2055 2023-04-18 18:55:19.000000 nobuco-0.2.0/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-18 18:55:19.000000 nobuco-0.2.0/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-18 18:55:19.000000 nobuco-0.2.0/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-18 18:55:19.000000 nobuco-0.2.0/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-18 10:02:06.000000 nobuco-0.2.0/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-18 18:55:19.569498 nobuco-0.2.0/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.501697 nobuco-0.2.1/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.2.1/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)       14 2023-04-15 10:44:29.000000 nobuco-0.2.1/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)    18223 2023-04-19 08:39:45.501697 nobuco-0.2.1/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16389 2023-04-19 08:38:31.000000 nobuco-0.2.1/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.493697 nobuco-0.2.1/docs/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    64876 2023-03-25 20:16:55.000000 nobuco-0.2.1/docs/channel_ordering.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    63145 2023-03-25 20:46:53.000000 nobuco-0.2.1/docs/channel_ordering_forced.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    67966 2023-04-18 11:28:12.000000 nobuco-0.2.1/docs/control_if.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2110 2023-04-05 14:55:45.000000 nobuco-0.2.1/docs/converter_inside_converter1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    26497 2023-04-05 19:25:33.000000 nobuco-0.2.1/docs/converter_inside_converter1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2319 2023-04-05 14:56:10.000000 nobuco-0.2.1/docs/converter_inside_converter2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    30325 2023-04-05 19:25:54.000000 nobuco-0.2.1/docs/converter_inside_converter2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3070 2023-04-06 09:06:34.000000 nobuco-0.2.1/docs/essentials1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    35615 2023-04-06 09:06:58.000000 nobuco-0.2.1/docs/essentials1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2811 2023-04-05 14:47:00.000000 nobuco-0.2.1/docs/essentials2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    32971 2023-04-05 19:22:33.000000 nobuco-0.2.1/docs/essentials2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2281 2023-04-05 14:48:33.000000 nobuco-0.2.1/docs/essentials3.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    28090 2023-04-05 19:22:46.000000 nobuco-0.2.1/docs/essentials3.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1559 2023-04-05 14:51:28.000000 nobuco-0.2.1/docs/inplace1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    18606 2023-04-05 19:23:57.000000 nobuco-0.2.1/docs/inplace1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1050 2023-04-05 14:52:17.000000 nobuco-0.2.1/docs/inplace2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11981 2023-04-05 19:24:22.000000 nobuco-0.2.1/docs/inplace2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-04-05 14:52:18.000000 nobuco-0.2.1/docs/inplace3.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14409 2023-04-05 19:25:18.000000 nobuco-0.2.1/docs/inplace3.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6859 2023-03-24 11:40:17.000000 nobuco-0.2.1/docs/inplace_empty.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)   926558 2023-04-16 10:49:50.000000 nobuco-0.2.1/docs/nobuco.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    82036 2023-03-03 12:08:40.000000 nobuco-0.2.1/docs/tutorial.png
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.497697 nobuco-0.2.1/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      461 2023-04-18 17:44:04.000000 nobuco-0.2.1/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      798 2023-03-07 13:07:06.000000 nobuco-0.2.1/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13145 2023-04-19 08:35:20.000000 nobuco-0.2.1/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.497697 nobuco-0.2.1/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.2.1/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-18 11:13:00.000000 nobuco-0.2.1/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2455 2023-04-18 11:52:51.000000 nobuco-0.2.1/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-18 18:43:24.000000 nobuco-0.2.1/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.2.1/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3497 2023-03-07 10:32:51.000000 nobuco-0.2.1/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.497697 nobuco-0.2.1/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.2.1/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3106 2023-04-18 10:12:58.000000 nobuco-0.2.1/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13309 2023-04-18 18:06:08.000000 nobuco-0.2.1/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1275 2023-04-18 18:43:04.000000 nobuco-0.2.1/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.497697 nobuco-0.2.1/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.2.1/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.2.1/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4886 2023-04-18 10:06:25.000000 nobuco-0.2.1/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.2.1/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-18 10:06:25.000000 nobuco-0.2.1/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.501697 nobuco-0.2.1/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-18 09:00:20.000000 nobuco-0.2.1/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4398 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4675 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9840 2023-04-18 17:59:47.000000 nobuco-0.2.1/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6822 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3071 2023-04-19 08:28:44.000000 nobuco-0.2.1/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2568 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10232 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/tensor_manipulation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.501697 nobuco-0.2.1/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.2.1/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.2.1/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9670 2023-04-18 11:49:04.000000 nobuco-0.2.1/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-18 18:22:15.000000 nobuco-0.2.1/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.501697 nobuco-0.2.1/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.2.1/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1943 2023-04-18 10:12:57.000000 nobuco-0.2.1/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3167 2023-04-18 10:12:58.000000 nobuco-0.2.1/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.497697 nobuco-0.2.1/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    18223 2023-04-19 08:39:45.000000 nobuco-0.2.1/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2055 2023-04-19 08:39:45.000000 nobuco-0.2.1/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-19 08:39:45.000000 nobuco-0.2.1/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-19 08:39:45.000000 nobuco-0.2.1/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-19 08:39:45.000000 nobuco-0.2.1/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-19 08:39:27.000000 nobuco-0.2.1/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-19 08:39:45.501697 nobuco-0.2.1/setup.cfg
```

### Comparing `nobuco-0.2.0/LICENSE` & `nobuco-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/PKG-INFO` & `nobuco-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,14 +57,16 @@
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
+  - Control flows
+  - Dynamic shapes
 - [So we put a converter inside your converter](#so-we-put-a-converter-inside-your-converter)
 
 <!-- tocstop -->
 
 ## Essentials
 
 Suppose we want to convert a pytorch module similar to this one:
@@ -282,14 +284,15 @@
         return x
 ```
 
 <img src="docs/inplace3.svg" width="100%">
 
 ## Going dynamic
 
+### Control flows
 Introducing python control flow statements into the compute graph is no easy feat.
 Tensorflow can do so via `tf.autograph`, but at a cost of [system's complexity](https://www.youtube.com/watch?v=NIEgzljyDyI) and with some notable [limitations](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/python/autograph/g3doc/reference/control_flow.md).
 Stuff like that is way above Nobuco's paygrade, so the following module cannot be properly handled without human intervention.
 
 ```python
 class ControlIf(nn.Module):
     def __init__(self):
@@ -372,14 +375,17 @@
 
 <p align="center">
 <img src="docs/control_if.png" width="30%">
 </p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
+### Dynamic shapes
+:construction: See [examples/dynamic_shape](https://github.com/AlexanderLutsenko/nobuco/blob/master/examples/dynamic_shape.py) :construction:
+
 ## So we put a converter inside your converter
 
 One of the operations currently not supported is mask assign.
 There's no particular reason why, I just haven't done it yet (and your contribution is highly welcome!) 
 For now, let's use it as an excuse to explain the concept of nested converters.
 Like I said, for this module, conversion will fail:
```

### Comparing `nobuco-0.2.0/README.md` & `nobuco-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
+  - Control flows
+  - Dynamic shapes
 - [So we put a converter inside your converter](#so-we-put-a-converter-inside-your-converter)
 
 <!-- tocstop -->
 
 ## Essentials
 
 Suppose we want to convert a pytorch module similar to this one:
@@ -246,14 +248,15 @@
         return x
 ```
 
 <img src="docs/inplace3.svg" width="100%">
 
 ## Going dynamic
 
+### Control flows
 Introducing python control flow statements into the compute graph is no easy feat.
 Tensorflow can do so via `tf.autograph`, but at a cost of [system's complexity](https://www.youtube.com/watch?v=NIEgzljyDyI) and with some notable [limitations](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/python/autograph/g3doc/reference/control_flow.md).
 Stuff like that is way above Nobuco's paygrade, so the following module cannot be properly handled without human intervention.
 
 ```python
 class ControlIf(nn.Module):
     def __init__(self):
@@ -336,14 +339,17 @@
 
 <p align="center">
 <img src="docs/control_if.png" width="30%">
 </p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
+### Dynamic shapes
+:construction: See [examples/dynamic_shape](https://github.com/AlexanderLutsenko/nobuco/blob/master/examples/dynamic_shape.py) :construction:
+
 ## So we put a converter inside your converter
 
 One of the operations currently not supported is mask assign.
 There's no particular reason why, I just haven't done it yet (and your contribution is highly welcome!) 
 For now, let's use it as an excuse to explain the concept of nested converters.
 Like I said, for this module, conversion will fail:
```

### Comparing `nobuco-0.2.0/docs/channel_ordering.png` & `nobuco-0.2.1/docs/channel_ordering.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/channel_ordering_forced.png` & `nobuco-0.2.1/docs/channel_ordering_forced.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/control_if.png` & `nobuco-0.2.1/docs/control_if.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/converter_inside_converter1.html` & `nobuco-0.2.1/docs/converter_inside_converter1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/converter_inside_converter1.svg` & `nobuco-0.2.1/docs/converter_inside_converter1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/converter_inside_converter2.html` & `nobuco-0.2.1/docs/converter_inside_converter2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/converter_inside_converter2.svg` & `nobuco-0.2.1/docs/converter_inside_converter2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/essentials1.html` & `nobuco-0.2.1/docs/essentials1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/essentials1.svg` & `nobuco-0.2.1/docs/essentials1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/essentials2.html` & `nobuco-0.2.1/docs/essentials2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/essentials2.svg` & `nobuco-0.2.1/docs/essentials2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/essentials3.html` & `nobuco-0.2.1/docs/essentials3.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/essentials3.svg` & `nobuco-0.2.1/docs/essentials3.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/inplace1.html` & `nobuco-0.2.1/docs/inplace1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/inplace1.svg` & `nobuco-0.2.1/docs/inplace1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/inplace2.html` & `nobuco-0.2.1/docs/inplace2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/inplace2.svg` & `nobuco-0.2.1/docs/inplace2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/inplace3.html` & `nobuco-0.2.1/docs/inplace3.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/inplace3.svg` & `nobuco-0.2.1/docs/inplace3.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/inplace_empty.png` & `nobuco-0.2.1/docs/inplace_empty.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/nobuco.png` & `nobuco-0.2.1/docs/nobuco.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/docs/tutorial.png` & `nobuco-0.2.1/docs/tutorial.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/commons.py` & `nobuco-0.2.1/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/convert.py` & `nobuco-0.2.1/nobuco/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,16 @@
         if input_shapes is not None and obj in input_shapes:
             shape = input_shapes.get(obj)
             if channel_order == ChannelOrder.TENSORFLOW:
                 shape = permute_pytorch2keras(shape)
         else:
             shape = tens.shape
 
-        return set_channel_order(keras.Input(batch_shape=shape), channel_order)
+        print()
+        return set_channel_order(keras.backend.placeholder(shape=shape), channel_order)
 
     return replace_recursively_func(inputs_pt, collect_func, replace_func)
 
 
 def postprocess_outputs_tf(outputs, outputs_channel_order):
     processed = []
     outputs = collect_recursively(outputs, TF_TENSOR_CLASSES)
```

### Comparing `nobuco-0.2.0/nobuco/converters/channel_ordering.py` & `nobuco-0.2.1/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/converters/node_converter.py` & `nobuco-0.2.1/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/converters/tensor.py` & `nobuco-0.2.1/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/converters/type_cast.py` & `nobuco-0.2.1/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/converters/validation.py` & `nobuco-0.2.1/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/entity/keras.py` & `nobuco-0.2.1/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/entity/pytorch.py` & `nobuco-0.2.1/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/funcs.py` & `nobuco-0.2.1/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/layers/channel_order.py` & `nobuco-0.2.1/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/layers/container.py` & `nobuco-0.2.1/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/layers/weight.py` & `nobuco-0.2.1/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/activation.py` & `nobuco-0.2.1/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/boolean.py` & `nobuco-0.2.1/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/boolean_mask.py` & `nobuco-0.2.1/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/comparison.py` & `nobuco-0.2.1/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/convolution.py` & `nobuco-0.2.1/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/dropout.py` & `nobuco-0.2.1/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/interpolation.py` & `nobuco-0.2.1/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/linear.py` & `nobuco-0.2.1/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/math.py` & `nobuco-0.2.1/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/misc.py` & `nobuco-0.2.1/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/normalization.py` & `nobuco-0.2.1/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/padding.py` & `nobuco-0.2.1/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/pooling.py` & `nobuco-0.2.1/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/recurrent.py` & `nobuco-0.2.1/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/slice.py` & `nobuco-0.2.1/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/tensor_cast.py` & `nobuco-0.2.1/nobuco/node_converters/tensor_cast.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 
 
 @converter(torch.Tensor.type, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_type(self, dtype=None, non_blocking=False, **kwargs):
     return type_func
 
 
+@converter(torch.Tensor.float, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_type(self, memory_format=None):
+    return lambda x: type_func(x, dtype=torch.float32)
+
+
 @converter(torch.Tensor.to, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_to(self, device=None, dtype=None, non_blocking=False, copy=False, memory_format=torch.preserve_format):
     def func(self, device=None, dtype=None, non_blocking=False, copy=False, memory_format=torch.preserve_format):
         if dtype is not None:
             return type_func(self, dtype=dtype, non_blocking=non_blocking)
         elif isinstance(device, torch._C.dtype):
             return type_func(self, dtype=device, non_blocking=non_blocking)
```

### Comparing `nobuco-0.2.0/nobuco/node_converters/tensor_creation.py` & `nobuco-0.2.1/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.2.1/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/trace/tensor_storage.py` & `nobuco-0.2.1/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/trace/trace.py` & `nobuco-0.2.1/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/util.py` & `nobuco-0.2.1/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/vis/console_stylizer.py` & `nobuco-0.2.1/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco/vis/html_stylizer.py` & `nobuco-0.2.1/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/nobuco.egg-info/PKG-INFO` & `nobuco-0.2.1/nobuco.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,14 +57,16 @@
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
+  - Control flows
+  - Dynamic shapes
 - [So we put a converter inside your converter](#so-we-put-a-converter-inside-your-converter)
 
 <!-- tocstop -->
 
 ## Essentials
 
 Suppose we want to convert a pytorch module similar to this one:
@@ -282,14 +284,15 @@
         return x
 ```
 
 <img src="docs/inplace3.svg" width="100%">
 
 ## Going dynamic
 
+### Control flows
 Introducing python control flow statements into the compute graph is no easy feat.
 Tensorflow can do so via `tf.autograph`, but at a cost of [system's complexity](https://www.youtube.com/watch?v=NIEgzljyDyI) and with some notable [limitations](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/python/autograph/g3doc/reference/control_flow.md).
 Stuff like that is way above Nobuco's paygrade, so the following module cannot be properly handled without human intervention.
 
 ```python
 class ControlIf(nn.Module):
     def __init__(self):
@@ -372,14 +375,17 @@
 
 <p align="center">
 <img src="docs/control_if.png" width="30%">
 </p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
+### Dynamic shapes
+:construction: See [examples/dynamic_shape](https://github.com/AlexanderLutsenko/nobuco/blob/master/examples/dynamic_shape.py) :construction:
+
 ## So we put a converter inside your converter
 
 One of the operations currently not supported is mask assign.
 There's no particular reason why, I just haven't done it yet (and your contribution is highly welcome!) 
 For now, let's use it as an excuse to explain the concept of nested converters.
 Like I said, for this module, conversion will fail:
```

### Comparing `nobuco-0.2.0/nobuco.egg-info/SOURCES.txt` & `nobuco-0.2.1/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.0/pyproject.toml` & `nobuco-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.2.0"
+version = "0.2.1"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

