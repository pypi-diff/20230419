# Comparing `tmp/pharmpy-core-0.92.0.tar.gz` & `tmp/pharmpy-core-0.93.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pharmpy-core-0.92.0.tar", last modified: Wed Apr  5 15:37:57 2023, max compression
+gzip compressed data, was "pharmpy-core-0.93.0.tar", last modified: Wed Apr 19 08:41:17 2023, max compression
```

## Comparing `pharmpy-core-0.92.0.tar` & `pharmpy-core-0.93.0.tar`

### file list

```diff
@@ -1,1177 +1,1182 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.938387 pharmpy-core-0.92.0/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    43920 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/LICENSE.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    45885 2023-04-05 15:37:57.946387 pharmpy-core-0.92.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.818385 pharmpy-core-0.92.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/NONMEM.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/Pharmpy_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/Pharmpy_logo_dark.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.818385 pharmpy-core-0.92.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/_ext/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/_ext/pharmpy_snippet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/allometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/amd.rst
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/api_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/api_modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/api_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/api_workflows.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/bootstrap.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/cdd.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/code_of_conduct.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/contributors.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/covsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/crossval.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/design.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/developers.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/estmethod.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/frem.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/iivsearch.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.818385 pharmpy-core-0.92.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/images/Pharmpy_symbol.svg
--rw-r--r--   0 runner    (1001) docker     (123)   179150 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/images/tools.png
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/iovsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/linearize.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/modelfit.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28177 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/modelsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/nonmem_plugin.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/pharmr_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/plots.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/projects.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/psn_resmod.rst
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/psn_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/qa.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/ruvsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/scm.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/simeval.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/docs/using_r.rst
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-05 15:37:57.946387 pharmpy-core-0.92.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.818385 pharmpy-core-0.92.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.818385 pharmpy-core-0.92.0/src/pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    80309 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.818385 pharmpy-core-0.92.0/src/pharmpy/deps/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/deps/altair.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/deps/rich.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/deps/scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/deps/sympy_printing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.822385 pharmpy-core-0.92.0/src/pharmpy/internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/code_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.822385 pharmpy-core-0.92.0/src/pharmpy/internals/ds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/ds/ordered_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.822385 pharmpy-core-0.92.0/src/pharmpy/internals/expr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/expr/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/expr/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/expr/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/expr/leaves.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/expr/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/expr/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/expr/subs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/expr/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/expr/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.822385 pharmpy-core-0.92.0/src/pharmpy/internals/fn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/fn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/fn/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/fn/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.822385 pharmpy-core-0.92.0/src/pharmpy/internals/fs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/fs/cwd.py
--rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/fs/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/fs/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/fs/tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.802384 pharmpy-core-0.92.0/src/pharmpy/internals/graph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.822385 pharmpy-core-0.92.0/src/pharmpy/internals/graph/directed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/graph/directed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/graph/directed/connected_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/graph/directed/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/graph/directed/reachability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/immutable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.822385 pharmpy-core-0.92.0/src/pharmpy/internals/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/module/lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.826385 pharmpy-core-0.92.0/src/pharmpy/internals/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/parse/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/parse/ignored.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/parse/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/parse/prettyprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/parse/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/parse/treeprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.826385 pharmpy-core-0.92.0/src/pharmpy/internals/sequence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/sequence/lcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.826385 pharmpy-core-0.92.0/src/pharmpy/internals/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/set/partitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/set/subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/internals/unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.826385 pharmpy-core-0.92.0/src/pharmpy/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/model/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28256 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/model/datainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.826385 pharmpy-core-0.92.0/src/pharmpy/model/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/model/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/model/distributions/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/model/distributions/symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/model/estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/model/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    31661 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/model/random_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/model/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    65647 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/model/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.830385 pharmpy-core-0.92.0/src/pharmpy/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/basic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/block_rvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/blq.py
--rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/compartments.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    49857 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    33829 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/estimation_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/eta_additions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/eta_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.834385 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/
--rw-r--r--   0 runner    (1001) docker     (123)    50310 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/moxo.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/moxo.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.cov
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.tab
--rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno_linear.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno_linear.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno_linear.lst
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno_linear.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno_linear.phi
--rw-r--r--   0 runner    (1001) docker     (123)    45291 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/metabolite.py
--rw-r--r--   0 runner    (1001) docker     (123)    69049 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/odes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/parameter_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/remove_iiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/remove_iov.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/update_inits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/modeling/write_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.834385 pharmpy-core-0.92.0/src/pharmpy/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.834385 pharmpy-core-0.92.0/src/pharmpy/plugins/fcon/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/fcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/fcon/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.834385 pharmpy-core-0.92.0/src/pharmpy/plugins/nlmixr/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nlmixr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nlmixr/error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nlmixr/ini.py
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nlmixr/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nlmixr/model_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nlmixr/name_mangle.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nlmixr/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    10589 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nlmixr/sanity_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.834385 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/advan.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    14797 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/nmtran_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    27628 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.838385 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/abbreviated_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/code_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/data_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/estimation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/etas_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.838385 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/code_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/data_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/definitions.lark
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/option_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/problem_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/model_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    17573 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/omega_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/option_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/problem_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/raw_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/record.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/simulation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/sizes_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/subroutine_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/table_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/theta_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/results_file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7135 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    63092 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/plugins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.838385 pharmpy-core-0.92.0/src/pharmpy/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/reporting/altairplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/reporting/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/reporting/custom.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     5562 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/reporting/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.842385 pharmpy-core-0.92.0/src/pharmpy/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.842385 pharmpy-core-0.92.0/src/pharmpy/tools/allometry/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/allometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/allometry/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.842385 pharmpy-core-0.92.0/src/pharmpy/tools/amd/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/amd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/amd/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/amd/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    16039 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/amd/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.842385 pharmpy-core-0.92.0/src/pharmpy/tools/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/bootstrap/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/bootstrap/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/bootstrap/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.842385 pharmpy-core-0.92.0/src/pharmpy/tools/cdd/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/cdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/cdd/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.842385 pharmpy-core-0.92.0/src/pharmpy/tools/covsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/covsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/covsearch/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/covsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.842385 pharmpy-core-0.92.0/src/pharmpy/tools/crossval/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/crossval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/crossval/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.842385 pharmpy-core-0.92.0/src/pharmpy/tools/estmethod/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/estmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/estmethod/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/estmethod/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/estmethod/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.842385 pharmpy-core-0.92.0/src/pharmpy/tools/evaldesign/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/evaldesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/evaldesign/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.842385 pharmpy-core-0.92.0/src/pharmpy/tools/frem/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/frem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/frem/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/frem/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)    38407 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/frem/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/frem/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.842385 pharmpy-core-0.92.0/src/pharmpy/tools/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/funcs/ml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.846385 pharmpy-core-0.92.0/src/pharmpy/tools/funcs/ml_models/
--rw-r--r--   0 runner    (1001) docker     (123)    91484 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite
--rw-r--r--   0 runner    (1001) docker     (123)    93596 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/funcs/summarize_individuals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.846385 pharmpy-core-0.92.0/src/pharmpy/tools/iivsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/iivsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/iivsearch/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/iivsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.846385 pharmpy-core-0.92.0/src/pharmpy/tools/iovsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/iovsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/iovsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.846385 pharmpy-core-0.92.0/src/pharmpy/tools/linearize/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/linearize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/linearize/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/linearize/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.846385 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.846385 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/feature/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/feature/covariate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/feature/elimination.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/feature/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/feature/lagtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/feature/peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/feature/transits.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.846385 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.850385 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/covariate.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/elimination.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/lagtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/transits.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/mfl/stringify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.850385 pharmpy-core-0.92.0/src/pharmpy/tools/modelfit/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/modelfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/modelfit/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/modelfit/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.850385 pharmpy-core-0.92.0/src/pharmpy/tools/modelsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/modelsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/modelsearch/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/modelsearch/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/psn_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.850385 pharmpy-core-0.92.0/src/pharmpy/tools/qa/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/qa/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/rankfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31466 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.850385 pharmpy-core-0.92.0/src/pharmpy/tools/ruvsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/ruvsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/ruvsearch/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    16608 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/ruvsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.850385 pharmpy-core-0.92.0/src/pharmpy/tools/scm/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/scm/psn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/scm/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.850385 pharmpy-core-0.92.0/src/pharmpy/tools/simeval/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/simeval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/simeval/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.850385 pharmpy-core-0.92.0/src/pharmpy/tools/simfit/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/simfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/simfit/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/tools/wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.850385 pharmpy-core-0.92.0/src/pharmpy/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.850385 pharmpy-core-0.92.0/src/pharmpy/workflows/dispatchers/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/dispatchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/dispatchers/local_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.850385 pharmpy-core-0.92.0/src/pharmpy/workflows/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/model_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/model_database/baseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/model_database/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/model_database/null_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.854385 pharmpy-core-0.92.0/src/pharmpy/workflows/tool_database/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/tool_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/tool_database/baseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/tool_database/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/tool_database/null_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/src/pharmpy/workflows/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.854385 pharmpy-core-0.92.0/src/pharmpy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45885 2023-04-05 15:37:57.000000 pharmpy-core-0.92.0/src/pharmpy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    46519 2023-04-05 15:37:57.000000 pharmpy-core-0.92.0/src/pharmpy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 15:37:57.000000 pharmpy-core-0.92.0/src/pharmpy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-05 15:37:57.000000 pharmpy-core-0.92.0/src/pharmpy_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 15:32:03.000000 pharmpy-core-0.92.0/src/pharmpy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-05 15:37:57.000000 pharmpy-core-0.92.0/src/pharmpy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-05 15:37:57.000000 pharmpy-core-0.92.0/src/pharmpy_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.854385 pharmpy-core-0.92.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.854385 pharmpy-core-0.92.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/cli/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.854385 pharmpy-core-0.92.0/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.854385 pharmpy-core-0.92.0/tests/deps/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/deps/test_deps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.854385 pharmpy-core-0.92.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/integration/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/integration/test_amd.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/integration/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/integration/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/integration/test_covsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/integration/test_estmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/integration/test_evaldesign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/integration/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/integration/test_iivsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/integration/test_iovsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/integration/test_modelsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/integration/test_resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/integration/test_ruvsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.854385 pharmpy-core-0.92.0/tests/internals/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.854385 pharmpy-core-0.92.0/tests/internals/fs/
--rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/internals/fs/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/internals/fs/test_tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.858385 pharmpy-core-0.92.0/tests/internals/module/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/internals/module/test_lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/internals/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/internals/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.858385 pharmpy-core-0.92.0/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/model/test_datainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/model/test_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/model/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    26575 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/model/test_random_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/model/test_statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.862385 pharmpy-core-0.92.0/tests/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_add_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_basic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_block_rvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_blq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_compartments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_data_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_estimation_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_eta_additions.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_eta_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_has_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_metabolite.py
--rw-r--r--   0 runner    (1001) docker     (123)    99698 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_parameter_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_remove_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/modeling/test_units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.862385 pharmpy-core-0.92.0/tests/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.862385 pharmpy-core-0.92.0/tests/nonmem/output/
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/output/test_nonmem_results_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.862385 pharmpy-core-0.92.0/tests/nonmem/records/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/test_abbreviated.py
--rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/test_estimation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/test_etas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/test_model_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/test_omega.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/test_option_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/test_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/test_subroutines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/records/test_theta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/test_advan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/test_des.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/test_fcon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/test_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/test_modelfit_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    34984 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/test_nonmem_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/test_nonmem_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/nonmem/test_read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.862385 pharmpy-core-0.92.0/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/plugins/test_nlmixr.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/plugins/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.862385 pharmpy-core-0.92.0/tests/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.866385 pharmpy-core-0.92.0/tests/testdata/frem/
--rw-r--r--   0 runner    (1001) docker     (123)    52275 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/frem/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.870385 pharmpy-core-0.92.0/tests/testdata/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/DDMODEL00000130
--rw-r--r--   0 runner    (1001) docker     (123)    59142 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.870385 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real.lst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.870385 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.874385 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22454 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/skipped_individuals1.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.878385 pharmpy-core-0.92.0/tests/testdata/nonmem/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/errors/control_stream_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/errors/est_step_warning.lst
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst
--rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/errors/no_header_error.ext
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/errors/no_header_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/errors/rounding_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/errors/run_interrupted.ext
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/errors/run_interrupted.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/errors/zero_gradient_error.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.878385 pharmpy-core-0.92.0/tests/testdata/nonmem/fcon/
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/fcon/FCON
--rw-r--r--   0 runner    (1001) docker     (123)    39432 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/fcon/FDATA
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/file.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.806384 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.878385 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/
--rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.878385 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/
--rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.806384 pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.882386 pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-05 15:30:52.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.882386 pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/minimal.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.806384 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.882386 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/covariance/
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.806384 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/multPROB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.806384 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.882386 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91887 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.806384 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.806384 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.882386 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi
--rw-r--r--   0 runner    (1001) docker     (123)    59168 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov
--rw-r--r--   0 runner    (1001) docker     (123)   115118 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext
--rw-r--r--   0 runner    (1001) docker     (123)    82511 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod
--rw-r--r--   0 runner    (1001) docker     (123)    75841 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.882386 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.ext
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.806384 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.886386 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    26695 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17548 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)    16143 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst
--rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst
--rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst
--rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst
--rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.890386 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/
--rw-r--r--   0 runner    (1001) docker     (123)   178666 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext
--rw-r--r--   0 runner    (1001) docker     (123)  1091059 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.890386 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/simfit/
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    38485 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.890386 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_1transit.mod
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_2transits.mod
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan1.mod
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan11.mod
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan12.mod
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan3.mod
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan4.mod
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod
--rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.898386 pharmpy-core-0.92.0/tests/testdata/nonmem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/fviii6.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/fviii6.mod
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/fviii6.prn
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox2.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_2comp.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_2comp.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21336 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_2comp.lst
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_2comp.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_2comp.phi
--rw-r--r--   0 runner    (1001) docker     (123)   175384 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_simulated_log.csv
--rw-r--r--   0 runner    (1001) docker     (123)   185992 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_simulated_normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)   105888 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/mytab_mox2
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pef.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pef.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_advan3_trans1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_dvid.csv
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_dvid.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_noifs.coi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_noifs.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_noifs.cov
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_noifs.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_noifs.lst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_noifs.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_noifs.phi
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_trans1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_trans1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_trans1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_trans1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_abbr.mod
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_abbr_comments.mod
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_block.mod
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_clashing_symbols.mod
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_etas.mod
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_nm750.mod
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36053 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_rate.dta
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.coi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.cor
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.lst
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.phi
--rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.tab
--rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.xml
--rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real_linbase.tab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.902386 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/
--rw-r--r--   0 runner    (1001) docker     (123)   370034 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/add_etas_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/add_etas_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/add_etas_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/add_etas_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/boxcox.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/boxcox.lst
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/boxcox.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/boxcox.phi
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/cdd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/fullblock.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/fullblock.lst
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/fullblock.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/fullblock.phi
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/iov.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/iov.lst
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/iov.mod
--rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/iov.phi
--rw-r--r--   0 runner    (1001) docker     (123)   262826 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/pheno_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/pheno_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/pheno_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/pheno_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/pheno_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/resmod_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/scm_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   392990 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/simeval_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/tdist.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/tdist.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/tdist.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/qa/tdist.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.902386 pharmpy-core-0.92.0/tests/testdata/nonmem/ruvsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/ruvsearch/mox3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/ruvsearch/mox3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/ruvsearch/mox3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/ruvsearch/mox3.phi
--rw-r--r--   0 runner    (1001) docker     (123)   276902 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv
--rw-r--r--   0 runner    (1001) docker     (123)   180553 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/ruvsearch/mytab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.902386 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.902386 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/backward_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/backward_dir1/config_fake.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.902386 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/gofofv_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/localmin.logf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.902386 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/log_steps/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/log_steps/backward_pval_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/log_steps/backward_pval_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/log_steps/forward_pval_4.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.902386 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/mergeofv_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/mergeofv_dir1/config_havebaserun.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.906386 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/mergeofv_dir2/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/mergeofv_dir2/config_havebaserun.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.906386 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/onlyforward_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/onlyforward_dir1/config_normal.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.906386 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.906386 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/scmplus_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)   108031 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/sdtab1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.906386 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/pheno.cov
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/pheno_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.810384 pharmpy-core-0.92.0/tests/testdata/psn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.910386 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/est_data0.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/est_data1.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/est_data2.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/est_data3.dta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.914386 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/pred_data0.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/pred_data1.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/pred_data2.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/pred_data3.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/xv_result.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.914386 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/covariates_summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.914386 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/final_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/frem_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.918386 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi
--rw-r--r--   0 runner    (1001) docker     (123)    93135 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_1b.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_2.cor
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_2.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/proposal_density.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.918386 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/command.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.918386 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/linearize_run/
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/linearize_run/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.918386 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi
--rw-r--r--   0 runner    (1001) docker     (123)   137744 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table
--rw-r--r--   0 runner    (1001) docker     (123)   316422 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/results_summary.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.918386 pharmpy-core-0.92.0/tests/testdata/psn/resmod_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/resmod_dir1/resmod_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.918386 pharmpy-core-0.92.0/tests/testdata/psn/resmod_dir2/
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/resmod_dir2/resmod_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.918386 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.926386 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)    63331 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/original.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/original.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/original.ext
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/original.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/original.phi
--rw-r--r--   0 runner    (1001) docker     (123)    54391 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-4.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-5.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-6.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-7.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-8.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi
--rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta
--rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta
--rw-r--r--   0 runner    (1001) docker     (123)    21489 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.930386 pharmpy-core-0.92.0/tests/testdata/results/
--rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/allometry_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   263999 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/amd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   130598 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/bootstrap_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/cdd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)  1360720 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/covsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/estmethod_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   205797 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/iivsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   197228 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/iovsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/linearize_results.json
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)   105603 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/modelsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/qa_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    57352 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/ruvsearch_results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.810384 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.930386 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.930386 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.930386 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.810384 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.930386 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/input_model.csv
--rw-r--r--   0 runner    (1001) docker     (123)   183701 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:33:54.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.930386 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.930386 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.930386 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.934386 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91188 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.934386 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.934386 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91119 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.934386 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.934386 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    53630 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91754 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.934386 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.938387 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91879 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout
--rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/results.csv
--rw-r--r--   0 runner    (1001) docker     (123)   105597 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.938387 pharmpy-core-0.92.0/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_amd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_cdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_covsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_crossval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_estmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)    27774 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_frem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_iivsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_iovsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_linearize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_mfl.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_modelfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_modelsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_rankfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_runtool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_ruvsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_simeval.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_start_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_summarize_individuals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/tools/test_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:57.938387 pharmpy-core-0.92.0/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/workflows/test_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/workflows/test_execute.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/workflows/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/workflows/test_model_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/workflows/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/workflows/test_tool_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tests/workflows/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-05 15:30:53.000000 pharmpy-core-0.92.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.959406 pharmpy-core-0.93.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    44506 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/LICENSE.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    46471 2023-04-19 08:41:17.963406 pharmpy-core-0.93.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.835404 pharmpy-core-0.93.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/NONMEM.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/Pharmpy_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/Pharmpy_logo_dark.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.835404 pharmpy-core-0.93.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/_ext/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/_ext/pharmpy_snippet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/allometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/amd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/api_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/api_modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/api_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/api_workflows.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/bootstrap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/cdd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/code_of_conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/covsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/crossval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/design.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/developers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/estmethod.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/frem.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/iivsearch.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.835404 pharmpy-core-0.93.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/images/Pharmpy_symbol.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   179150 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/images/tools.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/iovsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/linearize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/modelfit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28177 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/modelsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/nonmem_plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/pharmr_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/plots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/projects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/psn_resmod.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/psn_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/qa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/ruvsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/scm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/simeval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/docs/using_r.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-19 08:41:17.963406 pharmpy-core-0.93.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.835404 pharmpy-core-0.93.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.835404 pharmpy-core-0.93.0/src/pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80309 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.835404 pharmpy-core-0.93.0/src/pharmpy/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/deps/altair.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/deps/rich.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/deps/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/deps/sympy_printing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.835404 pharmpy-core-0.93.0/src/pharmpy/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/code_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.835404 pharmpy-core-0.93.0/src/pharmpy/internals/ds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/ds/ordered_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.839403 pharmpy-core-0.93.0/src/pharmpy/internals/expr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/expr/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/expr/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/expr/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/expr/leaves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/expr/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/expr/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/expr/subs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/expr/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/expr/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.839403 pharmpy-core-0.93.0/src/pharmpy/internals/fn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/fn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/fn/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/fn/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.839403 pharmpy-core-0.93.0/src/pharmpy/internals/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/fs/cwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/fs/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/fs/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/fs/tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.819403 pharmpy-core-0.93.0/src/pharmpy/internals/graph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.839403 pharmpy-core-0.93.0/src/pharmpy/internals/graph/directed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/graph/directed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/graph/directed/connected_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/graph/directed/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/graph/directed/reachability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/immutable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.839403 pharmpy-core-0.93.0/src/pharmpy/internals/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/module/lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.839403 pharmpy-core-0.93.0/src/pharmpy/internals/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/parse/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/parse/ignored.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/parse/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/parse/prettyprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/parse/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/parse/treeprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.839403 pharmpy-core-0.93.0/src/pharmpy/internals/sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/sequence/lcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.839403 pharmpy-core-0.93.0/src/pharmpy/internals/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/set/partitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/set/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/internals/unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.839403 pharmpy-core-0.93.0/src/pharmpy/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/model/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28256 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/model/datainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.839403 pharmpy-core-0.93.0/src/pharmpy/model/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/model/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/model/distributions/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/model/distributions/symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/model/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/model/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32839 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/model/random_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/model/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65698 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/model/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.843404 pharmpy-core-0.93.0/src/pharmpy/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/basic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/block_rvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/blq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/compartments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49857 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33829 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/estimation_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/eta_additions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/eta_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.847404 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/
+-rw-r--r--   0 runner    (1001) docker     (123)    50310 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/moxo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/moxo.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.tab
+-rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno_linear.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno_linear.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno_linear.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno_linear.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno_linear.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    45291 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/metabolite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/odes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/parameter_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/remove_iiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/remove_iov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/tmdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/update_inits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/modeling/write_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.847404 pharmpy-core-0.93.0/src/pharmpy/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.847404 pharmpy-core-0.93.0/src/pharmpy/plugins/fcon/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/fcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/fcon/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.847404 pharmpy-core-0.93.0/src/pharmpy/plugins/nlmixr/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nlmixr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nlmixr/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nlmixr/ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23568 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nlmixr/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nlmixr/model_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nlmixr/name_mangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nlmixr/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nlmixr/sanity_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.851404 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/advan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14797 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/nmtran_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28069 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.851404 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/abbreviated_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/code_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/data_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/estimation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/etas_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.851404 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/code_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/data_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/definitions.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/option_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/problem_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/model_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17573 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/omega_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/option_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/problem_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/raw_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/simulation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/sizes_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/subroutine_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/table_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/theta_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20153 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/results_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7135 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63905 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.851404 pharmpy-core-0.93.0/src/pharmpy/plugins/rxode/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/rxode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/rxode/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/plugins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.855404 pharmpy-core-0.93.0/src/pharmpy/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/reporting/altairplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/reporting/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/reporting/custom.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5562 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/reporting/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.855404 pharmpy-core-0.93.0/src/pharmpy/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.855404 pharmpy-core-0.93.0/src/pharmpy/tools/allometry/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/allometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/allometry/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.855404 pharmpy-core-0.93.0/src/pharmpy/tools/amd/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/amd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/amd/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/amd/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16039 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/amd/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.855404 pharmpy-core-0.93.0/src/pharmpy/tools/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/bootstrap/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/bootstrap/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/bootstrap/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.855404 pharmpy-core-0.93.0/src/pharmpy/tools/cdd/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/cdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/cdd/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.855404 pharmpy-core-0.93.0/src/pharmpy/tools/covsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/covsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/covsearch/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/covsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.855404 pharmpy-core-0.93.0/src/pharmpy/tools/crossval/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/crossval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/crossval/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.855404 pharmpy-core-0.93.0/src/pharmpy/tools/estmethod/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/estmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/estmethod/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/estmethod/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/estmethod/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.855404 pharmpy-core-0.93.0/src/pharmpy/tools/evaldesign/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/evaldesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/evaldesign/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.855404 pharmpy-core-0.93.0/src/pharmpy/tools/frem/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/frem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/frem/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/frem/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    38407 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/frem/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/frem/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.855404 pharmpy-core-0.93.0/src/pharmpy/tools/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/funcs/ml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.859404 pharmpy-core-0.93.0/src/pharmpy/tools/funcs/ml_models/
+-rw-r--r--   0 runner    (1001) docker     (123)    91484 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)    93596 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/funcs/summarize_individuals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.859404 pharmpy-core-0.93.0/src/pharmpy/tools/iivsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/iivsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/iivsearch/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/iivsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.859404 pharmpy-core-0.93.0/src/pharmpy/tools/iovsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/iovsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/iovsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.859404 pharmpy-core-0.93.0/src/pharmpy/tools/linearize/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/linearize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/linearize/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/linearize/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.859404 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.859404 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/feature/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/feature/covariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/feature/elimination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/feature/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/feature/lagtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/feature/peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/feature/transits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.859404 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.859404 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/covariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/elimination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/lagtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/transits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/mfl/stringify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.863404 pharmpy-core-0.93.0/src/pharmpy/tools/modelfit/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/modelfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/modelfit/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/modelfit/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.863404 pharmpy-core-0.93.0/src/pharmpy/tools/modelsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/modelsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/modelsearch/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/modelsearch/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/psn_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.863404 pharmpy-core-0.93.0/src/pharmpy/tools/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/qa/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/rankfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31937 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.863404 pharmpy-core-0.93.0/src/pharmpy/tools/ruvsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/ruvsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/ruvsearch/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16608 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/ruvsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.863404 pharmpy-core-0.93.0/src/pharmpy/tools/scm/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/scm/psn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/scm/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.863404 pharmpy-core-0.93.0/src/pharmpy/tools/simeval/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/simeval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/simeval/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.863404 pharmpy-core-0.93.0/src/pharmpy/tools/simfit/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/simfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/simfit/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/tools/wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.863404 pharmpy-core-0.93.0/src/pharmpy/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.863404 pharmpy-core-0.93.0/src/pharmpy/workflows/dispatchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/dispatchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/dispatchers/local_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.863404 pharmpy-core-0.93.0/src/pharmpy/workflows/model_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/model_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/model_database/baseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/model_database/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/model_database/null_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.863404 pharmpy-core-0.93.0/src/pharmpy/workflows/tool_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/tool_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/tool_database/baseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/tool_database/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/tool_database/null_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/src/pharmpy/workflows/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.867404 pharmpy-core-0.93.0/src/pharmpy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46471 2023-04-19 08:41:17.000000 pharmpy-core-0.93.0/src/pharmpy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    46649 2023-04-19 08:41:17.000000 pharmpy-core-0.93.0/src/pharmpy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:41:17.000000 pharmpy-core-0.93.0/src/pharmpy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-19 08:41:17.000000 pharmpy-core-0.93.0/src/pharmpy_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:36:06.000000 pharmpy-core-0.93.0/src/pharmpy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-19 08:41:17.000000 pharmpy-core-0.93.0/src/pharmpy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 08:41:17.000000 pharmpy-core-0.93.0/src/pharmpy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.867404 pharmpy-core-0.93.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.867404 pharmpy-core-0.93.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/cli/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.867404 pharmpy-core-0.93.0/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.867404 pharmpy-core-0.93.0/tests/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/deps/test_deps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.867404 pharmpy-core-0.93.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/integration/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/integration/test_amd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/integration/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/integration/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/integration/test_covsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/integration/test_estmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/integration/test_evaldesign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/integration/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/integration/test_iivsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/integration/test_iovsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/integration/test_modelsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/integration/test_resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/integration/test_ruvsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.867404 pharmpy-core-0.93.0/tests/internals/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.867404 pharmpy-core-0.93.0/tests/internals/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/internals/fs/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/internals/fs/test_tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.867404 pharmpy-core-0.93.0/tests/internals/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/internals/module/test_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/internals/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/internals/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.867404 pharmpy-core-0.93.0/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/model/test_datainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/model/test_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/model/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27417 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/model/test_random_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/model/test_statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.875404 pharmpy-core-0.93.0/tests/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_add_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_basic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_block_rvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_blq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_compartments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_data_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_estimation_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_eta_additions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_eta_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_has_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_metabolite.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100179 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_parameter_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_remove_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_tmdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/modeling/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.875404 pharmpy-core-0.93.0/tests/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.875404 pharmpy-core-0.93.0/tests/nonmem/output/
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/output/test_nonmem_results_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.875404 pharmpy-core-0.93.0/tests/nonmem/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/test_abbreviated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/test_estimation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/test_etas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/test_model_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/test_omega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/test_option_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/test_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/test_subroutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/records/test_theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/test_advan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/test_des.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/test_fcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/test_modelfit_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35592 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/test_nonmem_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/test_nonmem_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/nonmem/test_read.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.875404 pharmpy-core-0.93.0/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/plugins/test_nlmixr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/plugins/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.879404 pharmpy-core-0.93.0/tests/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.879404 pharmpy-core-0.93.0/tests/testdata/frem/
+-rw-r--r--   0 runner    (1001) docker     (123)    52275 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/frem/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.887404 pharmpy-core-0.93.0/tests/testdata/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/DDMODEL00000130
+-rw-r--r--   0 runner    (1001) docker     (123)    59142 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.887404 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.887404 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.895405 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22454 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/skipped_individuals1.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.895405 pharmpy-core-0.93.0/tests/testdata/nonmem/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/errors/control_stream_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/errors/est_step_warning.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/errors/no_header_error.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/errors/no_header_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/errors/rounding_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/errors/run_interrupted.ext
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/errors/run_interrupted.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/errors/zero_gradient_error.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.895405 pharmpy-core-0.93.0/tests/testdata/nonmem/fcon/
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/fcon/FCON
+-rw-r--r--   0 runner    (1001) docker     (123)    39432 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/fcon/FDATA
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/file.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.823403 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.895405 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/
+-rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.899405 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/
+-rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.823403 pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.899405 pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.899405 pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/minimal.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.823403 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.899405 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/covariance/
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.823403 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/multPROB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.823403 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.899405 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91887 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.823403 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.823403 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.899405 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    59168 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov
+-rw-r--r--   0 runner    (1001) docker     (123)   115118 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    82511 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    75841 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.903405 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.823403 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.903405 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    26695 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17548 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    16143 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.907405 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)   178666 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext
+-rw-r--r--   0 runner    (1001) docker     (123)  1091059 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.907405 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/simfit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    38485 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.907405 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_1transit.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_2transits.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan11.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan12.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.915405 pharmpy-core-0.93.0/tests/testdata/nonmem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/fviii6.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/fviii6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/fviii6.prn
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_2comp.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_2comp.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21336 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_2comp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_2comp.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_2comp.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   175384 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_simulated_log.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   185992 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_simulated_normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)   105888 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/mytab_mox2
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pef.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pef.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_advan3_trans1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_dvid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_dvid.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_noifs.coi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_noifs.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_noifs.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_noifs.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_noifs.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_noifs.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_noifs.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_trans1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_trans1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_trans1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_trans1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_abbr.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_abbr_comments.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_block.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_clashing_symbols.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_etas.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_nm750.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36053 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_rate.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.coi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.tab
+-rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real_linbase.tab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.919405 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)   370034 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/add_etas_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/add_etas_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/add_etas_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/add_etas_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/boxcox.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/boxcox.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/boxcox.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/boxcox.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/cdd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/fullblock.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/fullblock.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/fullblock.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/fullblock.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/iov.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/iov.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/iov.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/iov.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   262826 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/pheno_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/pheno_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/pheno_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/pheno_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/pheno_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/resmod_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/scm_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   392990 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/simeval_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/tdist.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/tdist.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/tdist.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/qa/tdist.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.919405 pharmpy-core-0.93.0/tests/testdata/nonmem/ruvsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/ruvsearch/mox3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/ruvsearch/mox3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/ruvsearch/mox3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/ruvsearch/mox3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   276902 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   180553 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/ruvsearch/mytab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.919405 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.919405 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/backward_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/backward_dir1/config_fake.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.919405 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/gofofv_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/localmin.logf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.919405 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/log_steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/log_steps/backward_pval_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/log_steps/backward_pval_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/log_steps/forward_pval_4.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.919405 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/mergeofv_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/mergeofv_dir1/config_havebaserun.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.919405 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/mergeofv_dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/mergeofv_dir2/config_havebaserun.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.923405 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/onlyforward_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/onlyforward_dir1/config_normal.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.923405 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.923405 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/scmplus_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   108031 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/sdtab1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.923405 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/pheno.cov
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/pheno_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.827403 pharmpy-core-0.93.0/tests/testdata/psn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.923405 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/est_data0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/est_data1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/est_data2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/est_data3.dta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.931405 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/pred_data0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/pred_data1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/pred_data2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/pred_data3.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/xv_result.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.931405 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/covariates_summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.931405 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/final_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/frem_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.935405 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    93135 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_1b.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_2.cor
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/proposal_density.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.935405 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/command.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.935405 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/linearize_run/
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/linearize_run/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.939405 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   137744 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table
+-rw-r--r--   0 runner    (1001) docker     (123)   316422 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/results_summary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.939405 pharmpy-core-0.93.0/tests/testdata/psn/resmod_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/resmod_dir1/resmod_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.939405 pharmpy-core-0.93.0/tests/testdata/psn/resmod_dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/resmod_dir2/resmod_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.939405 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.947405 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)    63331 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/original.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/original.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/original.ext
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/original.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/original.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    54391 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    21489 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.951406 pharmpy-core-0.93.0/tests/testdata/results/
+-rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/allometry_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   263999 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/amd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   130598 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/bootstrap_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/cdd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1360720 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/covsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/estmethod_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205797 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/iivsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197228 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/iovsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/linearize_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)   105603 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/modelsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/qa_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57352 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/ruvsearch_results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.827403 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.951406 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.951406 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.951406 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.827403 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.951406 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/input_model.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   183701 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:37:23.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.951406 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.951406 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.951406 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.951406 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91188 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.955406 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.955406 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91119 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.955406 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.955406 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53630 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91754 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.955406 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.959406 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91879 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout
+-rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   105597 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.959406 pharmpy-core-0.93.0/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_amd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_cdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_covsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_crossval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_estmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27814 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_frem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_iivsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_iovsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_linearize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_mfl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_modelfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_modelsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_rankfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_runtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_ruvsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_simeval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_start_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_summarize_individuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/tools/test_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:41:17.959406 pharmpy-core-0.93.0/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/workflows/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/workflows/test_execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/workflows/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/workflows/test_model_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/workflows/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/workflows/test_tool_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tests/workflows/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-19 08:33:51.000000 pharmpy-core-0.93.0/tox.ini
```

### Comparing `pharmpy-core-0.92.0/AUTHORS.rst` & `pharmpy-core-0.93.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/CHANGELOG.rst` & `pharmpy-core-0.93.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+0.93.0 (2023-04-19)
+-------------------
+
+New features
+============
+
+* Add function ``modeling.get_zero_order_inputs``
+* Add function ``modeling.set_zero_order_input``
+* Add function ``modeling.set_tmdd``
+* Added plugin to convert models to RxODE
+* Support conversion of more models to nlmixr
+
+Changes
+=======
+
+* ``modeling.generate_model_code`` was renamed to ``modeling.get_model_code`` since the code is not generated by this function
+* Do not use ADVAN7 because models that should work with ADVAN7 didn't were found
+
+Bugfixes
+========
+
+* Fix multiple bugs in parsing $TABLE headers
+
 0.92.0 (2023-04-05)
 -------------------
 
 New features
 ============
 
 * Add function ``modeling.is_linearized``
