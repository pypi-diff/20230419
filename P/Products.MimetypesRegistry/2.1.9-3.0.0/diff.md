# Comparing `tmp/Products.MimetypesRegistry-2.1.9.tar.gz` & `tmp/Products.MimetypesRegistry-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.MimetypesRegistry-2.1.9.tar", last modified: Wed Jan 19 14:32:27 2022, max compression
+gzip compressed data, was "Products.MimetypesRegistry-3.0.0.tar", last modified: Wed Apr 19 07:20:14 2023, max compression
```

## Comparing `Products.MimetypesRegistry-2.1.9.tar` & `Products.MimetypesRegistry-3.0.0.tar`

### file list

```diff
@@ -1,126 +1,129 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:32:27.295136 Products.MimetypesRegistry-2.1.9/
--rw-r--r--   0 maurits    (501) staff       (20)      149 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)    13046 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      250 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    15340 2022-01-19 14:32:27.295292 Products.MimetypesRegistry-2.1.9/PKG-INFO
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:32:27.264474 Products.MimetypesRegistry-2.1.9/Products/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:32:27.269272 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/
--rw-r--r--   0 maurits    (501) staff       (20)     4060 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/MimeTypeItem.py
--rw-r--r--   0 maurits    (501) staff       (20)    16437 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/MimeTypesRegistry.py
--rw-r--r--   0 maurits    (501) staff       (20)      612 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      331 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/common.py
--rw-r--r--   0 maurits    (501) staff       (20)      647 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2357 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/encoding.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:32:27.284709 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/
--rw-r--r--   0 maurits    (501) staff       (20)      331 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/application.png
--rw-r--r--   0 maurits    (501) staff       (20)      681 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/audio.png
--rw-r--r--   0 maurits    (501) staff       (20)      350 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/avi.png
--rw-r--r--   0 maurits    (501) staff       (20)      445 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/c.png
--rw-r--r--   0 maurits    (501) staff       (20)      640 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/core.png
--rw-r--r--   0 maurits    (501) staff       (20)      421 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/cpp.png
--rw-r--r--   0 maurits    (501) staff       (20)      469 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/deb.png
--rw-r--r--   0 maurits    (501) staff       (20)      761 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/doc.png
--rw-r--r--   0 maurits    (501) staff       (20)      761 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/docx.png
--rw-r--r--   0 maurits    (501) staff       (20)      572 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/down.png
--rw-r--r--   0 maurits    (501) staff       (20)      700 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/dvi.png
--rw-r--r--   0 maurits    (501) staff       (20)      331 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/exe.png
--rw-r--r--   0 maurits    (501) staff       (20)      420 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/f.png
--rw-r--r--   0 maurits    (501) staff       (20)      550 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/font.png
--rw-r--r--   0 maurits    (501) staff       (20)      252 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/gf.png
--rw-r--r--   0 maurits    (501) staff       (20)      417 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/h.png
--rw-r--r--   0 maurits    (501) staff       (20)      599 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/html.png
--rw-r--r--   0 maurits    (501) staff       (20)      330 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/image.png
--rw-r--r--   0 maurits    (501) staff       (20)      662 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/info.png
--rw-r--r--   0 maurits    (501) staff       (20)      711 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/iso.png
--rw-r--r--   0 maurits    (501) staff       (20)      573 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/java.png
--rw-r--r--   0 maurits    (501) staff       (20)      668 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/log.png
--rw-r--r--   0 maurits    (501) staff       (20)      613 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/man.png
--rw-r--r--   0 maurits    (501) staff       (20)      355 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/message.png
--rw-r--r--   0 maurits    (501) staff       (20)      681 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/midi.png
--rw-r--r--   0 maurits    (501) staff       (20)      331 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/mime.png
--rw-r--r--   0 maurits    (501) staff       (20)      420 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/o.png
--rw-r--r--   0 maurits    (501) staff       (20)      513 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/pdf.png
--rw-r--r--   0 maurits    (501) staff       (20)      272 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/pk.png
--rw-r--r--   0 maurits    (501) staff       (20)      422 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/pl.png
--rw-r--r--   0 maurits    (501) staff       (20)      330 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/png.png
--rw-r--r--   0 maurits    (501) staff       (20)      413 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/ppt.png
--rw-r--r--   0 maurits    (501) staff       (20)      413 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/pptx.png
--rw-r--r--   0 maurits    (501) staff       (20)      638 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/ps.png
--rw-r--r--   0 maurits    (501) staff       (20)      641 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/py.png
--rw-r--r--   0 maurits    (501) staff       (20)      350 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/quicktime.png
--rw-r--r--   0 maurits    (501) staff       (20)      469 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/rar.png
--rw-r--r--   0 maurits    (501) staff       (20)      469 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/rpm.png
--rw-r--r--   0 maurits    (501) staff       (20)      722 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/sh.png
--rw-r--r--   0 maurits    (501) staff       (20)      869 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/sxc.png
--rw-r--r--   0 maurits    (501) staff       (20)      897 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/sxd.png
--rw-r--r--   0 maurits    (501) staff       (20)      861 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/sxg.png
--rw-r--r--   0 maurits    (501) staff       (20)      844 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/sxi.png
--rw-r--r--   0 maurits    (501) staff       (20)      888 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/sxm.png
--rw-r--r--   0 maurits    (501) staff       (20)      861 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/sxw.png
--rw-r--r--   0 maurits    (501) staff       (20)      469 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/tar.png
--rw-r--r--   0 maurits    (501) staff       (20)      349 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/tex.png
--rw-r--r--   0 maurits    (501) staff       (20)      249 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/text.png
--rw-r--r--   0 maurits    (501) staff       (20)      662 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/tgz.png
--rw-r--r--   0 maurits    (501) staff       (20)      249 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/txt.png
--rw-r--r--   0 maurits    (501) staff       (20)      295 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/unknown.png
--rw-r--r--   0 maurits    (501) staff       (20)      591 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/up.png
--rw-r--r--   0 maurits    (501) staff       (20)      453 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/vcal.png
--rw-r--r--   0 maurits    (501) staff       (20)      564 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/vcard.png
--rw-r--r--   0 maurits    (501) staff       (20)      350 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/video.png
--rw-r--r--   0 maurits    (501) staff       (20)      681 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/wav.png
--rw-r--r--   0 maurits    (501) staff       (20)      622 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/xls.png
--rw-r--r--   0 maurits    (501) staff       (20)      622 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/xlsx.png
--rw-r--r--   0 maurits    (501) staff       (20)      469 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/zip.png
--rw-r--r--   0 maurits    (501) staff       (20)     2695 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:32:27.290001 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/
--rw-r--r--   0 maurits    (501) staff       (20)      352 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)  2166281 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/freedesktop.org.xml
--rw-r--r--   0 maurits    (501) staff       (20)    17824 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/magic.py
--rw-r--r--   0 maurits    (501) staff       (20)    20298 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/mime.types
--rw-r--r--   0 maurits    (501) staff       (20)     3277 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/mtr_mimetypes.py
--rw-r--r--   0 maurits    (501) staff       (20)     2112 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/py_mimetypes.py
--rw-r--r--   0 maurits    (501) staff       (20)     4803 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/smi_mimetypes.py
--rw-r--r--   0 maurits    (501) staff       (20)     1091 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/suppl_mimetypes.py
--rw-r--r--   0 maurits    (501) staff       (20)     2701 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/windows_mimetypes.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:32:27.260892 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:32:27.290897 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      243 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/profiles/default/componentregistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)       68 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      178 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/profiles/default/toolset.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1233 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1025 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:32:27.292207 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:32:27.293798 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/input/
--rw-r--r--   0 maurits    (501) staff       (20)    32120 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/input/OOoCalc
--rw-r--r--   0 maurits    (501) staff       (20)     5360 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/input/OOoWriter
--rw-r--r--   0 maurits    (501) staff       (20)       73 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/input/rest1.rst
--rw-r--r--   0 maurits    (501) staff       (20)      210 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/input/simplezip
--rw-r--r--   0 maurits    (501) staff       (20)     8283 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/input/sxw-ooo-trolltech
--rw-r--r--   0 maurits    (501) staff       (20)     3578 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/test_encoding.py
--rw-r--r--   0 maurits    (501) staff       (20)     1689 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/test_magic.py
--rw-r--r--   0 maurits    (501) staff       (20)     6605 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/test_mimetypes.py
--rw-r--r--   0 maurits    (501) staff       (20)      937 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      235 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tool.gif
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:32:27.294656 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/www/
--rw-r--r--   0 maurits    (501) staff       (20)     1997 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/www/addMimeType.zpt
--rw-r--r--   0 maurits    (501) staff       (20)     2009 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/www/editMimeType.zpt
--rw-r--r--   0 maurits    (501) staff       (20)     1994 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/www/listMimeTypes.zpt
--rw-r--r--   0 maurits    (501) staff       (20)      268 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/Products/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:32:27.266526 Products.MimetypesRegistry-2.1.9/Products.MimetypesRegistry.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    15340 2022-01-19 14:32:27.000000 Products.MimetypesRegistry-2.1.9/Products.MimetypesRegistry.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4664 2022-01-19 14:32:27.000000 Products.MimetypesRegistry-2.1.9/Products.MimetypesRegistry.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-01-19 14:32:27.000000 Products.MimetypesRegistry-2.1.9/Products.MimetypesRegistry.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2022-01-19 14:32:27.000000 Products.MimetypesRegistry-2.1.9/Products.MimetypesRegistry.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-01-19 14:32:27.000000 Products.MimetypesRegistry-2.1.9/Products.MimetypesRegistry.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      149 2022-01-19 14:32:27.000000 Products.MimetypesRegistry-2.1.9/Products.MimetypesRegistry.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2022-01-19 14:32:27.000000 Products.MimetypesRegistry-2.1.9/Products.MimetypesRegistry.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1328 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6525 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/bootstrap.py
--rw-r--r--   0 maurits    (501) staff       (20)      421 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/buildout.cfg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:32:27.294912 Products.MimetypesRegistry-2.1.9/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1600 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      246 2022-01-19 14:32:27.295885 Products.MimetypesRegistry-2.1.9/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1625 2022-01-19 14:32:26.000000 Products.MimetypesRegistry-2.1.9/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:20:14.849243 Products.MimetypesRegistry-3.0.0/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1019 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/.editorconfig
+-rw-r--r--   0 gil       (1000) gil       (1000)      149 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/.gitignore
+-rw-r--r--   0 gil       (1000) gil       (1000)      128 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/.meta.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1098 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 gil       (1000) gil       (1000)    13225 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      250 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    15455 2023-04-19 07:20:14.849243 Products.MimetypesRegistry-3.0.0/PKG-INFO
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:20:14.837243 Products.MimetypesRegistry-3.0.0/Products/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:20:14.839243 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/
+-rw-r--r--   0 gil       (1000) gil       (1000)     3932 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/MimeTypeItem.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    16065 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/MimeTypesRegistry.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      588 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      286 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/common.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      655 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2314 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/encoding.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:20:14.845243 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/
+-rw-r--r--   0 gil       (1000) gil       (1000)      331 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/application.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      681 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/audio.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      350 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/avi.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      445 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/c.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      640 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/core.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      421 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/cpp.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      469 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/deb.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      761 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/doc.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      761 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/docx.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      572 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/down.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      700 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/dvi.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      331 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/exe.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      420 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/f.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      550 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/font.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      252 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/gf.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      417 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/h.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      599 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/html.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      330 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/image.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      662 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/info.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      711 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/iso.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      573 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/java.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      668 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/log.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      613 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/man.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      355 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/message.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      681 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/midi.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      331 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/mime.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      420 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/o.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      513 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/pdf.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      272 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/pk.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      422 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/pl.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      330 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/png.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      413 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/ppt.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      413 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/pptx.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      638 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/ps.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      641 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/py.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      350 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/quicktime.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      469 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/rar.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      469 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/rpm.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      722 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/sh.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      869 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/sxc.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      897 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/sxd.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      861 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/sxg.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      844 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/sxi.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      888 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/sxm.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      861 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/sxw.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      469 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/tar.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      349 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/tex.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      249 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/text.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      662 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/tgz.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      249 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/txt.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      295 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/unknown.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      591 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/up.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      453 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/vcal.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      564 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/vcard.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      350 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/video.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      681 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/wav.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      622 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/xls.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      622 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/xlsx.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      469 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/zip.png
+-rw-r--r--   0 gil       (1000) gil       (1000)     2654 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/interfaces.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:20:14.847243 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/
+-rw-r--r--   0 gil       (1000) gil       (1000)      346 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)  2166281 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/freedesktop.org.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)    18077 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/magic.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    20298 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/mime.types
+-rw-r--r--   0 gil       (1000) gil       (1000)     3228 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/mtr_mimetypes.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2088 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/py_mimetypes.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4656 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/smi_mimetypes.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1067 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/suppl_mimetypes.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2622 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/windows_mimetypes.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:20:14.836243 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/profiles/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:20:14.847243 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/profiles/default/
+-rw-r--r--   0 gil       (1000) gil       (1000)      258 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/profiles/default/componentregistry.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)       85 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/profiles/default/metadata.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      195 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/profiles/default/toolset.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1192 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/setuphandlers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1000 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/testing.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:20:14.848243 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:20:14.848243 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/input/
+-rw-r--r--   0 gil       (1000) gil       (1000)    32120 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/input/OOoCalc
+-rw-r--r--   0 gil       (1000) gil       (1000)     5360 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/input/OOoWriter
+-rw-r--r--   0 gil       (1000) gil       (1000)       73 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/input/rest1.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      210 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/input/simplezip
+-rw-r--r--   0 gil       (1000) gil       (1000)     8283 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/input/sxw-ooo-trolltech
+-rw-r--r--   0 gil       (1000) gil       (1000)     3737 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/test_encoding.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1673 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/test_magic.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6601 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/test_mimetypes.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      841 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/utils.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      235 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tool.gif
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:20:14.849243 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/www/
+-rw-r--r--   0 gil       (1000) gil       (1000)     2246 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/www/addMimeType.zpt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2325 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/www/editMimeType.zpt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2397 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/www/listMimeTypes.zpt
+-rw-r--r--   0 gil       (1000) gil       (1000)      245 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:20:14.838243 Products.MimetypesRegistry-3.0.0/Products.MimetypesRegistry.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    15455 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products.MimetypesRegistry.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     4708 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products.MimetypesRegistry.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products.MimetypesRegistry.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        9 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products.MimetypesRegistry.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products.MimetypesRegistry.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      124 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products.MimetypesRegistry.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        9 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/Products.MimetypesRegistry.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1328 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/README.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      421 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/buildout.cfg
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:20:14.849243 Products.MimetypesRegistry-3.0.0/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1600 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/docs/LICENSE.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2899 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-19 07:20:14.849243 Products.MimetypesRegistry-3.0.0/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1482 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/setup.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1733 2023-04-19 07:20:14.000000 Products.MimetypesRegistry-3.0.0/tox.ini
```

### Comparing `Products.MimetypesRegistry-2.1.9/CHANGES.rst` & `Products.MimetypesRegistry-3.0.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.0 (2023-04-19)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7 support.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5cc689e5)
+
+
 2.1.9 (2022-01-19)
 ------------------
 
 Bug fixes:
 
 
 - Fix missing comma in install_requires.
