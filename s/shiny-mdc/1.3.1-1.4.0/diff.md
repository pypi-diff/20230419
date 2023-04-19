# Comparing `tmp/shiny_mdc-1.3.1.tar.gz` & `tmp/shiny_mdc-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiny_mdc-1.3.1.tar", max compression
+gzip compressed data, was "shiny_mdc-1.4.0.tar", max compression
```

## Comparing `shiny_mdc-1.3.1.tar` & `shiny_mdc-1.4.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     2895 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/LICENSE
--rw-r--r--   0        0        0       78 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/README.md
--rw-r--r--   0        0        0     2297 2023-04-18 08:26:05.426183 shiny_mdc-1.3.1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/__init__.py
--rw-r--r--   0        0        0     1061 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/_latexmk.py
--rw-r--r--   0        0        0     1867 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/_liquid.py
--rw-r--r--   0        0        0     4643 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/_pandoc.py
--rw-r--r--   0        0        0     4936 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/_templates.py
--rw-r--r--   0        0        0       64 2023-04-18 08:26:05.430183 shiny_mdc-1.3.1/shinymdc/_version.py
--rw-r--r--   0        0        0      337 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/dynamic/addappendices.tex
--rw-r--r--   0        0        0      853 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/dynamic/authsetup.tex
--rw-r--r--   0        0        0      290 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/dynamic/authsetupshort.tex
--rw-r--r--   0        0        0      572 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/dynamic/dblfloatsetup.tex
--rw-r--r--   0        0        0      426 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/static/bibnonatsetup.tex
--rw-r--r--   0        0        0     2503 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/static/bibsupersetup.tex
--rw-r--r--   0        0        0     3359 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/static/floatsetup.tex
--rw-r--r--   0        0        0    19901 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/static/iccv/bibstyle.bst
--rw-r--r--   0        0        0     9433 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/static/iccv/esopic.sty
--rw-r--r--   0        0        0     3869 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/iccv/everyshi.sty
--rw-r--r--   0        0        0     8276 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/iccv/iccv.sty
--rw-r--r--   0        0        0    26973 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/iclr/bibstyle.bst
--rw-r--r--   0        0        0     9153 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/iclr/iclr.sty
--rw-r--r--   0        0        0    12284 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/iclr/mathcommands.tex
--rw-r--r--   0        0        0    27146 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/icml/bibstyle.bst
--rw-r--r--   0        0        0    27887 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/icml/icml.sty
--rw-r--r--   0        0        0      735 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/mathsetup.tex
--rw-r--r--   0        0        0      848 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/miscsetup.tex
--rw-r--r--   0        0        0    11306 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/neurips/neurips.sty
--rw-r--r--   0        0        0      406 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/reqsetup.tex
--rw-r--r--   0        0        0    19149 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/shinymdc.py
--rw-r--r--   0        0        0      935 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/basic.tex
--rw-r--r--   0        0        0     1302 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/iccv.tex
--rw-r--r--   0        0        0     1397 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/iclr.tex
--rw-r--r--   0        0        0     2144 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/icml.tex
--rw-r--r--   0        0        0      890 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/neurips.tex
--rw-r--r--   0        0        0     2057 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/spacious.tex
--rw-r--r--   0        0        0      469 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/standalone.tex
--rw-r--r--   0        0        0     2255 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/stylish.tex
--rw-r--r--   0        0        0    15953 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/figures/anscombe.pdf
--rw-r--r--   0        0        0    40892 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/figures/densities.pdf
--rw-r--r--   0        0        0    10736 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/figures/diamonds.pdf
--rw-r--r--   0        0        0   197017 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/figures/gaussian2d.pdf
--rw-r--r--   0        0        0    28282 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/figures/lines.png
--rw-r--r--   0        0        0     2972 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/main.md
--rwxr-xr-x   0        0        0      315 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/make.sh
--rw-r--r--   0        0        0     1166 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/references.bib
--rw-r--r--   0        0        0   682300 2023-04-18 08:25:42.709568 shiny_mdc-1.3.1/test/samples/basic.pdf
--rw-r--r--   0        0        0   412224 2023-04-18 08:25:42.713568 shiny_mdc-1.3.1/test/samples/iccv.pdf
--rw-r--r--   0        0        0   405928 2023-04-18 08:25:42.713568 shiny_mdc-1.3.1/test/samples/iclr.pdf
--rw-r--r--   0        0        0   445680 2023-04-18 08:25:42.717568 shiny_mdc-1.3.1/test/samples/icml.pdf
--rw-r--r--   0        0        0   450203 2023-04-18 08:25:42.717568 shiny_mdc-1.3.1/test/samples/neurips.pdf
--rw-r--r--   0        0        0   600967 2023-04-18 08:25:42.721568 shiny_mdc-1.3.1/test/samples/spacious.pdf
--rw-r--r--   0        0        0   551977 2023-04-18 08:25:42.721568 shiny_mdc-1.3.1/test/samples/standalone.pdf
--rw-r--r--   0        0        0   423226 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/samples/stylish.pdf
--rw-r--r--   0        0        0     1535 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/sections/appendix1.md
--rw-r--r--   0        0        0     1625 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/sections/appendix2.md
--rw-r--r--   0        0        0        0 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/sections/empty.md
--rw-r--r--   0        0        0     1837 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/sections/main1.md
--rw-r--r--   0        0        0     1353 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/sections/main2.md
--rw-r--r--   0        0        0      992 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/utils/commands.md
--rw-r--r--   0        0        0       41 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/utils/ext.md
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 shiny_mdc-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3330 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/LICENSE
+-rw-r--r--   0        0        0       78 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/README.md
+-rw-r--r--   0        0        0     2297 2023-04-19 06:08:04.539123 shiny_mdc-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/__init__.py
+-rw-r--r--   0        0        0     1061 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/_latexmk.py
+-rw-r--r--   0        0        0     1867 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/_liquid.py
+-rw-r--r--   0        0        0     4643 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/_pandoc.py
+-rw-r--r--   0        0        0     4936 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/_templates.py
+-rw-r--r--   0        0        0       64 2023-04-19 06:08:04.539123 shiny_mdc-1.4.0/shinymdc/_version.py
+-rw-r--r--   0        0        0      337 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/dynamic/addappendices.tex
+-rw-r--r--   0        0        0      853 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/dynamic/authsetup.tex
+-rw-r--r--   0        0        0      290 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/dynamic/authsetupshort.tex
+-rw-r--r--   0        0        0      572 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/dynamic/dblfloatsetup.tex
+-rw-r--r--   0        0        0      482 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/static/bibnonatsetup.tex
+-rw-r--r--   0        0        0     2602 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/static/bibsupersetup.tex
+-rw-r--r--   0        0        0     3359 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/static/floatsetup.tex
+-rw-r--r--   0        0        0    19901 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/static/iccv/bibstyle.bst
+-rw-r--r--   0        0        0     9433 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/iccv/esopic.sty
+-rw-r--r--   0        0        0     3869 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/iccv/everyshi.sty
+-rw-r--r--   0        0        0     8276 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/iccv/iccv.sty
+-rw-r--r--   0        0        0    26973 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/iclr/bibstyle.bst
+-rw-r--r--   0        0        0     9153 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/iclr/iclr.sty
+-rw-r--r--   0        0        0    12284 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/iclr/mathcommands.tex
+-rw-r--r--   0        0        0    27146 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/icml/bibstyle.bst
+-rw-r--r--   0        0        0    27887 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/icml/icml.sty
+-rw-r--r--   0        0        0      735 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/mathsetup.tex
+-rw-r--r--   0        0        0      848 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/miscsetup.tex
+-rw-r--r--   0        0        0    11306 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/neurips/neurips.sty
+-rw-r--r--   0        0        0      406 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/reqsetup.tex
+-rw-r--r--   0        0        0    19149 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/shinymdc.py
+-rw-r--r--   0        0        0      935 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/basic.tex
+-rw-r--r--   0        0        0     1302 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/iccv.tex
+-rw-r--r--   0        0        0     1397 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/iclr.tex
+-rw-r--r--   0        0        0     2144 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/icml.tex
+-rw-r--r--   0        0        0      890 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/neurips.tex
+-rw-r--r--   0        0        0     2057 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/spacious.tex
+-rw-r--r--   0        0        0      469 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/standalone.tex
+-rw-r--r--   0        0        0     2286 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/stylish.tex
+-rw-r--r--   0        0        0    15953 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/test/figures/anscombe.pdf
+-rw-r--r--   0        0        0    40892 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/test/figures/densities.pdf
+-rw-r--r--   0        0        0    10736 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/test/figures/diamonds.pdf
+-rw-r--r--   0        0        0   197017 2023-04-19 06:07:37.185623 shiny_mdc-1.4.0/test/figures/gaussian2d.pdf
+-rw-r--r--   0        0        0    28282 2023-04-19 06:07:37.185623 shiny_mdc-1.4.0/test/figures/lines.png
+-rw-r--r--   0        0        0     2972 2023-04-19 06:07:37.185623 shiny_mdc-1.4.0/test/main.md
+-rwxr-xr-x   0        0        0      315 2023-04-19 06:07:37.185623 shiny_mdc-1.4.0/test/make.sh
+-rw-r--r--   0        0        0     1166 2023-04-19 06:07:37.185623 shiny_mdc-1.4.0/test/references.bib
+-rw-r--r--   0        0        0   683424 2023-04-19 06:07:37.185623 shiny_mdc-1.4.0/test/samples/basic.pdf
+-rw-r--r--   0        0        0   412896 2023-04-19 06:07:37.189623 shiny_mdc-1.4.0/test/samples/iccv.pdf
+-rw-r--r--   0        0        0   406337 2023-04-19 06:07:37.189623 shiny_mdc-1.4.0/test/samples/iclr.pdf
+-rw-r--r--   0        0        0   446430 2023-04-19 06:07:37.193623 shiny_mdc-1.4.0/test/samples/icml.pdf
+-rw-r--r--   0        0        0   450734 2023-04-19 06:07:37.197623 shiny_mdc-1.4.0/test/samples/neurips.pdf
+-rw-r--r--   0        0        0   601766 2023-04-19 06:07:37.197623 shiny_mdc-1.4.0/test/samples/spacious.pdf
+-rw-r--r--   0        0        0   553251 2023-04-19 06:07:37.201624 shiny_mdc-1.4.0/test/samples/standalone.pdf
+-rw-r--r--   0        0        0   424279 2023-04-19 06:07:37.201624 shiny_mdc-1.4.0/test/samples/stylish.pdf
+-rw-r--r--   0        0        0     1535 2023-04-19 06:07:37.205624 shiny_mdc-1.4.0/test/sections/appendix1.md
+-rw-r--r--   0        0        0     1625 2023-04-19 06:07:37.205624 shiny_mdc-1.4.0/test/sections/appendix2.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:07:37.205624 shiny_mdc-1.4.0/test/sections/empty.md
+-rw-r--r--   0        0        0     2100 2023-04-19 06:07:37.205624 shiny_mdc-1.4.0/test/sections/main1.md
+-rw-r--r--   0        0        0     1353 2023-04-19 06:07:37.205624 shiny_mdc-1.4.0/test/sections/main2.md
+-rw-r--r--   0        0        0      992 2023-04-19 06:07:37.205624 shiny_mdc-1.4.0/test/utils/commands.md
+-rw-r--r--   0        0        0       41 2023-04-19 06:07:37.205624 shiny_mdc-1.4.0/test/utils/ext.md
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 shiny_mdc-1.4.0/PKG-INFO
```

### Comparing `shiny_mdc-1.3.1/CHANGELOG.md` & `shiny_mdc-1.4.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+## [1.4.0](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.3.1...v1.4.0) (2023-04-19)
+
+
+### Features
+
+* make small tables in stylish template opt-in ([24cdca5](https://github.com/jayanthkoushik/shiny-mdc/commit/24cdca56f336ee69b178a89420c3fe1560be3c94))
+
+
+### Bug Fixes
+
+* handle additional cases for citations with notes ([1fcce8d](https://github.com/jayanthkoushik/shiny-mdc/commit/1fcce8d9549ebfc0896b46eaadb38f8064f25ace))
+
 ### [1.3.1](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.3.0...v1.3.1) (2023-04-18)
 
 
 ### Bug Fixes
 
 * fix handling of notes in citations ([9a272a6](https://github.com/jayanthkoushik/shiny-mdc/commit/9a272a661971a25dc78703a2889dcadf00c429ed))
```

### Comparing `shiny_mdc-1.3.1/LICENSE` & `shiny_mdc-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/pyproject.toml` & `shiny_mdc-1.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shiny-mdc"
-version = "1.3.1"  # managed by `poetry-dynamic-versioning`
+version = "1.4.0"  # managed by `poetry-dynamic-versioning`
 description = "Tool to compile markdown files to tex/pdf using pandoc, latexmk"
 readme = "README.md"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 repository = "https://github.com/jayanthkoushik/shinymdc"
 packages = [
   { include = "shinymdc" }
```

### Comparing `shiny_mdc-1.3.1/shinymdc/_latexmk.py` & `shiny_mdc-1.4.0/shinymdc/_latexmk.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/_liquid.py` & `shiny_mdc-1.4.0/shinymdc/_liquid.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/_pandoc.py` & `shiny_mdc-1.4.0/shinymdc/_pandoc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/_templates.py` & `shiny_mdc-1.4.0/shinymdc/_templates.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/dynamic/authsetup.tex` & `shiny_mdc-1.4.0/shinymdc/resources/dynamic/authsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/dynamic/dblfloatsetup.tex` & `shiny_mdc-1.4.0/shinymdc/resources/dynamic/dblfloatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/static/bibsupersetup.tex` & `shiny_mdc-1.4.0/shinymdc/resources/static/bibsupersetup.tex`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 \newcommand*{\nolink}[1]{{\protect\NoHyper#1\protect\endNoHyper}}
 \let\origcitet\citet
 \renewcommand{\citet}[2][]{%
   % \nolink{\citeauthor{#2} (\citeyear{#2})}~\textsuperscript{\!\mbox{\oldcitep[#1]{#2}}}%
   \nolink{\citeauthor{#2} (\citeyear{#2})}~\citep[#1]{#2}%
 }
 
+\let\origcitetext\citetext
+\renewcommand{\citetext}[1]{%
+  \textsuperscript{\origcitetext{#1}}%
+}
+
 % \newtoggle{HasArgOne}
 % \newtoggle{HasArgTwo}
 % \LetLtxMacro\oldcitep\citep
 % \RenewDocumentCommand\citep{o o m}{%
 %   % First, check if the two optional arguments have values.
 %   % This involves checking for presence, as well as checking
 %   % if the value is blank.
```

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/static/floatsetup.tex` & `shiny_mdc-1.4.0/shinymdc/resources/static/floatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/static/iccv/bibstyle.bst` & `shiny_mdc-1.4.0/shinymdc/resources/static/iccv/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/static/iccv/esopic.sty` & `shiny_mdc-1.4.0/shinymdc/resources/static/iccv/esopic.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/static/iccv/everyshi.sty` & `shiny_mdc-1.4.0/shinymdc/resources/static/iccv/everyshi.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/static/iccv/iccv.sty` & `shiny_mdc-1.4.0/shinymdc/resources/static/iccv/iccv.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/static/iclr/bibstyle.bst` & `shiny_mdc-1.4.0/shinymdc/resources/static/iclr/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/static/iclr/iclr.sty` & `shiny_mdc-1.4.0/shinymdc/resources/static/iclr/iclr.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/static/iclr/mathcommands.tex` & `shiny_mdc-1.4.0/shinymdc/resources/static/iclr/mathcommands.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/static/icml/bibstyle.bst` & `shiny_mdc-1.4.0/shinymdc/resources/static/icml/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/static/icml/icml.sty` & `shiny_mdc-1.4.0/shinymdc/resources/static/icml/icml.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/static/mathsetup.tex` & `shiny_mdc-1.4.0/shinymdc/resources/static/mathsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/static/miscsetup.tex` & `shiny_mdc-1.4.0/shinymdc/resources/static/miscsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/resources/static/neurips/neurips.sty` & `shiny_mdc-1.4.0/shinymdc/resources/static/neurips/neurips.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/shinymdc.py` & `shiny_mdc-1.4.0/shinymdc/shinymdc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/templates/basic.tex` & `shiny_mdc-1.4.0/shinymdc/templates/basic.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/templates/iccv.tex` & `shiny_mdc-1.4.0/shinymdc/templates/iccv.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/templates/iclr.tex` & `shiny_mdc-1.4.0/shinymdc/templates/iclr.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/templates/icml.tex` & `shiny_mdc-1.4.0/shinymdc/templates/icml.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/templates/neurips.tex` & `shiny_mdc-1.4.0/shinymdc/templates/neurips.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/templates/spacious.tex` & `shiny_mdc-1.4.0/shinymdc/templates/spacious.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/shinymdc/templates/stylish.tex` & `shiny_mdc-1.4.0/shinymdc/templates/stylish.tex`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,19 @@
 \input{$reqsetup$}
 \input{$floatsetup$}
 \input{$dblfloatsetup$}
 \input{$mathsetup$}
 \input{$bibsupersetup$}
 \input{$miscsetup$}
 
+$if(smalltabs)$
 % Use small font for tables.
 \AtBeginEnvironment{tabular}{\smaller}
+$else$
+$endif$
 
 % Configure caption font.
 \captionsetup{justification=raggedright,font={sf,small}}
 
 % Add periods after section numbers.
 \titlelabel{\thetitle.\enskip}
```

### Comparing `shiny_mdc-1.3.1/test/figures/anscombe.pdf` & `shiny_mdc-1.4.0/test/figures/anscombe.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/test/figures/densities.pdf` & `shiny_mdc-1.4.0/test/figures/densities.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/test/figures/diamonds.pdf` & `shiny_mdc-1.4.0/test/figures/diamonds.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/test/figures/gaussian2d.pdf` & `shiny_mdc-1.4.0/test/figures/gaussian2d.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/test/figures/lines.png` & `shiny_mdc-1.4.0/test/figures/lines.png`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/test/main.md` & `shiny_mdc-1.4.0/test/main.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/test/references.bib` & `shiny_mdc-1.4.0/test/references.bib`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/test/samples/basic.pdf` & `shiny_mdc-1.4.0/test/samples/basic.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 7% similar despite different names*

#### pdftotext {} -

```diff
@@ -179,29 +179,33 @@
 • Pointer to footnote 1
 
 7
 
 Citations
 • Short citation [2]
 • Short citation with pre note [see 2]
-• Short citation with post note [2, p. 1]
-• Short citation with pre/post notes [see 2, p. 1]
+• Short citation with locator [2, p. 1]
+• Short citation with post note [2, for more]
+• Short citation with locators and pre/post notes [see 2, chap. 1-4, for more]
 • Long citation: Lesk and Kernighan (1977) [3]
-• Long citation with note: Lesk and Kernighan (1977) [3, p. 1]
+• Long citation with locator: Lesk and Kernighan (1977) [3, chap. 1]
+• Long citation with note: Lesk and Kernighan (1977) [3, for more]
 • Multi citation [2–4]
 • Multi citation with pre note [see 2–4]
-• Multi citation with post note [2–4, for more]
-• Multi citation with pre/post notes [see 2–4, for more]
 1 Example footnote text.
 
 3
 
 (2)
 
-8
+• Multi citation with locators [3, sec. 1; 4; 2, p. 1-3]
+• Multi citation with post note [2–4, for more]
+• Multi citation with locators and pre/post notes [see 3, p. 1; 4; 2, chap. 1-2, for more]
+
+8
 
 Tables
 • Table 1
 • Table 2
 Col1
 
 Col2
```

### Comparing `shiny_mdc-1.3.1/test/samples/iccv.pdf` & `shiny_mdc-1.4.0/test/samples/iccv.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -124,54 +124,60 @@
 rutrum in sapien et, condimentum lacinia nibh.
 
 2. Typography
 • Bold
 • Italic
 • Bold italic.
 
-6. Links
+3. Numbers
+• Normal: 0123456789
+• Math: 0123456789
+
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
 • Pointer to footnote ¹
 
 7. Citations
 • Short citation [4]
 • Short citation with pre note [4]
-• Short citation with post note [4, p. 1]
-• Short citation with pre/post notes [4, p. 1]
+• Short citation with locator [4, p. 1]
+• Short citation with post note [4, for more]
+• Short citation with locators and pre/post notes [4,
+chap. 1-4, for more]
 • Long citation: [3]
-• Long citation with note: [3, p. 1]
+• Long citation with locator: [3, chap. 1]
+• Long citation with note: [3, for more]
 • Multi citation [3, 1, 4]
 • Multi citation with pre note [3, 1, 4]
+• Multi citation with locators ([3, sec. 1]; [1]; [4, p. 1-3])
 • Multi citation with post note [3, 1, 4, for more]
-• Multi citation with pre/post notes [3, 1, 4, for more]
+• Multi citation with locators and pre/post notes ([3, p. 1];
+[1]; [4, chap. 1-2, for more])
 
 8. Tables
 
-3. Numbers
-
-• Table 1
-• Table 2
-
-• Normal: 0123456789
-• Math: 0123456789
-
 4. Acronyms
 • Default (short+long): Carnegie Mellon University
 (CMU)
 • Repeated (short): CMU
 • Forced short: USA
 • Repeated after forced short (short+long): United States
 of America (USA)
 • Plural: social security numbers (SSNs)
 
 5. Math
+Z ∞
+
+6. Links
+
+• Table 1
+• Table 2
 
 Col1
 
 Col2
 
 Col3
 
@@ -190,43 +196,37 @@
 333
 
 4
 44
 444
 
 Table 1: Short table
+−x2
 
-9. Figures
-Z ∞
-
-2
-
-exp−x dx
+exp
 
-0
+dx
 
 (1)
 
-• Figure 2
-• Figure 3
-• Figure 4, Figure 4a, Figure 4b
+0
 
-a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
+9.2,Figures
+a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1,
+3, 4, 5, 6, 7, 8, 9
 (2)
-10. Includes
+• Figure 2
 R∞
 2
-• Commands from metadata include: arg min R
+• Figure 3
 • Inline: 0 exp−x dx
-• Include command in body (there should be text after
+• Figure 4, Figure 4a, Figure 4b
 • Block: Equation 1, Equation 2
-this):
 • Commands defined in body (P[x in X]): P[x ∈ X ]
 • Aligned:
-Content added through include statement.
 x=1
 x + y = 10
 x + y + z = 100
 
 ¹ Example footnote text.
 ² Footnote in sub-figure caption.
 ³ Footnote in figure caption.
@@ -377,14 +377,20 @@
 
 5
 
 6
 
 Table 2: Wide table
 
+10. Includes
+• Commands from metadata include: arg min R
+• Include command in body (there should be text after
+this):
+Content added through include statement.
+
 References
 [1] Donald E. Knuth. Literate programming. The Computer
 Journal, 27(2):97–111, 1984.
 [2] Donald E. Knuth. The TEX Book. Addison-Wesley Professional,
 1986.
 [3] Michael Lesk and Brian Kernighan. Computer typesetting
 of technical journals on UNIX. In Proceedings of American
```

### Comparing `shiny_mdc-1.3.1/test/samples/iclr.pdf` & `shiny_mdc-1.4.0/test/samples/iclr.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 5% similar despite different names*

#### pdftotext {} -

```diff
@@ -149,24 +149,23 @@
 0
 
 2
 
 (1)
 
 a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
-
-(2)
-
 R∞
 2
 • Inline: 0 exp−x dx
 • Block: Equation 1, Equation 2
 • Commands defined in body (P[x in X]): P[x ∈ X ]
 • Aligned:
 
+(2)
+
 x=1
 x + y = 10
 x + y + z = 100
 
 6
 
 Links
@@ -178,33 +177,49 @@
 • Pointer to footnote ¹
 
 7
 
 Citations
 • Short citation (Mittelbach et al., 2004)
 • Short citation with pre note (see Mittelbach et al., 2004)
-• Short citation with post note (Mittelbach et al., 2004, p. 1)
-• Short citation with pre/post notes (see Mittelbach et al., 2004, p. 1)
+• Short citation with locator (Mittelbach et al., 2004, p. 1)
+• Short citation with post note (Mittelbach et al., 2004, for more)
+• Short citation with locators and pre/post notes (see Mittelbach et al., 2004, chap. 1-4, for
+more)
 • Long citation: Lesk & Kernighan (1977)
-• Long citation with note: Lesk & Kernighan (1977, p. 1)
+• Long citation with locator: Lesk & Kernighan (1977, chap. 1)
+• Long citation with note: Lesk & Kernighan (1977, for more)
 • Multi citation (Lesk & Kernighan, 1977; Knuth, 1984; Mittelbach et al., 2004)
 • Multi citation with pre note (see Lesk & Kernighan, 1977; Knuth, 1984; Mittelbach et al.,
 2004)
+• Multi citation with locators (Lesk & Kernighan, 1977, sec. 1; Knuth, 1984; Mittelbach et al.,
+2004, p. 1-3)
 • Multi citation with post note (Lesk & Kernighan, 1977; Knuth, 1984; Mittelbach et al., 2004,
 for more)
-• Multi citation with pre/post notes (see Lesk & Kernighan, 1977; Knuth, 1984; Mittelbach
-et al., 2004, for more)
+• Multi citation with locators and pre/post notes (see Lesk & Kernighan, 1977, p. 1; Knuth,
+1984; Mittelbach et al., 2004, chap. 1-2, for more)
 
 8
 
 Tables
 • Table 1
 • Table 2
 
-Col1
+9
+
+Figures
+• Figure 2
+• Figure 3
+• Figure 4, Figure 4a, Figure 4b
+¹ Example footnote text.
+² Footnote in sub-figure caption.
+
+3
+
+Col1
 
 Col2
 
 Col3
 
 Col4
 
@@ -221,18 +236,15 @@
 333
 
 4
 44
 444
 
 Table 1: Short table
-
-3
-
-Col1
+Col1
 
 Col2
 
 Col3
 
 Col4
 
@@ -297,17 +309,35 @@
 
 5
 
 6
 
 Table 2: Wide table
 
+10
+
+Includes
+• Commands from metadata include: arg min R
+• Include command in body (there should be text after this):
+
+Content added through include statement.
+
+References
+Donald E. Knuth. Literate programming. The Computer Journal, 27(2):97–111, 1984.
+Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
+Michael Lesk and Brian Kernighan. Computer typesetting of technical journals on UNIX. In
+Proceedings of American Federation of Information Processing Societies: 1977 National Computer
+Conference, pp. 879–888, Dallas, Texas, 1977.
+
 Figure 2: Narrow figure
+³ Footnote in figure caption.
 
-A
+4
+
+A
 B
 C
 D
 E
 F
 G
 H
@@ -322,24 +352,26 @@
 
 68
 
 x
 
 70
 
-Figure 3: Wide figure
-
-4
-
 72
 
 74
 
 76
 
+Figure 3: Wide figure
+Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle, and Chris Rowley. The LATEX
+Companion. Addison-Wesley Professional, 2 edition, 2004.
+
+5
+
 (a) Figure with ‘width=2.5in’
 
 dataset = I
 
 dataset = II
 
 dataset = III
@@ -373,52 +405,22 @@
 
 5
 
 (b) Figure with ‘width=3.5in’ ²
 
 Figure 4: Sub-figures ³
 
-9
-
-Figures
-• Figure 2
-• Figure 3
-• Figure 4, Figure 4a, Figure 4b
-
-¹ Example footnote text.
-² Footnote in sub-figure caption.
-³ Footnote in figure caption.
-
-5
+6
 
 10
 
 x
 
 15
 
-10
-
-Includes
-• Commands from metadata include: arg min R
-• Include command in body (there should be text after this):
-
-Content added through include statement.
-
-References
-Donald E. Knuth. Literate programming. The Computer Journal, 27(2):97–111, 1984.
-Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
-Michael Lesk and Brian Kernighan. Computer typesetting of technical journals on UNIX. In
-Proceedings of American Federation of Information Processing Societies: 1977 National Computer
-Conference, pp. 879–888, Dallas, Texas, 1977.
-Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle, and Chris Rowley. The LATEX
-Companion. Addison-Wesley Professional, 2 edition, 2004.
-
-6
-
 A
 B
 C
 D
 E
 F
 G
```

### Comparing `shiny_mdc-1.3.1/test/samples/icml.pdf` & `shiny_mdc-1.4.0/test/samples/icml.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -127,111 +127,110 @@
 (C M U )
 • Repeated (short): C M U
 • Forced short: U S A
 • Repeated after forced short (short+long): United States
 of America ( U S A )
 • Plural: social security numbers ( S S N S )
 
+5. Math
+Z ∞
+
+2
+
+exp−x dx
+
+0
+
+(1)
+
 • Pointer to footnote 1
 
 7. Citations
 • Short citation (Mittelbach et al., 2004)
 • Short citation with pre note (see Mittelbach et al., 2004)
-• Short citation with post note (Mittelbach et al., 2004,
+• Short citation with locator (Mittelbach et al., 2004,
 p. 1)
-• Short citation with pre/post notes (see Mittelbach et al.,
-2004, p. 1)
+• Short citation with post note (Mittelbach et al., 2004,
+for more)
+• Short citation with locators and pre/post notes (see
+Mittelbach et al., 2004, chap. 1-4, for more)
 • Long citation: Lesk & Kernighan (1977)
-• Long citation with note: Lesk & Kernighan (1977, p. 1)
+• Long citation with locator: Lesk & Kernighan (1977,
+chap. 1)
+• Long citation with note: Lesk & Kernighan (1977, for
+more)
 • Multi citation (Lesk & Kernighan, 1977; Knuth, 1984;
 Mittelbach et al., 2004)
 • Multi citation with pre note (see Lesk & Kernighan,
 1977; Knuth, 1984; Mittelbach et al., 2004)
+• Multi citation with locators (Lesk & Kernighan, 1977,
+sec. 1; Knuth, 1984; Mittelbach et al., 2004, p. 1-3)
 • Multi citation with post note (Lesk & Kernighan, 1977;
 Knuth, 1984; Mittelbach et al., 2004, for more)
-• Multi citation with pre/post notes (see Lesk &
-Kernighan, 1977; Knuth, 1984; Mittelbach et al., 2004,
-for more)
+• Multi citation with locators and pre/post notes (see
+Lesk & Kernighan, 1977, p. 1; Knuth, 1984; Mittelbach
+et al., 2004, chap. 1-2, for more)
 
 8. Tables
 • Table 1
 • Table 2
 
-5. Math
-Z ∞
+a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
+(2)
+Col1 Col2
+1
+11
+111
 
+R∞
 2
+• Inline: 0 exp−x dx
+• Block: Equation 1, Equation 2
+• Commands defined in body (P[x in X]): P[x ∈ X ]
+• Aligned:
 
-exp−x dx
-
-(1)
-
-0
+x=1
+x + y = 10
+x + y + z = 100
 
-Col1
+6. Links
+• Section: Section 1, Section 1.2
+• Appendix section: Section B, Section A.1.1
+• Appendix figure: Figure A1
+• Appendix table: Table B1
+• Appendix math: Equation 4
 
-Col2
+2
+22
+222
 
 Col3
 
 Col4
 
-1
-11
-111
-
-2
-22
-222
-
 3
 33
 333
 
 4
 44
 444
 
-a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9Table 1. Short table
-(2)
-R∞
-2
-• Inline: 0 exp−x dx
-• Block: Equation 1, Equation 2
-• Commands defined in body (P[x in X]): P[x ∈ X ]
-• Aligned:
+Table 1. Short table
 
 9. Figures
 • Figure 2
 • Figure 3
 • Figure 4, Figure 4a, Figure 4b
 
-x=1
-x + y = 10
-x + y + z = 100
-
-10. Includes
-• Commands from metadata include: arg min R
-
-6. Links
-• Section: Section 1, Section 1.2
-• Appendix section: Section B, Section A.1.1
-• Appendix figure: Figure A1
-• Appendix table: Table B1
-• Appendix math: Equation 4
-
 1
+2
 
 Example footnote text.
 Footnote in sub-figure caption.
-3
-Footnote in figure caption.
-4
-Footnote in figure caption.
-2
 
 A
 B
 C
 D
 E
 F
@@ -375,20 +374,28 @@
 
 5
 
 6
 
 Table 2. Wide table
 
+10. Includes
+• Commands from metadata include: arg min R
 • Include command in body (there should be text after
 this):
 Content added through include statement.
 
 Figure 2. Narrow figure
 
+3
+4
+
+Footnote in figure caption.
+Footnote in figure caption.
+
 References
 Knuth, D. E. Literate programming. The Computer Journal,
 27(2):97–111, 1984.
 Knuth, D. E. The TEX Book. Addison-Wesley Professional,
 1986.
 Lesk, M. and Kernighan, B. Computer typesetting of
 technical journals on UNIX. In Proceedings of American
```

### Comparing `shiny_mdc-1.3.1/test/samples/neurips.pdf` & `shiny_mdc-1.4.0/test/samples/neurips.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 7% similar despite different names*

#### pdftotext {} -

```diff
@@ -155,15 +155,14 @@
 a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
 R∞
 2
 • Inline: 0 exp−x dx
 • Block: Equation 1, Equation 2
 • Commands defined in body (P[x in X]): P[x ∈ X ]
 • Aligned:
-
 x=1
 x + y = 10
 x + y + z = 100
 
 6
 
 Links
@@ -175,34 +174,57 @@
 • Pointer to footnote 1
 
 7
 
 Citations
 • Short citation [2]
 • Short citation with pre note [see 2]
-• Short citation with post note [2, p. 1]
-• Short citation with pre/post notes [see 2, p. 1]
+• Short citation with locator [2, p. 1]
+• Short citation with post note [2, for more]
+• Short citation with locators and pre/post notes [see 2, chap. 1-4, for more]
 • Long citation: Lesk and Kernighan [3]
-• Long citation with note: Lesk and Kernighan [3, p. 1]
+• Long citation with locator: Lesk and Kernighan [3, chap. 1]
+• Long citation with note: Lesk and Kernighan [3, for more]
 • Multi citation [2–4]
 • Multi citation with pre note [see 2–4]
+• Multi citation with locators [3, sec. 1; 4; 2, p. 1-3]
 • Multi citation with post note [2–4, for more]
-• Multi citation with pre/post notes [see 2–4, for more]
+• Multi citation with locators and pre/post notes [see 3, p. 1; 4; 2, chap. 1-2, for more]
 
 8
 
 Tables
 • Table 1
 • Table 2
 
-Col1
+9
+
+Figures
+• Figure 2
+• Figure 3
+• Figure 4, Figure 4a, Figure 4b
+1
+
+Example footnote text.
+Footnote in sub-figure caption.
+3
+Footnote in figure caption.
+2
+
+3
+
+(2)
+
+Col1
 1
 11
 111
 
+10
+
 Col2
 
 Col3
 
 Col4
 
 2
@@ -210,19 +232,15 @@
 4
 22
 33
 44
 222 333 444
 Table 1: Short table
 
-3
-
-(2)
-
-Col1
+Col1
 
 Col2
 
 Col3
 
 Col4
 
@@ -284,17 +302,24 @@
 
 4
 
 5
 
 6
 
+Includes
+• Commands from metadata include: arg min R
+• Include command in body (there should be text after this):
+
+Content added through include statement.
+
 Figure 2: Narrow figure
+4
 
-A
+A
 B
 C
 D
 E
 F
 G
 H
@@ -311,15 +336,15 @@
 
 x
 
 70
 
 Figure 3: Wide figure
 
-4
+5
 
 72
 
 74
 
 76
 
@@ -360,47 +385,22 @@
 
 5
 
 (b) Figure with ‘width=3.5in’ 2
 
 Figure 4: Sub-figures 3
 
-9
-
-Figures
-• Figure 2
-• Figure 3
-• Figure 4, Figure 4a, Figure 4b
-
-1
-
-Example footnote text.
-Footnote in sub-figure caption.
-3
-Footnote in figure caption.
-2
-
-5
+6
 
 10
 
 x
 
 15
 
-10
-
-Includes
-• Commands from metadata include: arg min R
-• Include command in body (there should be text after this):
-
-Content added through include statement.
-
-6
-
 References
 [1] Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
 [2] Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle, and Chris Rowley. The
 LATEX Companion. Addison-Wesley Professional, 2 edition, 2004.
 [3] Michael Lesk and Brian Kernighan. Computer typesetting of technical journals on UNIX.
 In Proceedings of American Federation of Information Processing Societies: 1977 National
 Computer Conference, pages 879–888, Dallas, Texas, 1977.
```

### Comparing `shiny_mdc-1.3.1/test/samples/spacious.pdf` & `shiny_mdc-1.4.0/test/samples/spacious.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 8% similar despite different names*

#### pdftotext {} -

```diff
@@ -155,22 +155,25 @@
 • Appendix table: Table B1
 • Appendix math: Equation 4
 • Pointer to footnote 1
 
 7. Citations
 • Short citation [2]
 • Short citation with pre note [see 2]
-• Short citation with post note [2, p. 1]
-• Short citation with pre/post notes [see 2, p. 1]
+• Short citation with locator [2, p. 1]
+• Short citation with post note [2, for more]
+• Short citation with locators and pre/post notes [see 2, chap. 1-4, for more]
 • Long citation: Lesk and Kernighan (1977) [3]
-• Long citation with note: Lesk and Kernighan (1977) [3, p. 1]
+• Long citation with locator: Lesk and Kernighan (1977) [3, chap. 1]
+• Long citation with note: Lesk and Kernighan (1977) [3, for more]
 • Multi citation [2–4]
 • Multi citation with pre note [see 2–4]
+• Multi citation with locators [3, sec. 1; 4; 2, p. 1-3]
 • Multi citation with post note [2–4, for more]
-• Multi citation with pre/post notes [see 2–4, for more]
+• Multi citation with locators and pre/post notes [see 3, p. 1; 4; 2, chap. 1-2, for more]
 
 8. Tables
 • Table 1
 • Table 2
 
 1
```

### Comparing `shiny_mdc-1.3.1/test/samples/standalone.pdf` & `shiny_mdc-1.4.0/test/samples/standalone.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 7% similar despite different names*

#### pdftotext {} -

```diff
@@ -155,22 +155,32 @@
 • Pointer to footnote a
 
 7
 
 Citations
 • Short citation [1]
 • Short citation with pre note [see 1]
-• Short citation with post note [1, p. 1]
-• Short citation with pre/post notes [see 1, p. 1]
+• Short citation with locator [1, p. 1]
+• Short citation with post note [1, for more]
+• Short citation with locators and pre/post notes [see 1, chap. 1-4, for more]
 • Long citation: Lesk and Kernighan (1977) [2]
-• Long citation with note: Lesk and Kernighan (1977) [2, p. 1]
+• Long citation with locator: Lesk and Kernighan (1977) [2, chap. 1]
+• Long citation with note: Lesk and Kernighan (1977) [2, for more]
 • Multi citation [1–3]
 • Multi citation with pre note [see 1–3]
+• Multi citation with locators [2, sec. 1; 3; 1, p. 1-3]
 • Multi citation with post note [1–3, for more]
-• Multi citation with pre/post notes [see 1–3, for more]
+• Multi
+citation
+with
+locators
+and
+pre/post
+notes
+[see 2, p. 1; 3; 1, chap. 1-2, for more]
 
 8
 
 Tables
 • Table 1
 • Table 2
 Col1
```

### Comparing `shiny_mdc-1.3.1/test/samples/stylish.pdf` & `shiny_mdc-1.4.0/test/samples/stylish.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -29,15 +29,15 @@
 Phasellus ultrices mi non nulla hendrerit, at rhoncus augue suscipit. Pellentesque a lectus eget felis maximus feugiat
 nec ut ante. Sed eget laoreet lectus. Vestibulum iaculis enim
 nec libero sollicitudin, id rhoncus libero consectetur. Integer
 eget sem quis urna vulputate aliquet.
 
 1.1. Subsection 1
 In mollis tortor vel ante cursus, ac consectetur nibh commodo.
-Aenean ultricies ornare ante ac fermentum. Vestibulum malesuada lectus at pellentesque hendrerit. Praesent a tempor ex,
+Aenean ultricies ornare ante ac fermentum. Vestibulum male-
 
 Equal contribution. 1 Institute One. 2 Institute Two at City, State.
 
 1.2. Subsection 2
 1.2.1. Subsubsection 1
 Suspendisse erat est, imperdiet sed dolor at, sagittis lobortis
 tortor. Nulla facilisi. Aliquam pharetra scelerisque auctor.
@@ -47,17 +47,15 @@
 In ut nunc libero. Duis eu elementum purus. Etiam dictum,
 ipsum nec aliquam lobortis, magna magna pellentesque ligula,
 sed ultricies odio ligula vitae orci. Fusce bibendum maximus
 ligula, id gravida felis dictum a. In dapibus nulla eget volutpat
 vulputate. Quisque congue erat quis nibh molestie, eget varius
 eros ultrices.
 Subsubsubsection Proin eleifend lorem semper, commodo
-tellus nec, porta purus. Nullam commodo lectus nibh, consequat maximus lorem faucibus in. Nam purus eros, rutrum in
-sapien et, condimentum lacinia nibh.
-dataset = I
+tellus nec, porta purus. Nullam commodo lectus nibh, consedataset = I
 
 dataset = II
 
 dataset = III
 
 dataset = IV
 
@@ -73,14 +71,15 @@
 12
 10
 
 y
 
 *
 
+suada lectus at pellentesque hendrerit. Praesent a tempor ex,
 eget iaculis mauris. Integer turpis nunc, varius ac posuere
 consequat, molestie sed felis. Fusce cursus velit eu magna
 pellentesque posuere sed eget ex. Vivamus in gravida quam,
 in volutpat erat.
 
 8
 6
@@ -107,105 +106,26 @@
 
 (c) Sub-figure with ‘width=2in’
 
 Figure 1: Sub-figures
 
 1
 
-Col1
-
-Col2
-
-Col3
-
-Col4
-
-Col5
-
-Col6
-
-Col7
-
-Col8
-
-Col9
-
-Col10
-
-a
-b
-
-1
-11
-
-2
-22
-
-3
-33
-
-123
-456
-
-abcd
-efgh
-
-1234
-567
-
-444
-44
-
-555
-55
-
-666
-66
-
-Mid
-c
-
-111
-
-222
-
-333
-
-789
-
-ijkl
-
-89
-
-4
-
-5
-
-6
-
-Table 2: Wide table
+quat maximus lorem faucibus in. Nam purus eros, rutrum in
+sapien et, condimentum lacinia nibh.
 
 2. Typography
-
-• Appendix table: Table B1
-• Appendix math: Equation 4
-• Pointer to footnote ¹
-
 • Bold
 • Italic
 • Bold italic.
 
 3. Numbers
 • Normal: 0123456789
 • Math: 0123456789
 
-¹ Example footnote text.
-
-7. Citations
-
 4. Acronyms
 • Default (short+long): Carnegie Mellon University
 (CMU)
 • Repeated (short): CMU
 • Forced short: USA
 • Repeated after forced short (short+long): United States
 of America (USA)
@@ -214,87 +134,99 @@
 5. Math
 Z ∞
 
 2
 
 exp−x dx
 
-0
-
-(1)
-
+7. Citations
 • Short citation[²]
 • Short citation with pre note[ˢᵉᵉ ²]
-• Short citation with post note[²𝄒 ᵖ⋅ ¹]
-• Short citation with pre/post notes[ˢᵉᵉ ²𝄒 ᵖ⋅ ¹]
+• Short citation with locator[²𝄒 ᵖ⋅ ¹]
+• Short citation with post note[²𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
+• Short citation with locators and pre/post notes[ˢᵉᵉ ²𝄒 ᶜʰᵃᵖ⋅ ¹⁻
+⁴𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
 • Long citation: Lesk and Kernighan (1977)[³]
+• Long citation with locator: Lesk and Kernighan
+(1977)[³𝄒 ᶜʰᵃᵖ⋅ ¹]
 • Long citation with note: Lesk and Kernighan
-(1977)[³𝄒 ᵖ⋅ ¹]
+(1977)[³𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
 • Multi citation[²𝄒 ³𝄒 ⁴]
 • Multi citation with pre note[ˢᵉᵉ ²𝄒 ³𝄒 ⁴]
+• Multi citation with locators [³𝄒 ˢᵉᶜ⋅ ¹; ⁴; ²𝄒 ᵖ⋅ ¹⁻³]
 • Multi citation with post note[²𝄒 ³𝄒 ⁴𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
-• Multi citation with pre/post notes[ˢᵉᵉ ²𝄒 ³𝄒 ⁴𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
+• Multi citation with locators and pre/post notes [ˢᵉᵉ ³𝄒 ᵖ⋅ ¹;
+⁴; ²𝄒 ᶜʰᵃᵖ⋅ ¹⁻²𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
 
 8. Tables
+• Table 1
+• Table 2
+
+(1)
 
-1 6, 7, 8, 9
-a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1,•2,Table
-3, 4, 5,
-•
-Table
-2
-(2)
-R∞
-2
-• Inline: 0 exp−x dx
-• Block: Equation 1, Equation 2
 Col1
-• Commands defined in body (P[x in X]): P[x ∈ X ]
-1
-• Aligned:
-11
-111
+
+0
 
 Col2
 
 Col3
 
 Col4
 
+1
 2
-22
-222
-
 3
-33
-333
-
 4
+a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 11
+7, 8, 9
+22
+33
 44
-444
-
+(2)
+111
+222 333 444
+R∞
+2
+• Inline: 0 exp−x dx
 Table 1: Short table
+• Block: Equation 1, Equation 2
+• Commands defined in body (P[x in X]): P[x ∈ X ]
+• Aligned:
+
+9. Figures
 
 x=1
 x + y = 10
 x + y + z = 100
 
 6. Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
+• Appendix table: Table B1
+• Appendix math: Equation 4
+• Pointer to footnote ¹
+
+¹ Example footnote text.
 
-9. Figures
 • Figure 2
 • Figure 3
 • Figure 4, Figure 4a, Figure 4b
 
-2
+10. Includes
+• Commands from metadata include: arg min R
+• Include command in body (there should be text after
+this):
+Content added through include statement.
 
 ² Footnote in sub-figure caption.
+³ Footnote in figure caption.
+
+2
 
 A
 B
 C
 D
 E
 F
@@ -367,19 +299,86 @@
 
 (b) Figure with ‘width=3.5in’ ²
 
 Figure 4: Sub-figures ³
 
 3
 
-10. Includes
-• Commands from metadata include: arg min R
-• Include command in body (there should be text after
-this):
-Content added through include statement.
+Col1
+
+Col2
+
+Col3
+
+Col4
+
+Col5
+
+Col6
+
+Col7
+
+Col8
+
+Col9
+
+Col10
+
+a
+b
+
+1
+11
+
+2
+22
+
+3
+33
+
+123
+456
+
+abcd
+efgh
+
+1234
+567
+
+444
+44
+
+555
+55
+
+666
+66
+
+Mid
+c
+
+111
+
+222
+
+333
+
+789
+
+ijkl
+
+89
+
+4
+
+5
+
+6
+
+Table 2: Wide table
 
 References
 [1] Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
 [2] Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle,
 and Chris Rowley. The LATEX Companion. Addison-Wesley Professional,
 2 edition, 2004.
 [3] Michael Lesk and Brian Kernighan. Computer typesetting of technical
@@ -428,43 +427,33 @@
 Appendix 1
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi purus, bibendum non neque sed, lacinia tristique
 tortor. Vestibulum eu lectus sed velit luctus varius. Sed sollicitudin ligula ante. Integer porta a erat commodo dignissim.
 Duis et lectus diam. Nulla id erat vestibulum nisi placerat
 efficitur. Nulla a semper libero. Praesent pharetra ullamcorper massa vel tincidunt. Sed dignissim magna et tellus
 efficitur, vitae sollicitudin lorem tincidunt. Nam non velit et
+
 enim rutrum euismod.
 
 A.1 Appendix subsection
-A.1.1
-
-Appendix subsubsection
-
+A.1.1 Appendix subsubsection
 Proin eleifend lorem semper, commodo tellus nec, porta purus.
 Nullam commodo lectus nibh, consequat maximus lorem faucibus in. Nam purus eros, rutrum in sapien et, condimentum
 lacinia nibh.
 
 A.2 Appendix figures
 • Figure A1
 • Figure A2
 
 A.3 Appendix includes
 • Commands from metadata include (argmin R):
 • Include command in body (there should be text after
 this):
 Content added through include statement.
 
-A.4 Appendix links
-• Appendix section: Section A.1.1, Section B
-• Main body section: Section 1
-• Main body figure: Figure 2
-• Main body table: Table 1
-• Main body equation: Equation 1
-• Citation: Knuth (1984)[⁴]
-
 5
 
 (a) Figure with non-default extension
 
 (b) Sub-figure
 
 dataset = I
@@ -510,14 +499,24 @@
 
 (c) Sub-figure
 
 Figure A2: Sub-figures with large combined size.
 
 6
 
+A.4 Appendix links
+• Appendix section: Section A.1.1, Section B
+• Main body section: Section 1
+• Main body figure: Figure 2
+• Main body table: Table 1
+• Main body equation: Equation 1
+• Citation: Knuth (1984)[⁴]
+
+7
+
 Col1
 
 Col2
 
 Col3
 
 Col4
@@ -664,10 +663,10 @@
 • Block without tag:
 x + y + z = 100
 
 ¹ Footnote in table.
 ² Footnote in table.
 ³ Footnote in table caption.
 
-7
+8
```

### Comparing `shiny_mdc-1.3.1/test/sections/appendix1.md` & `shiny_mdc-1.4.0/test/sections/appendix1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/test/sections/appendix2.md` & `shiny_mdc-1.4.0/test/sections/appendix2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/test/sections/main1.md` & `shiny_mdc-1.4.0/test/sections/main1.md`

 * *Files 20% similar despite different names*

```diff
@@ -64,15 +64,18 @@
 
 [^1]: Example footnote text.
 
 # Citations
 
 * Short citation [@latex:companion]
 * Short citation with pre note [see @latex:companion]
-* Short citation with post note [@latex:companion, p. 1]
-* Short citation with pre/post notes [see @latex:companion, p. 1]
+* Short citation with locator [@latex:companion, p. 1]
+* Short citation with post note [@latex:companion, for more]
+* Short citation with locators and pre/post notes [see @latex:companion, chap. 1-4, for more]
 * Long citation: @lesk:1977
-* Long citation with note: @lesk:1977 [p. 1]
+* Long citation with locator: @lesk:1977 [chap. 1]
+* Long citation with note: @lesk:1977 [for more]
 * Multi citation [@lesk:1977; @knuth:1984; @latex:companion]
 * Multi citation with pre note [see @lesk:1977; @knuth:1984; @latex:companion]
+* Multi citation with locators [@lesk:1977, sec. 1; @knuth:1984; @latex:companion, p. 1-3]
 * Multi citation with post note [@lesk:1977; @knuth:1984; @latex:companion, for more]
-* Multi citation with pre/post notes [see @lesk:1977; @knuth:1984; @latex:companion, for more]
+* Multi citation with locators and pre/post notes [see @lesk:1977, p. 1; @knuth:1984; @latex:companion, chap. 1-2, for more]
```

### Comparing `shiny_mdc-1.3.1/test/sections/main2.md` & `shiny_mdc-1.4.0/test/sections/main2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/test/utils/commands.md` & `shiny_mdc-1.4.0/test/utils/commands.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.1/PKG-INFO` & `shiny_mdc-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny-mdc
-Version: 1.3.1
+Version: 1.4.0
 Summary: Tool to compile markdown files to tex/pdf using pandoc, latexmk
 Home-page: https://github.com/jayanthkoushik/shinymdc
 License: MIT
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