```

### Comparing `pharmpy-core-0.92.0/CODE_OF_CONDUCT.rst` & `pharmpy-core-0.93.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/LICENSE` & `pharmpy-core-0.93.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/LICENSE.LESSER` & `pharmpy-core-0.93.0/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/MANIFEST.in` & `pharmpy-core-0.93.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/PKG-INFO` & `pharmpy-core-0.93.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmpy-core
-Version: 0.92.0
+Version: 0.93.0
 Summary: Pharmacometric modeling
 Home-page: https://pharmpy.github.io
 Author: Rikard Nordgren
 Author-email: rikard.nordgren@farmaci.uu.se
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Bug Tracker, https://github.com/pharmpy/pharmpy/issues
 Project-URL: Source Code, https://github.com/pharmpy/pharmpy
@@ -41,14 +41,37 @@
 * A model abstraction as a foundation for higher level operations on models
 * Functions for manipulation of models, e.g. changing model components like elimination or absorption
 * Reading NONMEM models and results
 * Running models and complex workflows (with NONMEM or to some extent nlmixr)
 
 This is the `team behind Pharmpy <https://pharmpy.github.io/latest/contributors.html>`_
 
+0.93.0 (2023-04-19)
+-------------------
+
+New features
+============
+
+* Add function ``modeling.get_zero_order_inputs``
+* Add function ``modeling.set_zero_order_input``
+* Add function ``modeling.set_tmdd``
+* Added plugin to convert models to RxODE
+* Support conversion of more models to nlmixr
+
+Changes
+=======
+
+* ``modeling.generate_model_code`` was renamed to ``modeling.get_model_code`` since the code is not generated by this function
+* Do not use ADVAN7 because models that should work with ADVAN7 didn't were found
+
+Bugfixes
+========
+
+* Fix multiple bugs in parsing $TABLE headers
+
 0.92.0 (2023-04-05)
 -------------------
 
 New features
 ============
 
 * Add function ``modeling.is_linearized``
```

### Comparing `pharmpy-core-0.92.0/README.rst` & `pharmpy-core-0.93.0/README.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/NONMEM.rst` & `pharmpy-core-0.93.0/docs/NONMEM.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/Pharmpy_logo.svg` & `pharmpy-core-0.93.0/docs/Pharmpy_logo.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/Pharmpy_logo_dark.svg` & `pharmpy-core-0.93.0/docs/Pharmpy_logo_dark.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/_ext/conversion.py` & `pharmpy-core-0.93.0/docs/_ext/conversion.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/_ext/pharmpy_snippet.py` & `pharmpy-core-0.93.0/docs/_ext/pharmpy_snippet.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/allometry.rst` & `pharmpy-core-0.93.0/docs/allometry.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/amd.rst` & `pharmpy-core-0.93.0/docs/amd.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/api.rst` & `pharmpy-core-0.93.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/bootstrap.rst` & `pharmpy-core-0.93.0/docs/bootstrap.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/cdd.rst` & `pharmpy-core-0.93.0/docs/cdd.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/cli.rst` & `pharmpy-core-0.93.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/conf.py` & `pharmpy-core-0.93.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'Pharmpy'
 year = '2018-2023'
 authors = ['the Pharmpy development team']
 copyright = '{0}; {1}'.format(year, ', '.join(authors))
-version = release = '0.92.0'
+version = release = '0.93.0'
 html_show_sourcelink = False
 
 pygments_style = 'trac'
 templates_path = ['.']
 
 html_static_path = ['.']
 html_theme = "pydata_sphinx_theme"
```

### Comparing `pharmpy-core-0.92.0/docs/configuration.rst` & `pharmpy-core-0.93.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/contribute.rst` & `pharmpy-core-0.93.0/docs/contribute.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/covsearch.rst` & `pharmpy-core-0.93.0/docs/covsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/crossval.rst` & `pharmpy-core-0.93.0/docs/crossval.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/custom.css` & `pharmpy-core-0.93.0/docs/custom.css`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/data.rst` & `pharmpy-core-0.93.0/docs/data.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/design.rst` & `pharmpy-core-0.93.0/docs/design.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/estmethod.rst` & `pharmpy-core-0.93.0/docs/estmethod.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/frem.rst` & `pharmpy-core-0.93.0/docs/frem.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/getting_started.rst` & `pharmpy-core-0.93.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/help_functions.py` & `pharmpy-core-0.93.0/docs/help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/iivsearch.rst` & `pharmpy-core-0.93.0/docs/iivsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/images/Pharmpy_symbol.svg` & `pharmpy-core-0.93.0/docs/images/Pharmpy_symbol.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/images/tools.png` & `pharmpy-core-0.93.0/docs/images/tools.png`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/index.rst` & `pharmpy-core-0.93.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/iovsearch.rst` & `pharmpy-core-0.93.0/docs/iovsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/license.rst` & `pharmpy-core-0.93.0/docs/license.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/linearize.rst` & `pharmpy-core-0.93.0/docs/linearize.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/model.rst` & `pharmpy-core-0.93.0/docs/model.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/modelfit.rst` & `pharmpy-core-0.93.0/docs/modelfit.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/modeling.rst` & `pharmpy-core-0.93.0/docs/modeling.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/modelsearch.rst` & `pharmpy-core-0.93.0/docs/modelsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/nonmem_plugin.rst` & `pharmpy-core-0.93.0/docs/nonmem_plugin.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/pharmr_logo.svg` & `pharmpy-core-0.93.0/docs/pharmr_logo.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/plots.rst` & `pharmpy-core-0.93.0/docs/plots.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/plugins.rst` & `pharmpy-core-0.93.0/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/projects.rst` & `pharmpy-core-0.93.0/docs/projects.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/qa.rst` & `pharmpy-core-0.93.0/docs/qa.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/ruvsearch.rst` & `pharmpy-core-0.93.0/docs/ruvsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/scm.rst` & `pharmpy-core-0.93.0/docs/scm.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/simeval.rst` & `pharmpy-core-0.93.0/docs/simeval.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/tools.rst` & `pharmpy-core-0.93.0/docs/tools.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/docs/using_r.rst` & `pharmpy-core-0.93.0/docs/using_r.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/requirements.txt` & `pharmpy-core-0.93.0/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 alabaster==0.7.13
 altair==4.2.2
 appdirs==1.4.4
 asttokens==2.2.1
-attrs==22.2.0
+attrs==23.1.0
 Babel==2.12.1
 backcall==0.2.0
-beautifulsoup4==4.12.0
+beautifulsoup4==4.12.2
 bleach==6.0.0
 certifi==2022.12.7
 charset-normalizer==3.1.0
 click==8.1.3
 cloudpickle==2.2.1
 comm==0.1.3
 commonmark==0.9.1
 csscompressor==0.9.5
-dask==2023.3.2
-debugpy==1.6.6
+dask==2023.4.0
+debugpy==1.6.7
 decorator==5.1.1
 defusedxml==0.7.1
-distributed==2023.3.2
+distributed==2023.4.0
 docutils==0.19.0
 entrypoints==0.4
 executing==1.2.0
 fastjsonschema==2.16.3
-fsspec==2023.3.0
+fsspec==2023.4.0
 HeapDict==1.0.1
 idna==3.4
 imagesize==1.4.1
-importlib_metadata==6.1.0
+importlib_metadata==6.5.0
 ipykernel==6.22.0
 ipython==8.12.0
 ipywidgets==8.0.6
 jedi==0.18.2
 Jinja2==3.1.2
 jsonschema==4.17.3
 jupyter-client==7.3.4
@@ -44,67 +44,67 @@
 lxml==4.9.2
 MarkupSafe==2.1.2
 matplotlib-inline==0.1.6
 mistune==2.0.5
 mpmath==1.3.0
 msgpack==1.0.5
 nbclient==0.7.3
-nbconvert==7.3.0
+nbconvert==7.3.1
 nbformat==5.8.0
 nest-asyncio==1.5.6
 networkx==3.1
 numexpr==2.8.4
 numpy==1.24.2
-packaging==23.0
+packaging==23.1
 pandas==1.5.3
 pandocfilters==1.5.0
 parso==0.8.3
-partd==1.3.0
+partd==1.4.0
 pexpect==4.8.0
 pickleshare==0.7.5
 platformdirs==3.2.0
 prompt-toolkit==3.0.38
-psutil==5.9.4
+psutil==5.9.5
 ptyprocess==0.7.0
 pure-eval==0.2.2
-Pygments==2.14.0
+Pygments==2.15.1
 pyreadr==0.4.7
 pyrsistent==0.19.3
 python-dateutil==2.8.2
 pytz==2023.3
 pywin32>=302,!=304; sys_platform == 'win32' and platform_python_implementation != 'PyPy'
 PyYAML==6.0
 requests==2.28.2
 pyzmq==25.0.2
-rich==13.3.3
+rich==13.3.4
 scipy==1.10.1
 six==1.16.0
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
-soupsieve==2.4
+soupsieve==2.4.1
 Sphinx==6.1.3
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 sphinxcontrib.applehelp==1.0.4
 stack-data==0.6.2
 symengine==0.10.0
 sympy==1.11.1
 tblib==1.7.0
 tinycss2==1.2.1
 toolz==0.12.0
-tornado==6.1
+tornado==6.3
 traitlets==5.9.0
 urllib3==1.26.15
 wcwidth==0.2.6
 webencodings==0.5.1
 widgetsnbextension==4.0.7