@@ -287,15 +304,15 @@
 - Compile the 750KiB freedesktop.org.xml file to a binary format which gets
   loaded on Zope startup instead of reparsing the XML file each time. If the
   modification time of the source xml file changes, the binary file is
   automatically recreated. If the binary file cannot be created the xml file
   is reparsed each time as before.
   [hannosch]
 
-- Change some mimetypes returnd by guessMime to match the mimetypes
+- Change some mimetypes returned by guessMime to match the mimetypes
   registered in mtr (from freedesktop.org's mime database).
   [csenger]
 
 - Ensure that lookup doesn't return an empty tuple if asked with a
   mimetypestring returned by guessMime.
   Fixes http://dev.plone.org/plone/ticket/7876
   [csenger]
@@ -492,15 +509,15 @@
 
 - after one night sleeping over it I removed the yesterday added method.
   therefore I added according to some heuristics and OOo-Documentation
   some magic bytes to magic.py and made better tests.
   [yenzenz]
 
 - added a method to detect mimetypes of zipped files,
-  here specialy for OOo now all Openofice files and zip
+  here specially for OOo now all Openoffice files and zip
   files are detected properly.  my simple tests are working:
   a OOo-Writer and a simpe zipfile are detected.
   [yenzenz]
 
 - updated freedesktop.org.xml file to latest CVS version rev 1.57 from
   http://cvs.freedesktop.org/mime/shared-mime-info/freedesktop.org.xml
   [yenzenz]
@@ -598,26 +615,26 @@
 
 1.3.1-1 (2004-08-16)
 --------------------
 
 - Added text/x-html-safe mime type for new transformation
   [tiran]
 
-- Don't return acquisition wrapped mimetype items beause they may lead to
+- Don't return acquisition wrapped mimetype items because they may lead to
   memory leaks.
   [tiran]
 
 
 1.3.0-3 (2004-08-06)
 --------------------
 
 - Added text/wiki mime type
   [tiran]
 
-- Don't log redefine warning if the currrent and the new object are equal
+- Don't log redefine warning if the current and the new object are equal
   [tiran]
 
 - initialize() MTR on __setstate__ aka when the MTR is loaded from ZODB.
   [tiran]
 
 
 1.3.0-2 (2004-07-29)
```

### Comparing `Products.MimetypesRegistry-2.1.9/PKG-INFO` & `Products.MimetypesRegistry-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: Products.MimetypesRegistry
-Version: 2.1.9
+Version: 3.0.0
 Summary: MIME type handling for Zope
 Home-page: https://pypi.org/project/Products.MimetypesRegistry
 Author: Benjamin Saller
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: Zope mimetype registry
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Zope2
-Classifier: Framework :: Zope :: 4
+Classifier: Framework :: Zope :: 5
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.1
-Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 
 ==================
 Mimetypes Registry
 ==================
 
 Provide a registry of mimetypes, accessible via the ``mimetypes_registry`` tool.
@@ -79,14 +77,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.0 (2023-04-19)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7 support.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5cc689e5)
+
+
 2.1.9 (2022-01-19)
 ------------------
 
 Bug fixes:
 
 
 - Fix missing comma in install_requires.
@@ -362,15 +377,15 @@
 - Compile the 750KiB freedesktop.org.xml file to a binary format which gets
   loaded on Zope startup instead of reparsing the XML file each time. If the
   modification time of the source xml file changes, the binary file is
   automatically recreated. If the binary file cannot be created the xml file
   is reparsed each time as before.
   [hannosch]
 
-- Change some mimetypes returnd by guessMime to match the mimetypes
+- Change some mimetypes returned by guessMime to match the mimetypes
   registered in mtr (from freedesktop.org's mime database).
   [csenger]
 
 - Ensure that lookup doesn't return an empty tuple if asked with a
   mimetypestring returned by guessMime.
   Fixes http://dev.plone.org/plone/ticket/7876
   [csenger]
@@ -567,15 +582,15 @@
 
 - after one night sleeping over it I removed the yesterday added method.
   therefore I added according to some heuristics and OOo-Documentation
   some magic bytes to magic.py and made better tests.
   [yenzenz]
 
 - added a method to detect mimetypes of zipped files,
-  here specialy for OOo now all Openofice files and zip
+  here specially for OOo now all Openoffice files and zip
   files are detected properly.  my simple tests are working:
   a OOo-Writer and a simpe zipfile are detected.
   [yenzenz]
 
 - updated freedesktop.org.xml file to latest CVS version rev 1.57 from
   http://cvs.freedesktop.org/mime/shared-mime-info/freedesktop.org.xml
   [yenzenz]
@@ -673,32 +688,30 @@
 
 1.3.1-1 (2004-08-16)
 --------------------
 
 - Added text/x-html-safe mime type for new transformation
   [tiran]
 
-- Don't return acquisition wrapped mimetype items beause they may lead to
+- Don't return acquisition wrapped mimetype items because they may lead to
   memory leaks.
   [tiran]
 
 
 1.3.0-3 (2004-08-06)
 --------------------
 
 - Added text/wiki mime type
   [tiran]
 
-- Don't log redefine warning if the currrent and the new object are equal
+- Don't log redefine warning if the current and the new object are equal
   [tiran]
 
 - initialize() MTR on __setstate__ aka when the MTR is loaded from ZODB.
   [tiran]
 
 
 1.3.0-2 (2004-07-29)
 --------------------
 
 - Changed version to stick to Archetypes version.
   [tiran]
-
-
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/MimeTypeItem.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/MimeTypeItem.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-# -*- coding: utf-8 -*-
-
 from AccessControl import ClassSecurityInfo
-from Acquisition import Explicit
 from AccessControl.class_init import InitializeClass
+from Acquisition import Explicit
 from OFS.SimpleItem import Item
 from Persistence import Persistent
 from Products.CMFCore.permissions import ManagePortal
 from Products.MimetypesRegistry.interfaces import IMimetype
-from six.moves import urllib
 from zope.interface import implementer
 
 import os
-import six
+import urllib
 
 
 @implementer(IMimetype)
 class MimeTypeItem(Persistent, Explicit, Item):
     security = ClassSecurityInfo()
 
     extensions = ()
     globs = ()
 
-    def __init__(self, name='', mimetypes=None, extensions=None,
-                 binary=None, icon_path='', globs=None):
+    def __init__(
+        self,
+        name="",
+        mimetypes=None,
+        extensions=None,
+        binary=None,
+        icon_path="",
+        globs=None,
+    ):
         if name:
             self.__name__ = self.id = name
         if mimetypes is not None:
             self.mimetypes = mimetypes
         if extensions is not None:
             self.extensions = extensions
         if binary is not None:
@@ -47,78 +51,76 @@
         return not (other in self.mimetypes)
 
     def __hash__(self):
         return hash(self.name())
 
     @security.public
     def name(self):
-        """ The name of this object """
+        """The name of this object"""
         return self.__name__
 
     @security.public
     def major(self):
-        """ return the major part of the RFC-2046 name for this mime type """
-        return self.normalized().split('/', 1)[0]
+        """return the major part of the RFC-2046 name for this mime type"""
+        return self.normalized().split("/", 1)[0]
 
     @security.public
     def minor(self):
-        """ return the minor part of the RFC-2046 name for this mime type """
-        return self.normalized().split('/', 1)[1]
+        """return the minor part of the RFC-2046 name for this mime type"""
+        return self.normalized().split("/", 1)[1]
 
     @security.public
     def normalized(self):
-        """ return the main RFC-2046 name for this mime type
+        """return the main RFC-2046 name for this mime type
 
         e.g. if this object has names ('text/restructured', 'text-x-rst')
         then self.normalized() will always return the first form.
         """
         return self.mimetypes[0]
 
     @security.public
     def urlsafe(self):
         """Return a url safe version of the normalized version of this
         mime type.
         """
         return urllib.parse.quote(self.normalized())
 
     @security.protected(ManagePortal)
-    def edit(self, name, mimetypes, extensions, icon_path,
-             binary=0, globs=None, REQUEST=None):
+    def edit(
+        self, name, mimetypes, extensions, icon_path, binary=0, globs=None, REQUEST=None
+    ):
         """edit this mime type"""
         # if mimetypes and extensions are string instead of lists,
         # split them on new lines
-        if isinstance(mimetypes, six.string_types):
-            mimetypes = [mts.strip() for mts in mimetypes.split('\n')
-                         if mts.strip()]
-        if isinstance(extensions, six.string_types):
-            extensions = [mts.strip() for mts in extensions.split('\n')
-                          if mts.strip()]
-        if isinstance(globs, six.string_types):
-            globs = [glob.strip() for glob in globs.split('\n')
-                     if glob.strip()]
+        if isinstance(mimetypes, str):
+            mimetypes = [mts.strip() for mts in mimetypes.split("\n") if mts.strip()]
+        if isinstance(extensions, str):
+            extensions = [mts.strip() for mts in extensions.split("\n") if mts.strip()]
+        if isinstance(globs, str):
+            globs = [glob.strip() for glob in globs.split("\n") if glob.strip()]
         self.__name__ = self.id = name
         self.mimetypes = mimetypes
         self.globs = globs
         self.extensions = extensions
         self.binary = binary
         self.icon_path = icon_path
         if REQUEST is not None:
-            REQUEST['RESPONSE'].redirect(self.absolute_url() + '/manage_main')
+            REQUEST["RESPONSE"].redirect(self.absolute_url() + "/manage_main")
 
 
 InitializeClass(MimeTypeItem)
 
 
-ICONS_DIR = os.path.join(os.path.dirname(__file__), 'icons')
-PREFIX = '++resource++mimetype.icons/'
+ICONS_DIR = os.path.join(os.path.dirname(__file__), "icons")
+PREFIX = "++resource++mimetype.icons/"
 
 
-def guess_icon_path(mimetype, icons_dir=ICONS_DIR, icon_ext='png'):
+def guess_icon_path(mimetype, icons_dir=ICONS_DIR, icon_ext="png"):
     if mimetype.extensions:
         for ext in mimetype.extensions:
-            icon_path = '%s.%s' % (ext, icon_ext)
+            icon_path = f"{ext}.{icon_ext}"
             if os.path.exists(os.path.join(icons_dir, icon_path)):
                 return PREFIX + icon_path
-    icon_path = '%s.png' % mimetype.major()
+    icon_path = "%s.png" % mimetype.major()
     if os.path.exists(os.path.join(icons_dir, icon_path)):
         return PREFIX + icon_path
-    return PREFIX + 'unknown.png'
+    return PREFIX + "unknown.png"
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/MimeTypesRegistry.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/MimeTypesRegistry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-# -*- coding: utf-8 -*-
 from AccessControl import ClassSecurityInfo
-from Acquisition import aq_base
 from AccessControl.class_init import InitializeClass
+from Acquisition import aq_base
 from BTrees.OOBTree import OOBTree
 from OFS.Folder import Folder
 from Persistence import PersistentMapping
 from Products.CMFCore.ActionProviderBase import ActionProviderBase
 from Products.CMFCore.permissions import ManagePortal
 from Products.CMFCore.utils import registerToolInterface
 from Products.CMFCore.utils import UniqueObject
@@ -23,60 +22,56 @@
 from zope.contenttype import guess_content_type
 from zope.interface import implementer
 
 import fnmatch
 import logging
 import os
 import re
-import six
 
 
 logger = logging.getLogger(__name__)
 
 
 suffix_map = {
-    'tgz': '.tar.gz',
-    'taz': '.tar.gz',
-    'tz': '.tar.gz',
+    "tgz": ".tar.gz",
+    "taz": ".tar.gz",
+    "tz": ".tar.gz",
 }
 
 encodings_map = {
-    'gz': 'gzip',
-    'Z': 'compress',
+    "gz": "gzip",
+    "Z": "compress",
 }
 
-_www = os.path.join(os.path.dirname(__file__), 'www')
+_www = os.path.join(os.path.dirname(__file__), "www")
 
 
 @implementer(IMimetypesRegistry, ISourceAdapter)
 class MimeTypesRegistry(UniqueObject, ActionProviderBase, Folder):
     """Mimetype registry that deals with
     a) registering types
     b) wildcarding of rfc-2046 types
     c) classifying data into a given type
     """
 
-    id = 'mimetypes_registry'
-    meta_type = 'MimeTypes Registry'
+    id = "mimetypes_registry"
+    meta_type = "MimeTypes Registry"
     isPrincipiaFolderish = 1  # Show up in the ZMI
 
     meta_types = all_meta_types = (
-        {'name': 'MimeType',
-         'action': 'manage_addMimeTypeForm'},
+        {"name": "MimeType", "action": "manage_addMimeTypeForm"},
     )
 
     manage_options = (
-        ({'label': 'MimeTypes',
-            'action': 'manage_main'},) +
-        Folder.manage_options[2:]
-    )
+        {"label": "MimeTypes", "action": "manage_main"},
+    ) + Folder.manage_options[2:]
 
-    manage_addMimeTypeForm = PageTemplateFile('addMimeType', _www)
-    manage_main = PageTemplateFile('listMimeTypes', _www)
-    manage_editMimeTypeForm = PageTemplateFile('editMimeType', _www)
+    manage_addMimeTypeForm = PageTemplateFile("addMimeType", _www)
+    manage_main = PageTemplateFile("listMimeTypes", _www)
+    manage_editMimeTypeForm = PageTemplateFile("editMimeType", _www)
 
     security = ClassSecurityInfo()
 
     # FIXME
     __allow_access_to_unprotected_subobjects__ = 1
 
     def __init__(self, id=None):
@@ -86,30 +81,26 @@
         self.suffix_map = suffix_map.copy()
         # Major key -> minor IMimetype objects
         self._mimetypes = PersistentMapping()
         # ext -> IMimetype mapping
         self.extensions = PersistentMapping()
         # glob -> (regex, mimetype) mapping
         self.globs = OOBTree()
-        self.manage_addProperty('defaultMimetype', 'text/plain', 'string')
-        self.manage_addProperty('unicodePolicies', 'strict ignore replace',
-                                'tokens')
-        self.manage_addProperty(
-            'unicodePolicy',
-            'unicodePolicies',
-            'selection')
-        self.manage_addProperty('fallbackEncoding', 'latin1', 'string')
+        self.manage_addProperty("defaultMimetype", "text/plain", "string")
+        self.manage_addProperty("unicodePolicies", "strict ignore replace", "tokens")
+        self.manage_addProperty("unicodePolicy", "unicodePolicies", "selection")
+        self.manage_addProperty("fallbackEncoding", "latin1", "string")
 
         # initialize mime types
         initialize(self)
         self._new_style_mtr = 1
 
     @security.protected(ManagePortal)
     def register(self, mimetype):
-        """ Register a new mimetype
+        """Register a new mimetype
 
         mimetype must implement IMimetype
         """
         mimetype = aq_base(mimetype)
         assert IMimetype.providedBy(mimetype)
         for t in mimetype.mimetypes:
             self.register_mimetype(t, mimetype)
