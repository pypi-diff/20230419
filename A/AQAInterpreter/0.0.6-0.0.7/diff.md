# Comparing `tmp/aqainterpreter-0.0.6.tar.gz` & `tmp/aqainterpreter-0.0.7.tar.gz`

## Comparing `aqainterpreter-0.0.6.tar` & `aqainterpreter-0.0.7.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/README.md
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/input.txt
--rwxr-xr-x   0        0        0      997 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/setup.sh
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/.vscode/extentions.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/.vscode/launch.json
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/.vscode/settings.json
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/AQAInterpreter/__init__.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/AQAInterpreter/environment.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/AQAInterpreter/errors.py
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/AQAInterpreter/interpreter.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/AQAInterpreter/main.py
--rw-r--r--   0        0        0     8915 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/AQAInterpreter/parser.py
--rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/AQAInterpreter/scanner.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/AQAInterpreter/test_.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/AQAInterpreter/tokens.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/add_code.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/aqa.xml
--rwxr-xr-x   0        0        0      601 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/compile_report.sh
--rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/compile_report_no_font.sh
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/notes.md
--rw-r--r--   0        0        0    44260 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/report.md
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/watch.py
--rw-r--r--   0        0        0    39279 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/classes.svg
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/comparison.svg
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/compiler.svg
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/declaration.svg
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/declarations.svg
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/end.svg
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/equality.svg
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/expression.svg
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/factor.svg
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/for.svg
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/if.svg
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/logic_and.svg
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/logic_or.svg
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/mermaid_config.json
--rw-r--r--   0        0        0    21859 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/packages.svg
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/parser.svg
--rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/primary.svg
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/print.svg
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/program.svg
--rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/scanner.svg
--rw-r--r--   0        0        0   234850 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/screenshot1.png
--rw-r--r--   0        0        0    67423 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/screenshot2.png
--rw-r--r--   0        0        0    76110 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/screenshot3.png
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/statement.svg
--rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/symbol_table.svg
--rw-r--r--   0        0        0    28131 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/syntax_tree.svg
--rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/syntax_tree_edit.svg
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/term.svg
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/unary.svg
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/variable_declaration.svg
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/while.svg
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/classes.mmd
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/comparison.pikchr
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/compiler.pikchr
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/declaration.pikchr
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/declarations.pikchr
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/end.pikchr
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/equality.pikchr
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/expression.pikchr
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/factor.pikchr
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/for.pikchr
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/if.pikchr
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/logic_and.pikchr
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/logic_or.pikchr
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/packages.mmd
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/parser.mmd
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/primary.pikchr
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/print.pikchr
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/program.pikchr
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/scanner.mmd
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/statement.pikchr
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/symbol_table.mmd
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/syntax_tree.mmd
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/term.pikchr
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/unary.pikchr
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/variable_declaration.pikchr
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/report/assets/input/while.pikchr
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/LICENSE
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aqainterpreter-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/README.md
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/input.txt
+-rwxr-xr-x   0        0        0     1013 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/setup.sh
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/.vscode/extentions.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/.vscode/launch.json
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/.vscode/settings.json
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/__main__.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/environment.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/errors.py
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/interpreter.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/main.py
+-rw-r--r--   0        0        0     8915 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/parser.py
+-rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/scanner.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/test_.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/tokens.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/add_code.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/aqa.xml
+-rwxr-xr-x   0        0        0      601 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/compile_report.sh
+-rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/compile_report_no_font.sh
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/notes.md
+-rw-r--r--   0        0        0    44260 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/report.md
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/watch.py
+-rw-r--r--   0        0        0    39279 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/classes.svg
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/comparison.svg
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/compiler.svg
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/declaration.svg
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/declarations.svg
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/end.svg
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/equality.svg
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/expression.svg
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/factor.svg
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/for.svg
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/if.svg
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/logic_and.svg
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/logic_or.svg
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/mermaid_config.json
+-rw-r--r--   0        0        0    21859 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/packages.svg
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/parser.svg
+-rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/primary.svg
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/print.svg
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/program.svg
+-rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/scanner.svg
+-rw-r--r--   0        0        0   234850 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/screenshot1.png
+-rw-r--r--   0        0        0    67423 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/screenshot2.png
+-rw-r--r--   0        0        0    76110 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/screenshot3.png
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/statement.svg
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/symbol_table.svg
+-rw-r--r--   0        0        0    28131 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/syntax_tree.svg
+-rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/syntax_tree_edit.svg
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/term.svg
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/unary.svg
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/variable_declaration.svg
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/while.svg
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/classes.mmd
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/comparison.pikchr
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/compiler.pikchr
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/declaration.pikchr
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/declarations.pikchr
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/end.pikchr
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/equality.pikchr
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/expression.pikchr
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/factor.pikchr
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/for.pikchr
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/if.pikchr
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/logic_and.pikchr
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/logic_or.pikchr
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/packages.mmd
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/parser.mmd
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/primary.pikchr
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/print.pikchr
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/program.pikchr
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/scanner.mmd
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/statement.pikchr
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/symbol_table.mmd
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/syntax_tree.mmd
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/term.pikchr
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/unary.pikchr
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/variable_declaration.pikchr
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/while.pikchr
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/LICENSE
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/PKG-INFO
```

### Comparing `aqainterpreter-0.0.6/README.md` & `aqainterpreter-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/setup.sh` & `aqainterpreter-0.0.7/setup.sh`

 * *Files 14% similar despite different names*

```diff
@@ -26,13 +26,12 @@
 # # auto generate packages.mmd and classes.md
 # pyreverse ./AQAInterpreter/ -o mmd
 
 # # setup project
 # hatch shell
 
 # # publish to pypi