-zict==2.2.0
+zict==3.0.0
 zipp==3.15.0
 tflite-runtime==2.11.0; sys_platform == 'linux' and python_version == '3.8'
 tflite-runtime==2.11.0; sys_platform == 'linux' and python_version == '3.9'
 tflite-runtime==2.5.0; sys_platform == 'darwin' and python_version == '3.8'
 tflite_runtime @ https://github.com/hjonnala/snippets/raw/main/wheels/python3.10/tflite_runtime-2.5.0.post1-cp310-cp310-linux_x86_64.whl ; sys_platform == 'linux' and python_version == '3.10'
 --extra-index-url https://google-coral.github.io/py-repo/
 tflite_runtime==2.5.0.post1; sys_platform == 'darwin' and python_version == '3.9'
```

### Comparing `pharmpy-core-0.92.0/setup.cfg` & `pharmpy-core-0.93.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/setup.py` & `pharmpy-core-0.93.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     txt = re.compile(pat, re.MULTILINE | re.DOTALL).findall(text_str)
     txt = [dedent(block).strip() for block in txt]
     return '\n\n'.join(txt)
 
 
 setup(
     name='pharmpy-core',
-    version='0.92.0',
+    version='0.93.0',
     license='GNU Lesser General Public License v3 (LGPLv3)',
     description='Pharmacometric modeling',
     long_description='%s\n\n%s'
     % (strip_refs(longdesc(read('README.rst'))), strip_refs(read('CHANGELOG.rst'))),
     author='Rikard Nordgren',
     author_email='rikard.nordgren@farmaci.uu.se',
     url='https://pharmpy.github.io',
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/cli.py` & `pharmpy-core-0.93.0/src/pharmpy/cli.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/config.py` & `pharmpy-core-0.93.0/src/pharmpy/config.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/deps/__init__.py` & `pharmpy-core-0.93.0/src/pharmpy/deps/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/deps/altair.py` & `pharmpy-core-0.93.0/src/pharmpy/deps/altair.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/df.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/df.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/ds/ordered_set.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/ds/ordered_set.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/expr/eval.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/expr/eval.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/expr/funcs.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/expr/funcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/expr/leaves.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/expr/leaves.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/expr/ode.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/expr/ode.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/expr/subs.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/expr/subs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/expr/tree.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/expr/tree.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/expr/units.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/expr/units.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/fn/signature.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/fn/signature.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/fn/type.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/fn/type.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/fs/lock.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/fs/lock.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/fs/path.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/fs/path.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/fs/tmp.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/fs/tmp.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/graph/directed/connected_components.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/graph/directed/connected_components.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/immutable.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/immutable.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/math.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/module/lazy.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/module/lazy.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/parse/generic.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/parse/generic.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/parse/ignored.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/parse/ignored.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/parse/missing.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/parse/missing.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/parse/prettyprint.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/parse/prettyprint.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/parse/tree.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/parse/tree.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/parse/treeprint.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/parse/treeprint.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/sequence/lcs.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/sequence/lcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/set/partitions.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/set/partitions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/set/subsets.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/set/subsets.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/internals/unicode.py` & `pharmpy-core-0.93.0/src/pharmpy/internals/unicode.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/model/__init__.py` & `pharmpy-core-0.93.0/src/pharmpy/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/model/data.py` & `pharmpy-core-0.93.0/src/pharmpy/model/data.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/model/datainfo.py` & `pharmpy-core-0.93.0/src/pharmpy/model/datainfo.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/model/distributions/numeric.py` & `pharmpy-core-0.93.0/src/pharmpy/model/distributions/numeric.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/model/distributions/symbolic.py` & `pharmpy-core-0.93.0/src/pharmpy/model/distributions/symbolic.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/model/estimation.py` & `pharmpy-core-0.93.0/src/pharmpy/model/estimation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/model/model.py` & `pharmpy-core-0.93.0/src/pharmpy/model/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/model/parameters.py` & `pharmpy-core-0.93.0/src/pharmpy/model/parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/model/random_variables.py` & `pharmpy-core-0.93.0/src/pharmpy/model/random_variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from collections.abc import Container as CollectionsContainer
 from collections.abc import Sequence as CollectionsSequence
 from itertools import chain, product
 from typing import Container, Dict, Iterable, List, Optional, Sequence, Set, Tuple, Union, overload
 
 from pharmpy.deps import numpy as np
-from pharmpy.deps import symengine, sympy
+from pharmpy.deps import symengine, sympy, sympy_stats
 from pharmpy.internals.expr.eval import eval_expr
 from pharmpy.internals.expr.parse import parse as parse_expr
 from pharmpy.internals.expr.subs import subs, xreplace_dict
 from pharmpy.internals.immutable import Immutable
 from pharmpy.internals.math import cov2corr, is_positive_semidefinite, nearest_postive_semidefinite
 
 from .distributions.numeric import NumericDistribution
@@ -789,18 +789,47 @@
         """
         _, dist_input = self._lookup_rv(rv)
 
         rvs = [dist for dist in self if dist.variance == dist_input.variance]
 
         return RandomVariables.create(rvs)
 
+    def replace_with_sympy_rvs(self, expr):
+        """Replaces Pharmpy RVs in a Sympy expression with Sympy RVs
+
+        Takes a Sympy expression and replaces all RVs with Sympy RVs, resulting expression
+        can be used in different Sympy functions (e.g. sympy.stats.std())
+
+        Parameters
+        ----------
+        expr : sympy.Expr
+            Expression which will get RVs replaced
+
+        Returns
+        -------
+        sympy.Expr
+            Expression with replaced RVs
+        """
+        rvs_in_expr = {self[rv] for rv in expr.free_symbols.intersection(self.free_symbols)}
+        subs_dict = {}
+        for i, rv in enumerate(rvs_in_expr):
+            if isinstance(rv, JointNormalDistribution):
+                # sympy.stats.MultivariateNormal uses variance, sympy.stats.Normal takes std
+                dist = sympy.stats.MultivariateNormal(f'__rv{i}', rv.mean, rv.variance)
+                for j in range(0, len(rv.names)):
+                    subs_dict[rv.names[j]] = dist[j]
+            else:
+                subs_dict[rv.names[0]] = sympy_stats.Normal(
+                    f'__rv{i}', rv.mean, sympy.sqrt(rv.variance)
+                )
+        return expr.subs(subs_dict)
+
 
 def _sample_from_distributions(distributions, expr, parameters, nsamples, rng):
     random_variable_symbols = expr.free_symbols.difference(parameters.keys())
-    print(random_variable_symbols)
     filtered_distributions = filter_distributions(distributions, random_variable_symbols)
     sampling_rvs = subs_distributions(filtered_distributions, parameters)
     sampled_expr = subs(expr, parameters, simultaneous=True)
     return sample_expr_from_rvs(sampling_rvs, sampled_expr, nsamples, rng)
 
 
 def filter_distributions(
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/model/results.py` & `pharmpy-core-0.93.0/src/pharmpy/model/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/model/statements.py` & `pharmpy-core-0.93.0/src/pharmpy/model/statements.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,14 +367,34 @@
             The new updated compartment
         """
         new_comp = compartment.replace(bioavailability=bioavailability)
         mapping = {compartment: new_comp}
         nx.relabel_nodes(self._g, mapping, copy=False)
         return new_comp
 
+    def set_input(self, compartment, input):
+        """Set zero order input of compartment
+
+        Parameters
+        ----------
+        compartment : Compartment
+            Compartment for which to change zero order input
+        input : expr
+            New input
+
+        Returns
+        -------
+        Compartment
+            The new updated compartment
+        """
+        new_comp = compartment.replace(input=input)
+        mapping = {compartment: new_comp}
+        nx.relabel_nodes(self._g, mapping, copy=False)
+        return new_comp
+
 
 def _is_positive(expr: sympy.Expr) -> bool:
     return sympy.ask(
         sympy.Q.positive(expr), assume_all(sympy.Q.positive, free_images_and_symbols(expr))
     )
 
 
@@ -1006,49 +1026,39 @@
             a = list(x)
             if output in a:
                 a.remove(output)
             a = sorted(a, key=lambda x: x.name)
             return iter(a)
 
         nodes = list(nx.bfs_tree(self._g, dosecmt, sort_neighbors=sortfunc))
+
+        remaining = set(self._g.nodes) - {output} - set(nodes)
+        if remaining:  # Disjoint graph
+            # Start with the one compartment having a zero order input (target for TMDD)
+            for comp in remaining:
+                if comp.input != 0:
+                    break
+            ordered_remaining = list(nx.bfs_tree(self._g, comp, sort_neighbors=sortfunc))
+            nodes += ordered_remaining
         return nodes
 
     @property
     def zero_order_inputs(self):
         """Vector of all zero order inputs to each compartment
 
         Example
         -------
         >>> from pharmpy.modeling import load_example_model, set_zero_order_absorption
         >>> import sympy
         >>> model = load_example_model("pheno")
         >>> sympy.pprint(model.statements.ode_system.zero_order_inputs)
         [0]
-        >>> model = set_zero_order_absorption(model)    # doctest: +ELLIPSIS
-        >>> sympy.pprint(model.statements.ode_system.zero_order_inputs)
-                ⎡⎧AMT            ⎤
-                ⎢⎪───  for D₁ > t⎥
-                ⎢⎨ D₁            ⎥
-                ⎢⎪               ⎥
-                ⎣⎩ 0   otherwise ⎦
 
         """
-        inputs = []
-        for node in self._order_compartments():  # self._g.nodes:
-            if node.dose is not None and isinstance(node.dose, Infusion):
-                if node.dose.rate is not None:
-                    expr = node.dose.rate
-                    cond = node.dose.amount / node.dose.rate
-                else:
-                    expr = node.dose.amount / node.dose.duration
-                    cond = node.dose.duration
-                infusion_func = sympy.Piecewise((expr, self.t < cond), (0, True))
-                inputs.append(infusion_func)
-            else:
-                inputs.append(0)
+        inputs = [node.input for node in self._order_compartments()]
         return sympy.Matrix(inputs)
 
     def __len__(self):
         """The number of compartments"""
         return len(self._g.nodes) - 1
 
     def _repr_html_(self):
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/__init__.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from .basic_models import create_basic_pk_model
 from .block_rvs import create_joint_distribution, split_joint_distribution
 from .blq import transform_blq
 from .common import (
     bump_model_number,
     convert_model,
     create_config_template,
-    generate_model_code,
     get_config_path,
+    get_model_code,
     get_model_covariates,
     load_example_model,
     print_model_code,
     print_model_symbols,
     read_model,
     read_model_from_string,
     remove_unused_parameters_and_rvs,
@@ -125,14 +125,15 @@
     add_individual_parameter,
     add_lag_time,
     add_peripheral_compartment,
     display_odes,
     find_clearance_parameters,
     find_volume_parameters,
     get_initial_conditions,
+    get_zero_order_inputs,
     has_first_order_elimination,
     has_linear_odes,
     has_linear_odes_with_real_eigenvalues,
     has_michaelis_menten_elimination,
     has_mixed_mm_fo_elimination,
     has_odes,
     has_zero_order_absorption,
@@ -147,14 +148,15 @@
     set_mixed_mm_fo_elimination,
     set_ode_solver,
     set_peripheral_compartments,
     set_seq_zo_fo_absorption,
     set_transit_compartments,
     set_zero_order_absorption,
     set_zero_order_elimination,
+    set_zero_order_input,
     solve_ode_system,
 )
 from .parameter_sampling import (
     create_rng,
     sample_individual_estimates,
     sample_parameters_from_covariance_matrix,
     sample_parameters_uniformly,
@@ -188,14 +190,15 @@
     calculate_eta_shrinkage,
     calculate_individual_parameter_statistics,
     calculate_individual_shrinkage,
     calculate_pk_parameters_statistics,
     check_high_correlations,
     check_parameters_near_bounds,
 )
+from .tmdd import set_tmdd
 from .units import get_unit_of
 from .update_inits import update_initial_individual_estimates, update_inits
 from .write_csv import write_csv
 
 # Must be set directly, otherwise errors about unused imports
 __all__ = [
     'add_allometry',
@@ -254,15 +257,14 @@
     'evaluate_weighted_residuals',
     'expand_additional_doses',
     'find_clearance_parameters',
     'find_volume_parameters',
     'fix_or_unfix_parameters',
     'fix_parameters',
     'fix_parameters_to',
-    'generate_model_code',
     'get_baselines',
     'get_bioavailability',
     'get_cmt',
     'get_concentration_parameters_from_data',
     'get_config_path',
     'get_covariate_baselines',
     'get_doses',
@@ -271,27 +273,29 @@
     'get_evid',
     'get_ids',
     'get_individual_parameters',
     'get_individual_prediction_expression',
     'get_initial_conditions',
     'get_lag_times',
     'get_mdv',
+    'get_model_code',
     'get_model_covariates',
     'get_number_of_individuals',
     'get_number_of_observations',
     'get_number_of_observations_per_individual',
     'get_omegas',
     'get_observations',
     'get_observation_expression',
     'get_pk_parameters',
     'get_population_prediction_expression',
     'get_rv_parameters',
     'get_sigmas',
     'get_thetas',
     'get_unit_of',
+    'get_zero_order_inputs',
     'greekify_model',
     'has_additive_error_model',
     'has_combined_error_model',
     'has_covariate_effect',
     'has_first_order_elimination',
     'has_linear_odes',
     'has_linear_odes_with_real_eigenvalues',
@@ -353,18 +357,20 @@
     'set_name',
     'set_ode_solver',
     'set_peripheral_compartments',
     'set_power_on_ruv',
     'set_proportional_error_model',
     'set_seq_zo_fo_absorption',
     'set_time_varying_error_model',
+    'set_tmdd',
     'set_transit_compartments',
     'set_weighted_error_model',
     'set_zero_order_absorption',
     'set_zero_order_elimination',
+    'set_zero_order_input',
     'simplify_expression',
     'solve_ode_system',
     'split_joint_distribution',
     'transform_blq',
     'transform_etas_boxcox',
     'transform_etas_john_draper',
     'transform_etas_tdist',
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/allometry.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/basic_models.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/basic_models.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/block_rvs.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/block_rvs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/blq.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/blq.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+"""
+:meta private:
+"""
 from typing import Optional
 
 from pharmpy.deps import sympy
 from pharmpy.internals.expr.funcs import PHI
 from pharmpy.model import Assignment, EstimationSteps, JointNormalDistribution, Model
 
 from .data import remove_loq_data
-from .error import has_additive_error_model, has_combined_error_model, has_proportional_error_model
-from .expressions import create_symbol
+from .expressions import create_symbol, simplify_expression
 
 SUPPORTED_METHODS = frozenset(['m1', 'm3', 'm4'])
 
 
 def transform_blq(model: Model, method: str = 'm4', lloq: Optional[float] = None):
     """Transform for BLQ data
 
@@ -83,105 +85,115 @@
     model = model.replace(estimation_steps=est_steps_new)
 
     # FIXME: handle other DVs?
     y_symb = list(model.dependent_variables.keys())[0]
     y = sset.find_assignment(y_symb)
     ipred = y.expression.subs({rv: 0 for rv in model.random_variables.epsilons.names})
 
+    blq_symb, blq_type = get_blq_symb_and_type(model)
     if isinstance(lloq, float):
-        symb_lloq = create_symbol(model, 'LLOQ')
-        lloq_type = 'lloq'
-    else:
-        try:
-            lloq_datainfo = model.datainfo.typeix['blq']
-            lloq_type = 'blq'
-        except IndexError:
-            lloq_datainfo = model.datainfo.typeix['lloq']
-            lloq_type = 'lloq'
-        if len(lloq_datainfo.names) > 1:
-            raise ValueError(f'Can only have one of column type: {lloq_datainfo}')
-        symb_lloq = sympy.Symbol(lloq_datainfo[0].name)
+        blq_symb = create_symbol(model, blq_symb)
 
-    sd_assignments, symb_sd = _weight_as_sd(model, y, ipred)
+    sd = _get_sd(model, y)
     symb_dv = sympy.Symbol(model.datainfo.dv_column.name)
     symb_fflag = create_symbol(model, 'F_FLAG')
     symb_cumd = create_symbol(model, 'CUMD')
 
-    if lloq_type == 'lloq':
-        is_above_lloq = sympy.GreaterThan(symb_dv, symb_lloq)
+    if blq_type == 'lloq':
+        is_above_lloq = sympy.GreaterThan(symb_dv, blq_symb)
     else:
-        is_above_lloq = sympy.Equality(symb_lloq, 1)
+        is_above_lloq = sympy.Equality(blq_symb, 1)
 
-    assignments = sd_assignments
+    assignments = [sd]
 
     if isinstance(lloq, float):
-        lloq = Assignment(symb_lloq, sympy.Float(lloq))
+        lloq = Assignment(blq_symb, sympy.Float(lloq))
         assignments.append(lloq)
 
     assignments += Assignment(symb_fflag, sympy.Piecewise((0, is_above_lloq), (1, True)))
 
-    cumd = Assignment(symb_cumd, PHI((symb_lloq - ipred) / symb_sd))
+    cumd = Assignment(symb_cumd, PHI((blq_symb - ipred) / sd.symbol))
     if method == 'm3':
         assignments += Assignment(
             y.symbol, sympy.Piecewise((y.expression, is_above_lloq), (cumd.expression, True))
         )
     else:
         assignments += cumd
         symb_cumdz = create_symbol(model, 'CUMDZ')
-        assignments += Assignment(symb_cumdz, PHI(-ipred / symb_sd))
+        assignments += Assignment(symb_cumdz, PHI(-ipred / sd.symbol))
 
         y_below_lloq = (symb_cumd - symb_cumdz) / (1 - symb_cumdz)
         assignments += Assignment(
             y.symbol, sympy.Piecewise((y.expression, is_above_lloq), (y_below_lloq, True))
         )
 
     y_idx = sset.find_assignment_index(y.symbol)
     sset_new = sset[:y_idx] + assignments + sset[y_idx + 1 :]
     model = model.replace(statements=sset_new)
 
     return model.update_source()
 
 
+def has_blq_transformation(model: Model, y_expr):
+    # FIXME: make more general
+    if not isinstance(y_expr, sympy.Piecewise):
+        return False
+    for statement, cond in y_expr.args:
+        blq_symb, _ = get_blq_symb_and_type(model)
+        if blq_symb in cond.free_symbols:
+            break
+    else:
+        return False
+
+    expected_m3 = ['SD', 'F_FLAG']
+    expected_m4 = ['SD', 'F_FLAG', 'CUMD', 'CUMDZ']
+    return _has_all_expected_symbs(model.statements.error, expected_m3) or _has_all_expected_symbs(
+        model.statements.error, expected_m4
+    )
+
+
+def get_blq_symb_and_type(model: Model):
+    try:
+        blq_datainfo = model.datainfo.typeix['blq']
+        return sympy.Symbol(blq_datainfo[0].name), 'blq'
+    except IndexError:
+        try:
+            blq_datainfo = model.datainfo.typeix['lloq']
+            return sympy.Symbol(blq_datainfo[0].name), 'lloq'
+        except IndexError:
+            return sympy.Symbol('LLOQ'), 'lloq'
+
+
+def _has_all_expected_symbs(sset, expected_symbs):
+    symb_names = [s.symbol.name for s in sset]
+    return all(symb in symb_names for symb in expected_symbs)
+
+
 def _verify_model(model, method):
     rvs = model.random_variables.epsilons
     if any(isinstance(rv, JointNormalDistribution) for rv in rvs):
         raise ValueError(
             f'Invalid input model: covariance between epsilons not supported in `method` {method}'
         )
-    if not (
-        has_additive_error_model(model)
-        or has_proportional_error_model(model)
-        or has_combined_error_model(model)
-    ):
-        raise ValueError('Invalid input model: error model not supported')
 
 
-def _weight_as_sd(model, y, ipred):
-    # FIXME: make more general
-    sd_assignments = []
-
-    expr = model.statements.find_assignment(y.symbol).expression
+def _get_sd(model, y):
+    y_expr = model.statements.find_assignment(y.symbol).expression
     rvs = model.random_variables.epsilons
-    rvs_in_y = {sympy.Symbol(name) for name in rvs.names if sympy.Symbol(name) in expr.free_symbols}
 
-    for arg in expr.args:
-        if not rvs_in_y.intersection(arg.free_symbols):
-            continue
-        if isinstance(arg, sympy.Symbol):
-            eps = model.random_variables[arg]
-            sigma = eps.variance
-            symb_add = create_symbol(model, 'ADD')
-            add = Assignment(symb_add, sympy.sqrt(sigma))
-            sd_assignments.append(add)
-        else:
-            rv = rvs_in_y.intersection(arg.free_symbols).pop()
-            eps = model.random_variables[rv]
-            sigma = eps.variance
-            symb_prop = create_symbol(model, 'PROP')
-            prop = Assignment(symb_prop, sympy.sqrt(sigma) * ipred)
-            sd_assignments.append(prop)
+    rv_terms = [arg for arg in y_expr.args if arg.free_symbols.intersection(rvs.free_symbols)]
+    sd_expr = []
+    for i, term in enumerate(rv_terms, 1):
+        rvs_in_term = model.random_variables.free_symbols.intersection(term.free_symbols)
+        if len(rvs_in_term) > 1:
+            raise ValueError(
+                'Invalid input model: error model not supported, terms in error model cannot contain '
+                'more than one random variable'
+            )
+        expr = rvs.replace_with_sympy_rvs(term)
+        std_term = simplify_expression(model, sympy.stats.std(expr))
+        sd_expr.append(std_term)
 
     symb_sd = create_symbol(model, 'SD')
+    sd_expr_full = sympy.sqrt(sympy.Add(*[expr**2 for expr in sd_expr]))
 
-    sd = Assignment(symb_sd, sympy.sqrt(sympy.Add(*[ass.symbol**2 for ass in sd_assignments])))
-    sd_assignments.append(sd)
-    return sd_assignments, symb_sd
+    return Assignment(symb_sd, simplify_expression(model, sd_expr_full))
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/common.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,29 +146,29 @@
     Note that the operation is not done inplace.
 
     Parameters
     ----------
     model : Model
         Model to convert
     to_format : str
-        Name of format to convert into. Currently supported 'generic', 'nlmixr' and 'nonmem'
+        Name of format to convert into. Currently supported 'generic', 'nlmixr', 'nonmem', and 'rxode'
 
     Returns
     -------
     Model
         New model object with new underlying model format
 
     Example
     -------
     >>> from pharmpy.modeling import load_example_model, convert_model
     >>> model = load_example_model("pheno")
     >>> converted_model = convert_model(model, "nlmixr")    # doctest: +SKIP
 
     """
-    supported = ['generic', 'nlmixr', 'nonmem']
+    supported = ['generic', 'nlmixr', 'nonmem', 'rxode']
     if to_format not in supported:
         raise ValueError(f"Unknown format {to_format}: supported formats are f{supported}")
     # FIXME: Use code that can discover plugins below
     if to_format == 'generic':
         new = Model.create_model()
         new = new.replace(
             dataset=model.dataset,
@@ -186,39 +186,43 @@
             initial_individual_estimates=model.initial_individual_estimates,
         )
         return new
     elif to_format == 'nlmixr':
         import pharmpy.plugins.nlmixr.model as nlmixr
 
         new = nlmixr.convert_model(model)
+    elif to_format == 'rxode':
+        import pharmpy.plugins.rxode.model as rxode
+
+        new = rxode.convert_model(model)
     else:
         import pharmpy.plugins.nonmem.model as nonmem
 
         new = nonmem.convert_model(model)
     return new
 
 
-def generate_model_code(model: Model):
+def get_model_code(model: Model):
     """Get the model code of the underlying model language
 
     Parameters
     ----------
     model : Model
         Pharmpy model
 
     Returns
     -------
     str
         Model code
 
     Examples
     --------
-    >>> from pharmpy.modeling import generate_model_code, load_example_model
+    >>> from pharmpy.modeling import get_model_code, load_example_model
     >>> model = load_example_model("pheno")
-    >>> generate_model_code(model)  # doctest: +SKIP
+    >>> get_model_code(model)  # doctest: +SKIP
 
     """
     return model.model_code
 
 
 def print_model_code(model: Model):
     """Print the model code of the underlying model language
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/compartments.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/compartments.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/covariate_effect.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/data.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -982,15 +982,15 @@
     Note that all values are directly calculated from the dataset
 
     Parameters
     ----------
     model : Model
         Pharmpy model object
 
-    Results
+    Returns
     -------
     pd.DataFrame
         Concentration parameters
 
     Examples
     --------
     >>> from pharmpy.modeling import load_example_model, get_concentration_parameters_from_data
@@ -1333,15 +1333,15 @@
     model : Model
         Pharmpy model object
     lloq : float
         Lower limit of quantification. Default not specified.
     uloq : float
         Upper limit of quantification. Default not specified.
 
-    Results
+    Returns
     -------
     Model
         Pharmpy model object
 
     Examples
     --------
     >>> from pharmpy.modeling import *
@@ -1538,20 +1538,20 @@
 def check_dataset(model: Model, dataframe: bool = False, verbose: bool = False):
     """Check dataset for consistency across a set of rules
 
     Parameters
     ----------
     model : Model
         Pharmpy model object
-    dataframe : Bool
+    dataframe : bool
         True to return a DataFrame instead of printing to the console
-    verbose : Bool
+    verbose : bool
         Print out all rules checked if True else print only failed rules
 
-    Results
+    Returns
     -------
     pd.DataFrame
         Only returns a DataFrame is dataframe=True
     """
     di = model.datainfo
     df = model.dataset
     checker = Checker(di, df, verbose=verbose)
@@ -1622,15 +1622,15 @@
     Parameters
     ----------
     datainfo : DataInfo | Path | str
         A datainfo object or a path to a datainfo object
     datatype : str
         A string to specify dataset type
 
-    Results
+    Returns
     -------
     pd.DataFrame
         The dataset
     """
     if not isinstance(datainfo, DataInfo):
         datainfo = DataInfo.read_json(datainfo)
 
@@ -1680,15 +1680,15 @@
     df : pd.DataFrame
         A dataset
     id_column : str
         Name of the id column
     date_columns : list
         Names of all date columns
 
-    Results
+    Returns
     -------
     pd.DataFrame
         Deidentified dataset
     """
     df = df.copy()
     df[id_column] = pd.to_numeric(df[id_column])
     resampler = resample_data(df, id_column)
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/error.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/error.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/estimation.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/estimation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/estimation_steps.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/estimation_steps.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/eta_additions.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/eta_additions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/eta_transformations.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/eta_transformations.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/evaluation.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/evaluation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/moxo.csv` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/moxo.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/moxo.mod` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/moxo.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.cov` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.datainfo` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.dta` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.ext` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.lst` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.mod` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.phi` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno.tab` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno_linear.dta` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno_linear.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno_linear.ext` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno_linear.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno_linear.lst` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno_linear.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno_linear.mod` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno_linear.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/example_models/pheno_linear.phi` & `pharmpy-core-0.93.0/src/pharmpy/modeling/example_models/pheno_linear.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/expressions.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,15 @@
     Each symbol will only be declared once.
 
     Parameters
     ----------
     model : Model
         Pharmpy model
 
-    Results
+    Returns
     -------
     Model
         Pharmpy model object
 
     Examples
     --------
     >>> from pharmpy.modeling import *
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/help_functions.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/iterators.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/iterators.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/lrt.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/lrt.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/math.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/metabolite.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/metabolite.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/odes.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/odes.py`

 * *Files 2% similar despite different names*

```diff
@@ -2030,14 +2030,84 @@
             statements = (
                 model.statements.before_odes + assignment + odes + model.statements.after_odes
             )
     model = model.replace(statements=statements)
     return model.update_source()
 
 
+def get_zero_order_inputs(model: Model) -> sympy.Matrix:
+    """Get zero order inputs for all compartments
+
+    Parameters
+    ----------
+    model : Model
+        Pharmpy model
+
+    Return
+    ------
+    sympy.Matrix
+        Vector of inputs
+
+    Examples
+    --------
+    >>> from pharmpy.modeling import get_zero_order_inputs, load_example_model
+    >>> model = load_example_model("pheno")
+    >>> get_zero_order_inputs(model)
+    Matrix([[0]])
+    """
+    odes = model.statements.ode_system
+    if odes is None:
+        return sympy.Matrix()
+    return odes.zero_order_inputs
+
+
+def set_zero_order_input(
+    model: Model, compartment: str, expression: Union[str, int, float, sympy.Expr]
+) -> Model:
+    """Set a zero order input for the ode system
+
+    If the zero order input is already set it will be updated.
+
+    Parameters
+    ----------
+    model : Model
+        Pharmpy model
+    compartment : str
+        Name of the compartment
+    expression : Union[str, sympy.Expr]
+        The expression of the zero order input
+
+    Return
+    ------
+    model
+        Pharmpy model object
+
+    Examples
+    --------
+    >>> from pharmpy.modeling import *
+    >>> model = load_example_model("pheno")
+    >>> model = set_zero_order_input(model, "CENTRAL", 10)
+    >>> get_zero_order_inputs(model)
+    Matrix([[10]])
+    """
+    odes = model.statements.ode_system
+    if odes is None:
+        raise ValueError("Model has no system of ODEs")
+    comp = odes.find_compartment(compartment)
+    if comp is None:
+        raise ValueError(f"Model has no compartment named {compartment}")
+    expr = sympy.sympify(expression)
+    cb = CompartmentalSystemBuilder(odes)
+    cb.set_input(comp, expr)
+    cs = CompartmentalSystem(cb)
+    statements = model.statements.before_odes + cs + model.statements.after_odes
+    model = model.replace(statements=statements)
+    return model.update_source()
+
+
 class ODEDisplayer:
     def __init__(self, eqs, ics):
         self._eqs = eqs
         self._ics = ics
 
     def __repr__(self):
         if self._eqs is None:
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/parameter_sampling.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/parameter_sampling.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/parameters.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/plots.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     iofv2 : pd.Series
         Estimated iOFV of the second model
     name1 : str
         Name of first model
     name2 : str
         Name of second model
 
-    Results
+    Returns
     -------
     alt.Chart
         Scatterplot
 
     """
     x_label = f'{name1} iOFV'
     y_label = f'{name2} iOFV'
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/remove_iiv.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/remove_iiv.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/remove_iov.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/remove_iov.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/results.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/units.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/units.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/update_inits.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/update_inits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/modeling/write_csv.py` & `pharmpy-core-0.93.0/src/pharmpy/modeling/write_csv.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/fcon/model.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/fcon/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nlmixr/__init__.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nlmixr/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nlmixr/ini.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nlmixr/ini.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pharmpy.model
 from pharmpy.deps import sympy
 from pharmpy.internals.code_generator import CodeGenerator
-from pharmpy.modeling import get_sigmas
 
 from .name_mangle import name_mangle
 
 
 def add_theta(model: pharmpy.model.Model, cg: CodeGenerator) -> None:
     """
     Add THETAs to code generator when converting a model
@@ -21,30 +20,35 @@
     for theta in thetas:
         if model.estimation_steps[0].method not in ["SAEM", "NLME"]:
             add_ini_parameter(cg, theta, boundary=True)
         else:
             add_ini_parameter(cg, theta)
 
 
-def add_eta(model: pharmpy.model.Model, cg: CodeGenerator) -> None:
+def add_eta(model: pharmpy.model.Model, cg: CodeGenerator, as_list=False) -> None:
     """
     Add ETAs to code generator when converting a model
 
     Parameters
     ----------
     model : pharmpy.model.Model
         Pharmpy model object.
     cg : CodeGenerator
         Code generator to add code upon.
+    as_list : bool
+        Add with separation character ","
     """
     for dist in model.random_variables.etas:
         omega = dist.variance
         if len(dist.names) == 1:
             init = model.parameters[omega.name].init
-            cg.add(f'{name_mangle(dist.names[0])} ~ {init}')
+            code_line = f'{name_mangle(dist.names[0])} ~ {init}'
+            if as_list and dist != model.random_variables.etas[-1]:
+                code_line += ","
+            cg.add(code_line)
         else:
             inits = []
             for row in range(omega.rows):
                 for col in range(row + 1):
                     inits.append(model.parameters[omega[row, col].name].init)
             cg.add(
                 f'{" + ".join([name_mangle(name) for name in dist.names])} ~ c({", ".join([str(x) for x in inits])})'
@@ -58,19 +62,31 @@
     Parameters
     ----------
     model : pharmpy.model.Model
         Pharmpy model object.
     cg : CodeGenerator
         Code generator to add code upon.
     """
-    for sigma in get_sigmas(model):
-        if model.estimation_steps[0].method not in ["SAEM", "NLME"]:
-            add_ini_parameter(cg, sigma, boundary=True)
+    for dist in model.random_variables.epsilons:
+        sigma = dist.variance
+        if len(dist.names) == 1:
+            sigma_param = model.parameters[sigma]
+            if sigma_param.init != 1 and not sigma_param.fix:
+                if model.estimation_steps[0].method not in ["SAEM", "NLME"]:
+                    add_ini_parameter(cg, sigma_param, boundary=True)
+                else:
+                    add_ini_parameter(cg, sigma_param)
         else:
-            add_ini_parameter(cg, sigma)
+            for row, col in zip(range(sigma.rows), range(sigma.rows + 1)):
+                sigma_param = model.parameters[sigma[row, col]]
+                if sigma_param.init != 1 and not sigma_param.fix:
+                    if model.estimation_steps[0].method not in ["SAEM", "NLME"]:
+                        add_ini_parameter(cg, sigma_param, boundary=True)
+                    else:
+                        add_ini_parameter(cg, sigma_param)
 
 
 def add_ini_parameter(cg: CodeGenerator, parameter: sympy.Symbol, boundary: bool = False) -> None:
     """
     Add a parameter to the ini block in nlmixr2. This is performed for theta
     and sigma parameter values as they are handled in the same manner.
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nlmixr/model.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nlmixr/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,20 @@
     set_evaluation_step,
     translate_nmtran_time,
     update_inits,
     write_csv,
 )
 from pharmpy.results import ModelfitResults
 from pharmpy.tools import fit
+from pharmpy.workflows.log import Log
 
+from .error_model import res_error_term
 from .ini import add_eta, add_sigma, add_theta
 from .model_block import add_ode, add_statements
-from .sanity_checks import check_model, print_warning
+from .sanity_checks import check_model
 
 
 def convert_model(
     model: pharmpy.model.Model, keep_etas: bool = False, skip_check: bool = False
 ) -> pharmpy.model.Model:
     """
     Convert a NONMEM model into an nlmixr model
@@ -70,15 +72,15 @@
         datainfo=model.datainfo,
         dataset=model.dataset,
         name=model.name,
         description=model.description,
     )
 
     # Update dataset
-    if model.dataset is not None or len(model.dataset) != 0:
+    if model.dataset is not None:
         if keep_etas is True:
             nlmixr_model = nlmixr_model.replace(
                 modelfit_results=ModelfitResults(
                     individual_estimates=model.modelfit_results.individual_estimates
                 )
             )
         nlmixr_model = translate_nmtran_time(nlmixr_model)
@@ -87,16 +89,16 @@
         if all(x in nlmixr_model.dataset.columns for x in ["RATE", "DUR"]):
             nlmixr_model = drop_columns(nlmixr_model, ["DUR"])
         nlmixr_model = nlmixr_model.replace(
             datainfo=nlmixr_model.datainfo.replace(path=None),
             dataset=nlmixr_model.dataset.reset_index(drop=True),
         )
 
-    # Add evid
-    nlmixr_model = add_evid(nlmixr_model)
+        # Add evid
+        nlmixr_model = add_evid(nlmixr_model)
 
     # Check model for warnings regarding data structure or model contents
     nlmixr_model = check_model(nlmixr_model, skip_error_model_check=skip_check)
 
     nlmixr_model.update_source()
 
     return nlmixr_model
@@ -158,22 +160,63 @@
         A code object associated with the model.
     model : pharmpy.model.Model
         A pharmpy.model object.
 
     """
 
     cg.add('model({')
-    cg.indent()
 
-    add_statements(model, cg, model.statements.before_odes)
+    # Add statements before ODEs
+    cg.indent()
+    if len(model.statements.after_odes) != 0:
+        add_statements(model, cg, model.statements.before_odes)
 
+    # Add the ODEs
     if model.statements.ode_system:
         add_ode(model, cg)
 
-    add_statements(model, cg, model.statements.after_odes)
+    # Find what kind of error model we are looking at
+    dv = list(model.dependent_variables.keys())[0]
+    dv_statement = model.statements.find_assignment(dv)
+
+    only_piecewise = False
+    if dv_statement.expression.is_Piecewise:
+        only_piecewise = True
+        dependencies = set()
+        res_alias = set()
+        for s in model.statements.after_odes:
+            if s.symbol == dv:
+                if s.expression.is_Piecewise:
+                    for value, cond in s.expression.args:
+                        if value != dv:
+                            dv_term = res_error_term(model, value)
+                            dependencies.update(dv_term.dependencies())
+
+                            dv_term.create_res_alias()
+                            res_alias.update(dv_term.res_alias)
+                else:
+                    dv_term = res_error_term(model, s.expression)
+                    dependencies.update(dv_term.dependencies())
+
+                    dv_term.create_res_alias()
+                    res_alias.update(dv_term.res_alias)
+    else:
+        dv_term = res_error_term(model, dv_statement.expression)
+        dependencies = dv_term.dependencies()
+        dv_term.create_res_alias()
+        res_alias = dv_term.res_alias
+
+    # Add statements after ODEs
+    if len(model.statements.after_odes) == 0:
+        statements = model.statements
+    else:
+        statements = model.statements.after_odes
+    add_statements(
+        model, cg, statements, only_piecewise, dependencies=dependencies, res_alias=res_alias
+    )
 
     cg.dedent()
     cg.add('})')
 
 
 def create_fit(cg: CodeGenerator, model: pharmpy.model.Model) -> None:
     """
@@ -201,17 +244,14 @@
 
     method = estimation_steps.method
     interaction = estimation_steps.interaction
 
     nonmem_method_to_nlmixr = {"FOCE": "foce", "FO": "fo", "SAEM": "saem"}
 
     if method not in nonmem_method_to_nlmixr.keys():
-        print_warning(
-            f"Estimation method {method} unknown to nlmixr2. Using 'FOCEI' as placeholder"
-        )
         nlmixr_method = "focei"
     else:
         nlmixr_method = nonmem_method_to_nlmixr[method]
 
     if interaction and nlmixr_method != "saem":
         nlmixr_method += "i"
 
@@ -306,28 +346,34 @@
         import pyreadr
     try:
         rdata = pyreadr.read_r(rdata_path)
     except (FileNotFoundError, OSError):
         return None
 
     rdata["thetas"] = rdata["thetas"].loc[get_thetas(model).names]
-    rdata["sigma"] = rdata["sigma"].loc[get_sigmas(model).names]
+    s = []
+    for sigma in get_sigmas(model):
+        if sigma.init != 1 and not sigma.fix:
+            s.append(sigma.name)
+    rdata["sigma"] = rdata["sigma"].loc[s]
 
     ofv = rdata['ofv']['ofv'][0]
     omegas_sigmas = {}
     omega = model.random_variables.etas.covariance_matrix
     for i in range(0, omega.rows):
         for j in range(0, omega.cols):
             symb = omega.row(i)[j]
             if symb != 0:
                 omegas_sigmas[symb.name] = rdata['omega'].values[i, j]
     sigma = model.random_variables.epsilons.covariance_matrix
     for i in range(len(sigma)):
         if sigma[i] != 0:
-            omegas_sigmas[sigma[i].name] = rdata['sigma']['fit$theta'][sigma[i].name]
+            s = sigma[i]
+            if model.parameters[s].init != 1 and not model.parameters[s].fix:
+                omegas_sigmas[sigma[i].name] = rdata['sigma']['fit$theta'][sigma[i].name]
     thetas_index = 0
     pe = {}
     for param in model.parameters:
         if param.fix:
             continue
         elif param.name in omegas_sigmas:
             pe[param.name] = omegas_sigmas[param.name]
@@ -340,15 +386,21 @@
     pe = pd.Series(pe)
     predictions = rdata['pred'].set_index(["ID", "TIME"])
     predictions.index = predictions.index.set_levels(
         predictions.index.levels[0].astype("float64"), level=0
     )
 
     res = ModelfitResults(
-        name=name, description=description, ofv=ofv, parameter_estimates=pe, predictions=predictions
+        name=name,
+        description=description,
+        ofv=ofv,
+        minimization_successful=True,  # FIXME: parse minimization status
+        parameter_estimates=pe,
+        predictions=predictions,
+        log=Log(),
     )
     return res
 
 
 def execute_model(model: pharmpy.model.Model, db: str) -> pharmpy.model.Model:
     """
     Executes a model using nlmixr2 estimation.
@@ -362,14 +414,15 @@
 
     Returns
     -------
     model : pharmpy.model.Model
         Model with accompanied results.
 
     """
+    db = pharmpy.workflows.LocalDirectoryToolDatabase(db)
     database = db.model_database
     model = convert_model(model)
     path = Path.cwd() / f'nlmixr_run_{model.name}-{uuid.uuid1()}'
     model.internals.path = path
     meta = path / '.pharmpy'
     meta.mkdir(parents=True, exist_ok=True)
     write_csv(model, path=path)
@@ -533,30 +586,30 @@
     else:
         nlmixr_model = convert_model(
             update_inits(nonmem_model, nonmem_model.modelfit_results.parameter_estimates)
         )
 
     # Execute the nlmixr model
     print_step("Executing nlmixr2 model... (this might take a while)")
-    import pharmpy.workflows
 
-    db = pharmpy.workflows.LocalDirectoryToolDatabase(db_name)
-    nlmixr_model = execute_model(nlmixr_model, db)
+    nlmixr_model = execute_model(nlmixr_model, db_name)
     nlmixr_results = nlmixr_model.modelfit_results.predictions
 
     pred = False
     ipred = False
     for p in nonmem_model.modelfit_results.predictions.columns:
         if p == "PRED":
             pred = True
             nonmem_results.rename(columns={p: 'PRED_NONMEM'}, inplace=True)
             nlmixr_results.rename(columns={p: 'PRED_NLMIXR'}, inplace=True)
-        elif p == "IPRED":
+        elif p == "IPRED" or p == "CIPREDI":
             ipred = True
             nonmem_results.rename(columns={p: 'IPRED_NONMEM'}, inplace=True)
+            if p == "CIPREDI":
+                p = "IPRED"
             nlmixr_results.rename(columns={p: 'IPRED_NLMIXR'}, inplace=True)
         else:
             print(
                 f"Unknown prediction value {p}. Currently only 'PRED' and 'IPRED' are supported and this is ignored"
             )
 
     if not (pred or ipred):
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nlmixr/model_block.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nlmixr/error_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,275 +1,272 @@
-import re
+from typing import Union
 
 import pharmpy.model
-from pharmpy.deps import sympy, sympy_printing
-from pharmpy.internals.code_generator import CodeGenerator
-from pharmpy.model import Assignment
-
-from .error_model import add_error_model, add_error_relation, convert_piecewise, find_term
-from .name_mangle import name_mangle
-
-
-class ExpressionPrinter(sympy_printing.str.StrPrinter):
-    def __init__(self, amounts):
-        self.amounts = amounts
-        super().__init__()
-
-    def _print_Symbol(self, expr):
-        return name_mangle(expr.name)
-
-    def _print_Derivative(self, expr):
-        fn = expr.args[0]
-        return f'd/dt({fn.name})'
-
-    def _print_Function(self, expr):
-        name = expr.func.__name__
-        if name in self.amounts:
-            return expr.func.__name__
-        else:
-            return expr.func.__name__ + f'({self.stringify(expr.args, ", ")})'
-
-
-def add_statements(
-    model: pharmpy.model.Model, cg: CodeGenerator, statements: pharmpy.model.statements
-) -> None:
-    """
-    Add statements to generated code generator. The statements should be before
-    or after the ODEs.
-
-    Parameters
-    ----------
-    model : pharmpy.model.Model
-        A pharmpy model object to add statements to.
-    cg : CodeGenerator
-        Codegenerator object holding the code to be added to.
-    statements : pharmpy.model.statements
-        Statements to be added to the code generator.
-    """
-    # FIXME: handle other DVs?
-    dv = list(model.dependent_variables.keys())[0]
-
-    error_model_found = False
-    dv_found = False
-
-    for s in statements:
-        if isinstance(s, Assignment):
-            if s.symbol == dv:
-                dv_found = True
-
-                # FIXME : Find another way to assert that a sigma exist
-                sigma = None
-                for dist in model.random_variables.epsilons:
-                    sigma = dist.variance
-                assert sigma is not None
-
-                if s.expression.is_Piecewise:
-                    convert_piecewise(s, cg, model)
-                else:
-                    expr, error = find_term(model, s.expression)
-                    add_error_model(cg, expr, error, s.symbol.name)
-                    add_error_relation(cg, error, s.symbol)
-                    error_model_found = True
+from pharmpy.deps import sympy
+from pharmpy.internals.expr.subs import subs
+from pharmpy.modeling import get_thetas
+
+
+class res_error_term:
+    def __init__(self, model, expr):
+        self.model = model
+        self.expr = sympy.expand(expr)
+
+        self.only_piecewise = None
+        self.is_only_piecewise()
+
+        self.res = None
+        self.res_alias = None
+        self.add = error()
+        self.prop = error()
+        self.find_term()
+
+    def create_res_alias(self):
+        if self.res is not None:
+            res_alias = set()
+            for s in self.res.free_symbols:
+                all_a = find_aliases(s, self.model)
+                for a in all_a:
+                    if a not in res_alias:
+                        res_alias.add(a)
+            self.res_alias = res_alias
+
+    def dependencies(self):
+        dependencies = set()
+        if self.add.expr is not None:
+            dependencies.update(self.add.dependencies)
+        elif self.prop.expr is not None:
+            dependencies.update(self.prop.dependencies)
+        return dependencies
+
+    def find_term(self):
+        # NEED TO BE
+        # VAR 1 : y = F + F*eps + eps
+        # VAR 2 : y = F + F*theta*eps + theta*eps (EPS FIX 1)
+        # VAR 3 : y = F + W*eps (W = sqrt(theta....)) (EPS FIX 1)
+        # VAR 4 : y = F + W*eps (W = F*theta + theta) (EPS FIX 1)
+        # ELSE raise error
+        terms = sympy.Add.make_args(self.expr)
+        # Assert that it follows the above set of format rules
+        assert len(terms) <= 3
+
+        errors = []
+        for term in terms:
+            error_term = False
+            for factor in sympy.Mul.make_args(term):
+                full_term = full_expression(factor, self.model)
+                all_symbols = full_term.free_symbols.union(factor.free_symbols)
+                for symbol in all_symbols:
+                    if str(symbol) in self.model.random_variables.epsilons.names:
+                        sigma = convert_eps_to_sigma(symbol, self.model)
+                        if self.model.parameters[str(sigma)].init == 1.0:
+                            if self.model.parameters[str(sigma)].fix:
+                                term.subs(factor, 1)
+                        if factor != symbol:
+                            sigma_alias = factor
+                        else:
+                            sigma_alias = None
+                        error_term = True
 
+            if error_term:
+                errors.append(
+                    {
+                        "term": term,
+                        "full_term": full_term,
+                        "sigma": sigma,
+                        "sigma_alias": sigma_alias,
+                    }
+                )
             else:
-                expr = s.expression
-                if expr.is_Piecewise:
-                    first = True
-                    for value, cond in expr.args:
-                        if cond is not sympy.S.true:
-                            if cond.atoms(sympy.Eq):
-                                cond = convert_eq(cond)
-                            if first:
-                                cg.add(f'if ({cond}) {{')
-                                first = False
-                            else:
-                                cg.add(f'}} else if ({cond}) {{')
-                        else:
-                            cg.add('} else {')
-                            if "NEWIND" in [t.name for t in expr.free_symbols] and value == 0:
-                                largest_value = expr.args[0].expr
-                                largest_cond = expr.args[0].cond
-                                for value, cond in expr.args[1:]:
-                                    if cond is not sympy.S.true:
-                                        if cond.rhs > largest_cond.rhs:
-                                            largest_value = value
-                                            largest_cond = cond
-                                        elif cond.rhs == largest_cond.rhs:
-                                            if not isinstance(cond, sympy.LessThan) and isinstance(
-                                                largest_cond, sympy.LessThan
-                                            ):
-                                                largest_value = value
-                                                largest_cond = cond
-                                value = largest_value
-                        cg.indent()
-                        cg.add(f'{s.symbol.name} <- {value}')
-                        cg.dedent()
-                    cg.add('}')
+                if self.res is None:
+                    self.res = term
+                    self.create_res_alias()
                 else:
-                    cg.add(f'{s.symbol.name} <- {expr}')
-
-    if dv_found and not error_model_found:
-        error = {"add": None, "prop": None}
-        add_error_relation(cg, error, dv)
-
-
-def add_ode(model: pharmpy.model.Model, cg: CodeGenerator) -> None:
-    """
-    Add the ODEs from a model to a code generator
-
-    Parameters
-    ----------
-    model : pharmpy.model.Model
-        A pharmpy model object to add ODEs to.
-    cg : CodeGenerator
-        Codegenerator object holding the code to be added to.
-    """
-    amounts = [am.name for am in list(model.statements.ode_system.amounts)]
-    printer = ExpressionPrinter(amounts)
+                    # FIXME : Should this be allowed??
+                    self.res += term
 
-    des = model.internals.DES
-    statements = []
-    if des:
-        pattern = re.compile(r"DADT\(\d*\)")
-        for s in des.statements:
-            if not pattern.match(s.symbol.name):
-                statements.append(s)
-        add_statements(model, cg, statements)
-    for eq in model.statements.ode_system.eqs:
-        # Should remove piecewise from these equations in nlmixr
-        if eq.atoms(sympy.Piecewise):
-            lhs = remove_piecewise(printer.doprint(eq.lhs))
-            rhs = remove_piecewise(printer.doprint(eq.rhs))
-
-            cg.add(f'{lhs} = {rhs}')
+        if self.res is None:
+            print("No resulting term found")
+            exit
+        elif len(errors) > 2:
+            print("Too many error terms found")
+            exit
+
+        prop = False
+
+        for t in errors:
+            prop = False
+            term = t["term"]
+            full_term = t["full_term"]
+            for symbol in full_term.free_symbols:
+                for ali in find_aliases(symbol, self.model).union(term.free_symbols):
+                    if ali in self.res_alias:
+                        prop = True
+                        # Remove the resulting symbol from the error term
+                        term = convert_eps_to_sigma(term, self.model)
+                        term = term.subs(ali, 1)
+                        self.prop = error(
+                            self.model, term, t["sigma"], sigma_alias=t["sigma_alias"], prop=True
+                        )
+
+            if prop is False:
+                term = convert_eps_to_sigma(term, self.model)
+                self.add = error(
+                    self.model, term, t["sigma"], sigma_alias=t["sigma_alias"], add=True
+                )
+
+    def is_only_piecewise(self):
+        dv = list(self.model.dependent_variables.keys())[0]
+        for s in reversed(self.model.statements.after_odes):
+            if s.symbol == dv:
+                if not s.expression.is_Piecewise:
+                    self.only_piecewise = False
+                    break
+
+        if self.only_piecewise is None:
+            self.only_piecewise = True
+
+    def __str__(self):
+        s = ""
+        s += str(f"add : {self.add.expr}\n")
+        s += str(f"add_sigma : {self.add.sigma}\n")
+        s += str(f"prop : {self.prop.expr}\n")
+        s += str(f"prop_sigma : {self.prop.sigma}\n")
+        s += str(f"Only piecewise : {self.only_piecewise}\n")
+        return s
+
+
+class error:
+    def __init__(self, model=None, expr=0, sigma=None, add=False, sigma_alias=None, prop=False):
+        self.model = model
+        self.expr = expr
+        self.sigma = sigma
+        self.sigma_alias = sigma_alias
+        self.sigma_fix = self.is_sigma_fix()
+        self.add = add
+        self.prop = prop
+        self.dependencies = set()
+        self.check_dependecies()
+
+    def is_sigma_fix(self):
+        if self.model is not None:
+            if self.model.parameters[str(self.sigma)].init == 1.0:
+                if self.model.parameters[str(self.sigma)].fix:
+                    return True
         else:
-            cg.add(f'{printer.doprint(eq.lhs)} = {printer.doprint(eq.rhs)}')
+            return False
 
+    def check_dependecies(self):
+        if self.model is not None and self.expr is not None:
+            accepted_symbols = set([self.sigma, self.sigma_alias])
+            thetas = get_thetas(self.model).symbols
+            accepted_symbols.update(thetas)
+            for symbol in self.expr.free_symbols:
+                if symbol not in accepted_symbols:
+                    # TODO : also aid  aliases for all dependencies
+                    self.dependencies.add(symbol)
 
-def remove_piecewise(expr: str) -> str:
-    """
-    Return an expression without Piecewise statements
 
-    Parameters
-    ----------
-    expr : str
-        A sympy expression, given as a string
-
-    Returns
-    -------
-    str
-        Return given expression but without Piecewise statements
-
-    """
-    all_piecewise = find_piecewise(expr)
-    # Go into each piecewise found
-    for p in all_piecewise:
-        expr = piecewise_replace(expr, p, "")
-    return expr
-
-
-def find_piecewise(expr: str) -> list:
-    """
-    Locate all Piecewise statements in an expression and return them as a list
-
-    Parameters
-    ----------
-    expr : str
-        A sympy expression in string form
-
-    Returns
-    -------
-    list
-        A list of all piecewise statements found in the expression
-
-    """
-    d = find_parentheses(expr)
-
-    piecewise_start = [m.start() + len("Piecewise") for m in re.finditer("Piecewise", expr)]
-
-    all_piecewise = []
-    for p in piecewise_start:
-        if p in d:
-            all_piecewise.append(expr[p + 1 : d[p]])
-    return all_piecewise
-
-
-def find_parentheses(s: str) -> dict:
+def full_expression(expression: sympy.Expr, model: pharmpy.model.Model) -> sympy.Expr:
     """
-    Find all matching parenthesis in a given string
+    Return the full expression of an expression (used for model statements)
 
     Parameters
     ----------
-    s : str
-        Any string
+    expression : sympy.Expr
+        Expression to be expanded.
+    model : pharmpy.model.Model
+        A pharmpy mode object with the expression as a statement.
 
     Returns
     -------
-    dict
-        A dictionary with keys corresponding to positions of the opening
-        parenthesis and value being the position of the closing parenthesis.
+    expression : sympy.Expr
+        The fully expanded expression
 
     """
-    start = []  # all opening parentheses
-    d = {}
-
-    for i, c in enumerate(s):
-        if c == '(':
-            start.append(i)
-        if c == ')':
-            try:
-                d[start.pop()] = i
-            except IndexError:
-                print('Too many closing parentheses')
-    if start:  # check if stack is empty afterwards
-        print('Too many opening parentheses')
+    if len(model.statements.after_odes) == 0:
+        statements = model.statements
+    else:
+        statements = model.statements.after_odes
 
-    return d
+    for statement in reversed(statements):
+        expression = subs(expression, {statement.symbol: statement.expression}, simultaneous=True)
+    return expression
 
 
-def piecewise_replace(expr: str, piecewise: sympy.Piecewise, s: str) -> str:
+def find_aliases(symbol: str, model: pharmpy.model, aliases: set = None) -> list:
     """
-    Will replace a given piecewise expression with wanted string, s
+    Returns a list of all variable names that are the same as the inputed symbol
 
     Parameters
     ----------
-    expr : str
-        A string representive a sympy expression
-    piecewise : sympy.Piecewise
-        A sympy Piecewise statement to be changed
-    s : str
-        A string with wanted information to change piecewise to
+    symbol : str
+        The name of the variable to find aliases to.
+    model : pharmpy.model
+        A model by which the inputed symbol is related to.
 
     Returns
     -------
-    str
-        Expression with replaced piecewise expressions.
+    aliases: list
+        A list of aliases for the symbol.
 
     """
-    if s == "":
-        expr = re.sub(r'([\+\-\/\*]\s*)(Piecewise)', r'\2', expr)
-        return expr.replace(f'Piecewise({piecewise})', s)
+    if aliases is None:
+        aliases = set([symbol])
     else:
-        return expr.replace(f'Piecewise({piecewise})', s)
-
-
-def convert_eq(cond: sympy.Eq) -> str:
+        aliases.add(symbol)
+    for expr in model.statements.after_odes:
+        # If RES = ALI
+        if symbol == expr.symbol and isinstance(expr.expression, sympy.Symbol):
+            if expr.expression not in aliases:
+                aliases.union(find_aliases(expr.expression, model, aliases))
+
+        # If RES = PIECEWISE or PIECEWISE = RES
+        if expr.expression.is_Piecewise:
+            for e, c in expr.expression.args:
+                if symbol == expr.symbol and isinstance(e, sympy.Symbol):
+                    if e not in aliases:
+                        aliases.union(find_aliases(e, model, aliases))
+                elif symbol == e:
+                    if expr.symbol not in aliases:
+                        aliases.union(find_aliases(expr.symbol, model, aliases))
+
+        # If ALI = RES
+        if symbol == expr.expression:
+            if expr.symbol not in aliases:
+                aliases.union(find_aliases(expr.symbol, model, aliases))
+    return aliases
+
+
+def convert_eps_to_sigma(
+    expr: Union[sympy.Symbol, sympy.Mul], model: pharmpy.model.Model
+) -> Union[sympy.Symbol, sympy.Mul]:
     """
-    Convert a sympy equal statement to R syntax
+    Change the use of epsilon names to sigma names instead. Mostly used for
+    converting NONMEM format to nlmxir2
 
     Parameters
     ----------
-    cond : sympy.Eq
-        Sympy equals statement
+    expr : Union[sympy.Symbol,sympy.Mul]
+        A sympy term to change a variable name in
+    model : pharmpy.Model
+        A pharmpy model object
 
     Returns
     -------
-    str
-        A string with R format for the same statement
+    Union[sympy.Symbol,sympy.Mul]
+        Same expression as inputed, but with epsilon names changed to sigma.
 
     """
-    cond = sympy.pretty(cond)
-    cond = cond.replace("=", "==")
-    cond = cond.replace("∧", "&")
-    cond = cond.replace("∨", "|")
-    cond = re.sub(r'(ID\s*==\s*)(\d+)', r"\1'\2'", cond)
-    return cond
+    # eps_to_sigma = {
+    #    sympy.Symbol(eps.names[0]): sympy.Symbol(str(eps.variance))
+    #    for eps in model.random_variables.epsilons
+    # }
+    eps_to_sigma = {}
+    for dist in model.random_variables.epsilons:
+        sigma = dist.variance
+        if len(dist.names) == 1:
+            eps_to_sigma[dist.names[0]] = sigma
+        else:
+            for row, col, eps in zip(range(sigma.rows), range(sigma.rows + 1), dist.names):
+                eps_to_sigma[eps] = sigma[row, col]
+    return expr.subs(eps_to_sigma)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nlmixr/sanity_checks.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nlmixr/sanity_checks.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 This module contain functions for checking the format of an nlmixr model conversion
 in order to inform the users of any errors or mistakes that can could be made.
 
 It serves purpose in catching known errors that are not yet solved, or limitations
 that are found in the conversion software
 """
 
-import warnings
-
 import pharmpy.model
 from pharmpy.deps import sympy
 from pharmpy.modeling import (
     has_additive_error_model,
     has_combined_error_model,
     has_proportional_error_model,
 )
@@ -36,16 +34,17 @@
 
     Returns
     -------
     pharmpy.model.Model
         Issues will be printed to the terminal and model is returned.
 
     """
+
     # Checks for the dataset
-    if model.dataset is not None or len(model.dataset) != 0:
+    if model.dataset is not None:
         if "TIME" in model.dataset.columns:
             if same_time(model):
                 print_warning(
                     "Observation and bolus dose at the same time in the data. Modified for nlmixr model"
                 )
                 model = change_same_time(model)
 
@@ -58,17 +57,32 @@
     if rvs_same(model, sigma=True):
         print_warning("Sigma with value same not supported. Updated as follows.")
         model = change_rvs_same(model, sigma=True)
     if rvs_same(model, omega=True):
         print_warning("Omega with value same not supported. Updated as follows.")
         model = change_rvs_same(model, omega=True)
 
+    # Checks regarding esimation method
+    method = model.estimation_steps[0].method
+    if not known_estimation_method(method):
+        print_warning(
+            f"Estimation method {method} unknown to nlmixr2. Using 'FOCEI' as placeholder"
+        )
+
     return model
 
 
+def known_estimation_method(method):
+    nonmem_method_to_nlmixr = {"FOCE": "foce", "FO": "fo", "SAEM": "saem"}
+    if method in nonmem_method_to_nlmixr.keys():
+        return True
+    else:
+        return False
+
+
 def known_error_model(model: pharmpy.model.Model) -> bool:
     """
     Check if the associated error model is known to pharmpy. Currently check if
     model hase
     - additive error model
     - proportional error model
     - combined error model
@@ -153,16 +167,15 @@
     Returns
     -------
     model : pharmpy.model.Model
         The same model with a changed dataset.
 
     """
     dataset = model.dataset.copy()
-    dataset = dataset.reset_index()
-    time = dataset["TIME"]
+    dataset = dataset.reset_index(drop=True)
 
     if "RATE" in dataset.columns:
         rate = True
     else:
         rate = False
 
     evid_ignore = [0, 3, 4]
@@ -174,44 +187,30 @@
                     ID = row["ID"]
                     TIME = row["TIME"]
                     subset = dataset[(dataset["ID"] == ID) & (dataset["TIME"] == TIME)]
                     if any([x not in evid_ignore for x in subset["EVID"].unique()]) and any(
                         [x in evid_ignore for x in subset["EVID"].unique()]
                     ):
                         if rate:
-                            if any([x != 0 for x in subset["RATE"].unique()]) and any(
-                                [x == 0 for x in subset["RATE"].unique()]
-                            ):
-                                dataset.loc[
-                                    (dataset["ID"] == ID)
-                                    & (dataset["TIME"] == TIME)
-                                    & (dataset["RATE"] == 0)
-                                    & (~dataset["EVID"].isin(evid_ignore)),
-                                    "TIME",
-                                ] += 0.000001
+                            dataset.loc[
+                                (dataset["ID"] == ID)
+                                & (dataset["TIME"] == TIME)
+                                & (dataset["RATE"] == 0)
+                                & (~dataset["EVID"].isin(evid_ignore)),
+                                "TIME",
+                            ] += 0.000001
                         else:
-                            return True
+                            dataset.loc[
+                                (dataset["ID"] == ID)
+                                & (dataset["TIME"] == TIME)
+                                & (~dataset["EVID"].isin(evid_ignore)),
+                                "TIME",
+                            ] += 0.000001
 
-    with warnings.catch_warnings():
-        # Supress a numpy deprecation warning
-        warnings.simplefilter("ignore")
-        for index, row in dataset.iterrows():
-            if index != 0:
-                if row["ID"] == dataset.loc[index - 1]["ID"]:
-                    if row["TIME"] == dataset.loc[index - 1]["TIME"]:
-                        temp = index - 1
-                        while dataset.loc[temp]["TIME"] == row["TIME"]:
-                            if dataset.loc[temp]["EVID"] not in [0, 3]:
-                                if rate:
-                                    if dataset.loc[temp]["RATE"] == 0:
-                                        time[temp] = time[temp] + 10**-6
-                                else:
-                                    time[temp] = time[temp] + 10**-6
-                            temp += 1
-    model.dataset["TIME"] = time
+    model = model.replace(dataset=dataset)
     return model
 
 
 def rvs_same(model: pharmpy.model.Model, sigma: bool = False, omega: bool = False) -> bool:
     """
     Check if there are random variables that are referencing the same
     distribution value.
@@ -276,47 +275,62 @@
     elif omega:
         rvs = model.random_variables.etas
 
     checked_variance = []
     var_to_add = {}
     rvs_and_var = {}
     for rv in rvs:
-        var = rv.variance
-        if var in checked_variance:
-            n = 1
-            new_var = sympy.Symbol(var.name + "_" + f'{n}')
-            while new_var in checked_variance:
-                n += 1
-                new_var = sympy.Symbol(var.name + "_" + f'{n}')
+        current_var = []
 
-            var_to_add[new_var] = var
+        if isinstance(rv.variance, sympy.Symbol):
+            variance = [rv.variance]
+        else:
+            variance = rv.variance
 
-            checked_variance.append(new_var)
+        for var in variance:
+            if var in checked_variance:
+                n = 1
+                new_var = sympy.Symbol(var.name + "_" + f'{n}')
+                while new_var in checked_variance:
+                    n += 1
+                    new_var = sympy.Symbol(var.name + "_" + f'{n}')
 
-            rvs_and_var[rv.names] = new_var
-            print(rv, " : ", new_var)
-        else:
-            checked_variance.append(var)
+                var_to_add[new_var] = var
 
-    for rv in rvs:
-        if rv.names in rvs_and_var:
-            new_rv = rv.replace(variance=rvs_and_var[rv.names])
+                current_var.append(new_var)
 
-            all_rvs = model.random_variables
-            keep = [name for name in all_rvs.names if name not in [rv.names[0]]]
+                rvs_and_var[(rv.names, var)] = new_var
+                # print(rv, " : ", new_var)
+            else:
+                current_var.append(var)
 
-            model = model.replace(random_variables=all_rvs[keep])
-            model = model.replace(random_variables=model.random_variables + new_rv)
+        checked_variance += current_var
 
     params = model.parameters
     for s in var_to_add:
         param = model.parameters[var_to_add[s]].replace(name=s.name)
         params = params + param
     model = model.replace(parameters=params)
 
+    etas = [e[0] for e in rvs_and_var.keys()]
+    for rv in rvs:
+        if rv.names in etas:
+            old_to_new = [name_var for name_var in rvs_and_var if name_var[0] == rv.names]
+            new_rv = rv
+            for el in old_to_new:
+                old = el[1]
+                new = rvs_and_var[el]
+                new_variance = new_rv.variance.replace(old, new)
+                new_rv = new_rv.replace(variance=new_variance)
+            all_rvs = model.random_variables
+
+            keep = [name for name in all_rvs.names if name not in rv.names]
+            model = model.replace(random_variables=all_rvs[keep])
+            model = model.replace(random_variables=model.random_variables + new_rv)
+
     # Add newline after all updated sigma values have been printed
     print()
     return model
 
 
 def print_warning(warning: str) -> None:
     """
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/__init__.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/advan.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/advan.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/config.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/config.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/dataset.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/dataset.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/model.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/nmtran_parser.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/nmtran_parser.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/parsing.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -770,25 +770,38 @@
         raise DatasetError('Could not identify observation rows in dataset')
     have_obs = set(df_obs['ID'].unique())
     all_ids = set(df['ID'].unique())
     ids_to_remove = all_ids - have_obs
     return df[~df['ID'].isin(ids_to_remove)]
 
 
-def parse_table_columns(control_stream):
+def parse_table_columns(control_stream, netas):
     # Handle synonyms and appended columns
 
     reserved = {'PRED', 'IPRED', 'CIPREDI'}
     synonyms = dict()
     all_columns = []
 
+    code_recs = (
+        control_stream.get_records('PK')
+        + control_stream.get_records('PRED')
+        + control_stream.get_records('ERROR')
+    )
+    symbs = set()
+    for rec in code_recs:
+        for s in rec.statements:
+            symbs.add(s.symbol.name)
+
+    (colnames, _, _, _) = parse_column_info(control_stream)
+    symbs |= set(colnames)
+
     for table_record in control_stream.get_records('TABLE'):
         noappend = False
         columns = []
-        for opt, key, value in table_record.parsed_options:
+        for opt, key, value in table_record.parse_options(nonoptions=symbs, netas=netas):
             if key == 'NOAPPEND':
                 noappend = True
             elif opt.need_value is None:
                 if value is None:
                     if key in synonyms:
                         columns.append(synonyms[key])
                     else:
@@ -801,15 +814,16 @@
                         columns.append(value)
                         synonyms[key] = value
                     else:
                         # FIXME: Fallback since we don't know all reserved names
                         columns.append(key)
 
         if not noappend:
-            toappend = ['DV', 'PRED', 'RES', 'WRES']
-            # Remove appended columns explicitly in $TABLE
-            columns = [col for col in columns if col not in toappend]
+            toremove = ['PRED', 'RES', 'WRES']
+            toappend = ['DV'] + toremove
+            # Remove appended columns explicitly in $TABLE except DV
+            columns = [col for col in columns if col not in toremove]
             columns.extend(toappend)
 
         all_columns.append(columns)
 
     return all_columns
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/abbreviated_record.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/abbreviated_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/code_record.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/code_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/data_record.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/data_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/factory.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/factory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/code_record.lark` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/code_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/data_record.lark` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/data_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/model_record.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/model_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/omega_record.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/omega_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/option_record.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/option_record.py`

 * *Files 5% similar despite different names*

```diff
@@ -374,16 +374,17 @@
                 else:
                     done.add(name)
 
             if curlength == 3:
                 break
             curlength -= 1
 
-    def parse_ast(self, tree):
+    def parse_ast(self, tree, nonoptions=None, netas=None):
         # Return a list of tuples of canonical option name, value (or None for no value)
+        # Nonoptions will not be matched against options but kept as WildOpts
         opt_nodes = list(tree.subtrees('option'))
         found_options = set()
         i = 0
         parsed = []
 
         def add_option(opt, name, value):
             # * Same MxOpt or SimpleOpt multiple times is ignored
@@ -402,14 +403,59 @@
                         )
             parsed.append((opt, name, value))
             found_options.add(opt)
 
         while i < len(opt_nodes):
             node = opt_nodes[i]
             key = _get_key(node)