@@ -117,90 +108,77 @@
             self.register_extension(extension, mimetype)
         for glob in mimetype.globs:
             self.register_glob(glob, mimetype)
 
     @security.protected(ManagePortal)
     def register_mimetype(self, mt, mimetype):
         major, minor = split(mt)
-        if not major or not minor or minor == '*':
-            raise MimeTypeException('Can\'t register mime type %s' % mt)
+        if not major or not minor or minor == "*":
+            raise MimeTypeException("Can't register mime type %s" % mt)
         group = self._mimetypes.setdefault(major, PersistentMapping())
         if minor in group:
             if group.get(minor) != mimetype:
-                logger.warning(
-                    'Redefining mime type {0} ({1})'.format(
-                        mt,
-                        mimetype.__class__
-                    )
-                )
+                logger.warning(f"Redefining mime type {mt} ({mimetype.__class__})")
         group[minor] = mimetype
 
     @security.protected(ManagePortal)
     def register_extension(self, extension, mimetype):
-        """ Associate a file's extension to a IMimetype
+        """Associate a file's extension to a IMimetype
 
         extension is a string representing a file extension (not
         prefixed by a dot) mimetype must implement IMimetype
         """
         mimetype = aq_base(mimetype)
         if extension in self.extensions:
             if self.extensions.get(extension) != mimetype:
                 logger.warning(
-                    'Redefining extension {0} from {1} to {2}'.format(
-                        extension,
-                        self.extensions[extension],
-                        mimetype
+                    "Redefining extension {} from {} to {}".format(
+                        extension, self.extensions[extension], mimetype
                     )
                 )
         # we don't validate fmt yet, but its ["txt", "html"]
         self.extensions[extension] = mimetype
 
     @security.protected(ManagePortal)
     def register_glob(self, glob, mimetype):
-        """ Associate a glob to a IMimetype
+        """Associate a glob to a IMimetype
 
         glob is a shell-like glob that will be translated to a regex
         to match against whole filename.
         mimetype must implement IMimetype.
         """
-        globs = getattr(self, 'globs', None)
+        globs = getattr(self, "globs", None)
         if globs is None:
             self.globs = globs = OOBTree()
         mimetype = aq_base(mimetype)
         existing = globs.get(glob)
         if existing is not None:
             regex, mt = existing
             if mt != mimetype:
-                logger.warning(
-                    'Redefining glob {0} from {1} to {2}'.format(
-                        glob,
-                        mt,
-                        mimetype
-                    )
-                )
+                logger.warning(f"Redefining glob {glob} from {mt} to {mimetype}")
         # we don't validate fmt yet, but its ["txt", "html"]
         pattern = re.compile(fnmatch.translate(glob))
         globs[glob] = (pattern, mimetype)
 
     @security.protected(ManagePortal)
     def unregister(self, mimetype):
-        """ Unregister a new mimetype
+        """Unregister a new mimetype
 
         mimetype must implement IMimetype
         """
         assert IMimetype.providedBy(mimetype)
         for t in mimetype.mimetypes:
             major, minor = split(t)
             group = self._mimetypes.get(major, {})
             if group.get(minor) == mimetype:
                 del group[minor]
         for e in mimetype.extensions:
             if self.extensions.get(e) == mimetype:
                 del self.extensions[e]
-        globs = getattr(self, 'globs', None)
+        globs = getattr(self, "globs", None)
         if globs is not None:
             for glob in mimetype.globs:
                 existing = globs.get(glob)
                 if existing is None:
                     continue
                 regex, mt = existing
                 if mt == mimetype:
@@ -230,19 +208,19 @@
         wildcard (*) mimetypestring may and IMimetype object (in this
         case it will be returned unchanged
 
         Return a list of mimetypes objects associated with the
         RFC-2046 name return an empty list if no one is known.
         """
         if IMimetype.providedBy(mimetypestring):
-            return (aq_base(mimetypestring), )
+            return (aq_base(mimetypestring),)
         __traceback_info__ = (repr(mimetypestring), str(mimetypestring))
         major, minor = split(str(mimetypestring))
         group = self._mimetypes.get(major, {})
-        if not minor or minor == '*':
+        if not minor or minor == "*":
             res = group.values()
         else:
             res = group.get(minor)
             if res:
                 res = (res,)
             else:
                 return ()
@@ -255,15 +233,15 @@
         Filename maybe a file name like 'content.txt' or an extension
         like 'rest'
 
         Return an IMimetype object associated with the file's
         extension or None
         """
         base = None
-        if filename.find('.') != -1:
+        if filename.find(".") != -1:
             base, ext = os.path.splitext(filename)
             ext = ext[1:]  # remove the dot
             while ext in self.suffix_map:
                 base, ext = os.path.splitext(base + self.suffix_map[ext])
                 ext = ext[1:]  # remove the dot
         else:
             ext = filename
@@ -281,24 +259,24 @@
     def globFilename(self, filename):
         """Lookup for IMimetypes object matching filename
 
         Filename must be a complete filename with extension.
 
         Return an IMimetype object associated with the glob's or None
         """
-        globs = getattr(self, 'globs', {})
+        globs = getattr(self, "globs", {})
         for key in globs:
             glob, mimetype = globs[key]
             if glob.match(filename):
                 return aq_base(mimetype)
         return None
 
     @security.public
     def lookupGlob(self, glob):
-        globs = getattr(self, 'globs', None)
+        globs = getattr(self, "globs", None)
         if globs is not None:
             return aq_base(globs.get(glob))
 
     def _classifiers(self):
         return [mt for mt in self.mimetypes() if IClassifier.providedBy(mt)]
 
     @security.public
@@ -335,132 +313,152 @@
                     _mt = self.lookup(mstr)
                     if len(_mt) > 0:
                         mt = _mt[0]
         if not mt:
             if not data:
                 mtlist = self.lookup(self.defaultMimetype)
             elif filename:
-                mtlist = self.lookup('application/octet-stream')
+                mtlist = self.lookup("application/octet-stream")
             else:
-                failed = 'text/x-unknown-content-type'
-                filename = filename or ''
-                data = data or ''
-                if six.PY3:
-                    data = data.encode()
+                failed = "text/x-unknown-content-type"
+                filename = filename or ""
+                data = data or ""
+                data = data.encode()
                 ct, enc = guess_content_type(filename, data, None)
                 if ct == failed:
-                    ct = 'text/plain'
+                    ct = "text/plain"
                 mtlist = self.lookup(ct)
             if len(mtlist) > 0:
                 mt = mtlist[0]
             else:
                 return None
 
         # Remove acquisition wrappers
         return aq_base(mt)
 
     def __call__(self, data, **kwargs):
-        """ Return a triple (data, filename, mimetypeobject) given
-        some raw data and optional paramters
+        """Return a triple (data, filename, mimetypeobject) given
+        some raw data and optional parameters
 
         method from the isourceAdapter interface
         """
-        mimetype = kwargs.get('mimetype', None)
-        filename = kwargs.get('filename', None)
-        encoding = kwargs.get('encoding', None)
+        mimetype = kwargs.get("mimetype", None)
+        filename = kwargs.get("filename", None)
+        encoding = kwargs.get("encoding", None)
         mt = None
-        if hasattr(data, 'filename'):
+        if hasattr(data, "filename"):
             filename = os.path.basename(data.filename)
-        elif hasattr(data, 'name'):
+        elif hasattr(data, "name"):
             filename = os.path.basename(data.name)
 
-        if hasattr(data, 'read'):
+        if hasattr(data, "read"):
             _data = data.read()
-            if hasattr(data, 'seek'):
+            if hasattr(data, "seek"):
                 data.seek(0)
             data = _data
 
         # We need to figure out if data is binary and skip encoding if
         # it is
         mt = self.classify(data, mimetype=mimetype, filename=filename)
 
-        if not mt.binary and not isinstance(data, six.text_type):
+        if not mt.binary and not isinstance(data, str):
             # if no encoding specified, try to guess it from data
             if encoding is None:
                 encoding = self.guess_encoding(data)
 
             # ugly workaround for
             # https://sourceforge.net/tracker/?func=detail&aid=1068001&group_id=75272&atid=543430
             # covered by
             # https://sourceforge.net/tracker/?func=detail&atid=355470&aid=843590&group_id=5470
             # dont remove this code unless python is fixed.
             if encoding == "macintosh":
-                encoding = 'mac_roman'
+                encoding = "mac_roman"
 
             try:
                 try:
-                    data = six.text_type(data, encoding, self.unicodePolicy)
+                    data = str(data, encoding, self.unicodePolicy)
                 except (ValueError, LookupError):
                     # wrong unicodePolicy
-                    data = six.text_type(data, encoding)
-            except:
-                data = six.text_type(data, self.fallbackEncoding)
+                    data = str(data, encoding)
+            except Exception:
+                data = str(data, self.fallbackEncoding)
 
         return (data, filename, aq_base(mt))
 
     @security.public
     def guess_encoding(self, data):