-# hatch build
-# hatch publish
+# hatch build && hatch publish && rm -rf dist
 #   # go on https://pypi.org
 #   # get a token https://pypi.org/help/#apitoke
 #   # copy paste the username and token in this command
```

### Comparing `aqainterpreter-0.0.6/.vscode/launch.json` & `aqainterpreter-0.0.7/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/.vscode/settings.json` & `aqainterpreter-0.0.7/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/AQAInterpreter/environment.py` & `aqainterpreter-0.0.7/AQAInterpreter/environment.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/AQAInterpreter/errors.py` & `aqainterpreter-0.0.7/AQAInterpreter/errors.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/AQAInterpreter/interpreter.py` & `aqainterpreter-0.0.7/AQAInterpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/AQAInterpreter/main.py` & `aqainterpreter-0.0.7/AQAInterpreter/main.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/AQAInterpreter/parser.py` & `aqainterpreter-0.0.7/AQAInterpreter/parser.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/AQAInterpreter/scanner.py` & `aqainterpreter-0.0.7/AQAInterpreter/scanner.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/AQAInterpreter/test_.py` & `aqainterpreter-0.0.7/AQAInterpreter/test_.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/AQAInterpreter/tokens.py` & `aqainterpreter-0.0.7/AQAInterpreter/tokens.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/add_code.py` & `aqainterpreter-0.0.7/report/add_code.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/aqa.xml` & `aqainterpreter-0.0.7/report/aqa.xml`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/compile_report.sh` & `aqainterpreter-0.0.7/report/compile_report.sh`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/notes.md` & `aqainterpreter-0.0.7/report/notes.md`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/report.md` & `aqainterpreter-0.0.7/report/report.md`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/watch.py` & `aqainterpreter-0.0.7/report/watch.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/classes.svg` & `aqainterpreter-0.0.7/report/assets/classes.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/comparison.svg` & `aqainterpreter-0.0.7/report/assets/comparison.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/compiler.svg` & `aqainterpreter-0.0.7/report/assets/compiler.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/declaration.svg` & `aqainterpreter-0.0.7/report/assets/declaration.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/declarations.svg` & `aqainterpreter-0.0.7/report/assets/declarations.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/end.svg` & `aqainterpreter-0.0.7/report/assets/end.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/equality.svg` & `aqainterpreter-0.0.7/report/assets/equality.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/expression.svg` & `aqainterpreter-0.0.7/report/assets/expression.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/factor.svg` & `aqainterpreter-0.0.7/report/assets/factor.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/for.svg` & `aqainterpreter-0.0.7/report/assets/for.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/if.svg` & `aqainterpreter-0.0.7/report/assets/if.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/logic_and.svg` & `aqainterpreter-0.0.7/report/assets/logic_and.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/logic_or.svg` & `aqainterpreter-0.0.7/report/assets/logic_or.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/packages.svg` & `aqainterpreter-0.0.7/report/assets/packages.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/parser.svg` & `aqainterpreter-0.0.7/report/assets/parser.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/primary.svg` & `aqainterpreter-0.0.7/report/assets/primary.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/print.svg` & `aqainterpreter-0.0.7/report/assets/print.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/program.svg` & `aqainterpreter-0.0.7/report/assets/program.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/scanner.svg` & `aqainterpreter-0.0.7/report/assets/scanner.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/screenshot1.png` & `aqainterpreter-0.0.7/report/assets/screenshot1.png`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/screenshot2.png` & `aqainterpreter-0.0.7/report/assets/screenshot2.png`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/screenshot3.png` & `aqainterpreter-0.0.7/report/assets/screenshot3.png`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/statement.svg` & `aqainterpreter-0.0.7/report/assets/statement.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/symbol_table.svg` & `aqainterpreter-0.0.7/report/assets/symbol_table.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/syntax_tree.svg` & `aqainterpreter-0.0.7/report/assets/syntax_tree.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/syntax_tree_edit.svg` & `aqainterpreter-0.0.7/report/assets/syntax_tree_edit.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/term.svg` & `aqainterpreter-0.0.7/report/assets/term.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/unary.svg` & `aqainterpreter-0.0.7/report/assets/unary.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/variable_declaration.svg` & `aqainterpreter-0.0.7/report/assets/variable_declaration.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/while.svg` & `aqainterpreter-0.0.7/report/assets/while.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/classes.mmd` & `aqainterpreter-0.0.7/report/assets/input/classes.mmd`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/comparison.pikchr` & `aqainterpreter-0.0.7/report/assets/input/comparison.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/declaration.pikchr` & `aqainterpreter-0.0.7/report/assets/input/declaration.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/end.pikchr` & `aqainterpreter-0.0.7/report/assets/input/end.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/equality.pikchr` & `aqainterpreter-0.0.7/report/assets/input/equality.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/factor.pikchr` & `aqainterpreter-0.0.7/report/assets/input/factor.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/for.pikchr` & `aqainterpreter-0.0.7/report/assets/input/for.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/if.pikchr` & `aqainterpreter-0.0.7/report/assets/input/if.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/logic_and.pikchr` & `aqainterpreter-0.0.7/report/assets/input/logic_and.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/logic_or.pikchr` & `aqainterpreter-0.0.7/report/assets/input/logic_or.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/packages.mmd` & `aqainterpreter-0.0.7/report/assets/input/packages.mmd`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/primary.pikchr` & `aqainterpreter-0.0.7/report/assets/input/primary.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/statement.pikchr` & `aqainterpreter-0.0.7/report/assets/input/statement.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/term.pikchr` & `aqainterpreter-0.0.7/report/assets/input/term.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/unary.pikchr` & `aqainterpreter-0.0.7/report/assets/input/unary.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/report/assets/input/while.pikchr` & `aqainterpreter-0.0.7/report/assets/input/while.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/LICENSE` & `aqainterpreter-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.6/pyproject.toml` & `aqainterpreter-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "AQAInterpreter"
 requires-python = ">=3.10"
 license = "MIT"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name = "CyberWarrior5466", email = "asaleen898@gmail.com" },
 ]
 dependencies = ["click==8.*"]
 
 [project.urls]
 Documentation = "https://github.com/CyberWarrior5466/nea"
```