+            # FIXME: This is special for $TABLE. Either have special case for this or have an Opt for it.
+            m = re.match(r'ETAS\(?', key)
+            if m:
+                # join all keys that belong with the ETAS
+                etas = key
+                while ')' not in key:
+                    i += 1
+                    node = opt_nodes[i]
+                    key = _get_key(node)
+                    etas += key
+                etas = etas[5:-1].replace(" ", "").replace("\t", "")
+                if ',' in etas:
+                    a = etas.split(',')
+                    for n in a:
+                        parsed.append((WildOpt(), f'ETA{n}', None))
+                else:
+                    m = re.match(r'(?P<start>\d+)(TO|:)(?P<end>\d+|LAST)(BY(?P<by>-?\d+))?', etas)
+                    if m:
+                        by = 1 if m.group('by') is None else int(m.group('by'))
+                        start = int(m.group('start'))
+                        end = m.group('end')
+                        if end == 'LAST':
+                            end = netas
+                        else:
+                            end = int(end)
+                        if start > end:
+                            end -= 1
+                            if by > 0:
+                                by = -by
+                        else:
+                            if by < 0:
+                                start, end = end, start
+                                end -= 1
+                            else:
+                                end += 1
+                        for n in range(start, end, by):
+                            parsed.append((WildOpt(), f'ETA{n}', None))
+                i += 1
+                continue
+
+            # FIXME: What happens if key=value for nonoption?
+            if key in nonoptions:
+                parsed.append((WildOpt(), key, None))
+                i += 1
+                continue
             value = _get_value(node)
             for opt in self.options:
                 if opt.match(key):
                     if opt.need_value is True:
                         if value is None:
                             i += 1
                             if i < len(opt_nodes):
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/parsers.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/parsers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/problem_record.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/problem_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/record.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/sizes_record.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/sizes_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/subroutine_record.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/subroutine_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/table_record.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/table_record.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,19 @@
     # BY and EXCLUDE_BY missing
 )
 
 
 class TableRecord(OptionRecord):
     option_defs = table_options
 