-        """ Try to guess encoding from a text value.
+        """Try to guess encoding from a text value.
 
         If no encoding can be guessed, fall back to utf-8.
         """
-        if isinstance(data, six.text_type):
+        if isinstance(data, str):
             # data maybe unicode but with another encoding specified
-            data = data.encode('UTF-8')
+            data = data.encode("UTF-8")
         encoding = guess_encoding(data)
         if encoding is None:
-            encoding = 'utf-8'
+            encoding = "utf-8"
         return encoding
 
     @security.protected(ManagePortal)
     def manage_delObjects(self, ids, REQUEST=None):
-        """ delete the selected mime types """
+        """delete the selected mime types"""
         for id in ids:
             self.unregister(self.lookup(id)[0])
         if REQUEST is not None:
-            REQUEST['RESPONSE'].redirect(self.absolute_url() + '/manage_main')
+            REQUEST["RESPONSE"].redirect(self.absolute_url() + "/manage_main")
 
     @security.protected(ManagePortal)
-    def manage_addMimeType(self, id, mimetypes, extensions, icon_path,
-                           binary=0, globs=None, REQUEST=None):
+    def manage_addMimeType(
+        self, id, mimetypes, extensions, icon_path, binary=0, globs=None, REQUEST=None
+    ):
         """add a mime type to the tool"""
-        mt = MimeTypeItem(id, mimetypes, extensions=extensions,
-                          binary=binary, icon_path=icon_path, globs=globs)
+        mt = MimeTypeItem(
+            id,
+            mimetypes,
+            extensions=extensions,
+            binary=binary,
+            icon_path=icon_path,
+            globs=globs,
+        )
         self.register(mt)
         if REQUEST is not None:
-            REQUEST['RESPONSE'].redirect(self.absolute_url() + '/manage_main')
+            REQUEST["RESPONSE"].redirect(self.absolute_url() + "/manage_main")
 
     @security.protected(ManagePortal)
-    def manage_editMimeType(self, name, new_name, mimetypes, extensions,
-                            icon_path, binary=0, globs=None, REQUEST=None):
-        """Edit a mime type by name
-        """
+    def manage_editMimeType(
+        self,
+        name,
+        new_name,
+        mimetypes,
+        extensions,
+        icon_path,
+        binary=0,
+        globs=None,
+        REQUEST=None,
+    ):
+        """Edit a mime type by name"""
         mt = self.lookup(name)[0]
         self.unregister(mt)
-        mt.edit(new_name, mimetypes, extensions, icon_path=icon_path,
-                binary=binary, globs=globs)
+        mt.edit(
+            new_name,
+            mimetypes,
+            extensions,
+            icon_path=icon_path,
+            binary=binary,
+            globs=globs,
+        )
         self.register(mt)
         if REQUEST is not None:
-            REQUEST['RESPONSE'].redirect(self.absolute_url() + '/manage_main')
+            REQUEST["RESPONSE"].redirect(self.absolute_url() + "/manage_main")
 
 
 InitializeClass(MimeTypesRegistry)
-registerToolInterface('mimetypes_registry', IMimetypesRegistryTool)
+registerToolInterface("mimetypes_registry", IMimetypesRegistryTool)
 
 
 def split(name):
-    """ split a mime type in a (major / minor) 2-uple """
+    """split a mime type in a (major / minor) 2-tuple"""
     try:
-        major, minor = name.split('/', 1)
-    except:
-        raise MimeTypeException('Malformed MIME type (%s)' % name)
+        major, minor = name.split("/", 1)
+    except Exception:
+        raise MimeTypeException("Malformed MIME type (%s)" % name)
     return major, minor
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/configure.zcml` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/configure.zcml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
-    i18n_domain="Products.MimetypesRegistry">
+    i18n_domain="Products.MimetypesRegistry"
+    >
 
- <browser:resourceDirectory
+  <browser:resourceDirectory
       name="mimetype.icons"
       directory="icons"
       />
 
   <genericsetup:registerProfile
       name="MimetypesRegistry"
       title="MimetypesRegistry"
-      directory="profiles/default"
       description="Extension profile for default MimetypesRegistry setup."
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/default"
       post_handler=".setuphandlers.post_install"
-    />
+      />
 
 </configure>
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/encoding.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/encoding.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-# -*- coding: utf-8 -*-
 import encodings
 import re
-import six
 
 
-EMACS_ENCODING_RGX = re.compile(r'[^#]*[#\s]*-\*-\s*coding: ([^\s]*)\s*-\*-\s*')
-VIM_ENCODING_RGX = re.compile(r'[^#]*[#\s]*vim:fileencoding=\s*([^\s]*)\s*')
-XML_ENCODING_RGX = re.compile(r'<\?xml version=[^\s]*\s*encoding=([^\s]*)\s*\?>')
+EMACS_ENCODING_RGX = re.compile(r"[^#]*[#\s]*-\*-\s*coding: ([^\s]*)\s*-\*-\s*")
+VIM_ENCODING_RGX = re.compile(r"[^#]*[#\s]*vim:fileencoding=\s*([^\s]*)\s*")
+XML_ENCODING_RGX = re.compile(r"<\?xml version=[^\s]*\s*encoding=([^\s]*)\s*\?>")
 CHARSET_RGX = re.compile(r'charset=([^\s"]*)')
 
 
 def guess_encoding(buffer):
     """Better guess encoding method
 
     It checks if python supports the encoding
     """
     encoding = _guess_encoding(buffer)
     # step 1: if the encoding was detected, use the lower() because python
     # is using lower case names for encodings
-    if encoding and isinstance(encoding, six.string_types):
+    if encoding and isinstance(encoding, str):
         # encoding = encoding.lower()
         pass
     else:
         return None
     # try to find an encoding function for the encoding
     # if None is returned or an exception is raised the encoding is invalid
     try:
         result = encodings.search_function(encoding.lower())
-    except:
+    except Exception:
         # XXX log
         result = None
 
     if result:
         # got a valid encoding
         return encoding
     else:
@@ -39,41 +37,41 @@
 
 
 def _guess_encoding(buffer):
     """try to guess encoding from a buffer
 
     FIXME: it could be mime type driven but it seems less painful like that
     """
-    assert isinstance(buffer, type('')), type(buffer)
+    assert isinstance(buffer, str), type(buffer)
     # default to ascii on empty buffer
     if not buffer:
-        return 'ascii'
+        return "ascii"
 
     # check for UTF-8 byte-order mark
-    if buffer.startswith('\xef\xbb\xbf'):
-        return 'UTF-8'
+    if buffer.startswith("\xef\xbb\xbf"):
+        return "UTF-8"
 
-    first_lines = buffer.split('\n')[:2]
+    first_lines = buffer.split("\n")[:2]
     for line in first_lines:
         # check for emacs encoding declaration
         m = EMACS_ENCODING_RGX.match(line)
         if m is not None:
             return m.group(1)
         # check for vim encoding declaration
         m = VIM_ENCODING_RGX.match(line)
         if m is not None:
             return m.group(1)
 
     # check for xml encoding declaration
-    if first_lines[0].startswith('<?xml'):
+    if first_lines[0].startswith("<?xml"):
         m = XML_ENCODING_RGX.match(first_lines[0])
         if m is not None:
             return m.group(1)[1:-1]
         # xml files with no encoding declaration default to UTF-8
-        return 'UTF-8'
+        return "UTF-8"
 
     # try to get charset declaration
     # FIXME: should we check it's html before ?
     m = CHARSET_RGX.search(buffer)
     if m is not None:
         return m.group(1)
     return None
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/audio.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/audio.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/core.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/core.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/doc.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/doc.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/docx.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/docx.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/down.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/down.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/dvi.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/dvi.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/font.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/font.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/html.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/html.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/info.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/info.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/iso.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/iso.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/java.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/java.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/log.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/log.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/man.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/man.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/midi.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/midi.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/pdf.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/pdf.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/ps.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/ps.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/py.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/py.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/sh.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/sh.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/sxc.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/sxc.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/sxd.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/sxd.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/sxg.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/sxg.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/sxi.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/sxi.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/sxm.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/sxm.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/sxw.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/sxw.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/tgz.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/tgz.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/up.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/up.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/vcard.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/vcard.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/wav.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/wav.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/xls.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/xls.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/icons/xlsx.png` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/icons/xlsx.png`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/interfaces.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from zope.interface import Interface
 
 
 class MimeTypeException(Exception):
     pass
 
 
@@ -15,44 +14,43 @@
     # binary = Attribute("""Boolean indicating if the mimetype should be
     # treated as binary (and not human readable)""")
 
     def name(self):
         """return the Human readable name of the mimetype"""
 
     def major(self):
-        """ return the major part of the RFC-2046 name for this mime type """
+        """return the major part of the RFC-2046 name for this mime type"""
 
     def minor(self):
-        """ return the minor part of the RFC-2046 name for this mime type """
+        """return the minor part of the RFC-2046 name for this mime type"""
 
     def normalized(self):
-        """ return the main RFC-2046 name for this mime type
+        """return the main RFC-2046 name for this mime type
 
         e.g. if this object has names ('text/restructured', 'text-x-rst')
         then self.normalized() will always return the first form.
         """
 
 
 class IClassifier(Interface):
     """Optional mixin interface for imimetype, code to test if the
     mimetype is present in data
     """
+
     def classify(data):
-        """ boolean indicating if the data fits the mimetype"""
+        """boolean indicating if the data fits the mimetype"""
 
 
 class ISourceAdapter(Interface):
-
     def __call__(data, **kwargs):
         """convert data to unicode, may take optional kwargs to aid in
         conversion"""
 
 
 class IMimetypesRegistry(Interface):
-
     def classify(data, mimetype=None, filename=None):
         """return a content type for this data or None
         None should rarely be returned as application/octet can be
         used to represent most types
         """
 
     def lookup(mimetypestring):
@@ -63,24 +61,23 @@
         it will be returned unchanged, else it should be a RFC-2046 name
 
         return a list of mimetypes objects associated with the RFC-2046 name
         return an empty list if no one is known.
         """
 
     def lookupExtension(filename):
