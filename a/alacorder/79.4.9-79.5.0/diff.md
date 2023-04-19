# Comparing `tmp/alacorder-79.4.9.tar.gz` & `tmp/alacorder-79.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-79.4.9.tar", max compression
+gzip compressed data, was "alacorder-79.5.0.tar", max compression
```

## Comparing `alacorder-79.4.9.tar` & `alacorder-79.5.0.tar`

### file list

```diff
@@ -1,14 +1,2046 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.4.9/LICENSE
--rw-r--r--   0        0        0     9974 2023-04-17 22:44:04.290109 alacorder-79.4.9/README.md
--rw-r--r--   0        0        0      682 2023-04-19 14:02:13.451687 alacorder-79.4.9/pyproject.toml
--rw-r--r--   0        0        0       72 2023-04-18 00:34:28.695299 alacorder-79.4.9/src/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.4.9/src/alacorder/.python-version
--rw-r--r--   0        0        0     2129 2023-03-28 18:45:29.612372 alacorder-79.4.9/src/alacorder/__init__.py
--rw-r--r--   0        0        0   134243 2023-04-19 13:59:38.511149 alacorder-79.4.9/src/alacorder/__main__.py
--rw-r--r--   0        0        0   134243 2023-04-19 13:59:21.516930 alacorder-79.4.9/src/alacorder/alac.py
--rw-r--r--   0        0        0   125941 2023-04-19 13:57:31.016776 alacorder-79.4.9/src/alacorder/graphical.py
--rw-r--r--   0        0        0    53236 2023-03-30 00:46:11.281022 alacorder-79.4.9/src/alacorder/img/alac.icns
--rw-r--r--   0        0        0    99678 2023-04-17 22:01:20.160909 alacorder-79.4.9/src/alacorder/img/alac.ico
--rw-r--r--   0        0        0     8334 2023-03-23 21:38:13.000000 alacorder-79.4.9/src/alacorder/img/alac.png
--rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.4.9/src/alacorder/~$E 302 Portfolio.docx
--rw-r--r--   0        0        0    10865 1970-01-01 00:00:00.000000 alacorder-79.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.5.0/LICENSE
+-rw-r--r--   0        0        0     9558 2023-04-19 15:07:38.263494 alacorder-79.5.0/README.md
+-rw-r--r--   0        0        0      682 2023-04-19 15:08:39.150315 alacorder-79.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-04-19 14:19:04.865786 alacorder-79.5.0/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0       72 2023-04-18 00:34:28.695299 alacorder-79.5.0/src/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0       34 2023-03-05 14:00:04.569426 alacorder-79.5.0/src/alacorder/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0        2 2023-03-05 14:01:12.571838 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0     1644 2023-03-05 13:59:58.452012 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/__init__.data.json
+-rw-r--r--   0        0        0     1634 2023-03-05 13:59:58.452197 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/__init__.meta.json
+-rw-r--r--   0        0        0     5613 2023-03-05 13:59:58.280947 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/autocall.data.json
+-rw-r--r--   0        0        0     1646 2023-03-05 13:59:58.281136 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/autocall.meta.json
+-rw-r--r--   0        0        0     8457 2023-03-05 13:59:59.353879 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/compilerop.data.json
+-rw-r--r--   0        0        0     1963 2023-03-05 13:59:59.354124 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/compilerop.meta.json
+-rw-r--r--   0        0        0     5511 2023-03-05 13:59:58.279859 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/error.data.json
+-rw-r--r--   0        0        0     1640 2023-03-05 13:59:58.280044 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/error.meta.json
+-rw-r--r--   0        0        0     7827 2023-03-05 13:59:58.278917 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/events.data.json
+-rw-r--r--   0        0        0     1679 2023-03-05 13:59:58.279120 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/events.meta.json
+-rw-r--r--   0        0        0     2130 2023-03-05 13:59:59.301267 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/excolors.data.json
+-rw-r--r--   0        0        0     1717 2023-03-05 13:59:59.301455 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/excolors.meta.json
+-rw-r--r--   0        0        0   125581 2023-03-05 13:59:59.283375 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/guarded_eval.data.json
+-rw-r--r--   0        0        0     2044 2023-03-05 13:59:59.283667 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/guarded_eval.meta.json
+-rw-r--r--   0        0        0    40463 2023-03-05 13:59:59.351233 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/inputtransformer2.data.json
+-rw-r--r--   0        0        0     1899 2023-03-05 13:59:59.351509 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/inputtransformer2.meta.json
+-rw-r--r--   0        0        0     2147 2023-03-05 13:59:58.056608 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/latex_symbols.data.json
+-rw-r--r--   0        0        0     1684 2023-03-05 13:59:58.056811 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/latex_symbols.meta.json
+-rw-r--r--   0        0        0     8873 2023-03-05 13:59:59.001609 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/logger.data.json
+-rw-r--r--   0        0        0     1857 2023-03-05 13:59:59.001806 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/logger.meta.json
+-rw-r--r--   0        0        0     4153 2023-03-05 14:00:01.011324 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/macro.data.json
+-rw-r--r--   0        0        0     1829 2023-03-05 14:00:01.011519 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/macro.meta.json
+-rw-r--r--   0        0        0    18119 2023-03-05 14:00:02.229094 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/magic_arguments.data.json
+-rw-r--r--   0        0        0     2048 2023-03-05 14:00:02.229315 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/magic_arguments.meta.json
+-rw-r--r--   0        0        0     5662 2023-03-05 13:59:58.454597 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/release.data.json
+-rw-r--r--   0        0        0     1709 2023-03-05 13:59:58.454783 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/release.meta.json
+-rw-r--r--   0        0        0     6331 2023-03-05 14:00:01.095908 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/splitinput.data.json
+-rw-r--r--   0        0        0     1836 2023-03-05 14:00:01.096145 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/splitinput.meta.json
+-rw-r--r--   0        0        0     3171 2023-03-05 13:59:58.998590 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/usage.data.json
+-rw-r--r--   0        0        0     1740 2023-03-05 13:59:58.998775 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/core/usage.meta.json
+-rw-r--r--   0        0        0     1692 2023-03-05 13:59:58.039131 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/extensions/__init__.data.json
+-rw-r--r--   0        0        0     1647 2023-03-05 13:59:58.039362 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/extensions/__init__.meta.json
+-rw-r--r--   0        0        0     2227 2023-03-05 13:59:57.904855 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/external/__init__.data.json
+-rw-r--r--   0        0        0     1643 2023-03-05 13:59:57.905037 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/external/__init__.meta.json
+-rw-r--r--   0        0        0     6086 2023-03-05 13:59:59.519735 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/external/qt_for_kernel.data.json
+-rw-r--r--   0        0        0     1796 2023-03-05 13:59:59.519930 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/external/qt_for_kernel.meta.json
+-rw-r--r--   0        0        0    10006 2023-03-05 13:59:59.195867 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/external/qt_loaders.data.json
+-rw-r--r--   0        0        0     2009 2023-03-05 13:59:59.196114 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/external/qt_loaders.meta.json
+-rw-r--r--   0        0        0     1636 2023-03-05 13:59:58.442799 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/lib/__init__.data.json
+-rw-r--r--   0        0        0     1634 2023-03-05 13:59:58.443014 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/lib/__init__.meta.json
+-rw-r--r--   0        0        0    47979 2023-03-05 14:00:01.117977 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/lib/pretty.data.json
+-rw-r--r--   0        0        0     2116 2023-03-05 14:00:01.118304 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/lib/pretty.meta.json
+-rw-r--r--   0        0        0     1676 2023-03-05 13:59:58.282327 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/terminal/__init__.data.json
+-rw-r--r--   0        0        0     1642 2023-03-05 13:59:58.282506 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/terminal/__init__.meta.json
+-rw-r--r--   0        0        0     5569 2023-03-05 13:59:59.557973 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/terminal/pt_inputhooks/__init__.data.json
+-rw-r--r--   0        0        0     1928 2023-03-05 13:59:59.558174 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/terminal/pt_inputhooks/__init__.meta.json
+-rw-r--r--   0        0        0    12623 2023-03-05 14:00:03.783050 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/terminal/shortcuts/auto_match.data.json
+-rw-r--r--   0        0        0     2034 2023-03-05 14:00:03.783307 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/terminal/shortcuts/auto_match.meta.json
+-rw-r--r--   0        0        0     2023 2023-03-05 13:59:58.245326 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/testing/__init__.data.json
+-rw-r--r--   0        0        0     1749 2023-03-05 13:59:58.245538 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1748 2023-03-05 13:59:58.449292 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/testing/skipdoctest.data.json
+-rw-r--r--   0        0        0     1657 2023-03-05 13:59:58.449470 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/testing/skipdoctest.meta.json
+-rw-r--r--   0        0        0     1652 2023-03-05 13:59:58.274389 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/__init__.data.json
+-rw-r--r--   0        0        0     1636 2023-03-05 13:59:58.274607 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/__init__.meta.json
+-rw-r--r--   0        0        0     3591 2023-03-05 14:00:01.093912 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/_process_common.data.json
+-rw-r--r--   0        0        0     1941 2023-03-05 14:00:01.094186 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/_process_common.meta.json
+-rw-r--r--   0        0        0     7627 2023-03-05 14:00:01.659307 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/_process_posix.data.json
+-rw-r--r--   0        0        0     1887 2023-03-05 14:00:01.659569 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/_process_posix.meta.json
+-rw-r--r--   0        0        0     1683 2023-03-05 13:59:58.258635 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/_sysinfo.data.json
+-rw-r--r--   0        0        0     1646 2023-03-05 13:59:58.258823 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/_sysinfo.meta.json
+-rw-r--r--   0        0        0    18814 2023-03-05 13:59:58.891307 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/coloransi.data.json
+-rw-r--r--   0        0        0     1762 2023-03-05 13:59:58.891503 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/coloransi.meta.json
+-rw-r--r--   0        0        0     4317 2023-03-05 13:59:59.237241 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/contexts.data.json
+-rw-r--r--   0        0        0     1667 2023-03-05 13:59:59.237463 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/contexts.meta.json
+-rw-r--r--   0        0        0     1918 2023-03-05 13:59:58.066456 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/data.data.json
+-rw-r--r--   0        0        0     1668 2023-03-05 13:59:58.066648 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/data.meta.json
+-rw-r--r--   0        0        0     3135 2023-03-05 13:59:58.997683 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/decorators.data.json
+-rw-r--r--   0        0        0     1681 2023-03-05 13:59:58.997882 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/decorators.meta.json
+-rw-r--r--   0        0        0     2353 2023-03-05 13:59:59.556053 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/dir2.data.json
+-rw-r--r--   0        0        0     1808 2023-03-05 13:59:59.556242 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/dir2.meta.json
+-rw-r--r--   0        0        0     1766 2023-03-05 13:59:58.057380 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/docs.data.json
+-rw-r--r--   0        0        0     1651 2023-03-05 13:59:58.057560 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/docs.meta.json
+-rw-r--r--   0        0        0     2580 2023-03-05 13:59:59.838183 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/encoding.data.json
+-rw-r--r--   0        0        0     1770 2023-03-05 13:59:59.838424 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/encoding.meta.json
+-rw-r--r--   0        0        0     2582 2023-03-05 13:59:58.453145 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/frame.data.json
+-rw-r--r--   0        0        0     1693 2023-03-05 13:59:58.453326 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/frame.meta.json
+-rw-r--r--   0        0        0     4323 2023-03-05 13:59:58.881791 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/generics.data.json
+-rw-r--r--   0        0        0     1717 2023-03-05 13:59:58.881975 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/generics.meta.json
+-rw-r--r--   0        0        0     1740 2023-03-05 13:59:58.073593 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/importstring.data.json
+-rw-r--r--   0        0        0     1692 2023-03-05 13:59:58.073833 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/importstring.meta.json
+-rw-r--r--   0        0        0     6937 2023-03-05 13:59:58.277130 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/ipstruct.data.json
+-rw-r--r--   0        0        0     1734 2023-03-05 13:59:58.277347 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/ipstruct.meta.json
+-rw-r--r--   0        0        0     1898 2023-03-05 13:59:57.949808 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/module_paths.data.json
+-rw-r--r--   0        0        0     1747 2023-03-05 13:59:57.950029 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/module_paths.meta.json
+-rw-r--r--   0        0        0     3830 2023-03-05 14:00:01.009760 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/openpy.data.json
+-rw-r--r--   0        0        0     1955 2023-03-05 14:00:01.009961 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/openpy.meta.json
+-rw-r--r--   0        0        0     8598 2023-03-05 14:00:02.234867 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/path.data.json
+-rw-r--r--   0        0        0     2148 2023-03-05 14:00:02.235174 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/path.meta.json
+-rw-r--r--   0        0        0     3779 2023-03-05 14:00:01.996773 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/process.data.json
+-rw-r--r--   0        0        0     1923 2023-03-05 14:00:01.997030 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/process.meta.json
+-rw-r--r--   0        0        0     5466 2023-03-05 14:00:01.068619 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/py3compat.data.json
+-rw-r--r--   0        0        0     1888 2023-03-05 14:00:01.068849 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/py3compat.meta.json
+-rw-r--r--   0        0        0     3293 2023-03-05 13:59:58.060565 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/sentinel.data.json
+-rw-r--r--   0        0        0     1712 2023-03-05 13:59:58.060758 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/sentinel.meta.json
+-rw-r--r--   0        0        0     3384 2023-03-05 14:00:01.070452 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/sysinfo.data.json
+-rw-r--r--   0        0        0     2010 2023-03-05 14:00:01.070681 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/sysinfo.meta.json
+-rw-r--r--   0        0        0     6168 2023-03-05 13:59:59.333192 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/syspathcontext.data.json
+-rw-r--r--   0        0        0     1764 2023-03-05 13:59:59.333391 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/syspathcontext.meta.json
+-rw-r--r--   0        0        0     5308 2023-03-05 13:59:59.300447 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/terminal.data.json
+-rw-r--r--   0        0        0     1782 2023-03-05 13:59:59.300650 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/terminal.meta.json
+-rw-r--r--   0        0        0    21454 2023-03-05 13:59:58.996542 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/text.data.json
+-rw-r--r--   0        0        0     1905 2023-03-05 13:59:58.996788 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/text.meta.json
+-rw-r--r--   0        0        0     3340 2023-03-05 13:59:58.685179 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/timing.data.json
+-rw-r--r--   0        0        0     1809 2023-03-05 13:59:58.685413 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/timing.meta.json
+-rw-r--r--   0        0        0    26574 2023-03-05 13:59:59.225546 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/tokenutil.data.json
+-rw-r--r--   0        0        0     1720 2023-03-05 13:59:59.225783 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/tokenutil.meta.json
+-rw-r--r--   0        0        0     4244 2023-03-05 13:59:59.786805 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/wildcard.data.json
+-rw-r--r--   0        0        0     1792 2023-03-05 13:59:59.787065 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/IPython/utils/wildcard.meta.json
+-rw-r--r--   0        0        0   128047 2023-03-05 14:01:08.842475 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PIL/Image.data.json
+-rw-r--r--   0        0        0     1842 2023-03-05 14:01:08.842682 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PIL/Image.meta.json
+-rw-r--r--   0        0        0    52687 2023-03-05 14:01:08.839752 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PIL/ImageFilter.data.json
+-rw-r--r--   0        0        0     1730 2023-03-05 14:01:08.839940 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PIL/ImageFilter.meta.json
+-rw-r--r--   0        0        0    12596 2023-03-05 14:01:08.838475 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PIL/ImagePalette.data.json
+-rw-r--r--   0        0        0     1679 2023-03-05 14:01:08.838688 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PIL/ImagePalette.meta.json
+-rw-r--r--   0        0        0    27729 2023-03-05 14:01:08.698509 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PIL/PyAccess.data.json
+-rw-r--r--   0        0        0     1651 2023-03-05 14:01:08.698765 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PIL/PyAccess.meta.json
+-rw-r--r--   0        0        0     2532 2023-03-05 14:01:08.401402 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PIL/__init__.data.json
+-rw-r--r--   0        0        0     1624 2023-03-05 14:01:08.401653 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PIL/__init__.meta.json
+-rw-r--r--   0        0        0     6092 2023-03-05 14:01:08.373559 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PIL/_imaging.data.json
+-rw-r--r--   0        0        0     1705 2023-03-05 14:01:08.373755 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PIL/_imaging.meta.json
+-rw-r--r--   0        0        0     3663 2023-03-05 14:00:03.804381 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/__init__.data.json
+-rw-r--r--   0        0        0     2032 2023-03-05 14:00:03.804640 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/__init__.meta.json
+-rw-r--r--   0        0        0    16555 2023-03-05 14:00:01.802605 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_cmap.data.json
+-rw-r--r--   0        0        0     2231 2023-03-05 14:00:01.802873 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_cmap.meta.json
+-rw-r--r--   0        0        0     7130 2023-03-05 13:59:58.957796 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/__init__.data.json
+-rw-r--r--   0        0        0     1893 2023-03-05 13:59:58.958696 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/__init__.meta.json
+-rw-r--r--   0        0        0     2406 2023-03-05 13:59:58.217308 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/adobe_glyphs.data.json
+-rw-r--r--   0        0        0     1688 2023-03-05 13:59:58.217624 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/adobe_glyphs.meta.json
+-rw-r--r--   0        0        0     1756 2023-03-05 13:59:57.991244 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/pdfdoc.data.json
+-rw-r--r--   0        0        0     1646 2023-03-05 13:59:57.991435 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/pdfdoc.meta.json
+-rw-r--r--   0        0        0     1723 2023-03-05 13:59:57.990191 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/std.data.json
+-rw-r--r--   0        0        0     1640 2023-03-05 13:59:57.990386 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/std.meta.json
+-rw-r--r--   0        0        0     1756 2023-03-05 13:59:57.989154 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/symbol.data.json
+-rw-r--r--   0        0        0     1646 2023-03-05 13:59:57.989354 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/symbol.meta.json
+-rw-r--r--   0        0        0     1778 2023-03-05 13:59:57.987988 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/zapfding.data.json
+-rw-r--r--   0        0        0     1650 2023-03-05 13:59:57.988213 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/zapfding.meta.json
+-rw-r--r--   0        0        0    60542 2023-03-05 14:00:01.856527 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_encryption.data.json
+-rw-r--r--   0        0        0     2287 2023-03-05 14:00:01.856829 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_encryption.meta.json
+-rw-r--r--   0        0        0    47002 2023-03-05 14:00:03.769631 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_merger.data.json
+-rw-r--r--   0        0        0     2431 2023-03-05 14:00:03.769906 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_merger.meta.json
+-rw-r--r--   0        0        0   111098 2023-03-05 14:00:02.127558 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_page.data.json
+-rw-r--r--   0        0        0     2322 2023-03-05 14:00:02.127913 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_page.meta.json
+-rw-r--r--   0        0        0    18237 2023-03-05 13:59:59.620861 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_protocols.data.json
+-rw-r--r--   0        0        0     1768 2023-03-05 13:59:59.621055 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_protocols.meta.json
+-rw-r--r--   0        0        0   129465 2023-03-05 14:00:02.323210 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_reader.data.json
+-rw-r--r--   0        0        0     2400 2023-03-05 14:00:02.323471 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_reader.meta.json
+-rw-r--r--   0        0        0     8690 2023-03-05 14:00:01.308344 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_security.data.json
+-rw-r--r--   0        0        0     1923 2023-03-05 14:01:09.662038 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_security.meta.json
+-rw-r--r--   0        0        0    38598 2023-03-05 13:59:59.430266 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_utils.data.json
+-rw-r--r--   0        0        0     2002 2023-03-05 13:59:59.430525 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_utils.meta.json
+-rw-r--r--   0        0        0     1642 2023-03-05 13:59:58.466457 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_version.data.json
+-rw-r--r--   0        0        0     1632 2023-03-05 13:59:58.466689 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_version.meta.json
+-rw-r--r--   0        0        0   157017 2023-03-05 14:00:02.554074 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_writer.data.json
+-rw-r--r--   0        0        0     2705 2023-03-05 14:00:02.554375 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/_writer.meta.json
+-rw-r--r--   0        0        0   110018 2023-03-05 13:59:58.372482 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/constants.data.json
+-rw-r--r--   0        0        0     1652 2023-03-05 13:59:58.372747 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/constants.meta.json
+-rw-r--r--   0        0        0    10374 2023-03-05 13:59:58.377723 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/errors.data.json
+-rw-r--r--   0        0        0     1629 2023-03-05 13:59:58.377918 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/errors.meta.json
+-rw-r--r--   0        0        0    40327 2023-03-05 14:00:01.311286 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/filters.data.json
+-rw-r--r--   0        0        0     2137 2023-03-05 14:01:09.664119 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/filters.meta.json
+-rw-r--r--   0        0        0    10470 2023-03-05 14:00:01.307705 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/__init__.data.json
+-rw-r--r--   0        0        0     2012 2023-03-05 14:01:09.661585 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/__init__.meta.json
+-rw-r--r--   0        0        0    17626 2023-03-05 14:00:01.306627 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_annotations.data.json
+-rw-r--r--   0        0        0     2033 2023-03-05 14:01:09.660779 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_annotations.meta.json
+-rw-r--r--   0        0        0    82838 2023-03-05 14:00:01.300337 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_base.data.json
+-rw-r--r--   0        0        0     2076 2023-03-05 14:01:09.655537 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_base.meta.json
+-rw-r--r--   0        0        0   137855 2023-03-05 14:00:01.303929 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_data_structures.data.json
+-rw-r--r--   0        0        0     2227 2023-03-05 14:01:09.658510 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_data_structures.meta.json
+-rw-r--r--   0        0        0    17997 2023-03-05 14:00:01.298271 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_fit.data.json
+-rw-r--r--   0        0        0     1849 2023-03-05 14:01:09.653675 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_fit.meta.json
+-rw-r--r--   0        0        0     6200 2023-03-05 14:00:01.305966 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_outline.data.json
+-rw-r--r--   0        0        0     1915 2023-03-05 14:01:09.660232 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_outline.meta.json
+-rw-r--r--   0        0        0    67789 2023-03-05 14:00:01.305519 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_rectangle.data.json
+-rw-r--r--   0        0        0     1970 2023-03-05 14:01:09.659875 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_rectangle.meta.json
+-rw-r--r--   0        0        0     7978 2023-03-05 14:00:01.300868 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_utils.data.json
+-rw-r--r--   0        0        0     2000 2023-03-05 14:01:09.655936 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_utils.meta.json
+-rw-r--r--   0        0        0    12082 2023-03-05 13:59:59.060467 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/pagerange.data.json
+-rw-r--r--   0        0        0     1786 2023-03-05 13:59:59.060677 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/pagerange.meta.json
+-rw-r--r--   0        0        0    28090 2023-03-05 13:59:58.465855 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/papersizes.data.json
+-rw-r--r--   0        0        0     1659 2023-03-05 13:59:58.466106 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/papersizes.meta.json
+-rw-r--r--   0        0        0     6989 2023-03-05 14:00:01.307091 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/types.data.json
+-rw-r--r--   0        0        0     1863 2023-03-05 14:01:09.661130 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/types.meta.json
+-rw-r--r--   0        0        0    49070 2023-03-05 14:00:01.309910 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/xmp.data.json
+-rw-r--r--   0        0        0     2224 2023-03-05 14:01:09.663164 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/PyPDF2/xmp.meta.json
+-rw-r--r--   0        0        0     8324 2023-03-05 13:59:58.305693 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/__future__.data.json
+-rw-r--r--   0        0        0     1672 2023-03-05 13:59:58.305888 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/__future__.meta.json
+-rw-r--r--   0        0        0   187134 2023-03-05 13:59:57.831848 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1760 2023-03-05 13:59:57.832039 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    46789 2023-03-05 13:59:57.865471 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_bisect.data.json
+-rw-r--r--   0        0        0     1697 2023-03-05 13:59:57.865738 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_bisect.meta.json
+-rw-r--r--   0        0        0   118849 2023-03-05 14:01:08.005896 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_cffi_backend/__init__.data.json
+-rw-r--r--   0        0        0     1812 2023-03-05 14:01:08.006147 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_cffi_backend/__init__.meta.json
+-rw-r--r--   0        0        0    55649 2023-03-05 13:59:57.828560 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1806 2023-03-05 13:59:57.828735 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    19484 2023-03-05 13:59:57.827285 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1714 2023-03-05 13:59:57.827448 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0    10601 2023-03-05 13:59:58.232432 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_compression.data.json
+-rw-r--r--   0        0        0     1769 2023-03-05 13:59:58.232699 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_compression.meta.json
+-rw-r--r--   0        0        0     3164 2023-03-05 13:59:57.826656 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1716 2023-03-05 13:59:57.826826 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0   229133 2023-03-05 13:59:57.968210 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_curses.data.json
+-rw-r--r--   0        0        0     1700 2023-03-05 13:59:57.968444 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_curses.meta.json
+-rw-r--r--   0        0        0   179168 2023-03-05 13:59:58.953707 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_decimal.data.json
+-rw-r--r--   0        0        0     1760 2023-03-05 13:59:58.954252 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_decimal.meta.json
+-rw-r--r--   0        0        0     7486 2023-03-05 13:59:57.856523 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_heapq.data.json
+-rw-r--r--   0        0        0     1636 2023-03-05 13:59:57.856704 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_heapq.meta.json
+-rw-r--r--   0        0        0     7846 2023-03-05 14:01:07.967582 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_markupbase.data.json
+-rw-r--r--   0        0        0     1680 2023-03-05 14:01:07.967795 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_markupbase.meta.json
+-rw-r--r--   0        0        0   118876 2023-03-05 13:59:58.105862 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_operator.data.json
+-rw-r--r--   0        0        0     1728 2023-03-05 13:59:58.106095 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_operator.meta.json
+-rw-r--r--   0        0        0     6391 2023-03-05 13:59:58.218933 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_random.data.json
+-rw-r--r--   0        0        0     1666 2023-03-05 13:59:58.219140 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_random.meta.json
+-rw-r--r--   0        0        0    97227 2023-03-05 13:59:58.012662 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_socket.data.json
+-rw-r--r--   0        0        0     1790 2023-03-05 13:59:58.012945 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_socket.meta.json
+-rw-r--r--   0        0        0    21142 2023-03-05 13:59:58.108166 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_stat.data.json
+-rw-r--r--   0        0        0     1677 2023-03-05 13:59:58.108361 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_stat.meta.json
+-rw-r--r--   0        0        0    25260 2023-03-05 13:59:58.323974 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_thread.data.json
+-rw-r--r--   0        0        0     1758 2023-03-05 13:59:58.324187 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_thread.meta.json
+-rw-r--r--   0        0        0    24127 2023-03-05 13:59:57.898533 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_tkinter.data.json
+-rw-r--r--   0        0        0     1702 2023-03-05 13:59:57.898755 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_tkinter.meta.json
+-rw-r--r--   0        0        0    92889 2023-03-05 13:59:57.826277 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1816 2023-03-05 13:59:57.826453 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0     5193 2023-03-05 13:59:58.014809 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_typeshed/xml.data.json
+-rw-r--r--   0        0        0     1650 2023-03-05 13:59:58.014999 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_typeshed/xml.meta.json
+-rw-r--r--   0        0        0    14158 2023-03-05 13:59:58.467877 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_warnings.data.json
+-rw-r--r--   0        0        0     1643 2023-03-05 13:59:58.468119 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_warnings.meta.json
+-rw-r--r--   0        0        0    28348 2023-03-05 13:59:57.999179 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_weakref.data.json
+-rw-r--r--   0        0        0     1741 2023-03-05 13:59:57.999473 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_weakref.meta.json
+-rw-r--r--   0        0        0    47160 2023-03-05 13:59:57.996138 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_weakrefset.data.json
+-rw-r--r--   0        0        0     1720 2023-03-05 13:59:57.996398 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_weakrefset.meta.json
+-rw-r--r--   0        0        0  3518265 2023-03-05 14:01:08.336557 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_win32typing/__init__.data.json
+-rw-r--r--   0        0        0     1716 2023-03-05 14:01:08.338044 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_win32typing/__init__.meta.json
+-rw-r--r--   0        0        0     2474 2023-03-05 13:59:58.018204 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_winapi.data.json
+-rw-r--r--   0        0        0     1724 2023-03-05 13:59:58.018402 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/_winapi.meta.json
+-rw-r--r--   0        0        0    21701 2023-03-05 13:59:57.824456 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1702 2023-03-05 13:59:57.824620 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0     1603 2023-03-05 13:59:58.496383 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/alacorder/__init__.data.json
+-rw-r--r--   0        0        0     1612 2023-03-05 13:59:58.496584 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/alacorder/__init__.meta.json
+-rw-r--r--   0        0        0   160642 2023-03-05 13:59:58.089168 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/argparse.data.json
+-rw-r--r--   0        0        0     1805 2023-03-05 13:59:58.089405 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/argparse.meta.json
+-rw-r--r--   0        0        0    62957 2023-03-05 13:59:57.823739 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1769 2023-03-05 13:59:57.823915 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0   143777 2023-03-05 13:59:58.304301 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ast.data.json
+-rw-r--r--   0        0        0     1824 2023-03-05 13:59:58.304542 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ast.meta.json
+-rw-r--r--   0        0        0     2505 2023-03-05 13:59:59.518098 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asttokens/__init__.data.json
+-rw-r--r--   0        0        0     1742 2023-03-05 14:01:09.924200 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asttokens/__init__.meta.json
+-rw-r--r--   0        0        0     2629 2023-03-05 13:59:57.867688 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asttokens/astroid_compat.data.json
+-rw-r--r--   0        0        0     1719 2023-03-05 13:59:57.867994 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asttokens/astroid_compat.meta.json
+-rw-r--r--   0        0        0    40307 2023-03-05 14:01:09.922135 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asttokens/asttokens.data.json
+-rw-r--r--   0        0        0     1946 2023-03-05 14:01:09.922417 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asttokens/asttokens.meta.json
+-rw-r--r--   0        0        0     7295 2023-03-05 13:59:59.117429 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asttokens/line_numbers.data.json
+-rw-r--r--   0        0        0     1733 2023-03-05 13:59:59.117640 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asttokens/line_numbers.meta.json
+-rw-r--r--   0        0        0    59837 2023-03-05 14:01:09.923698 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asttokens/mark_tokens.data.json
+-rw-r--r--   0        0        0     1982 2023-03-05 14:01:09.923926 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asttokens/mark_tokens.meta.json
+-rw-r--r--   0        0        0    64194 2023-03-05 14:01:09.853286 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asttokens/util.data.json
+-rw-r--r--   0        0        0     1899 2023-03-05 14:01:09.853582 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asttokens/util.meta.json
+-rw-r--r--   0        0        0    11557 2023-03-05 14:00:01.723452 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/__init__.data.json
+-rw-r--r--   0        0        0     2131 2023-03-05 14:00:01.723621 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/__init__.meta.json
+-rw-r--r--   0        0        0   106328 2023-03-05 14:00:01.719298 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/base_events.data.json
+-rw-r--r--   0        0        0     2078 2023-03-05 14:00:01.719499 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/base_events.meta.json
+-rw-r--r--   0        0        0    27410 2023-03-05 13:59:57.972499 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/coroutines.data.json
+-rw-r--r--   0        0        0     1747 2023-03-05 13:59:57.972738 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/coroutines.meta.json
+-rw-r--r--   0        0        0   205966 2023-03-05 14:00:01.717080 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/events.data.json
+-rw-r--r--   0        0        0     2103 2023-03-05 14:00:01.717296 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/events.meta.json
+-rw-r--r--   0        0        0     9353 2023-03-05 13:59:57.970739 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/exceptions.data.json
+-rw-r--r--   0        0        0     1696 2023-03-05 13:59:57.970980 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/exceptions.meta.json
+-rw-r--r--   0        0        0    35869 2023-03-05 14:00:01.713303 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/futures.data.json
+-rw-r--r--   0        0        0     1935 2023-03-05 14:00:01.713480 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/futures.meta.json
+-rw-r--r--   0        0        0    28341 2023-03-05 14:00:01.722192 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/locks.data.json
+-rw-r--r--   0        0        0     1887 2023-03-05 14:00:01.722368 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/locks.meta.json
+-rw-r--r--   0        0        0    17902 2023-03-05 14:00:01.707576 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/protocols.data.json
+-rw-r--r--   0        0        0     1839 2023-03-05 14:00:01.707769 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/protocols.meta.json
+-rw-r--r--   0        0        0    24473 2023-03-05 14:00:01.721409 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/queues.data.json
+-rw-r--r--   0        0        0     1775 2023-03-05 14:00:01.721572 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/queues.meta.json
+-rw-r--r--   0        0        0     4869 2023-03-05 14:00:01.720687 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/runners.data.json
+-rw-r--r--   0        0        0     1834 2023-03-05 14:00:01.720854 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/runners.meta.json
+-rw-r--r--   0        0        0     4031 2023-03-05 14:00:01.706839 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/selector_events.data.json
+-rw-r--r--   0        0        0     1813 2023-03-05 14:00:01.707081 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/selector_events.meta.json
+-rw-r--r--   0        0        0    36391 2023-03-05 14:00:01.720269 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/streams.data.json
+-rw-r--r--   0        0        0     1932 2023-03-05 14:00:01.720454 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/streams.meta.json
+-rw-r--r--   0        0        0    25574 2023-03-05 14:00:01.722958 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/subprocess.data.json
+-rw-r--r--   0        0        0     1955 2023-03-05 14:00:01.723127 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/subprocess.meta.json
+-rw-r--r--   0        0        0   107924 2023-03-05 14:00:01.712343 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/tasks.data.json
+-rw-r--r--   0        0        0     1936 2023-03-05 14:00:01.712535 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/tasks.meta.json
+-rw-r--r--   0        0        0     6038 2023-03-05 13:59:57.969160 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/threads.data.json
+-rw-r--r--   0        0        0     1706 2023-03-05 13:59:57.969408 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/threads.meta.json
+-rw-r--r--   0        0        0    28479 2023-03-05 14:00:01.710003 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/transports.data.json
+-rw-r--r--   0        0        0     1802 2023-03-05 14:00:01.710201 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/transports.meta.json
+-rw-r--r--   0        0        0    59557 2023-03-05 14:00:01.709114 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/unix_events.data.json
+-rw-r--r--   0        0        0     1920 2023-03-05 14:00:01.709322 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/asyncio/unix_events.meta.json
+-rw-r--r--   0        0        0     8751 2023-03-05 13:59:58.283327 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/atexit.data.json
+-rw-r--r--   0        0        0     1688 2023-03-05 13:59:58.283513 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/atexit.meta.json
+-rw-r--r--   0        0        0    17174 2023-03-05 13:59:58.457152 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/base64.data.json
+-rw-r--r--   0        0        0     1735 2023-03-05 13:59:58.457346 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/base64.meta.json
+-rw-r--r--   0        0        0    52029 2023-03-05 13:59:58.273786 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/bdb.data.json
+-rw-r--r--   0        0        0     1731 2023-03-05 13:59:58.274025 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/bdb.meta.json
+-rw-r--r--   0        0        0    14694 2023-03-05 13:59:58.451493 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/binascii.data.json
+-rw-r--r--   0        0        0     1782 2023-03-05 13:59:58.451703 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/binascii.meta.json
+-rw-r--r--   0        0        0    12190 2023-03-05 13:59:58.599840 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/bisect.data.json
+-rw-r--r--   0        0        0     1673 2023-03-05 13:59:58.600034 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/bisect.meta.json
+-rw-r--r--   0        0        0  1077780 2023-03-05 13:59:57.851144 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1866 2023-03-05 13:59:57.851427 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0    20683 2023-03-05 13:59:58.047211 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cProfile.data.json
+-rw-r--r--   0        0        0     1772 2023-03-05 13:59:58.047411 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cProfile.meta.json
+-rw-r--r--   0        0        0     2485 2023-03-05 13:59:59.304339 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/certifi/__init__.data.json
+-rw-r--r--   0        0        0     1696 2023-03-05 13:59:59.304521 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/certifi/__init__.meta.json
+-rw-r--r--   0        0        0     3446 2023-03-05 13:59:58.850059 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/certifi/core.data.json
+-rw-r--r--   0        0        0     1829 2023-03-05 13:59:58.850253 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/certifi/core.meta.json
+-rw-r--r--   0        0        0     2991 2023-03-05 14:01:08.767965 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cffi/__init__.data.json
+-rw-r--r--   0        0        0     1665 2023-03-05 14:01:08.768157 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cffi/__init__.meta.json
+-rw-r--r--   0        0        0    56091 2023-03-05 14:01:08.631782 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cffi/api.data.json
+-rw-r--r--   0        0        0     1891 2023-03-05 14:01:08.632022 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cffi/api.meta.json
+-rw-r--r--   0        0        0     6206 2023-03-05 14:01:08.015940 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cffi/error.data.json
+-rw-r--r--   0        0        0     1630 2023-03-05 14:01:08.016136 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cffi/error.meta.json
+-rw-r--r--   0        0        0     8347 2023-03-05 14:00:01.655804 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/__init__.data.json
+-rw-r--r--   0        0        0     1887 2023-03-05 14:00:01.656014 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/__init__.meta.json
+-rw-r--r--   0        0        0    49662 2023-03-05 14:00:01.032459 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/_compat.data.json
+-rw-r--r--   0        0        0     1993 2023-03-05 14:00:01.032731 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/_compat.meta.json
+-rw-r--r--   0        0        0    47515 2023-03-05 14:00:01.642919 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     2248 2023-03-05 14:00:01.643116 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0     5636 2023-03-05 13:59:59.014629 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/_textwrap.data.json
+-rw-r--r--   0        0        0     1721 2023-03-05 13:59:59.014833 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/_textwrap.meta.json
+-rw-r--r--   0        0        0   191965 2023-03-05 14:00:01.652441 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/core.data.json
+-rw-r--r--   0        0        0     2284 2023-03-05 14:00:01.652858 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/core.meta.json
+-rw-r--r--   0        0        0    60810 2023-03-05 14:00:01.655239 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/decorators.data.json
+-rw-r--r--   0        0        0     1974 2023-03-05 14:00:01.655469 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/decorators.meta.json
+-rw-r--r--   0        0        0    28813 2023-03-05 14:00:01.641477 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/exceptions.data.json
+-rw-r--r--   0        0        0     1888 2023-03-05 14:00:01.641759 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/exceptions.meta.json
+-rw-r--r--   0        0        0    18459 2023-03-05 14:00:01.644756 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/formatting.data.json
+-rw-r--r--   0        0        0     1920 2023-03-05 14:00:01.645100 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/formatting.meta.json
+-rw-r--r--   0        0        0     7446 2023-03-05 14:00:01.639200 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/globals.data.json
+-rw-r--r--   0        0        0     1747 2023-03-05 14:00:01.639500 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/globals.meta.json
+-rw-r--r--   0        0        0    30316 2023-03-05 14:00:01.643880 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/parser.data.json
+-rw-r--r--   0        0        0     1920 2023-03-05 14:00:01.644179 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/parser.meta.json
+-rw-r--r--   0        0        0    35390 2023-03-05 14:00:01.653759 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1979 2023-03-05 14:00:01.654004 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    24909 2023-03-05 14:00:01.648012 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/termui.data.json
+-rw-r--r--   0        0        0     2111 2023-03-05 14:00:01.648211 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/termui.meta.json
+-rw-r--r--   0        0        0    85218 2023-03-05 14:00:01.647045 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/types.data.json
+-rw-r--r--   0        0        0     2133 2023-03-05 14:00:01.647300 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/types.meta.json
+-rw-r--r--   0        0        0    33709 2023-03-05 14:00:01.640325 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/utils.data.json
+-rw-r--r--   0        0        0     2054 2023-03-05 14:00:01.640513 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/click/utils.meta.json
+-rw-r--r--   0        0        0    21484 2023-03-05 13:59:58.017388 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cmd.data.json
+-rw-r--r--   0        0        0     1683 2023-03-05 13:59:58.017586 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cmd.meta.json
+-rw-r--r--   0        0        0   126779 2023-03-05 13:59:57.822325 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1806 2023-03-05 13:59:57.822511 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0     6009 2023-03-05 13:59:58.068498 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/codeop.data.json
+-rw-r--r--   0        0        0     1652 2023-03-05 13:59:58.068675 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/codeop.meta.json
+-rw-r--r--   0        0        0   390732 2023-03-05 13:59:57.819770 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1784 2023-03-05 13:59:57.819976 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4026 2023-03-05 13:59:57.813207 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1680 2023-03-05 13:59:57.813377 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0     2641 2023-03-05 14:01:08.704569 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/colorama/__init__.data.json
+-rw-r--r--   0        0        0     1717 2023-03-05 14:01:08.704770 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/colorama/__init__.meta.json
+-rw-r--r--   0        0        0    22050 2023-03-05 14:01:08.369752 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/colorama/ansi.data.json
+-rw-r--r--   0        0        0     1637 2023-03-05 14:01:08.369975 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/colorama/ansi.meta.json
+-rw-r--r--   0        0        0    24189 2023-03-05 14:01:08.367447 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/colorama/ansitowin32.data.json
+-rw-r--r--   0        0        0     1762 2023-03-05 14:01:08.367673 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/colorama/ansitowin32.meta.json
+-rw-r--r--   0        0        0     9594 2023-03-05 14:01:08.523769 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/colorama/initialise.data.json
+-rw-r--r--   0        0        0     1697 2023-03-05 14:01:08.524034 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/colorama/initialise.meta.json
+-rw-r--r--   0        0        0     8039 2023-03-05 13:59:57.901639 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/colorsys.data.json
+-rw-r--r--   0        0        0     1641 2023-03-05 13:59:57.901828 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/colorsys.meta.json
+-rw-r--r--   0        0        0     1649 2023-03-05 13:59:58.025966 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/concurrent/__init__.data.json
+-rw-r--r--   0        0        0     1652 2023-03-05 13:59:58.026146 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/concurrent/__init__.meta.json
+-rw-r--r--   0        0        0     4856 2023-03-05 14:00:01.090824 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/concurrent/futures/__init__.data.json
+-rw-r--r--   0        0        0     1860 2023-03-05 14:00:01.091018 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/concurrent/futures/__init__.meta.json
+-rw-r--r--   0        0        0    63653 2023-03-05 13:59:59.171016 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/concurrent/futures/_base.data.json
+-rw-r--r--   0        0        0     1810 2023-03-05 13:59:59.171238 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/concurrent/futures/_base.meta.json
+-rw-r--r--   0        0        0    63512 2023-03-05 14:00:00.941072 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/concurrent/futures/process.data.json
+-rw-r--r--   0        0        0     2103 2023-03-05 14:00:00.941334 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/concurrent/futures/process.meta.json
+-rw-r--r--   0        0        0    23356 2023-03-05 13:59:59.528953 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/concurrent/futures/thread.data.json
+-rw-r--r--   0        0        0     1904 2023-03-05 13:59:59.529163 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/concurrent/futures/thread.meta.json
+-rw-r--r--   0        0        0   127713 2023-03-05 13:59:57.986595 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/configparser.data.json
+-rw-r--r--   0        0        0     1760 2023-03-05 13:59:57.986858 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/configparser.meta.json
+-rw-r--r--   0        0        0   110453 2023-03-05 13:59:57.812787 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1744 2023-03-05 13:59:57.812965 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0    40461 2023-03-05 13:59:57.924454 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/contextvars.data.json
+-rw-r--r--   0        0        0     1748 2023-03-05 13:59:57.924673 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/contextvars.meta.json
+-rw-r--r--   0        0        0     5806 2023-03-05 13:59:58.443774 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/copy.data.json
+-rw-r--r--   0        0        0     1632 2023-03-05 13:59:58.443952 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/copy.meta.json
+-rw-r--r--   0        0        0    12928 2023-03-05 13:59:57.858215 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/copyreg.data.json
+-rw-r--r--   0        0        0     1710 2023-03-05 13:59:57.858433 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/copyreg.meta.json
+-rw-r--r--   0        0        0     2610 2023-03-05 14:01:08.012745 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/__about__.data.json
+-rw-r--r--   0        0        0     1647 2023-03-05 14:01:08.012971 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/__about__.meta.json
+-rw-r--r--   0        0        0     2805 2023-03-05 14:01:08.861411 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/__init__.data.json
+-rw-r--r--   0        0        0     1750 2023-03-05 14:01:08.861596 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/__init__.meta.json
+-rw-r--r--   0        0        0    16928 2023-03-05 14:01:09.048476 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/exceptions.data.json
+-rw-r--r--   0        0        0     1889 2023-03-05 14:01:09.048685 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/exceptions.meta.json
+-rw-r--r--   0        0        0     1700 2023-03-05 14:01:08.018727 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/__init__.data.json
+-rw-r--r--   0        0        0     1650 2023-03-05 14:01:08.018942 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/__init__.meta.json
+-rw-r--r--   0        0        0    45913 2023-03-05 14:01:09.434895 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/_oid.data.json
+-rw-r--r--   0        0        0     1827 2023-03-05 14:01:09.435068 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/_oid.meta.json
+-rw-r--r--   0        0        0     2542 2023-03-05 14:01:09.682929 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/__init__.data.json
+-rw-r--r--   0        0        0     1769 2023-03-05 14:01:09.683155 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/__init__.meta.json
+-rw-r--r--   0        0        0     2430 2023-03-05 14:01:09.473490 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/__init__.data.json
+-rw-r--r--   0        0        0     1738 2023-03-05 14:01:09.473662 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/__init__.meta.json
+-rw-r--r--   0        0        0    10998 2023-03-05 14:01:09.426640 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/aead.data.json
+-rw-r--r--   0        0        0     2190 2023-03-05 14:01:09.426835 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/aead.meta.json
+-rw-r--r--   0        0        0   163732 2023-03-05 14:01:09.472136 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/backend.data.json
+-rw-r--r--   0        0        0     4610 2023-03-05 14:01:09.472354 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/backend.meta.json
+-rw-r--r--   0        0        0    13025 2023-03-05 14:01:09.433928 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ciphers.data.json
+-rw-r--r--   0        0        0     2359 2023-03-05 14:01:09.434131 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ciphers.meta.json
+-rw-r--r--   0        0        0     8676 2023-03-05 14:01:09.433360 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/cmac.data.json
+-rw-r--r--   0        0        0     2221 2023-03-05 14:01:09.433539 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/cmac.meta.json
+-rw-r--r--   0        0        0    26433 2023-03-05 14:01:09.467844 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/dh.data.json
+-rw-r--r--   0        0        0     2232 2023-03-05 14:01:09.468029 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/dh.meta.json
+-rw-r--r--   0        0        0    25205 2023-03-05 14:01:09.467073 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/dsa.data.json
+-rw-r--r--   0        0        0     2382 2023-03-05 14:01:09.467260 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/dsa.meta.json
+-rw-r--r--   0        0        0    29434 2023-03-05 14:01:09.466334 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ec.data.json
+-rw-r--r--   0        0        0     2416 2023-03-05 14:01:09.466518 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ec.meta.json
+-rw-r--r--   0        0        0    13578 2023-03-05 14:01:09.465534 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ed25519.data.json
+-rw-r--r--   0        0        0     2269 2023-03-05 14:01:09.465717 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ed25519.meta.json
+-rw-r--r--   0        0        0    13642 2023-03-05 14:01:09.465001 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ed448.data.json
+-rw-r--r--   0        0        0     2263 2023-03-05 14:01:09.465178 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ed448.meta.json
+-rw-r--r--   0        0        0    12027 2023-03-05 14:01:09.432903 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/hashes.data.json
+-rw-r--r--   0        0        0     2069 2023-03-05 14:01:09.433073 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/hashes.meta.json
+-rw-r--r--   0        0        0     9895 2023-03-05 14:01:09.432374 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/hmac.data.json
+-rw-r--r--   0        0        0     2107 2023-03-05 14:01:09.432565 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/hmac.meta.json
+-rw-r--r--   0        0        0     7706 2023-03-05 14:01:09.425411 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/poly1305.data.json
+-rw-r--r--   0        0        0     2020 2023-03-05 14:01:09.425731 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/poly1305.meta.json
+-rw-r--r--   0        0        0    35099 2023-03-05 14:01:09.464445 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/rsa.data.json
+-rw-r--r--   0        0        0     2532 2023-03-05 14:01:09.464635 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/rsa.meta.json
+-rw-r--r--   0        0        0     4200 2023-03-05 14:01:09.436999 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/utils.data.json
+-rw-r--r--   0        0        0     2099 2023-03-05 14:01:09.437167 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/utils.meta.json
+-rw-r--r--   0        0        0    12785 2023-03-05 14:01:09.463484 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/x25519.data.json
+-rw-r--r--   0        0        0     2261 2023-03-05 14:01:09.463712 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/x25519.meta.json
+-rw-r--r--   0        0        0    12595 2023-03-05 14:01:09.462851 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/x448.data.json
+-rw-r--r--   0        0        0     2255 2023-03-05 14:01:09.463087 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/x448.meta.json
+-rw-r--r--   0        0        0     1772 2023-03-05 14:01:07.983955 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/__init__.data.json
+-rw-r--r--   0        0        0     1668 2023-03-05 14:01:07.984140 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/__init__.meta.json
+-rw-r--r--   0        0        0     2336 2023-03-05 14:01:07.976714 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_openssl.data.json
+-rw-r--r--   0        0        0     1678 2023-03-05 14:01:07.976898 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_openssl.meta.json
+-rw-r--r--   0        0        0    15743 2023-03-05 14:01:08.010886 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_rust/__init__.data.json
+-rw-r--r--   0        0        0     1681 2023-03-05 14:01:08.011125 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_rust/__init__.meta.json
+-rw-r--r--   0        0        0     6792 2023-03-05 14:01:08.011981 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_rust/asn1.data.json
+-rw-r--r--   0        0        0     1682 2023-03-05 14:01:08.012177 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_rust/asn1.meta.json
+-rw-r--r--   0        0        0    15180 2023-03-05 14:01:09.450682 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_rust/x509.data.json
+-rw-r--r--   0        0        0     2513 2023-03-05 14:01:09.450863 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_rust/x509.meta.json
+-rw-r--r--   0        0        0     1836 2023-03-05 14:01:08.009047 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/openssl/__init__.data.json
+-rw-r--r--   0        0        0     1684 2023-03-05 14:01:08.009237 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/openssl/__init__.meta.json
+-rw-r--r--   0        0        0    34261 2023-03-05 14:01:07.983431 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/openssl/_conditional.data.json
+-rw-r--r--   0        0        0     1703 2023-03-05 14:01:07.983638 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/openssl/_conditional.meta.json
+-rw-r--r--   0        0        0    38528 2023-03-05 14:01:09.049547 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/openssl/binding.data.json
+-rw-r--r--   0        0        0     1943 2023-03-05 14:01:09.049734 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/openssl/binding.meta.json
+-rw-r--r--   0        0        0     1788 2023-03-05 14:01:08.019263 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/__init__.data.json
+-rw-r--r--   0        0        0     1672 2023-03-05 14:01:08.019449 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/__init__.meta.json
+-rw-r--r--   0        0        0     3985 2023-03-05 14:01:08.018142 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/_asymmetric.data.json
+-rw-r--r--   0        0        0     1687 2023-03-05 14:01:08.018381 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/_asymmetric.meta.json
+-rw-r--r--   0        0        0     9970 2023-03-05 14:01:08.007693 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/_cipheralgorithm.data.json
+-rw-r--r--   0        0        0     1698 2023-03-05 14:01:08.007885 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/_cipheralgorithm.meta.json
+-rw-r--r--   0        0        0    31769 2023-03-05 14:01:09.435707 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/_serialization.data.json
+-rw-r--r--   0        0        0     1937 2023-03-05 14:01:09.435887 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/_serialization.meta.json
+-rw-r--r--   0        0        0     1876 2023-03-05 14:01:08.019767 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/__init__.data.json
+-rw-r--r--   0        0        0     1694 2023-03-05 14:01:08.019945 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/__init__.meta.json
+-rw-r--r--   0        0        0    50380 2023-03-05 14:01:09.441628 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/dh.data.json
+-rw-r--r--   0        0        0     2104 2023-03-05 14:01:09.441805 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/dh.meta.json
+-rw-r--r--   0        0        0    54550 2023-03-05 14:01:09.440514 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/dsa.data.json
+-rw-r--r--   0        0        0     2267 2023-03-05 14:01:09.440708 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/dsa.meta.json
+-rw-r--r--   0        0        0    99258 2023-03-05 14:01:09.444652 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/ec.data.json
+-rw-r--r--   0        0        0     2432 2023-03-05 14:01:09.444840 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/ec.meta.json
+-rw-r--r--   0        0        0    18398 2023-03-05 14:01:09.439356 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/ed25519.data.json
+-rw-r--r--   0        0        0     2018 2023-03-05 14:01:09.439535 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/ed25519.meta.json
+-rw-r--r--   0        0        0    17574 2023-03-05 14:01:09.438742 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/ed448.data.json
+-rw-r--r--   0        0        0     2014 2023-03-05 14:01:09.438924 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/ed448.meta.json
+-rw-r--r--   0        0        0    16939 2023-03-05 14:01:09.445678 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/padding.data.json
+-rw-r--r--   0        0        0     2083 2023-03-05 14:01:09.445856 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/padding.meta.json
+-rw-r--r--   0        0        0    57861 2023-03-05 14:01:09.442865 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/rsa.data.json
+-rw-r--r--   0        0        0     2338 2023-03-05 14:01:09.443052 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/rsa.meta.json
+-rw-r--r--   0        0        0     6470 2023-03-05 14:01:09.445076 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/types.data.json
+-rw-r--r--   0        0        0     2206 2023-03-05 14:01:09.445256 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/types.meta.json
+-rw-r--r--   0        0        0     7015 2023-03-05 14:01:09.436195 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/utils.data.json
+-rw-r--r--   0        0        0     1936 2023-03-05 14:01:09.436389 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/utils.meta.json
+-rw-r--r--   0        0        0    16229 2023-03-05 14:01:09.438144 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/x25519.data.json
+-rw-r--r--   0        0        0     2016 2023-03-05 14:01:09.438319 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/x25519.meta.json
+-rw-r--r--   0        0        0    15999 2023-03-05 14:01:09.437571 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/x448.data.json
+-rw-r--r--   0        0        0     2012 2023-03-05 14:01:09.437751 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/x448.meta.json
+-rw-r--r--   0        0        0     3339 2023-03-05 14:01:09.429469 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/__init__.data.json
+-rw-r--r--   0        0        0     1799 2023-03-05 14:01:09.429656 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/__init__.meta.json
+-rw-r--r--   0        0        0    34892 2023-03-05 14:01:09.473106 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/aead.data.json
+-rw-r--r--   0        0        0     2129 2023-03-05 14:01:09.473291 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/aead.meta.json
+-rw-r--r--   0        0        0    53114 2023-03-05 14:01:09.430611 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/algorithms.data.json
+-rw-r--r--   0        0        0     1888 2023-03-05 14:01:09.430791 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/algorithms.meta.json
+-rw-r--r--   0        0        0    45452 2023-03-05 14:01:09.427751 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/base.data.json
+-rw-r--r--   0        0        0     2102 2023-03-05 14:01:09.427958 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/base.meta.json
+-rw-r--r--   0        0        0    60656 2023-03-05 14:01:09.429052 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/modes.data.json
+-rw-r--r--   0        0        0     1978 2023-03-05 14:01:09.429246 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/modes.meta.json
+-rw-r--r--   0        0        0     2344 2023-03-05 14:01:08.466230 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/constant_time.data.json
+-rw-r--r--   0        0        0     1815 2023-03-05 14:01:08.466492 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/constant_time.meta.json
+-rw-r--r--   0        0        0    59362 2023-03-05 14:01:09.431847 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/hashes.data.json
+-rw-r--r--   0        0        0     2034 2023-03-05 14:01:09.432043 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/hashes.meta.json
+-rw-r--r--   0        0        0     5920 2023-03-05 14:01:08.008553 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/kdf/__init__.data.json
+-rw-r--r--   0        0        0     1680 2023-03-05 14:01:08.008735 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/kdf/__init__.meta.json
+-rw-r--r--   0        0        0     7520 2023-03-05 14:01:09.426074 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/kdf/scrypt.data.json
+-rw-r--r--   0        0        0     2086 2023-03-05 14:01:09.426274 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/kdf/scrypt.meta.json
+-rw-r--r--   0        0        0     4811 2023-03-05 14:01:09.446551 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/__init__.data.json
+-rw-r--r--   0        0        0     1875 2023-03-05 14:01:09.446719 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/__init__.meta.json
+-rw-r--r--   0        0        0     7669 2023-03-05 14:01:09.446161 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/base.data.json
+-rw-r--r--   0        0        0     2409 2023-03-05 14:01:09.446334 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/base.meta.json
+-rw-r--r--   0        0        0    29666 2023-03-05 14:01:09.468662 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/pkcs12.data.json
+-rw-r--r--   0        0        0     2765 2023-03-05 14:01:09.468851 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/pkcs12.meta.json
+-rw-r--r--   0        0        0    18012 2023-03-05 14:01:09.469291 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/pkcs7.data.json
+-rw-r--r--   0        0        0     2355 2023-03-05 14:01:09.469468 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/pkcs7.meta.json
+-rw-r--r--   0        0        0    58639 2023-03-05 14:01:09.447876 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/ssh.data.json
+-rw-r--r--   0        0        0     2731 2023-03-05 14:01:09.448118 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/ssh.meta.json
+-rw-r--r--   0        0        0    19736 2023-03-05 14:01:08.767315 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/utils.data.json
+-rw-r--r--   0        0        0     1818 2023-03-05 14:01:08.767545 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/utils.meta.json
+-rw-r--r--   0        0        0    32436 2023-03-05 14:01:09.462242 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/x509/__init__.data.json
+-rw-r--r--   0        0        0     2026 2023-03-05 14:01:09.462444 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/x509/__init__.meta.json
+-rw-r--r--   0        0        0   155738 2023-03-05 14:01:09.461305 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/x509/base.data.json
+-rw-r--r--   0        0        0     2926 2023-03-05 14:01:09.461587 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/x509/base.meta.json
+-rw-r--r--   0        0        0    21759 2023-03-05 14:01:09.450030 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/x509/certificate_transparency.data.json
+-rw-r--r--   0        0        0     2029 2023-03-05 14:01:09.450245 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/x509/certificate_transparency.meta.json
+-rw-r--r--   0        0        0   358332 2023-03-05 14:01:09.458363 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/x509/extensions.data.json
+-rw-r--r--   0        0        0     3049 2023-03-05 14:01:09.458636 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/x509/extensions.meta.json
+-rw-r--r--   0        0        0    50346 2023-03-05 14:01:09.451859 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/x509/general_name.data.json
+-rw-r--r--   0        0        0     2009 2023-03-05 14:01:09.452087 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/x509/general_name.meta.json
+-rw-r--r--   0        0        0    54874 2023-03-05 14:01:09.449251 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/x509/name.data.json
+-rw-r--r--   0        0        0     2145 2023-03-05 14:01:09.449503 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/x509/name.meta.json
+-rw-r--r--   0        0        0     3308 2023-03-05 14:01:09.436614 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/x509/oid.data.json
+-rw-r--r--   0        0        0     1679 2023-03-05 14:01:09.436779 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/cryptography/x509/oid.meta.json
+-rw-r--r--   0        0        0   135879 2023-03-05 13:59:57.810595 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1812 2023-03-05 13:59:57.810785 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     2191 2023-03-05 13:59:57.871488 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ctypes/util.data.json
+-rw-r--r--   0        0        0     1661 2023-03-05 13:59:57.871675 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ctypes/util.meta.json
+-rw-r--r--   0        0        0    58772 2023-03-05 13:59:58.031486 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ctypes/wintypes.data.json
+-rw-r--r--   0        0        0     1700 2023-03-05 13:59:58.031722 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ctypes/wintypes.meta.json
+-rw-r--r--   0        0        0    38052 2023-03-05 13:59:58.887995 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/curses/__init__.data.json
+-rw-r--r--   0        0        0     1728 2023-03-05 13:59:58.888181 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/curses/__init__.meta.json
+-rw-r--r--   0        0        0    58283 2023-03-05 13:59:58.223995 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1763 2023-03-05 13:59:58.224228 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0   147292 2023-03-05 13:59:59.087765 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/datetime.data.json
+-rw-r--r--   0        0        0     1715 2023-03-05 13:59:59.088038 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/datetime.meta.json
+-rw-r--r--   0        0        0     1618 2023-03-05 14:01:08.338993 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/__init__.data.json
+-rw-r--r--   0        0        0     1633 2023-03-05 14:01:08.339181 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/__init__.meta.json
+-rw-r--r--   0        0        0     6101 2023-03-05 14:01:08.017356 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/_common.data.json
+-rw-r--r--   0        0        0     1669 2023-03-05 14:01:08.017550 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/_common.meta.json
+-rw-r--r--   0        0        0    22099 2023-03-05 14:01:08.814783 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/parser/__init__.data.json
+-rw-r--r--   0        0        0     1754 2023-03-05 14:01:08.814989 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/parser/__init__.meta.json
+-rw-r--r--   0        0        0     8524 2023-03-05 14:01:08.663906 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/parser/isoparser.data.json
+-rw-r--r--   0        0        0     1724 2023-03-05 14:01:08.664101 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/parser/isoparser.meta.json
+-rw-r--r--   0        0        0    51946 2023-03-05 14:01:08.636450 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/relativedelta.data.json
+-rw-r--r--   0        0        0     1725 2023-03-05 14:01:08.636681 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/relativedelta.meta.json
+-rw-r--r--   0        0        0     2935 2023-03-05 14:01:08.873446 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/tz/__init__.data.json
+-rw-r--r--   0        0        0     1684 2023-03-05 14:01:08.873658 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/tz/__init__.meta.json
+-rw-r--r--   0        0        0    13570 2023-03-05 14:01:08.638422 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/tz/_common.data.json
+-rw-r--r--   0        0        0     1666 2023-03-05 14:01:08.638663 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/tz/_common.meta.json
+-rw-r--r--   0        0        0    51080 2023-03-05 14:01:08.779868 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/tz/tz.data.json
+-rw-r--r--   0        0        0     1764 2023-03-05 14:01:08.780089 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dateutil/tz/tz.meta.json
+-rw-r--r--   0        0        0     5285 2023-03-05 13:59:59.383634 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/decimal.data.json
+-rw-r--r--   0        0        0     1706 2023-03-05 13:59:59.383877 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/decimal.meta.json
+-rw-r--r--   0        0        0    40509 2023-03-05 14:01:08.819735 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/decorator/__init__.data.json
+-rw-r--r--   0        0        0     1753 2023-03-05 14:01:08.819935 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/decorator/__init__.meta.json
+-rw-r--r--   0        0        0    62436 2023-03-05 13:59:58.312278 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/difflib.data.json
+-rw-r--r--   0        0        0     1713 2023-03-05 13:59:58.312482 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/difflib.meta.json
+-rw-r--r--   0        0        0    43155 2023-03-05 13:59:59.064110 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dis.data.json
+-rw-r--r--   0        0        0     1748 2023-03-05 13:59:59.064310 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/dis.meta.json
+-rw-r--r--   0        0        0     1641 2023-03-05 14:01:08.006489 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/distutils/__init__.data.json
+-rw-r--r--   0        0        0     1650 2023-03-05 14:01:08.006668 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/distutils/__init__.meta.json
+-rw-r--r--   0        0        0    27630 2023-03-05 14:01:07.976084 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/distutils/cmd.data.json
+-rw-r--r--   0        0        0     1699 2023-03-05 14:01:07.976267 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/distutils/cmd.meta.json
+-rw-r--r--   0        0        0     7954 2023-03-05 14:01:08.473287 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/distutils/core.data.json
+-rw-r--r--   0        0        0     1754 2023-03-05 14:01:08.473527 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/distutils/core.meta.json
+-rw-r--r--   0        0        0    34337 2023-03-05 14:01:07.975204 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/distutils/dist.data.json
+-rw-r--r--   0        0        0     1733 2023-03-05 14:01:07.975416 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/distutils/dist.meta.json
+-rw-r--r--   0        0        0    10757 2023-03-05 14:01:07.969464 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/distutils/extension.data.json
+-rw-r--r--   0        0        0     1664 2023-03-05 14:01:07.969697 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/distutils/extension.meta.json
+-rw-r--r--   0        0        0    73895 2023-03-05 13:59:59.526681 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/doctest.data.json
+-rw-r--r--   0        0        0     1843 2023-03-05 13:59:59.526898 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/doctest.meta.json
+-rw-r--r--   0        0        0     8108 2023-03-05 13:59:57.807952 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1741 2023-03-05 13:59:57.808113 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    12835 2023-03-05 13:59:57.807504 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1677 2023-03-05 13:59:57.807665 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7695 2023-03-05 13:59:57.806939 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1712 2023-03-05 13:59:57.807109 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25479 2023-03-05 13:59:57.806486 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1684 2023-03-05 13:59:57.806658 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9685 2023-03-05 13:59:57.805802 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1697 2023-03-05 13:59:57.805965 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    62343 2023-03-05 13:59:57.805275 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1834 2023-03-05 13:59:57.805454 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0     1649 2023-03-05 14:01:07.968158 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/mime/__init__.data.json
+-rw-r--r--   0        0        0     1652 2023-03-05 14:01:07.968360 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/mime/__init__.meta.json
+-rw-r--r--   0        0        0     3908 2023-03-05 14:01:07.992693 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/mime/base.data.json
+-rw-r--r--   0        0        0     1716 2023-03-05 14:01:07.992881 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/mime/base.meta.json
+-rw-r--r--   0        0        0     4592 2023-03-05 14:01:08.472100 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/mime/multipart.data.json
+-rw-r--r--   0        0        0     1775 2023-03-05 14:01:08.472323 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/mime/multipart.meta.json
+-rw-r--r--   0        0        0     2864 2023-03-05 14:01:08.471177 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/mime/nonmultipart.data.json
+-rw-r--r--   0        0        0     1720 2023-03-05 14:01:08.471402 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/mime/nonmultipart.meta.json
+-rw-r--r--   0        0        0     3898 2023-03-05 14:01:08.623082 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/mime/text.data.json
+-rw-r--r--   0        0        0     1760 2023-03-05 14:01:08.623262 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/mime/text.meta.json
+-rw-r--r--   0        0        0    32684 2023-03-05 13:59:57.803873 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1770 2023-03-05 13:59:57.804041 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0    23686 2023-03-05 14:01:08.581687 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/utils.data.json
+-rw-r--r--   0        0        0     1765 2023-03-05 14:01:08.581929 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/email/utils.meta.json
+-rw-r--r--   0        0        0    64237 2023-03-05 13:59:57.802954 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1733 2023-03-05 13:59:57.803122 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    21224 2023-03-05 13:59:58.357164 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/errno.data.json
+-rw-r--r--   0        0        0     1695 2023-03-05 13:59:58.357363 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/errno.meta.json
+-rw-r--r--   0        0        0    23335 2023-03-05 14:00:00.934100 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/executing/__init__.data.json
+-rw-r--r--   0        0        0     1872 2023-03-05 14:00:00.934289 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/executing/__init__.meta.json
+-rw-r--r--   0        0        0    84326 2023-03-05 13:59:59.725613 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/executing/executing.data.json
+-rw-r--r--   0        0        0     2249 2023-03-05 14:01:10.042287 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/executing/executing.meta.json
+-rw-r--r--   0        0        0     1658 2023-03-05 13:59:57.866867 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/executing/version.data.json
+-rw-r--r--   0        0        0     1636 2023-03-05 13:59:57.867080 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/executing/version.meta.json
+-rw-r--r--   0        0        0     7252 2023-03-05 13:59:58.246579 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/faulthandler.data.json
+-rw-r--r--   0        0        0     1695 2023-03-05 13:59:58.246806 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/faulthandler.meta.json
+-rw-r--r--   0        0        0     6514 2023-03-05 13:59:57.947111 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/fnmatch.data.json
+-rw-r--r--   0        0        0     1663 2023-03-05 13:59:57.947347 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/fnmatch.meta.json
+-rw-r--r--   0        0        0    92861 2023-03-05 13:59:59.609574 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/fractions.data.json
+-rw-r--r--   0        0        0     1830 2023-03-05 13:59:59.609887 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/fractions.meta.json
+-rw-r--r--   0        0        0   136168 2023-03-05 13:59:58.354722 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/functools.data.json
+-rw-r--r--   0        0        0     1743 2023-03-05 13:59:58.354955 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/functools.meta.json
+-rw-r--r--   0        0        0    16854 2023-03-05 13:59:58.062662 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/gc.data.json
+-rw-r--r--   0        0        0     1715 2023-03-05 13:59:58.062847 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/gc.meta.json
+-rw-r--r--   0        0        0    23876 2023-03-05 13:59:57.801500 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1731 2023-03-05 13:59:57.801674 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0     6690 2023-03-05 13:59:58.067502 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/getopt.data.json
+-rw-r--r--   0        0        0     1637 2023-03-05 13:59:58.067669 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/getopt.meta.json
+-rw-r--r--   0        0        0     3943 2023-03-05 13:59:58.307135 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/getpass.data.json
+-rw-r--r--   0        0        0     1638 2023-03-05 13:59:58.307304 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/getpass.meta.json
+-rw-r--r--   0        0        0    54812 2023-03-05 13:59:58.346430 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/gettext.data.json
+-rw-r--r--   0        0        0     1737 2023-03-05 13:59:58.346668 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/gettext.meta.json
+-rw-r--r--   0        0        0    10067 2023-03-05 13:59:58.495045 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/glob.data.json
+-rw-r--r--   0        0        0     1691 2023-03-05 13:59:58.495234 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/glob.meta.json
+-rw-r--r--   0        0        0    48617 2023-03-05 13:59:59.048012 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/gzip.data.json
+-rw-r--r--   0        0        0     1821 2023-03-05 13:59:59.048253 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/gzip.meta.json
+-rw-r--r--   0        0        0    28879 2023-03-05 13:59:58.376289 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/hashlib.data.json
+-rw-r--r--   0        0        0     1789 2023-03-05 13:59:58.376552 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/hashlib.meta.json
+-rw-r--r--   0        0        0     9621 2023-03-05 13:59:58.584792 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/heapq.data.json
+-rw-r--r--   0        0        0     1694 2023-03-05 13:59:58.584989 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/heapq.meta.json
+-rw-r--r--   0        0        0    17881 2023-03-05 13:59:58.033717 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/hmac.data.json
+-rw-r--r--   0        0        0     1798 2023-03-05 13:59:58.033995 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/hmac.meta.json
+-rw-r--r--   0        0        0     4481 2023-03-05 13:59:58.448729 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/html/__init__.data.json
+-rw-r--r--   0        0        0     1641 2023-03-05 13:59:58.448910 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/html/__init__.meta.json
+-rw-r--r--   0        0        0     2943 2023-03-05 13:59:57.883399 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/html/entities.data.json
+-rw-r--r--   0        0        0     1651 2023-03-05 13:59:57.883568 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/html/entities.meta.json
+-rw-r--r--   0        0        0    20592 2023-03-05 14:01:08.470431 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/html/parser.data.json
+-rw-r--r--   0        0        0     1681 2023-03-05 14:01:08.470670 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/html/parser.meta.json
+-rw-r--r--   0        0        0    20890 2023-03-05 13:59:58.381953 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/http/__init__.data.json
+-rw-r--r--   0        0        0     1718 2023-03-05 13:59:58.382144 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/http/__init__.meta.json
+-rw-r--r--   0        0        0    69551 2023-03-05 13:59:59.627787 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/http/client.data.json
+-rw-r--r--   0        0        0     1949 2023-03-05 13:59:59.628007 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/http/client.meta.json
+-rw-r--r--   0        0        0    60806 2023-03-05 13:59:59.867388 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/http/cookiejar.data.json
+-rw-r--r--   0        0        0     1847 2023-03-05 13:59:59.867618 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/http/cookiejar.meta.json
+-rw-r--r--   0        0        0    42565 2023-03-05 14:01:07.991829 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/http/cookies.data.json
+-rw-r--r--   0        0        0     1750 2023-03-05 14:01:07.992031 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/http/cookies.meta.json
+-rw-r--r--   0        0        0    38023 2023-03-05 14:01:08.758264 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/http/server.data.json
+-rw-r--r--   0        0        0     1829 2023-03-05 14:01:08.758507 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/http/server.meta.json
+-rw-r--r--   0        0        0     6502 2023-03-05 13:59:57.800752 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1715 2023-03-05 13:59:57.800927 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    73157 2023-03-05 13:59:57.800308 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1863 2023-03-05 13:59:57.800480 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    68131 2023-03-05 13:59:57.798732 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1874 2023-03-05 13:59:57.798919 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    94672 2023-03-05 13:59:57.797237 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1852 2023-03-05 13:59:57.797433 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12472 2023-03-05 13:59:57.795341 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1697 2023-03-05 13:59:57.795510 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    11341 2023-03-05 13:59:57.912081 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/importlib/resources.data.json
+-rw-r--r--   0        0        0     1838 2023-03-05 13:59:57.912285 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/importlib/resources.meta.json
+-rw-r--r--   0        0        0    22985 2023-03-05 13:59:57.904132 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/importlib/util.data.json
+-rw-r--r--   0        0        0     1879 2023-03-05 13:59:57.904341 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/importlib/util.meta.json
+-rw-r--r--   0        0        0   364855 2023-03-05 13:59:59.484482 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/inspect.data.json
+-rw-r--r--   0        0        0     1841 2023-03-05 13:59:59.484779 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/inspect.meta.json
+-rw-r--r--   0        0        0    88656 2023-03-05 13:59:57.794721 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1825 2023-03-05 13:59:57.794907 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0   137068 2023-03-05 14:01:07.965983 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipaddress.data.json
+-rw-r--r--   0        0        0     1728 2023-03-05 14:01:07.966334 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipaddress.meta.json
+-rw-r--r--   0        0        0     7243 2023-03-05 13:59:58.608151 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/_eventloop_macos.data.json
+-rw-r--r--   0        0        0     1792 2023-03-05 13:59:58.608350 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/_eventloop_macos.meta.json
+-rw-r--r--   0        0        0     3748 2023-03-05 13:59:58.038467 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/_version.data.json
+-rw-r--r--   0        0        0     1764 2023-03-05 13:59:58.038724 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/_version.meta.json
+-rw-r--r--   0        0        0     4064 2023-03-05 14:00:03.792906 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/control.data.json
+-rw-r--r--   0        0        0     1899 2023-03-05 14:00:03.793098 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/control.meta.json
+-rw-r--r--   0        0        0     1652 2023-03-05 13:59:57.879119 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/gui/__init__.data.json
+-rw-r--r--   0        0        0     1638 2023-03-05 13:59:57.879301 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/gui/__init__.meta.json
+-rw-r--r--   0        0        0     5803 2023-03-05 13:59:59.163652 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/gui/gtk3embed.data.json
+-rw-r--r--   0        0        0     1854 2023-03-05 13:59:59.163854 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/gui/gtk3embed.meta.json
+-rw-r--r--   0        0        0     5459 2023-03-05 13:59:59.165063 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/gui/gtkembed.data.json
+-rw-r--r--   0        0        0     1882 2023-03-05 13:59:59.165335 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/gui/gtkembed.meta.json
+-rw-r--r--   0        0        0     6733 2023-03-05 14:00:01.135726 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/heartbeat.data.json
+-rw-r--r--   0        0        0     2022 2023-03-05 14:00:01.135961 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/heartbeat.meta.json
+-rw-r--r--   0        0        0     5254 2023-03-05 13:59:59.222496 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/jsonutil.data.json
+-rw-r--r--   0        0        0     1887 2023-03-05 13:59:59.222827 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/jsonutil.meta.json
+-rw-r--r--   0        0        0     5290 2023-03-05 13:59:59.331814 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/trio_runner.data.json
+-rw-r--r--   0        0        0     1854 2023-03-05 13:59:59.332034 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ipykernel/trio_runner.meta.json
+-rw-r--r--   0        0        0   267183 2023-03-05 13:59:58.340980 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/itertools.data.json
+-rw-r--r--   0        0        0     1744 2023-03-05 13:59:58.341214 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/itertools.meta.json
+-rw-r--r--   0        0        0    16677 2023-03-05 13:59:59.049733 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/json/__init__.data.json
+-rw-r--r--   0        0        0     1730 2023-03-05 13:59:59.049928 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/json/__init__.meta.json
+-rw-r--r--   0        0        0    15568 2023-03-05 13:59:58.235753 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/json/decoder.data.json
+-rw-r--r--   0        0        0     1674 2023-03-05 13:59:58.236075 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/json/decoder.meta.json
+-rw-r--r--   0        0        0    11577 2023-03-05 13:59:58.234077 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/json/encoder.data.json
+-rw-r--r--   0        0        0     1686 2023-03-05 13:59:58.234330 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/json/encoder.meta.json
+-rw-r--r--   0        0        0     4292 2023-03-05 14:01:08.499292 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jsonschema/__init__.data.json
+-rw-r--r--   0        0        0     1791 2023-03-05 14:01:08.499468 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jsonschema/__init__.meta.json
+-rw-r--r--   0        0        0    29969 2023-03-05 14:01:08.049373 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jsonschema/_format.data.json
+-rw-r--r--   0        0        0     1698 2023-03-05 14:01:08.049570 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jsonschema/_format.meta.json
+-rw-r--r--   0        0        0    15221 2023-03-05 14:01:08.046373 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jsonschema/_types.data.json
+-rw-r--r--   0        0        0     1670 2023-03-05 14:01:08.046620 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jsonschema/_types.meta.json
+-rw-r--r--   0        0        0    17667 2023-03-05 14:01:08.022610 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jsonschema/_utils.data.json
+-rw-r--r--   0        0        0     1688 2023-03-05 14:01:08.022815 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jsonschema/_utils.meta.json
+-rw-r--r--   0        0        0    36635 2023-03-05 14:01:08.496968 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jsonschema/exceptions.data.json
+-rw-r--r--   0        0        0     1851 2023-03-05 14:01:08.497240 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jsonschema/exceptions.meta.json
+-rw-r--r--   0        0        0    13917 2023-03-05 14:01:08.498874 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jsonschema/protocols.data.json
+-rw-r--r--   0        0        0     1819 2023-03-05 14:01:08.499060 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jsonschema/protocols.meta.json
+-rw-r--r--   0        0        0    47152 2023-03-05 14:01:08.498251 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jsonschema/validators.data.json
+-rw-r--r--   0        0        0     1857 2023-03-05 14:01:08.498467 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jsonschema/validators.meta.json
+-rw-r--r--   0        0        0     3959 2023-03-05 13:59:58.035625 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/_version.data.json
+-rw-r--r--   0        0        0     1774 2023-03-05 13:59:58.035843 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/_version.meta.json
+-rw-r--r--   0        0        0    10411 2023-03-05 13:59:57.919097 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/channelsabc.data.json
+-rw-r--r--   0        0        0     1656 2023-03-05 13:59:57.919299 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/channelsabc.meta.json
+-rw-r--r--   0        0        0    18522 2023-03-05 13:59:57.917818 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/clientabc.data.json
+-rw-r--r--   0        0        0     1653 2023-03-05 13:59:57.918031 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/clientabc.meta.json
+-rw-r--r--   0        0        0     5980 2023-03-05 14:01:09.059862 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/jsonutil.data.json
+-rw-r--r--   0        0        0     2044 2023-03-05 14:01:09.060152 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/jsonutil.meta.json
+-rw-r--r--   0        0        0    11762 2023-03-05 13:59:59.234715 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/localinterfaces.data.json
+-rw-r--r--   0        0        0     1834 2023-03-05 13:59:59.234974 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/localinterfaces.meta.json
+-rw-r--r--   0        0        0    11677 2023-03-05 13:59:57.916201 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/managerabc.data.json
+-rw-r--r--   0        0        0     1654 2023-03-05 13:59:57.916404 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/managerabc.meta.json
+-rw-r--r--   0        0        0     2314 2023-03-05 14:00:01.091360 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/ssh/__init__.data.json
+-rw-r--r--   0        0        0     1731 2023-03-05 14:01:11.363236 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/ssh/__init__.meta.json
+-rw-r--r--   0        0        0     7663 2023-03-05 13:59:59.530229 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/ssh/forward.data.json
+-rw-r--r--   0        0        0     1802 2023-03-05 13:59:59.530424 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/ssh/forward.meta.json
+-rw-r--r--   0        0        0     9253 2023-03-05 14:01:11.166357 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/ssh/tunnel.data.json
+-rw-r--r--   0        0        0     2201 2023-03-05 14:01:11.166711 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/ssh/tunnel.meta.json
+-rw-r--r--   0        0        0     2246 2023-03-05 14:00:02.175819 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/utils.data.json
+-rw-r--r--   0        0        0     1957 2023-03-05 14:00:02.176017 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/utils.meta.json
+-rw-r--r--   0        0        0     4043 2023-03-05 13:59:57.868686 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/win_interrupt.data.json
+-rw-r--r--   0        0        0     1676 2023-03-05 13:59:57.869231 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_client/win_interrupt.meta.json
+-rw-r--r--   0        0        0     1868 2023-03-05 13:59:58.875936 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_core/__init__.data.json
+-rw-r--r--   0        0        0     1665 2023-03-05 13:59:58.876119 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_core/__init__.meta.json
+-rw-r--r--   0        0        0    23908 2023-03-05 14:00:02.219317 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_core/paths.data.json
+-rw-r--r--   0        0        0     2193 2023-03-05 14:01:09.876059 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_core/paths.meta.json
+-rw-r--r--   0        0        0    13145 2023-03-05 14:00:01.937099 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_core/utils/__init__.data.json
+-rw-r--r--   0        0        0     2193 2023-03-05 14:00:01.937330 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_core/utils/__init__.meta.json
+-rw-r--r--   0        0        0     2980 2023-03-05 13:59:57.930930 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_core/version.data.json
+-rw-r--r--   0        0        0     1768 2023-03-05 13:59:57.931133 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/jupyter_core/version.meta.json
+-rw-r--r--   0        0        0     3743 2023-03-05 13:59:58.065584 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/keyword.data.json
+-rw-r--r--   0        0        0     1698 2023-03-05 13:59:58.065764 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/keyword.meta.json
+-rw-r--r--   0        0        0     9835 2023-03-05 13:59:58.070122 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/linecache.data.json
+-rw-r--r--   0        0        0     1703 2023-03-05 13:59:58.070381 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/linecache.meta.json
+-rw-r--r--   0        0        0    34120 2023-03-05 13:59:59.553557 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/locale.data.json
+-rw-r--r--   0        0        0     1783 2023-03-05 13:59:59.553756 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/locale.meta.json
+-rw-r--r--   0        0        0   149635 2023-03-05 13:59:59.032114 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/logging/__init__.data.json
+-rw-r--r--   0        0        0     1838 2023-03-05 13:59:59.032388 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/logging/__init__.meta.json
+-rw-r--r--   0        0        0    14995 2023-03-05 13:59:59.303166 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/logging/config.data.json
+-rw-r--r--   0        0        0     1794 2023-03-05 13:59:59.303360 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/logging/config.meta.json
+-rw-r--r--   0        0        0    80466 2023-03-05 13:59:59.782810 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/logging/handlers.data.json
+-rw-r--r--   0        0        0     2007 2023-03-05 13:59:59.783041 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/logging/handlers.meta.json
+-rw-r--r--   0        0        0    53989 2023-03-05 13:59:58.493401 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/math.data.json
+-rw-r--r--   0        0        0     1719 2023-03-05 13:59:58.493632 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/math.meta.json
+-rw-r--r--   0        0        0    16138 2023-03-05 13:59:58.447957 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/mimetypes.data.json
+-rw-r--r--   0        0        0     1714 2023-03-05 13:59:58.448162 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/mimetypes.meta.json
+-rw-r--r--   0        0        0    28133 2023-03-05 13:59:57.792831 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1741 2023-03-05 13:59:57.793006 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0     1629 2023-03-05 13:59:58.114296 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/msvcrt.data.json
+-rw-r--r--   0        0        0     1678 2023-03-05 13:59:58.114485 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/msvcrt.meta.json
+-rw-r--r--   0        0        0    34049 2023-03-05 13:59:59.774157 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/__init__.data.json
+-rw-r--r--   0        0        0     2172 2023-03-05 13:59:59.774389 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/__init__.meta.json
+-rw-r--r--   0        0        0    31566 2023-03-05 13:59:59.123558 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/connection.data.json
+-rw-r--r--   0        0        0     1878 2023-03-05 13:59:59.123753 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/connection.meta.json
+-rw-r--r--   0        0        0   100927 2023-03-05 13:59:59.772819 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/context.data.json
+-rw-r--r--   0        0        0     2336 2023-03-05 13:59:59.773015 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/context.meta.json
+-rw-r--r--   0        0        0   154754 2023-03-05 13:59:59.769981 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/managers.data.json
+-rw-r--r--   0        0        0     1969 2023-03-05 13:59:59.770204 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/managers.meta.json
+-rw-r--r--   0        0        0    53330 2023-03-05 13:59:57.863072 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/pool.data.json
+-rw-r--r--   0        0        0     1765 2023-03-05 13:59:57.863408 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/pool.meta.json
+-rw-r--r--   0        0        0     9476 2023-03-05 13:59:59.487577 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_fork.data.json
+-rw-r--r--   0        0        0     1802 2023-03-05 13:59:59.487785 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_fork.meta.json
+-rw-r--r--   0        0        0     6015 2023-03-05 13:59:59.764125 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_forkserver.data.json
+-rw-r--r--   0        0        0     1844 2023-03-05 13:59:59.764323 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_forkserver.meta.json
+-rw-r--r--   0        0        0     6736 2023-03-05 13:59:59.763573 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_spawn_posix.data.json
+-rw-r--r--   0        0        0     1846 2023-03-05 13:59:59.763836 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_spawn_posix.meta.json
+-rw-r--r--   0        0        0     2122 2023-03-05 13:59:59.485970 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_spawn_win32.data.json
+-rw-r--r--   0        0        0     1816 2023-03-05 13:59:59.486320 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_spawn_win32.meta.json
+-rw-r--r--   0        0        0    18627 2023-03-05 13:59:57.882714 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/process.data.json
+-rw-r--r--   0        0        0     1730 2023-03-05 13:59:57.882928 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/process.meta.json
+-rw-r--r--   0        0        0    20797 2023-03-05 13:59:59.126234 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/queues.data.json
+-rw-r--r--   0        0        0     1734 2023-03-05 13:59:59.126433 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/queues.meta.json
+-rw-r--r--   0        0        0    30807 2023-03-05 13:59:59.765092 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/reduction.data.json
+-rw-r--r--   0        0        0     1989 2023-03-05 13:59:59.765273 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/reduction.meta.json
+-rw-r--r--   0        0        0    29231 2023-03-05 13:59:57.855508 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/shared_memory.data.json
+-rw-r--r--   0        0        0     1756 2023-03-05 13:59:57.855717 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/shared_memory.meta.json
+-rw-r--r--   0        0        0    71994 2023-03-05 13:59:59.766780 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/sharedctypes.data.json
+-rw-r--r--   0        0        0     1904 2023-03-05 13:59:59.766985 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/sharedctypes.meta.json
+-rw-r--r--   0        0        0    10341 2023-03-05 13:59:57.880518 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/spawn.data.json
+-rw-r--r--   0        0        0     1706 2023-03-05 13:59:57.880697 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/spawn.meta.json
+-rw-r--r--   0        0        0    26724 2023-03-05 13:59:59.770837 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/synchronize.data.json
+-rw-r--r--   0        0        0     1869 2023-03-05 13:59:59.771018 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/synchronize.meta.json
+-rw-r--r--   0        0        0    24714 2023-03-05 13:59:59.110848 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/util.data.json
+-rw-r--r--   0        0        0     1773 2023-03-05 13:59:59.111063 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/multiprocessing/util.meta.json
+-rw-r--r--   0        0        0     1668 2023-03-05 13:59:57.941390 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/_imports.data.json
+-rw-r--r--   0        0        0     1674 2023-03-05 13:59:57.941587 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/_imports.meta.json
+-rw-r--r--   0        0        0     6775 2023-03-05 13:59:57.944287 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/_struct.data.json
+-rw-r--r--   0        0        0     1722 2023-03-05 13:59:57.944540 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/_struct.meta.json
+-rw-r--r--   0        0        0     3211 2023-03-05 13:59:58.042388 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/_version.data.json
+-rw-r--r--   0        0        0     1852 2023-03-05 13:59:58.042609 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/_version.meta.json
+-rw-r--r--   0        0        0     1668 2023-03-05 13:59:57.883950 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/corpus/__init__.data.json
+-rw-r--r--   0        0        0     1640 2023-03-05 13:59:57.884168 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/corpus/__init__.meta.json
+-rw-r--r--   0        0        0     1790 2023-03-05 13:59:58.673120 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/corpus/words.data.json
+-rw-r--r--   0        0        0     1660 2023-03-05 13:59:58.673305 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/corpus/words.meta.json
+-rw-r--r--   0        0        0    10248 2023-03-05 14:01:08.680729 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/json_compat.data.json
+-rw-r--r--   0        0        0     1868 2023-03-05 14:01:08.681036 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/json_compat.meta.json
+-rw-r--r--   0        0        0     3218 2023-03-05 13:59:58.040088 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/sentinel.data.json
+-rw-r--r--   0        0        0     1702 2023-03-05 13:59:58.040368 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/sentinel.meta.json
+-rw-r--r--   0        0        0     1689 2023-03-05 13:59:57.945938 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v1/convert.data.json
+-rw-r--r--   0        0        0     1641 2023-03-05 13:59:57.946173 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v1/convert.meta.json
+-rw-r--r--   0        0        0     3946 2023-03-05 13:59:57.887728 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v1/rwbase.data.json
+-rw-r--r--   0        0        0     1640 2023-03-05 13:59:57.887922 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v1/rwbase.meta.json
+-rw-r--r--   0        0        0     2384 2023-03-05 13:59:59.189191 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v2/convert.data.json
+-rw-r--r--   0        0        0     1671 2023-03-05 13:59:59.189380 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v2/convert.meta.json
+-rw-r--r--   0        0        0     4874 2023-03-05 13:59:58.676647 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v2/nbbase.data.json
+-rw-r--r--   0        0        0     1780 2023-03-05 13:59:58.676894 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v2/nbbase.meta.json
+-rw-r--r--   0        0        0     2406 2023-03-05 13:59:57.945211 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v2/nbxml.data.json
+-rw-r--r--   0        0        0     1637 2023-03-05 13:59:57.945454 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v2/nbxml.meta.json
+-rw-r--r--   0        0        0     5725 2023-03-05 13:59:58.589761 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v2/rwbase.data.json
+-rw-r--r--   0        0        0     1722 2023-03-05 13:59:58.589959 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v2/rwbase.meta.json
+-rw-r--r--   0        0        0     6240 2023-03-05 13:59:58.587486 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v3/rwbase.data.json
+-rw-r--r--   0        0        0     1721 2023-03-05 13:59:58.587686 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v3/rwbase.meta.json
+-rw-r--r--   0        0        0     5834 2023-03-05 13:59:57.886699 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v4/rwbase.data.json
+-rw-r--r--   0        0        0     1705 2023-03-05 13:59:57.886908 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/v4/rwbase.meta.json
+-rw-r--r--   0        0        0     3081 2023-03-05 13:59:57.937922 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/warnings.data.json
+-rw-r--r--   0        0        0     1637 2023-03-05 13:59:57.938130 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/nbformat/warnings.meta.json
+-rw-r--r--   0        0        0    77674 2023-03-05 14:01:08.530489 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ntsecuritycon/__init__.data.json
+-rw-r--r--   0        0        0     1677 2023-03-05 14:01:08.530690 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ntsecuritycon/__init__.meta.json
+-rw-r--r--   0        0        0    84003 2023-03-05 13:59:58.025429 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numbers.data.json
+-rw-r--r--   0        0        0     1638 2023-03-05 13:59:58.025632 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numbers.meta.json
+-rw-r--r--   0        0        0  2384203 2023-03-05 14:00:00.883866 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3369 2023-03-05 14:00:00.884558 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     5239 2023-03-05 13:59:58.463976 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1666 2023-03-05 13:59:58.464164 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0    22339 2023-03-05 14:00:00.777296 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/__init__.data.json
+-rw-r--r--   0        0        0     2094 2023-03-05 14:00:00.777480 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/__init__.meta.json
+-rw-r--r--   0        0        0     3910 2023-03-05 14:00:00.922306 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1874 2023-03-05 14:00:00.922492 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    27226 2023-03-05 14:00:00.771301 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_array_like.data.json
+-rw-r--r--   0        0        0     1865 2023-03-05 14:00:00.771499 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_array_like.meta.json
+-rw-r--r--   0        0        0   277852 2023-03-05 14:00:00.838853 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_callable.data.json
+-rw-r--r--   0        0        0     1905 2023-03-05 14:00:00.839086 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_callable.meta.json
+-rw-r--r--   0        0        0    45396 2023-03-05 13:59:58.290941 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1653 2023-03-05 13:59:58.291135 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    32835 2023-03-05 14:00:00.765570 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1853 2023-03-05 14:00:00.765749 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     6215 2023-03-05 14:00:00.833714 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1759 2023-03-05 14:00:00.833889 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    36648 2023-03-05 14:00:00.764024 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1904 2023-03-05 14:00:00.764348 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4746 2023-03-05 13:59:58.306348 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_nbit.data.json
+-rw-r--r--   0        0        0     1640 2023-03-05 13:59:58.306533 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_nbit.meta.json
+-rw-r--r--   0        0        0    17703 2023-03-05 13:59:59.009120 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1711 2023-03-05 13:59:59.009328 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     6364 2023-03-05 14:00:00.764637 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_scalars.data.json
+-rw-r--r--   0        0        0     1711 2023-03-05 14:00:00.764847 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2487 2023-03-05 13:59:58.286822 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_shape.data.json
+-rw-r--r--   0        0        0     1642 2023-03-05 13:59:58.287013 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_shape.meta.json
+-rw-r--r--   0        0        0   280489 2023-03-05 14:00:00.928018 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1911 2023-03-05 14:00:00.928306 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_typing/_ufunc.meta.json
+-rw-r--r--   0        0        0     1957 2023-03-05 13:59:59.354577 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_version.data.json
+-rw-r--r--   0        0        0     1718 2023-03-05 13:59:59.354793 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/_version.meta.json
+-rw-r--r--   0        0        0     5426 2023-03-05 13:59:58.845346 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/compat/__init__.data.json
+-rw-r--r--   0        0        0     1696 2023-03-05 13:59:58.845539 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/compat/__init__.meta.json
+-rw-r--r--   0        0        0     5986 2023-03-05 13:59:58.097408 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/compat/_inspect.data.json
+-rw-r--r--   0        0        0     1755 2023-03-05 13:59:58.097610 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/compat/_inspect.meta.json
+-rw-r--r--   0        0        0    12299 2023-03-05 13:59:57.908006 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/compat/py3k.data.json
+-rw-r--r--   0        0        0     1922 2023-03-05 13:59:57.908221 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/compat/py3k.meta.json
+-rw-r--r--   0        0        0     1628 2023-03-05 13:59:58.463094 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1633 2023-03-05 13:59:58.463271 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    14745 2023-03-05 14:00:00.824038 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1826 2023-03-05 14:00:00.824202 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    23443 2023-03-05 14:00:00.839694 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1750 2023-03-05 14:00:00.839871 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     5153 2023-03-05 14:00:00.823464 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1715 2023-03-05 14:00:00.823633 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    11857 2023-03-05 14:00:00.823041 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1741 2023-03-05 14:00:00.823211 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    30117 2023-03-05 14:00:00.822500 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1794 2023-03-05 14:00:00.822681 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   180955 2023-03-05 14:00:00.904669 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1847 2023-03-05 14:00:00.904916 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    38950 2023-03-05 14:00:00.821566 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1872 2023-03-05 14:00:00.821764 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0   357183 2023-03-05 14:00:00.831811 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1894 2023-03-05 14:00:00.832102 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    53356 2023-03-05 14:00:00.833234 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1853 2023-03-05 14:00:00.833432 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   324101 2023-03-05 14:00:00.820316 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1952 2023-03-05 14:00:00.820644 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   211121 2023-03-05 14:00:00.812837 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1896 2023-03-05 14:00:00.813098 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    48957 2023-03-05 14:00:00.808279 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1962 2023-03-05 14:00:00.808463 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    27023 2023-03-05 13:59:59.006043 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/overrides.data.json
+-rw-r--r--   0        0        0     1902 2023-03-05 13:59:59.006249 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/overrides.meta.json
+-rw-r--r--   0        0        0    56774 2023-03-05 14:00:00.900555 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1911 2023-03-05 14:00:00.900722 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    56748 2023-03-05 14:00:00.807057 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1871 2023-03-05 14:00:00.807245 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3289 2023-03-05 13:59:59.007242 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1693 2023-03-05 13:59:59.007433 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0   120294 2023-03-05 14:00:00.776554 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1988 2023-03-05 14:00:00.776762 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     4625 2023-03-05 14:00:00.915679 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1766 2023-03-05 14:00:00.915842 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    19981 2023-03-05 14:00:00.896424 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1833 2023-03-05 14:00:00.896590 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    23352 2023-03-05 14:00:00.895738 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1800 2023-03-05 14:00:00.895905 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    26146 2023-03-05 14:00:00.773886 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2400 2023-03-05 14:00:00.774073 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     9401 2023-03-05 13:59:58.285037 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1640 2023-03-05 13:59:58.285220 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    19429 2023-03-05 14:00:00.805710 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1805 2023-03-05 14:00:00.805896 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   167194 2023-03-05 14:00:00.804877 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1811 2023-03-05 14:00:00.805148 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    27863 2023-03-05 14:00:00.801090 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1797 2023-03-05 14:00:00.801336 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7237 2023-03-05 13:59:58.286146 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1635 2023-03-05 13:59:58.286322 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   240651 2023-03-05 14:00:00.799981 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     2006 2023-03-05 14:00:00.800251 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0     9558 2023-03-05 14:00:00.794645 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1817 2023-03-05 14:00:00.794874 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    67811 2023-03-05 14:00:00.794088 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1907 2023-03-05 14:00:00.794287 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    49712 2023-03-05 14:00:00.894997 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1699 2023-03-05 14:00:00.895161 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    97113 2023-03-05 14:00:00.792442 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1921 2023-03-05 14:00:00.792646 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0   103869 2023-03-05 14:00:00.790446 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     2037 2023-03-05 14:00:00.790643 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0   103615 2023-03-05 14:00:00.788068 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1810 2023-03-05 14:00:00.788320 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0    66510 2023-03-05 14:00:00.893850 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1802 2023-03-05 14:00:00.894035 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    95306 2023-03-05 14:00:00.785688 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1923 2023-03-05 14:00:00.785905 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    25177 2023-03-05 14:00:00.783693 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1839 2023-03-05 14:00:00.783862 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    82804 2023-03-05 14:00:00.782912 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1872 2023-03-05 14:00:00.783091 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0   104203 2023-03-05 14:00:00.781132 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1871 2023-03-05 14:00:00.781309 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    26752 2023-03-05 14:00:00.778994 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1806 2023-03-05 14:00:00.779182 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    27948 2023-03-05 14:00:00.778188 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1786 2023-03-05 14:00:00.778369 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5678 2023-03-05 14:00:00.899213 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1745 2023-03-05 14:00:00.899378 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   115542 2023-03-05 14:00:00.898801 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1856 2023-03-05 14:00:00.898972 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    29854 2023-03-05 14:00:00.773118 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1756 2023-03-05 14:00:00.773300 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   140392 2023-03-05 14:00:00.769468 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1778 2023-03-05 14:00:00.769763 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    23680 2023-03-05 14:00:00.770439 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1758 2023-03-05 14:00:00.770629 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    14850 2023-03-05 14:00:00.771947 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1744 2023-03-05 14:00:00.772122 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     2967 2023-03-05 14:00:00.772333 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1771 2023-03-05 14:00:00.772508 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6637 2023-03-05 14:00:00.766062 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1878 2023-03-05 14:00:00.766233 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4358 2023-03-05 14:00:00.915281 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1936 2023-03-05 14:00:00.915452 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    27675 2023-03-05 13:59:58.095022 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1656 2023-03-05 13:59:58.095207 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    16931 2023-03-05 14:00:00.892428 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1792 2023-03-05 14:00:00.892593 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    14576 2023-03-05 14:00:00.891815 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1788 2023-03-05 14:00:00.891979 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    14629 2023-03-05 14:00:00.891245 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1792 2023-03-05 14:00:00.891411 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    14404 2023-03-05 14:00:00.890659 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1790 2023-03-05 14:00:00.890832 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    14404 2023-03-05 14:00:00.890074 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1790 2023-03-05 14:00:00.890244 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    13519 2023-03-05 14:00:00.889490 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1794 2023-03-05 14:00:00.889660 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4735 2023-03-05 13:59:58.091725 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1656 2023-03-05 13:59:58.091904 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0    10544 2023-03-05 14:00:00.921897 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1937 2023-03-05 14:00:00.922063 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   271081 2023-03-05 14:00:00.921316 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1937 2023-03-05 14:00:00.921569 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    11101 2023-03-05 14:00:00.914406 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1845 2023-03-05 14:00:00.914573 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    16178 2023-03-05 14:00:00.913871 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1750 2023-03-05 14:00:00.914051 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    11994 2023-03-05 14:00:00.913252 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1766 2023-03-05 14:00:00.913430 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     9431 2023-03-05 14:00:00.912682 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1764 2023-03-05 14:00:00.912866 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    72274 2023-03-05 14:00:00.888879 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1902 2023-03-05 14:00:00.889063 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   347968 2023-03-05 14:00:00.911954 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1906 2023-03-05 14:00:00.912282 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     9282 2023-03-05 14:00:00.914871 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1774 2023-03-05 14:00:00.915045 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1724 2023-03-05 13:59:58.090722 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1654 2023-03-05 13:59:58.090918 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   122268 2023-03-05 14:00:00.887254 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     2084 2023-03-05 14:00:00.887457 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0     3046 2023-03-05 14:00:00.922721 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     1782 2023-03-05 14:00:00.922887 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0     3508 2023-03-05 13:59:59.636465 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/version.data.json
+-rw-r--r--   0        0        0     1750 2023-03-05 13:59:59.636656 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/numpy/version.meta.json
+-rw-r--r--   0        0        0     6614 2023-03-05 13:59:58.378820 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/opcode.data.json
+-rw-r--r--   0        0        0     1699 2023-03-05 13:59:58.379006 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/opcode.meta.json
+-rw-r--r--   0        0        0    51024 2023-03-05 13:59:59.011513 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/operator.data.json
+-rw-r--r--   0        0        0     1723 2023-03-05 13:59:59.011713 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/operator.meta.json
+-rw-r--r--   0        0        0   338829 2023-03-05 13:59:57.791955 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1883 2023-03-05 13:59:57.792149 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     5305 2023-03-05 13:59:57.785873 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1672 2023-03-05 13:59:57.786049 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     3451 2023-03-05 13:59:57.878450 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/packaging/__init__.data.json
+-rw-r--r--   0        0        0     1630 2023-03-05 13:59:57.878681 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/packaging/__init__.meta.json
+-rw-r--r--   0        0        0    14453 2023-03-05 13:59:57.877550 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/packaging/_structures.data.json
+-rw-r--r--   0        0        0     1646 2023-03-05 13:59:57.877834 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/packaging/_structures.meta.json
+-rw-r--r--   0        0        0    69662 2023-03-05 13:59:58.668662 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/packaging/version.data.json
+-rw-r--r--   0        0        0     1857 2023-03-05 13:59:58.668918 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/packaging/version.meta.json
+-rw-r--r--   0        0        0     6546 2023-03-05 14:01:10.055112 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/__init__.data.json
+-rw-r--r--   0        0        0     2291 2023-03-05 14:01:10.055319 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/__init__.meta.json
+-rw-r--r--   0        0        0    31892 2023-03-05 14:01:09.826457 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/agent.data.json
+-rw-r--r--   0        0        0     1818 2023-03-05 14:01:09.826663 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/agent.meta.json
+-rw-r--r--   0        0        0    23965 2023-03-05 14:01:09.736789 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/auth_handler.data.json
+-rw-r--r--   0        0        0     1825 2023-03-05 14:01:09.737032 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/auth_handler.meta.json
+-rw-r--r--   0        0        0    11969 2023-03-05 14:01:08.484252 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/buffered_pipe.data.json
+-rw-r--r--   0        0        0     1672 2023-03-05 14:01:08.484440 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/buffered_pipe.meta.json
+-rw-r--r--   0        0        0    49554 2023-03-05 14:01:09.742935 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/channel.data.json
+-rw-r--r--   0        0        0     1837 2023-03-05 14:01:09.743112 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/channel.meta.json
+-rw-r--r--   0        0        0    24917 2023-03-05 14:01:09.822937 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/client.data.json
+-rw-r--r--   0        0        0     1925 2023-03-05 14:01:09.823149 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/client.meta.json
+-rw-r--r--   0        0        0    28759 2023-03-05 14:01:08.345324 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/common.data.json
+-rw-r--r--   0        0        0     1641 2023-03-05 14:01:08.345522 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/common.meta.json
+-rw-r--r--   0        0        0     6323 2023-03-05 14:01:08.482230 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/compress.data.json
+-rw-r--r--   0        0        0     1658 2023-03-05 14:01:08.482406 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/compress.meta.json
+-rw-r--r--   0        0        0    19702 2023-03-05 14:01:08.781867 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/config.data.json
+-rw-r--r--   0        0        0     1736 2023-03-05 14:01:08.782066 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/config.meta.json
+-rw-r--r--   0        0        0    14974 2023-03-05 14:01:08.673545 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/dsskey.data.json
+-rw-r--r--   0        0        0     1714 2023-03-05 14:01:08.673726 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/dsskey.meta.json
+-rw-r--r--   0        0        0    26043 2023-03-05 14:01:09.691458 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/ecdsakey.data.json
+-rw-r--r--   0        0        0     1965 2023-03-05 14:01:09.691670 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/ecdsakey.meta.json
+-rw-r--r--   0        0        0     8915 2023-03-05 14:01:08.671720 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/ed25519key.data.json
+-rw-r--r--   0        0        0     1696 2023-03-05 14:01:08.671913 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/ed25519key.meta.json
+-rw-r--r--   0        0        0    26482 2023-03-05 14:01:09.055048 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/file.data.json
+-rw-r--r--   0        0        0     1684 2023-03-05 14:01:09.055237 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/file.meta.json
+-rw-r--r--   0        0        0    28415 2023-03-05 14:01:08.670308 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/hostkeys.data.json
+-rw-r--r--   0        0        0     1720 2023-03-05 14:01:08.670516 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/hostkeys.meta.json
+-rw-r--r--   0        0        0    23353 2023-03-05 14:01:08.343115 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/message.data.json
+-rw-r--r--   0        0        0     1706 2023-03-05 14:01:08.343303 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/message.meta.json
+-rw-r--r--   0        0        0    24910 2023-03-05 14:01:09.686687 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/packet.data.json
+-rw-r--r--   0        0        0     2002 2023-03-05 14:01:09.686897 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/packet.meta.json
+-rw-r--r--   0        0        0    30907 2023-03-05 14:01:08.487677 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/pkey.data.json
+-rw-r--r--   0        0        0     1701 2023-03-05 14:01:08.487867 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/pkey.meta.json
+-rw-r--r--   0        0        0     8240 2023-03-05 14:01:09.052085 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/proxy.data.json
+-rw-r--r--   0        0        0     1680 2023-03-05 14:01:09.052273 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/proxy.meta.json
+-rw-r--r--   0        0        0    16831 2023-03-05 14:01:09.688702 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/rsakey.data.json
+-rw-r--r--   0        0        0     1915 2023-03-05 14:01:09.688898 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/rsakey.meta.json
+-rw-r--r--   0        0        0    30724 2023-03-05 14:01:09.741784 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/server.data.json
+-rw-r--r--   0        0        0     1788 2023-03-05 14:01:09.741958 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/server.meta.json
+-rw-r--r--   0        0        0    13497 2023-03-05 14:01:09.740961 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/sftp.data.json
+-rw-r--r--   0        0        0     1704 2023-03-05 14:01:09.741132 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/sftp.meta.json
+-rw-r--r--   0        0        0    10648 2023-03-05 14:01:08.340378 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/sftp_attr.data.json
+-rw-r--r--   0        0        0     1705 2023-03-05 14:01:08.340575 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/sftp_attr.meta.json
+-rw-r--r--   0        0        0    33946 2023-03-05 14:01:09.740404 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/sftp_client.data.json
+-rw-r--r--   0        0        0     1921 2023-03-05 14:01:09.740576 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/sftp_client.meta.json
+-rw-r--r--   0        0        0    16952 2023-03-05 14:01:09.739481 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/sftp_file.data.json
+-rw-r--r--   0        0        0     1830 2023-03-05 14:01:09.739659 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/sftp_file.meta.json
+-rw-r--r--   0        0        0     6801 2023-03-05 14:01:09.050907 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/sftp_handle.data.json
+-rw-r--r--   0        0        0     1701 2023-03-05 14:01:09.051086 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/sftp_handle.meta.json
+-rw-r--r--   0        0        0    11215 2023-03-05 14:01:09.925511 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/sftp_server.data.json
+-rw-r--r--   0        0        0     1898 2023-03-05 14:01:09.925718 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/sftp_server.meta.json
+-rw-r--r--   0        0        0    15086 2023-03-05 14:01:09.820064 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/sftp_si.data.json
+-rw-r--r--   0        0        0     1749 2023-03-05 14:01:09.820266 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/sftp_si.meta.json
+-rw-r--r--   0        0        0    22265 2023-03-05 14:01:08.666861 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/ssh_exception.data.json
+-rw-r--r--   0        0        0     1720 2023-03-05 14:01:08.667052 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/ssh_exception.meta.json
+-rw-r--r--   0        0        0    30038 2023-03-05 14:01:08.026118 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/ssh_gss.data.json
+-rw-r--r--   0        0        0     1642 2023-03-05 14:01:08.026325 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/ssh_gss.meta.json
+-rw-r--r--   0        0        0    91286 2023-03-05 14:01:09.738823 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/transport.data.json
+-rw-r--r--   0        0        0     2050 2023-03-05 14:01:09.739025 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/transport.meta.json
+-rw-r--r--   0        0        0    22713 2023-03-05 14:01:08.864311 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/util.data.json
+-rw-r--r--   0        0        0     1764 2023-03-05 14:01:08.864550 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/paramiko/util.meta.json
+-rw-r--r--   0        0        0    92975 2023-03-05 13:59:57.785409 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1834 2023-03-05 13:59:57.785601 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    99151 2023-03-05 13:59:59.618853 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pdb.data.json
+-rw-r--r--   0        0        0     1871 2023-03-05 13:59:59.619069 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pdb.meta.json
+-rw-r--r--   0        0        0    47593 2023-03-05 13:59:57.783487 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1770 2023-03-05 13:59:57.783667 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    33493 2023-03-05 13:59:58.385111 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pkgutil.data.json
+-rw-r--r--   0        0        0     1740 2023-03-05 13:59:58.385318 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pkgutil.meta.json
+-rw-r--r--   0        0        0    37135 2023-03-05 13:59:58.258093 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/platform.data.json
+-rw-r--r--   0        0        0     1675 2023-03-05 13:59:58.258299 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/platform.meta.json
+-rw-r--r--   0        0        0    21800 2023-03-05 13:59:59.549907 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/platformdirs/__init__.data.json
+-rw-r--r--   0        0        0     1911 2023-03-05 13:59:59.550105 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/platformdirs/__init__.meta.json
+-rw-r--r--   0        0        0    17704 2023-03-05 13:59:59.174094 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/platformdirs/android.data.json
+-rw-r--r--   0        0        0     1811 2023-03-05 13:59:59.174315 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/platformdirs/android.meta.json
+-rw-r--r--   0        0        0    31813 2023-03-05 13:59:58.672497 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/platformdirs/api.data.json
+-rw-r--r--   0        0        0     1738 2023-03-05 13:59:58.672708 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/platformdirs/api.meta.json
+-rw-r--r--   0        0        0    14999 2023-03-05 13:59:59.176694 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/platformdirs/macos.data.json
+-rw-r--r--   0        0        0     1719 2023-03-05 13:59:59.176954 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/platformdirs/macos.meta.json
+-rw-r--r--   0        0        0     2900 2023-03-05 13:59:57.929140 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/platformdirs/version.data.json
+-rw-r--r--   0        0        0     1643 2023-03-05 13:59:57.929320 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/platformdirs/version.meta.json
+-rw-r--r--   0        0        0    80904 2023-03-05 13:59:57.782301 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1764 2023-03-05 13:59:57.782479 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0    12669 2023-03-05 13:59:58.254831 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pprint.data.json
+-rw-r--r--   0        0        0     1671 2023-03-05 13:59:58.255021 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pprint.meta.json
+-rw-r--r--   0        0        0    19634 2023-03-05 13:59:57.890466 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/profile.data.json
+-rw-r--r--   0        0        0     1723 2023-03-05 13:59:57.890681 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/profile.meta.json
+-rw-r--r--   0        0        0     3878 2023-03-05 14:00:03.583537 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/__init__.data.json
+-rw-r--r--   0        0        0     2124 2023-03-05 14:01:11.159370 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/__init__.meta.json
+-rw-r--r--   0        0        0     3806 2023-03-05 14:00:03.576593 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/__init__.data.json
+-rw-r--r--   0        0        0     2050 2023-03-05 14:01:11.153152 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/__init__.meta.json
+-rw-r--r--   0        0        0   110705 2023-03-05 14:00:03.574363 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/application.data.json
+-rw-r--r--   0        0        0     4647 2023-03-05 14:01:11.151553 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/application.meta.json
+-rw-r--r--   0        0        0    17588 2023-03-05 14:00:03.513758 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/current.data.json
+-rw-r--r--   0        0        0     2245 2023-03-05 14:01:11.101896 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/current.meta.json
+-rw-r--r--   0        0        0     9564 2023-03-05 14:00:03.576125 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/dummy.data.json
+-rw-r--r--   0        0        0     2724 2023-03-05 14:01:11.152877 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/dummy.meta.json
+-rw-r--r--   0        0        0     6934 2023-03-05 14:00:03.514201 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/run_in_terminal.data.json
+-rw-r--r--   0        0        0     2337 2023-03-05 14:01:11.102262 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/run_in_terminal.meta.json
+-rw-r--r--   0        0        0    25227 2023-03-05 14:00:03.525841 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/auto_suggest.data.json
+-rw-r--r--   0        0        0     2234 2023-03-05 14:01:11.111713 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/auto_suggest.meta.json
+-rw-r--r--   0        0        0   115144 2023-03-05 14:00:03.554715 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/buffer.data.json
+-rw-r--r--   0        0        0     3256 2023-03-05 14:01:11.134028 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/buffer.meta.json
+-rw-r--r--   0        0        0    21902 2023-03-05 13:59:58.844560 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/cache.data.json
+-rw-r--r--   0        0        0     1750 2023-03-05 13:59:58.844787 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/cache.meta.json
+-rw-r--r--   0        0        0     2966 2023-03-05 13:59:59.726404 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/__init__.data.json
+-rw-r--r--   0        0        0     1812 2023-03-05 13:59:59.726592 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/__init__.meta.json
+-rw-r--r--   0        0        0    19797 2023-03-05 13:59:59.120176 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/base.data.json
+-rw-r--r--   0        0        0     1729 2023-03-05 13:59:59.120391 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/base.meta.json
+-rw-r--r--   0        0        0     7335 2023-03-05 13:59:59.489368 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/in_memory.data.json
+-rw-r--r--   0        0        0     1850 2023-03-05 13:59:59.489578 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/in_memory.meta.json
+-rw-r--r--   0        0        0     4485 2023-03-05 14:00:03.551452 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/__init__.data.json
+-rw-r--r--   0        0        0     2141 2023-03-05 14:01:11.131339 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/__init__.meta.json
+-rw-r--r--   0        0        0    45627 2023-03-05 14:00:03.545702 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/base.data.json
+-rw-r--r--   0        0        0     2458 2023-03-05 14:01:11.127226 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/base.meta.json
+-rw-r--r--   0        0        0     5921 2023-03-05 14:00:03.547927 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/deduplicate.data.json
+-rw-r--r--   0        0        0     1948 2023-03-05 14:01:11.129060 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/deduplicate.meta.json
+-rw-r--r--   0        0        0    10558 2023-03-05 14:00:03.550989 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/filesystem.data.json
+-rw-r--r--   0        0        0     2454 2023-03-05 14:01:11.131054 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/filesystem.meta.json
+-rw-r--r--   0        0        0    33125 2023-03-05 14:00:03.550396 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/fuzzy_completer.data.json
+-rw-r--r--   0        0        0     2596 2023-03-05 14:01:11.130654 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/fuzzy_completer.meta.json
+-rw-r--r--   0        0        0    10200 2023-03-05 14:00:03.549396 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/nested.data.json
+-rw-r--r--   0        0        0     2533 2023-03-05 14:01:11.129887 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/nested.meta.json
+-rw-r--r--   0        0        0    10690 2023-03-05 14:00:03.548790 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/word_completer.data.json
+-rw-r--r--   0        0        0     2399 2023-03-05 14:01:11.129479 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/word_completer.meta.json
+-rw-r--r--   0        0        0    19855 2023-03-05 14:00:03.510129 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/cursor_shapes.data.json
+-rw-r--r--   0        0        0     2150 2023-03-05 14:01:11.098579 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/cursor_shapes.meta.json
+-rw-r--r--   0        0        0    30460 2023-03-05 13:59:58.591476 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/data_structures.data.json
+-rw-r--r--   0        0        0     1682 2023-03-05 13:59:58.591696 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/data_structures.meta.json
+-rw-r--r--   0        0        0    87962 2023-03-05 14:00:03.521626 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/document.data.json
+-rw-r--r--   0        0        0     2216 2023-03-05 14:01:11.108526 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/document.meta.json
+-rw-r--r--   0        0        0     3945 2023-03-05 13:59:58.892010 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/enums.data.json
+-rw-r--r--   0        0        0     1677 2023-03-05 13:59:58.892190 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/enums.meta.json
+-rw-r--r--   0        0        0     3658 2023-03-05 14:00:02.365510 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/__init__.data.json
+-rw-r--r--   0        0        0     1993 2023-03-05 14:00:02.365710 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/__init__.meta.json
+-rw-r--r--   0        0        0    10864 2023-03-05 14:00:02.174624 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/async_generator.data.json
+-rw-r--r--   0        0        0     2025 2023-03-05 14:00:02.174835 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/async_generator.meta.json
+-rw-r--r--   0        0        0    19208 2023-03-05 14:00:01.869481 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/inputhook.data.json
+-rw-r--r--   0        0        0     2183 2023-03-05 14:00:01.869725 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/inputhook.meta.json
+-rw-r--r--   0        0        0     7927 2023-03-05 14:00:01.864488 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/utils.data.json
+-rw-r--r--   0        0        0     1981 2023-03-05 14:00:01.864764 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/utils.meta.json
+-rw-r--r--   0        0        0    10713 2023-03-05 14:00:03.516480 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/__init__.data.json
+-rw-r--r--   0        0        0     2007 2023-03-05 14:01:11.104012 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/__init__.meta.json
+-rw-r--r--   0        0        0    30926 2023-03-05 14:00:03.515056 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/app.data.json
+-rw-r--r--   0        0        0     3161 2023-03-05 14:01:11.103002 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/app.meta.json
+-rw-r--r--   0        0        0    33195 2023-03-05 13:59:58.832163 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/base.data.json
+-rw-r--r--   0        0        0     1676 2023-03-05 13:59:58.832419 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/base.meta.json
+-rw-r--r--   0        0        0    21205 2023-03-05 14:00:03.515775 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/cli.data.json
+-rw-r--r--   0        0        0     2122 2023-03-05 14:01:11.103589 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/cli.meta.json
+-rw-r--r--   0        0        0     5068 2023-03-05 13:59:59.191923 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/utils.data.json
+-rw-r--r--   0        0        0     1715 2023-03-05 13:59:59.192273 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/utils.meta.json
+-rw-r--r--   0        0        0     4356 2023-03-05 14:00:03.542170 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/__init__.data.json
+-rw-r--r--   0        0        0     2100 2023-03-05 14:01:11.124281 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/__init__.meta.json
+-rw-r--r--   0        0        0    17413 2023-03-05 14:00:03.541763 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/ansi.data.json
+-rw-r--r--   0        0        0     2192 2023-03-05 14:01:11.123985 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/ansi.meta.json
+-rw-r--r--   0        0        0    17303 2023-03-05 14:00:03.508803 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/base.data.json
+-rw-r--r--   0        0        0     2066 2023-03-05 14:01:11.097449 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/base.meta.json
+-rw-r--r--   0        0        0    10370 2023-03-05 14:00:03.511118 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/html.data.json
+-rw-r--r--   0        0        0     2180 2023-03-05 14:01:11.099517 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/html.meta.json
+-rw-r--r--   0        0        0     6374 2023-03-05 14:01:11.098887 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/pygments.data.json
+-rw-r--r--   0        0        0     2056 2023-03-05 14:01:11.099111 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/pygments.meta.json
+-rw-r--r--   0        0        0     7085 2023-03-05 14:00:03.512562 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/utils.data.json
+-rw-r--r--   0        0        0     2033 2023-03-05 14:01:11.100842 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/utils.meta.json
+-rw-r--r--   0        0        0    27475 2023-03-05 14:00:01.960642 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/history.data.json
+-rw-r--r--   0        0        0     2106 2023-03-05 14:00:01.960961 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/history.meta.json
+-rw-r--r--   0        0        0     2881 2023-03-05 14:00:03.539168 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/__init__.data.json
+-rw-r--r--   0        0        0     1924 2023-03-05 14:01:11.121989 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/__init__.meta.json
+-rw-r--r--   0        0        0     4273 2023-03-05 13:59:59.107693 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/ansi_escape_sequences.data.json
+-rw-r--r--   0        0        0     1847 2023-03-05 13:59:59.107954 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/ansi_escape_sequences.meta.json
+-rw-r--r--   0        0        0    31155 2023-03-05 14:00:03.535376 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/base.data.json
+-rw-r--r--   0        0        0     1958 2023-03-05 14:01:11.119218 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/base.meta.json
+-rw-r--r--   0        0        0     4533 2023-03-05 14:00:03.537753 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/defaults.data.json
+-rw-r--r--   0        0        0     2009 2023-03-05 14:01:11.120889 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/defaults.meta.json
+-rw-r--r--   0        0        0    18460 2023-03-05 14:00:03.538802 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/posix_pipe.data.json
+-rw-r--r--   0        0        0     1987 2023-03-05 14:01:11.121719 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/posix_pipe.meta.json
+-rw-r--r--   0        0        0     6081 2023-03-05 13:59:58.581369 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/posix_utils.data.json
+-rw-r--r--   0        0        0     1799 2023-03-05 13:59:58.581563 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/posix_utils.meta.json
+-rw-r--r--   0        0        0     5412 2023-03-05 14:00:03.537081 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/typeahead.data.json
+-rw-r--r--   0        0        0     2029 2023-03-05 14:01:11.120590 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/typeahead.meta.json
+-rw-r--r--   0        0        0    30618 2023-03-05 14:00:03.536660 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/vt100.data.json
+-rw-r--r--   0        0        0     2212 2023-03-05 14:01:11.120263 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/vt100.meta.json
+-rw-r--r--   0        0        0    17493 2023-03-05 14:00:03.527259 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/vt100_parser.data.json
+-rw-r--r--   0        0        0     2208 2023-03-05 14:01:11.112698 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/vt100_parser.meta.json
+-rw-r--r--   0        0        0     3319 2023-03-05 14:00:03.533123 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/__init__.data.json
+-rw-r--r--   0        0        0     1962 2023-03-05 14:01:11.117377 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/__init__.meta.json
+-rw-r--r--   0        0        0     1828 2023-03-05 13:59:57.973215 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/__init__.data.json
+-rw-r--r--   0        0        0     1680 2023-03-05 13:59:57.973441 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/__init__.meta.json
+-rw-r--r--   0        0        0     4097 2023-03-05 14:00:03.530822 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/auto_suggest.data.json
+-rw-r--r--   0        0        0     2424 2023-03-05 14:01:11.115574 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/auto_suggest.meta.json
+-rw-r--r--   0        0        0     5644 2023-03-05 14:00:03.561022 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/basic.data.json
+-rw-r--r--   0        0        0     2547 2023-03-05 14:01:11.139572 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/basic.meta.json
+-rw-r--r--   0        0        0     8035 2023-03-05 14:00:03.552032 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/completion.data.json
+-rw-r--r--   0        0        0     3601 2023-03-05 14:01:11.131710 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/completion.meta.json
+-rw-r--r--   0        0        0     3577 2023-03-05 14:00:03.528756 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/cpr.data.json
+-rw-r--r--   0        0        0     2345 2023-03-05 14:01:11.113821 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/cpr.meta.json
+-rw-r--r--   0        0        0     8228 2023-03-05 14:00:03.560614 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/emacs.data.json
+-rw-r--r--   0        0        0     2850 2023-03-05 14:01:11.139253 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/emacs.meta.json
+-rw-r--r--   0        0        0     4040 2023-03-05 14:00:03.529641 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/focus.data.json
+-rw-r--r--   0        0        0     2109 2023-03-05 14:01:11.114482 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/focus.meta.json
+-rw-r--r--   0        0        0    13631 2023-03-05 14:00:03.528353 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/mouse.data.json
+-rw-r--r--   0        0        0     2531 2023-03-05 14:01:11.113528 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/mouse.meta.json
+-rw-r--r--   0        0        0    78608 2023-03-05 14:00:03.559305 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/named_commands.data.json
+-rw-r--r--   0        0        0     3170 2023-03-05 14:01:11.138100 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/named_commands.meta.json
+-rw-r--r--   0        0        0     5555 2023-03-05 14:00:03.561420 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/open_in_editor.data.json
+-rw-r--r--   0        0        0     2214 2023-03-05 14:01:11.139894 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/open_in_editor.meta.json
+-rw-r--r--   0        0        0     6935 2023-03-05 14:00:03.533578 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/page_navigation.data.json
+-rw-r--r--   0        0        0     2209 2023-03-05 14:01:11.117715 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/page_navigation.meta.json
+-rw-r--r--   0        0        0     8523 2023-03-05 14:00:03.527776 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/scroll.data.json
+-rw-r--r--   0        0        0     2352 2023-03-05 14:01:11.113082 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/scroll.meta.json
+-rw-r--r--   0        0        0    11950 2023-03-05 14:00:03.526520 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/search.data.json
+-rw-r--r--   0        0        0     2458 2023-03-05 14:01:11.112155 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/search.meta.json
+-rw-r--r--   0        0        0    31790 2023-03-05 14:00:03.560166 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/vi.data.json
+-rw-r--r--   0        0        0     3266 2023-03-05 14:01:11.138884 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/vi.meta.json
+-rw-r--r--   0        0        0     4865 2023-03-05 14:00:03.565383 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/defaults.data.json
+-rw-r--r--   0        0        0     2330 2023-03-05 14:01:11.143655 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/defaults.meta.json
+-rw-r--r--   0        0        0     2898 2023-03-05 13:59:58.579433 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/digraphs.data.json
+-rw-r--r--   0        0        0     1695 2023-03-05 13:59:58.579686 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/digraphs.meta.json
+-rw-r--r--   0        0        0     8419 2023-03-05 14:00:03.529248 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/emacs_state.data.json
+-rw-r--r--   0        0        0     1926 2023-03-05 14:01:11.114191 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/emacs_state.meta.json
+-rw-r--r--   0        0        0    63950 2023-03-05 14:00:03.518054 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/key_bindings.data.json
+-rw-r--r--   0        0        0     2393 2023-03-05 14:01:11.105335 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/key_bindings.meta.json
+-rw-r--r--   0        0        0    41469 2023-03-05 14:00:03.524415 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/key_processor.data.json
+-rw-r--r--   0        0        0     2768 2023-03-05 14:01:11.110718 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/key_processor.meta.json
+-rw-r--r--   0        0        0    18190 2023-03-05 14:00:03.509475 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/vi_state.data.json
+-rw-r--r--   0        0        0     2127 2023-03-05 14:01:11.098012 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/vi_state.meta.json
+-rw-r--r--   0        0        0    70984 2023-03-05 13:59:58.605526 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/keys.data.json
+-rw-r--r--   0        0        0     1740 2023-03-05 13:59:58.605737 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/keys.meta.json
+-rw-r--r--   0        0        0     7543 2023-03-05 14:00:03.571697 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/__init__.data.json
+-rw-r--r--   0        0        0     2145 2023-03-05 14:01:11.149160 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/__init__.meta.json
+-rw-r--r--   0        0        0   185167 2023-03-05 14:00:03.564905 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/containers.data.json
+-rw-r--r--   0        0        0     3079 2023-03-05 14:01:11.143294 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/containers.meta.json
+-rw-r--r--   0        0        0   101505 2023-03-05 14:00:03.556850 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/controls.data.json
+-rw-r--r--   0        0        0     3148 2023-03-05 14:01:11.135918 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/controls.meta.json
+-rw-r--r--   0        0        0    17147 2023-03-05 13:59:58.598937 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/dimension.data.json
+-rw-r--r--   0        0        0     1799 2023-03-05 13:59:58.599164 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/dimension.meta.json
+-rw-r--r--   0        0        0     4023 2023-03-05 14:00:03.571262 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/dummy.data.json
+-rw-r--r--   0        0        0     2658 2023-03-05 14:01:11.148815 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/dummy.meta.json
+-rw-r--r--   0        0        0    35286 2023-03-05 14:00:03.568999 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/layout.data.json
+-rw-r--r--   0        0        0     2810 2023-03-05 14:01:11.146826 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/layout.meta.json
+-rw-r--r--   0        0        0    28065 2023-03-05 14:00:03.557669 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/margins.data.json
+-rw-r--r--   0        0        0     2407 2023-03-05 14:01:11.136628 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/margins.meta.json
+-rw-r--r--   0        0        0    41688 2023-03-05 14:00:03.568023 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/menus.data.json
+-rw-r--r--   0        0        0     3168 2023-03-05 14:01:11.145985 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/menus.meta.json
+-rw-r--r--   0        0        0     6947 2023-03-05 14:00:03.508100 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/mouse_handlers.data.json
+-rw-r--r--   0        0        0     2029 2023-03-05 14:01:11.096881 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/mouse_handlers.meta.json
+-rw-r--r--   0        0        0    80241 2023-03-05 14:00:03.547414 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/processors.data.json
+-rw-r--r--   0        0        0     3173 2023-03-05 14:01:11.128714 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/processors.meta.json
+-rw-r--r--   0        0        0    26873 2023-03-05 14:00:03.507434 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/screen.data.json
+-rw-r--r--   0        0        0     2098 2023-03-05 14:01:11.096386 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/screen.meta.json
+-rw-r--r--   0        0        0    24465 2023-03-05 14:00:03.567022 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/scrollable_pane.data.json
+-rw-r--r--   0        0        0     2708 2023-03-05 14:01:11.145064 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/scrollable_pane.meta.json
+-rw-r--r--   0        0        0    37663 2023-03-05 14:00:03.512077 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/utils.data.json
+-rw-r--r--   0        0        0     1981 2023-03-05 14:01:11.100444 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/utils.meta.json
+-rw-r--r--   0        0        0     3133 2023-03-05 14:00:03.535778 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/__init__.data.json
+-rw-r--r--   0        0        0     1928 2023-03-05 14:01:11.119505 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/__init__.meta.json
+-rw-r--r--   0        0        0    14260 2023-03-05 14:00:03.522261 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/base.data.json
+-rw-r--r--   0        0        0     1968 2023-03-05 14:01:11.109047 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/base.meta.json
+-rw-r--r--   0        0        0    23666 2023-03-05 14:01:11.115063 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/pygments.data.json
+-rw-r--r--   0        0        0     2335 2023-03-05 14:01:11.115276 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/pygments.meta.json
+-rw-r--r--   0        0        0    14038 2023-03-05 13:59:59.135212 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/mouse_events.data.json
+-rw-r--r--   0        0        0     1735 2023-03-05 13:59:59.135487 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/mouse_events.meta.json
+-rw-r--r--   0        0        0     2777 2023-03-05 14:00:03.539520 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/__init__.data.json
+-rw-r--r--   0        0        0     1971 2023-03-05 14:01:11.122252 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/__init__.meta.json
+-rw-r--r--   0        0        0    78156 2023-03-05 14:00:03.532689 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/base.data.json
+-rw-r--r--   0        0        0     2124 2023-03-05 14:01:11.117090 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/base.meta.json
+-rw-r--r--   0        0        0    10286 2023-03-05 14:00:03.513069 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/color_depth.data.json
+-rw-r--r--   0        0        0     2025 2023-03-05 14:01:11.101293 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/color_depth.meta.json
+-rw-r--r--   0        0        0     4358 2023-03-05 14:00:03.538159 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/defaults.data.json
+-rw-r--r--   0        0        0     2230 2023-03-05 14:01:11.121182 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/defaults.meta.json
+-rw-r--r--   0        0        0     5097 2023-03-05 13:59:58.583627 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/flush_stdout.data.json
+-rw-r--r--   0        0        0     1754 2023-03-05 13:59:58.583829 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/flush_stdout.meta.json
+-rw-r--r--   0        0        0    31425 2023-03-05 14:00:03.534472 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/plain_text.data.json
+-rw-r--r--   0        0        0     2216 2023-03-05 14:01:11.118456 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/plain_text.meta.json
+-rw-r--r--   0        0        0    55786 2023-03-05 14:00:03.541081 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/vt100.data.json
+-rw-r--r--   0        0        0     2366 2023-03-05 14:01:11.123435 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/vt100.meta.json
+-rw-r--r--   0        0        0    23377 2023-03-05 14:00:03.582292 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/patch_stdout.data.json
+-rw-r--r--   0        0        0     2310 2023-03-05 14:01:11.158109 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/patch_stdout.meta.json
+-rw-r--r--   0        0        0    42172 2023-03-05 14:00:03.543253 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/renderer.data.json
+-rw-r--r--   0        0        0     2974 2023-03-05 14:01:11.125217 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/renderer.meta.json
+-rw-r--r--   0        0        0    13392 2023-03-05 14:00:03.519722 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/search.data.json
+-rw-r--r--   0        0        0     2713 2023-03-05 14:01:11.106749 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/search.meta.json
+-rw-r--r--   0        0        0     9949 2023-03-05 13:59:58.601265 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/selection.data.json
+-rw-r--r--   0        0        0     1686 2023-03-05 13:59:58.601458 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/selection.meta.json
+-rw-r--r--   0        0        0     4761 2023-03-05 14:00:03.583148 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/__init__.data.json
+-rw-r--r--   0        0        0     2031 2023-03-05 14:01:11.158956 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/__init__.meta.json
+-rw-r--r--   0        0        0    22151 2023-03-05 14:00:03.579243 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/dialogs.data.json
+-rw-r--r--   0        0        0     3893 2023-03-05 14:01:11.155439 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/dialogs.meta.json
+-rw-r--r--   0        0        0     4211 2023-03-05 14:00:03.582741 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/__init__.data.json
+-rw-r--r--   0        0        0     1994 2023-03-05 14:01:11.158447 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/__init__.meta.json
+-rw-r--r--   0        0        0    51945 2023-03-05 14:00:03.577848 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/base.data.json
+-rw-r--r--   0        0        0     3590 2023-03-05 14:01:11.154271 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/base.meta.json
+-rw-r--r--   0        0        0    49462 2023-03-05 14:00:03.544527 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/formatters.data.json
+-rw-r--r--   0        0        0     2456 2023-03-05 14:01:11.126233 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/formatters.meta.json
+-rw-r--r--   0        0        0   103285 2023-03-05 14:00:03.581359 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/prompt.data.json
+-rw-r--r--   0        0        0     4315 2023-03-05 14:01:11.157391 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/prompt.meta.json
+-rw-r--r--   0        0        0    10977 2023-03-05 14:00:03.578474 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/utils.data.json
+-rw-r--r--   0        0        0     3245 2023-03-05 14:01:11.154749 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/utils.meta.json
+-rw-r--r--   0        0        0     5819 2023-03-05 14:00:03.525016 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/__init__.data.json
+-rw-r--r--   0        0        0     2107 2023-03-05 14:01:11.111048 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/__init__.meta.json
+-rw-r--r--   0        0        0    52830 2023-03-05 13:59:58.825893 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/base.data.json
+-rw-r--r--   0        0        0     1701 2023-03-05 13:59:58.826108 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/base.meta.json
+-rw-r--r--   0        0        0     7461 2023-03-05 13:59:59.540204 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/defaults.data.json
+-rw-r--r--   0        0        0     1896 2023-03-05 13:59:59.540393 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/defaults.meta.json
+-rw-r--r--   0        0        0     2547 2023-03-05 13:59:58.820538 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/named_colors.data.json
+-rw-r--r--   0        0        0     1691 2023-03-05 13:59:58.820746 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/named_colors.meta.json
+-rw-r--r--   0        0        0     5208 2023-03-05 14:01:08.821870 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/pygments.data.json
+-rw-r--r--   0        0        0     1922 2023-03-05 14:01:08.822152 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/pygments.meta.json
+-rw-r--r--   0        0        0    28427 2023-03-05 13:59:59.216223 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/style.data.json
+-rw-r--r--   0        0        0     1913 2023-03-05 13:59:59.216445 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/style.meta.json
+-rw-r--r--   0        0        0    43235 2023-03-05 14:00:03.519116 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/style_transformation.data.json
+-rw-r--r--   0        0        0     2334 2023-03-05 14:01:11.106259 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/style_transformation.meta.json
+-rw-r--r--   0        0        0    33097 2023-03-05 13:59:58.840698 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/utils.data.json
+-rw-r--r--   0        0        0     1914 2023-03-05 13:59:58.840966 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/utils.meta.json
+-rw-r--r--   0        0        0    28835 2023-03-05 14:00:03.523097 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/validation.data.json
+-rw-r--r--   0        0        0     2113 2023-03-05 14:01:11.109783 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/validation.meta.json
+-rw-r--r--   0        0        0     4794 2023-03-05 14:00:03.575562 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/__init__.data.json
+-rw-r--r--   0        0        0     2015 2023-03-05 14:01:11.152484 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/__init__.meta.json
+-rw-r--r--   0        0        0    88345 2023-03-05 14:00:03.570849 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/base.data.json
+-rw-r--r--   0        0        0     3384 2023-03-05 14:01:11.148510 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/base.meta.json
+-rw-r--r--   0        0        0     8559 2023-03-05 14:00:03.572183 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/dialogs.data.json
+-rw-r--r--   0        0        0     2599 2023-03-05 14:01:11.149540 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/dialogs.meta.json
+-rw-r--r--   0        0        0    20393 2023-03-05 14:00:03.575101 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/menus.data.json
+-rw-r--r--   0        0        0     2878 2023-03-05 14:01:11.152174 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/menus.meta.json
+-rw-r--r--   0        0        0    29788 2023-03-05 14:00:03.566267 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/toolbars.data.json
+-rw-r--r--   0        0        0     3364 2023-03-05 14:01:11.144407 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/toolbars.meta.json
+-rw-r--r--   0        0        0    42144 2023-03-05 13:59:58.683257 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pstats.data.json
+-rw-r--r--   0        0        0     1806 2023-03-05 13:59:58.683502 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pstats.meta.json
+-rw-r--r--   0        0        0    69566 2023-03-05 14:01:08.872765 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/psutil/__init__.data.json
+-rw-r--r--   0        0        0     1817 2023-03-05 14:01:08.873013 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/psutil/__init__.meta.json
+-rw-r--r--   0        0        0   459802 2023-03-05 14:01:08.659690 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/psutil/_common.data.json
+-rw-r--r--   0        0        0     1753 2023-03-05 14:01:08.659947 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/psutil/_common.meta.json
+-rw-r--r--   0        0        0   106929 2023-03-05 14:01:08.773963 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/psutil/_psosx.data.json
+-rw-r--r--   0        0        0     1679 2023-03-05 14:01:08.774170 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/psutil/_psosx.meta.json
+-rw-r--r--   0        0        0     2307 2023-03-05 14:00:01.656772 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pure_eval/__init__.data.json
+-rw-r--r--   0        0        0     1767 2023-03-05 14:00:01.657005 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pure_eval/__init__.meta.json
+-rw-r--r--   0        0        0    17272 2023-03-05 14:00:01.089774 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pure_eval/core.data.json
+-rw-r--r--   0        0        0     2009 2023-03-05 14:00:01.090032 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pure_eval/core.meta.json
+-rw-r--r--   0        0        0     7726 2023-03-05 14:00:00.931825 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pure_eval/my_getattr_static.data.json
+-rw-r--r--   0        0        0     1833 2023-03-05 14:00:00.932028 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pure_eval/my_getattr_static.meta.json
+-rw-r--r--   0        0        0    14265 2023-03-05 13:59:59.650997 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pure_eval/utils.data.json
+-rw-r--r--   0        0        0     1995 2023-03-05 13:59:59.651237 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pure_eval/utils.meta.json
+-rw-r--r--   0        0        0     1658 2023-03-05 13:59:57.866253 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pure_eval/version.data.json
+-rw-r--r--   0        0        0     1636 2023-03-05 13:59:57.866489 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pure_eval/version.meta.json
+-rw-r--r--   0        0        0   109208 2023-03-05 13:59:58.903390 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pydoc.data.json
+-rw-r--r--   0        0        0     1752 2023-03-05 13:59:58.903602 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pydoc.meta.json
+-rw-r--r--   0        0        0    38603 2023-03-05 13:59:58.848848 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pyexpat/__init__.data.json
+-rw-r--r--   0        0        0     1833 2023-03-05 13:59:58.849050 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pyexpat/__init__.meta.json
+-rw-r--r--   0        0        0    11077 2023-03-05 13:59:57.909966 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pyexpat/errors.data.json
+-rw-r--r--   0        0        0     1688 2023-03-05 13:59:57.910157 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pyexpat/errors.meta.json
+-rw-r--r--   0        0        0     3512 2023-03-05 13:59:57.908745 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pyexpat/model.data.json
+-rw-r--r--   0        0        0     1651 2023-03-05 13:59:57.908933 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pyexpat/model.meta.json
+-rw-r--r--   0        0        0    15061 2023-03-05 14:01:08.569581 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/__init__.data.json
+-rw-r--r--   0        0        0     1681 2023-03-05 14:01:08.569795 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/__init__.meta.json
+-rw-r--r--   0        0        0    12596 2023-03-05 14:01:08.405329 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatter.data.json
+-rw-r--r--   0        0        0     1645 2023-03-05 14:01:08.405519 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatter.meta.json
+-rw-r--r--   0        0        0     6802 2023-03-05 14:01:08.847511 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/__init__.data.json
+-rw-r--r--   0        0        0     2110 2023-03-05 14:01:08.847755 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/__init__.meta.json
+-rw-r--r--   0        0        0     5938 2023-03-05 14:01:08.557698 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/bbcode.data.json
+-rw-r--r--   0        0        0     1689 2023-03-05 14:01:08.557896 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/bbcode.meta.json
+-rw-r--r--   0        0        0    17954 2023-03-05 14:01:08.556823 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/html.data.json
+-rw-r--r--   0        0        0     1705 2023-03-05 14:01:08.557015 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/html.meta.json
+-rw-r--r--   0        0        0    26743 2023-03-05 14:01:08.555019 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/img.data.json
+-rw-r--r--   0        0        0     1684 2023-03-05 14:01:08.555233 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/img.meta.json
+-rw-r--r--   0        0        0     6457 2023-03-05 14:01:08.552601 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/irc.data.json
+-rw-r--r--   0        0        0     1683 2023-03-05 14:01:08.552782 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/irc.meta.json
+-rw-r--r--   0        0        0    14567 2023-03-05 14:01:08.708006 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/latex.data.json
+-rw-r--r--   0        0        0     1711 2023-03-05 14:01:08.708197 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/latex.meta.json
+-rw-r--r--   0        0        0    13276 2023-03-05 14:01:08.551691 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/other.data.json
+-rw-r--r--   0        0        0     1687 2023-03-05 14:01:08.551893 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/other.meta.json
+-rw-r--r--   0        0        0     6133 2023-03-05 14:01:08.549981 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/pangomarkup.data.json
+-rw-r--r--   0        0        0     1699 2023-03-05 14:01:08.550172 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/pangomarkup.meta.json
+-rw-r--r--   0        0        0     6142 2023-03-05 14:01:08.549117 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/rtf.data.json
+-rw-r--r--   0        0        0     1683 2023-03-05 14:01:08.549296 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/rtf.meta.json
+-rw-r--r--   0        0        0     8986 2023-03-05 14:01:08.548241 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/svg.data.json
+-rw-r--r--   0        0        0     1683 2023-03-05 14:01:08.548444 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/svg.meta.json
+-rw-r--r--   0        0        0     6969 2023-03-05 14:01:08.547226 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/terminal.data.json
+-rw-r--r--   0        0        0     1693 2023-03-05 14:01:08.547431 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/terminal.meta.json
+-rw-r--r--   0        0        0    15695 2023-03-05 14:01:08.546168 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/terminal256.data.json
+-rw-r--r--   0        0        0     1719 2023-03-05 14:01:08.546412 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/formatters/terminal256.meta.json
+-rw-r--r--   0        0        0    43182 2023-03-05 14:01:08.562689 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/lexer.data.json
+-rw-r--r--   0        0        0     1729 2023-03-05 14:01:08.562915 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/lexer.meta.json
+-rw-r--r--   0        0        0    11933 2023-03-05 14:01:08.738330 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/lexers/__init__.data.json
+-rw-r--r--   0        0        0     1767 2023-03-05 14:01:08.738589 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/lexers/__init__.meta.json
+-rw-r--r--   0        0        0    11959 2023-03-05 14:01:08.535060 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/style.data.json
+-rw-r--r--   0        0        0     1715 2023-03-05 14:01:08.535256 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/style.meta.json
+-rw-r--r--   0        0        0     4682 2023-03-05 14:01:08.705469 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/styles/__init__.data.json
+-rw-r--r--   0        0        0     1777 2023-03-05 14:01:08.705656 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/styles/__init__.meta.json
+-rw-r--r--   0        0        0    11861 2023-03-05 14:01:08.393198 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/token.data.json
+-rw-r--r--   0        0        0     1689 2023-03-05 14:01:08.393434 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/token.meta.json
+-rw-r--r--   0        0        0    15519 2023-03-05 14:01:08.385877 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/util.data.json
+-rw-r--r--   0        0        0     1667 2023-03-05 14:01:08.386074 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/pygments/util.meta.json
+-rw-r--r--   0        0        0    32155 2023-03-05 13:59:58.879428 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/queue.data.json
+-rw-r--r--   0        0        0     1703 2023-03-05 13:59:58.879625 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/queue.meta.json
+-rw-r--r--   0        0        0    44133 2023-03-05 13:59:59.843167 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/random.data.json
+-rw-r--r--   0        0        0     1799 2023-03-05 13:59:59.843414 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/random.meta.json
+-rw-r--r--   0        0        0   151207 2023-03-05 13:59:57.780628 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1855 2023-03-05 13:59:57.780826 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    17427 2023-03-05 13:59:58.064688 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/reprlib.data.json
+-rw-r--r--   0        0        0     1727 2023-03-05 13:59:58.064875 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/reprlib.meta.json
+-rw-r--r--   0        0        0    43927 2023-03-05 13:59:57.894462 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/resource.data.json
+-rw-r--r--   0        0        0     1701 2023-03-05 13:59:57.894677 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/resource.meta.json
+-rw-r--r--   0        0        0    11069 2023-03-05 13:59:58.268268 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/runpy.data.json
+-rw-r--r--   0        0        0     1668 2023-03-05 13:59:58.268457 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/runpy.meta.json
+-rw-r--r--   0        0        0    25728 2023-03-05 13:59:57.927952 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/select.data.json
+-rw-r--r--   0        0        0     1737 2023-03-05 13:59:57.928161 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/select.meta.json
+-rw-r--r--   0        0        0    58547 2023-03-05 13:59:57.937087 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selectors.data.json
+-rw-r--r--   0        0        0     1792 2023-03-05 13:59:57.937305 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selectors.meta.json
+-rw-r--r--   0        0        0     1844 2023-03-05 13:59:58.480737 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/__init__.data.json
+-rw-r--r--   0        0        0     1628 2023-03-05 13:59:58.480934 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/__init__.meta.json
+-rw-r--r--   0        0        0     6903 2023-03-05 13:59:59.002365 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/common/__init__.data.json
+-rw-r--r--   0        0        0     1680 2023-03-05 13:59:59.002544 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/common/__init__.meta.json
+-rw-r--r--   0        0        0    37581 2023-03-05 13:59:58.462559 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/common/exceptions.data.json
+-rw-r--r--   0        0        0     1656 2023-03-05 13:59:58.462770 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/common/exceptions.meta.json
+-rw-r--r--   0        0        0     2578 2023-03-05 13:59:58.458282 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/types.data.json
+-rw-r--r--   0        0        0     1633 2023-03-05 13:59:58.458458 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/types.meta.json
+-rw-r--r--   0        0        0     4859 2023-03-05 14:00:03.770536 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/__init__.data.json
+-rw-r--r--   0        0        0     2704 2023-03-05 14:00:03.770741 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/__init__.meta.json
+-rw-r--r--   0        0        0     1748 2023-03-05 13:59:58.477153 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/__init__.data.json
+-rw-r--r--   0        0        0     1662 2023-03-05 13:59:58.477376 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/__init__.meta.json
+-rw-r--r--   0        0        0     5742 2023-03-05 13:59:59.639120 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/options.data.json
+-rw-r--r--   0        0        0     1940 2023-03-05 13:59:59.639342 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/options.meta.json
+-rw-r--r--   0        0        0     4143 2023-03-05 14:00:02.030949 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/service.data.json
+-rw-r--r--   0        0        0     2015 2023-03-05 14:00:02.031189 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/service.meta.json
+-rw-r--r--   0        0        0     5832 2023-03-05 14:00:02.561027 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/webdriver.data.json
+-rw-r--r--   0        0        0     2402 2023-03-05 14:00:02.561377 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/webdriver.meta.json
+-rw-r--r--   0        0        0     1764 2023-03-05 13:59:58.457669 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/__init__.data.json
+-rw-r--r--   0        0        0     1666 2023-03-05 13:59:58.457841 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/__init__.meta.json
+-rw-r--r--   0        0        0    24423 2023-03-05 13:59:59.465110 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/options.data.json
+-rw-r--r--   0        0        0     1987 2023-03-05 13:59:59.465353 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/options.meta.json
+-rw-r--r--   0        0        0     3914 2023-03-05 13:59:59.846450 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/remote_connection.data.json
+-rw-r--r--   0        0        0     1834 2023-03-05 14:01:09.707289 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/remote_connection.meta.json
+-rw-r--r--   0        0        0     5123 2023-03-05 14:00:01.728428 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/service.data.json
+-rw-r--r--   0        0        0     1806 2023-03-05 14:00:01.728644 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/service.meta.json
+-rw-r--r--   0        0        0    17717 2023-03-05 14:00:02.245859 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/webdriver.data.json
+-rw-r--r--   0        0        0     2395 2023-03-05 14:01:09.882553 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/webdriver.meta.json
+-rw-r--r--   0        0        0     1748 2023-03-05 13:59:58.479874 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/__init__.data.json
+-rw-r--r--   0        0        0     1662 2023-03-05 13:59:58.480235 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/__init__.meta.json
+-rw-r--r--   0        0        0    13594 2023-03-05 14:00:02.559460 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/action_chains.data.json
+-rw-r--r--   0        0        0     2279 2023-03-05 14:00:02.559702 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/action_chains.meta.json
+-rw-r--r--   0        0        0     1812 2023-03-05 13:59:58.230822 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/__init__.data.json
+-rw-r--r--   0        0        0     1678 2023-03-05 13:59:58.231048 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/__init__.meta.json
+-rw-r--r--   0        0        0    21140 2023-03-05 14:00:02.240410 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/action_builder.data.json
+-rw-r--r--   0        0        0     2479 2023-03-05 14:00:02.240641 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/action_builder.meta.json
+-rw-r--r--   0        0        0     4359 2023-03-05 13:59:58.986060 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/input_device.data.json
+-rw-r--r--   0        0        0     1712 2023-03-05 13:59:58.986263 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/input_device.meta.json
+-rw-r--r--   0        0        0     9216 2023-03-05 13:59:58.230235 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/interaction.data.json
+-rw-r--r--   0        0        0     1808 2023-03-05 13:59:58.230476 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/interaction.meta.json
+-rw-r--r--   0        0        0     4805 2023-03-05 14:00:01.120893 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/key_actions.data.json
+-rw-r--r--   0        0        0     1952 2023-03-05 14:00:01.121091 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/key_actions.meta.json
+-rw-r--r--   0        0        0    11074 2023-03-05 13:59:59.307061 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/key_input.data.json
+-rw-r--r--   0        0        0     1897 2023-03-05 13:59:59.307264 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/key_input.meta.json
+-rw-r--r--   0        0        0     3890 2023-03-05 13:59:58.013797 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/mouse_button.data.json
+-rw-r--r--   0        0        0     1695 2023-03-05 13:59:58.013992 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/mouse_button.meta.json
+-rw-r--r--   0        0        0     8252 2023-03-05 14:00:01.965347 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/pointer_actions.data.json
+-rw-r--r--   0        0        0     2349 2023-03-05 14:00:01.965546 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/pointer_actions.meta.json
+-rw-r--r--   0        0        0     7552 2023-03-05 14:00:01.726869 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/pointer_input.data.json
+-rw-r--r--   0        0        0     2147 2023-03-05 14:00:01.727092 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/pointer_input.meta.json
+-rw-r--r--   0        0        0     4270 2023-03-05 14:00:01.963113 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/wheel_actions.data.json
+-rw-r--r--   0        0        0     2045 2023-03-05 14:00:01.963335 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/wheel_actions.meta.json
+-rw-r--r--   0        0        0    17775 2023-03-05 14:00:01.820500 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/wheel_input.data.json
+-rw-r--r--   0        0        0     2227 2023-03-05 14:00:01.820753 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/wheel_input.meta.json
+-rw-r--r--   0        0        0     4852 2023-03-05 14:00:01.119604 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/alert.data.json
+-rw-r--r--   0        0        0     1837 2023-03-05 14:00:01.119821 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/alert.meta.json
+-rw-r--r--   0        0        0     4382 2023-03-05 13:59:58.495870 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/by.data.json
+-rw-r--r--   0        0        0     1660 2023-03-05 13:59:58.496060 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/by.meta.json
+-rw-r--r--   0        0        0     6606 2023-03-05 13:59:58.476553 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/desired_capabilities.data.json
+-rw-r--r--   0        0        0     1696 2023-03-05 13:59:58.476789 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/desired_capabilities.meta.json
+-rw-r--r--   0        0        0     1796 2023-03-05 13:59:58.227666 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/html5/__init__.data.json
+-rw-r--r--   0        0        0     1674 2023-03-05 13:59:58.227892 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/html5/__init__.meta.json
+-rw-r--r--   0        0        0     6289 2023-03-05 13:59:59.445296 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/html5/application_cache.data.json
+-rw-r--r--   0        0        0     1871 2023-03-05 13:59:59.445493 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/html5/application_cache.meta.json
+-rw-r--r--   0        0        0    19713 2023-03-05 13:59:58.475277 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/keys.data.json
+-rw-r--r--   0        0        0     1664 2023-03-05 13:59:58.475501 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/keys.meta.json
+-rw-r--r--   0        0        0    43425 2023-03-05 13:59:59.054328 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/options.data.json
+-rw-r--r--   0        0        0     1777 2023-03-05 13:59:59.054544 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/options.meta.json
+-rw-r--r--   0        0        0    46958 2023-03-05 13:59:58.398912 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/print_page_options.data.json
+-rw-r--r--   0        0        0     1820 2023-03-05 13:59:58.399164 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/print_page_options.meta.json
+-rw-r--r--   0        0        0    41912 2023-03-05 13:59:58.473632 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/proxy.data.json
+-rw-r--r--   0        0        0     1752 2023-03-05 13:59:58.473894 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/proxy.meta.json
+-rw-r--r--   0        0        0     7869 2023-03-05 13:59:59.219877 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/selenium_manager.data.json
+-rw-r--r--   0        0        0     1931 2023-03-05 13:59:59.220107 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/selenium_manager.meta.json
+-rw-r--r--   0        0        0    16679 2023-03-05 14:00:01.133259 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/service.data.json
+-rw-r--r--   0        0        0     2273 2023-03-05 14:00:01.133512 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/service.meta.json
+-rw-r--r--   0        0        0    15320 2023-03-05 13:59:58.390831 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/timeouts.data.json
+-rw-r--r--   0        0        0     1800 2023-03-05 13:59:58.391093 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/timeouts.meta.json
+-rw-r--r--   0        0        0    10986 2023-03-05 14:00:01.039296 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/utils.data.json
+-rw-r--r--   0        0        0     2005 2023-03-05 14:00:01.039586 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/utils.meta.json
+-rw-r--r--   0        0        0    34270 2023-03-05 13:59:59.042615 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/virtual_authenticator.data.json
+-rw-r--r--   0        0        0     1865 2023-03-05 13:59:59.042892 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/virtual_authenticator.meta.json
+-rw-r--r--   0        0        0     1732 2023-03-05 13:59:58.427753 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/__init__.data.json
+-rw-r--r--   0        0        0     1658 2023-03-05 13:59:58.427937 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/__init__.meta.json
+-rw-r--r--   0        0        0     9581 2023-03-05 13:59:59.638037 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/options.data.json
+-rw-r--r--   0        0        0     1936 2023-03-05 13:59:59.638271 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/options.meta.json
+-rw-r--r--   0        0        0     4244 2023-03-05 14:00:02.029970 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/service.data.json
+-rw-r--r--   0        0        0     2032 2023-03-05 14:00:02.030205 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/service.meta.json
+-rw-r--r--   0        0        0     6213 2023-03-05 14:00:02.556215 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/webdriver.data.json
+-rw-r--r--   0        0        0     2394 2023-03-05 14:00:02.556578 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/webdriver.meta.json
+-rw-r--r--   0        0        0     1756 2023-03-05 13:59:58.427243 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/__init__.data.json
+-rw-r--r--   0        0        0     1664 2023-03-05 13:59:58.427435 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/__init__.meta.json
+-rw-r--r--   0        0        0     9555 2023-03-05 14:00:01.316839 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/firefox_binary.data.json
+-rw-r--r--   0        0        0     2077 2023-03-05 14:00:01.317040 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/firefox_binary.meta.json
+-rw-r--r--   0        0        0    21852 2023-03-05 14:00:01.340092 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/firefox_profile.data.json
+-rw-r--r--   0        0        0     2327 2023-03-05 14:00:01.340400 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/firefox_profile.meta.json
+-rw-r--r--   0        0        0    26663 2023-03-05 14:00:01.861506 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/options.data.json
+-rw-r--r--   0        0        0     2255 2023-03-05 14:00:01.861745 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/options.meta.json
+-rw-r--r--   0        0        0     4316 2023-03-05 13:59:59.847547 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/remote_connection.data.json
+-rw-r--r--   0        0        0     1924 2023-03-05 14:01:09.709165 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/remote_connection.meta.json
+-rw-r--r--   0        0        0     5364 2023-03-05 14:00:01.816861 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/service.data.json
+-rw-r--r--   0        0        0     1988 2023-03-05 14:00:01.817084 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/service.meta.json
+-rw-r--r--   0        0        0    17781 2023-03-05 14:00:02.336923 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/webdriver.data.json
+-rw-r--r--   0        0        0     2675 2023-03-05 14:01:09.894607 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/webdriver.meta.json
+-rw-r--r--   0        0        0     1716 2023-03-05 13:59:58.400110 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/__init__.data.json
+-rw-r--r--   0        0        0     1654 2023-03-05 13:59:58.400332 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/__init__.meta.json
+-rw-r--r--   0        0        0    70437 2023-03-05 13:59:59.459397 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/options.data.json
+-rw-r--r--   0        0        0     1977 2023-03-05 13:59:59.459674 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/options.meta.json
+-rw-r--r--   0        0        0     5028 2023-03-05 14:00:01.815292 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/service.data.json
+-rw-r--r--   0        0        0     1922 2023-03-05 14:00:01.815533 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/service.meta.json
+-rw-r--r--   0        0        0     8894 2023-03-05 14:00:02.330586 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/webdriver.data.json
+-rw-r--r--   0        0        0     2195 2023-03-05 14:00:02.330815 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/webdriver.meta.json
+-rw-r--r--   0        0        0     1748 2023-03-05 13:59:58.399530 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/__init__.data.json
+-rw-r--r--   0        0        0     1662 2023-03-05 13:59:58.399758 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/__init__.meta.json
+-rw-r--r--   0        0        0     4438 2023-03-05 13:59:58.387843 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/bidi_connection.data.json
+-rw-r--r--   0        0        0     1685 2023-03-05 13:59:58.388030 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/bidi_connection.meta.json
+-rw-r--r--   0        0        0    25487 2023-03-05 13:59:58.387110 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/command.data.json
+-rw-r--r--   0        0        0     1670 2023-03-05 13:59:58.387296 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/command.meta.json
+-rw-r--r--   0        0        0    22349 2023-03-05 13:59:59.444269 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/errorhandler.data.json
+-rw-r--r--   0        0        0     1946 2023-03-05 13:59:59.444505 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/errorhandler.meta.json
+-rw-r--r--   0        0        0     8366 2023-03-05 14:00:01.313122 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/file_detector.data.json
+-rw-r--r--   0        0        0     1870 2023-03-05 14:00:01.313325 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/file_detector.meta.json
+-rw-r--r--   0        0        0    13913 2023-03-05 13:59:59.435452 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/mobile.data.json
+-rw-r--r--   0        0        0     1799 2023-03-05 13:59:59.435654 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/mobile.meta.json
+-rw-r--r--   0        0        0    17637 2023-03-05 14:01:09.671857 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/remote_connection.data.json
+-rw-r--r--   0        0        0     2303 2023-03-05 14:01:09.672163 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/remote_connection.meta.json
+-rw-r--r--   0        0        0     4936 2023-03-05 13:59:59.036999 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/script_key.data.json
+-rw-r--r--   0        0        0     1692 2023-03-05 13:59:59.037211 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/script_key.meta.json
+-rw-r--r--   0        0        0     8313 2023-03-05 13:59:59.035798 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/shadowroot.data.json
+-rw-r--r--   0        0        0     1926 2023-03-05 13:59:59.036042 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/shadowroot.meta.json
+-rw-r--r--   0        0        0    10787 2023-03-05 14:00:01.810133 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/switch_to.data.json
+-rw-r--r--   0        0        0     2226 2023-03-05 14:00:01.810446 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/switch_to.meta.json
+-rw-r--r--   0        0        0     3211 2023-03-05 13:59:59.305088 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/utils.data.json
+-rw-r--r--   0        0        0     1776 2023-03-05 13:59:59.305269 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/utils.meta.json
+-rw-r--r--   0        0        0    91970 2023-03-05 14:00:02.158329 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/webdriver.data.json
+-rw-r--r--   0        0        0     3414 2023-03-05 14:01:09.818020 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/webdriver.meta.json
+-rw-r--r--   0        0        0    40435 2023-03-05 14:00:01.332392 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/webelement.data.json
+-rw-r--r--   0        0        0     2291 2023-03-05 14:00:01.332692 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/webelement.meta.json
+-rw-r--r--   0        0        0     1748 2023-03-05 13:59:58.382463 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/__init__.data.json
+-rw-r--r--   0        0        0     1662 2023-03-05 13:59:58.382647 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/__init__.meta.json
+-rw-r--r--   0        0        0    22656 2023-03-05 13:59:59.433543 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/options.data.json
+-rw-r--r--   0        0        0     1877 2023-03-05 13:59:59.433770 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/options.meta.json
+-rw-r--r--   0        0        0     4073 2023-03-05 13:59:59.844344 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/remote_connection.data.json
+-rw-r--r--   0        0        0     1922 2023-03-05 14:01:09.704850 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/remote_connection.meta.json
+-rw-r--r--   0        0        0     8421 2023-03-05 14:00:01.807872 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/service.data.json
+-rw-r--r--   0        0        0     1989 2023-03-05 14:00:01.808073 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/service.meta.json
+-rw-r--r--   0        0        0     7381 2023-03-05 14:00:02.327877 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/webdriver.data.json
+-rw-r--r--   0        0        0     2450 2023-03-05 14:01:09.887455 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/webdriver.meta.json
+-rw-r--r--   0        0        0     1756 2023-03-05 13:59:58.477751 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/__init__.data.json
+-rw-r--r--   0        0        0     1664 2023-03-05 13:59:58.477991 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/__init__.meta.json
+-rw-r--r--   0        0        0    13107 2023-03-05 14:00:01.813306 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/relative_locator.data.json
+-rw-r--r--   0        0        0     2089 2023-03-05 14:00:01.813550 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/relative_locator.meta.json
+-rw-r--r--   0        0        0    13030 2023-03-05 13:59:59.071510 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/select.data.json
+-rw-r--r--   0        0        0     1901 2023-03-05 13:59:59.071756 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/select.meta.json
+-rw-r--r--   0        0        0     1741 2023-03-05 13:59:59.485193 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/ui.data.json
+-rw-r--r--   0        0        0     1796 2023-03-05 13:59:59.485395 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/ui.meta.json
+-rw-r--r--   0        0        0     7966 2023-03-05 13:59:59.066790 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/wait.data.json
+-rw-r--r--   0        0        0     1884 2023-03-05 13:59:59.067008 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/wait.meta.json
+-rw-r--r--   0        0        0     1772 2023-03-05 13:59:58.379850 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/__init__.data.json
+-rw-r--r--   0        0        0     1668 2023-03-05 13:59:58.380038 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/__init__.meta.json
+-rw-r--r--   0        0        0    11454 2023-03-05 13:59:59.450822 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/options.data.json
+-rw-r--r--   0        0        0     1862 2023-03-05 13:59:59.451012 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/options.meta.json
+-rw-r--r--   0        0        0     5211 2023-03-05 14:00:01.805852 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/service.data.json
+-rw-r--r--   0        0        0     1950 2023-03-05 14:00:01.806083 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/service.meta.json
+-rw-r--r--   0        0        0     4048 2023-03-05 14:00:02.325486 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/webdriver.data.json
+-rw-r--r--   0        0        0     2197 2023-03-05 14:00:02.325674 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/webdriver.meta.json
+-rw-r--r--   0        0        0     1772 2023-03-05 13:59:58.379343 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/__init__.data.json
+-rw-r--r--   0        0        0     1668 2023-03-05 13:59:58.379536 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/__init__.meta.json
+-rw-r--r--   0        0        0     9242 2023-03-05 13:59:59.449381 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/options.data.json
+-rw-r--r--   0        0        0     1862 2023-03-05 13:59:59.449583 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/options.meta.json
+-rw-r--r--   0        0        0     5211 2023-03-05 14:00:01.804332 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/service.data.json
+-rw-r--r--   0        0        0     1950 2023-03-05 14:00:01.804576 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/service.meta.json
+-rw-r--r--   0        0        0     4065 2023-03-05 14:00:02.324511 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/webdriver.data.json
+-rw-r--r--   0        0        0     2163 2023-03-05 14:00:02.324702 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/webdriver.meta.json
+-rw-r--r--   0        0        0    17092 2023-03-05 13:59:58.314564 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/shlex.data.json
+-rw-r--r--   0        0        0     1693 2023-03-05 13:59:58.314747 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/shlex.meta.json
+-rw-r--r--   0        0        0    75994 2023-03-05 13:59:58.426675 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/shutil.data.json
+-rw-r--r--   0        0        0     1735 2023-03-05 13:59:58.426889 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/shutil.meta.json
+-rw-r--r--   0        0        0    33917 2023-03-05 13:59:58.251165 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/signal.data.json
+-rw-r--r--   0        0        0     1751 2023-03-05 13:59:58.251396 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/signal.meta.json
+-rw-r--r--   0        0        0    16136 2023-03-05 13:59:58.260551 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/site.data.json
+-rw-r--r--   0        0        0     1691 2023-03-05 13:59:58.260741 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/site.meta.json
+-rw-r--r--   0        0        0    65683 2023-03-05 14:01:09.716253 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/__init__.data.json
+-rw-r--r--   0        0        0     1931 2023-03-05 14:01:09.716470 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/__init__.meta.json
+-rw-r--r--   0        0        0     2064 2023-03-05 14:01:08.860692 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/BaseHTTPServer.data.json
+-rw-r--r--   0        0        0     1678 2023-03-05 14:01:08.860871 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/BaseHTTPServer.meta.json
+-rw-r--r--   0        0        0     2057 2023-03-05 14:01:08.860213 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/CGIHTTPServer.data.json
+-rw-r--r--   0        0        0     1676 2023-03-05 14:01:08.860400 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/CGIHTTPServer.meta.json
+-rw-r--r--   0        0        0     2078 2023-03-05 14:01:08.859711 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/SimpleHTTPServer.data.json
+-rw-r--r--   0        0        0     1682 2023-03-05 14:01:08.859911 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/SimpleHTTPServer.meta.json
+-rw-r--r--   0        0        0     8164 2023-03-05 14:01:09.683840 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/__init__.data.json
+-rw-r--r--   0        0        0     2932 2023-03-05 14:01:09.684044 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/__init__.meta.json
+-rw-r--r--   0        0        0     2552 2023-03-05 14:01:08.481099 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/_dummy_thread.data.json
+-rw-r--r--   0        0        0     1707 2023-03-05 14:01:08.481275 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/_dummy_thread.meta.json
+-rw-r--r--   0        0        0     2389 2023-03-05 14:01:08.480404 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/_thread.data.json
+-rw-r--r--   0        0        0     1660 2023-03-05 14:01:08.480583 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/_thread.meta.json
+-rw-r--r--   0        0        0    15901 2023-03-05 14:01:08.014732 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/builtins.data.json
+-rw-r--r--   0        0        0     1645 2023-03-05 14:01:08.014936 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/builtins.meta.json
+-rw-r--r--   0        0        0     8791 2023-03-05 14:01:08.013676 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/cPickle.data.json
+-rw-r--r--   0        0        0     1659 2023-03-05 14:01:08.013915 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/cPickle.meta.json
+-rw-r--r--   0        0        0     4004 2023-03-05 14:01:08.479822 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/configparser.data.json
+-rw-r--r--   0        0        0     1676 2023-03-05 14:01:08.480054 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/configparser.meta.json
+-rw-r--r--   0        0        0     1937 2023-03-05 14:01:08.479019 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/copyreg.data.json
+-rw-r--r--   0        0        0     1660 2023-03-05 14:01:08.479331 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/copyreg.meta.json
+-rw-r--r--   0        0        0     1579 2023-03-05 14:01:08.478031 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_base.data.json
+-rw-r--r--   0        0        0     1684 2023-03-05 14:01:08.478273 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_base.meta.json
+-rw-r--r--   0        0        0     1629 2023-03-05 14:01:08.626865 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_multipart.data.json
+-rw-r--r--   0        0        0     1699 2023-03-05 14:01:08.627075 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_multipart.meta.json
+-rw-r--r--   0        0        0     1659 2023-03-05 14:01:08.626329 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_nonmultipart.data.json
+-rw-r--r--   0        0        0     1708 2023-03-05 14:01:08.626548 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_nonmultipart.meta.json
+-rw-r--r--   0        0        0     1579 2023-03-05 14:01:08.761338 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_text.data.json
+-rw-r--r--   0        0        0     1684 2023-03-05 14:01:08.761510 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_text.meta.json
+-rw-r--r--   0        0        0     1879 2023-03-05 14:01:08.477365 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/html_entities.data.json
+-rw-r--r--   0        0        0     1678 2023-03-05 14:01:08.477625 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/html_entities.meta.json
+-rw-r--r--   0        0        0     1551 2023-03-05 14:01:08.625785 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/html_parser.data.json
+-rw-r--r--   0        0        0     1672 2023-03-05 14:01:08.626000 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/html_parser.meta.json
+-rw-r--r--   0        0        0     9807 2023-03-05 14:01:08.859213 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/http_client.data.json
+-rw-r--r--   0        0        0     1674 2023-03-05 14:01:08.859397 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/http_client.meta.json
+-rw-r--r--   0        0        0     2328 2023-03-05 14:01:09.042354 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/http_cookiejar.data.json
+-rw-r--r--   0        0        0     1681 2023-03-05 14:01:09.042539 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/http_cookiejar.meta.json
+-rw-r--r--   0        0        0     1860 2023-03-05 14:01:08.476775 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/http_cookies.data.json
+-rw-r--r--   0        0        0     1676 2023-03-05 14:01:08.476978 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/http_cookies.meta.json
+-rw-r--r--   0        0        0     1947 2023-03-05 14:01:08.625233 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/queue.data.json
+-rw-r--r--   0        0        0     1654 2023-03-05 14:01:08.625456 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/queue.meta.json
+-rw-r--r--   0        0        0     1695 2023-03-05 14:01:08.476257 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/reprlib.data.json
+-rw-r--r--   0        0        0     1660 2023-03-05 14:01:08.476466 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/reprlib.meta.json
+-rw-r--r--   0        0        0     3290 2023-03-05 14:01:08.760873 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/socketserver.data.json
+-rw-r--r--   0        0        0     1675 2023-03-05 14:01:08.761057 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/socketserver.meta.json
+-rw-r--r--   0        0        0    13745 2023-03-05 14:01:08.624657 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/tkinter.data.json
+-rw-r--r--   0        0        0     1660 2023-03-05 14:01:08.624893 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/tkinter.meta.json
+-rw-r--r--   0        0        0     1615 2023-03-05 14:01:08.475724 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_commondialog.data.json
+-rw-r--r--   0        0        0     1699 2023-03-05 14:01:08.475947 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_commondialog.meta.json
+-rw-r--r--   0        0        0     8903 2023-03-05 14:01:08.475179 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_constants.data.json
+-rw-r--r--   0        0        0     1690 2023-03-05 14:01:08.475408 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_constants.meta.json
+-rw-r--r--   0        0        0     1567 2023-03-05 14:01:08.760391 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_dialog.data.json
+-rw-r--r--   0        0        0     1681 2023-03-05 14:01:08.760557 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_dialog.meta.json
+-rw-r--r--   0        0        0     2937 2023-03-05 14:01:08.759938 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_filedialog.data.json
+-rw-r--r--   0        0        0     1693 2023-03-05 14:01:08.760115 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_filedialog.meta.json
+-rw-r--r--   0        0        0     2951 2023-03-05 14:01:08.759439 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_tkfiledialog.data.json
+-rw-r--r--   0        0        0     1697 2023-03-05 14:01:08.759625 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_tkfiledialog.meta.json
+-rw-r--r--   0        0        0     3891 2023-03-05 14:01:08.758918 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_ttk.data.json
+-rw-r--r--   0        0        0     1672 2023-03-05 14:01:08.759108 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_ttk.meta.json
+-rw-r--r--   0        0        0     2179 2023-03-05 14:01:09.071858 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1827 2023-03-05 14:01:09.072082 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib/__init__.meta.json
+-rw-r--r--   0        0        0     1775 2023-03-05 14:01:08.582253 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib/error.data.json
+-rw-r--r--   0        0        0     1676 2023-03-05 14:01:08.582452 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib/error.meta.json
+-rw-r--r--   0        0        0     3575 2023-03-05 14:01:08.467841 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib/parse.data.json
+-rw-r--r--   0        0        0     1676 2023-03-05 14:01:08.468008 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib/parse.meta.json
+-rw-r--r--   0        0        0     5326 2023-03-05 14:01:09.041831 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib/request.data.json
+-rw-r--r--   0        0        0     1683 2023-03-05 14:01:09.042020 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib/request.meta.json
+-rw-r--r--   0        0        0     1583 2023-03-05 14:01:08.467319 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib/response.data.json
+-rw-r--r--   0        0        0     1685 2023-03-05 14:01:08.467505 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib/response.meta.json
+-rw-r--r--   0        0        0     1617 2023-03-05 14:01:08.466847 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib/robotparser.data.json
+-rw-r--r--   0        0        0     1693 2023-03-05 14:01:08.467031 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib/robotparser.meta.json
+-rw-r--r--   0        0        0     1775 2023-03-05 14:01:08.623777 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib_error.data.json
+-rw-r--r--   0        0        0     1675 2023-03-05 14:01:08.624014 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib_error.meta.json
+-rw-r--r--   0        0        0     3613 2023-03-05 14:01:08.474479 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib_parse.data.json
+-rw-r--r--   0        0        0     1675 2023-03-05 14:01:08.474695 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib_parse.meta.json
+-rw-r--r--   0        0        0     1617 2023-03-05 14:01:08.473868 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib_robotparser.data.json
+-rw-r--r--   0        0        0     1693 2023-03-05 14:01:08.474094 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/six/moves/urllib_robotparser.meta.json
+-rw-r--r--   0        0        0    86759 2023-03-05 13:59:58.984945 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/socket.data.json
+-rw-r--r--   0        0        0     1843 2023-03-05 13:59:58.985175 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/socket.meta.json
+-rw-r--r--   0        0        0    65585 2023-03-05 13:59:59.133392 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/socketserver.data.json
+-rw-r--r--   0        0        0     1848 2023-03-05 13:59:59.133607 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/socketserver.meta.json
+-rw-r--r--   0        0        0    10113 2023-03-05 13:59:59.298601 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/sqlite3/__init__.data.json
+-rw-r--r--   0        0        0     1671 2023-03-05 13:59:59.298782 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/sqlite3/__init__.meta.json
+-rw-r--r--   0        0        0   128383 2023-03-05 13:59:59.298040 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/sqlite3/dbapi2.data.json
+-rw-r--r--   0        0        0     1868 2023-03-05 13:59:59.298273 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/sqlite3/dbapi2.meta.json
+-rw-r--r--   0        0        0    15087 2023-03-05 13:59:57.777717 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1700 2023-03-05 13:59:57.777888 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    29752 2023-03-05 13:59:57.777156 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1684 2023-03-05 13:59:57.777327 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    52521 2023-03-05 13:59:57.776302 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1764 2023-03-05 13:59:57.776497 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0   197333 2023-03-05 13:59:59.327668 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ssl.data.json
+-rw-r--r--   0        0        0     1894 2023-03-05 13:59:59.327914 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/ssl.meta.json
+-rw-r--r--   0        0        0     3342 2023-03-05 14:00:02.195008 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/stack_data/__init__.data.json
+-rw-r--r--   0        0        0     1926 2023-03-05 14:01:11.397050 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/stack_data/__init__.meta.json
+-rw-r--r--   0        0        0   109628 2023-03-05 14:00:01.911180 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/stack_data/core.data.json
+-rw-r--r--   0        0        0     2231 2023-03-05 14:01:11.362148 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/stack_data/core.meta.json
+-rw-r--r--   0        0        0    19167 2023-03-05 14:00:02.194559 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/stack_data/formatting.data.json
+-rw-r--r--   0        0        0     2169 2023-03-05 14:01:11.396750 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/stack_data/formatting.meta.json
+-rw-r--r--   0        0        0    18775 2023-03-05 14:00:02.193660 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/stack_data/serializing.data.json
+-rw-r--r--   0        0        0     2256 2023-03-05 14:01:11.396116 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/stack_data/serializing.meta.json
+-rw-r--r--   0        0        0    18281 2023-03-05 13:59:59.738055 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/stack_data/utils.data.json
+-rw-r--r--   0        0        0     1893 2023-03-05 14:01:10.054463 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/stack_data/utils.meta.json
+-rw-r--r--   0        0        0     1666 2023-03-05 13:59:57.973823 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/stack_data/version.data.json
+-rw-r--r--   0        0        0     1638 2023-03-05 13:59:57.974678 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/stack_data/version.meta.json
+-rw-r--r--   0        0        0     7079 2023-03-05 13:59:59.012156 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/stat.data.json
+-rw-r--r--   0        0        0     1647 2023-03-05 13:59:59.012326 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/stat.meta.json
+-rw-r--r--   0        0        0    28271 2023-03-05 13:59:58.227007 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/string.data.json
+-rw-r--r--   0        0        0     1749 2023-03-05 13:59:58.227251 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/string.meta.json
+-rw-r--r--   0        0        0    16134 2023-03-05 13:59:58.445777 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/struct.data.json
+-rw-r--r--   0        0        0     1746 2023-03-05 13:59:58.445965 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/struct.meta.json
+-rw-r--r--   0        0        0   170345 2023-03-05 13:59:57.775023 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1824 2023-03-05 13:59:57.775212 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   147982 2023-03-05 13:59:57.771706 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1803 2023-03-05 13:59:57.771904 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0   118973 2023-03-05 13:59:58.420881 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tempfile.data.json
+-rw-r--r--   0        0        0     1768 2023-03-05 13:59:58.421132 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tempfile.meta.json
+-rw-r--r--   0        0        0    51601 2023-03-05 13:59:58.112567 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/termios.data.json
+-rw-r--r--   0        0        0     1699 2023-03-05 13:59:58.112777 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/termios.meta.json
+-rw-r--r--   0        0        0    20620 2023-03-05 13:59:58.120113 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/textwrap.data.json
+-rw-r--r--   0        0        0     1679 2023-03-05 13:59:58.120312 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/textwrap.meta.json
+-rw-r--r--   0        0        0    67623 2023-03-05 13:59:58.325619 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/threading.data.json
+-rw-r--r--   0        0        0     1734 2023-03-05 13:59:58.325856 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/threading.meta.json
+-rw-r--r--   0        0        0    45246 2023-03-05 13:59:58.486404 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1693 2023-03-05 13:59:58.486643 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0    12783 2023-03-05 13:59:57.948922 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/timeit.data.json
+-rw-r--r--   0        0        0     1689 2023-03-05 13:59:57.949145 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/timeit.meta.json
+-rw-r--r--   0        0        0  1132743 2023-03-05 13:59:58.816870 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tkinter/__init__.data.json
+-rw-r--r--   0        0        0     1911 2023-03-05 13:59:58.817181 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tkinter/__init__.meta.json
+-rw-r--r--   0        0        0     5838 2023-03-05 14:01:07.987231 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tkinter/commondialog.data.json
+-rw-r--r--   0        0        0     1722 2023-03-05 14:01:07.987421 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tkinter/commondialog.meta.json
+-rw-r--r--   0        0        0    20007 2023-03-05 13:59:57.900380 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tkinter/constants.data.json
+-rw-r--r--   0        0        0     1687 2023-03-05 13:59:57.900604 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tkinter/constants.meta.json
+-rw-r--r--   0        0        0     5652 2023-03-05 14:01:08.622277 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tkinter/dialog.data.json
+-rw-r--r--   0        0        0     1727 2023-03-05 14:01:08.622489 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tkinter/dialog.meta.json
+-rw-r--r--   0        0        0    42762 2023-03-05 14:01:08.621195 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tkinter/filedialog.data.json
+-rw-r--r--   0        0        0     1807 2023-03-05 14:01:08.621417 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tkinter/filedialog.meta.json
+-rw-r--r--   0        0        0    46653 2023-03-05 13:59:58.794883 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tkinter/font.data.json
+-rw-r--r--   0        0        0     1747 2023-03-05 13:59:58.795151 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tkinter/font.meta.json
+-rw-r--r--   0        0        0   414945 2023-03-05 14:01:08.616570 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tkinter/ttk.data.json
+-rw-r--r--   0        0        0     1792 2023-03-05 14:01:08.616848 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tkinter/ttk.meta.json
+-rw-r--r--   0        0        0    16221 2023-03-05 13:59:58.059713 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/token.data.json
+-rw-r--r--   0        0        0     1670 2023-03-05 13:59:58.059900 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/token.meta.json
+-rw-r--r--   0        0        0    52823 2023-03-05 13:59:58.886341 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tokenize.data.json
+-rw-r--r--   0        0        0     1766 2023-03-05 13:59:58.886540 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tokenize.meta.json
+-rw-r--r--   0        0        0     2322 2023-03-05 13:59:58.247211 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/__init__.data.json
+-rw-r--r--   0        0        0     1627 2023-03-05 13:59:58.247407 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/__init__.meta.json
+-rw-r--r--   0        0        0    27215 2023-03-05 14:00:03.725587 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/concurrent.data.json
+-rw-r--r--   0        0        0     2085 2023-03-05 14:01:11.316802 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/concurrent.meta.json
+-rw-r--r--   0        0        0    32193 2023-03-05 14:00:02.171811 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/escape.data.json
+-rw-r--r--   0        0        0     2105 2023-03-05 14:00:02.172051 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/escape.meta.json
+-rw-r--r--   0        0        0    58686 2023-03-05 14:00:03.729865 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/gen.data.json
+-rw-r--r--   0        0        0     2291 2023-03-05 14:01:11.320794 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/gen.meta.json
+-rw-r--r--   0        0        0    69509 2023-03-05 14:00:03.727405 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/ioloop.data.json
+-rw-r--r--   0        0        0     2637 2023-03-05 14:01:11.318549 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/ioloop.meta.json
+-rw-r--r--   0        0        0    79926 2023-03-05 14:00:03.731684 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/iostream.data.json
+-rw-r--r--   0        0        0     2502 2023-03-05 14:01:11.322505 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/iostream.meta.json
+-rw-r--r--   0        0        0    35943 2023-03-05 14:00:03.779546 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/locks.data.json
+-rw-r--r--   0        0        0     2214 2023-03-05 14:00:03.779820 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/locks.meta.json
+-rw-r--r--   0        0        0     9760 2023-03-05 14:01:09.954166 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/log.data.json
+-rw-r--r--   0        0        0     2041 2023-03-05 14:01:09.954484 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/log.meta.json
+-rw-r--r--   0        0        0    36166 2023-03-05 14:00:03.728451 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/netutil.data.json
+-rw-r--r--   0        0        0     2303 2023-03-05 14:01:11.319484 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/netutil.meta.json
+-rw-r--r--   0        0        0    42399 2023-03-05 14:00:02.364748 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/options.data.json
+-rw-r--r--   0        0        0     2159 2023-03-05 14:01:09.955589 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/options.meta.json
+-rw-r--r--   0        0        0     1676 2023-03-05 13:59:57.928546 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/platform/__init__.data.json
+-rw-r--r--   0        0        0     1642 2023-03-05 13:59:57.928735 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/platform/__init__.meta.json
+-rw-r--r--   0        0        0    57261 2023-03-05 14:00:03.733022 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/platform/asyncio.data.json
+-rw-r--r--   0        0        0     2350 2023-03-05 14:01:11.323753 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/platform/asyncio.meta.json
+-rw-r--r--   0        0        0    20538 2023-03-05 14:00:03.733762 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/process.data.json
+-rw-r--r--   0        0        0     2406 2023-03-05 14:01:11.324391 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/process.meta.json
+-rw-r--r--   0        0        0    40269 2023-03-05 14:00:03.812585 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/queues.data.json
+-rw-r--r--   0        0        0     2301 2023-03-05 14:00:03.812881 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/queues.meta.json
+-rw-r--r--   0        0        0    42511 2023-03-05 14:00:01.932095 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/util.data.json
+-rw-r--r--   0        0        0     2201 2023-03-05 14:00:01.932340 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tornado/util.meta.json
+-rw-r--r--   0        0        0     5659 2023-03-05 14:01:08.917555 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/__init__.data.json
+-rw-r--r--   0        0        0     1818 2023-03-05 14:01:08.917788 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/__init__.meta.json
+-rw-r--r--   0        0        0     7167 2023-03-05 14:01:08.571896 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/_monitor.data.json
+-rw-r--r--   0        0        0     1674 2023-03-05 14:01:08.572093 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/_monitor.meta.json
+-rw-r--r--   0        0        0     2675 2023-03-05 14:01:08.438395 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/_tqdm_pandas.data.json
+-rw-r--r--   0        0        0     1643 2023-03-05 14:01:08.438567 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/_tqdm_pandas.meta.json
+-rw-r--r--   0        0        0    66131 2023-03-05 14:01:08.858250 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/asyncio.data.json
+-rw-r--r--   0        0        0     1744 2023-03-05 14:01:08.858458 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/asyncio.meta.json
+-rw-r--r--   0        0        0     1965 2023-03-05 14:01:09.041109 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/auto.data.json
+-rw-r--r--   0        0        0     1649 2023-03-05 14:01:09.041406 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/auto.meta.json
+-rw-r--r--   0        0        0     2733 2023-03-05 14:01:08.437828 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/cli.data.json
+-rw-r--r--   0        0        0     1651 2023-03-05 14:01:08.438003 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/cli.meta.json
+-rw-r--r--   0        0        0    27887 2023-03-05 14:01:08.853500 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/gui.data.json
+-rw-r--r--   0        0        0     1709 2023-03-05 14:01:08.853697 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/gui.meta.json
+-rw-r--r--   0        0        0    40061 2023-03-05 14:01:08.851002 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/notebook.data.json
+-rw-r--r--   0        0        0     1719 2023-03-05 14:01:08.851214 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/notebook.meta.json
+-rw-r--r--   0        0        0   104587 2023-03-05 14:01:08.746596 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/std.data.json
+-rw-r--r--   0        0        0     1796 2023-03-05 14:01:08.746826 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/std.meta.json
+-rw-r--r--   0        0        0    30940 2023-03-05 14:01:08.414127 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/utils.data.json
+-rw-r--r--   0        0        0     1713 2023-03-05 14:01:08.414342 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/utils.meta.json
+-rw-r--r--   0        0        0     1587 2023-03-05 14:01:08.437123 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/version.data.json
+-rw-r--r--   0        0        0     1633 2023-03-05 14:01:08.437343 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tqdm/version.meta.json
+-rw-r--r--   0        0        0    54443 2023-03-05 13:59:58.266744 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traceback.data.json
+-rw-r--r--   0        0        0     1743 2023-03-05 13:59:58.266961 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traceback.meta.json
+-rw-r--r--   0        0        0    11487 2023-03-05 14:00:01.136847 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/__init__.data.json
+-rw-r--r--   0        0        0     1940 2023-03-05 14:00:01.137062 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/__init__.meta.json
+-rw-r--r--   0        0        0     2956 2023-03-05 13:59:58.071651 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/_version.data.json
+-rw-r--r--   0        0        0     1764 2023-03-05 13:59:58.071887 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/_version.meta.json
+-rw-r--r--   0        0        0    10223 2023-03-05 13:59:58.909113 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/config/argcomplete_config.data.json
+-rw-r--r--   0        0        0     1839 2023-03-05 13:59:58.909336 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/config/argcomplete_config.meta.json
+-rw-r--r--   0        0        0   174172 2023-03-05 13:59:59.836772 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/traitlets.data.json
+-rw-r--r--   0        0        0     2291 2023-03-05 13:59:59.837128 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/traitlets.meta.json
+-rw-r--r--   0        0        0     2592 2023-03-05 13:59:58.252655 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/__init__.data.json
+-rw-r--r--   0        0        0     1809 2023-03-05 13:59:58.252884 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/__init__.meta.json
+-rw-r--r--   0        0        0     3280 2023-03-05 13:59:58.072713 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/bunch.data.json
+-rw-r--r--   0        0        0     1645 2023-03-05 13:59:58.072957 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/bunch.meta.json
+-rw-r--r--   0        0        0     3960 2023-03-05 14:00:00.949052 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/decorators.data.json
+-rw-r--r--   0        0        0     1831 2023-03-05 14:00:00.949251 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/decorators.meta.json
+-rw-r--r--   0        0        0     3084 2023-03-05 13:59:59.545834 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/descriptions.data.json
+-rw-r--r--   0        0        0     1849 2023-03-05 13:59:59.546029 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/descriptions.meta.json
+-rw-r--r--   0        0        0     1911 2023-03-05 13:59:59.543824 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/getargspec.data.json
+-rw-r--r--   0        0        0     1835 2023-03-05 13:59:59.544019 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/getargspec.meta.json
+-rw-r--r--   0        0        0     1756 2023-03-05 13:59:58.281826 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/importstring.data.json
+-rw-r--r--   0        0        0     1761 2023-03-05 13:59:58.282007 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/importstring.meta.json
+-rw-r--r--   0        0        0     1781 2023-03-05 13:59:58.090164 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/nested_update.data.json
+-rw-r--r--   0        0        0     1681 2023-03-05 13:59:58.090352 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/nested_update.meta.json
+-rw-r--r--   0        0        0     3862 2023-03-05 13:59:58.019287 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/sentinel.data.json
+-rw-r--r--   0        0        0     1716 2023-03-05 13:59:58.019470 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/sentinel.meta.json
+-rw-r--r--   0        0        0     2832 2023-03-05 13:59:58.910459 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/text.data.json
+-rw-r--r--   0        0        0     1689 2023-03-05 13:59:58.910652 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/traitlets/utils/text.meta.json
+-rw-r--r--   0        0        0     5215 2023-03-05 13:59:58.113689 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tty.data.json
+-rw-r--r--   0        0        0     1671 2023-03-05 13:59:58.113898 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/tty.meta.json
+-rw-r--r--   0        0        0   242405 2023-03-05 13:59:57.768979 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1775 2023-03-05 13:59:57.769191 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   430606 2023-03-05 13:59:57.764584 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1842 2023-03-05 13:59:57.764833 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    71533 2023-03-05 13:59:57.755998 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1765 2023-03-05 13:59:57.756331 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    25457 2023-03-05 13:59:58.050448 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unicodedata.data.json
+-rw-r--r--   0        0        0     1707 2023-03-05 13:59:58.050655 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unicodedata.meta.json
+-rw-r--r--   0        0        0     6387 2023-03-05 13:59:59.382990 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1941 2023-03-05 13:59:59.383193 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    25783 2023-03-05 13:59:59.374580 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/_log.data.json
+-rw-r--r--   0        0        0     1789 2023-03-05 13:59:59.374767 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/_log.meta.json
+-rw-r--r--   0        0        0     8109 2023-03-05 13:59:59.379451 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1820 2023-03-05 13:59:59.379631 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   221008 2023-03-05 13:59:59.378920 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/case.data.json
+-rw-r--r--   0        0        0     1940 2023-03-05 13:59:59.379146 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/case.meta.json
+-rw-r--r--   0        0        0    15471 2023-03-05 13:59:59.381827 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/loader.data.json
+-rw-r--r--   0        0        0     1851 2023-03-05 13:59:59.382059 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/loader.meta.json
+-rw-r--r--   0        0        0    12425 2023-03-05 13:59:59.382484 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/main.data.json
+-rw-r--r--   0        0        0     1860 2023-03-05 13:59:59.382701 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/main.meta.json
+-rw-r--r--   0        0        0    21795 2023-03-05 13:59:59.373746 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/result.data.json
+-rw-r--r--   0        0        0     1807 2023-03-05 13:59:59.373974 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/result.meta.json
+-rw-r--r--   0        0        0    11341 2023-03-05 13:59:59.381170 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/runner.data.json
+-rw-r--r--   0        0        0     1850 2023-03-05 13:59:59.381383 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/runner.meta.json
+-rw-r--r--   0        0        0    12147 2023-03-05 13:59:59.380559 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/signals.data.json
+-rw-r--r--   0        0        0     1802 2023-03-05 13:59:59.380784 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11760 2023-03-05 13:59:59.379987 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/suite.data.json
+-rw-r--r--   0        0        0     1823 2023-03-05 13:59:59.380161 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1617 2023-03-05 13:59:58.240199 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1644 2023-03-05 13:59:58.240409 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib/__init__.meta.json
+-rw-r--r--   0        0        0    11137 2023-03-05 13:59:58.988694 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib/error.data.json
+-rw-r--r--   0        0        0     1712 2023-03-05 13:59:58.988933 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib/error.meta.json
+-rw-r--r--   0        0        0   152232 2023-03-05 13:59:58.442114 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib/parse.data.json
+-rw-r--r--   0        0        0     1723 2023-03-05 13:59:58.442386 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib/parse.meta.json
+-rw-r--r--   0        0        0   159266 2023-03-05 13:59:59.870660 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib/request.data.json
+-rw-r--r--   0        0        0     2041 2023-03-05 13:59:59.870878 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib/request.meta.json
+-rw-r--r--   0        0        0    29584 2023-03-05 13:59:58.239627 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib/response.data.json
+-rw-r--r--   0        0        0     1832 2023-03-05 13:59:58.239854 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib/response.meta.json
+-rw-r--r--   0        0        0    24428 2023-03-05 14:01:07.986173 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib/robotparser.data.json
+-rw-r--r--   0        0        0     1719 2023-03-05 14:01:07.986364 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib/robotparser.meta.json
+-rw-r--r--   0        0        0    12146 2023-03-05 14:01:08.908762 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/__init__.data.json
+-rw-r--r--   0        0        0     2053 2023-03-05 14:01:08.908979 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/__init__.meta.json
+-rw-r--r--   0        0        0    25682 2023-03-05 14:01:08.377381 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/_collections.data.json
+-rw-r--r--   0        0        0     1690 2023-03-05 14:01:08.377576 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/_collections.meta.json
+-rw-r--r--   0        0        0    21622 2023-03-05 14:01:08.905784 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/connection.data.json
+-rw-r--r--   0        0        0     1917 2023-03-05 14:01:08.905970 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/connection.meta.json
+-rw-r--r--   0        0        0    34741 2023-03-05 14:01:08.909756 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/connectionpool.data.json
+-rw-r--r--   0        0        0     2239 2023-03-05 14:01:08.909988 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/connectionpool.meta.json
+-rw-r--r--   0        0        0     1674 2023-03-05 14:01:08.381426 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/contrib/__init__.data.json
+-rw-r--r--   0        0        0     1647 2023-03-05 14:01:08.381594 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/contrib/__init__.meta.json
+-rw-r--r--   0        0        0    13461 2023-03-05 14:01:09.061711 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/contrib/socks.data.json
+-rw-r--r--   0        0        0     1856 2023-03-05 14:01:09.061908 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/contrib/socks.meta.json
+-rw-r--r--   0        0        0    46021 2023-03-05 14:01:08.913260 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/exceptions.data.json
+-rw-r--r--   0        0        0     1843 2023-03-05 14:01:08.913492 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/exceptions.meta.json
+-rw-r--r--   0        0        0    13505 2023-03-05 14:01:08.378923 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/fields.data.json
+-rw-r--r--   0        0        0     1690 2023-03-05 14:01:08.379115 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/fields.meta.json
+-rw-r--r--   0        0        0     3293 2023-03-05 14:01:08.904525 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/filepost.data.json
+-rw-r--r--   0        0        0     1684 2023-03-05 14:01:08.904757 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/filepost.meta.json
+-rw-r--r--   0        0        0     1682 2023-03-05 14:01:08.379440 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/packages/__init__.data.json
+-rw-r--r--   0        0        0     1649 2023-03-05 14:01:08.379621 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/packages/__init__.meta.json
+-rw-r--r--   0        0        0     2952 2023-03-05 14:01:08.815767 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/packages/ssl_match_hostname/__init__.data.json
+-rw-r--r--   0        0        0     1702 2023-03-05 14:01:08.815959 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/packages/ssl_match_hostname/__init__.meta.json
+-rw-r--r--   0        0        0    10966 2023-03-05 14:01:08.541195 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/poolmanager.data.json
+-rw-r--r--   0        0        0     1715 2023-03-05 14:01:08.541450 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/poolmanager.meta.json
+-rw-r--r--   0        0        0     4744 2023-03-05 14:01:08.380339 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/request.data.json
+-rw-r--r--   0        0        0     1639 2023-03-05 14:01:08.380524 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/request.meta.json
+-rw-r--r--   0        0        0    42034 2023-03-05 14:01:08.910915 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/response.data.json
+-rw-r--r--   0        0        0     1970 2023-03-05 14:01:08.911136 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/response.meta.json
+-rw-r--r--   0        0        0    13666 2023-03-05 14:01:08.906366 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/__init__.data.json
+-rw-r--r--   0        0        0     1869 2023-03-05 14:01:08.906544 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/__init__.meta.json
+-rw-r--r--   0        0        0     2948 2023-03-05 14:01:08.380948 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/connection.data.json
+-rw-r--r--   0        0        0     1655 2023-03-05 14:01:08.381129 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/connection.meta.json
+-rw-r--r--   0        0        0     2526 2023-03-05 14:01:08.699260 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/queue.data.json
+-rw-r--r--   0        0        0     1659 2023-03-05 14:01:08.699467 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/queue.meta.json
+-rw-r--r--   0        0        0     2227 2023-03-05 14:01:08.403337 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/request.data.json
+-rw-r--r--   0        0        0     1649 2023-03-05 14:01:08.403582 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/request.meta.json
+-rw-r--r--   0        0        0     1708 2023-03-05 14:01:08.374452 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/response.data.json
+-rw-r--r--   0        0        0     1651 2023-03-05 14:01:08.374639 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/response.meta.json
+-rw-r--r--   0        0        0    47266 2023-03-05 14:01:08.912150 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/retry.data.json
+-rw-r--r--   0        0        0     1849 2023-03-05 14:01:08.912374 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/retry.meta.json
+-rw-r--r--   0        0        0     5838 2023-03-05 14:01:08.905048 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/ssl_.data.json
+-rw-r--r--   0        0        0     1704 2023-03-05 14:01:08.905229 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/ssl_.meta.json
+-rw-r--r--   0        0        0     8569 2023-03-05 14:01:08.908153 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/timeout.data.json
+-rw-r--r--   0        0        0     1696 2023-03-05 14:01:08.908359 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/timeout.meta.json
+-rw-r--r--   0        0        0    44985 2023-03-05 14:01:08.907590 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/url.data.json
+-rw-r--r--   0        0        0     1688 2023-03-05 14:01:08.907803 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/urllib3/util/url.meta.json
+-rw-r--r--   0        0        0    35323 2023-03-05 13:59:58.362832 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/uuid.data.json
+-rw-r--r--   0        0        0     1760 2023-03-05 13:59:58.363039 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/uuid.meta.json
+-rw-r--r--   0        0        0    23606 2023-03-05 13:59:59.074351 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/warnings.data.json
+-rw-r--r--   0        0        0     1761 2023-03-05 13:59:59.074594 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/warnings.meta.json
+-rw-r--r--   0        0        0    56221 2023-03-05 13:59:58.432763 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/wave.data.json
+-rw-r--r--   0        0        0     1758 2023-03-05 13:59:58.433004 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/wave.meta.json
+-rw-r--r--   0        0        0   129763 2023-03-05 13:59:58.974457 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/weakref.data.json
+-rw-r--r--   0        0        0     1767 2023-03-05 13:59:58.974692 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/weakref.meta.json
+-rw-r--r--   0        0        0    28219 2023-03-05 13:59:58.117751 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/webbrowser.data.json
+-rw-r--r--   0        0        0     1711 2023-03-05 13:59:58.117974 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/webbrowser.meta.json
+-rw-r--r--   0        0        0     1594 2023-03-05 14:01:08.338502 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32/__init__.data.json
+-rw-r--r--   0        0        0     1627 2023-03-05 14:01:08.338693 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32/__init__.meta.json
+-rw-r--r--   0        0        0     1626 2023-03-05 14:01:08.051448 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32/lib/__init__.data.json
+-rw-r--r--   0        0        0     1635 2023-03-05 14:01:08.051639 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32/lib/__init__.meta.json
+-rw-r--r--   0        0        0   139485 2023-03-05 14:01:08.359031 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32/lib/ntsecuritycon.data.json
+-rw-r--r--   0        0        0     1685 2023-03-05 14:01:08.359268 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32/lib/ntsecuritycon.meta.json
+-rw-r--r--   0        0        0    18511 2023-03-05 14:01:08.662627 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32/lib/pywintypes.data.json
+-rw-r--r--   0        0        0     1738 2023-03-05 14:01:08.662831 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32/lib/pywintypes.meta.json
+-rw-r--r--   0        0        0   152994 2023-03-05 14:01:08.812178 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32/win32api.data.json
+-rw-r--r--   0        0        0     1784 2023-03-05 14:01:08.812399 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32/win32api.meta.json
+-rw-r--r--   0        0        0    15962 2023-03-05 14:01:08.783715 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32/win32clipboard.data.json
+-rw-r--r--   0        0        0     1681 2023-03-05 14:01:08.783906 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32/win32clipboard.meta.json
+-rw-r--r--   0        0        0   168289 2023-03-05 14:01:08.797648 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32/win32security.data.json
+-rw-r--r--   0        0        0     1742 2023-03-05 14:01:08.797883 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32/win32security.meta.json
+-rw-r--r--   0        0        0    30155 2023-03-05 14:01:08.884498 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32api/__init__.data.json
+-rw-r--r--   0        0        0     1658 2023-03-05 14:01:08.884685 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32api/__init__.meta.json
+-rw-r--r--   0        0        0     6929 2023-03-05 14:01:08.881569 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32clipboard/__init__.data.json
+-rw-r--r--   0        0        0     1676 2023-03-05 14:01:08.881773 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32clipboard/__init__.meta.json
+-rw-r--r--   0        0        0    65049 2023-03-05 14:01:08.883381 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32security/__init__.data.json
+-rw-r--r--   0        0        0     1673 2023-03-05 14:01:08.883578 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/win32security/__init__.meta.json
+-rw-r--r--   0        0        0     2320 2023-03-05 13:59:58.228375 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/winreg.data.json
+-rw-r--r--   0        0        0     1712 2023-03-05 13:59:58.228565 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/winreg.meta.json
+-rw-r--r--   0        0        0     1679 2023-03-05 13:59:59.787437 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/__init__.data.json
+-rw-r--r--   0        0        0     1710 2023-03-05 13:59:59.787667 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/__init__.meta.json
+-rw-r--r--   0        0        0    26139 2023-03-05 13:59:59.447948 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/dom/__init__.data.json
+-rw-r--r--   0        0        0     1721 2023-03-05 13:59:59.448143 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/dom/__init__.meta.json
+-rw-r--r--   0        0        0     5029 2023-03-05 13:59:58.986959 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/dom/domreg.data.json
+-rw-r--r--   0        0        0     1721 2023-03-05 13:59:58.987213 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/dom/domreg.meta.json
+-rw-r--r--   0        0        0    65369 2023-03-05 14:00:01.062328 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/dom/expatbuilder.data.json
+-rw-r--r--   0        0        0     1851 2023-03-05 14:00:01.062598 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/dom/expatbuilder.meta.json
+-rw-r--r--   0        0        0   158529 2023-03-05 14:00:01.066721 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/dom/minidom.data.json
+-rw-r--r--   0        0        0     1936 2023-03-05 14:00:01.066932 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/dom/minidom.meta.json
+-rw-r--r--   0        0        0    35261 2023-03-05 14:00:01.063373 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/dom/xmlbuilder.data.json
+-rw-r--r--   0        0        0     1852 2023-03-05 14:00:01.063576 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/dom/xmlbuilder.meta.json
+-rw-r--r--   0        0        0     1747 2023-03-05 13:59:59.540738 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/parsers/__init__.data.json
+-rw-r--r--   0        0        0     1732 2023-03-05 13:59:59.540924 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/parsers/__init__.meta.json
+-rw-r--r--   0        0        0     3195 2023-03-05 13:59:59.303774 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/parsers/expat/__init__.data.json
+-rw-r--r--   0        0        0     1733 2023-03-05 13:59:59.303959 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/parsers/expat/__init__.meta.json
+-rw-r--r--   0        0        0    18310 2023-03-05 13:59:58.852394 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/sax/__init__.data.json
+-rw-r--r--   0        0        0     1823 2023-03-05 13:59:58.852582 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/sax/__init__.meta.json
+-rw-r--r--   0        0        0    19177 2023-03-05 13:59:57.914888 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/sax/handler.data.json
+-rw-r--r--   0        0        0     1689 2023-03-05 13:59:57.915089 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/sax/handler.meta.json
+-rw-r--r--   0        0        0    24582 2023-03-05 13:59:58.243941 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/sax/xmlreader.data.json
+-rw-r--r--   0        0        0     1685 2023-03-05 13:59:58.244178 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/xml/sax/xmlreader.meta.json
+-rw-r--r--   0        0        0    72877 2023-03-05 13:59:58.408739 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zipfile.data.json
+-rw-r--r--   0        0        0     1829 2023-03-05 13:59:58.408945 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zipfile.meta.json
+-rw-r--r--   0        0        0    13835 2023-03-05 13:59:58.044500 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zipimport.data.json
+-rw-r--r--   0        0        0     1777 2023-03-05 13:59:58.044736 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zipimport.meta.json
+-rw-r--r--   0        0        0    18083 2023-03-05 13:59:58.359414 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zlib.data.json
+-rw-r--r--   0        0        0     1759 2023-03-05 13:59:58.359609 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zlib.meta.json
+-rw-r--r--   0        0        0    33030 2023-03-05 14:00:01.007795 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/__init__.data.json
+-rw-r--r--   0        0        0     1751 2023-03-05 14:00:01.007967 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/__init__.meta.json
+-rw-r--r--   0        0        0    69457 2023-03-05 14:00:01.951668 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/_future.data.json
+-rw-r--r--   0        0        0     2277 2023-03-05 14:00:01.951940 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/_future.meta.json
+-rw-r--r--   0        0        0     1795 2023-03-05 13:59:58.036894 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/_typing.data.json
+-rw-r--r--   0        0        0     1658 2023-03-05 13:59:58.037124 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/_typing.meta.json
+-rw-r--r--   0        0        0    17089 2023-03-05 14:00:03.788290 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/asyncio.data.json
+-rw-r--r--   0        0        0     2334 2023-03-05 14:00:03.788515 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/asyncio.meta.json
+-rw-r--r--   0        0        0    38399 2023-03-05 14:00:01.000376 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/backend/__init__.data.json
+-rw-r--r--   0        0        0     1978 2023-03-05 14:00:01.000634 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/backend/__init__.meta.json
+-rw-r--r--   0        0        0     2757 2023-03-05 13:59:57.920517 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/backend/select.data.json
+-rw-r--r--   0        0        0     1673 2023-03-05 13:59:57.920717 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/backend/select.meta.json
+-rw-r--r--   0        0        0   177007 2023-03-05 13:59:58.875313 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/constants.data.json
+-rw-r--r--   0        0        0     1803 2023-03-05 13:59:58.875567 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/constants.meta.json
+-rw-r--r--   0        0        0    17018 2023-03-05 14:00:00.998965 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/error.data.json
+-rw-r--r--   0        0        0     1908 2023-03-05 14:00:00.999151 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/error.meta.json
+-rw-r--r--   0        0        0     2191 2023-03-05 14:00:03.788948 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/eventloop/__init__.data.json
+-rw-r--r--   0        0        0     1840 2023-03-05 14:00:03.789227 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/eventloop/__init__.meta.json
+-rw-r--r--   0        0        0    65591 2023-03-05 14:00:03.803470 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/eventloop/zmqstream.data.json
+-rw-r--r--   0        0        0     2509 2023-03-05 14:01:11.376379 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/eventloop/zmqstream.meta.json
+-rw-r--r--   0        0        0     4243 2023-03-05 14:00:01.006876 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/__init__.data.json
+-rw-r--r--   0        0        0     1883 2023-03-05 14:00:01.007061 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/__init__.meta.json
+-rw-r--r--   0        0        0    10283 2023-03-05 14:00:00.998176 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/attrsettr.data.json
+-rw-r--r--   0        0        0     1782 2023-03-05 14:00:00.998453 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/attrsettr.meta.json
+-rw-r--r--   0        0        0    50766 2023-03-05 14:00:01.006420 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/context.data.json
+-rw-r--r--   0        0        0     2174 2023-03-05 14:00:01.006628 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/context.meta.json
+-rw-r--r--   0        0        0     7720 2023-03-05 14:00:01.002413 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/frame.data.json
+-rw-r--r--   0        0        0     1767 2023-03-05 14:00:01.002579 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/frame.meta.json
+-rw-r--r--   0        0        0    10246 2023-03-05 14:00:01.001953 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/poll.data.json
+-rw-r--r--   0        0        0     1837 2023-03-05 14:00:01.002121 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/poll.meta.json
+-rw-r--r--   0        0        0    93213 2023-03-05 14:00:01.004930 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/socket.data.json
+-rw-r--r--   0        0        0     2247 2023-03-05 14:00:01.005216 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/socket.meta.json
+-rw-r--r--   0        0        0     7030 2023-03-05 14:00:01.001442 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/tracker.data.json
+-rw-r--r--   0        0        0     1762 2023-03-05 14:00:01.001613 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/tracker.meta.json
+-rw-r--r--   0        0        0     8454 2023-03-05 14:00:01.000975 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/version.data.json
+-rw-r--r--   0        0        0     1833 2023-03-05 14:00:01.001154 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/sugar/version.meta.json
+-rw-r--r--   0        0        0     1620 2023-03-05 13:59:58.036201 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/utils/__init__.data.json
+-rw-r--r--   0        0        0     1628 2023-03-05 13:59:58.036407 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/utils/__init__.meta.json
+-rw-r--r--   0        0        0     2190 2023-03-05 13:59:57.870736 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/utils/interop.data.json
+-rw-r--r--   0        0        0     1824 2023-03-05 14:01:08.865530 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/utils/interop.meta.json
+-rw-r--r--   0        0        0     4472 2023-03-05 13:59:59.236169 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/utils/jsonapi.data.json
+-rw-r--r--   0        0        0     1809 2023-03-05 13:59:59.236385 alacorder-79.5.0/src/alacorder/.mypy_cache/3.10/zmq/utils/jsonapi.meta.json
+-rw-r--r--   0        0        0      190 2023-03-05 14:00:04.569522 alacorder-79.5.0/src/alacorder/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.5.0/src/alacorder/.python-version
+-rw-r--r--   0        0        0     2129 2023-03-28 18:45:29.612372 alacorder-79.5.0/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   134243 2023-04-19 15:08:11.299347 alacorder-79.5.0/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   134243 2023-04-19 15:08:19.046432 alacorder-79.5.0/src/alacorder/alac.py
+-rw-r--r--   0        0        0   125941 2023-04-19 15:08:25.427180 alacorder-79.5.0/src/alacorder/graphical.py
+-rw-r--r--   0        0        0    53236 2023-03-30 00:46:11.281022 alacorder-79.5.0/src/alacorder/img/alac.icns
+-rw-r--r--   0        0        0    99678 2023-04-17 22:01:20.160909 alacorder-79.5.0/src/alacorder/img/alac.ico
+-rw-r--r--   0        0        0     8334 2023-03-23 21:38:13.000000 alacorder-79.5.0/src/alacorder/img/alac.png
+-rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.5.0/src/alacorder/~$E 302 Portfolio.docx
+-rw-r--r--   0        0        0    10449 1970-01-01 00:00:00.000000 alacorder-79.5.0/PKG-INFO
```

### Comparing `alacorder-79.4.9/LICENSE` & `alacorder-79.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-79.4.9/README.md` & `alacorder-79.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -34,591 +34,565 @@
 00000210: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
 00000220: 7267 2f70 726f 6a65 6374 2f61 6c61 636f  rg/project/alaco
 00000230: 7264 6572 2f29 2020 2020 207c 205b 5265  rder/)     | [Re
 00000240: 706f 7274 2061 6e20 6973 7375 655d 286d  port an issue](m
 00000250: 6169 6c74 6f3a 7362 726f 6273 6f6e 4063  ailto:sbrobson@c
 00000260: 7269 6d73 6f6e 2e75 612e 6564 7529 0a3c  rimson.ua.edu).<
 00000270: 2f73 7570 3e0a 0a23 2320 2a2a 496e 7374  /sup>..## **Inst
-00000280: 616c 6c61 7469 6f6e 2a2a 0a0a 2a2a 416c  allation**..**Al
-00000290: 6163 6f72 6465 7220 6361 6e20 7275 6e20  acorder can run 
-000002a0: 6f6e 206d 6f73 7420 6465 7669 6365 732e  on most devices.
-000002b0: 2049 6620 796f 7572 2064 6576 6963 6520   If your device 
-000002c0: 6361 6e20 7275 6e20 5079 7468 6f6e 2033  can run Python 3
-000002d0: 2e39 206f 7220 6c61 7465 722c 2069 7420  .9 or later, it 
-000002e0: 6361 6e20 7275 6e20 416c 6163 6f72 6465  can run Alacorde
-000002f0: 722e 2a2a 0a2a 2054 6f20 736b 6970 2069  r.**.* To skip i
-00000300: 6e73 7461 6c6c 6174 696f 6e2c 2064 6f77  nstallation, dow
-00000310: 6e6c 6f61 6420 7468 6520 7072 6562 7569  nload the prebui
-00000320: 6c74 2065 7865 6375 7461 626c 6520 666f  lt executable fo
-00000330: 7220 796f 7572 206f 7065 7261 7469 6e67  r your operating
-00000340: 2073 7973 7465 6d20 284d 6163 4f53 206f   system (MacOS o
-00000350: 7220 5769 6e64 6f77 7329 2066 726f 6d20  r Windows) from 
-00000360: 4769 7448 7562 2e20 4f70 656e 2074 6865  GitHub. Open the
-00000370: 2065 7865 6375 7461 626c 6520 6669 6c65   executable file
-00000380: 2061 6e64 2077 6169 7420 666f 7220 416c   and wait for Al
-00000390: 6163 6f72 6465 7220 746f 206c 6175 6e63  acorder to launc
-000003a0: 682e 0a2a 2049 6620 796f 7520 616c 7265  h..* If you alre
-000003b0: 6164 7920 6861 7665 2050 7974 686f 6e20  ady have Python 
-000003c0: 696e 7374 616c 6c65 642c 206f 7065 6e20  installed, open 
-000003d0: 436f 6d6d 616e 6420 5072 6f6d 7074 206f  Command Prompt o
-000003e0: 7220 5465 726d 696e 616c 2061 6e64 2065  r Terminal and e
-000003f0: 6e74 6572 2060 7069 7020 696e 7374 616c  nter `pip instal
-00000400: 6c20 616c 6163 6f72 6465 7260 206f 7220  l alacorder` or 
-00000410: 6070 6970 3320 696e 7374 616c 6c20 616c  `pip3 install al
-00000420: 6163 6f72 6465 7260 2e20 0a2a 2049 6e73  acorder`. .* Ins
-00000430: 7461 6c6c 205b 5079 7468 6f6e 5d28 6874  tall [Python](ht
-00000440: 7470 733a 2f2f 7777 772e 7079 7468 6f6e  tps://www.python
-00000450: 2e6f 7267 2f64 6f77 6e6c 6f61 6473 2f29  .org/downloads/)
-00000460: 2062 6566 6f72 6520 7573 696e 6720 6070   before using `p
-00000470: 6970 6020 6966 2074 6865 2061 626f 7665  ip` if the above
-00000480: 206d 6574 686f 6473 2064 6f20 6e6f 7420   methods do not 
-00000490: 776f 726b 2e20 4f6e 6365 2079 6f75 7220  work. Once your 
-000004a0: 5079 7468 6f6e 2065 6e76 6972 6f6e 6d65  Python environme
-000004b0: 6e74 2069 7320 636f 6e66 6967 7572 6564  nt is configured
-000004c0: 2c20 7265 7065 6174 2074 6865 7365 2069  , repeat these i
-000004d0: 6e73 7461 6c6c 6174 696f 6e20 696e 7374  nstallation inst
-000004e0: 7275 6374 696f 6e73 2069 6e20 6120 7465  ructions in a te
-000004f0: 726d 696e 616c 2e0a 0a60 6060 0a55 7361  rminal...```.Usa
-00000500: 6765 3a20 7079 7468 6f6e 202d 6d20 616c  ge: python -m al
-00000510: 6163 6f72 6465 7220 5b4f 5054 494f 4e53  acorder [OPTIONS
-00000520: 5d20 434f 4d4d 414e 4420 5b41 5247 535d  ] COMMAND [ARGS]
-00000530: 2e2e 2e0a 0a20 2041 4c41 434f 5244 4552  .....  ALACORDER
-00000540: 2037 390a 0a4f 7074 696f 6e73 3a0a 2020   79..Options:.  
-00000550: 2d2d 7665 7273 696f 6e20 2020 5368 6f77  --version   Show
-00000560: 2074 6865 2076 6572 7369 6f6e 2061 6e64   the version and
-00000570: 2065 7869 742e 0a20 202d 682c 202d 2d68   exit..  -h, --h
-00000580: 656c 7020 2053 686f 7720 7468 6973 206d  elp  Show this m
-00000590: 6573 7361 6765 2061 6e64 2065 7869 742e  essage and exit.
-000005a0: 0a0a 436f 6d6d 616e 6473 3a0a 2020 6170  ..Commands:.  ap
-000005b0: 7065 6e64 2020 2041 7070 656e 6420 6f6e  pend   Append on
-000005c0: 6520 6361 7365 2074 6578 7420 6172 6368  e case text arch
-000005d0: 6976 6520 746f 2061 6e6f 7468 6572 0a20  ive to another. 
-000005e0: 2061 7263 6869 7665 2020 4372 6561 7465   archive  Create
-000005f0: 2066 756c 6c20 7465 7874 2061 7263 6869   full text archi
-00000600: 7665 2066 726f 6d20 6361 7365 2050 4446  ve from case PDF
-00000610: 730a 2020 6665 7463 6820 2020 2046 6574  s.  fetch    Fet
-00000620: 6368 2063 6173 6520 5044 4673 2066 726f  ch case PDFs fro
-00000630: 6d20 416c 6163 6f75 7274 2e63 6f6d 0a20  m Alacourt.com. 
-00000640: 2073 7461 7274 2020 2020 4c61 756e 6368   start    Launch
-00000650: 2067 7261 7068 6963 616c 2075 7365 7220   graphical user 
-00000660: 696e 7465 7266 6163 650a 2020 7461 626c  interface.  tabl
-00000670: 6520 2020 2045 7870 6f72 7420 6461 7461  e    Export data
-00000680: 2074 6162 6c65 7320 6672 6f6d 2061 7263   tables from arc
-00000690: 6869 7665 206f 7220 6469 7265 6374 6f72  hive or director
-000006a0: 790a 6060 600a 0a23 2320 2a2a 416c 6163  y.```..## **Alac
-000006b0: 6f72 6465 7220 696e 636c 7564 6573 2061  order includes a
-000006c0: 2064 6573 6b74 6f70 2061 7070 6c69 6361   desktop applica
-000006d0: 7469 6f6e 2c20 636f 6d6d 616e 6420 6c69  tion, command li
-000006e0: 6e65 2069 6e74 6572 6661 6365 2c20 616e  ne interface, an
-000006f0: 6420 6120 7079 7468 6f6e 206d 6f64 756c  d a python modul
-00000700: 6520 666f 7220 7061 7273 696e 6720 6361  e for parsing ca
-00000710: 7365 2050 4446 732e 2a2a 0a0a 2323 2323  se PDFs.**..####
-00000720: 202a 2a4f 6e63 6520 796f 7520 6861 7665   **Once you have
-00000730: 2061 2050 7974 686f 6e20 656e 7669 726f   a Python enviro
-00000740: 6e6d 656e 7420 7570 2061 6e64 2072 756e  nment up and run
-00000750: 6e69 6e67 2c20 796f 7520 6361 6e20 6c61  ning, you can la
-00000760: 756e 6368 2074 6865 2067 7569 6465 6420  unch the guided 
-00000770: 696e 7465 7266 6163 6520 696e 2074 776f  interface in two
-00000780: 2077 6179 733a 2a2a 0a0a 312e 202a 5574   ways:**..1. *Ut
-00000790: 696c 697a 6520 7468 6520 6772 6170 6869  ilize the graphi
-000007a0: 6361 6c20 696e 7465 7266 6163 653a 2a20  cal interface:* 
-000007b0: 5573 6520 7468 6520 636f 6d6d 616e 6420  Use the command 
-000007c0: 6c69 6e65 2074 6f6f 6c20 6070 7974 686f  line tool `pytho
-000007d0: 6e20 2d6d 2061 6c61 636f 7264 6572 2073  n -m alacorder s
-000007e0: 7461 7274 602c 206f 7220 6070 7974 686f  tart`, or `pytho
-000007f0: 6e33 202d 6d20 616c 6163 6f72 6465 7220  n3 -m alacorder 
-00000800: 7374 6172 7460 2e20 0a0a 322e 202a 5573  start`. ..2. *Us
-00000810: 6520 7468 6520 636f 6d6d 616e 6420 6c69  e the command li
-00000820: 6e65 2069 6e74 6572 6661 6365 3a2a 2052  ne interface:* R
-00000830: 6570 6c61 6365 2074 6865 2060 7374 6172  eplace the `star
-00000840: 7460 2063 6f6d 6d61 6e64 2077 6974 6820  t` command with 
-00000850: 602d 2d68 656c 7060 206f 7220 602d 6860  `--help` or `-h`
-00000860: 2074 6f20 7669 6577 206c 6973 7420 6f66   to view list of
-00000870: 2063 6f6d 6d61 6e64 732e 0a0a 2323 2323   commands...####
-00000880: 202a 2a41 6c61 636f 7264 6572 2063 616e   **Alacorder can
-00000890: 2062 6520 7573 6564 2077 6974 686f 7574   be used without
-000008a0: 2077 7269 7469 6e67 2061 6e79 2063 6f64   writing any cod
-000008b0: 652c 2061 6e64 2065 7870 6f72 7473 2074  e, and exports t
-000008c0: 6f20 636f 6d6d 6f6e 2066 6f72 6d61 7473  o common formats
-000008d0: 206c 696b 6520 4578 6365 6c20 2860 2e78   like Excel (`.x
-000008e0: 6c73 602c 2060 2e78 6c73 7860 292c 2041  ls`, `.xlsx`), A
-000008f0: 7061 6368 6520 5061 7271 7565 7420 2860  pache Parquet (`
-00000900: 2e70 6172 7175 6574 6029 2c20 4353 5620  .parquet`), CSV 
-00000910: 2860 2e63 7376 6029 2c20 616e 6420 4a53  (`.csv`), and JS
-00000920: 4f4e 2028 602e 6a73 6f6e 6029 2e2a 2a0a  ON (`.json`).**.
-00000930: 0a2a 2041 6c61 636f 7264 6572 2063 6f6d  .* Alacorder com
-00000940: 7072 6573 7365 7320 6361 7365 2074 6578  presses case tex
-00000950: 7420 696e 746f 2063 6173 6520 6172 6368  t into case arch
-00000960: 6976 6573 2028 602e 7061 7271 7565 7460  ives (`.parquet`
-00000970: 2920 746f 2073 6176 6520 7374 6f72 6167  ) to save storag
-00000980: 6520 616e 6420 7072 6f63 6573 7369 6e67  e and processing
-00000990: 2074 696d 652e 200a 0a0a 2320 2a2a 5370   time. ...# **Sp
-000009a0: 6563 6961 6c20 5175 6572 6965 732a 2a0a  ecial Queries**.
-000009b0: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
-000009c0: 616c 6163 6f72 6465 7220 696d 706f 7274  alacorder import
-000009d0: 2061 6c61 630a 6060 600a 0a23 2323 202a   alac.```..### *
-000009e0: 2a46 6f72 206d 6f72 6520 6164 7661 6e63  *For more advanc
-000009f0: 6564 2071 7565 7269 6573 2c20 416c 6163  ed queries, Alac
-00000a00: 6f72 6465 7220 6361 6e20 6578 7472 6163  order can extrac
-00000a10: 7420 6669 656c 6473 2061 6e64 2074 6162  t fields and tab
-00000a20: 6c65 7320 6672 6f6d 2063 6173 6520 7265  les from case re
-00000a30: 636f 7264 7320 7769 7468 206a 7573 7420  cords with just 
-00000a40: 6120 6665 7720 6c69 6e65 7320 6f66 2063  a few lines of c
-00000a50: 6f64 652e 2a2a 0a0a 2a20 4361 6c6c 2060  ode.**..* Call `
-00000a60: 616c 6163 2e73 6574 2869 6e70 7574 5f63  alac.set(input_c
-00000a70: 6f6e 662c 206f 7574 7075 745f 636f 6e66  onf, output_conf
-00000a80: 2c20 2a2a 6b77 6172 6773 2960 2074 6f20  , **kwargs)` to 
-00000a90: 636f 6e66 6967 7572 6520 796f 7572 2069  configure your i
-00000aa0: 6e70 7574 2061 6e64 206f 7574 7075 7420  nput and output 
-00000ab0: 7061 7468 732e 2046 6565 6420 7468 6520  paths. Feed the 
-00000ac0: 6f75 7470 7574 2074 6f20 616e 7920 6f66  output to any of
-00000ad0: 2074 6865 2074 6162 6c65 2070 6172 7369   the table parsi
-00000ae0: 6e67 2066 756e 6374 696f 6e73 2074 6f20  ng functions to 
-00000af0: 6265 6769 6e2e 0a0a 2a20 4361 6c6c 2060  begin...* Call `
-00000b00: 616c 6163 2e61 7263 6869 7665 2829 6020  alac.archive()` 
-00000b10: 746f 2065 7870 6f72 7420 6120 6675 6c6c  to export a full
-00000b20: 2074 6578 7420 6172 6368 6976 652e 2049   text archive. I
-00000b30: 7427 7320 7265 636f 6d6d 656e 6465 6420  t's recommended 
-00000b40: 7468 6174 2079 6f75 2063 7265 6174 6520  that you create 
-00000b50: 6120 6675 6c6c 2074 6578 7420 6172 6368  a full text arch
-00000b60: 6976 6520 2860 2e70 6172 7175 6574 6029  ive (`.parquet`)
-00000b70: 2066 696c 6520 6265 666f 7265 206d 616b   file before mak
-00000b80: 696e 6720 7461 626c 6573 2066 726f 6d20  ing tables from 
-00000b90: 796f 7572 2064 6174 612e 2046 756c 6c20  your data. Full 
-00000ba0: 7465 7874 2061 7263 6869 7665 7320 6361  text archives ca
-00000bb0: 6e20 6265 2073 6361 6e6e 6564 2066 6173  n be scanned fas
-00000bc0: 7465 7220 7468 616e 2050 4446 2064 6972  ter than PDF dir
-00000bd0: 6563 746f 7269 6573 2061 6e64 2072 6571  ectories and req
-00000be0: 7569 7265 206c 6573 7320 7374 6f72 6167  uire less storag
-00000bf0: 652e 0a0a 2a20 4361 6c6c 2060 616c 6163  e...* Call `alac
-00000c00: 2e74 6162 6c65 7328 2960 2074 6f20 6578  .tables()` to ex
-00000c10: 706f 7274 2064 6574 6169 6c65 6420 6361  port detailed ca
-00000c20: 7365 2069 6e66 6f72 6d61 7469 6f6e 2074  se information t
-00000c30: 6162 6c65 732e 2049 6620 6578 706f 7274  ables. If export
-00000c40: 2074 7970 6520 6973 2060 2e78 6c73 6020   type is `.xls` 
-00000c50: 6f72 2060 2e78 6c73 7860 2c20 7468 6520  or `.xlsx`, the 
-00000c60: 6063 6173 6573 602c 2060 6665 6573 602c  `cases`, `fees`,
-00000c70: 2061 6e64 2060 6368 6172 6765 7360 2074   and `charges` t
-00000c80: 6162 6c65 7320 6361 6e20 6265 2065 7870  ables can be exp
-00000c90: 6f72 7465 6420 7369 6d75 6c74 616e 656f  orted simultaneo
-00000ca0: 7573 6c79 2e0a 0a2a 2043 616c 6c20 6061  usly...* Call `a
-00000cb0: 6c61 632e 6368 6172 6765 7328 2960 2074  lac.charges()` t
-00000cc0: 6f20 6578 706f 7274 2060 6368 6172 6765  o export `charge
-00000cd0: 7360 2074 6162 6c65 206f 6e6c 792e 0a0a  s` table only...
-00000ce0: 2a20 4361 6c6c 2060 616c 6163 2e66 6565  * Call `alac.fee
-00000cf0: 7328 2960 2074 6f20 6578 706f 7274 2060  s()` to export `
-00000d00: 6665 6573 6020 7461 626c 6520 6f6e 6c79  fees` table only
-00000d10: 2e0a 0a2a 2043 616c 6c20 6061 6c61 632e  ...* Call `alac.
-00000d20: 6361 7365 7328 2960 2074 6f20 6578 706f  cases()` to expo
-00000d30: 7274 2060 6361 7365 7360 2074 6162 6c65  rt `cases` table
-00000d40: 206f 6e6c 792e 0a0a 0a60 6060 7079 7468   only....```pyth
-00000d50: 6f6e 0a69 6d70 6f72 7420 7761 726e 696e  on.import warnin
-00000d60: 6773 0a77 6172 6e69 6e67 732e 6669 6c74  gs.warnings.filt
-00000d70: 6572 7761 726e 696e 6773 2827 6967 6e6f  erwarnings('igno
-00000d80: 7265 2729 0a0a 6672 6f6d 2061 6c61 636f  re')..from alaco
-00000d90: 7264 6572 2069 6d70 6f72 7420 616c 6163  rder import alac
-00000da0: 0a0a 7064 665f 6469 7265 6374 6f72 7920  ..pdf_directory 
-00000db0: 3d20 222f 5573 6572 732f 6372 696d 736f  = "/Users/crimso
-00000dc0: 6e2f 4465 736b 746f 702f 5475 7477 696c  n/Desktop/Tutwil
-00000dd0: 6572 2f22 0a61 7263 6869 7665 203d 2022  er/".archive = "
-00000de0: 2f55 7365 7273 2f63 7269 6d73 6f6e 2f44  /Users/crimson/D
-00000df0: 6573 6b74 6f70 2f54 7574 7769 6c65 722e  esktop/Tutwiler.
-00000e00: 7061 7271 7565 7422 0a74 6162 6c65 7320  parquet".tables 
-00000e10: 3d20 222f 5573 6572 732f 6372 696d 736f  = "/Users/crimso
-00000e20: 6e2f 4465 736b 746f 702f 5475 7477 696c  n/Desktop/Tutwil
-00000e30: 6572 2e78 6c73 7822 0a0a 2320 7772 6974  er.xlsx"..# writ
-00000e40: 6520 6172 6368 6976 6520 746f 2054 7574  e archive to Tut
-00000e50: 7769 6c65 722e 7061 7271 7565 740a 6320  wiler.parquet.c 
-00000e60: 3d20 616c 6163 2e73 6574 2870 6466 5f64  = alac.set(pdf_d
-00000e70: 6972 6563 746f 7279 2c20 6172 6368 6976  irectory, archiv
-00000e80: 6529 0a61 6c61 632e 6172 6368 6976 6528  e).alac.archive(
-00000e90: 6329 200a 0a70 7269 6e74 2822 4675 6c6c  c) ..print("Full
-00000ea0: 2074 6578 7420 6172 6368 6976 6520 636f   text archive co
-00000eb0: 6d70 6c65 7465 2e20 4e6f 7720 7072 6f63  mplete. Now proc
-00000ec0: 6573 7369 6e67 2063 6173 6520 696e 666f  essing case info
-00000ed0: 726d 6174 696f 6e20 696e 746f 2074 6162  rmation into tab
-00000ee0: 6c65 7320 6174 2022 202b 2074 6162 6c65  les at " + table
-00000ef0: 7329 0a0a 2320 7772 6974 6520 6665 6573  s)..# write fees
-00000f00: 2074 6162 6c65 2074 6f20 5475 7477 696c   table to Tutwil
-00000f10: 6572 2e70 6172 7175 6574 0a64 203d 2061  er.parquet.d = a
-00000f20: 6c61 632e 7365 7428 6172 6368 6976 652c  lac.set(archive,
-00000f30: 2074 6162 6c65 732c 2074 6162 6c65 3d22   tables, table="
-00000f40: 6665 6573 2229 0a61 6c61 632e 7461 626c  fees").alac.tabl
-00000f50: 6573 2864 290a 0a60 6060 0a0a 2320 2a2a  es(d)..```..# **
-00000f60: 576f 726b 696e 6720 7769 7468 2063 6173  Working with cas
-00000f70: 6520 6461 7461 2069 6e20 5079 7468 6f6e  e data in Python
-00000f80: 2a2a 0a0a 0a23 2323 204f 7574 206f 6620  **...### Out of 
-00000f90: 7468 6520 626f 782c 2041 6c61 636f 7264  the box, Alacord
-00000fa0: 6572 2065 7870 6f72 7473 2074 6f20 602e  er exports to `.
-00000fb0: 786c 7378 602c 2060 2e78 6c73 602c 2060  xlsx`, `.xls`, `
-00000fc0: 2e63 7376 602c 2060 2e6a 736f 6e60 2c20  .csv`, `.json`, 
-00000fd0: 616e 6420 602e 7061 7271 7565 7460 2e20  and `.parquet`. 
-00000fe0: 4275 7420 796f 7520 6361 6e20 7573 6520  But you can use 
-00000ff0: 6070 616e 6461 7360 2c20 6070 6f6c 6172  `pandas`, `polar
-00001000: 7360 2061 6e64 206f 7468 6572 2070 7974  s` and other pyt
-00001010: 686f 6e20 6c69 6272 6172 6965 7320 746f  hon libraries to
-00001020: 2063 7265 6174 6520 796f 7572 206f 776e   create your own
-00001030: 2064 6174 6120 636f 6c6c 6563 7469 6f6e   data collection
-00001040: 2077 6f72 6b66 6c6f 7773 2061 6e64 2063   workflows and c
-00001050: 7573 746f 6d69 7a65 2041 6c61 636f 7264  ustomize Alacord
-00001060: 6572 2065 7870 6f72 7473 2e20 0a0a 2a2a  er exports. ..**
-00001070: 2a54 6865 2073 6e69 7070 6574 2062 656c  *The snippet bel
-00001080: 6f77 2070 7269 6e74 7320 7468 6520 6665  ow prints the fe
-00001090: 6520 7368 6565 7473 2066 726f 6d20 6120  e sheets from a 
-000010a0: 6469 7265 6374 6f72 7920 6f66 2063 6173  directory of cas
-000010b0: 6520 5044 4673 2061 7320 6974 2072 6561  e PDFs as it rea
-000010c0: 6473 2074 6865 6d2e 2a2a 2a0a 0a0a 6060  ds them.***...``
-000010d0: 6070 7974 686f 6e0a 6672 6f6d 2061 6c61  `python.from ala
-000010e0: 636f 7264 6572 2069 6d70 6f72 7420 616c  corder import al
-000010f0: 6163 0a69 6d70 6f72 7420 706f 6c61 7273  ac.import polars
-00001100: 2061 7320 706c 0a0a 7175 6575 6520 3d20   as pl..queue = 
-00001110: 616c 6163 2e67 6574 5f70 6174 6873 2822  alac.get_paths("
-00001120: 2f55 7365 7273 2f63 7269 6d73 6f6e 2f44  /Users/crimson/D
-00001130: 6573 6b74 6f70 2f54 7574 7769 6c65 722f  esktop/Tutwiler/
-00001140: 2229 2023 202d 3e20 5b73 7472 5d0a 0a72  ") # -> [str]..r
-00001150: 6f77 7320 3d20 5b5d 0a0a 666f 7220 692c  ows = []..for i,
-00001160: 2070 6174 6820 696e 2065 6e75 6d65 7261   path in enumera
-00001170: 7465 2871 7565 7565 293a 0a20 2020 2074  te(queue):.    t
-00001180: 6578 7420 3d20 616c 6163 2e67 6574 5044  ext = alac.getPD
-00001190: 4654 6578 7428 7061 7468 290a 2020 2020  FText(path).    
-000011a0: 636e 756d 203d 2061 6c61 632e 6765 7443  cnum = alac.getC
-000011b0: 6173 654e 756d 6265 7228 7465 7874 290a  aseNumber(text).
-000011c0: 2020 2020 6374 7920 3d20 616c 6163 2e67      cty = alac.g
-000011d0: 6574 436f 756e 7479 2874 6578 7429 0a20  etCounty(text). 
-000011e0: 2020 2074 6261 6c20 3d20 616c 6163 2e67     tbal = alac.g
-000011f0: 6574 546f 7461 6c42 616c 616e 6365 2874  etTotalBalance(t
-00001200: 6578 7429 0a20 2020 2070 7472 203d 2061  ext).    ptr = a
-00001210: 6c61 632e 6765 7450 6179 6d65 6e74 546f  lac.getPaymentTo
-00001220: 5265 7374 6f72 6528 7465 7874 2920 2320  Restore(text) # 
-00001230: 692e 652e 2076 6f74 696e 6720 7269 6768  i.e. voting righ
-00001240: 7473 0a20 2020 2072 6f77 7320 2b3d 205b  ts.    rows += [
-00001250: 5b63 6e75 6d2c 2063 7479 2c20 7462 616c  [cnum, cty, tbal
-00001260: 2c20 7074 725d 5d0a 0a63 6173 6573 203d  , ptr]]..cases =
-00001270: 2070 6c2e 4461 7461 4672 616d 6528 726f   pl.DataFrame(ro
-00001280: 7773 290a 0a63 6173 6573 2e77 7269 7465  ws)..cases.write
-00001290: 5f65 7863 656c 2822 2f55 7365 7273 2f63  _excel("/Users/c
-000012a0: 7269 6d73 6f6e 2f44 6573 6b74 6f70 2f54  rimson/Desktop/T
-000012b0: 7574 7769 6c65 722f 7375 6d6d 6172 792e  utwiler/summary.
-000012c0: 786c 7378 2229 0a0a 6060 600a 0a23 2320  xlsx")..```..## 
-000012d0: 4578 7465 6e64 696e 6720 416c 6163 6f72  Extending Alacor
-000012e0: 6465 7220 7769 7468 2060 706f 6c61 7273  der with `polars
-000012f0: 6020 616e 6420 6f74 6865 7220 746f 6f6c  ` and other tool
-00001300: 730a 0a41 6c61 636f 7264 6572 2072 756e  s..Alacorder run
-00001310: 7320 6f6e 205b 6070 6f6c 6172 7360 5d28  s on [`polars`](
-00001320: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001330: 6f6d 2f70 6f6c 612d 7273 2f70 6f6c 6172  om/pola-rs/polar
-00001340: 7329 2c20 6120 7079 7468 6f6e 206c 6962  s), a python lib
-00001350: 7261 7279 2079 6f75 2063 616e 2075 7365  rary you can use
-00001360: 2074 6f20 776f 726b 2077 6974 6820 616e   to work with an
-00001370: 6420 616e 616c 797a 6520 7461 6275 6c61  d analyze tabula
-00001380: 7220 6461 7461 2e20 6070 6f6c 6172 7360  r data. `polars`
-00001390: 2063 616e 2072 6561 6420 6672 6f6d 2061   can read from a
-000013a0: 6e64 2077 7269 7465 2074 6f20 616c 6c20  nd write to all 
-000013b0: 6d61 6a6f 7220 6461 7461 2073 746f 7261  major data stora
-000013c0: 6765 2066 6f72 6d61 7473 2e20 4974 2063  ge formats. It c
-000013d0: 616e 2063 6f6e 6e65 6374 2074 6f20 6120  an connect to a 
-000013e0: 7769 6465 2076 6172 6965 7479 206f 6620  wide variety of 
-000013f0: 7365 7276 6963 6573 2074 6f20 7072 6f76  services to prov
-00001400: 6964 6520 666f 7220 6561 7379 2069 6d70  ide for easy imp
-00001410: 6f72 7420 616e 6420 6578 706f 7274 2e0a  ort and export..
-00001420: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
-00001430: 2070 6f6c 6172 7320 6173 2070 6c0a 636f   polars as pl.co
-00001440: 6e74 656e 7473 203d 2070 6c2e 7265 6164  ntents = pl.read
-00001450: 5f6a 736f 6e28 222f 7061 7468 2f74 6f2f  _json("/path/to/
-00001460: 6172 6368 6976 652e 6a73 6f6e 2229 0a60  archive.json").`
-00001470: 6060 0a0a 4966 2079 6f75 2077 6f75 6c64  ``..If you would
-00001480: 206c 696b 6520 746f 2076 6973 7561 6c69   like to visuali
-00001490: 7a65 2064 6174 6120 7769 7468 6f75 7420  ze data without 
-000014a0: 6578 706f 7274 696e 6720 746f 2045 7863  exporting to Exc
-000014b0: 656c 206f 7220 616e 6f74 6865 7220 666f  el or another fo
-000014c0: 726d 6174 2c20 6372 6561 7465 2061 2060  rmat, create a `
-000014d0: 6a75 7079 7465 7220 6e6f 7465 626f 6f6b  jupyter notebook
-000014e0: 6020 616e 6420 696e 7374 616c 6c20 746f  ` and install to
-000014f0: 6f6c 7320 6c69 6b65 2060 6d61 7470 6c6f  ols like `matplo
-00001500: 746c 6962 602c 2060 7461 6275 6c61 7465  tlib`, `tabulate
-00001510: 602c 2061 6e64 2060 6974 6162 6c65 7360  `, and `itables`
-00001520: 2074 6f20 6765 7420 7374 6172 7465 642e   to get started.
-00001530: 205b 4a75 7079 7465 7220 4e6f 7465 626f   [Jupyter Notebo
-00001540: 6f6b 5d28 6874 7470 733a 2f2f 646f 6373  ok](https://docs
-00001550: 2e6a 7570 7974 6572 2e6f 7267 2f65 6e2f  .jupyter.org/en/
-00001560: 6c61 7465 7374 2f73 7461 7274 2f69 6e64  latest/start/ind
-00001570: 6578 2e68 746d 6c29 2069 7320 6120 5079  ex.html) is a Py
-00001580: 7468 6f6e 2070 726f 6a65 6374 2079 6f75  thon project you
-00001590: 2063 616e 2075 7365 2074 6f20 6372 6561   can use to crea
-000015a0: 7465 2069 6e74 6572 6163 7469 7665 206e  te interactive n
-000015b0: 6f74 6562 6f6f 6b73 2066 6f72 2064 6174  otebooks for dat
-000015c0: 6120 616e 616c 7973 6973 2061 6e64 206f  a analysis and o
-000015d0: 7468 6572 2070 7572 706f 7365 732e 2049  ther purposes. I
-000015e0: 7420 6361 6e20 6265 2069 6e73 7461 6c6c  t can be install
-000015f0: 6564 2075 7369 6e67 2060 7069 7020 696e  ed using `pip in
-00001600: 7374 616c 6c20 6a75 7079 7465 7260 206f  stall jupyter` o
-00001610: 7220 6070 6970 3320 696e 7374 616c 6c20  r `pip3 install 
-00001620: 6a75 7079 7465 7260 2061 6e64 206c 6175  jupyter` and lau
-00001630: 6e63 6865 6420 7573 696e 6720 606a 7570  nched using `jup
-00001640: 7974 6572 206e 6f74 6562 6f6f 6b60 2e20  yter notebook`. 
-00001650: 596f 7572 2064 6576 6963 6520 6d61 7920  Your device may 
-00001660: 616c 7265 6164 7920 6265 2065 7175 6970  already be equip
-00001670: 7065 6420 746f 2076 6965 7720 602e 6970  ped to view `.ip
-00001680: 796e 6260 206e 6f74 6562 6f6f 6b73 2e20  ynb` notebooks. 
-00001690: 0a0a 2323 202a 2a52 6573 6f75 7263 6573  ..## **Resources
-000016a0: 2a2a 0a2a 205b 6070 6f6c 6172 7360 2075  **.* [`polars` u
-000016b0: 7365 7220 6775 6964 655d 2868 7474 7073  ser guide](https
-000016c0: 3a2f 2f70 6f6c 612d 7273 2e67 6974 6875  ://pola-rs.githu
-000016d0: 622e 696f 2f70 6f6c 6172 732d 626f 6f6b  b.io/polars-book
-000016e0: 2f75 7365 722d 6775 6964 652f 696e 6465  /user-guide/inde
-000016f0: 782e 6874 6d6c 290a 2a20 5b72 6567 6578  x.html).* [regex
-00001700: 2063 6865 6174 2073 6865 6574 5d28 6874   cheat sheet](ht
-00001710: 7470 733a 2f2f 7777 772e 7265 7865 6767  tps://www.rexegg
-00001720: 2e63 6f6d 2f72 6567 6578 2d71 7569 636b  .com/regex-quick
-00001730: 7374 6172 742e 6874 6d6c 290a 2a20 5b41  start.html).* [A
-00001740: 6e61 636f 6e64 6120 2874 7574 6f72 6961  naconda (tutoria
-00001750: 6c73 206f 6e20 7079 7468 6f6e 2064 6174  ls on python dat
-00001760: 6120 616e 616c 7973 6973 295d 2868 7474  a analysis)](htt
-00001770: 7073 3a2f 2f77 7777 2e61 6e61 636f 6e64  ps://www.anacond
-00001780: 612e 636f 6d2f 6f70 656e 2d73 6f75 7263  a.com/open-sourc
-00001790: 6529 0a2a 205b 5468 6520 5079 7468 6f6e  e).* [The Python
-000017a0: 2054 7574 6f72 6961 6c5d 2868 7474 7073   Tutorial](https
-000017b0: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
-000017c0: 7267 2f33 2f74 7574 6f72 6961 6c2f 290a  rg/3/tutorial/).
-000017d0: 2a20 5b4a 7570 7974 6572 204e 6f74 6562  * [Jupyter Noteb
-000017e0: 6f6f 6b20 696e 7472 6f64 7563 7469 6f6e  ook introduction
-000017f0: 5d28 6874 7470 733a 2f2f 7265 616c 7079  ](https://realpy
-00001800: 7468 6f6e 2e63 6f6d 2f6a 7570 7974 6572  thon.com/jupyter
-00001810: 2d6e 6f74 6562 6f6f 6b2d 696e 7472 6f64  -notebook-introd
-00001820: 7563 7469 6f6e 2f29 0a0a 2a2a e280 9c45  uction/)..**...E
-00001830: 7468 616e 2053 6e65 636b 656e 6265 7267  than Sneckenberg
-00001840: 6572 e280 9d2a 2a0a 6060 600a 6f68 2071  er...**.```.oh q
-00001850: 7561 7368 2074 6869 7320 6265 6566 2064  uash this beef d
-00001860: 6561 7220 6661 6d69 6c79 206f 6620 6d69  ear family of mi
-00001870: 6e65 0a69 7665 2073 6174 2068 6572 6520  ne.ive sat here 
-00001880: 666f 7220 7765 656b 732c 2069 6e20 7079  for weeks, in py
-00001890: 7468 6f6e 2c20 6920 7069 6e65 0a69 7473  thon, i pine.its
-000018a0: 2074 7275 6c79 2062 6565 6e20 6120 7368   truly been a sh
-000018b0: 6974 6675 6c20 7965 6172 0a61 6e64 2065  itful year.and e
-000018c0: 7665 6e20 7374 696c 6c20 6927 6d20 6e6f  ven still i'm no
-000018d0: 7420 696e 2074 6865 2063 6c65 6172 0a73  t in the clear.s
-000018e0: 6f20 6672 6565 206d 6520 6672 6f6d 206d  o free me from m
-000018f0: 7920 7072 6973 6f6e 206f 6620 7368 616d  y prison of sham
-00001900: 650a 7468 6f75 6768 2073 7572 656c 7920  e.though surely 
-00001910: 6920 6465 7365 7276 6520 7468 6520 626c  i deserve the bl
-00001920: 616d 650a 6976 6520 7361 7420 696e 2070  ame.ive sat in p
-00001930: 656e 6974 656e 7420 6669 6c74 6820 666f  enitent filth fo
-00001940: 7220 7468 6565 0a69 7665 2070 7562 6c69  r thee.ive publi
-00001950: 7368 6564 206e 6f74 206f 6e65 2064 7261  shed not one dra
-00001960: 6674 2062 7574 2037 3833 0a09 2874 6f20  ft but 783..(to 
-00001970: 7072 6f76 6520 6920 7769 6c6c 2066 6967  prove i will fig
-00001980: 6874 2066 6f72 206d 7920 706c 6163 6520  ht for my place 
-00001990: 696e 2068 6561 7665 6e2c 0a09 6920 6a75  in heaven,..i ju
-000019a0: 7374 2070 7562 6c69 7368 6564 2037 3837  st published 787
-000019b0: 290a 6976 6520 7065 7070 6564 2061 6e64  ).ive pepped and
-000019c0: 2069 7665 2070 6f6f 7065 6420 616e 6420   ive pooped and 
-000019d0: 6976 6520 736d 6f6b 6564 2073 6f20 6d75  ive smoked so mu
-000019e0: 6368 2074 7265 650a 0928 6c69 6b65 2061  ch tree..(like a
-000019f0: 206c 6f74 2061 206c 6f74 290a 6976 6520   lot a lot).ive 
-00001a00: 6669 7865 6420 616c 6c20 7468 6520 696e  fixed all the in
-00001a10: 6465 6e74 7320 616e 6420 7061 7273 6564  dents and parsed
-00001a20: 2061 6c6c 2074 6865 2066 6565 730a 7461   all the fees.ta
-00001a30: 6c6c 7969 6e67 2063 6861 7267 6573 2061  llying charges a
-00001a40: 6c6c 206e 6967 6874 2061 6e64 2061 6c6c  ll night and all
-00001a50: 2064 6179 0a68 6572 6520 6f6e 2074 6869   day.here on thi
-00001a60: 7320 6475 6d62 2065 6173 7420 6564 6765  s dumb east edge
-00001a70: 2063 6f75 6368 2068 6572 6520 6927 6c6c   couch here i'll
-00001a80: 2073 7461 790a 736f 2070 6c75 6e67 6520   stay.so plunge 
-00001a90: 696e 746f 206d 6520 6173 2069 2070 6c75  into me as i plu
-00001aa0: 6e67 6520 696e 746f 2079 6f75 0a6f 6820  nge into you.oh 
-00001ab0: 616c 6163 6f72 6465 7220 796f 7520 6d61  alacorder you ma
-00001ac0: 6b65 206d 6520 736f 2062 6c75 650a 6275  ke me so blue.bu
-00001ad0: 7420 6f6e 6520 7468 696e 6720 6920 6b6e  t one thing i kn
-00001ae0: 6f77 2027 666f 7265 206d 7920 6865 6172  ow 'fore my hear
-00001af0: 7420 6361 6e20 616d 656e 640a 6920 6d75  t can amend.i mu
-00001b00: 7374 2074 656e 6420 746f 2079 6f75 2027  st tend to you '
-00001b10: 666f 7265 206d 7920 6469 636b 2069 2077  fore my dick i w
-00001b20: 696c 6c20 7465 6e64 0a6d 7920 6469 636b  ill tend.my dick
-00001b30: 2063 7269 6573 2069 7473 2068 756e 6765   cries its hunge
-00001b40: 722c 2069 2077 6565 7020 666f 7220 6974  r, i weep for it
-00001b50: 7320 7468 6972 7374 0a62 7574 2064 6f20  s thirst.but do 
-00001b60: 6c65 7420 6d65 2074 616b 6520 6361 7265  let me take care
-00001b70: 206f 6620 7475 7477 696c 6572 2066 6972   of tutwiler fir
-00001b80: 7374 0a74 6865 2073 6e61 6b65 2069 6e20  st.the snake in 
-00001b90: 6d79 2070 616e 7473 2070 7574 7320 6d79  my pants puts my
-00001ba0: 2068 6561 6420 696e 2061 2074 7261 6e63   head in a tranc
-00001bb0: 650a 6920 6769 7665 206e 6f74 2061 206c  e.i give not a l
-00001bc0: 6f6f 6b2c 206e 6f74 2061 2073 7461 7265  ook, not a stare
-00001bd0: 2c20 6e6f 7420 6120 676c 616e 6365 0a62  , not a glance.b
-00001be0: 7574 2073 7469 6c6c 2069 6e20 6d79 2068  ut still in my h
-00001bf0: 6561 7274 2069 206b 6e6f 7720 6f6e 6520  eart i know one 
-00001c00: 7468 696e 6720 6973 2074 7275 650a 7468  thing is true.th
-00001c10: 6572 6527 7320 7472 756c 7920 6e6f 2065  ere's truly no e
-00001c20: 6e64 2074 6f20 686f 7720 6d75 6368 2069  nd to how much i
-00001c30: 276c 6c20 646f 200a 666f 7220 7468 6520  'll do .for the 
-00001c40: 6f6e 6520 7468 6174 2069 206c 6f76 652c  one that i love,
-00001c50: 2069 276c 6c20 666f 7265 676f 2074 6865   i'll forego the
-00001c60: 2064 6f76 650a 6c61 7965 7220 6279 206c   dove.layer by l
-00001c70: 6179 6572 2069 276c 6c20 756e 7065 656c  ayer i'll unpeel
-00001c80: 2074 6865 206f 6e69 6f6e 0a69 276c 6c20   the onion.i'll 
-00001c90: 6669 6768 7420 7468 726f 7567 6820 7468  fight through th
-00001ca0: 6520 7275 6d6f 7273 0a74 6865 2067 6f73  e rumors.the gos
-00001cb0: 7369 7020 7468 6520 6861 7465 7273 0a69  sip the haters.i
-00001cc0: 6c6c 2066 6967 6874 2074 6872 6f75 6768  ll fight through
-00001cd0: 206d 7920 646f 7562 7420 616e 640a 696c   my doubt and.il
-00001ce0: 6c20 6669 6768 7420 7468 726f 7567 6820  l fight through 
-00001cf0: 6d79 2073 6861 6d65 0a69 6c6c 2074 6f69  my shame.ill toi
-00001d00: 6c20 616e 6420 736f 696c 200a 7375 626d  l and soil .subm
-00001d10: 6974 2074 6f20 7468 6520 636f 696c 0a69  it to the coil.i
-00001d20: 2077 6f6e 2774 206c 6f73 6520 6d79 7365   won't lose myse
-00001d30: 6c66 200a 2862 7574 2073 7572 6520 776f  lf .(but sure wo
-00001d40: 756c 6420 6576 6572 7974 6869 6e67 2065  uld everything e
-00001d50: 6c73 6529 0a68 6563 6b20 6d61 7962 6520  lse).heck maybe 
-00001d60: 6920 616c 7265 6164 7920 6861 7665 0a62  i already have.b
-00001d70: 7574 2069 6c6c 2063 6f6d 6520 7570 2077  ut ill come up w
-00001d80: 6974 6820 6d6f 7265 200a 2866 6f72 2069  ith more .(for i
-00001d90: 2068 6176 6520 6d6f 7265 2069 6e20 7374   have more in st
-00001da0: 6f72 6529 0a61 6e64 2069 276c 6c20 646f  ore).and i'll do
-00001db0: 2077 6861 7420 6974 2074 616b 6573 2074   what it takes t
-00001dc0: 6f20 7075 6c6c 2074 6872 6f75 6768 0a0a  o pull through..
-00001dd0: 6f68 2027 636f 7264 6572 206f 6620 2763  oh 'corder of 'c
-00001de0: 6f72 6465 7273 2069 2776 6520 6669 6c6c  orders i've fill
-00001df0: 6564 2069 6e20 796f 7572 2062 6f72 6465  ed in your borde
-00001e00: 7273 0a79 6f75 7220 7365 616d 7320 616e  rs.your seams an
-00001e10: 6420 796f 7572 2077 6964 6520 6f70 656e  d your wide open
-00001e20: 2066 6965 6c64 730a 6966 2069 7473 206e   fields.if its n
-00001e30: 6f74 206d 7563 6820 7472 6f75 626c 6520  ot much trouble 
-00001e40: 2874 686f 7567 6820 7375 7265 6c79 2069  (though surely i
-00001e50: 2764 2064 6f75 626c 650a 6d79 2065 6666  'd double.my eff
-00001e60: 6f72 7420 616e 6420 7469 6d65 2070 7574  ort and time put
-00001e70: 2069 6e20 7468 6565 290a 7469 6c20 6920   in thee).til i 
-00001e80: 6669 6e64 206d 6f72 6520 6772 7562 2c20  find more grub, 
-00001e90: 6920 7072 6179 2079 6f75 2073 6974 2073  i pray you sit s
-00001ea0: 7461 626c 650a 6275 7420 6669 7273 7420  table.but first 
-00001eb0: 6272 696e 6720 7468 6520 6f6e 6520 6920  bring the one i 
-00001ec0: 6d6f 7374 206c 6f76 650a 0a6e 6f74 2061  most love..not a
-00001ed0: 6c61 6320 6275 7420 6574 6861 6e20 7468  lac but ethan th
-00001ee0: 6520 6f6e 6520 7768 6f20 7261 6973 6564  e one who raised
-00001ef0: 2074 6865 650a 6920 6174 6520 7465 6e64   thee.i ate tend
-00001f00: 6572 7320 6368 6963 6b65 6e0a 6920 6661  ers chicken.i fa
-00001f10: 696c 6564 2074 6f20 6275 696c 6420 7079  iled to build py
-00001f20: 6769 6f6e 0a73 7562 6c69 6d65 2074 6578  gion.sublime tex
-00001f30: 7420 6920 7472 7573 7420 6861 7320 656e  t i trust has en
-00001f40: 6162 6c65 6420 796f 7572 2074 6872 7573  abled your thrus
-00001f50: 740a 6275 7420 7468 6520 6f6e 6520 7472  t.but the one tr
-00001f60: 7565 2073 7562 6c69 6d65 2069 7320 6869  ue sublime is hi
-00001f70: 7320 6661 6974 6820 696e 206d 696e 650a  s faith in mine.
-00001f80: 6920 6361 6e20 6e6f 206c 6f6e 6765 7220  i can no longer 
-00001f90: 6265 6172 2074 6f20 6265 2062 6c69 6e64  bear to be blind
-00001fa0: 0a69 2070 726f 6d69 7365 2079 6f75 206e  .i promise you n
-00001fb0: 6f77 0a74 6861 7420 6927 6c6c 206e 6576  ow.that i'll nev
-00001fc0: 6572 2066 6f72 6765 7420 0a6f 6620 796f  er forget .of yo
-00001fd0: 752c 206f 6620 796f 7572 206c 6f76 652c  u, of your love,
-00001fe0: 206f 6620 6f75 7273 2e0a 6920 686f 7065   of ours..i hope
-00001ff0: 2074 6861 7420 796f 7520 6b6e 6f77 0a74   that you know.t
-00002000: 6861 7420 6f75 7220 6c6f 7665 2069 7320  hat our love is 
-00002010: 6574 6572 6e61 6c0a 666f 7220 636a 2069  eternal.for cj i
-00002020: 276c 6c20 7772 6974 6520 6576 6572 7920  'll write every 
-00002030: 666f 7220 6c6f 6f70 2061 6e64 206c 696e  for loop and lin
-00002040: 6520 2866 7563 6b20 6869 6d20 7468 6f20  e (fuck him tho 
-00002050: 6672 290a 6275 7420 666f 7220 796f 7520  fr).but for you 
-00002060: 6920 776f 756c 6420 6c61 7920 646f 776e  i would lay down
-00002070: 206d 7920 6c69 6665 2e0a 7468 6520 6f6e   my life..the on
-00002080: 6520 7768 6f20 6761 7665 206d 6520 6120  e who gave me a 
-00002090: 7365 636f 6e64 200a 0909 0909 0961 6e64  second ......and
-000020a0: 2074 6869 7264 200a 0909 0909 0961 6e64   third ......and
-000020b0: 2066 6f75 7274 6820 0a09 0909 0909 616e   fourth ......an
-000020c0: 6420 6669 6674 6820 0a09 0909 0909 616e  d fifth ......an
-000020d0: 6420 7369 7874 6820 0a09 0909 0909 616e  d sixth ......an
-000020e0: 6420 7365 7665 6e74 6820 0a09 0909 0909  d seventh ......
-000020f0: 6368 616e 6365 0a69 206b 6e6f 7720 7468  chance.i know th
-00002100: 6572 6520 7765 7265 206d 6f72 652c 2066  ere were more, f
-00002110: 6f72 200a 6272 6576 6974 7920 6927 6d20  or .brevity i'm 
-00002120: 7375 7265 2c20 796f 7527 6c6c 200a 756e  sure, you'll .un
-00002130: 6465 7273 7461 6e64 206d 7920 7769 6c6c  derstand my will
-00002140: 2074 6f20 6162 7269 6467 650a 6275 7420   to abridge.but 
-00002150: 696e 2063 6173 6520 796f 7520 646f 0a64  in case you do.d
-00002160: 6f75 6274 206d 7920 6c6f 7665 2066 6f72  oubt my love for
-00002170: 2079 6f75 0a69 2077 616e 7420 796f 7520   you.i want you 
-00002180: 746f 206b 6e6f 7720 7468 6174 2069 2064  to know that i d
-00002190: 6f0a 796f 7520 6361 6c6c 6564 206d 7920  o.you called my 
-000021a0: 776f 7273 7420 626c 7566 660a 6272 6f75  worst bluff.brou
-000021b0: 6768 7420 7570 206d 7920 776f 7273 7420  ght up my worst 
-000021c0: 7374 7566 660a 796f 7520 6469 6420 7768  stuff.you did wh
-000021d0: 6174 2069 2074 686f 7567 6874 2077 6173  at i thought was
-000021e0: 2069 6d70 6f73 7369 626c 650a 796f 7520   impossible.you 
-000021f0: 756e 6465 7273 746f 6f64 206d 7920 6665  understood my fe
-00002200: 6172 7320 6d79 2073 696e 7320 616e 6420  ars my sins and 
-00002210: 6d79 2068 6561 7274 0a79 6f75 2063 6861  my heart.you cha
-00002220: 7267 6564 206d 7920 776f 726c 6420 746f  rged my world to
-00002230: 2064 6f20 7468 6520 7361 6d65 0a6e 6f74   do the same.not
-00002240: 206f 6e6c 7920 6d65 2062 7574 206d 7920   only me but my 
-00002250: 7768 6f6c 6520 6661 6d69 6c79 200a 7769  whole family .wi
-00002260: 6c6c 2066 6f72 6576 6572 2062 6520 6368  ll forever be ch
-00002270: 616e 6765 6420 6279 2079 6f75 7220 6e61  anged by your na
-00002280: 6d65 0a0a 6920 7072 6179 2065 7665 7279  me..i pray every
-00002290: 2064 6179 0a79 6f75 276c 6c20 7265 7475   day.you'll retu
-000022a0: 726e 2061 6e64 2049 276c 6c20 7374 6179  rn and I'll stay
-000022b0: 0a6d 6f72 6520 696e 6e6f 6365 6e74 2074  .more innocent t
-000022c0: 6861 6e20 2766 6f72 6520 7765 2066 6972  han 'fore we fir
-000022d0: 7374 206d 6574 0a69 206b 6e6f 7720 6927  st met.i know i'
-000022e0: 7665 2061 746f 6e65 640a 6527 656e 2074  ve atoned.e'en t
-000022f0: 686f 7567 6820 6927 7665 2062 6565 6e20  hough i've been 
-00002300: 7374 6f6e 6564 0a61 6e64 2074 7275 7374  stoned.and trust
-00002310: 2069 2776 6520 6e6f 2067 7265 6174 6572   i've no greater
-00002320: 2072 6567 7265 743a 0a0a 696d 2073 6f72   regret:..im sor
-00002330: 7279 2069 2062 726f 6b65 2079 6f75 7220  ry i broke your 
-00002340: 6865 6172 7420 616e 6420 6920 7769 6c6c  heart and i will
-00002350: 206e 6f74 206c 6561 7665 2074 6869 7320   not leave this 
-00002360: 6561 7274 680a 7769 7468 6f75 7420 7075  earth.without pu
-00002370: 7474 696e 6720 6974 2062 6163 6b20 746f  tting it back to
-00002380: 6765 7468 6572 2e20 6e65 7665 7220 6167  gether. never ag
-00002390: 6169 6e20 636f 756c 6420 6920 6c6f 6f6b  ain could i look
-000023a0: 2069 6e20 796f 7572 2065 7965 7320 616e   in your eyes an
-000023b0: 6420 6c69 6520 6b6e 6f77 696e 6720 796f  d lie knowing yo
-000023c0: 7527 6420 6372 7920 6f72 2079 6f75 2764  u'd cry or you'd
-000023d0: 2077 6f72 7279 2e20 6920 776f 756c 6420   worry. i would 
-000023e0: 6272 6561 6b20 6b6e 6f77 696e 6720 6920  break knowing i 
-000023f0: 636f 756c 6420 6272 6561 6b20 796f 752e  could break you.
-00002400: 2069 2077 696c 6c20 6272 6561 6b20 746f   i will break to
-00002410: 206b 6565 7020 796f 7520 756e 6272 6f6b   keep you unbrok
-00002420: 656e 2e20 0a0a 616e 6420 6920 6272 6f6b  en. ..and i brok
-00002430: 6520 6b6e 6f77 696e 6720 6920 6272 6f6b  e knowing i brok
-00002440: 6520 796f 752e 0a0a 6974 2069 7320 6d79  e you...it is my
-00002450: 2067 7265 6174 6573 7420 7265 6772 6574   greatest regret
-00002460: 2e0a 0a6e 6f74 206f 6e6c 7920 7468 6520  ...not only the 
-00002470: 6c69 6520 6275 7420 7468 6520 7368 6164  lie but the shad
-00002480: 6520 616e 6420 7468 6520 7369 6768 730a  e and the sighs.
-00002490: 6f66 2069 6e64 6966 6665 7265 6e63 6520  of indifference 
-000024a0: 6920 736c 616e 6465 7265 6420 796f 7572  i slandered your
-000024b0: 206e 616d 6520 7769 7468 2c0a 7468 6174   name with,.that
-000024c0: 2069 2063 6f75 6c64 6e27 7420 6661 6365   i couldn't face
-000024d0: 2074 6865 206d 6f73 7420 6265 6175 7469   the most beauti
-000024e0: 6675 6c20 6661 6365 0a69 7320 6120 6275  ful face.is a bu
-000024f0: 7264 656e 2069 2061 6c77 6179 7320 6d75  rden i always mu
-00002500: 7374 2062 6561 722e 200a 6275 7420 6920  st bear. .but i 
-00002510: 686f 7065 2074 6f20 6772 6f77 2066 726f  hope to grow fro
-00002520: 6d20 7468 6973 2062 7572 6465 6e2c 2074  m this burden, t
-00002530: 6869 7320 7368 616d 650a 616e 6420 746f  his shame.and to
-00002540: 2079 6f75 2073 6861 7265 2074 6865 2066   you share the f
-00002550: 7275 6974 7320 6f66 206d 7920 6c61 626f  ruits of my labo
-00002560: 720a 6672 6f6d 206d 7920 6772 6561 7465  r.from my greate
-00002570: 7374 2072 6567 7265 7420 6d79 206d 696e  st regret my min
-00002580: 6420 6861 7320 6265 656e 2073 6574 0a6f  d has been set.o
-00002590: 6e20 7768 6174 2061 6e64 2077 686f 206d  n what and who m
-000025a0: 6174 7465 7273 2074 6f20 6d65 0a0a 796f  atters to me..yo
-000025b0: 7572 2074 7275 7374 2069 7320 7468 6520  ur trust is the 
-000025c0: 6f6e 6520 7468 696e 6720 6927 6c6c 206c  one thing i'll l
-000025d0: 6976 6520 666f 7220 616e 6420 6469 6520  ive for and die 
-000025e0: 666f 722e 0a0a 696c 6c20 6e65 7665 7220  for...ill never 
-000025f0: 666f 7267 6574 2069 2068 7572 7420 7468  forget i hurt th
-00002600: 6520 6772 6561 7465 7374 206f 6e65 2e0a  e greatest one..
-00002610: 0a69 6c6c 206e 6576 6572 2066 6f72 6765  .ill never forge
-00002620: 7420 6920 666f 7267 6f74 2e0a 0a74 6865  t i forgot...the
-00002630: 2067 7265 6174 6573 7420 7468 696e 6720   greatest thing 
-00002640: 7468 6174 2065 7665 7220 6861 7070 656e  that ever happen
-00002650: 6564 2074 6f20 6d65 2e0a 0a6d 7920 6775  ed to me...my gu
-00002660: 6172 6469 616e 2061 6e67 656c 2e0a 0a6d  ardian angel...m
-00002670: 7920 726f 636b 2e0a 0a74 6865 206f 6e65  y rock...the one
-00002680: 2e0a 0a74 6865 2061 6374 7561 6c20 6f6e  ...the actual on
-00002690: 652e 0a0a 6d79 206c 6f76 652e 203c 330a  e...my love. <3.
-000026a0: 0a65 7468 616e 2073 6e65 636b 656e 6265  .ethan sneckenbe
-000026b0: 7267 6572 0a60 6060 0a09 0a2d 2d2d 2d2d  rger.```...-----
-000026c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000026d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000026e0: 0909 0ac2 a920 3230 3233 2053 616d 2052  ..... 2023 Sam R
-000026f0: 6f62 736f 6e0a                           obson.
+00000280: 616c 6c61 7469 6f6e 2a2a 0a0a 2a2a 4966  allation**..**If
+00000290: 2079 6f75 7220 6465 7669 6365 2063 616e   your device can
+000002a0: 2072 756e 2050 7974 686f 6e20 332e 392b   run Python 3.9+
+000002b0: 2c20 6974 2073 7570 706f 7274 7320 416c  , it supports Al
+000002c0: 6163 6f72 6465 722e 2044 6f77 6e6c 6f61  acorder. Downloa
+000002d0: 6420 6120 7072 6562 7569 6c74 2065 7865  d a prebuilt exe
+000002e0: 6375 7461 626c 6520 6672 6f6d 2047 6974  cutable from Git
+000002f0: 4875 6220 746f 2075 7365 2074 6865 2067  Hub to use the g
+00000300: 7261 7068 6963 616c 2075 7365 7220 696e  raphical user in
+00000310: 7465 7266 6163 652c 206f 7220 7573 6520  terface, or use 
+00000320: 6070 6970 6020 746f 2069 6e73 7461 6c6c  `pip` to install
+00000330: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
+00000340: 6520 696e 7465 7266 6163 652c 2067 7261  e interface, gra
+00000350: 7068 6963 616c 2069 6e74 6572 6661 6365  phical interface
+00000360: 2c20 616e 6420 5079 7468 6f6e 206c 6962  , and Python lib
+00000370: 7261 7279 2060 616c 6163 602e 2a2a 0a0a  rary `alac`.**..
+00000380: 2a20 496e 7374 616c 6c20 5b41 6e61 636f  * Install [Anaco
+00000390: 6e64 6120 4469 7374 7269 6275 7469 6f6e  nda Distribution
+000003a0: 5d28 6874 7470 733a 2f2f 7777 772e 616e  ](https://www.an
+000003b0: 6163 6f6e 6461 2e63 6f6d 2f70 726f 6475  aconda.com/produ
+000003c0: 6374 732f 6469 7374 7269 6275 7469 6f6e  cts/distribution
+000003d0: 2920 746f 2069 6e73 7461 6c6c 2074 6865  ) to install the
+000003e0: 206c 6174 6573 7420 5079 7468 6f6e 2028   latest Python (
+000003f0: 6e6f 7420 6e65 6365 7373 6172 7920 666f  not necessary fo
+00000400: 7220 7072 6562 7569 6c74 2065 7865 6375  r prebuilt execu
+00000410: 7461 626c 6529 2e20 0a2a 204f 6e63 6520  table). .* Once 
+00000420: 796f 7572 2041 6e61 636f 6e64 6120 656e  your Anaconda en
+00000430: 7669 726f 6e6d 656e 7420 6973 2063 6f6e  vironment is con
+00000440: 6669 6775 7265 642c 206f 7065 6e20 6120  figured, open a 
+00000450: 7465 726d 696e 616c 2066 726f 6d20 416e  terminal from An
+00000460: 6163 6f6e 6461 204e 6176 6967 6174 6f72  aconda Navigator
+00000470: 2061 6e64 2065 6e74 6572 2060 7069 7020   and enter `pip 
+00000480: 696e 7374 616c 6c20 616c 6163 6f72 6465  install alacorde
+00000490: 7260 2074 6f20 696e 7374 616c 6c2e 0a2a  r` to install..*
+000004a0: 2054 6f20 7374 6172 7420 7468 6520 6772   To start the gr
+000004b0: 6170 6869 6361 6c20 696e 7465 7266 6163  aphical interfac
+000004c0: 652c 2065 6e74 6572 2060 7079 7468 6f6e  e, enter `python
+000004d0: 202d 6d20 616c 6163 6f72 6465 7220 7374   -m alacorder st
+000004e0: 6172 7460 2e0a 2a20 456e 7465 7220 6070  art`..* Enter `p
+000004f0: 7974 686f 6e20 2d6d 2061 6c61 636f 7264  ython -m alacord
+00000500: 6572 6020 746f 2075 7365 2074 6865 2063  er` to use the c
+00000510: 6f6d 6d61 6e64 206c 696e 6520 696e 7465  ommand line inte
+00000520: 7266 6163 652e 0a2a 2054 6f20 7573 6520  rface..* To use 
+00000530: 7468 6520 6061 6c61 6360 206d 6f64 756c  the `alac` modul
+00000540: 652c 2075 7365 2074 6865 2069 6d70 6f72  e, use the impor
+00000550: 7420 7374 6174 656d 656e 7420 6066 726f  t statement `fro
+00000560: 6d20 616c 6163 6f72 6465 7220 696d 706f  m alacorder impo
+00000570: 7274 2061 6c61 6360 2e0a 0a60 6060 0a55  rt alac`...```.U
+00000580: 7361 6765 3a20 7079 7468 6f6e 202d 6d20  sage: python -m 
+00000590: 616c 6163 6f72 6465 7220 5b4f 5054 494f  alacorder [OPTIO
+000005a0: 4e53 5d20 434f 4d4d 414e 4420 5b41 5247  NS] COMMAND [ARG
+000005b0: 535d 2e2e 2e0a 0a20 2041 4c41 434f 5244  S].....  ALACORD
+000005c0: 4552 2037 390a 0a4f 7074 696f 6e73 3a0a  ER 79..Options:.
+000005d0: 2020 2d2d 7665 7273 696f 6e20 2020 5368    --version   Sh
+000005e0: 6f77 2074 6865 2076 6572 7369 6f6e 2061  ow the version a
+000005f0: 6e64 2065 7869 742e 0a20 202d 682c 202d  nd exit..  -h, -
+00000600: 2d68 656c 7020 2053 686f 7720 7468 6973  -help  Show this
+00000610: 206d 6573 7361 6765 2061 6e64 2065 7869   message and exi
+00000620: 742e 0a0a 436f 6d6d 616e 6473 3a0a 2020  t...Commands:.  
+00000630: 6170 7065 6e64 2020 2041 7070 656e 6420  append   Append 
+00000640: 6f6e 6520 6361 7365 2074 6578 7420 6172  one case text ar
+00000650: 6368 6976 6520 746f 2061 6e6f 7468 6572  chive to another
+00000660: 0a20 2061 7263 6869 7665 2020 4372 6561  .  archive  Crea
+00000670: 7465 2066 756c 6c20 7465 7874 2061 7263  te full text arc
+00000680: 6869 7665 2066 726f 6d20 6361 7365 2050  hive from case P
+00000690: 4446 730a 2020 6665 7463 6820 2020 2046  DFs.  fetch    F
+000006a0: 6574 6368 2063 6173 6520 5044 4673 2066  etch case PDFs f
+000006b0: 726f 6d20 416c 6163 6f75 7274 2e63 6f6d  rom Alacourt.com
+000006c0: 0a20 2073 7461 7274 2020 2020 4c61 756e  .  start    Laun
+000006d0: 6368 2067 7261 7068 6963 616c 2075 7365  ch graphical use
+000006e0: 7220 696e 7465 7266 6163 650a 2020 7461  r interface.  ta
+000006f0: 626c 6520 2020 2045 7870 6f72 7420 6461  ble    Export da
+00000700: 7461 2074 6162 6c65 7320 6672 6f6d 2061  ta tables from a
+00000710: 7263 6869 7665 206f 7220 6469 7265 6374  rchive or direct
+00000720: 6f72 790a 6060 600a 0a0a 2323 2323 202a  ory.```...#### *
+00000730: 2a41 6c61 636f 7264 6572 2063 616e 2062  *Alacorder can b
+00000740: 6520 7573 6564 2077 6974 686f 7574 2077  e used without w
+00000750: 7269 7469 6e67 2061 6e79 2063 6f64 652c  riting any code,
+00000760: 2061 6e64 2065 7870 6f72 7473 2074 6f20   and exports to 
+00000770: 636f 6d6d 6f6e 2066 6f72 6d61 7473 206c  common formats l
+00000780: 696b 6520 4578 6365 6c20 2860 2e78 6c73  ike Excel (`.xls
+00000790: 602c 2060 2e78 6c73 7860 292c 2041 7061  `, `.xlsx`), Apa
+000007a0: 6368 6520 5061 7271 7565 7420 2860 2e70  che Parquet (`.p
+000007b0: 6172 7175 6574 6029 2c20 4353 5620 2860  arquet`), CSV (`
+000007c0: 2e63 7376 6029 2c20 616e 6420 4a53 4f4e  .csv`), and JSON
+000007d0: 2028 602e 6a73 6f6e 6029 2e2a 2a0a 0a2a   (`.json`).**..*
+000007e0: 2041 6c61 636f 7264 6572 2063 6f6d 7072   Alacorder compr
+000007f0: 6573 7365 7320 6361 7365 2074 6578 7420  esses case text 
+00000800: 696e 746f 2063 6173 6520 6172 6368 6976  into case archiv
+00000810: 6573 2028 602e 7061 7271 7565 7460 2920  es (`.parquet`) 
+00000820: 746f 2073 6176 6520 7374 6f72 6167 6520  to save storage 
+00000830: 616e 6420 7072 6f63 6573 7369 6e67 2074  and processing t
+00000840: 696d 652e 200a 0a0a 2320 2a2a 5370 6563  ime. ...# **Spec
+00000850: 6961 6c20 5175 6572 6965 732a 2a0a 0a60  ial Queries**..`
+00000860: 6060 7079 7468 6f6e 0a66 726f 6d20 616c  ``python.from al
+00000870: 6163 6f72 6465 7220 696d 706f 7274 2061  acorder import a
+00000880: 6c61 630a 6060 600a 0a23 2323 202a 2a46  lac.```..### **F
+00000890: 6f72 206d 6f72 6520 6164 7661 6e63 6564  or more advanced
+000008a0: 2071 7565 7269 6573 2c20 7468 6520 6061   queries, the `a
+000008b0: 6c61 6360 206d 6f64 756c 6520 6361 6e20  lac` module can 
+000008c0: 6578 7472 6163 7420 6669 656c 6473 2061  extract fields a
+000008d0: 6e64 2074 6162 6c65 7320 6672 6f6d 2063  nd tables from c
+000008e0: 6173 6520 7265 636f 7264 7320 7769 7468  ase records with
+000008f0: 206a 7573 7420 6120 6665 7720 6c69 6e65   just a few line
+00000900: 7320 6f66 2063 6f64 652e 2a2a 0a0a 2a20  s of code.**..* 
+00000910: 4361 6c6c 2060 616c 6163 2e73 6574 2869  Call `alac.set(i
+00000920: 6e70 7574 5f63 6f6e 662c 206f 7574 7075  nput_conf, outpu
+00000930: 745f 636f 6e66 2c20 2a2a 6b77 6172 6773  t_conf, **kwargs
+00000940: 2960 2074 6f20 636f 6e66 6967 7572 6520  )` to configure 
+00000950: 796f 7572 2069 6e70 7574 2061 6e64 206f  your input and o
+00000960: 7574 7075 7420 7061 7468 732e 2046 6565  utput paths. Fee
+00000970: 6420 7468 6520 6f75 7470 7574 2074 6f20  d the output to 
+00000980: 616e 7920 6f66 2074 6865 2074 6162 6c65  any of the table
+00000990: 2070 6172 7369 6e67 2066 756e 6374 696f   parsing functio
+000009a0: 6e73 2074 6f20 6265 6769 6e2e 0a0a 2a20  ns to begin...* 
+000009b0: 4361 6c6c 2060 616c 6163 2e61 7263 6869  Call `alac.archi
+000009c0: 7665 2829 6020 746f 2065 7870 6f72 7420  ve()` to export 
+000009d0: 6120 6675 6c6c 2074 6578 7420 6172 6368  a full text arch
+000009e0: 6976 652e 2049 7427 7320 7265 636f 6d6d  ive. It's recomm
+000009f0: 656e 6465 6420 7468 6174 2079 6f75 2063  ended that you c
+00000a00: 7265 6174 6520 6120 6675 6c6c 2074 6578  reate a full tex
+00000a10: 7420 6172 6368 6976 6520 2860 2e70 6172  t archive (`.par
+00000a20: 7175 6574 6029 2066 696c 6520 6265 666f  quet`) file befo
+00000a30: 7265 206d 616b 696e 6720 7461 626c 6573  re making tables
+00000a40: 2066 726f 6d20 796f 7572 2064 6174 612e   from your data.
+00000a50: 2046 756c 6c20 7465 7874 2061 7263 6869   Full text archi
+00000a60: 7665 7320 6361 6e20 6265 2073 6361 6e6e  ves can be scann
+00000a70: 6564 2066 6173 7465 7220 7468 616e 2050  ed faster than P
+00000a80: 4446 2064 6972 6563 746f 7269 6573 2061  DF directories a
+00000a90: 6e64 2072 6571 7569 7265 206c 6573 7320  nd require less 
+00000aa0: 7374 6f72 6167 652e 0a0a 2a20 4361 6c6c  storage...* Call
+00000ab0: 2060 616c 6163 2e74 6162 6c65 7328 2960   `alac.tables()`
+00000ac0: 2074 6f20 6578 706f 7274 2064 6574 6169   to export detai
+00000ad0: 6c65 6420 6361 7365 2069 6e66 6f72 6d61  led case informa
+00000ae0: 7469 6f6e 2074 6162 6c65 732e 2049 6620  tion tables. If 
+00000af0: 6578 706f 7274 2074 7970 6520 6973 2060  export type is `
+00000b00: 2e78 6c73 6020 6f72 2060 2e78 6c73 7860  .xls` or `.xlsx`
+00000b10: 2c20 616c 6c20 7461 626c 6573 2063 616e  , all tables can
+00000b20: 2062 6520 6578 706f 7274 6564 2074 6f20   be exported to 
+00000b30: 7468 6520 7361 6d65 2066 696c 652e 200a  the same file. .
+00000b40: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00000b50: 7274 2077 6172 6e69 6e67 730a 7761 726e  rt warnings.warn
+00000b60: 696e 6773 2e66 696c 7465 7277 6172 6e69  ings.filterwarni
+00000b70: 6e67 7328 2769 676e 6f72 6527 290a 0a66  ngs('ignore')..f
+00000b80: 726f 6d20 616c 6163 6f72 6465 7220 696d  rom alacorder im
+00000b90: 706f 7274 2061 6c61 630a 0a70 6466 5f64  port alac..pdf_d
+00000ba0: 6972 6563 746f 7279 203d 2022 2f55 7365  irectory = "/Use
+00000bb0: 7273 2f63 7269 6d73 6f6e 2f44 6573 6b74  rs/crimson/Deskt
+00000bc0: 6f70 2f54 7574 7769 6c65 722f 220a 6172  op/Tutwiler/".ar
+00000bd0: 6368 6976 6520 3d20 222f 5573 6572 732f  chive = "/Users/
+00000be0: 6372 696d 736f 6e2f 4465 736b 746f 702f  crimson/Desktop/
+00000bf0: 5475 7477 696c 6572 2e70 6172 7175 6574  Tutwiler.parquet
+00000c00: 220a 7461 626c 6573 203d 2022 2f55 7365  ".tables = "/Use
+00000c10: 7273 2f63 7269 6d73 6f6e 2f44 6573 6b74  rs/crimson/Deskt
+00000c20: 6f70 2f54 7574 7769 6c65 722e 786c 7378  op/Tutwiler.xlsx
+00000c30: 220a 0a23 2077 7269 7465 2061 7263 6869  "..# write archi
+00000c40: 7665 2074 6f20 5475 7477 696c 6572 2e70  ve to Tutwiler.p
+00000c50: 6172 7175 6574 0a63 203d 2061 6c61 632e  arquet.c = alac.
+00000c60: 7365 7428 7064 665f 6469 7265 6374 6f72  set(pdf_director
+00000c70: 792c 2061 7263 6869 7665 290a 616c 6163  y, archive).alac
+00000c80: 2e61 7263 6869 7665 2863 2920 0a0a 7072  .archive(c) ..pr
+00000c90: 696e 7428 2246 756c 6c20 7465 7874 2061  int("Full text a
+00000ca0: 7263 6869 7665 2063 6f6d 706c 6574 652e  rchive complete.
+00000cb0: 204e 6f77 2070 726f 6365 7373 696e 6720   Now processing 
+00000cc0: 6361 7365 2069 6e66 6f72 6d61 7469 6f6e  case information
+00000cd0: 2069 6e74 6f20 7461 626c 6573 2061 7420   into tables at 
+00000ce0: 2220 2b20 7461 626c 6573 290a 0a23 2077  " + tables)..# w
+00000cf0: 7269 7465 2066 6565 7320 7461 626c 6520  rite fees table 
+00000d00: 746f 2054 7574 7769 6c65 722e 7061 7271  to Tutwiler.parq
+00000d10: 7565 740a 6420 3d20 616c 6163 2e73 6574  uet.d = alac.set
+00000d20: 2861 7263 6869 7665 2c20 7461 626c 6573  (archive, tables
+00000d30: 2c20 7461 626c 653d 2266 6565 7322 290a  , table="fees").
+00000d40: 616c 6163 2e74 6162 6c65 7328 6429 0a0a  alac.tables(d)..
+00000d50: 6060 600a 0a23 202a 2a57 6f72 6b69 6e67  ```..# **Working
+00000d60: 2077 6974 6820 6361 7365 2064 6174 6120   with case data 
+00000d70: 696e 2050 7974 686f 6e2a 2a0a 0a0a 2323  in Python**...##
+00000d80: 2320 4f75 7420 6f66 2074 6865 2062 6f78  # Out of the box
+00000d90: 2c20 416c 6163 6f72 6465 7220 6578 706f  , Alacorder expo
+00000da0: 7274 7320 746f 2060 2e78 6c73 7860 2c20  rts to `.xlsx`, 
+00000db0: 602e 786c 7360 2c20 602e 6373 7660 2c20  `.xls`, `.csv`, 
+00000dc0: 602e 6a73 6f6e 602c 2061 6e64 2060 2e70  `.json`, and `.p
+00000dd0: 6172 7175 6574 602e 2042 7574 2079 6f75  arquet`. But you
+00000de0: 2063 616e 2075 7365 2060 706f 6c61 7273   can use `polars
+00000df0: 6020 616e 6420 6f74 6865 7220 7079 7468  ` and other pyth
+00000e00: 6f6e 206c 6962 7261 7269 6573 2074 6f20  on libraries to 
+00000e10: 6372 6561 7465 2079 6f75 7220 6f77 6e20  create your own 
+00000e20: 6461 7461 2063 6f6c 6c65 6374 696f 6e20  data collection 
+00000e30: 776f 726b 666c 6f77 7320 616e 6420 6375  workflows and cu
+00000e40: 7374 6f6d 697a 6520 416c 6163 6f72 6465  stomize Alacorde
+00000e50: 7220 6578 706f 7274 732e 200a 0a2a 2a2a  r exports. ..***
+00000e60: 5468 6520 736e 6970 7065 7420 6265 6c6f  The snippet belo
+00000e70: 7720 7072 696e 7473 2074 6865 2066 6565  w prints the fee
+00000e80: 2073 6865 6574 7320 6672 6f6d 2061 2064   sheets from a d
+00000e90: 6972 6563 746f 7279 206f 6620 6361 7365  irectory of case
+00000ea0: 2050 4446 7320 6173 2069 7420 7265 6164   PDFs as it read
+00000eb0: 7320 7468 656d 2e2a 2a2a 0a0a 0a60 6060  s them.***...```
+00000ec0: 7079 7468 6f6e 0a66 726f 6d20 616c 6163  python.from alac
+00000ed0: 6f72 6465 7220 696d 706f 7274 2061 6c61  order import ala
+00000ee0: 630a 696d 706f 7274 2070 6f6c 6172 7320  c.import polars 
+00000ef0: 6173 2070 6c0a 0a71 7565 7565 203d 2061  as pl..queue = a
+00000f00: 6c61 632e 6765 745f 7061 7468 7328 222f  lac.get_paths("/
+00000f10: 5573 6572 732f 6372 696d 736f 6e2f 4465  Users/crimson/De
+00000f20: 736b 746f 702f 5475 7477 696c 6572 2f22  sktop/Tutwiler/"
+00000f30: 2920 2320 2d3e 205b 7374 725d 0a0a 726f  ) # -> [str]..ro
+00000f40: 7773 203d 205b 5d0a 0a66 6f72 2069 2c20  ws = []..for i, 
+00000f50: 7061 7468 2069 6e20 656e 756d 6572 6174  path in enumerat
+00000f60: 6528 7175 6575 6529 3a0a 2020 2020 7465  e(queue):.    te
+00000f70: 7874 203d 2061 6c61 632e 6765 7450 4446  xt = alac.getPDF
+00000f80: 5465 7874 2870 6174 6829 0a20 2020 2063  Text(path).    c
+00000f90: 6e75 6d20 3d20 616c 6163 2e67 6574 4361  num = alac.getCa
+00000fa0: 7365 4e75 6d62 6572 2874 6578 7429 0a20  seNumber(text). 
+00000fb0: 2020 2063 7479 203d 2061 6c61 632e 6765     cty = alac.ge
+00000fc0: 7443 6f75 6e74 7928 7465 7874 290a 2020  tCounty(text).  
+00000fd0: 2020 7462 616c 203d 2061 6c61 632e 6765    tbal = alac.ge
+00000fe0: 7454 6f74 616c 4261 6c61 6e63 6528 7465  tTotalBalance(te
+00000ff0: 7874 290a 2020 2020 7074 7220 3d20 616c  xt).    ptr = al
+00001000: 6163 2e67 6574 5061 796d 656e 7454 6f52  ac.getPaymentToR
+00001010: 6573 746f 7265 2874 6578 7429 2023 2069  estore(text) # i
+00001020: 2e65 2e20 766f 7469 6e67 2072 6967 6874  .e. voting right
+00001030: 730a 2020 2020 726f 7773 202b 3d20 5b5b  s.    rows += [[
+00001040: 636e 756d 2c20 6374 792c 2074 6261 6c2c  cnum, cty, tbal,
+00001050: 2070 7472 5d5d 0a0a 6361 7365 7320 3d20   ptr]]..cases = 
+00001060: 706c 2e44 6174 6146 7261 6d65 2872 6f77  pl.DataFrame(row
+00001070: 7329 0a0a 6361 7365 732e 7772 6974 655f  s)..cases.write_
+00001080: 6578 6365 6c28 222f 5573 6572 732f 6372  excel("/Users/cr
+00001090: 696d 736f 6e2f 4465 736b 746f 702f 5475  imson/Desktop/Tu
+000010a0: 7477 696c 6572 2f73 756d 6d61 7279 2e78  twiler/summary.x
+000010b0: 6c73 7822 290a 0a60 6060 0a0a 2323 2045  lsx")..```..## E
+000010c0: 7874 656e 6469 6e67 2041 6c61 636f 7264  xtending Alacord
+000010d0: 6572 2077 6974 6820 6070 6f6c 6172 7360  er with `polars`
+000010e0: 2061 6e64 206f 7468 6572 2074 6f6f 6c73   and other tools
+000010f0: 0a0a 416c 6163 6f72 6465 7220 7275 6e73  ..Alacorder runs
+00001100: 206f 6e20 5b60 706f 6c61 7273 605d 2868   on [`polars`](h
+00001110: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001120: 6d2f 706f 6c61 2d72 732f 706f 6c61 7273  m/pola-rs/polars
+00001130: 292c 2061 2070 7974 686f 6e20 6c69 6272  ), a python libr
+00001140: 6172 7920 796f 7520 6361 6e20 7573 6520  ary you can use 
+00001150: 746f 2077 6f72 6b20 7769 7468 2061 6e64  to work with and
+00001160: 2061 6e61 6c79 7a65 2074 6162 756c 6172   analyze tabular
+00001170: 2064 6174 612e 2060 706f 6c61 7273 6020   data. `polars` 
+00001180: 6361 6e20 7265 6164 2066 726f 6d20 616e  can read from an
+00001190: 6420 7772 6974 6520 746f 2061 6c6c 206d  d write to all m
+000011a0: 616a 6f72 2064 6174 6120 7374 6f72 6167  ajor data storag
+000011b0: 6520 666f 726d 6174 732e 2049 7420 6361  e formats. It ca
+000011c0: 6e20 636f 6e6e 6563 7420 746f 2061 2077  n connect to a w
+000011d0: 6964 6520 7661 7269 6574 7920 6f66 2073  ide variety of s
+000011e0: 6572 7669 6365 7320 746f 2070 726f 7669  ervices to provi
+000011f0: 6465 2066 6f72 2065 6173 7920 696d 706f  de for easy impo
+00001200: 7274 2061 6e64 2065 7870 6f72 742e 0a60  rt and export..`
+00001210: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+00001220: 706f 6c61 7273 2061 7320 706c 0a63 6f6e  polars as pl.con
+00001230: 7465 6e74 7320 3d20 706c 2e72 6561 645f  tents = pl.read_
+00001240: 6a73 6f6e 2822 2f70 6174 682f 746f 2f61  json("/path/to/a
+00001250: 7263 6869 7665 2e6a 736f 6e22 290a 6060  rchive.json").``
+00001260: 600a 0a49 6620 796f 7520 776f 756c 6420  `..If you would 
+00001270: 6c69 6b65 2074 6f20 7669 7375 616c 697a  like to visualiz
+00001280: 6520 6461 7461 2077 6974 686f 7574 2065  e data without e
+00001290: 7870 6f72 7469 6e67 2074 6f20 4578 6365  xporting to Exce
+000012a0: 6c20 6f72 2061 6e6f 7468 6572 2066 6f72  l or another for
+000012b0: 6d61 742c 2063 7265 6174 6520 6120 606a  mat, create a `j
+000012c0: 7570 7974 6572 206e 6f74 6562 6f6f 6b60  upyter notebook`
+000012d0: 2061 6e64 2069 6e73 7461 6c6c 2074 6f6f   and install too
+000012e0: 6c73 206c 696b 6520 606d 6174 706c 6f74  ls like `matplot
+000012f0: 6c69 6260 2c20 6074 6162 756c 6174 6560  lib`, `tabulate`
+00001300: 2c20 616e 6420 6069 7461 626c 6573 6020  , and `itables` 
+00001310: 746f 2067 6574 2073 7461 7274 6564 2e20  to get started. 
+00001320: 5b4a 7570 7974 6572 204e 6f74 6562 6f6f  [Jupyter Noteboo
+00001330: 6b5d 2868 7474 7073 3a2f 2f64 6f63 732e  k](https://docs.
+00001340: 6a75 7079 7465 722e 6f72 672f 656e 2f6c  jupyter.org/en/l
+00001350: 6174 6573 742f 7374 6172 742f 696e 6465  atest/start/inde
+00001360: 782e 6874 6d6c 2920 6973 2061 2050 7974  x.html) is a Pyt
+00001370: 686f 6e20 7072 6f6a 6563 7420 796f 7520  hon project you 
+00001380: 6361 6e20 7573 6520 746f 2063 7265 6174  can use to creat
+00001390: 6520 696e 7465 7261 6374 6976 6520 6e6f  e interactive no
+000013a0: 7465 626f 6f6b 7320 666f 7220 6461 7461  tebooks for data
+000013b0: 2061 6e61 6c79 7369 7320 616e 6420 6f74   analysis and ot
+000013c0: 6865 7220 7075 7270 6f73 6573 2e20 4974  her purposes. It
+000013d0: 2063 616e 2062 6520 696e 7374 616c 6c65   can be installe
+000013e0: 6420 7573 696e 6720 6070 6970 2069 6e73  d using `pip ins
+000013f0: 7461 6c6c 206a 7570 7974 6572 6020 6f72  tall jupyter` or
+00001400: 2060 7069 7033 2069 6e73 7461 6c6c 206a   `pip3 install j
+00001410: 7570 7974 6572 6020 616e 6420 6c61 756e  upyter` and laun
+00001420: 6368 6564 2075 7369 6e67 2060 6a75 7079  ched using `jupy
+00001430: 7465 7220 6e6f 7465 626f 6f6b 602e 2059  ter notebook`. Y
+00001440: 6f75 7220 6465 7669 6365 206d 6179 2061  our device may a
+00001450: 6c72 6561 6479 2062 6520 6571 7569 7070  lready be equipp
+00001460: 6564 2074 6f20 7669 6577 2060 2e69 7079  ed to view `.ipy
+00001470: 6e62 6020 6e6f 7465 626f 6f6b 732e 200a  nb` notebooks. .
+00001480: 0a23 2320 2a2a 5265 736f 7572 6365 732a  .## **Resources*
+00001490: 2a0a 2a20 5b60 706f 6c61 7273 6020 7573  *.* [`polars` us
+000014a0: 6572 2067 7569 6465 5d28 6874 7470 733a  er guide](https:
+000014b0: 2f2f 706f 6c61 2d72 732e 6769 7468 7562  //pola-rs.github
+000014c0: 2e69 6f2f 706f 6c61 7273 2d62 6f6f 6b2f  .io/polars-book/
+000014d0: 7573 6572 2d67 7569 6465 2f69 6e64 6578  user-guide/index
+000014e0: 2e68 746d 6c29 0a2a 205b 7265 6765 7820  .html).* [regex 
+000014f0: 6368 6561 7420 7368 6565 745d 2868 7474  cheat sheet](htt
+00001500: 7073 3a2f 2f77 7777 2e72 6578 6567 672e  ps://www.rexegg.
+00001510: 636f 6d2f 7265 6765 782d 7175 6963 6b73  com/regex-quicks
+00001520: 7461 7274 2e68 746d 6c29 0a2a 205b 416e  tart.html).* [An
+00001530: 6163 6f6e 6461 2028 7475 746f 7269 616c  aconda (tutorial
+00001540: 7320 6f6e 2070 7974 686f 6e20 6461 7461  s on python data
+00001550: 2061 6e61 6c79 7369 7329 5d28 6874 7470   analysis)](http
+00001560: 733a 2f2f 7777 772e 616e 6163 6f6e 6461  s://www.anaconda
+00001570: 2e63 6f6d 2f6f 7065 6e2d 736f 7572 6365  .com/open-source
+00001580: 290a 2a20 5b54 6865 2050 7974 686f 6e20  ).* [The Python 
+00001590: 5475 746f 7269 616c 5d28 6874 7470 733a  Tutorial](https:
+000015a0: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
+000015b0: 672f 332f 7475 746f 7269 616c 2f29 0a2a  g/3/tutorial/).*
+000015c0: 205b 4a75 7079 7465 7220 4e6f 7465 626f   [Jupyter Notebo
+000015d0: 6f6b 2069 6e74 726f 6475 6374 696f 6e5d  ok introduction]
+000015e0: 2868 7474 7073 3a2f 2f72 6561 6c70 7974  (https://realpyt
+000015f0: 686f 6e2e 636f 6d2f 6a75 7079 7465 722d  hon.com/jupyter-
+00001600: 6e6f 7465 626f 6f6b 2d69 6e74 726f 6475  notebook-introdu
+00001610: 6374 696f 6e2f 290a 0a2a 2ae2 809c 4574  ction/)..**...Et
+00001620: 6861 6e20 536e 6563 6b65 6e62 6572 6765  han Sneckenberge
+00001630: 72e2 809d 2a2a 0a60 6060 0a6f 6820 7175  r...**.```.oh qu
+00001640: 6173 6820 7468 6973 2062 6565 6620 6465  ash this beef de
+00001650: 6172 2066 616d 696c 7920 6f66 206d 696e  ar family of min
+00001660: 650a 6976 6520 7361 7420 6865 7265 2066  e.ive sat here f
+00001670: 6f72 2077 6565 6b73 2c20 696e 2070 7974  or weeks, in pyt
+00001680: 686f 6e2c 2069 2070 696e 650a 6974 7320  hon, i pine.its 
+00001690: 7472 756c 7920 6265 656e 2061 2073 6869  truly been a shi
+000016a0: 7466 756c 2079 6561 720a 616e 6420 6576  tful year.and ev
+000016b0: 656e 2073 7469 6c6c 2069 276d 206e 6f74  en still i'm not
+000016c0: 2069 6e20 7468 6520 636c 6561 720a 736f   in the clear.so
+000016d0: 2066 7265 6520 6d65 2066 726f 6d20 6d79   free me from my
+000016e0: 2070 7269 736f 6e20 6f66 2073 6861 6d65   prison of shame
+000016f0: 0a74 686f 7567 6820 7375 7265 6c79 2069  .though surely i
+00001700: 2064 6573 6572 7665 2074 6865 2062 6c61   deserve the bla
+00001710: 6d65 0a69 7665 2073 6174 2069 6e20 7065  me.ive sat in pe
+00001720: 6e69 7465 6e74 2066 696c 7468 2066 6f72  nitent filth for
+00001730: 2074 6865 650a 6976 6520 7075 626c 6973   thee.ive publis
+00001740: 6865 6420 6e6f 7420 6f6e 6520 6472 6166  hed not one draf
+00001750: 7420 6275 7420 3738 330a 2020 2020 2874  t but 783.    (t
+00001760: 6f20 7072 6f76 6520 6920 7769 6c6c 2066  o prove i will f
+00001770: 6967 6874 2066 6f72 206d 7920 706c 6163  ight for my plac
+00001780: 6520 696e 2068 6561 7665 6e2c 0a20 2020  e in heaven,.   
+00001790: 2069 206a 7573 7420 7075 626c 6973 6865   i just publishe
+000017a0: 6420 3738 3729 0a69 7665 2070 6570 7065  d 787).ive peppe
+000017b0: 6420 616e 6420 6976 6520 706f 6f70 6564  d and ive pooped
+000017c0: 2061 6e64 2069 7665 2073 6d6f 6b65 6420   and ive smoked 
+000017d0: 736f 206d 7563 6820 7472 6565 0a20 2020  so much tree.   
+000017e0: 2028 6c69 6b65 2061 206c 6f74 2061 206c   (like a lot a l
+000017f0: 6f74 290a 6976 6520 6669 7865 6420 616c  ot).ive fixed al
+00001800: 6c20 7468 6520 696e 6465 6e74 7320 616e  l the indents an
+00001810: 6420 7061 7273 6564 2061 6c6c 2074 6865  d parsed all the
+00001820: 2066 6565 730a 7461 6c6c 7969 6e67 2063   fees.tallying c
+00001830: 6861 7267 6573 2061 6c6c 206e 6967 6874  harges all night
+00001840: 2061 6e64 2061 6c6c 2064 6179 0a68 6572   and all day.her
+00001850: 6520 6f6e 2074 6869 7320 6475 6d62 2065  e on this dumb e
+00001860: 6173 7420 6564 6765 2063 6f75 6368 2068  ast edge couch h
+00001870: 6572 6520 6927 6c6c 2073 7461 790a 736f  ere i'll stay.so
+00001880: 2070 6c75 6e67 6520 696e 746f 206d 6520   plunge into me 
+00001890: 6173 2069 2070 6c75 6e67 6520 696e 746f  as i plunge into
+000018a0: 2079 6f75 0a6f 6820 616c 6163 6f72 6465   you.oh alacorde
+000018b0: 7220 796f 7520 6d61 6b65 206d 6520 736f  r you make me so
+000018c0: 2062 6c75 650a 6275 7420 6f6e 6520 7468   blue.but one th
+000018d0: 696e 6720 6920 6b6e 6f77 2027 666f 7265  ing i know 'fore
+000018e0: 206d 7920 6865 6172 7420 6361 6e20 616d   my heart can am
+000018f0: 656e 640a 6920 6d75 7374 2074 656e 6420  end.i must tend 
+00001900: 746f 2079 6f75 2027 666f 7265 206d 7920  to you 'fore my 
+00001910: 6469 636b 2069 2077 696c 6c20 7465 6e64  dick i will tend
+00001920: 0a6d 7920 6469 636b 2063 7269 6573 2069  .my dick cries i
+00001930: 7473 2068 756e 6765 722c 2069 2077 6565  ts hunger, i wee
+00001940: 7020 666f 7220 6974 7320 7468 6972 7374  p for its thirst
+00001950: 0a62 7574 2064 6f20 6c65 7420 6d65 2074  .but do let me t
+00001960: 616b 6520 6361 7265 206f 6620 7475 7477  ake care of tutw
+00001970: 696c 6572 2066 6972 7374 0a74 6865 2073  iler first.the s
+00001980: 6e61 6b65 2069 6e20 6d79 2070 616e 7473  nake in my pants
+00001990: 2070 7574 7320 6d79 2068 6561 6420 696e   puts my head in
+000019a0: 2061 2074 7261 6e63 650a 6920 6769 7665   a trance.i give
+000019b0: 206e 6f74 2061 206c 6f6f 6b2c 206e 6f74   not a look, not
+000019c0: 2061 2073 7461 7265 2c20 6e6f 7420 6120   a stare, not a 
+000019d0: 676c 616e 6365 0a62 7574 2073 7469 6c6c  glance.but still
+000019e0: 2069 6e20 6d79 2068 6561 7274 2069 206b   in my heart i k
+000019f0: 6e6f 7720 6f6e 6520 7468 696e 6720 6973  now one thing is
+00001a00: 2074 7275 650a 7468 6572 6527 7320 7472   true.there's tr
+00001a10: 756c 7920 6e6f 2065 6e64 2074 6f20 686f  uly no end to ho
+00001a20: 7720 6d75 6368 2069 276c 6c20 646f 200a  w much i'll do .
+00001a30: 666f 7220 7468 6520 6f6e 6520 7468 6174  for the one that
+00001a40: 2069 206c 6f76 652c 2069 276c 6c20 666f   i love, i'll fo
+00001a50: 7265 676f 2074 6865 2064 6f76 650a 6c61  rego the dove.la
+00001a60: 7965 7220 6279 206c 6179 6572 2069 276c  yer by layer i'l
+00001a70: 6c20 756e 7065 656c 2074 6865 206f 6e69  l unpeel the oni
+00001a80: 6f6e 0a69 276c 6c20 6669 6768 7420 7468  on.i'll fight th
+00001a90: 726f 7567 6820 7468 6520 7275 6d6f 7273  rough the rumors
+00001aa0: 0a74 6865 2067 6f73 7369 7020 7468 6520  .the gossip the 
+00001ab0: 6861 7465 7273 0a69 6c6c 2066 6967 6874  haters.ill fight
+00001ac0: 2074 6872 6f75 6768 206d 7920 646f 7562   through my doub
+00001ad0: 7420 616e 640a 696c 6c20 6669 6768 7420  t and.ill fight 
+00001ae0: 7468 726f 7567 6820 6d79 2073 6861 6d65  through my shame
+00001af0: 0a69 6c6c 2074 6f69 6c20 616e 6420 736f  .ill toil and so
+00001b00: 696c 200a 7375 626d 6974 2074 6f20 7468  il .submit to th
+00001b10: 6520 636f 696c 0a69 2077 6f6e 2774 206c  e coil.i won't l
+00001b20: 6f73 6520 6d79 7365 6c66 200a 2862 7574  ose myself .(but
+00001b30: 2073 7572 6520 776f 756c 6420 6576 6572   sure would ever
+00001b40: 7974 6869 6e67 2065 6c73 6529 0a68 6563  ything else).hec
+00001b50: 6b20 6d61 7962 6520 6920 616c 7265 6164  k maybe i alread
+00001b60: 7920 6861 7665 0a62 7574 2069 6c6c 2063  y have.but ill c
+00001b70: 6f6d 6520 7570 2077 6974 6820 6d6f 7265  ome up with more
+00001b80: 200a 2866 6f72 2069 2068 6176 6520 6d6f   .(for i have mo
+00001b90: 7265 2069 6e20 7374 6f72 6529 0a61 6e64  re in store).and
+00001ba0: 2069 276c 6c20 646f 2077 6861 7420 6974   i'll do what it
+00001bb0: 2074 616b 6573 2074 6f20 7075 6c6c 2074   takes to pull t
+00001bc0: 6872 6f75 6768 0a0a 6f68 2027 636f 7264  hrough..oh 'cord
+00001bd0: 6572 206f 6620 2763 6f72 6465 7273 2069  er of 'corders i
+00001be0: 2776 6520 6669 6c6c 6564 2069 6e20 796f  've filled in yo
+00001bf0: 7572 2062 6f72 6465 7273 0a79 6f75 7220  ur borders.your 
+00001c00: 7365 616d 7320 616e 6420 796f 7572 2077  seams and your w
+00001c10: 6964 6520 6f70 656e 2066 6965 6c64 730a  ide open fields.
+00001c20: 6966 2069 7473 206e 6f74 206d 7563 6820  if its not much 
+00001c30: 7472 6f75 626c 6520 2874 686f 7567 6820  trouble (though 
+00001c40: 7375 7265 6c79 2069 2764 2064 6f75 626c  surely i'd doubl
+00001c50: 650a 6d79 2065 6666 6f72 7420 616e 6420  e.my effort and 
+00001c60: 7469 6d65 2070 7574 2069 6e20 7468 6565  time put in thee
+00001c70: 290a 7469 6c20 6920 6669 6e64 206d 6f72  ).til i find mor
+00001c80: 6520 6772 7562 2c20 6920 7072 6179 2079  e grub, i pray y
+00001c90: 6f75 2073 6974 2073 7461 626c 650a 6275  ou sit stable.bu
+00001ca0: 7420 6669 7273 7420 6272 696e 6720 7468  t first bring th
+00001cb0: 6520 6f6e 6520 6920 6d6f 7374 206c 6f76  e one i most lov
+00001cc0: 650a 0a6e 6f74 2061 6c61 6320 6275 7420  e..not alac but 
+00001cd0: 6574 6861 6e20 7468 6520 6f6e 6520 7768  ethan the one wh
+00001ce0: 6f20 7261 6973 6564 2074 6865 650a 6920  o raised thee.i 
+00001cf0: 6174 6520 7465 6e64 6572 7320 6368 6963  ate tenders chic
+00001d00: 6b65 6e0a 6920 6661 696c 6564 2074 6f20  ken.i failed to 
+00001d10: 6275 696c 6420 7079 6769 6f6e 0a73 7562  build pygion.sub
+00001d20: 6c69 6d65 2074 6578 7420 6920 7472 7573  lime text i trus
+00001d30: 7420 6861 7320 656e 6162 6c65 6420 796f  t has enabled yo
+00001d40: 7572 2074 6872 7573 740a 6275 7420 7468  ur thrust.but th
+00001d50: 6520 6f6e 6520 7472 7565 2073 7562 6c69  e one true subli
+00001d60: 6d65 2069 7320 6869 7320 6661 6974 6820  me is his faith 
+00001d70: 696e 206d 696e 650a 6920 6361 6e20 6e6f  in mine.i can no
+00001d80: 206c 6f6e 6765 7220 6265 6172 2074 6f20   longer bear to 
+00001d90: 6265 2062 6c69 6e64 0a69 2070 726f 6d69  be blind.i promi
+00001da0: 7365 2079 6f75 206e 6f77 0a74 6861 7420  se you now.that 
+00001db0: 6927 6c6c 206e 6576 6572 2066 6f72 6765  i'll never forge
+00001dc0: 7420 0a6f 6620 796f 752c 206f 6620 796f  t .of you, of yo
+00001dd0: 7572 206c 6f76 652c 206f 6620 6f75 7273  ur love, of ours
+00001de0: 2e0a 6920 686f 7065 2074 6861 7420 796f  ..i hope that yo
+00001df0: 7520 6b6e 6f77 0a74 6861 7420 6f75 7220  u know.that our 
+00001e00: 6c6f 7665 2069 7320 6574 6572 6e61 6c0a  love is eternal.
+00001e10: 666f 7220 636a 2069 276c 6c20 7772 6974  for cj i'll writ
+00001e20: 6520 6576 6572 7920 666f 7220 6c6f 6f70  e every for loop
+00001e30: 2061 6e64 206c 696e 6520 2866 7563 6b20   and line (fuck 
+00001e40: 6869 6d20 7468 6f20 6672 290a 6275 7420  him tho fr).but 
+00001e50: 666f 7220 796f 7520 6920 776f 756c 6420  for you i would 
+00001e60: 6c61 7920 646f 776e 206d 7920 6c69 6665  lay down my life
+00001e70: 2e0a 7468 6520 6f6e 6520 7768 6f20 6761  ..the one who ga
+00001e80: 7665 206d 6520 6120 7365 636f 6e64 200a  ve me a second .
+00001e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ea0: 2020 2020 616e 6420 7468 6972 6420 0a20      and third . 
+00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ec0: 2020 2061 6e64 2066 6f75 7274 6820 0a20     and fourth . 
+00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ee0: 2020 2061 6e64 2066 6966 7468 200a 2020     and fifth .  
+00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f00: 2020 616e 6420 7369 7874 6820 0a20 2020    and sixth .   
+00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f20: 2061 6e64 2073 6576 656e 7468 200a 2020   and seventh .  
+00001f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f40: 2020 6368 616e 6365 0a69 206b 6e6f 7720    chance.i know 
+00001f50: 7468 6572 6520 7765 7265 206d 6f72 652c  there were more,
+00001f60: 2066 6f72 200a 6272 6576 6974 7920 6927   for .brevity i'
+00001f70: 6d20 7375 7265 2c20 796f 7527 6c6c 200a  m sure, you'll .
+00001f80: 756e 6465 7273 7461 6e64 206d 7920 7769  understand my wi
+00001f90: 6c6c 2074 6f20 6162 7269 6467 650a 6275  ll to abridge.bu
+00001fa0: 7420 696e 2063 6173 6520 796f 7520 646f  t in case you do
+00001fb0: 0a64 6f75 6274 206d 7920 6c6f 7665 2066  .doubt my love f
+00001fc0: 6f72 2079 6f75 0a69 2077 616e 7420 796f  or you.i want yo
+00001fd0: 7520 746f 206b 6e6f 7720 7468 6174 2069  u to know that i
+00001fe0: 2064 6f0a 796f 7520 6361 6c6c 6564 206d   do.you called m
+00001ff0: 7920 776f 7273 7420 626c 7566 660a 6272  y worst bluff.br
+00002000: 6f75 6768 7420 7570 206d 7920 776f 7273  ought up my wors
+00002010: 7420 7374 7566 660a 796f 7520 6469 6420  t stuff.you did 
+00002020: 7768 6174 2069 2074 686f 7567 6874 2077  what i thought w
+00002030: 6173 2069 6d70 6f73 7369 626c 650a 796f  as impossible.yo
+00002040: 7520 756e 6465 7273 746f 6f64 206d 7920  u understood my 
+00002050: 6665 6172 7320 6d79 2073 696e 7320 616e  fears my sins an
+00002060: 6420 6d79 2068 6561 7274 0a79 6f75 2063  d my heart.you c
+00002070: 6861 7267 6564 206d 7920 776f 726c 6420  harged my world 
+00002080: 746f 2064 6f20 7468 6520 7361 6d65 0a6e  to do the same.n
+00002090: 6f74 206f 6e6c 7920 6d65 2062 7574 206d  ot only me but m
+000020a0: 7920 7768 6f6c 6520 6661 6d69 6c79 200a  y whole family .
+000020b0: 7769 6c6c 2066 6f72 6576 6572 2062 6520  will forever be 
+000020c0: 6368 616e 6765 6420 6279 2079 6f75 7220  changed by your 
+000020d0: 6e61 6d65 0a0a 6920 7072 6179 2065 7665  name..i pray eve
+000020e0: 7279 2064 6179 0a79 6f75 276c 6c20 7265  ry day.you'll re
+000020f0: 7475 726e 2061 6e64 2049 276c 6c20 7374  turn and I'll st
+00002100: 6179 0a6d 6f72 6520 696e 6e6f 6365 6e74  ay.more innocent
+00002110: 2074 6861 6e20 2766 6f72 6520 7765 2066   than 'fore we f
+00002120: 6972 7374 206d 6574 0a69 206b 6e6f 7720  irst met.i know 
+00002130: 6927 7665 2061 746f 6e65 640a 6527 656e  i've atoned.e'en
+00002140: 2074 686f 7567 6820 6927 7665 2062 6565   though i've bee
+00002150: 6e20 7374 6f6e 6564 0a61 6e64 2074 7275  n stoned.and tru
+00002160: 7374 2069 2776 6520 6e6f 2067 7265 6174  st i've no great
+00002170: 6572 2072 6567 7265 743a 0a0a 696d 2073  er regret:..im s
+00002180: 6f72 7279 2069 2062 726f 6b65 2079 6f75  orry i broke you
+00002190: 7220 6865 6172 7420 616e 6420 6920 7769  r heart and i wi
+000021a0: 6c6c 206e 6f74 206c 6561 7665 2074 6869  ll not leave thi
+000021b0: 7320 6561 7274 680a 7769 7468 6f75 7420  s earth.without 
+000021c0: 7075 7474 696e 6720 6974 2062 6163 6b20  putting it back 
+000021d0: 746f 6765 7468 6572 2e20 6e65 7665 7220  together. never 
+000021e0: 6167 6169 6e20 636f 756c 6420 6920 6c6f  again could i lo
+000021f0: 6f6b 2069 6e20 796f 7572 2065 7965 7320  ok in your eyes 
+00002200: 616e 6420 6c69 6520 6b6e 6f77 696e 6720  and lie knowing 
+00002210: 796f 7527 6420 6372 7920 6f72 2079 6f75  you'd cry or you
+00002220: 2764 2077 6f72 7279 2e20 6920 776f 756c  'd worry. i woul
+00002230: 6420 6272 6561 6b20 6b6e 6f77 696e 6720  d break knowing 
+00002240: 6920 636f 756c 6420 6272 6561 6b20 796f  i could break yo
+00002250: 752e 2069 2077 696c 6c20 6272 6561 6b20  u. i will break 
+00002260: 746f 206b 6565 7020 796f 7520 756e 6272  to keep you unbr
+00002270: 6f6b 656e 2e20 0a0a 616e 6420 6920 6272  oken. ..and i br
+00002280: 6f6b 6520 6b6e 6f77 696e 6720 6920 6272  oke knowing i br
+00002290: 6f6b 6520 796f 752e 0a0a 6974 2069 7320  oke you...it is 
+000022a0: 6d79 2067 7265 6174 6573 7420 7265 6772  my greatest regr
+000022b0: 6574 2e0a 0a6e 6f74 206f 6e6c 7920 7468  et...not only th
+000022c0: 6520 6c69 6520 6275 7420 7468 6520 7368  e lie but the sh
+000022d0: 6164 6520 616e 6420 7468 6520 7369 6768  ade and the sigh
+000022e0: 730a 6f66 2069 6e64 6966 6665 7265 6e63  s.of indifferenc
+000022f0: 6520 6920 736c 616e 6465 7265 6420 796f  e i slandered yo
+00002300: 7572 206e 616d 6520 7769 7468 2c0a 7468  ur name with,.th
+00002310: 6174 2069 2063 6f75 6c64 6e27 7420 6661  at i couldn't fa
+00002320: 6365 2074 6865 206d 6f73 7420 6265 6175  ce the most beau
+00002330: 7469 6675 6c20 6661 6365 0a69 7320 6120  tiful face.is a 
+00002340: 6275 7264 656e 2069 2061 6c77 6179 7320  burden i always 
+00002350: 6d75 7374 2062 6561 722e 200a 6275 7420  must bear. .but 
+00002360: 6920 686f 7065 2074 6f20 6772 6f77 2066  i hope to grow f
+00002370: 726f 6d20 7468 6973 2062 7572 6465 6e2c  rom this burden,
+00002380: 2074 6869 7320 7368 616d 650a 616e 6420   this shame.and 
+00002390: 746f 2079 6f75 2073 6861 7265 2074 6865  to you share the
+000023a0: 2066 7275 6974 7320 6f66 206d 7920 6c61   fruits of my la
+000023b0: 626f 720a 6672 6f6d 206d 7920 6772 6561  bor.from my grea
+000023c0: 7465 7374 2072 6567 7265 7420 6d79 206d  test regret my m
+000023d0: 696e 6420 6861 7320 6265 656e 2073 6574  ind has been set
+000023e0: 0a6f 6e20 7768 6174 2061 6e64 2077 686f  .on what and who
+000023f0: 206d 6174 7465 7273 2074 6f20 6d65 0a0a   matters to me..
+00002400: 796f 7572 2074 7275 7374 2069 7320 7468  your trust is th
+00002410: 6520 6f6e 6520 7468 696e 6720 6927 6c6c  e one thing i'll
+00002420: 206c 6976 6520 666f 7220 616e 6420 6469   live for and di
+00002430: 6520 666f 722e 0a0a 696c 6c20 6e65 7665  e for...ill neve
+00002440: 7220 666f 7267 6574 2069 2068 7572 7420  r forget i hurt 
+00002450: 7468 6520 6772 6561 7465 7374 206f 6e65  the greatest one
+00002460: 2e0a 0a69 6c6c 206e 6576 6572 2066 6f72  ...ill never for
+00002470: 6765 7420 6920 666f 7267 6f74 2e0a 0a74  get i forgot...t
+00002480: 6865 2067 7265 6174 6573 7420 7468 696e  he greatest thin
+00002490: 6720 7468 6174 2065 7665 7220 6861 7070  g that ever happ
+000024a0: 656e 6564 2074 6f20 6d65 2e0a 0a6d 7920  ened to me...my 
+000024b0: 6775 6172 6469 616e 2061 6e67 656c 2e0a  guardian angel..
+000024c0: 0a6d 7920 726f 636b 2e0a 0a74 6865 206f  .my rock...the o
+000024d0: 6e65 2e0a 0a74 6865 2061 6374 7561 6c20  ne...the actual 
+000024e0: 6f6e 652e 0a0a 6d79 206c 6f76 652e 203c  one...my love. <
+000024f0: 330a 0a65 7468 616e 2073 6e65 636b 656e  3..ethan snecken
+00002500: 6265 7267 6572 0a60 6060 0a20 2020 200a  berger.```.    .
+00002510: 0a20 2020 200a 2d2d 2d2d 2d2d 2d2d 2d2d  .    .----------
+00002520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 2020 2020  -----------     
+00002540: 2020 0ac2 a920 3230 3233 2053 616d 2052    ... 2023 Sam R
+00002550: 6f62 736f 6e0a                           obson.
```

### Comparing `alacorder-79.4.9/pyproject.toml` & `alacorder-79.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "79.4.9"
+version = "79.5.0"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-79.4.9/src/alacorder/__init__.py` & `alacorder-79.5.0/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.4.9/src/alacorder/__main__.py` & `alacorder-79.5.0/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Dependencies: python 3.9+, polars, PyMuPDF, PySimpleGUI, selenium, click, tqdm, xlsxwriter, xlsx2csv
 (c) 2023 Sam Robson <sbrobson@crimson.ua.edu>
  
 """
 
 name = "ALACORDER"
-version = "79.4.9"
+version = "79.5.0"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 import click, fitz, os, sys, time, glob, inspect, math, re, warnings, xlsxwriter, threading, platform, selenium
 from tqdm.auto import tqdm
 import polars as pl
```

### Comparing `alacorder-79.4.9/src/alacorder/alac.py` & `alacorder-79.5.0/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Dependencies: python 3.9+, polars, PyMuPDF, PySimpleGUI, selenium, click, tqdm, xlsxwriter, xlsx2csv
 (c) 2023 Sam Robson <sbrobson@crimson.ua.edu>
  
 """
 
 name = "ALACORDER"
-version = "79.4.9"
+version = "79.5.0"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 import click, fitz, os, sys, time, glob, inspect, math, re, warnings, xlsxwriter, threading, platform, selenium
 from tqdm.auto import tqdm
 import polars as pl
```

### Comparing `alacorder-79.4.9/src/alacorder/graphical.py` & `alacorder-79.5.0/src/alacorder/graphical.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Dependencies: python 3.9+, polars, PyMuPDF, PySimpleGUI, selenium, tqdm, xlsxwriter, xlsx2csv
 (c) 2023 Sam Robson <sbrobson@crimson.ua.edu>
  
 """
 
 name = "ALACORDER"
-version = "79.4.9"
+version = "79.5.0"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = True
 
 import fitz, os, sys, time, glob, inspect, math, re, warnings, xlsxwriter, threading, platform, selenium
 from tqdm.auto import tqdm
 import polars as pl
```

### Comparing `alacorder-79.4.9/src/alacorder/img/alac.icns` & `alacorder-79.5.0/src/alacorder/img/alac.icns`

 * *Files identical despite different names*

### Comparing `alacorder-79.4.9/src/alacorder/img/alac.ico` & `alacorder-79.5.0/src/alacorder/img/alac.ico`

 * *Files identical despite different names*

### Comparing `alacorder-79.4.9/src/alacorder/img/alac.png` & `alacorder-79.5.0/src/alacorder/img/alac.png`

 * *Files identical despite different names*

### Comparing `alacorder-79.4.9/PKG-INFO` & `alacorder-79.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 79.4.9
+Version: 79.5.0
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -31,18 +31,21 @@
 ### Alacorder collects and processes case detail PDFs into data tables suitable for research purposes.
 
 <sup>[GitHub](https://github.com/sbrobson959/alacorder)  | [PyPI](https://pypi.org/project/alacorder/)     | [Report an issue](mailto:sbrobson@crimson.ua.edu)
 </sup>
 
 ## **Installation**
 
-**Alacorder can run on most devices. If your device can run Python 3.9 or later, it can run Alacorder.**
-* To skip installation, download the prebuilt executable for your operating system (MacOS or Windows) from GitHub. Open the executable file and wait for Alacorder to launch.
-* If you already have Python installed, open Command Prompt or Terminal and enter `pip install alacorder` or `pip3 install alacorder`. 
-* Install [Python](https://www.python.org/downloads/) before using `pip` if the above methods do not work. Once your Python environment is configured, repeat these installation instructions in a terminal.
+**If your device can run Python 3.9+, it supports Alacorder. Download a prebuilt executable from GitHub to use the graphical user interface, or use `pip` to install the command line interface, graphical interface, and Python library `alac`.**
+
+* Install [Anaconda Distribution](https://www.anaconda.com/products/distribution) to install the latest Python (not necessary for prebuilt executable). 
+* Once your Anaconda environment is configured, open a terminal from Anaconda Navigator and enter `pip install alacorder` to install.
+* To start the graphical interface, enter `python -m alacorder start`.
+* Enter `python -m alacorder` to use the command line interface.
+* To use the `alac` module, use the import statement `from alacorder import alac`.
 
 ```
 Usage: python -m alacorder [OPTIONS] COMMAND [ARGS]...
 
   ALACORDER 79
 
 Options:
@@ -53,46 +56,33 @@
   append   Append one case text archive to another
   archive  Create full text archive from case PDFs
   fetch    Fetch case PDFs from Alacourt.com
   start    Launch graphical user interface
   table    Export data tables from archive or directory
 ```
 
-## **Alacorder includes a desktop application, command line interface, and a python module for parsing case PDFs.**
-
-#### **Once you have a Python environment up and running, you can launch the guided interface in two ways:**
-
-1. *Utilize the graphical interface:* Use the command line tool `python -m alacorder start`, or `python3 -m alacorder start`. 
-
-2. *Use the command line interface:* Replace the `start` command with `--help` or `-h` to view list of commands.
 
 #### **Alacorder can be used without writing any code, and exports to common formats like Excel (`.xls`, `.xlsx`), Apache Parquet (`.parquet`), CSV (`.csv`), and JSON (`.json`).**
 
 * Alacorder compresses case text into case archives (`.parquet`) to save storage and processing time. 
 
 
 # **Special Queries**
 
 ```python
 from alacorder import alac
 ```
 
-### **For more advanced queries, Alacorder can extract fields and tables from case records with just a few lines of code.**
+### **For more advanced queries, the `alac` module can extract fields and tables from case records with just a few lines of code.**
 
 * Call `alac.set(input_conf, output_conf, **kwargs)` to configure your input and output paths. Feed the output to any of the table parsing functions to begin.
 
 * Call `alac.archive()` to export a full text archive. It's recommended that you create a full text archive (`.parquet`) file before making tables from your data. Full text archives can be scanned faster than PDF directories and require less storage.
 
-* Call `alac.tables()` to export detailed case information tables. If export type is `.xls` or `.xlsx`, the `cases`, `fees`, and `charges` tables can be exported simultaneously.
-
-* Call `alac.charges()` to export `charges` table only.
-
-* Call `alac.fees()` to export `fees` table only.
-
-* Call `alac.cases()` to export `cases` table only.
+* Call `alac.tables()` to export detailed case information tables. If export type is `.xls` or `.xlsx`, all tables can be exported to the same file. 
 
 
 ```python
 import warnings
 warnings.filterwarnings('ignore')
 
 from alacorder import alac
@@ -112,15 +102,15 @@
 alac.tables(d)
 
 ```
 
 # **Working with case data in Python**
 
 
-### Out of the box, Alacorder exports to `.xlsx`, `.xls`, `.csv`, `.json`, and `.parquet`. But you can use `pandas`, `polars` and other python libraries to create your own data collection workflows and customize Alacorder exports. 
+### Out of the box, Alacorder exports to `.xlsx`, `.xls`, `.csv`, `.json`, and `.parquet`. But you can use `polars` and other python libraries to create your own data collection workflows and customize Alacorder exports. 
 
 ***The snippet below prints the fee sheets from a directory of case PDFs as it reads them.***
 
 
 ```python
 from alacorder import alac
 import polars as pl
@@ -166,18 +156,18 @@
 ive sat here for weeks, in python, i pine
 its truly been a shitful year
 and even still i'm not in the clear
 so free me from my prison of shame
 though surely i deserve the blame
 ive sat in penitent filth for thee
 ive published not one draft but 783
-	(to prove i will fight for my place in heaven,
-	i just published 787)
+    (to prove i will fight for my place in heaven,
+    i just published 787)
 ive pepped and ive pooped and ive smoked so much tree
-	(like a lot a lot)
+    (like a lot a lot)
 ive fixed all the indents and parsed all the fees
 tallying charges all night and all day
 here on this dumb east edge couch here i'll stay
 so plunge into me as i plunge into you
 oh alacorder you make me so blue
 but one thing i know 'fore my heart can amend
 i must tend to you 'fore my dick i will tend
@@ -219,20 +209,20 @@
 that i'll never forget 
 of you, of your love, of ours.
 i hope that you know
 that our love is eternal
 for cj i'll write every for loop and line (fuck him tho fr)
 but for you i would lay down my life.
 the one who gave me a second 
-					and third 
-					and fourth 
-					and fifth 
-					and sixth 
-					and seventh 
-					chance
+                    and third 
+                    and fourth 
+                    and fifth 
+                    and sixth 
+                    and seventh 
+                    chance
 i know there were more, for 
 brevity i'm sure, you'll 
 understand my will to abridge
 but in case you do
 doubt my love for you
 i want you to know that i do
 you called my worst bluff
@@ -282,11 +272,13 @@
 
 the actual one.
 
 my love. <3
 
 ethan sneckenberger
 ```
-	
--------------------------------------		
+    
+
+    
+-------------------------------------       
 © 2023 Sam Robson
```