+    def __init__(self, name, raw_name, root):
+        # Overriding to not parse options at parse time.
+        # Need other records to be parsed first.
+        super(OptionRecord, self).__init__(name, raw_name, root)
+
     @property
     def path(self):
         file_option = self.option_pairs['FILE']
         assert file_option is not None
         return Path(file_option)
 
     def set_path(self, value):
@@ -72,12 +77,14 @@
             if not m and value is not None:
                 m = re.match(regexp, value)
             if m:
                 n = m.group(1)
                 derivs.append(int(n))
         return derivs
 
+    def parse_options(self, nonoptions, netas):
+        return self.option_defs.parse_ast(self.root, nonoptions=nonoptions, netas=netas)
+
 
 # FIXME: These situations are not handled
-# Names (from $INPUT, $PK, $ERROR and $PRED?) can override options
 # No columns are allowed after first option
 # Overridden names are ignored after first option (not error)
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/records/theta_record.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/records/theta_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/results.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         final_pe,
         sdcorr,
         pe_iterations,
         ses,
         ses_sdcorr,
     ) = _parse_ext(control_stream, name_map, ext_tables, subproblem, parameters)
 
-    table_df = _parse_tables(path, control_stream)
+    table_df = _parse_tables(path, control_stream, netas=len(model.random_variables.etas.names))
     residuals = _parse_residuals(table_df)
     predictions = _parse_predictions(table_df)
     iofv, ie, iec = _parse_phi(path, control_stream, name_map, etas, subproblem)
     rse = _calculate_relative_standard_errors(final_pe, ses)
     (
         runtime_total,
         log_likelihood,
@@ -318,15 +318,15 @@
         ]
         covs = pd.Series(etc_frames, index=ids, dtype='object')
         return individual_ofv, individual_estimates, covs
     except KeyError:
         return None, None, None
 
 