-        """ return the mimetypes object associated with the file's extension
+        """return the mimetypes object associated with the file's extension
         return None if it is not known.
 
         filename maybe a file name like 'content.txt' or an extension like
         'rest'
         """
 
     def mimetypes():
-        """return all defined mime types, each one implements at least imimetype
-        """
+        """return all defined mime types, each one implements at least imimetype"""
 
     def list_mimetypes():
         """return all defined mime types, as string"""
 
 
 class IMimetypesRegistryTool(Interface):
     """Marker interface for the mimetypes_registry tool."""
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/freedesktop.org.xml` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/freedesktop.org.xml`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/mime.types` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/mime.types`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/mtr_mimetypes.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/mtr_mimetypes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,139 +1,126 @@
-# -*- coding: utf-8 -*-
 from Products.MimetypesRegistry.interfaces import IClassifier
 from Products.MimetypesRegistry.MimeTypeItem import MimeTypeItem
 from zope.interface import implementer
 
 import inspect
 import re
 
 
 class text_plain(MimeTypeItem):
-
     __name__ = "Plain Text"
-    mimetypes = ('text/plain',)
-    extensions = ('txt',)
+    mimetypes = ("text/plain",)
+    extensions = ("txt",)
     binary = 0
 
 
 class text_pre_plain(MimeTypeItem):
-
     __name__ = "Pre-formatted Text (<pre>)"
-    mimetypes = ('text/plain-pre',)
+    mimetypes = ("text/plain-pre",)
     extensions = ()
     binary = 0
 
 
 class text_structured(MimeTypeItem):
-
     __name__ = "Structured Text"
-    mimetypes = ('text/structured',)
-    extensions = ('stx',)
+    mimetypes = ("text/structured",)
+    extensions = ("stx",)
     binary = 0
 
 
 class text_rest(MimeTypeItem):
-
     __name__ = "reStructured Text"
-    mimetypes = ("text/x-rst", "text/restructured",)
+    mimetypes = (
+        "text/x-rst",
+        "text/restructured",
+    )
     extensions = ("rst", "rest", "restx")  # txt?
     binary = 0
 
 
 class text_python(MimeTypeItem):
-
     __name__ = "Python Source"
     mimetypes = ("text/x-python",)
     extensions = ("py",)
     binary = 0
 
 
 class text_wiki(MimeTypeItem):
-
     __name__ = "Wiki text"
     mimetypes = ("text/wiki",)
     extensions = ()
     binary = 0
 
 
 class application_rtf(MimeTypeItem):
-
-    __name__ = 'Rich Text Format (RTF)'
-    mimetypes = ('application/rtf',)
-    extensions = ('rtf',)
+    __name__ = "Rich Text Format (RTF)"
+    mimetypes = ("application/rtf",)
+    extensions = ("rtf",)
     binary = 1
 
 
 class application_msword(MimeTypeItem):
-
     __name__ = "Microsoft Word Document"
-    mimetypes = ('application/msword',)
-    extensions = ('doc',)
+    mimetypes = ("application/msword",)
+    extensions = ("doc",)
     binary = 1
 
 
 @implementer(IClassifier)
 class text_xml(MimeTypeItem):
-
     __name__ = "Extensible Markup Language (XML)"
-    mimetypes = ('text/xml',)
-    extensions = ('xml',)
+    mimetypes = ("text/xml",)
+    extensions = ("xml",)
     binary = 0
 
     def classify(self, data):
-        pat = b'^\\s*<\\?xml.*\\?>' if isinstance(data, bytes) else '^\\s*<\\?xml.*\\?>'
-        m = re.search(pat, data)
+        pat = b"^\\s*<\\?xml.*\\?>" if isinstance(data, bytes) else "^\\s*<\\?xml.*\\?>"
         return 1 if re.search(pat, data) else None
 
 
 class application_octet_stream(MimeTypeItem):
     # we need to be sure this one exists
     __name__ = "Octet Stream"
-    mimetypes = ('application/octet-stream',)
+    mimetypes = ("application/octet-stream",)
     binary = 1
     extensions = ()
 
 
 class text_html(MimeTypeItem):
-
     __name__ = "HTML"
-    mimetypes = ('text/html',)
-    extensions = ('html', 'htm')
+    mimetypes = ("text/html",)
+    extensions = ("html", "htm")
     binary = 0
 
 
 class text_html_safe(MimeTypeItem):
-
     __name__ = "Safe HTML"
-    mimetypes = ('text/x-html-safe',)
+    mimetypes = ("text/x-html-safe",)
     extensions = ()
     binary = 0
 
 
 class text_web_intelligent(MimeTypeItem):
-
     __name__ = "Web Intelligent Plain Text"
-    mimetypes = ('text/x-web-intelligent',)
+    mimetypes = ("text/x-web-intelligent",)
     extensions = ()
     binary = 0
 
 
 class text_web_markdown(MimeTypeItem):
-
     __name__ = "Markdown"
-    mimetypes = ('text/x-web-markdown',)
-    extensions = ('markdown',)
+    mimetypes = ("text/x-web-markdown",)
+    extensions = ("markdown",)
     binary = 0
 
 
 class text_web_textile(MimeTypeItem):
-
     __name__ = "Textile"
-    mimetypes = ('text/x-web-textile',)
-    extensions = ('textile',)
+    mimetypes = ("text/x-web-textile",)
+    extensions = ("textile",)
     binary = 0
 
 
 reg_types = [
     text_plain,
     text_pre_plain,
     application_msword,
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/py_mimetypes.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/py_mimetypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from Products.MimetypesRegistry.interfaces import MimeTypeException
 from Products.MimetypesRegistry.MimeTypeItem import guess_icon_path
 from Products.MimetypesRegistry.MimeTypeItem import MimeTypeItem
 from zope.contenttype import add_files
 
 import mimetypes as pymimetypes
 import os.path
@@ -14,15 +13,15 @@
 def mimes_initialize():
     global mimes_initialized
     if mimes_initialized:
         return
     mimes_initialized = True
     # Augment known mime-types.
     here = os.path.dirname(os.path.abspath(__file__))
-    add_files([os.path.join(here, 'mime.types')])
+    add_files([os.path.join(here, "mime.types")])
 
 
 # don't register the mimetype from python mimetypes if matching on of
 # this extensions.
 skip_extensions = ()
 
 
@@ -35,22 +34,23 @@
     # mimetypes python module might have found.
     mimes_initialize()
 
     # Initialize from registry known mimetypes if we are on Windows
     # and pywin32 is available.
     try:
         from .windows_mimetypes import initialize
+
         initialize()
     except ImportError:
         pass
 
     for ext, mt in pymimetypes.types_map.items():
         if not ext:
             continue
-        if ext.startswith('.'):
+        if ext.startswith("."):
             ext = ext[1:]
         if registry.lookupExtension(ext):
             continue
         if ext in skip_extensions:
             continue
 
         try:
@@ -58,13 +58,13 @@
         except MimeTypeException:
             # malformed MIME type
             continue
         if mto:
             mto = mto[0]
             if ext not in mto.extensions:
                 registry.register_extension(ext, mto)
-                mto.extensions += (ext, )
+                mto.extensions += (ext,)
                 # here we guess icon path again, to find icon match the new ext
                 mto.icon_path = guess_icon_path(mto)
             continue
-        isBin = mt.split('/', 1)[0] != "text"
+        isBin = mt.split("/", 1)[0] != "text"
         registry.register(MimeTypeItem(mt, (mt,), (ext,), isBin))
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/smi_mimetypes.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/smi_mimetypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
-from six.moves.cPickle import dump
-from six.moves.cPickle import load
+from pickle import dump
+from pickle import load
 from stat import ST_MTIME
 from xml.sax import parse
 from xml.sax.handler import ContentHandler
 
 import os
 
 
@@ -12,139 +11,140 @@
 SMI_NAME = "freedesktop.org.xml"
 SMI_COMPILED_NAME = "freedesktop.org.xml.bin"
 SMI_FILE = os.path.join(DIR, SMI_NAME)
 SMI_COMPILED_FILE = os.path.join(DIR, SMI_COMPILED_NAME)
 
 
 class SharedMimeInfoHandler(ContentHandler):
-
     current = None
     collect_comment = None
 
     def __init__(self):
         ContentHandler.__init__(self)
         self.mimes = []
 
     def startElement(self, name, attrs):
-        if name in ('mime-type',):
-            current = {'type': attrs['type'],
-                       'comments': {},
-                       'globs': [],
-                       'aliases': []}
+        if name in ("mime-type",):
+            current = {
+                "type": attrs["type"],
+                "comments": {},
+                "globs": [],
+                "aliases": [],
+            }
             self.mimes.append(current)
             self.current = current
             return
-        if name in ('comment',):
+        if name in ("comment",):
             # If no lang, assume 'en'
-            lang = attrs.get('xml:lang', 'en')
-            if lang not in ('en',):
+            lang = attrs.get("xml:lang", "en")
+            if lang not in ("en",):
                 # Ignore for now.
                 return
             self.__comment_buffer = []
             self.__comment_lang = lang
             self.collect_comment = True
             return
-        if name in ('glob',):
-            globs = self.current['globs']
-            globs.append(attrs['pattern'])
+        if name in ("glob",):
+            globs = self.current["globs"]
+            globs.append(attrs["pattern"])
             return
-        if name in ('alias',):
-            aliases = self.current['aliases']
-            aliases.append(attrs['type'])
+        if name in ("alias",):
+            aliases = self.current["aliases"]
+            aliases.append(attrs["type"])
 
     def endElement(self, name):
-        if self.collect_comment and name in ('comment',):
+        if self.collect_comment and name in ("comment",):
             self.collect_comment = False
             lang = self.__comment_lang
-            comment = u''.join(self.__comment_buffer)
+            comment = "".join(self.__comment_buffer)
             if not comment:
-                comment = self.current['type']
-            self.current['comments'][lang] = comment
+                comment = self.current["type"]
+            self.current["comments"][lang] = comment
 
     def characters(self, contents):
         if self.collect_comment:
             self.__comment_buffer.append(contents)
 
 
 def parseSMIFile(infofile):
     handler = SharedMimeInfoHandler()
     parse(infofile, handler)
     return handler.mimes
 
 
 def readSMIFile():
-    """Reads a shared mime info XML file
-    """
+    """Reads a shared mime info XML file"""
     mtime = 0
     try:
         mtime = os.stat(SMI_FILE)[ST_MTIME]
-    except (IOError, OSError):
+    except OSError:
         pass
 
     if os.path.exists(SMI_COMPILED_FILE):
         # If SMI_COMPILED_FILE has equal or newer modification time than the
         # xml file, use the binary one for performance reasons.
 
         bin_mtime = 0
         try:
             bin_mtime = os.stat(SMI_COMPILED_FILE)[ST_MTIME]
-        except (IOError, OSError):
+        except OSError:
             pass
 
         if mtime <= bin_mtime:
             # file is current
             result = None
             try:
-                fd = open(SMI_COMPILED_FILE, 'rb')
+                fd = open(SMI_COMPILED_FILE, "rb")
                 result = load(fd)
                 fd.close()
-            except (IOError, OSError, EOFError):
+            except (OSError, EOFError):
                 pass
 
             if result:
                 return result
 
     result = parseSMIFile(SMI_FILE)
     try:
         # Write the SMI_COMPILED_FILE from the parsed xml file.
-        fd = open(SMI_COMPILED_FILE, 'wb')
+        fd = open(SMI_COMPILED_FILE, "wb")
         dump(result, fd, protocol=2)
         fd.close()
-    except (IOError, OSError):
+    except OSError:
         pass
 
     return result
 
 
 mimetypes = readSMIFile()
 
 
 def initialize(registry):
     global mimetypes
     from Products.MimetypesRegistry.interfaces import MimeTypeException
     from Products.MimetypesRegistry.MimeTypeItem import MimeTypeItem
+
     # Find things that are not in the specially registered mimetypes
     # and add them using some default policy, none of these will impl
     # iclassifier
     for res in mimetypes:
-        mt = str(res['type'])
-        mts = (mt,) + tuple(res['aliases'])
+        mt = str(res["type"])
+        mts = (mt,) + tuple(res["aliases"])
 
         # check the mime type
         try:
             mto = registry.lookup(mt)
         except MimeTypeException:
             # malformed MIME type
             continue
 
-        name = str(res['comments'].get(u'en', mt))
+        name = str(res["comments"].get("en", mt))
 
         # build a list of globs
         globs = []
-        for glob in res['globs']:
+        for glob in res["globs"]:
             if registry.lookupGlob(glob):
                 continue
             else:
                 globs.append(glob)
 
         if mto:
             mto = mto[0]
@@ -153,12 +153,10 @@
                     mto.globs = list(mto.globs) + [glob]
                     registry.register_glob(glob, mto)
             for mt in mts:
                 if mt not in mto.mimetypes:
                     mto.mimetypes = list(mto.mimetypes) + [mt]
                     registry.register_mimetype(mt, mto)
         else:
-            isBin = mt.split('/', 1)[0] != "text"
-            mti = MimeTypeItem(name, mimetypes=mts,
-                               binary=isBin,
-                               globs=globs)
+            isBin = mt.split("/", 1)[0] != "text"
+            mti = MimeTypeItem(name, mimetypes=mts, binary=isBin, globs=globs)
             registry.register(mti)
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/suppl_mimetypes.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/suppl_mimetypes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-# -*- coding: utf-8 -*-
 from Products.MimetypesRegistry.interfaces import MimeTypeException
 from Products.MimetypesRegistry.MimeTypeItem import MimeTypeItem
 
 
 map = {
     # '.extension' : 'mimetype',
-    '.pjpg': 'image/pjpeg',  # progressive jpeg - is this is still a thing?
-    '.woff2': 'font/woff2'
+    ".pjpg": "image/pjpeg",  # progressive jpeg - is this is still a thing?
+    ".woff2": "font/woff2",
 }
 
 
 def initialize(registry):
     # Find things that are not in the specially registered mimetypes
     # and add them using some default policy, none of these will impl
     # iclassifier
     for ext, mt in map.items():
-        if ext[0] == '.':
+        if ext[0] == ".":
             ext = ext[1:]
 
         if registry.lookupExtension(ext):
             continue
 
         try:
             mto = registry.lookup(mt)
         except MimeTypeException:
             # malformed MIME type
             continue
         if mto:
             mto = mto[0]
             if ext not in mto.extensions:
                 registry.register_extension(ext, mto)
-                mto.extensions += (ext, )
+                mto.extensions += (ext,)
             continue
-        isBin = mt.split('/', 1)[0] != "text"
+        isBin = mt.split("/", 1)[0] != "text"
         registry.register(MimeTypeItem(mt, (mt,), (ext,), isBin))
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/mime_types/windows_mimetypes.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/mime_types/windows_mimetypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,89 +1,94 @@
-# -*- coding: utf-8 -*-
 # Utilities for mime-types and the Windows registry.
-import six.moves.winreg
 import logging
 import mimetypes
 import win32api
 import win32con
 
 
-logger = logging.getLogger('mimetypes.win32')
+logger = logging.getLogger("mimetypes.win32")
 
 # "safely" query a value, returning a default when it doesn't exist.
 
 
 def _RegQueryValue(key, value, default=None):
     try:
         data, typ = win32api.RegQueryValueEx(key, value)
     except win32api.error:
         return default
     if typ == win32con.REG_EXPAND_SZ:
         data = win32api.ExpandEnvironmentStrings(data)
     if type in (win32con.REG_EXPAND_SZ, win32con.REG_SZ):
         # Occasionally see trailing \0 chars.
-        data = data.rstrip('\0')
+        data = data.rstrip("\0")
     return data
 
 
 def get_desc_for_mimetype(mime_type):
     try:
-        hk = win32api.RegOpenKey(win32con.HKEY_CLASSES_ROOT,
-                                 r"MIME\Database\Content Type\\" + mime_type)
+        hk = win32api.RegOpenKey(
+            win32con.HKEY_CLASSES_ROOT, r"MIME\Database\Content Type\\" + mime_type
+        )
         desc = _RegQueryValue(hk, "")
     except win32api.error as details:
-        logger.info("win32api error fetching description for mime-type %r: %s",
-                    mime_type, details)
+        logger.info(
+            "win32api error fetching description for mime-type %r: %s",
+            mime_type,
+            details,
+        )
         desc = None
     logger.debug("mime-type %s has description %s", mime_type, desc)
     return desc
 
 
 def get_ext_for_mimetype(mime_type):
     try:
-        hk = win32api.RegOpenKey(win32con.HKEY_CLASSES_ROOT,
-                                 r"MIME\Database\Content Type\\" + mime_type)
+        hk = win32api.RegOpenKey(
+            win32con.HKEY_CLASSES_ROOT, r"MIME\Database\Content Type\\" + mime_type
+        )
         ext = _RegQueryValue(hk, "Extension")
     except win32api.error as details:
-        logger.info("win32api error fetching extension for mime-type %r: %s",
-                    mime_type, details)
+        logger.info(
+            "win32api error fetching extension for mime-type %r: %s", mime_type, details
+        )
         ext = None
     logger.debug("mime-type %s has extension %s", mime_type, ext)
     return ext
 
 
 def get_mime_types():
     try:
-        hk = win32api.RegOpenKey(win32con.HKEY_CLASSES_ROOT,
-                                 r"MIME\Database\Content Type")
+        hk = win32api.RegOpenKey(
+            win32con.HKEY_CLASSES_ROOT, r"MIME\Database\Content Type"
+        )
         items = win32api.RegEnumKeyEx(hk)
     except win32api.error as details:
-        logger.info("win32api error fetching mimetypes: %s",
-                    details)
+        logger.info("win32api error fetching mimetypes: %s", details)
         items = []
     return [i[0] for i in items if i[0]]
 
 
 def normalize(mt):
     # Some mimetypes might have extra ';q=value' params.
-    return mt.lower().split(';')[0]
+    return mt.lower().split(";")[0]
 
 
 def initialize():
     if not mimetypes.inited:
         mimetypes.init()
 
     for mt in get_mime_types():
         ext = get_ext_for_mimetype(mt)
         if not ext:
             continue
         if ext not in mimetypes.types_map:
             mimetypes.add_type(normalize(mt), ext)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     for mt in get_mime_types():
         ext = get_ext_for_mimetype(mt)
         desc = get_desc_for_mimetype(mt)
-        print("%s (%s) - %s" % (mt.lower(), desc, ext))
+        print(f"{mt.lower()} ({desc}) - {ext}")
     import code
+
     code.interact(local=locals())
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/setuphandlers.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/setuphandlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-# -*- coding: utf-8 -*-
 from Products.CMFCore.utils import getToolByName
 from Products.MimetypesRegistry.mime_types import smi_mimetypes
 
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
 def fixUpSMIGlobs(context, reinit=True):
     # This method is used both in migrations where we need the reinit and
     # during site creation, where the registry has already been initialized.
-    mtr = getToolByName(context, 'mimetypes_registry')
+    mtr = getToolByName(context, "mimetypes_registry")
     if reinit:
         smi_mimetypes.initialize(mtr)
 
     # Now comes the fun part. For every glob, lookup a extension
     # matching the glob and unregister it.
     for glob in mtr.globs.keys():
         if glob not in mtr.extensions:
             continue
-        logger.debug(
-            'Found glob %s in extensions registry, removing.' % glob
-        )
+        logger.debug("Found glob %s in extensions registry, removing." % glob)
         mti = mtr.extensions[glob]
         del mtr.extensions[glob]
         if glob in mti.extensions:
-            logger.debug('Found glob %s in mimetype %s extensions, '
-                         'removing.' % (glob, mti))
+            logger.debug(
+                "Found glob %s in mimetype %s extensions, " "removing." % (glob, mti)
+            )
             exts = list(mti.extensions)
             exts.remove(glob)
             mti.extensions = tuple(exts)
             mtr.register(mti)
 
 
 def post_install(context):
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/testing.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/testing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-# -*- coding: utf-8 -*-
 from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
 from plone.app.testing import applyProfile
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PloneSandboxLayer
 
 import Products.MimetypesRegistry
 
 
 class ProductsMimetypesregistryLayer(PloneSandboxLayer):
-
     defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         # Load any other ZCML that is required for your tests.
         # The z3c.autoinclude feature is disabled in the Plone fixture base
         # layer.
         self.loadZCML(package=Products.MimetypesRegistry)
 
     def setUpPloneSite(self, portal):
-        applyProfile(portal, 'Products.MimetypesRegistry:MimetypesRegistry')
+        applyProfile(portal, "Products.MimetypesRegistry:MimetypesRegistry")
 
 
 PRODUCTS_MIMETYPESREGISTRY_FIXTURE = ProductsMimetypesregistryLayer()
 
 
 PRODUCTS_MIMETYPESREGISTRY_INTEGRATION_TESTING = IntegrationTesting(
     bases=(PRODUCTS_MIMETYPESREGISTRY_FIXTURE,),
-    name='ProductsMimetypesregistryLayer:IntegrationTesting',
+    name="ProductsMimetypesregistryLayer:IntegrationTesting",
 )
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/input/OOoCalc` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/input/OOoCalc`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/input/OOoWriter` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/input/OOoWriter`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/input/sxw-ooo-trolltech` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/input/sxw-ooo-trolltech`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/test_encoding.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/test_encoding.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,81 @@
-# -*- coding: utf-8 -*-
 from Products.MimetypesRegistry.encoding import guess_encoding
-from Products.MimetypesRegistry.testing import PRODUCTS_MIMETYPESREGISTRY_INTEGRATION_TESTING
+from Products.MimetypesRegistry.testing import (
+    PRODUCTS_MIMETYPESREGISTRY_INTEGRATION_TESTING,
+)
 
 import unittest
 
 
 class TestGuessEncoding(unittest.TestCase):
-
     layer = PRODUCTS_MIMETYPESREGISTRY_INTEGRATION_TESTING
 
-
     def testUTF8(self):
-        e = guess_encoding('\xef\xbb\xbf any UTF-8 data')
-        self.assertEqual(e, 'UTF-8')
-        e = guess_encoding(' any UTF-8 data \xef\xbb\xbf')
+        e = guess_encoding("\xef\xbb\xbf any UTF-8 data")
+        self.assertEqual(e, "UTF-8")
+        e = guess_encoding(" any UTF-8 data \xef\xbb\xbf")
         self.assertEqual(e, None)
 
     def testEmacs(self):
-        e = guess_encoding('# -*- coding: UTF-8  -*-')
-        self.assertEqual(e, 'UTF-8')
-        e = guess_encoding('''
+        e = guess_encoding("# -*- coding: UTF-8  -*-")
+        self.assertEqual(e, "UTF-8")
+        e = guess_encoding(
+            """
         ### -*- coding: ISO-8859-1  -*-