-def _parse_tables(path: Path, control_stream: NMTranControlStream) -> pd.DataFrame:
+def _parse_tables(path: Path, control_stream: NMTranControlStream, netas) -> pd.DataFrame:
     """Parse $TABLE and table files into one large dataframe of useful columns"""
     interesting_columns = {
         'ID',
         'TIME',
         'PRED',
         'CIPREDI',
         'CPRED',
@@ -334,15 +334,15 @@
         'RES',
         'WRES',
         'CWRES',
         'MDV',
     }
 
     table_recs = control_stream.get_records('TABLE')
-    colnames_list = parse_table_columns(control_stream)
+    colnames_list = parse_table_columns(control_stream, netas)
     found = set()
     df = pd.DataFrame()
     for table_rec, colnames in zip(table_recs, colnames_list):
         columns_in_table = []
         colnames_in_table = []
         for i, name in enumerate(colnames):
             if name in interesting_columns and name not in found:
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/results_file.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/results_file.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/run.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/table.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/table.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/nonmem/update.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/nonmem/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Parameter,
     Parameters,
     RandomVariables,
     Statements,
     data,
     output,
 )
-from pharmpy.modeling import get_ids, has_linear_odes_with_real_eigenvalues, simplify_expression
+from pharmpy.modeling import get_ids, simplify_expression
 from pharmpy.plugins.nonmem.records.parsers import CodeRecordParser
 
 if TYPE_CHECKING:
     from .model import Model
 
 from .nmtran_parser import NMTranControlStream
 from .parsing import parse_column_info
@@ -371,17 +371,17 @@
     Handle changes from to CompartmentSystem
     """
     if old is None:
         old = CompartmentalSystem(CompartmentalSystemBuilder())
 
     model = update_lag_time(model, old, new)
 
-    advan, trans, nonlin = new_advan_trans(model)
+    advan, trans, nonlin, haszo = new_advan_trans(model)
 
-    if nonlin:
+    if nonlin or haszo:
         model = to_des(model, new)
     else:
         if isinstance(new.dosing_compartment.dose, Bolus) and 'RATE' in model.datainfo.names:
             df = model.dataset.drop(columns=['RATE'])
             model = model.replace(dataset=df)
 
         model = pk_param_conversion(model, advan=advan, trans=trans)
@@ -399,14 +399,20 @@
 def is_nonlinear_odes(model: Model):
     """Check if ode system is nonlinear"""
     odes = model.statements.ode_system
     M = odes.compartmental_matrix
     return odes.t in M.free_symbols
 
 
+def has_zero_order_inputs(model: Model):
+    odes = model.statements.ode_system
+    zo = odes.zero_order_inputs
+    return not all(a == 0 for a in zo)
+
+
 def update_infusion(model: Model, old: ODESystem):
     statements = model.statements
     new = statements.ode_system
     assert new is not None
     if isinstance(new.dosing_compartment.dose, Infusion) and not statements.find_assignment('D1'):
         # Handle direct moving of Infusion dose
         statements = statements.subs({'D2': 'D1'})
@@ -522,14 +528,34 @@
             dose = False
         mod = mod.add_compartment(name, dosing=dose)
     cs = cs.replace_records([old_mod], [mod])
     model = model.replace(internals=model.internals.replace(control_stream=cs))
     return model
 
 
+def update_ics(statements, odes):
+    if odes is not None:
+        trans = {}
+        for i, amount in enumerate(odes.amounts, start=1):
+            trans[sympy.Function(amount.name)(0)] = sympy.Function('A_0')(i)
+
+        new = []
+        update = False
+        for s in statements:
+            if s.symbol.is_Function:
+                newsymb = trans[s.symbol]
+                s = s.replace(symbol=newsymb)
+                update = True
+            new.append(s)
+        if update:
+            return Statements(new)
+
+    return statements
+
+
 def update_statements(model: Model, old: Statements, new: Statements, trans):
     trans['NaN'] = int(data.conf.na_rep)
     main_statements = Statements()
     error_statements = Statements()
 
     new_odes = new.ode_system
     updated_dataset = False
@@ -557,14 +583,15 @@
                     subs = model.internals.control_stream.get_records('SUBROUTINES')[0]
                     newsubs = subs.set_advan(advan)
                     newcs = model.internals.control_stream.replace_records([subs], [newsubs])
                     model = model.replace(internals=model.internals.replace(control_stream=newcs))
                     model = update_model_record(model, advan)
 
     main_statements = model.statements.before_odes
+    main_statements = update_ics(main_statements, new_odes)
     error_statements = model.statements.after_odes
 
     rec = model.internals.control_stream.get_pred_pk_record()
     newrec = rec.update_statements(main_statements.subs(trans), model.random_variables, trans)
     newcs = model.internals.control_stream.replace_records([rec], [newrec])
     model = model.replace(internals=model.internals.replace(control_stream=newcs))
 
@@ -956,33 +983,33 @@
     if all_subs:
         subs = all_subs[0]
         oldtrans = subs.get_option_startswith('TRANS')
     else:
         oldtrans = None
     odes = model.statements.ode_system
     nonlin = is_nonlinear_odes(model)
-    if nonlin:
+    has_zo = has_zero_order_inputs(model)
+    if nonlin or has_zo:
         advan = 'ADVAN13'
     elif match_advan1(odes):
         advan = 'ADVAN1'
     elif match_advan2(odes):
         advan = 'ADVAN2'
     elif match_advan3(odes):
         advan = 'ADVAN3'
     elif match_advan4(odes):
         advan = 'ADVAN4'
     elif match_advan11(odes):
         advan = 'ADVAN11'
     elif match_advan12(odes):
         advan = 'ADVAN12'
     else:  # General linear
-        if has_linear_odes_with_real_eigenvalues(model):
-            advan = 'ADVAN7'
-        else:
-            advan = 'ADVAN5'
+        # We could use ADVAN7 if has_linear_odes_with_real_eigenvalues
+        # but ADVAN7 seems to be unstable in NONMEM
+        advan = 'ADVAN5'
 
     if nonlin:
         trans = None
     elif oldtrans == 'TRANS1':
         trans = oldtrans
     elif oldtrans == 'TRANS2':
         if advan in ['ADVAN1', 'ADVAN2']:
@@ -1017,15 +1044,15 @@
             else:
                 trans = 'TRANS4'
         else:
             trans = 'TRANS1'
     else:
         trans = 'TRANS1'
 
-    return advan, trans, nonlin
+    return advan, trans, nonlin, has_zo
 
 
 def update_subroutines_record(model: Model, advan, trans):
     """Update $SUBROUTINES with new advan and trans"""
     all_subs = model.internals.control_stream.get_records('SUBROUTINES')
     if not all_subs:
         content = f'$SUBROUTINES {advan} {trans}\n'
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/plugins/utils.py` & `pharmpy-core-0.93.0/src/pharmpy/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/reporting/altairplot.py` & `pharmpy-core-0.93.0/src/pharmpy/reporting/altairplot.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/reporting/custom.css` & `pharmpy-core-0.93.0/src/pharmpy/reporting/custom.css`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/reporting/reporting.py` & `pharmpy-core-0.93.0/src/pharmpy/reporting/reporting.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/results.py` & `pharmpy-core-0.93.0/src/pharmpy/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/__init__.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/allometry/tool.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/allometry/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/amd/funcs.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/amd/funcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/amd/run.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/amd/run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/bootstrap/report.rst` & `pharmpy-core-0.93.0/src/pharmpy/tools/bootstrap/report.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/bootstrap/results.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/bootstrap/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/bootstrap/tool.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/bootstrap/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/cdd/results.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/cdd/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/common.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/covsearch/tool.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/covsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/crossval/results.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/crossval/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/estmethod/algorithms.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/estmethod/algorithms.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/estmethod/report.rst` & `pharmpy-core-0.93.0/src/pharmpy/tools/estmethod/report.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/estmethod/tool.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/estmethod/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/evaldesign/tool.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/evaldesign/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/frem/models.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/frem/models.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/frem/results.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/frem/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/frem/tool.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/frem/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/funcs/ml.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/funcs/ml.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite` & `pharmpy-core-0.93.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite` & `pharmpy-core-0.93.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/funcs/summarize_individuals.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/funcs/summarize_individuals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/iivsearch/algorithms.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/iivsearch/algorithms.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/iivsearch/tool.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/iivsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/iovsearch/tool.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/iovsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/linearize/results.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/linearize/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/linearize/tool.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/linearize/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/feature/absorption.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/feature/absorption.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/feature/covariate.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/feature/covariate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/feature/elimination.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/feature/elimination.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/feature/peripherals.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/feature/peripherals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/feature/transits.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/feature/transits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/filter.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/filter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/grammar.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/grammar.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/helpers.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/helpers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/interpreter.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/interpreter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/parse.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/parse.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/definition.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/definition.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/absorption.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/absorption.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/covariate.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/covariate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/elimination.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/elimination.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/statement/feature/transits.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/statement/feature/transits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/mfl/stringify.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/mfl/stringify.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/modelfit/__init__.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/modelfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/modelfit/results.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/modelfit/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/modelfit/tool.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/modelfit/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/modelsearch/algorithms.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/modelsearch/algorithms.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/modelsearch/tool.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/modelsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/psn_helpers.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/psn_helpers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/qa/results.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/qa/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/rankfuncs.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/rankfuncs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/run.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -955,35 +955,53 @@
         minsucc = res.minimization_successful
 
     if minsucc is not None:
         summary_dict['minimization_successful'] = minsucc
     else:
         summary_dict['minimization_successful'] = False
 
-    if i == -1:
+    if i == -1 and res.ofv_iterations is not None:
         i = max(res.ofv_iterations.index.get_level_values(0)) - 1
-    ofv = res.ofv_iterations[i + 1,].iloc[-1]
-    summary_dict['ofv'] = ofv
+
+    summary_dict['ofv'] = _get_ofv(res, i)
     summary_dict['runtime_total'] = res.runtime_total
-    summary_dict['estimation_runtime'] = res.estimation_runtime_iterations.iloc[i]
+    summary_dict['estimation_runtime'] = _get_estimation_runtime(res, i)
 
-    pe = res.parameter_estimates_iterations.loc[i + 1,].iloc[-1]
+    pe = _get_parameter_estimates(res, i)
     ses = res.standard_errors
     rses = res.relative_standard_errors
 
     for param in pe.index:
         summary_dict[f'{param}_estimate'] = pe[param]
         if ses is not None:
             summary_dict[f'{param}_SE'] = ses[param]
         if rses is not None:
             summary_dict[f'{param}_RSE'] = rses[param]
 
     return summary_dict
 
 
+def _get_ofv(res, i):
+    if res.ofv_iterations is None:
+        return res.ofv
+    return res.ofv_iterations[i + 1,].iloc[-1]
+
+
+def _get_parameter_estimates(res, i):
+    if res.parameter_estimates_iterations is None:
+        return res.parameter_estimates
+    return res.parameter_estimates_iterations.loc[i + 1,].iloc[-1]
+
+
+def _get_estimation_runtime(res, i):
+    if res.estimation_runtime_iterations is None:
+        return res.runtime_total
+    return res.estimation_runtime_iterations.iloc[i]
+
+
 def read_modelfit_results(path: Union[str, Path]) -> ModelfitResults:
     """Read results from external tool for a model
 
     Parameters
     ----------
     path : Path or str
         Path to model file
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/ruvsearch/results.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/ruvsearch/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/ruvsearch/tool.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/ruvsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/scm/psn_wrapper.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/scm/psn_wrapper.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/scm/results.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/scm/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/simeval/results.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/simeval/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/simfit/results.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/simfit/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/tools/wrap.py` & `pharmpy-core-0.93.0/src/pharmpy/tools/wrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/visualization.py` & `pharmpy-core-0.93.0/src/pharmpy/visualization.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/workflows/__init__.py` & `pharmpy-core-0.93.0/src/pharmpy/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/workflows/args.py` & `pharmpy-core-0.93.0/src/pharmpy/workflows/args.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/workflows/call.py` & `pharmpy-core-0.93.0/src/pharmpy/workflows/call.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/workflows/dispatchers/local_dask.py` & `pharmpy-core-0.93.0/src/pharmpy/workflows/dispatchers/local_dask.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/workflows/execute.py` & `pharmpy-core-0.93.0/src/pharmpy/workflows/execute.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/workflows/log.py` & `pharmpy-core-0.93.0/src/pharmpy/workflows/log.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/workflows/model_database/baseclass.py` & `pharmpy-core-0.93.0/src/pharmpy/workflows/model_database/baseclass.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/workflows/model_database/local_directory.py` & `pharmpy-core-0.93.0/src/pharmpy/workflows/model_database/local_directory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/workflows/model_database/null_database.py` & `pharmpy-core-0.93.0/src/pharmpy/workflows/model_database/null_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/workflows/optimize.py` & `pharmpy-core-0.93.0/src/pharmpy/workflows/optimize.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/workflows/tool_database/baseclass.py` & `pharmpy-core-0.93.0/src/pharmpy/workflows/tool_database/baseclass.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/workflows/tool_database/local_directory.py` & `pharmpy-core-0.93.0/src/pharmpy/workflows/tool_database/local_directory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/workflows/tool_database/null_database.py` & `pharmpy-core-0.93.0/src/pharmpy/workflows/tool_database/null_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy/workflows/workflow.py` & `pharmpy-core-0.93.0/src/pharmpy/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/src/pharmpy_core.egg-info/PKG-INFO` & `pharmpy-core-0.93.0/src/pharmpy_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmpy-core
-Version: 0.92.0
+Version: 0.93.0
 Summary: Pharmacometric modeling
 Home-page: https://pharmpy.github.io
 Author: Rikard Nordgren
 Author-email: rikard.nordgren@farmaci.uu.se
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Bug Tracker, https://github.com/pharmpy/pharmpy/issues
 Project-URL: Source Code, https://github.com/pharmpy/pharmpy
@@ -41,14 +41,37 @@
 * A model abstraction as a foundation for higher level operations on models
 * Functions for manipulation of models, e.g. changing model components like elimination or absorption
 * Reading NONMEM models and results
 * Running models and complex workflows (with NONMEM or to some extent nlmixr)
 
 This is the `team behind Pharmpy <https://pharmpy.github.io/latest/contributors.html>`_
 
+0.93.0 (2023-04-19)
+-------------------
+
+New features
+============
+
+* Add function ``modeling.get_zero_order_inputs``
+* Add function ``modeling.set_zero_order_input``
+* Add function ``modeling.set_tmdd``
+* Added plugin to convert models to RxODE
+* Support conversion of more models to nlmixr
+
+Changes
+=======
+
+* ``modeling.generate_model_code`` was renamed to ``modeling.get_model_code`` since the code is not generated by this function
+* Do not use ADVAN7 because models that should work with ADVAN7 didn't were found
+
+Bugfixes
+========
+
+* Fix multiple bugs in parsing $TABLE headers
+
 0.92.0 (2023-04-05)
 -------------------
 
 New features
 ============
 
 * Add function ``modeling.is_linearized``
```

### Comparing `pharmpy-core-0.92.0/src/pharmpy_core.egg-info/SOURCES.txt` & `pharmpy-core-0.93.0/src/pharmpy_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,15 @@
 src/pharmpy/modeling/parameter_sampling.py
 src/pharmpy/modeling/parameters.py
 src/pharmpy/modeling/plots.py
 src/pharmpy/modeling/remove_iiv.py
 src/pharmpy/modeling/remove_iov.py
 src/pharmpy/modeling/reporting.py
 src/pharmpy/modeling/results.py
+src/pharmpy/modeling/tmdd.py
 src/pharmpy/modeling/units.py
 src/pharmpy/modeling/update_inits.py
 src/pharmpy/modeling/write_csv.py
 src/pharmpy/modeling/example_models/moxo.csv
 src/pharmpy/modeling/example_models/moxo.mod
 src/pharmpy/modeling/example_models/pheno.cov
 src/pharmpy/modeling/example_models/pheno.datainfo
@@ -233,14 +234,16 @@
 src/pharmpy/plugins/nonmem/records/grammars/data_record.lark
 src/pharmpy/plugins/nonmem/records/grammars/definitions.lark
 src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark
 src/pharmpy/plugins/nonmem/records/grammars/option_record.lark
 src/pharmpy/plugins/nonmem/records/grammars/problem_record.lark
 src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark
 src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark
+src/pharmpy/plugins/rxode/__init__.py
+src/pharmpy/plugins/rxode/model.py
 src/pharmpy/reporting/altairplot.py
 src/pharmpy/reporting/conf.py
 src/pharmpy/reporting/custom.css
 src/pharmpy/reporting/reporting.py
 src/pharmpy/tools/__init__.py
 src/pharmpy/tools/common.py
 src/pharmpy/tools/psn_helpers.py
@@ -416,14 +419,15 @@
 tests/modeling/test_metabolite.py
 tests/modeling/test_modeling.py
 tests/modeling/test_parameter_sampling.py
 tests/modeling/test_parameters.py
 tests/modeling/test_plots.py
 tests/modeling/test_remove_covariate_effect.py
 tests/modeling/test_results.py
+tests/modeling/test_tmdd.py
 tests/modeling/test_units.py
 tests/nonmem/conftest.py
 tests/nonmem/test_advan.py
 tests/nonmem/test_des.py
 tests/nonmem/test_fcon.py
 tests/nonmem/test_input.py
 tests/nonmem/test_modelfit_results.py
```

### Comparing `pharmpy-core-0.92.0/tests/cli/test_cli.py` & `pharmpy-core-0.93.0/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/conftest.py` & `pharmpy-core-0.93.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/integration/conftest.py` & `pharmpy-core-0.93.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/integration/test_allometry.py` & `pharmpy-core-0.93.0/tests/integration/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/integration/test_amd.py` & `pharmpy-core-0.93.0/tests/integration/test_amd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/integration/test_bootstrap.py` & `pharmpy-core-0.93.0/tests/integration/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/integration/test_common.py` & `pharmpy-core-0.93.0/tests/integration/test_common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/integration/test_covsearch.py` & `pharmpy-core-0.93.0/tests/integration/test_covsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/integration/test_estmethod.py` & `pharmpy-core-0.93.0/tests/integration/test_estmethod.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/integration/test_evaldesign.py` & `pharmpy-core-0.93.0/tests/integration/test_evaldesign.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/integration/test_fit.py` & `pharmpy-core-0.93.0/tests/integration/test_fit.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/integration/test_iivsearch.py` & `pharmpy-core-0.93.0/tests/integration/test_iivsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/integration/test_iovsearch.py` & `pharmpy-core-0.93.0/tests/integration/test_iovsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/integration/test_modelsearch.py` & `pharmpy-core-0.93.0/tests/integration/test_modelsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/integration/test_resume.py` & `pharmpy-core-0.93.0/tests/integration/test_resume.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/integration/test_ruvsearch.py` & `pharmpy-core-0.93.0/tests/integration/test_ruvsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/internals/fs/test_lock.py` & `pharmpy-core-0.93.0/tests/internals/fs/test_lock.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/internals/module/test_lazy.py` & `pharmpy-core-0.93.0/tests/internals/module/test_lazy.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/internals/test_math.py` & `pharmpy-core-0.93.0/tests/internals/test_math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/internals/test_parse.py` & `pharmpy-core-0.93.0/tests/internals/test_parse.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/model/test_datainfo.py` & `pharmpy-core-0.93.0/tests/model/test_datainfo.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/model/test_estimation.py` & `pharmpy-core-0.93.0/tests/model/test_estimation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/model/test_model.py` & `pharmpy-core-0.93.0/tests/model/test_model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/model/test_parameter.py` & `pharmpy-core-0.93.0/tests/model/test_parameter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/model/test_random_variables.py` & `pharmpy-core-0.93.0/tests/model/test_random_variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -780,7 +780,33 @@
     x3 = VariabilityLevel.create('iov', reference=False, group='OCC')
     h = VariabilityHierarchy.create([x1, x2])
     assert h[x2].group == 'ID'
     with pytest.raises(KeyError):
         h[x3]
     with pytest.raises(KeyError):
         h['NOTHING']
+
+
+def test_replace_with_sympy_rvs():
+    var1 = symbol('OMEGA(1,1)')
+
+    dist = NormalDistribution.create('ETA(1)', 'iiv', 0, var1)
+    rvs = RandomVariables.create([dist])
+
+    expr_symbs = symbol('ETA(1)') + symbol('x')
+    expr_sympy = rvs.replace_with_sympy_rvs(expr_symbs)
+
+    assert expr_symbs != expr_sympy
+    assert not all(isinstance(arg, symbol) for arg in expr_sympy.args)
+
+    var2, cov = symbol('OMEGA(2,2)'), symbol('OMEGA(2,1)')
+
+    dist = JointNormalDistribution.create(
+        ['ETA(1)', 'ETA(2)'], 'iiv', [0, 0], [[var1, cov], [cov, var2]]
+    )
+    rvs = RandomVariables.create([dist])
+
+    expr_symbs = symbol('ETA(1)') + symbol('ETA(2)') + symbol('x')
+    expr_sympy = rvs.replace_with_sympy_rvs(expr_symbs)
+
+    assert expr_symbs != expr_sympy
+    assert not all(isinstance(arg, symbol) for arg in expr_sympy.args)
```

### Comparing `pharmpy-core-0.92.0/tests/model/test_statements.py` & `pharmpy-core-0.93.0/tests/model/test_statements.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_add_covariate_effect.py` & `pharmpy-core-0.93.0/tests/modeling/test_add_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_allometry.py` & `pharmpy-core-0.93.0/tests/modeling/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_block_rvs.py` & `pharmpy-core-0.93.0/tests/modeling/test_block_rvs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_common.py` & `pharmpy-core-0.93.0/tests/modeling/test_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 from pharmpy.model import Model as BaseModel
 from pharmpy.modeling import (
     convert_model,
     create_basic_pk_model,
     create_joint_distribution,
     fix_parameters,
-    generate_model_code,
     get_config_path,
+    get_model_code,
     get_model_covariates,
     load_example_model,
     read_model,
     read_model_from_string,
     remove_unused_parameters_and_rvs,
     set_name,
     write_model,
@@ -78,15 +78,15 @@
     write_model(model, tmp_path / 'run1.mod')
     assert Path(tmp_path / 'run1.mod').is_file()
 
 
 def test_generate_model_code(testdata, load_model_for_test):
     model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
     model = fix_parameters(model, ['THETA_1'])
-    assert generate_model_code(model).split('\n')[7] == '$THETA 0.1 FIX'
+    assert get_model_code(model).split('\n')[7] == '$THETA 0.1 FIX'
 
 
 def test_load_example_model():
     model = load_example_model("pheno")
     assert len(model.parameters) == 6
     assert len(model.modelfit_results.parameter_estimates) == 6
```

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_covariate_effect.py` & `pharmpy-core-0.93.0/tests/modeling/test_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_data_funcs.py` & `pharmpy-core-0.93.0/tests/modeling/test_data_funcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_distribution.py` & `pharmpy-core-0.93.0/tests/modeling/test_distribution.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_error.py` & `pharmpy-core-0.93.0/tests/modeling/test_error.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_estimation_steps.py` & `pharmpy-core-0.93.0/tests/modeling/test_estimation_steps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pytest
 
 from pharmpy.modeling import (
     add_covariance_step,
     add_estimation_step,
     append_estimation_step_options,
-    generate_model_code,
     remove_covariance_step,
     remove_estimation_step,
     set_estimation_step,
     set_evaluation_step,
 )
 
 
@@ -41,15 +40,15 @@
             '$ESTIMATION METHOD=ZERO MAXEVAL=0 PRINT=2 POSTHOC',
         ),
     ],
 )
 def test_set_estimation_step(testdata, load_model_for_test, method, kwargs, code_ref):
     model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
     model = set_estimation_step(model, method, **kwargs)
-    assert generate_model_code(model).split('\n')[-2] == code_ref
+    assert model.model_code.split('\n')[-2] == code_ref
 
 
 def test_set_estimation_step_est_middle(testdata, load_model_for_test):
     model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
     model = set_estimation_step(model, 'FOCE', interaction=True, cov=True, idx=0)
     assert (
         '$ESTIMATION METHOD=COND INTER MAXEVAL=9990 PRINT=2 POSTHOC\n$COVARIANCE'
@@ -58,54 +57,53 @@
 
 
 def test_add_estimation_step(testdata, load_model_for_test):
     model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
     assert len(model.estimation_steps) == 1
     model = add_estimation_step(model, 'fo')
     assert len(model.estimation_steps) == 2
-    assert generate_model_code(model).split('\n')[-2] == '$ESTIMATION METHOD=ZERO'
+    assert model.model_code.split('\n')[-2] == '$ESTIMATION METHOD=ZERO'
 
     model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
     assert len(model.estimation_steps) == 1
     model = add_estimation_step(model, 'fo', evaluation=True)
     assert len(model.estimation_steps) == 2
-    assert generate_model_code(model).split('\n')[-2] == '$ESTIMATION METHOD=ZERO MAXEVAL=0'
+    assert model.model_code.split('\n')[-2] == '$ESTIMATION METHOD=ZERO MAXEVAL=0'
 
 
 def test_add_estimation_step_non_int(testdata, load_model_for_test):
     model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
     model = add_estimation_step(model, 'fo', idx=1.0)
     with pytest.raises(TypeError, match='Index must be integer'):
         add_estimation_step(model, 'fo', idx=1.5)
 
 
 def test_remove_estimation_step(testdata, load_model_for_test):
     model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
     assert len(model.estimation_steps) == 1
     model = remove_estimation_step(model, 0)
     assert not model.estimation_steps
-    assert generate_model_code(model).split('\n')[-2] == '$SIGMA 1'
+    assert model.model_code.split('\n')[-2] == '$SIGMA 1'
 
 
 def test_add_covariance_step(testdata, load_model_for_test):
     model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
     assert len(model.estimation_steps) == 1
     model = add_covariance_step(model)
-    print(model.model_code)
     assert len(model.estimation_steps) == 1
-    assert generate_model_code(model).split('\n')[-2] == '$COVARIANCE'
+    assert model.model_code.split('\n')[-2] == '$COVARIANCE'
 
 
 def test_remove_covariance_step(testdata, load_model_for_test):
     model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
     model = add_covariance_step(model)
-    assert generate_model_code(model).split('\n')[-2] == '$COVARIANCE'
+    assert model.model_code.split('\n')[-2] == '$COVARIANCE'
     model = remove_covariance_step(model)
     assert (
-        generate_model_code(model).split('\n')[-2]
+        model.model_code.split('\n')[-2]
         == '$ESTIMATION METHOD=COND INTER MAXEVAL=9990 PRINT=2 POSTHOC'
     )
 
 
 def test_append_estimation_step_options(testdata, load_model_for_test):
     model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
     assert len(model.estimation_steps) == 1
```

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_eta_additions.py` & `pharmpy-core-0.93.0/tests/modeling/test_eta_additions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_eta_transformations.py` & `pharmpy-core-0.93.0/tests/modeling/test_eta_transformations.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_evaluate.py` & `pharmpy-core-0.93.0/tests/modeling/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_expressions.py` & `pharmpy-core-0.93.0/tests/modeling/test_expressions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_has_covariate_effect.py` & `pharmpy-core-0.93.0/tests/modeling/test_has_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_help_functions.py` & `pharmpy-core-0.93.0/tests/modeling/test_help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_iterators.py` & `pharmpy-core-0.93.0/tests/modeling/test_iterators.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_lrt.py` & `pharmpy-core-0.93.0/tests/modeling/test_lrt.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_modeling.py` & `pharmpy-core-0.93.0/tests/modeling/test_modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     add_iov,
     add_lag_time,
     add_peripheral_compartment,
     add_pk_iiv,
     create_joint_distribution,
     fix_parameters_to,
     get_initial_conditions,
+    get_zero_order_inputs,
     has_first_order_elimination,
     has_linear_odes,
     has_linear_odes_with_real_eigenvalues,
     has_michaelis_menten_elimination,
     has_mixed_mm_fo_elimination,
     has_odes,
     has_zero_order_absorption,
@@ -39,14 +40,15 @@
     set_mixed_mm_fo_elimination,
     set_ode_solver,
     set_peripheral_compartments,
     set_seq_zo_fo_absorption,
     set_transit_compartments,
     set_zero_order_absorption,
     set_zero_order_elimination,
+    set_zero_order_input,
     split_joint_distribution,
     transform_etas_boxcox,
     transform_etas_john_draper,
     transform_etas_tdist,
     update_initial_individual_estimates,
     update_inits,
 )