-        ''')
-        self.assertEqual(e, 'ISO-8859-1')
-        e = guess_encoding('''
+        """
+        )
+        self.assertEqual(e, "ISO-8859-1")
+        e = guess_encoding(
+            """
 
         ### -*- coding: ISO-8859-1  -*-
-        ''')
+        """
+        )
         self.assertEqual(e, None)
 
     def testVim(self):
-        e = guess_encoding('# vim:fileencoding=UTF-8')
-        self.assertEqual(e, 'UTF-8')
-        e = guess_encoding('''
+        e = guess_encoding("# vim:fileencoding=UTF-8")
+        self.assertEqual(e, "UTF-8")
+        e = guess_encoding(
+            """
         ### vim:fileencoding=ISO-8859-1
-        ''')
-        self.assertEqual(e, 'ISO-8859-1')
-        e = guess_encoding('''
+        """
+        )
+        self.assertEqual(e, "ISO-8859-1")
+        e = guess_encoding(
+            """
 
         ### vim:fileencoding= ISO-8859-1
-        ''')
+        """
+        )
         self.assertEqual(e, None)
 
     def testXML(self):
-        e = guess_encoding('<?xml?>')
-        self.assertEqual(e, 'UTF-8')
-        e = guess_encoding('''<?xml version="1.0" encoding="ISO-8859-1" ?>
-        ''')
-        self.assertEqual(e, 'ISO-8859-1')
-        e = guess_encoding('''<?xml version="1.0" encoding="ISO-8859-1"?>
-        ''')
-        self.assertEqual(e, 'ISO-8859-1')
-        e = guess_encoding('''<?xml version="1.0" encoding="ISO-8859-1"?><truc encoding="UTF-8">
+        e = guess_encoding("<?xml?>")
+        self.assertEqual(e, "UTF-8")
+        e = guess_encoding(
+            """<?xml version="1.0" encoding="ISO-8859-1" ?>
+        """
+        )
+        self.assertEqual(e, "ISO-8859-1")
+        e = guess_encoding(
+            """<?xml version="1.0" encoding="ISO-8859-1"?>
+        """
+        )
+        self.assertEqual(e, "ISO-8859-1")
+        e = guess_encoding(
+            """<?xml version="1.0" encoding="ISO-8859-1"?><truc encoding="UTF-8">
         </truc>
-        ''')
-        self.assertEqual(e, 'ISO-8859-1')
+        """
+        )
+        self.assertEqual(e, "ISO-8859-1")
 
     def testHTML(self):
-        e = guess_encoding('''<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">
+        e = guess_encoding(
+            """<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">
 <html>
 <head>
 <title>ASPN : Python Cookbook : Auto-detect XML encoding</title>
     <meta http-equiv="Content-Type" content="text/html; charset=iso-8859-1" />
     <meta name="robots" content="all" />
     <meta name="description" content="ActiveState Open Source Programming tools for Perl Python XML xslt scripting with free trials. Quality development tools for programmers systems administrators database administrators network administrators and webmasters" />
     <meta name="keywords" content="ActiveState,Perl,xml,xslt,mozilla,Open Source,Python,Perl for Win32,resources,PerlScript,ActivePerl,Programming,Programmers,Integrated,Development,Environment,SOAP,Linux,Solaris,Web,development,tools,free,software,download,support,Perl Resource Kit,System Administration,Sys Admin,WinNT,SQL,Oracle,Email,XML,Linux,Programming,perl,NT,2000,windows,Unix,Software,Security,   Administration,systems,windows,database,database,consulting,support,Microsoft,developer,resource,code,tutorials,IDE,Integrated development environment,developer,resources,tcl,php" />
@@ -69,16 +83,17 @@
 <link rel="stylesheet" href="/ASPN/aspn.css" />
 
 </head>
 
 <body bgcolor="#FFFFFF" leftmargin="0" topmargin="0" marginwidth="0" marginheight="0">
 charset=utf-8
 </body>