@@ -802,15 +804,15 @@
     model = set_transit_compartments(model, 3)
     transits = model.statements.ode_system.find_transit_compartments(model.statements)
     assert len(transits) == 3
     correct = (
         """$PROBLEM PHENOBARB SIMPLE MODEL
 $DATA ../pheno.dta IGNORE=@
 $INPUT ID TIME AMT WGT APGR DV FA1 FA2
-$SUBROUTINE ADVAN7 TRANS1
+$SUBROUTINE ADVAN5 TRANS1
 
 $MODEL COMPARTMENT=(TRANSIT1 DEFDOSE) COMPARTMENT=(TRANSIT2) COMPARTMENT=(TRANSIT3) """
         + """COMPARTMENT=(CENTRAL)
 $PK
 MDT = THETA(4)
 IF(AMT.GT.0) BTIME=TIME
 TAD=TIME-BTIME
@@ -853,15 +855,15 @@
 def test_transit_compartments_change_number(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'pheno.mod')
     model = set_transit_compartments(model, 3)
     model = set_transit_compartments(model, 2)
     correct = """$PROBLEM PHENOBARB SIMPLE MODEL
 $DATA pheno.dta IGNORE=@
 $INPUT ID TIME AMT WGT APGR DV
-$SUBROUTINE ADVAN7 TRANS1
+$SUBROUTINE ADVAN5 TRANS1
 
 $MODEL COMPARTMENT=(TRANSIT1 DEFDOSE) COMPARTMENT=(TRANSIT2) COMPARTMENT=(CENTRAL)
 $PK
 MDT = THETA(3)
 CL=THETA(1)*EXP(ETA(1))
 V=THETA(2)*EXP(ETA(2))
 S3 = V
@@ -885,15 +887,15 @@
 
     model = load_model_for_test(testdata / 'nonmem' / 'pheno.mod')
     model = set_transit_compartments(model, 2)
     model = set_transit_compartments(model, 3)
     correct = """$PROBLEM PHENOBARB SIMPLE MODEL
 $DATA pheno.dta IGNORE=@
 $INPUT ID TIME AMT WGT APGR DV
-$SUBROUTINE ADVAN7 TRANS1
+$SUBROUTINE ADVAN5 TRANS1
 
 $MODEL COMPARTMENT=(TRANSIT1 DEFDOSE) COMPARTMENT=(TRANSIT2) COMPARTMENT=(TRANSIT3) COMPARTMENT=(CENTRAL)
 $PK
 MDT = THETA(3)
 CL=THETA(1)*EXP(ETA(1))
 V=THETA(2)*EXP(ETA(2))
 S4 = V
@@ -3346,20 +3348,33 @@
     mod2 = model.replace(statements=statements)
     assert get_initial_conditions(mod2) == {sympy.Function('A_CENTRAL')(0): sympy.Integer(23)}
     path = datadir / 'minimal.mod'
     model = load_model_for_test(path)
     assert get_initial_conditions(model) == {}
 
 
-def test_set_initial_conditions(load_example_model_for_test):
+def test_set_intial_conditions(load_example_model_for_test):
     model = load_example_model_for_test("pheno")
     model = set_initial_condition(model, "CENTRAL", 10)
     assert len(model.statements) == 16
     ic = Assignment(sympy.Function('A_CENTRAL')(0), sympy.Integer(10))
     assert model.statements.before_odes[-1] == ic
     assert get_initial_conditions(model) == {sympy.Function('A_CENTRAL')(0): sympy.Integer(10)}
     model = set_initial_condition(model, "CENTRAL", 23)
     assert len(model.statements) == 16
     ic = Assignment(sympy.Function('A_CENTRAL')(0), sympy.Integer(23))
     assert model.statements.before_odes[-1] == ic
     model = set_initial_condition(model, "CENTRAL", 0)
     assert len(model.statements) == 15
+
+
+def test_get_zero_order_inputs(load_example_model_for_test):
+    model = load_example_model_for_test('pheno')
+    zo = get_zero_order_inputs(model)
+    assert zo == sympy.Matrix([[0]])
+
+
+def test_set_zero_order_input(load_example_model_for_test):
+    model = load_example_model_for_test('pheno')
+    model = set_zero_order_input(model, "CENTRAL", 10)
+    zo = get_zero_order_inputs(model)
+    assert zo == sympy.Matrix([[10]])
```

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_parameter_sampling.py` & `pharmpy-core-0.93.0/tests/modeling/test_parameter_sampling.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_parameters.py` & `pharmpy-core-0.93.0/tests/modeling/test_parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_plots.py` & `pharmpy-core-0.93.0/tests/modeling/test_plots.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_remove_covariate_effect.py` & `pharmpy-core-0.93.0/tests/modeling/test_remove_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/modeling/test_results.py` & `pharmpy-core-0.93.0/tests/modeling/test_results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/output/test_nonmem_results_file.py` & `pharmpy-core-0.93.0/tests/nonmem/output/test_nonmem_results_file.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/records/test_abbreviated.py` & `pharmpy-core-0.93.0/tests/nonmem/records/test_abbreviated.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/records/test_code.py` & `pharmpy-core-0.93.0/tests/nonmem/records/test_code.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/records/test_data.py` & `pharmpy-core-0.93.0/tests/nonmem/records/test_data.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/records/test_estimation_record.py` & `pharmpy-core-0.93.0/tests/nonmem/records/test_estimation_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/records/test_factory.py` & `pharmpy-core-0.93.0/tests/nonmem/records/test_factory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/records/test_model_record.py` & `pharmpy-core-0.93.0/tests/nonmem/records/test_model_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/records/test_omega.py` & `pharmpy-core-0.93.0/tests/nonmem/records/test_omega.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/records/test_option_record.py` & `pharmpy-core-0.93.0/tests/nonmem/records/test_option_record.py`

 * *Files 14% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     newrec = rec.remove_suboption_for_all('COMPARTMENT', 'DEFDOSE')
     assert str(newrec) == '$MODEL COMP=(COMP1) COMP=(COMP2)'
 
 
 def test_options(parser):
     assert table_options['NOPRINT'].abbreviations == ['NOPRINT', 'NOPRIN', 'NOPRI', 'NOPR', 'NOP']
     rec = parser.parse('$TABLE IPRED DV FILE=sdtab').records[0]
-    assert rec.parsed_options == [
+    assert rec.parse_options(nonoptions=set(), netas=2) == [
         (WildOpt(), 'IPRED', None),
         (WildOpt(), 'DV', None),
         (StrOpt('FILE'), 'FILE', 'sdtab'),
     ]
 
 
 @pytest.mark.usefixtures('parser')
@@ -181,8 +181,31 @@
         '$TABLE ESAMPLE=str',
         '$TABLE ID TIME PRINT NOPRINT',
         '$TABLE CLOCKSEED=0 CLOCK=0',
     ],
 )
 def test_option_errors(parser, buf):
     with pytest.raises(ValueError):
-        parser.parse(buf).records[0]
+        parser.parse(buf).records[0].parse_options(nonoptions=set(), netas=2)
+
+
+@pytest.mark.usefixtures('parser')
+@pytest.mark.parametrize(
+    "buf,netas,correct",
+    [
+        ('$TABLE ID TIME', 1, ['ID', 'TIME']),
+        ('$TABLE ID TIME ETAS(1:2)', 2, ['ID', 'TIME', 'ETA1', 'ETA2']),
+        ('$TABLE ID ETAS(1:2) TIME', 2, ['ID', 'ETA1', 'ETA2', 'TIME']),
+        ('$TABLE ID ETAS (1 : 2   ) TIME', 2, ['ID', 'ETA1', 'ETA2', 'TIME']),
+        ('$TABLE ID ETAS(1:LAST) TIME', 3, ['ID', 'ETA1', 'ETA2', 'ETA3', 'TIME']),
+        ('$TABLE ID ETAS(1 TO LAST) TIME', 3, ['ID', 'ETA1', 'ETA2', 'ETA3', 'TIME']),
+        ('$TABLE ID ETAS(1 TO LAST BY 2) TIME', 4, ['ID', 'ETA1', 'ETA3', 'TIME']),
+        ('$TABLE ID ETAS(1,2,4) TIME', 4, ['ID', 'ETA1', 'ETA2', 'ETA4', 'TIME']),
+        ('$TABLE ID ETAS(3:1) TIME', 3, ['ID', 'ETA3', 'ETA2', 'ETA1', 'TIME']),
+        ('$TABLE ID ETAS(4:1 BY -2) TIME', 4, ['ID', 'ETA4', 'ETA2', 'TIME']),
+        ('$TABLE ID ETAS(1:4 BY -1) TIME', 4, ['ID', 'ETA4', 'ETA3', 'ETA2', 'ETA1', 'TIME']),
+    ],
+)
+def test_table_parsing(parser, buf, netas, correct):
+    res = parser.parse(buf).records[0].parse_options(nonoptions=set(), netas=netas)
+    names = [col[1] for col in res]
+    assert names == correct
```

### Comparing `pharmpy-core-0.92.0/tests/nonmem/records/test_problem.py` & `pharmpy-core-0.93.0/tests/nonmem/records/test_problem.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/records/test_sizes.py` & `pharmpy-core-0.93.0/tests/nonmem/records/test_sizes.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/records/test_theta.py` & `pharmpy-core-0.93.0/tests/nonmem/records/test_theta.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/test_advan.py` & `pharmpy-core-0.93.0/tests/nonmem/test_advan.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/test_des.py` & `pharmpy-core-0.93.0/tests/nonmem/test_des.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/test_input.py` & `pharmpy-core-0.93.0/tests/nonmem/test_input.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/test_modelfit_results.py` & `pharmpy-core-0.93.0/tests/nonmem/test_modelfit_results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/test_nonmem_model.py` & `pharmpy-core-0.93.0/tests/nonmem/test_nonmem_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 )
 from pharmpy.modeling import (
     add_iiv,
     add_population_parameter,
     create_joint_distribution,
     remove_iiv,
     set_estimation_step,
+    set_initial_condition,
     set_initial_estimates,
     set_zero_order_absorption,
     set_zero_order_elimination,
+    set_zero_order_input,
 )
 from pharmpy.plugins.nonmem import convert_model
 from pharmpy.plugins.nonmem.nmtran_parser import NMTranParser
 from pharmpy.plugins.nonmem.records.factory import create_record
 from pharmpy.tools.amd.funcs import create_start_model
 
 
@@ -1166,7 +1168,23 @@
     $OMEGA 0.01
     $SIGMA 1
     '''
     model = Model.create_model(StringIO(code))
 
     with pytest.raises(ValueError, match='NONMEM does not allow etas named `eta`'):
         add_iiv(model, ['Y'], 'exp', '+', eta_names=['eta'])
+
+
+def test_ics(load_model_for_test, pheno_path):
+    model = load_model_for_test(pheno_path)
+    model = set_initial_condition(model, 'CENTRAL', 23)
+    pk = model.internals.control_stream.get_pred_pk_record()
+    a = str(pk).split('\n')
+    assert a[9] == 'A_0(1) = 23'
+
+
+def test_zo(load_model_for_test, pheno_path):
+    model = load_model_for_test(pheno_path)
+    model = set_zero_order_input(model, "CENTRAL", 10)
+    des = model.internals.control_stream.get_records("DES")[0]
+    print(des)
+    assert str(des) == "$DES\nDADT(1) = -A(1)*CL/V + 10\n"
```

### Comparing `pharmpy-core-0.92.0/tests/nonmem/test_nonmem_table.py` & `pharmpy-core-0.93.0/tests/nonmem/test_nonmem_table.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/nonmem/test_parser.py` & `pharmpy-core-0.93.0/tests/nonmem/test_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,9 +52,9 @@
     ],
 )
 def test_table_columns(buf, columns):
     parser = NMTranParser()
 
     cs = parser.parse(buf)
     cs._active_problem = -1  # To trick cs.get_records
-    parsed_columns = parse_table_columns(cs)
+    parsed_columns = parse_table_columns(cs, netas=2)
     assert parsed_columns == columns
```

### Comparing `pharmpy-core-0.92.0/tests/nonmem/test_read.py` & `pharmpy-core-0.93.0/tests/nonmem/test_read.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/frem/results.json` & `pharmpy-core-0.93.0/tests/testdata/frem/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/DDMODEL00000130` & `pharmpy-core-0.93.0/tests/testdata/nonmem/DDMODEL00000130`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv` & `pharmpy-core-0.93.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml` & `pharmpy-core-0.93.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/errors/control_stream_error.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/errors/control_stream_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/errors/est_step_warning.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/errors/est_step_warning.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/errors/no_header_error.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/errors/no_header_error.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/errors/no_header_error.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/errors/no_header_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/errors/rounding_error.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/errors/rounding_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/errors/run_interrupted.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/errors/run_interrupted.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/errors/zero_gradient_error.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/errors/zero_gradient_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/fcon/FCON` & `pharmpy-core-0.93.0/tests/testdata/nonmem/fcon/FCON`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/fcon/FDATA` & `pharmpy-core-0.93.0/tests/testdata/nonmem/fcon/FDATA`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_3.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_3.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_3.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_3.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_4.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_4.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_4.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_4.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_4.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_1transit.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_1transit.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_2transits.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_2transits.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan1.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan11.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan11.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan12.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan12.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan2.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan3.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan4.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/fviii6.datainfo` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/fviii6.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/fviii6.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/fviii6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox1.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox1.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox1.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox1.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox1.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox2.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox2.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox2.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox2.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_2comp.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_2comp.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_2comp.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_2comp.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_2comp.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_2comp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_2comp.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_2comp.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_2comp.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_2comp.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_simulated_log.csv` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_simulated_log.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_simulated_normal.csv` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_simulated_normal.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/mytab_mox2` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/mytab_mox2`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pef.csv` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pef.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_dvid.csv` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_dvid.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_dvid.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_dvid.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_noifs.coi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_noifs.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_noifs.cor` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_noifs.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_noifs.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_noifs.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_noifs.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_noifs.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_noifs.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_noifs.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_noifs.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_noifs.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_trans1.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_trans1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_trans1.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_trans1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/models/pheno_trans1.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/models/pheno_trans1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno.datainfo` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno.dta` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_block.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_block.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_etas.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_etas.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_rate.dta` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_rate.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.coi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.cor` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.tab` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real.xml` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real.xml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real_linbase.dta` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real_linbase.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real_linbase.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real_linbase.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real_linbase.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/pheno_real_linbase.tab` & `pharmpy-core-0.93.0/tests/testdata/nonmem/pheno_real_linbase.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/add_etas_linbase.dta` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/add_etas_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/add_etas_linbase.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/add_etas_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/add_etas_linbase.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/add_etas_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/add_etas_linbase.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/add_etas_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/boxcox.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/boxcox.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/boxcox.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/boxcox.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/boxcox.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/boxcox.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/boxcox.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/boxcox.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/cdd_results.json` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/cdd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/fullblock.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/fullblock.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/fullblock.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/fullblock.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/fullblock.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/fullblock.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/fullblock.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/fullblock.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/iov.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/iov.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/iov.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/iov.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/iov.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/iov.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/iov.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/iov.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/pheno_linbase.dta` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/pheno_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/pheno_linbase.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/pheno_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/pheno_linbase.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/pheno_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/pheno_linbase.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/pheno_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/pheno_linbase.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/pheno_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/resmod_results.json` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/resmod_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/scm_results.json` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/scm_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/simeval_results.json` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/simeval_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/tdist.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/tdist.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/tdist.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/tdist.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/tdist.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/tdist.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/qa/tdist.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/qa/tdist.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/ruvsearch/mox3.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/ruvsearch/mox3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/ruvsearch/mox3.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/ruvsearch/mox3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/ruvsearch/mox3.mod` & `pharmpy-core-0.93.0/tests/testdata/nonmem/ruvsearch/mox3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/ruvsearch/mox3.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/ruvsearch/mox3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv` & `pharmpy-core-0.93.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/ruvsearch/mytab` & `pharmpy-core-0.93.0/tests/testdata/nonmem/ruvsearch/mytab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/localmin.logf` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/localmin.logf`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/meta.yaml` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt` & `pharmpy-core-0.93.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/sdtab1` & `pharmpy-core-0.93.0/tests/testdata/nonmem/sdtab1`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/pheno.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/pheno.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/pheno.dta` & `pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/pheno.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/pheno.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/pheno.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run1.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run1.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run1.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run1.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run2.cov` & `pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run2.ext` & `pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run2.lst` & `pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/nonmem/secondary_parameters/run2.phi` & `pharmpy-core-0.93.0/tests/testdata/nonmem/secondary_parameters/run2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/pheno_data.csv` & `pharmpy-core-0.93.0/tests/testdata/pheno_data.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/est_data0.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/est_data0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/est_data1.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/est_data1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/est_data2.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/est_data2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/est_data3.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/est_data3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/meta.yaml` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/pred_data0.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/pred_data0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/pred_data1.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/pred_data1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/pred_data2.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/pred_data2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/pred_data3.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/pred_data3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt` & `pharmpy-core-0.93.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/frem_dataset.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/frem_results.csv` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/frem_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_1.cov` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_1.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_1.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_1.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_2.cor` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_2.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_2.cov` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_2.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_2.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_2.mod` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_2.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3.mod` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/meta.yaml` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/proposal_density.cov` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/proposal_density.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt` & `pharmpy-core-0.93.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/linearize_run/results.json` & `pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/linearize_run/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod` & `pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table` & `pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod` & `pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/qa_dir1/results_summary.yaml` & `pharmpy-core-0.93.0/tests/testdata/psn/qa_dir1/results_summary.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/resmod_dir1/resmod_results.csv` & `pharmpy-core-0.93.0/tests/testdata/psn/resmod_dir1/resmod_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/resmod_dir2/resmod_results.csv` & `pharmpy-core-0.93.0/tests/testdata/psn/resmod_dir2/resmod_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/original.cor` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/original.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/original.cov` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/original.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/original.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/original.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/original.mod` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/original.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/original.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/original.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv` & `pharmpy-core-0.93.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/allometry_results.json` & `pharmpy-core-0.93.0/tests/testdata/results/allometry_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/amd_results.json` & `pharmpy-core-0.93.0/tests/testdata/results/amd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/bootstrap_results.json` & `pharmpy-core-0.93.0/tests/testdata/results/bootstrap_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/cdd_results.json` & `pharmpy-core-0.93.0/tests/testdata/results/cdd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/covsearch_results.json` & `pharmpy-core-0.93.0/tests/testdata/results/covsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/estmethod_results.json` & `pharmpy-core-0.93.0/tests/testdata/results/estmethod_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/iivsearch_results.json` & `pharmpy-core-0.93.0/tests/testdata/results/iivsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/iovsearch_results.json` & `pharmpy-core-0.93.0/tests/testdata/results/iovsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/linearize_results.json` & `pharmpy-core-0.93.0/tests/testdata/results/linearize_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/metadata.json` & `pharmpy-core-0.93.0/tests/testdata/results/metadata.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/modelsearch_results.json` & `pharmpy-core-0.93.0/tests/testdata/results/modelsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/qa_results.json` & `pharmpy-core-0.93.0/tests/testdata/results/qa_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/ruvsearch_results.json` & `pharmpy-core-0.93.0/tests/testdata/results/ruvsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/metadata.json` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/metadata.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/results.csv` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/testdata/results/tool_databases/modelsearch/results.json` & `pharmpy-core-0.93.0/tests/testdata/results/tool_databases/modelsearch/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_allometry.py` & `pharmpy-core-0.93.0/tests/tools/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_amd.py` & `pharmpy-core-0.93.0/tests/tools/test_amd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_bootstrap.py` & `pharmpy-core-0.93.0/tests/tools/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_cdd.py` & `pharmpy-core-0.93.0/tests/tools/test_cdd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_covsearch.py` & `pharmpy-core-0.93.0/tests/tools/test_covsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_estmethod.py` & `pharmpy-core-0.93.0/tests/tools/test_estmethod.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_exports.py` & `pharmpy-core-0.93.0/tests/tools/test_exports.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_frem.py` & `pharmpy-core-0.93.0/tests/tools/test_frem.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 57,CL,1.060138503325679,1.043458933657303,1.1198727965741848
 57,V,0.9713027400777485,0.9613644126949645,1.009755277835067
 58,CL,0.9493585916770979,0.9168219777534304,0.9781229378966473
 58,V,1.0551004552760428,1.0074271830514618,1.0558192686142556
 59,CL,0.976533341560172,0.9298917166331006,0.9915919601050044
 59,V,0.9980614650127685,0.9734701845573707,1.014970713377564
 """
-    correct = pd.read_csv(StringIO(correct), index_col=[0, 1])
+    correct = pd.read_csv(StringIO(correct), dtype={0: 'int32'}, index_col=[0, 1])
     correct.index.set_names(['ID', 'parameter'], inplace=True)
     pd.testing.assert_frame_equal(res.individual_effects, correct)
 
     correct = """parameter,covariate,sd_observed,sd_5th,sd_95th
 CL,none,0.19836380718266122,0.10698386364464521,0.22813605494479994
 CL,APGR,0.1932828383897819,0.08207800471169897,0.22738951605057137
 CL,WGT,0.19363776172900196,0.10259365732821585,0.19906614312476859
@@ -384,15 +384,15 @@
 57,V,0.9946766605413693,0.9476823542166756,1.0074749102503402
 58,CL,0.9912884661387944,0.9823252452775585,1.005189333353676
 58,V,1.0011657907076288,0.9983757554340882,1.0119068964710976
 59,CL,0.9707579766809108,0.9413143707818629,1.017990941398883
 59,V,1.0039597917474488,0.9945015889322739,1.0411260478578415
 """
 
-    correct = pd.read_csv(StringIO(correct), index_col=[0, 1])
+    correct = pd.read_csv(StringIO(correct), dtype={0: 'int32'}, index_col=[0, 1])
     correct.index.set_names(['ID', 'parameter'], inplace=True)
     pd.testing.assert_frame_equal(res.individual_effects, correct)
 
     correct = """parameter,covariate,sd_observed,sd_5th,sd_95th
 CL,none,0.1876414133393799,0.1211647441717813,0.2252670442425513
 CL,WGT,0.1824855585272548,0.1000742727854050,0.1989308616423449
 CL,APGRX,0.1785985176170080,0.1194859118429075,0.2170526201633760
```

### Comparing `pharmpy-core-0.92.0/tests/tools/test_iivsearch.py` & `pharmpy-core-0.93.0/tests/tools/test_iivsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_iovsearch.py` & `pharmpy-core-0.93.0/tests/tools/test_iovsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_linearize.py` & `pharmpy-core-0.93.0/tests/tools/test_linearize.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_mfl.py` & `pharmpy-core-0.93.0/tests/tools/test_mfl.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_ml.py` & `pharmpy-core-0.93.0/tests/tools/test_ml.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_modelfit.py` & `pharmpy-core-0.93.0/tests/tools/test_modelfit.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_modelsearch.py` & `pharmpy-core-0.93.0/tests/tools/test_modelsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_qa.py` & `pharmpy-core-0.93.0/tests/tools/test_qa.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_rankfuncs.py` & `pharmpy-core-0.93.0/tests/tools/test_rankfuncs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_run.py` & `pharmpy-core-0.93.0/tests/tools/test_run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_runtool.py` & `pharmpy-core-0.93.0/tests/tools/test_runtool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_ruvsearch.py` & `pharmpy-core-0.93.0/tests/tools/test_ruvsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_scm.py` & `pharmpy-core-0.93.0/tests/tools/test_scm.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_start_model.py` & `pharmpy-core-0.93.0/tests/tools/test_start_model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_summarize_individuals.py` & `pharmpy-core-0.93.0/tests/tools/test_summarize_individuals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/tools/test_wrap.py` & `pharmpy-core-0.93.0/tests/tools/test_wrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/workflows/test_call.py` & `pharmpy-core-0.93.0/tests/workflows/test_call.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,43 @@
+import warnings
 from uuid import uuid4
 
 import pytest
 
 import pharmpy.workflows.dispatchers
 from pharmpy.config import ConfigurationContext
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.workflows import Task, Workflow, call_workflow, execute_workflow
 
 
+def ignore_scratch_warning():
+    warnings.filterwarnings(
+        "ignore",
+        message=".*creating scratch directories is taking a surprisingly long time",
+        category=UserWarning,
+    )
+
+
 def sub(a, b):
     t1 = Task('t1', lambda: a)
     t2 = Task('t2', lambda: b)
     t3 = Task('t3', lambda x, y: x + y)
     wf = Workflow([t1, t2])
     wf.add_task(t3, predecessors=[t1, t2])
     return wf
 
 
+@pytest.mark.xdist_group(name="workflow")
 def f(context, a, b):
     wf = sub(a, b)
     name = uuid4()
-    return call_workflow(wf, name, context)
+    with warnings.catch_warnings():
+        ignore_scratch_warning()
+        res = call_workflow(wf, name, context)
+    return res
 
 
 def add(a, b):
     t1 = Task('t1', lambda: a)
     t2 = Task('t2', lambda: b)
     t3 = Task('t3', f)
     wf = Workflow([t1, t2], name='add')
@@ -36,20 +49,24 @@
 def test_call_workflow_threaded(tmp_path):
     a, b = 1, 2
     wf = add(a, b)
 
     with ConfigurationContext(pharmpy.workflows.dispatchers.conf, dask_dispatcher='threaded'):
         with chdir(tmp_path):
             with pytest.raises(ValueError, match='No global client found and no address provided'):
-                execute_workflow(wf)
+                with warnings.catch_warnings():
+                    ignore_scratch_warning()
+                    execute_workflow(wf)
 
 
 @pytest.mark.xdist_group(name="workflow")
 def test_call_workflow_distributed(tmp_path):
     a, b = 1, 2
     wf = add(a, b)
 
     with ConfigurationContext(pharmpy.workflows.dispatchers.conf, dask_dispatcher='distributed'):
         with chdir(tmp_path):
-            res = execute_workflow(wf)
+            with warnings.catch_warnings():
+                ignore_scratch_warning()
+                res = execute_workflow(wf)
 
     assert res == a + b
```

### Comparing `pharmpy-core-0.92.0/tests/workflows/test_execute.py` & `pharmpy-core-0.93.0/tests/workflows/test_execute.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from dataclasses import dataclass, replace
 from typing import Optional
 
 import pytest
 
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.model import Results
@@ -12,37 +13,49 @@
 
 # All workflow tests are run by the same xdist test worker
 # This is to limit the number of sporadic failures on GHA on Windows
 # The failures seem like races in dask distributed because the tmp-dir takes to long to create
 # on C: (main drive is D:).
 
 
+def ignore_scratch_warning():
+    warnings.filterwarnings(
+        "ignore",
+        message=".*creating scratch directories is taking a surprisingly long time",
+        category=UserWarning,
+    )
+
+
 @pytest.mark.xdist_group(name="workflow")
 def test_execute_workflow_constant(tmp_path):
     a = lambda: 1  # noqa E731
     t1 = Task('t1', a)
     wf = Workflow([t1], name='test-workflow')
 
     with chdir(tmp_path):
-        res = execute_workflow(wf)
+        with warnings.catch_warnings():
+            ignore_scratch_warning()
+            res = execute_workflow(wf)
 
     assert res == a()
 
 
 @pytest.mark.xdist_group(name="workflow")
 def test_execute_workflow_unary(tmp_path):
     a = lambda: 2  # noqa E731
     f = lambda x: x**2  # noqa E731
     t1 = Task('t1', a)
     t2 = Task('t2', f)
     wf = Workflow([t1], name='test-workflow')
     wf.add_task(t2, predecessors=[t1])
 
     with chdir(tmp_path):
-        res = execute_workflow(wf)
+        with warnings.catch_warnings():
+            ignore_scratch_warning()
+            res = execute_workflow(wf)
 
     assert res == f(a())
 
 
 @pytest.mark.xdist_group(name="workflow")
 def test_execute_workflow_binary(tmp_path):
     a = lambda: 1  # noqa E731
@@ -51,15 +64,17 @@
     t1 = Task('t1', a)
     t2 = Task('t2', b)
     t3 = Task('t3', f)
     wf = Workflow([t1, t2], name='test-workflow')
     wf.add_task(t3, predecessors=[t1, t2])
 
     with chdir(tmp_path):
-        res = execute_workflow(wf)
+        with warnings.catch_warnings():
+            ignore_scratch_warning()
+            res = execute_workflow(wf)
 
     assert res == f(a(), b())
 
 
 @pytest.mark.xdist_group(name="workflow")
 def test_execute_workflow_map_reduce(tmp_path):
     n = 10
@@ -68,15 +83,17 @@
     layer_map = list(map(lambda i: Task(f'f(x{i})', f), range(n)))
     layer_reduce = [Task('reduce', lambda *y: sum(y))]
     wf = Workflow(layer_init, name='test-workflow')
     wf.insert_workflow(Workflow(layer_map))
     wf.insert_workflow(Workflow(layer_reduce))
 
     with chdir(tmp_path):
-        res = execute_workflow(wf)
+        with warnings.catch_warnings():
+            ignore_scratch_warning()
+            res = execute_workflow(wf)
 
     assert res == sum(map(f, range(n)))
 
 
 @pytest.mark.xdist_group(name="workflow")
 def test_execute_workflow_set_bolus_absorption(load_model_for_test, testdata, tmp_path):
     model1 = load_model_for_test(testdata / 'nonmem' / 'modeling' / 'pheno_advan1.mod')
@@ -87,15 +104,17 @@
     t2 = Task('update', set_bolus_absorption)
     t3 = Task('postprocess', lambda x: x)
     wf = Workflow([t1], name='test-workflow')
     wf.insert_workflow(Workflow([t2]))
     wf.insert_workflow(Workflow([t3]))
 
     with chdir(tmp_path):
-        res = execute_workflow(wf)
+        with warnings.catch_warnings():
+            ignore_scratch_warning()
+            res = execute_workflow(wf)
 
     assert res.model_code == advan1_before
 
 
 @pytest.mark.xdist_group(name="workflow")
 def test_execute_workflow_fit_mock(load_model_for_test, testdata, tmp_path):
     models = (
@@ -113,16 +132,17 @@
     process = map(lambda i: Task(f'fit{i}', fit, ofvs[i]), indices)
     wf = Workflow(init, name='test-workflow')
     wf.insert_workflow(Workflow(process))
     gather = Task('gather', lambda *x: x)
     wf.insert_workflow(Workflow([gather]))
 
     with chdir(tmp_path):
-        # res = execute_workflow(wf)
-        execute_workflow(wf)
+        with warnings.catch_warnings():
+            ignore_scratch_warning()
+            execute_workflow(wf)
 
     # FIXME: These cannot be updated in place
     # for orig, fitted, ofv in zip(models, res, ofvs):
     #    assert orig.modelfit_results.ofv == ofv
     #    assert fitted.modelfit_results.ofv == ofv
     #    assert orig.modelfit_results == fitted.modelfit_results
 
@@ -131,15 +151,17 @@
 def test_execute_workflow_results(tmp_path):
     ofv = 3
     mfr = ModelfitResults(ofv=ofv)
 
     wf = Workflow([Task('result', lambda: mfr)], name='test-workflow')
 
     with chdir(tmp_path):
-        res = execute_workflow(wf)
+        with warnings.catch_warnings():
+            ignore_scratch_warning()
+            res = execute_workflow(wf)
 
     assert res.ofv == ofv
     assert not hasattr(res, 'tool_database')
 
 
 @dataclass(frozen=True)
 class MyResults(Results):
@@ -151,28 +173,32 @@
 def test_execute_workflow_results_with_tool_database(tmp_path):
     ofv = 3
     mfr = MyResults(ofv=ofv)
 
     wf = Workflow([Task('result', lambda: mfr)], name='test-workflow')
 
     with chdir(tmp_path):
-        res = execute_workflow(wf)
+        with warnings.catch_warnings():
+            ignore_scratch_warning()
+            res = execute_workflow(wf)
         assert res.tool_database is not None
 
     assert res.ofv == ofv
 
 
 @pytest.mark.xdist_group(name="workflow")
 def test_execute_workflow_results_with_report(testdata, tmp_path):
     mfr = replace(read_results(testdata / 'frem' / 'results.json'), tool_database=None)
 
     wf = Workflow([Task('result', lambda: mfr)], name='test-workflow')
 
     with chdir(tmp_path):
-        res = execute_workflow(wf)
+        with warnings.catch_warnings():
+            ignore_scratch_warning()
+            res = execute_workflow(wf)
         html = res.tool_database.path / 'results.html'
         assert html.is_file()
         assert html.stat().st_size > 500000
 
 
 @pytest.mark.xdist_group(name="workflow")
 def test_local_dispatcher():
```

### Comparing `pharmpy-core-0.92.0/tests/workflows/test_model_database.py` & `pharmpy-core-0.93.0/tests/workflows/test_model_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tests/workflows/test_workflow.py` & `pharmpy-core-0.93.0/tests/workflows/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.92.0/tox.ini` & `pharmpy-core-0.93.0/tox.ini`

 * *Files identical despite different names*