-</html> ''')
-        self.assertEqual(e, 'iso-8859-1')
+</html> """
+        )
+        self.assertEqual(e, "iso-8859-1")
 
     def test_broken_percent(self):
         e = guess_encoding(
             r"""<pre>
 &lt;metal:block tal:define="dummy python:
 request.RESPONSE.setHeader('Content-Type',
 'text/html;;charset=%s' % charset)" /&gt;
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/test_magic.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/test_magic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# -*- coding: utf-8 -*-
-from Products.MimetypesRegistry.tests.utils import input_file_path
 from Products.CMFCore.utils import getToolByName
 from Products.MimetypesRegistry.mime_types.magic import guessMime
-from Products.MimetypesRegistry.testing import PRODUCTS_MIMETYPESREGISTRY_INTEGRATION_TESTING
 from Products.MimetypesRegistry.MimeTypeItem import MimeTypeItem
+from Products.MimetypesRegistry.testing import (
+    PRODUCTS_MIMETYPESREGISTRY_INTEGRATION_TESTING,
+)
+from Products.MimetypesRegistry.tests.utils import input_file_path
 
 import unittest
 
 
 samplefiles = [
-    ('OOoWriter', 'application/vnd.sun.xml.writer'),
-    ('OOoCalc', 'application/vnd.sun.xml.calc'),
-    ('sxw-ooo-trolltech', 'application/vnd.sun.xml.writer'),  # file from limi
-    ('simplezip', 'application/zip'),
+    ("OOoWriter", "application/vnd.sun.xml.writer"),
+    ("OOoCalc", "application/vnd.sun.xml.calc"),
+    ("sxw-ooo-trolltech", "application/vnd.sun.xml.writer"),  # file from limi
+    ("simplezip", "application/zip"),
 ]
 
 
 class TestGuessMagic(unittest.TestCase):
-
     layer = PRODUCTS_MIMETYPESREGISTRY_INTEGRATION_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        self.registry = getToolByName(self.portal, 'mimetypes_registry')
+        self.portal = self.layer["portal"]
+        self.registry = getToolByName(self.portal, "mimetypes_registry")
 
     def test_guessMime(self):
         for filename, expected in samplefiles:
-            file = open(input_file_path(filename), 'rb')
+            file = open(input_file_path(filename), "rb")
             data = file.read()
             file.close()
 
             # use method direct
             got = guessMime(data)
             self.assertEqual(got, expected)
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/test_mimetypes.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/test_mimetypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,175 +1,178 @@
-# -*- coding: utf-8 -*-
 from Products.CMFCore.utils import getToolByName
 from Products.MimetypesRegistry.mime_types import application_octet_stream
 from Products.MimetypesRegistry.mime_types import text_plain
 from Products.MimetypesRegistry.mime_types import text_xml
-from Products.MimetypesRegistry.testing import PRODUCTS_MIMETYPESREGISTRY_INTEGRATION_TESTING
+from Products.MimetypesRegistry.testing import (
+    PRODUCTS_MIMETYPESREGISTRY_INTEGRATION_TESTING,
+)
 from Products.MimetypesRegistry.tests.utils import input_file_path
 
 import unittest
 
 
 class TestMimeTypesclass(unittest.TestCase):
-
     layer = PRODUCTS_MIMETYPESREGISTRY_INTEGRATION_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        self.registry = getToolByName(self.portal, 'mimetypes_registry')
+        self.portal = self.layer["portal"]
+        self.registry = getToolByName(self.portal, "mimetypes_registry")
 
     def testClassify(self):
         reg = self.registry
         c = reg._classifiers()
-        self.assertTrue(c[0].name().startswith("Extensible Markup Language"),
-                        c[0].name())
+        self.assertTrue(
+            c[0].name().startswith("Extensible Markup Language"), c[0].name()
+        )
 
         # Real XML
         data = "<?xml version='1.0'?><foo>bar</foo>"
         mt = reg.classify(data)
         self.assertTrue(isinstance(mt, text_xml), str(mt))
 
         # with leading whitespace (http://dev.plone.org/archetypes/ticket/622)
         # still valid xml
         data = " <?xml version='1.0'?><foo>bar</foo>"
         mt = reg.classify(data)
         self.assertTrue(isinstance(mt, text_xml), str(mt))
 
         # also #622: this is not xml
-        data = 'xml > plain text'
+        data = "xml > plain text"
         mt = reg.classify(data)
-        self.assertTrue(str(mt) != 'text/xml')
+        self.assertTrue(str(mt) != "text/xml")
 
         # Passed in MT
         mt = reg.classify(data, mimetype="text/plain")
         self.assertTrue(isinstance(mt, text_plain), str(mt))
 
         # Passed in filename
         mt = reg.classify(data, filename="test.xml")
         self.assertTrue(isinstance(mt, text_xml), str(mt))
         mt = reg.classify(data, filename="test.jpg")
-        self.assertEqual(str(mt), 'image/jpeg')
+        self.assertEqual(str(mt), "image/jpeg")
 
         # Passed in uppercase filename
         mt = reg.classify(data, filename="test.JPG")
-        self.assertEqual(str(mt), 'image/jpeg')
+        self.assertEqual(str(mt), "image/jpeg")
 
         # use xml classifier
-        mt = reg.classify('<?xml ?>')
+        mt = reg.classify("<?xml ?>")
         self.assertTrue(isinstance(mt, text_xml), str(mt))
 
         # test no data return default
-        mt = reg.classify('')
+        mt = reg.classify("")
         self.assertTrue(isinstance(mt, text_plain), str(mt))
-        reg.defaultMimetype = 'text/xml'
-        mt = reg.classify('')
+        reg.defaultMimetype = "text/xml"
+        mt = reg.classify("")
         self.assertTrue(isinstance(mt, text_xml), str(mt))
 
         # test unclassifiable data and no stream flag (filename)
-        mt = reg.classify('xxx')
+        mt = reg.classify("xxx")
         self.assertTrue(isinstance(mt, text_plain), str(mt))
 
         # test unclassifiable data and file flag
-        mt = reg.classify('baz', filename='xxx')
+        mt = reg.classify("baz", filename="xxx")
         self.assertTrue(isinstance(mt, application_octet_stream), str(mt))
 
     def testExtension(self):
         reg = self.registry
         data = "<foo>bar</foo>"
         mt = reg.lookupExtension(filename="test.xml")
         self.assertTrue(isinstance(mt, text_xml), str(mt))
 
         mt = reg.classify(data, filename="test.foo")
         self.assertTrue(isinstance(mt, application_octet_stream), str(mt))
 
         mt = reg.classify(data, filename="test.tgz")
-        self.assertEqual(str(mt), 'application/x-tar')
+        self.assertEqual(str(mt), "application/x-tar")
 
         mt = reg.classify(data, filename="test.tar.gz")
-        self.assertEqual(str(mt), 'application/x-tar')
+        self.assertEqual(str(mt), "application/x-tar")
 
         mt = reg.classify(data, filename="test.pdf.gz")
-        self.assertEqual(str(mt), 'application/pdf')
+        self.assertEqual(str(mt), "application/pdf")
 
     def testFDOGlobs(self):
         # The mime types here might only match if they match a glob on
         # the freedesktop.org registry.
-        data = ''
+        data = ""
         reg = self.registry
 
         mt = reg.classify(data, filename="test.ogg")
-        self.assertEqual(str(mt), 'audio/ogg')
+        self.assertEqual(str(mt), "audio/ogg")
 
         mt = reg.classify(data, filename="test.docx")
-        self.assertEqual(str(mt), 'application/vnd.openxmlformats-officedocument.wordprocessingml.document')  # noqa
+        self.assertEqual(
+            str(mt),
+            "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
+        )  # noqa
 
         mt = reg.classify(data, filename="test.anim1")
-        self.assertEqual(str(mt), 'video/x-anim')
+        self.assertEqual(str(mt), "video/x-anim")
 
         mt = reg.classify(data, filename="test.ini~")
-        self.assertEqual(str(mt), 'application/x-trash')
+        self.assertEqual(str(mt), "application/x-trash")
 
         mt = reg.classify(data, filename="test.ini%")
-        self.assertEqual(str(mt), 'application/x-trash')
+        self.assertEqual(str(mt), "application/x-trash")
 
         mt = reg.classify(data, filename="test.ini.bak")
-        self.assertEqual(str(mt), 'application/x-trash')
+        self.assertEqual(str(mt), "application/x-trash")
 
         # TODO: wrongly recognized as text/plain...
         # mt = reg.classify(data, filename="test.f90")
         # self.assertEqual(str(mt), 'text/x-fortran')
 
         mt = reg.classify(data, filename="test.f95")
-        self.assertEqual(str(mt), 'text/x-fortran')
+        self.assertEqual(str(mt), "text/x-fortran")
 
         mt = reg.classify(data, filename="makefile")
-        self.assertEqual(str(mt), 'text/x-makefile')
+        self.assertEqual(str(mt), "text/x-makefile")
 
         # Updated freedesktop.org.xml changed "Makefile" glob to "Makefile."
         # See: https://bugs.freedesktop.org/show_bug.cgi?id=88625
         # mt = reg.classify(data, filename="Makefile")
         # self.assertEqual(str(mt), 'text/x-makefile')
 
         mt = reg.classify(data, filename="AUTHORS")
-        self.assertEqual(str(mt), 'text/x-authors')
+        self.assertEqual(str(mt), "text/x-authors")
 
         mt = reg.classify(data, filename="INSTALL")
         self.assertTrue(
-            str(mt) in [
-                'text/x-install',
-                'application/x-install-instructions'])
+            str(mt) in ["text/x-install", "application/x-install-instructions"]
+        )
 
     def testLookup(self):
         reg = self.registry
-        mt = reg.lookup('text/plain')
+        mt = reg.lookup("text/plain")
         self.assertTrue(isinstance(mt[0], text_plain), str(mt[0]))
 
         # Test lookup of aliases in SMI database (see smi_mimetypes)
-        mt1 = reg.lookup('application/vnd.wordperfect')
-        mt2 = reg.lookup('application/wordperfect')
+        mt1 = reg.lookup("application/vnd.wordperfect")
+        mt2 = reg.lookup("application/wordperfect")
         self.assertEqual(mt1, mt2)
 
-        mt = reg.lookup('text/notexistent')
+        mt = reg.lookup("text/notexistent")
         self.assertEqual(mt, ())
 
     def testAdaptMt(self):
-        data, filename, mt = self.registry('bar', mimetype='text/xml')
-        # this test that data has been adaped and file seeked to 0
-        self.assertEqual(data, 'bar')
+        data, filename, mt = self.registry("bar", mimetype="text/xml")
+        # this test that data has been adapted and file seeked to 0
+        self.assertEqual(data, "bar")
         self.assertEqual(filename, None)
         self.assertTrue(isinstance(mt, text_xml), str(mt))
 
     def testAdaptFile(self):
         file = open(input_file_path("rest1.rst"))
         data, filename, mt = self.registry(file)
-        # this test that data has been adaped and file seeked to 0
+        # this test that data has been adapted and file seeked to 0
         self.assertEqual(data, file.read())
         file.close()
         self.assertEqual(filename, "rest1.rst")
-        self.assertEqual(str(mt), 'text/x-rst')
+        self.assertEqual(str(mt), "text/x-rst")
 
     def testAdaptData(self):
-        data, filename, mt = self.registry('<?xml ?>')
-        # this test that data has been adaped and file seeked to 0
-        self.assertEqual(data, '<?xml ?>')
+        data, filename, mt = self.registry("<?xml ?>")
+        # this test that data has been adapted and file seeked to 0
+        self.assertEqual(data, "<?xml ?>")
         self.assertEqual(filename, None)
         self.assertTrue(isinstance(mt, text_xml), str(mt))
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/tests/utils.py` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/tests/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from os.path import abspath
 from os.path import basename
 from os.path import dirname
 from os.path import join
 
 import glob
 import re
@@ -11,34 +10,30 @@
 def normalize_html(s):
     s = re.sub(r"\s+", " ", s)
     s = re.sub(r"(?s)\s+<", "<", s)
     s = re.sub(r"(?s)>\s+", ">", s)
     s = re.sub(r"\r", "", s)
     return s
 
+
 PREFIX = abspath(dirname(__file__))
 
 
 def input_file_path(file):
-    return join(PREFIX, 'input', file)
+    return join(PREFIX, "input", file)
 
 
 def output_file_path(file):
-    return join(PREFIX, 'output', file)
+    return join(PREFIX, "output", file)
 
 
 def matching_inputs(pattern):
-    return [
-        basename(path) for path in glob.glob(
-            join(
-                PREFIX,
-                "input",
-                pattern))]
+    return [basename(path) for path in glob.glob(join(PREFIX, "input", pattern))]
 
 
 def load(dotted_name, globals=None):
-    """ load a python module from it's name """
+    """load a python module from it's name"""
     mod = __import__(dotted_name, globals)
-    components = dotted_name.split('.')
+    components = dotted_name.split(".")
     for comp in components[1:]:
         mod = getattr(mod, comp)
     return mod
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/www/addMimeType.zpt` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/www/addMimeType.zpt`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,86 @@
 <h1 tal:replace="structure here/manage_page_header|nothing">Header</h1>
-<h2 tal:define="manage_tabs_message options/manage_tabs_message | nothing"
-    tal:replace="structure here/manage_tabs">Tabs</h2>
+<h2 tal:define="
+      manage_tabs_message options/manage_tabs_message | nothing;
+    "
+    tal:replace="structure here/manage_tabs"
+>Tabs</h2>
 
 
-<form method="POST" action="manage_addMimeType"
-      tal:attributes="action string:${here/absolute_url}/manage_addMimeType;">
+<form action="manage_addMimeType"
+      method="POST"
+      tal:attributes="
+        action string:${here/absolute_url}/manage_addMimeType;
+      "
+>
   <div class="form-title">
     Add a new mime type
   </div>
 
-  <div tal:define="status python:request.get('portal_status', '')"
+  <div class="error"
+       tal:define="
+         status python:request.get('portal_status', '');
+       "
        tal:condition="status"
-       class="error"
        tal:content="status"
-       />
+  ></div>
 
   <table width="50%">
     <tr>
       <td class="form-label">Name</td>
       <td class="form-element">
         <input name="id"
-               tal:attributes="value python:request.get('id', '');"/>
+               tal:attributes="
+                 value python:request.get('id', '');
+               "
+        />
       </td>
-      </tr><tr>
+    </tr><tr>
       <td class="form-label">Icon path</td>
       <td class="form-element">
         <input name="icon_path"
-               tal:attributes="value python:request.get('icon_path', '');"/>
+               tal:attributes="
+                 value python:request.get('icon_path', '');
+               "
+        />
       </td>
-      </tr><tr>
+    </tr><tr>
       <td class="form-label">Binary?
       </td>
       <td class="form-element">
-        <input name="binary" type="checkbox"
-               tal:attributes="value python:request.get('binary', '');"/>
+        <input name="binary"
+               type="checkbox"
+               tal:attributes="
+                 value python:request.get('binary', '');
+               "
+        />
       </td>
-      </tr><tr>
+    </tr><tr>
       <td class="form-label">Mime-types
       </td>
       <td class="form-element">
         <textarea name="mimetypes:list"
-                  tal:content="python:request.get('mimetypes', '')"/>
+                  tal:content="python:request.get('mimetypes', '')"
+        ></textarea>
       </td>
-      </tr><tr>
+    </tr><tr>
       <td class="form-label">Extensions
       </td>
       <td class="form-element">
         <textarea name="extensions:list"
-                  tal:content="python:request.get('extensions', '')"/>
+                  tal:content="python:request.get('extensions', '')"
+        ></textarea>
       </td>
     </tr><tr>
       <td class="form-label">Globs
       </td>
       <td class="form-element">
         <textarea name="globs:list"
-                  tal:content="python:request.get('globs', '')"/>
+                  tal:content="python:request.get('globs', '')"
+        ></textarea>
       </td>
     </tr>
   </table>
 
   <input type="submit" />
 </form>
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/www/editMimeType.zpt` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/www/editMimeType.zpt`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,99 @@
 <h1 tal:replace="structure here/manage_page_header|nothing">Header</h1>
-<h2 tal:define="manage_tabs_message options/manage_tabs_message | nothing"
-    tal:replace="structure here/manage_tabs">Tabs</h2>
-
-
-<form method="POST" action=""
-      tal:attributes="action string:${here/absolute_url}/manage_editMimeType;"
-      tal:define="mt python:here.lookup(request.form.get('mt_name'))[0]">
+<h2 tal:define="
+      manage_tabs_message options/manage_tabs_message | nothing;
+    "
+    tal:replace="structure here/manage_tabs"
+>Tabs</h2>
+
+
+<form action=""
+      method="POST"
+      tal:define="
+        mt python:here.lookup(request.form.get('mt_name'))[0];
+      "
+      tal:attributes="
+        action string:${here/absolute_url}/manage_editMimeType;
+      "
+>
 
   <div class="form-title">
-    Edit mime type <b tal:content="mt/name"/>.
+    Edit mime type
+    <b tal:content="mt/name"></b>.
   </div>
 
-  <div tal:define="status python:request.get('portal_status', '')"
+  <div class="error"
+       tal:define="
+         status python:request.get('portal_status', '');
+       "
        tal:condition="status"
-       class="error"
        tal:content="status"
-       />
+  ></div>
 
-  <input type="hidden" name="name" tal:attributes="value request/mt_name"/>
+  <input name="name"
+         type="hidden"
+         tal:attributes="
+           value request/mt_name;
+         "
+  />
 
   <table width="50%">
     <tr>
       <td>Name</td>
       <td>
         <input name="new_name"
-               tal:attributes="value python:request.get('new_name', mt.name());"/>
+               tal:attributes="
+                 value python:request.get('new_name', mt.name());
+               "
+        />
       </td>
-      </tr><tr>
+    </tr><tr>
       <td>Icon path</td>
       <td>
         <input name="icon_path"
-               tal:attributes="value python:request.get('icon_path', mt.icon_path);"/>
+               tal:attributes="
+                 value python:request.get('icon_path', mt.icon_path);
+               "
+        />
       </td>
-      </tr><tr>
+    </tr><tr>
       <td>Binary?
       </td>
       <td>
-        <input name="binary" type="checkbox"
-               tal:attributes="checked python:request.get('binary', mt.binary) and 1 or 0;"/>
+        <input name="binary"
+               type="checkbox"
+               tal:attributes="
+                 checked python:request.get('binary', mt.binary) and 1 or 0;
+               "
+        />
       </td>
-      </tr><tr>
+    </tr><tr>
       <td>Mime-types
       </td>
       <td>
         <textarea name="mimetypes"
-                  tal:content="python:request.get('mimetypes', '\n'.join(mt.mimetypes))"/>
+                  tal:content="python:request.get('mimetypes', '\n'.join(mt.mimetypes))"
+        ></textarea>
       </td>
-      </tr><tr>
+    </tr><tr>
       <td>Extensions
       </td>
       <td>
         <textarea name="extensions"
-                  tal:content="python:request.get('extensions', '\n'.join(mt.extensions))"/>
+                  tal:content="python:request.get('extensions', '\n'.join(mt.extensions))"
+        ></textarea>
       </td>
-      </tr><tr>
+    </tr><tr>
       <td>Globs
       </td>
       <td>
         <textarea name="globs"
-                  tal:content="python:request.get('globs', '\n'.join(mt.globs))"/>
+                  tal:content="python:request.get('globs', '\n'.join(mt.globs))"
+        ></textarea>
       </td>
     </tr>
   </table>
 
-  <input type="submit"/>
+  <input type="submit" />
 </form>
 
 <tal:footer tal:replace="structure here/manage_page_footer|nothing">footer</tal:footer>
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products/MimetypesRegistry/www/listMimeTypes.zpt` & `Products.MimetypesRegistry-3.0.0/Products/MimetypesRegistry/www/listMimeTypes.zpt`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,92 @@
 <h1 tal:replace="structure here/manage_page_header|nothing">Header</h1>
-<h2 tal:define="manage_tabs_message options/manage_tabs_message | nothing"
-    tal:replace="structure here/manage_tabs">Tabs</h2>
-
-<tal:block tal:define="mimetypes here/list_mimetypes">
+<h2 tal:define="
+      manage_tabs_message options/manage_tabs_message | nothing;
+    "
+    tal:replace="structure here/manage_tabs"
+>Tabs</h2>
+
+<tal:block tal:define="
+             mimetypes here/list_mimetypes;
+           ">
 
   <div class="form-title">
-    Registered MIME types (<span tal:replace="python:len(mimetypes)"/>).
+    Registered MIME types (<span tal:replace="python:len(mimetypes)"></span>).
   </div>
 
   <div align="right">
-    <form method="POST" action="manage_addMimeTypeForm">
-      <input type="submit" value="Add a new MIME type"/>
+    <form action="manage_addMimeTypeForm"
+          method="POST"
+    >
+      <input type="submit"
+             value="Add a new MIME type"
+      />
     </form>
   </div>
 
-  <div tal:define="status python:request.get('portal_status', '')"
-       tal:condition="status" class="error"
-       tal:content="status" />
-
-  <form method="POST" action="manage_delObjects"
-        tal:define="dummy mimetypes/sort">
+  <div class="error"
+       tal:define="
+         status python:request.get('portal_status', '');
+       "
+       tal:condition="status"
+       tal:content="status"
+  ></div>
+
+  <form action="manage_delObjects"
+        method="POST"
+        tal:define="
+          dummy mimetypes/sort;
+        "
+  >
 
     <table width="90%">
       <tr class="form-label">
         <th colspan="3">Name</th>
         <th>Mime-types</th>
         <th>Extensions</th>
         <th>Globs</th>
         <th>Binary?</th>
       </tr>
 
-      <tr class="form-element" tal:repeat="mt_id mimetypes">
-        <tal:block tal:define="mt python:here.lookup(mt_id)[0];">
+      <tr class="form-element"
+          tal:repeat="mt_id mimetypes"
+      >
+        <tal:block tal:define="
+                     mt python:here.lookup(mt_id)[0];
+                   ">
           <td>
-            <input type="checkbox" name="ids:list"
-                   tal:attributes="value mt/normalized"/>
+            <input name="ids:list"
+                   type="checkbox"
+                   tal:attributes="
+                     value mt/normalized;
+                   "
+            />
           </td>
           <td>
-            <img tal:attributes="src string:${here/portal_url}/${mt/icon_path}"/>
+            <img tal:attributes="
+                   src string:${here/portal_url}/${mt/icon_path};
+                 " />
           </td>
           <td>
             <a tal:content="mt/name"
-               tal:attributes="href string:${here/absolute_url}/manage_editMimeTypeForm?mt_name=${mt/urlsafe}"/>
+               tal:attributes="
+                 href string:${here/absolute_url}/manage_editMimeTypeForm?mt_name=${mt/urlsafe};
+               "
+            ></a>
           </td>
-          <td tal:content="python:', '.join(mt.mimetypes)"/>
-          <td tal:content="python:', '.join(mt.extensions)"/>
-          <td tal:content="python:', '.join(mt.globs)"/>
-          <td tal:content="python: mt.binary and 'yes' or 'no'"/>
+          <td tal:content="python:', '.join(mt.mimetypes)"></td>
+          <td tal:content="python:', '.join(mt.extensions)"></td>
+          <td tal:content="python:', '.join(mt.globs)"></td>
+          <td tal:content="python: mt.binary and 'yes' or 'no'"></td>
         </tal:block>
       </tr>
     </table>
 
-    <input type="submit" value="Delete Selected Items" />
+    <input type="submit"
+           value="Delete Selected Items"
+    />
 
   </form>
 
 </tal:block>
 
 <tal:footer tal:replace="structure here/manage_page_footer|nothing">footer</tal:footer>
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products.MimetypesRegistry.egg-info/PKG-INFO` & `Products.MimetypesRegistry-3.0.0/Products.MimetypesRegistry.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: Products.MimetypesRegistry
-Version: 2.1.9
+Version: 3.0.0
 Summary: MIME type handling for Zope
 Home-page: https://pypi.org/project/Products.MimetypesRegistry
 Author: Benjamin Saller
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: Zope mimetype registry
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Zope2
-Classifier: Framework :: Zope :: 4
+Classifier: Framework :: Zope :: 5
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.1
-Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 
 ==================
 Mimetypes Registry
 ==================
 
 Provide a registry of mimetypes, accessible via the ``mimetypes_registry`` tool.
@@ -79,14 +77,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.0 (2023-04-19)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7 support.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5cc689e5)
+
+
 2.1.9 (2022-01-19)
 ------------------
 
 Bug fixes:
 
 
 - Fix missing comma in install_requires.
@@ -362,15 +377,15 @@
 - Compile the 750KiB freedesktop.org.xml file to a binary format which gets
   loaded on Zope startup instead of reparsing the XML file each time. If the
   modification time of the source xml file changes, the binary file is
   automatically recreated. If the binary file cannot be created the xml file
   is reparsed each time as before.
   [hannosch]
 
-- Change some mimetypes returnd by guessMime to match the mimetypes
+- Change some mimetypes returned by guessMime to match the mimetypes
   registered in mtr (from freedesktop.org's mime database).
   [csenger]
 
 - Ensure that lookup doesn't return an empty tuple if asked with a
   mimetypestring returned by guessMime.
   Fixes http://dev.plone.org/plone/ticket/7876
   [csenger]
@@ -567,15 +582,15 @@
 
 - after one night sleeping over it I removed the yesterday added method.
   therefore I added according to some heuristics and OOo-Documentation
   some magic bytes to magic.py and made better tests.
   [yenzenz]
 
 - added a method to detect mimetypes of zipped files,
-  here specialy for OOo now all Openofice files and zip
+  here specially for OOo now all Openoffice files and zip
   files are detected properly.  my simple tests are working:
   a OOo-Writer and a simpe zipfile are detected.
   [yenzenz]
 
 - updated freedesktop.org.xml file to latest CVS version rev 1.57 from
   http://cvs.freedesktop.org/mime/shared-mime-info/freedesktop.org.xml
   [yenzenz]
@@ -673,32 +688,30 @@
 
 1.3.1-1 (2004-08-16)
 --------------------
 
 - Added text/x-html-safe mime type for new transformation
   [tiran]
 
-- Don't return acquisition wrapped mimetype items beause they may lead to
+- Don't return acquisition wrapped mimetype items because they may lead to
   memory leaks.
   [tiran]
 
 
 1.3.0-3 (2004-08-06)
 --------------------
 
 - Added text/wiki mime type
   [tiran]
 
-- Don't log redefine warning if the currrent and the new object are equal
+- Don't log redefine warning if the current and the new object are equal
   [tiran]
 
 - initialize() MTR on __setstate__ aka when the MTR is loaded from ZODB.
   [tiran]
 
 
 1.3.0-2 (2004-07-29)
 --------------------
 
 - Changed version to stick to Archetypes version.
   [tiran]
-
-
```

### Comparing `Products.MimetypesRegistry-2.1.9/Products.MimetypesRegistry.egg-info/SOURCES.txt` & `Products.MimetypesRegistry-3.0.0/Products.MimetypesRegistry.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+.editorconfig
 .gitignore
+.meta.toml
+.pre-commit-config.yaml
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
-bootstrap.py
 buildout.cfg
 pyproject.toml
 setup.cfg
 setup.py
+tox.ini
 Products/__init__.py
 Products.MimetypesRegistry.egg-info/PKG-INFO
 Products.MimetypesRegistry.egg-info/SOURCES.txt
 Products.MimetypesRegistry.egg-info/dependency_links.txt
 Products.MimetypesRegistry.egg-info/namespace_packages.txt
 Products.MimetypesRegistry.egg-info/not-zip-safe
 Products.MimetypesRegistry.egg-info/requires.txt
```

### Comparing `Products.MimetypesRegistry-2.1.9/README.rst` & `Products.MimetypesRegistry-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/docs/LICENSE.txt` & `Products.MimetypesRegistry-3.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.MimetypesRegistry-2.1.9/setup.py` & `Products.MimetypesRegistry-3.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,47 @@
-# -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
-version = '2.1.9'
+
+version = "3.0.0"
 
 setup(
-    name='Products.MimetypesRegistry',
+    name="Products.MimetypesRegistry",
     version=version,
     description="MIME type handling for Zope",
-    long_description=open("README.rst").read() + "\n" +
-    open("CHANGES.rst").read(),
+    long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
-        "Framework :: Zope2",
-        "Framework :: Zope :: 4",
+        "Framework :: Zope :: 5",
         "Operating System :: OS Independent",
         "Framework :: Plone",
-        "Framework :: Plone :: 5.1",
-        "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    keywords='Zope mimetype registry',
-    author='Benjamin Saller',
-    author_email='plone-developers@lists.sourceforge.net',
-    url='https://pypi.org/project/Products.MimetypesRegistry',
+    keywords="Zope mimetype registry",
+    author="Benjamin Saller",
+    author_email="plone-developers@lists.sourceforge.net",
+    url="https://pypi.org/project/Products.MimetypesRegistry",
     packages=find_packages(),
-    namespace_packages=['Products'],
+    namespace_packages=["Products"],
     include_package_data=True,
-    license='GPL',
+    license="GPL",
     zip_safe=False,
+    python_requires=">=3.8",
     install_requires=[
-        'AccessControl>=3.0.0',
-        'Acquisition',
-        'Products.CMFCore',
-        'setuptools',
-        'six',
-        'zope.contenttype',
-        'zope.deferredimport',
-        'zope.interface',
-        'Zope2',
+        "Products.CMFCore",
+        "setuptools",
+        'pywin32 ; platform_system=="Windows"',
     ],
     extras_require=dict(
         test=[
-            'plone.app.testing',
+            "plone.app.contenttypes[test]",
+            "plone.app.testing",
         ]
     ),
 )
```

