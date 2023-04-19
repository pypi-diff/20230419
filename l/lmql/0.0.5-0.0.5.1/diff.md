# Comparing `tmp/lmql-0.0.5.tar.gz` & `tmp/lmql-0.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmql-0.0.5.tar", last modified: Mon Apr 17 14:49:12 2023, max compression
+gzip compressed data, was "lmql-0.0.5.1.tar", last modified: Wed Apr 19 15:29:32 2023, max compression
```

## Comparing `lmql-0.0.5.tar` & `lmql-0.0.5.1.tar`

### file list

```diff
@@ -1,230 +1,231 @@
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.881538 lmql-0.0.5/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.861538 lmql-0.0.5/.github/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.861538 lmql-0.0.5/.github/workflows/
--rw-rw-r--   0 luca      (1000) luca      (1000)     1618 2023-04-17 14:48:56.000000 lmql-0.0.5/.github/workflows/lmql-web.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)     2710 2023-04-17 14:48:56.000000 lmql-0.0.5/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.5/LICENSE
--rw-rw-r--   0 luca      (1000) luca      (1000)      140 2023-04-17 14:44:31.000000 lmql-0.0.5/MANIFEST.in
--rw-rw-r--   0 luca      (1000) luca      (1000)     4644 2023-04-17 14:49:12.881538 lmql-0.0.5/PKG-INFO
--rw-rw-r--   0 luca      (1000) luca      (1000)     4214 2023-04-17 14:44:31.000000 lmql-0.0.5/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)       75 2023-04-17 14:44:31.000000 lmql-0.0.5/TODO.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/
--rw-rw-r--   0 luca      (1000) luca      (1000)      638 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/Makefile
--rw-rw-r--   0 luca      (1000) luca      (1000)      444 2023-03-14 15:27:49.000000 lmql-0.0.5/docs/RELEASE.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      799 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/make.bat
--rw-rw-r--   0 luca      (1000) luca      (1000)       81 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/requirements.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/_ext/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5526 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/_ext/lmql_snippets.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.861538 lmql-0.0.5/docs/source/_static/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/_static/css/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5777 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/_static/css/lmql-docs.css
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/_static/images/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/_static/images/lmql.svg
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/_static/js/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2191 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/_static/js/lmql-playground.js
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/_templates/
--rw-rw-r--   0 luca      (1000) luca      (1000)      292 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/_templates/layout.html
--rw-rw-r--   0 luca      (1000) luca      (1000)     1167 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/conf.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1293 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/dev-setup.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     2709 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/index.rst
--rw-rw-r--   0 luca      (1000) luca      (1000)     2484 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/installation.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/language/
--rw-rw-r--   0 luca      (1000) luca      (1000)     7435 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/language/constraints.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     4067 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/language/decoders.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     7850 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/language/functions.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     6566 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/language/models.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8511 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/language/overview.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3676 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/language/scripted_prompts.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/lmql.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)    28444 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/logo.png
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/python/
--rw-rw-r--   0 luca      (1000) luca      (1000)       11 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/python/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    13222 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/python/langchain.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)    75148 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/python/lmql.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)     9213 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/python/python.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     3135 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/quickstart.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/releases/
--rw-rw-r--   0 luca      (1000) luca      (1000)      321 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/releases/release-0.0.5.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      257 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/todo.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      137 2023-03-14 15:27:49.000000 lmql-0.0.5/pyproject.toml
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-04-17 14:44:31.000000 lmql-0.0.5/requirements.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/scripts/
--rw-rw-r--   0 luca      (1000) luca      (1000)      295 2023-04-17 14:44:31.000000 lmql-0.0.5/scripts/activate-dev.sh
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/scripts/conda/
--rw-rw-r--   0 luca      (1000) luca      (1000)      210 2023-04-17 14:48:56.000000 lmql-0.0.5/scripts/conda/requirements-no-gpu.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)      344 2023-04-17 14:48:56.000000 lmql-0.0.5/scripts/conda/requirements.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)      486 2023-03-14 15:27:49.000000 lmql-0.0.5/scripts/pypi-release.sh
--rw-rw-r--   0 luca      (1000) luca      (1000)      817 2023-03-14 15:27:49.000000 lmql-0.0.5/scripts/wheel.sh
--rw-rw-r--   0 luca      (1000) luca      (1000)      826 2023-04-17 14:49:12.885538 lmql-0.0.5/setup.cfg
--rw-rw-r--   0 luca      (1000) luca      (1000)       37 2023-03-14 15:27:49.000000 lmql-0.0.5/setup.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/src/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/src/lmql/
--rw-rw-r--   0 luca      (1000) luca      (1000)     6700 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/__init__.py
--rwxrwxr-x   0 luca      (1000) luca      (1000)     7529 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/cli.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1577 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/demo.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1531 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/http.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.869538 lmql-0.0.5/src/lmql/language/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/language/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    20390 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/language/compiler.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    10194 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/language/fragment_parser.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      979 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/language/qstrings.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1804 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/language/validator.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.869538 lmql-0.0.5/src/lmql/model/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/model/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    24468 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/model/async_generation_utils.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1299 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/model/local_client.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    17924 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/model/serve.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     8387 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/model/served_model.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.869538 lmql-0.0.5/src/lmql/ops/
--rw-rw-r--   0 luca      (1000) luca      (1000)       93 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ops/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     7565 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ops/follow_map.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    39511 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ops/ops.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    18023 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ops/token_set.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.869538 lmql-0.0.5/src/lmql/runtime/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/runtime/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.869538 lmql-0.0.5/src/lmql/runtime/bopenai/
--rw-rw-r--   0 luca      (1000) luca      (1000)     1863 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/runtime/bopenai/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    25946 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/bopenai/batched_openai.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    17000 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/runtime/bopenai/openai_api.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.869538 lmql-0.0.5/src/lmql/runtime/dclib/
--rw-rw-r--   0 luca      (1000) luca      (1000)      467 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/runtime/dclib/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    18632 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/runtime/dclib/dclib_array.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      538 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/runtime/dclib/dclib_global.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    27495 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/dclib/dclib_model.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    29933 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/dclib/dclib_seq.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    20646 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/dclib/decoders.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4144 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/dclib/trie_cache.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3176 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/hf_integration.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    27888 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/interpreter.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      250 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/runtime/interrupt.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1084 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/runtime/langchain.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     6049 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/lmql_runtime.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1186 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/runtime/maiohttp.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      732 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/runtime/model_registry.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     5835 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/multi_head_interpretation.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    43100 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/openai_integration.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1971 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/openai_secret.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2437 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/output_writer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.869538 lmql-0.0.5/src/lmql/runtime/postprocessing/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/runtime/postprocessing/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3530 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/postprocessing/conditional_prob.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      152 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/postprocessing/group_by.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1980 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/program_state.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1317 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/stats.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     8456 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/tokenizer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.873538 lmql-0.0.5/src/lmql/tests/
--rw-rw-r--   0 luca      (1000) luca      (1000)      319 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/tests/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     5011 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/tests/expr_test_utils.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1611 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/mask_product_test.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2789 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/monotonicity.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      546 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/one_of_tests.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      758 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/sentences_op.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      984 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/starts_with_op_test.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1236 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/stops_at.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      537 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/str_in_str_tests.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.873538 lmql-0.0.5/src/lmql/tests/system/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3402 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/system/basic_use_cases.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4738 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/test_multi_head.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2149 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/tests/test_sample_queries.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3036 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/token_set_test.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.873538 lmql-0.0.5/src/lmql/ui/
--rw-rw-r--   0 luca      (1000) luca      (1000)       27 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.873538 lmql-0.0.5/src/lmql/ui/live/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/live/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     6747 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/live/live.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3256 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/live/live.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3885 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/live/livelib.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      349 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/live/package.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    33701 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/live/yarn.lock
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.873538 lmql-0.0.5/src/lmql/ui/playground/
--rw-rw-r--   0 luca      (1000) luca      (1000)       31 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/.dockerignore
--rw-rw-r--   0 luca      (1000) luca      (1000)       34 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/.env
--rw-rw-r--   0 luca      (1000) luca      (1000)      310 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)      354 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/Dockerfile
--rw-rw-r--   0 luca      (1000) luca      (1000)     3359 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1327 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/package.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.873538 lmql-0.0.5/src/lmql/ui/playground/public/
--rw-rw-r--   0 luca      (1000) luca      (1000)       90 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/_headers
--rw-rw-r--   0 luca      (1000) luca      (1000)     3870 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/favicon.ico
--rw-rw-r--   0 luca      (1000) luca      (1000)     1678 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/public/index.html
--rw-rw-r--   0 luca      (1000) luca      (1000)     2817 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/lmql.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)      306 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/manifest.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.877538 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/
--rw-rw-r--   0 luca      (1000) luca      (1000)  1227728 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/calc.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   295285 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/chat.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   160153 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/cot.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    81768 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/distribution.json
--rw-rw-r--   0 luca      (1000) luca      (1000)     5221 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/hello.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    89531 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/joke.json
--rw-rw-r--   0 luca      (1000) luca      (1000)  1710847 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/kv.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    52748 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/list.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   628184 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/meta.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   264768 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/translation.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   215050 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/wiki.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       67 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/robots.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.877538 lmql-0.0.5/src/lmql/ui/playground/public/snippets/
--rw-rw-r--   0 luca      (1000) luca      (1000)   381736 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   252806 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/public/snippets/json-parsing.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       62 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/ref.py
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/run-in-docker.sh
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.881538 lmql-0.0.5/src/lmql/ui/playground/src/
--rw-rw-r--   0 luca      (1000) luca      (1000)    68636 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/src/App.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      246 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/App.test.js
--rw-rw-r--   0 luca      (1000) luca      (1000)    29983 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/src/CodeScreenshot.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      807 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/Configuration.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     1174 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/DataListView.js
--rw-rw-r--   0 luca      (1000) luca      (1000)    20848 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/src/DecoderGraph.js
--rw-rw-r--   0 luca      (1000) luca      (1000)      329 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/DecodingTree.js
--rw-rw-r--   0 luca      (1000) luca      (1000)       89 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/Embed.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)     9601 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/Explore.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      675 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/SharedState.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3868 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/src/State.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     5763 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/src/ValidationGraph.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)     9360 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/browser_process.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     1163 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/build_info.js
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.881538 lmql-0.0.5/src/lmql/ui/playground/src/editor/
--rw-rw-r--   0 luca      (1000) luca      (1000)     8696 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     4758 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/editor/theme.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      889 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/explore.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     1345 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/graph-layout.css
--rw-rw-r--   0 luca      (1000) luca      (1000)     1698 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/index.css
--rw-rw-r--   0 luca      (1000) luca      (1000)      489 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/index.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     2632 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/logo.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     8104 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/src/queries.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     5990 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/remote_process.js
--rw-rw-r--   0 luca      (1000) luca      (1000)      362 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/reportWebVitals.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     9520 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/screenshot.css
--rw-rw-r--   0 luca      (1000) luca      (1000)      241 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/setupTests.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3466 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/spinner.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     2949 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/tagged-model-result.js
--rw-rw-r--   0 luca      (1000) luca      (1000)   449905 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/yarn.lock
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.881538 lmql-0.0.5/src/lmql/ui/vscode/
--rw-rw-r--   0 luca      (1000) luca      (1000)       76 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/.gitattributes
--rw-rw-r--   0 luca      (1000) luca      (1000)       19 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/.gitignore
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.881538 lmql-0.0.5/src/lmql/ui/vscode/.vscode/
--rw-rw-r--   0 luca      (1000) luca      (1000)      540 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/.vscode/launch.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       66 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/.vscodeignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/vscode/LICENSE
--rw-rw-r--   0 luca      (1000) luca      (1000)      357 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/vscode/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      959 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/language-configuration.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    11532 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/vscode/lmql-vscode.png
--rw-rw-r--   0 luca      (1000) luca      (1000)     1214 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/vscode/package.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.881538 lmql-0.0.5/src/lmql/ui/vscode/syntaxes/
--rw-rw-r--   0 luca      (1000) luca      (1000)      518 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      642 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      853 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/syntaxes/pylmql.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.881538 lmql-0.0.5/src/lmql/utils/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/utils/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     5384 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/utils/graph.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1882 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/utils/nputil.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      113 2023-04-17 14:49:07.000000 lmql-0.0.5/src/lmql/version.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/src/lmql.egg-info/
--rw-rw-r--   0 luca      (1000) luca      (1000)     4644 2023-04-17 14:49:12.000000 lmql-0.0.5/src/lmql.egg-info/PKG-INFO
--rw-rw-r--   0 luca      (1000) luca      (1000)     6371 2023-04-17 14:49:12.000000 lmql-0.0.5/src/lmql.egg-info/SOURCES.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)        1 2023-04-17 14:49:12.000000 lmql-0.0.5/src/lmql.egg-info/dependency_links.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)       39 2023-04-17 14:49:12.000000 lmql-0.0.5/src/lmql.egg-info/entry_points.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-04-17 14:49:12.000000 lmql-0.0.5/src/lmql.egg-info/requires.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)        5 2023-04-17 14:49:12.000000 lmql-0.0.5/src/lmql.egg-info/top_level.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)   115785 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql.svg
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.767986 lmql-0.0.5.1/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.747986 lmql-0.0.5.1/.github/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/.github/workflows/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1618 2023-04-17 14:48:56.000000 lmql-0.0.5.1/.github/workflows/lmql-web.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2733 2023-04-19 15:28:18.000000 lmql-0.0.5.1/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.5.1/LICENSE
+-rw-rw-r--   0 luca      (1000) luca      (1000)      140 2023-04-17 14:44:31.000000 lmql-0.0.5.1/MANIFEST.in
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4646 2023-04-19 15:29:32.767986 lmql-0.0.5.1/PKG-INFO
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4215 2023-04-18 06:55:18.000000 lmql-0.0.5.1/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)       75 2023-04-17 14:44:31.000000 lmql-0.0.5.1/TODO.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      638 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/Makefile
+-rw-rw-r--   0 luca      (1000) luca      (1000)      444 2023-03-14 15:27:49.000000 lmql-0.0.5.1/docs/RELEASE.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      799 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/make.bat
+-rw-rw-r--   0 luca      (1000) luca      (1000)       81 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/requirements.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/_ext/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5526 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/_ext/lmql_snippets.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.747986 lmql-0.0.5.1/docs/source/_static/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/_static/css/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5777 2023-04-17 14:48:56.000000 lmql-0.0.5.1/docs/source/_static/css/lmql-docs.css
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/_static/images/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/_static/images/lmql.svg
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/_static/js/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2191 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/_static/js/lmql-playground.js
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/_templates/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      292 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/_templates/layout.html
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1167 2023-04-17 14:48:56.000000 lmql-0.0.5.1/docs/source/conf.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1293 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/dev-setup.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2709 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/index.rst
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2484 2023-04-18 06:55:18.000000 lmql-0.0.5.1/docs/source/installation.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/language/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7435 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/language/constraints.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4067 2023-04-17 14:48:56.000000 lmql-0.0.5.1/docs/source/language/decoders.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7850 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/language/functions.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6564 2023-04-18 06:55:18.000000 lmql-0.0.5.1/docs/source/language/models.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8507 2023-04-18 06:55:18.000000 lmql-0.0.5.1/docs/source/language/overview.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3676 2023-04-18 06:55:18.000000 lmql-0.0.5.1/docs/source/language/scripted_prompts.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/lmql.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)    28444 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/logo.png
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/python/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       11 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/python/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    10831 2023-04-18 06:55:18.000000 lmql-0.0.5.1/docs/source/python/langchain.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)    75148 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/python/lmql.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8847 2023-04-19 15:28:18.000000 lmql-0.0.5.1/docs/source/python/python.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3135 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/quickstart.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/releases/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1078 2023-04-18 06:55:18.000000 lmql-0.0.5.1/docs/source/releases/misc-snippets.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      321 2023-04-17 14:48:56.000000 lmql-0.0.5.1/docs/source/releases/release-0.0.5.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      257 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/todo.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      137 2023-03-14 15:27:49.000000 lmql-0.0.5.1/pyproject.toml
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-04-17 14:44:31.000000 lmql-0.0.5.1/requirements.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/scripts/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      295 2023-04-17 14:44:31.000000 lmql-0.0.5.1/scripts/activate-dev.sh
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/scripts/conda/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      210 2023-04-19 15:28:18.000000 lmql-0.0.5.1/scripts/conda/requirements-no-gpu.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)      344 2023-04-19 15:28:18.000000 lmql-0.0.5.1/scripts/conda/requirements.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)      486 2023-03-14 15:27:49.000000 lmql-0.0.5.1/scripts/pypi-release.sh
+-rw-rw-r--   0 luca      (1000) luca      (1000)      817 2023-03-14 15:27:49.000000 lmql-0.0.5.1/scripts/wheel.sh
+-rw-rw-r--   0 luca      (1000) luca      (1000)      828 2023-04-19 15:29:32.771986 lmql-0.0.5.1/setup.cfg
+-rw-rw-r--   0 luca      (1000) luca      (1000)       37 2023-03-14 15:27:49.000000 lmql-0.0.5.1/setup.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/src/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/src/lmql/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6807 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/__init__.py
+-rwxrwxr-x   0 luca      (1000) luca      (1000)     7529 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/cli.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1577 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/demo.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1531 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/http.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql/language/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/language/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21177 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/language/compiler.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    10194 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/language/fragment_parser.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      979 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/language/qstrings.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1804 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/language/validator.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql/model/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/model/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    24468 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/model/async_generation_utils.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1299 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/model/local_client.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    17924 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/model/serve.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8387 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/model/served_model.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql/ops/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       93 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ops/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7565 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ops/follow_map.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    39794 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/ops/ops.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    18121 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/ops/token_set.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql/runtime/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/runtime/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql/runtime/bopenai/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1972 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/runtime/bopenai/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    25946 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/bopenai/batched_openai.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    17000 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/runtime/bopenai/openai_api.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql/runtime/dclib/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      467 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/runtime/dclib/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    18632 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_array.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      538 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_global.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    27495 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_model.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    29933 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_seq.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    20646 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/dclib/decoders.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4144 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/dclib/trie_cache.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3176 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/hf_integration.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    27896 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/runtime/interpreter.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      250 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/runtime/interrupt.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1084 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/runtime/langchain.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6076 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/runtime/lmql_runtime.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1186 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/runtime/maiohttp.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      732 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/runtime/model_registry.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5835 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/multi_head_interpretation.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    43100 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/openai_integration.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1971 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/openai_secret.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2437 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/output_writer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql/runtime/postprocessing/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/runtime/postprocessing/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3530 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/postprocessing/conditional_prob.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      152 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/postprocessing/group_by.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1980 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/program_state.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1317 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/stats.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8563 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/runtime/tokenizer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.759986 lmql-0.0.5.1/src/lmql/tests/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      319 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/tests/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5011 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/tests/expr_test_utils.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1611 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/mask_product_test.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2789 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/monotonicity.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      546 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/one_of_tests.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      758 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/sentences_op.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      984 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/starts_with_op_test.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1236 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/stops_at.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      537 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/str_in_str_tests.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.759986 lmql-0.0.5.1/src/lmql/tests/system/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3402 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/system/basic_use_cases.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4738 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/test_multi_head.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2149 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/tests/test_sample_queries.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3036 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/token_set_test.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.759986 lmql-0.0.5.1/src/lmql/ui/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       27 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.759986 lmql-0.0.5.1/src/lmql/ui/live/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/live/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6747 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/live/live.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3256 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/live/live.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3885 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/live/livelib.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      349 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/live/package.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    33701 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/live/yarn.lock
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.759986 lmql-0.0.5.1/src/lmql/ui/playground/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       31 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/.dockerignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)       34 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/.env
+-rw-rw-r--   0 luca      (1000) luca      (1000)      310 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)      354 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/Dockerfile
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3359 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1327 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/package.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.759986 lmql-0.0.5.1/src/lmql/ui/playground/public/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       90 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/_headers
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3870 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/favicon.ico
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1678 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/index.html
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2817 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/lmql.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)      306 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/manifest.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.763986 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/
+-rw-rw-r--   0 luca      (1000) luca      (1000)  1227728 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/calc.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   295285 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/chat.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   160153 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/cot.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    81768 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/distribution.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5221 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/hello.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    89531 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/joke.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)  1710847 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/kv.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    52748 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/list.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   628184 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/meta.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   264768 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/translation.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   215050 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/wiki.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       67 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/robots.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.763986 lmql-0.0.5.1/src/lmql/ui/playground/public/snippets/
+-rw-rw-r--   0 luca      (1000) luca      (1000)   381736 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   252806 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/snippets/json-parsing.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       62 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/ref.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/run-in-docker.sh
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.767986 lmql-0.0.5.1/src/lmql/ui/playground/src/
+-rw-rw-r--   0 luca      (1000) luca      (1000)    68636 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/App.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      246 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/App.test.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)    29983 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/CodeScreenshot.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      807 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/Configuration.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1174 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/DataListView.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)    20848 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/DecoderGraph.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)      329 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/DecodingTree.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)       89 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/Embed.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9601 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/Explore.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      675 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/SharedState.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3868 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/State.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5763 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/ValidationGraph.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9360 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/browser_process.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1163 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/build_info.js
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.767986 lmql-0.0.5.1/src/lmql/ui/playground/src/editor/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8696 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4758 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/editor/theme.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      889 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/explore.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1345 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/graph-layout.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1698 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/index.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)      489 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/index.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2632 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/logo.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8104 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/queries.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5990 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/remote_process.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)      362 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/reportWebVitals.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9520 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/screenshot.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)      241 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/setupTests.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3466 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/spinner.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2949 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/tagged-model-result.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)   449905 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/yarn.lock
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.767986 lmql-0.0.5.1/src/lmql/ui/vscode/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       76 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/.gitattributes
+-rw-rw-r--   0 luca      (1000) luca      (1000)       19 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/.gitignore
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.767986 lmql-0.0.5.1/src/lmql/ui/vscode/.vscode/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      540 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/.vscode/launch.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       66 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/.vscodeignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/vscode/LICENSE
+-rw-rw-r--   0 luca      (1000) luca      (1000)      357 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/vscode/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      959 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/language-configuration.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    11532 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/vscode/lmql-vscode.png
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1214 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/vscode/package.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.767986 lmql-0.0.5.1/src/lmql/ui/vscode/syntaxes/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      518 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      642 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      853 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/syntaxes/pylmql.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.767986 lmql-0.0.5.1/src/lmql/utils/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/utils/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5384 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/utils/graph.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1882 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/utils/nputil.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      115 2023-04-19 15:29:27.000000 lmql-0.0.5.1/src/lmql/version.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql.egg-info/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4646 2023-04-19 15:29:32.000000 lmql-0.0.5.1/src/lmql.egg-info/PKG-INFO
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6409 2023-04-19 15:29:32.000000 lmql-0.0.5.1/src/lmql.egg-info/SOURCES.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)        1 2023-04-19 15:29:32.000000 lmql-0.0.5.1/src/lmql.egg-info/dependency_links.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)       39 2023-04-19 15:29:32.000000 lmql-0.0.5.1/src/lmql.egg-info/entry_points.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-04-19 15:29:32.000000 lmql-0.0.5.1/src/lmql.egg-info/requires.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)        5 2023-04-19 15:29:32.000000 lmql-0.0.5.1/src/lmql.egg-info/top_level.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)   115785 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql.svg
```

### Comparing `lmql-0.0.5/.github/workflows/lmql-web.yml` & `lmql-0.0.5.1/.github/workflows/lmql-web.yml`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/.gitignore` & `lmql-0.0.5.1/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -167,7 +167,8 @@
 # Cython debug symbols
 cython_debug/
 
 # End of https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks
 
 wip-snippets
 .vscode
+.lmql-algorithms-cache
```

### Comparing `lmql-0.0.5/LICENSE` & `lmql-0.0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/PKG-INFO` & `lmql-0.0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.5
+Version: 0.0.5.1
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -34,36 +34,37 @@
     <br/>
   </p>
 </div>
 
 LMQL is a query language for large language models (LLMs). It facilitates LLM interaction by combining the benefits of natural language prompting with the expressiveness of Python. With only a few lines of LMQL code, users can express advanced, multi-part and tool-augmented LM queries, which then are optimized by the LMQL runtime to run efficiently as part of the LM decoding loop.
 
 ![lmql-overview](https://user-images.githubusercontent.com/17903049/222918379-84a00b9a-1ef0-45bf-9384-15a20f2874f0.png)
+
 <p align="center">Example of a simple LMQL program.</p>
 
 
 ## Getting Started
 
 To install the latest version of LMQL run the following command with Python >=3.10 installed.
 
 ```
 pip install lmql
 ```
 
-**Local GPU Support:** If you want to run models on a local GPU, make sure to install LMQL in an environment with a GPU-enabled installation of PyTorch >= 1.11 (cf. https://pytorch.org/get-started/locally/). 
+**Local GPU Support:** If you want to run models on a local GPU, make sure to install LMQL in an environment with a GPU-enabled installation of PyTorch >= 1.11 (cf. https://pytorch.org/get-started/locally/).
 
 ### Running LMQL Programs
 
 After installation, you can launch the LMQL playground IDE with the following command:
 
 ```
 lmql playground
 ```
 
-> Using the LMQL playground requires an installation of Node.js. If you are in a conda-managed environment you can install node.js via `conda install nodejs=14.20 -c conda-forge`. Otherwise, please see the offical Node.js website https://nodejs.org/en/download/ for instructions how to install it on your system.
+> Using the LMQL playground requires an installation of Node.js. If you are in a conda-managed environment you can install node.js via `conda install nodejs=14.20 -c conda-forge`. Otherwise, please see the official Node.js website https://nodejs.org/en/download/ for instructions how to install it on your system.
 
 This launches a browser-based playground IDE, including a showcase of many exemplary LMQL programs. If the IDE does not launch automatically, go to `http://localhost:3000`.
 
 Alternatively, `lmql run` can be used to execute local `.lmql` files. Note that when using local HuggingFace Transformers models in the Playground IDE or via `lmql run`, you have to first launch an instance of the LMQL Inference API for the corresponding model via the command `lmql serve-model`.
 
 ### Configuring OpenAI API Credentials
 
@@ -89,15 +90,15 @@
 source scripts/activate-dev.sh
 ```
 
 > **Operating System**: The GPU-enabled version of LMQL was tested to work on Ubuntu 22.04 with CUDA 12.0 and Windows 10 via WSL2 and CUDA 11.7. The no-GPU version (see below) was tested to work on Ubuntu 22.04 and macOS 13.2 Ventura or Windows 10 via WSL2.
 
 ### Development without GPU
 
-This section outlines how to setup an LMQL development environment without local GPU support. Note that LMQL without local GPU support only supports the use of API-integrated models like `openai/text-davinci-003`. Please see the OpenAI API documentation (https://platform.openai.com/docs/models/gpt-3-5) to learn more about the set of available models. 
+This section outlines how to setup an LMQL development environment without local GPU support. Note that LMQL without local GPU support only supports the use of API-integrated models like `openai/text-davinci-003`. Please see the OpenAI API documentation (https://platform.openai.com/docs/models/gpt-3-5) to learn more about the set of available models.
 
 To setup a `conda` environment for LMQL with GPU support, run the following commands:
 
 ```
 # prepare conda environment
 conda env create -f scripts/conda/requirements-no-gpu.yml -n lmql-no-gpu
 conda activate lmql-no-gpu
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.5 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.5.1 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
@@ -24,15 +24,15 @@
 Support:** If you want to run models on a local GPU, make sure to install LMQL
 in an environment with a GPU-enabled installation of PyTorch >= 1.11 (cf.
 https://pytorch.org/get-started/locally/). ### Running LMQL Programs After
 installation, you can launch the LMQL playground IDE with the following
 command: ``` lmql playground ``` > Using the LMQL playground requires an
 installation of Node.js. If you are in a conda-managed environment you can
 install node.js via `conda install nodejs=14.20 -c conda-forge`. Otherwise,
-please see the offical Node.js website https://nodejs.org/en/download/ for
+please see the official Node.js website https://nodejs.org/en/download/ for
 instructions how to install it on your system. This launches a browser-based
 playground IDE, including a showcase of many exemplary LMQL programs. If the
 IDE does not launch automatically, go to `http://localhost:3000`.
 Alternatively, `lmql run` can be used to execute local `.lmql` files. Note that
 when using local HuggingFace Transformers models in the Playground IDE or via
 `lmql run`, you have to first launch an instance of the LMQL Inference API for
 the corresponding model via the command `lmql serve-model`. ### Configuring
```

### Comparing `lmql-0.0.5/README.md` & `lmql-0.0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,36 +20,37 @@
     <br/>
   </p>
 </div>
 
 LMQL is a query language for large language models (LLMs). It facilitates LLM interaction by combining the benefits of natural language prompting with the expressiveness of Python. With only a few lines of LMQL code, users can express advanced, multi-part and tool-augmented LM queries, which then are optimized by the LMQL runtime to run efficiently as part of the LM decoding loop.
 
 ![lmql-overview](https://user-images.githubusercontent.com/17903049/222918379-84a00b9a-1ef0-45bf-9384-15a20f2874f0.png)
+
 <p align="center">Example of a simple LMQL program.</p>
 
 
 ## Getting Started
 
 To install the latest version of LMQL run the following command with Python >=3.10 installed.
 
 ```
 pip install lmql
 ```
 
-**Local GPU Support:** If you want to run models on a local GPU, make sure to install LMQL in an environment with a GPU-enabled installation of PyTorch >= 1.11 (cf. https://pytorch.org/get-started/locally/). 
+**Local GPU Support:** If you want to run models on a local GPU, make sure to install LMQL in an environment with a GPU-enabled installation of PyTorch >= 1.11 (cf. https://pytorch.org/get-started/locally/).
 
 ### Running LMQL Programs
 
 After installation, you can launch the LMQL playground IDE with the following command:
 
 ```
 lmql playground
 ```
 
-> Using the LMQL playground requires an installation of Node.js. If you are in a conda-managed environment you can install node.js via `conda install nodejs=14.20 -c conda-forge`. Otherwise, please see the offical Node.js website https://nodejs.org/en/download/ for instructions how to install it on your system.
+> Using the LMQL playground requires an installation of Node.js. If you are in a conda-managed environment you can install node.js via `conda install nodejs=14.20 -c conda-forge`. Otherwise, please see the official Node.js website https://nodejs.org/en/download/ for instructions how to install it on your system.
 
 This launches a browser-based playground IDE, including a showcase of many exemplary LMQL programs. If the IDE does not launch automatically, go to `http://localhost:3000`.
 
 Alternatively, `lmql run` can be used to execute local `.lmql` files. Note that when using local HuggingFace Transformers models in the Playground IDE or via `lmql run`, you have to first launch an instance of the LMQL Inference API for the corresponding model via the command `lmql serve-model`.
 
 ### Configuring OpenAI API Credentials
 
@@ -75,19 +76,19 @@
 source scripts/activate-dev.sh
 ```
 
 > **Operating System**: The GPU-enabled version of LMQL was tested to work on Ubuntu 22.04 with CUDA 12.0 and Windows 10 via WSL2 and CUDA 11.7. The no-GPU version (see below) was tested to work on Ubuntu 22.04 and macOS 13.2 Ventura or Windows 10 via WSL2.
 
 ### Development without GPU
 
-This section outlines how to setup an LMQL development environment without local GPU support. Note that LMQL without local GPU support only supports the use of API-integrated models like `openai/text-davinci-003`. Please see the OpenAI API documentation (https://platform.openai.com/docs/models/gpt-3-5) to learn more about the set of available models. 
+This section outlines how to setup an LMQL development environment without local GPU support. Note that LMQL without local GPU support only supports the use of API-integrated models like `openai/text-davinci-003`. Please see the OpenAI API documentation (https://platform.openai.com/docs/models/gpt-3-5) to learn more about the set of available models.
 
 To setup a `conda` environment for LMQL with GPU support, run the following commands:
 
 ```
 # prepare conda environment
 conda env create -f scripts/conda/requirements-no-gpu.yml -n lmql-no-gpu
 conda activate lmql-no-gpu
 
 # registers the `lmql` command in the current shell
 source scripts/activate-dev.sh
-```
+```
```

#### html2text {}

```diff
@@ -18,15 +18,15 @@
 Support:** If you want to run models on a local GPU, make sure to install LMQL
 in an environment with a GPU-enabled installation of PyTorch >= 1.11 (cf.
 https://pytorch.org/get-started/locally/). ### Running LMQL Programs After
 installation, you can launch the LMQL playground IDE with the following
 command: ``` lmql playground ``` > Using the LMQL playground requires an
 installation of Node.js. If you are in a conda-managed environment you can
 install node.js via `conda install nodejs=14.20 -c conda-forge`. Otherwise,
-please see the offical Node.js website https://nodejs.org/en/download/ for
+please see the official Node.js website https://nodejs.org/en/download/ for
 instructions how to install it on your system. This launches a browser-based
 playground IDE, including a showcase of many exemplary LMQL programs. If the
 IDE does not launch automatically, go to `http://localhost:3000`.
 Alternatively, `lmql run` can be used to execute local `.lmql` files. Note that
 when using local HuggingFace Transformers models in the Playground IDE or via
 `lmql run`, you have to first launch an instance of the LMQL Inference API for
 the corresponding model via the command `lmql serve-model`. ### Configuring
```

### Comparing `lmql-0.0.5/docs/Makefile` & `lmql-0.0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/make.bat` & `lmql-0.0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/source/_ext/lmql_snippets.py` & `lmql-0.0.5.1/docs/source/_ext/lmql_snippets.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/source/_static/css/lmql-docs.css` & `lmql-0.0.5.1/docs/source/_static/css/lmql-docs.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/source/_static/images/lmql.svg` & `lmql-0.0.5.1/docs/source/_static/images/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/source/_static/js/lmql-playground.js` & `lmql-0.0.5.1/docs/source/_static/js/lmql-playground.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/source/conf.py` & `lmql-0.0.5.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/source/dev-setup.md` & `lmql-0.0.5.1/docs/source/dev-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/source/index.rst` & `lmql-0.0.5.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/source/installation.md` & `lmql-0.0.5.1/docs/source/installation.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,47 +4,47 @@
 
 To install the latest version of LMQL locally, run the following command with Python >=3.10 installed.
 
 ```
 pip install lmql
 ```
 
-**Local GPU Support:** If you want to run models on a local GPU, make sure to install LMQL in an environment with a GPU-enabled installation of PyTorch >= 1.11 (cf. [https://pytorch.org/get-started/locally/]()). 
+**Local GPU Support:** If you want to run models on a local GPU, make sure to install LMQL in an environment with a GPU-enabled installation of PyTorch >= 1.11 (cf. [https://pytorch.org/get-started/locally/]()).
 
 ## Running LMQL Programs
 
 **Playground**
 
 After installation, you can launch a local instance of the Playground IDE using the following command:
 
 ```
 lmql playground
 ```
 
-> Using **the LMQL playground requires an installation of Node.js**. If you are in a conda-managed environment you can install node.js via `conda install nodejs=14.20 -c conda-forge`. Otherwise, please see the offical [Node.js website](https://nodejs.org/en/download/) for instructions on how to install it on your system.
+> Using **the LMQL playground requires an installation of Node.js**. If you are in a conda-managed environment you can install node.js via `conda install nodejs=14.20 -c conda-forge`. Otherwise, please see the official [Node.js website](https://nodejs.org/en/download/) for instructions on how to install it on your system.
 
 This launches a browser-based Playground IDE, including a showcase of many exemplary LMQL programs. If the IDE does not launch automatically, go to `http://localhost:3000`.
 
 **Command-Line Interface**
 
 As an alternative to the playground, the command-line tool `lmql run` can be used to execute local `.lmql` files.
 
 **Python Integration**
 
-LMQL can also be used directly from within Python. To use LMQL in Python, you can import the `lmql` package, run query code via `lmql.run` or use a decorator `@lmql.query` for LMQL query functions. 
+LMQL can also be used directly from within Python. To use LMQL in Python, you can import the `lmql` package, run query code via `lmql.run` or use a decorator `@lmql.query` for LMQL query functions.
 
 For more details, please see the [Python Integration](./python/python.ipynb) chapter.
 
 ## Self-Hosted Models
 
 Note that when using local [🤗 Transformers](https://huggingface.co/transformers) models in the Playground IDE or via `lmql run`, you have to first launch an instance of the LMQL Inference API for the corresponding model via the command `lmql serve-model`. For more details, please see [Models](./language/models.md) chapter.
 
 ## Configuring OpenAI API Credentials
 
-If you want to use OpenAI models, you have to configure your API credentials. To do so you can either define the `OPENAI_API_KEY` enviornment variable or create a file `api.env` in the active working directory, with the following contents.
+If you want to use OpenAI models, you have to configure your API credentials. To do so you can either define the `OPENAI_API_KEY` environment variable or create a file `api.env` in the active working directory, with the following contents.
 
 ```
 openai-org: <org identifier>
 openai-secret: <api secret>
 ```
 
-For system-wide configuration, you can also create an `api.env` file at `$HOME/.lmql/api.env` or at the project root of your LMQL distribution (e.g. `src/` in a development copy).
+For system-wide configuration, you can also create an `api.env` file at `$HOME/.lmql/api.env` or at the project root of your LMQL distribution (e.g. `src/` in a development copy).
```

### Comparing `lmql-0.0.5/docs/source/language/constraints.md` & `lmql-0.0.5.1/docs/source/language/constraints.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/source/language/decoders.md` & `lmql-0.0.5.1/docs/source/language/decoders.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/source/language/functions.md` & `lmql-0.0.5.1/docs/source/language/functions.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/source/language/models.md` & `lmql-0.0.5.1/docs/source/language/models.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 * The **OpenAI Completions API only provides the top-5 logprobs per predicted token**. This means that decoding algorithms that explore e.g. the top-n probabilities to make decisions like beam search, are limited to a branching factor of 5.
 
 * The **OpenAI Chat API does not provide any way to mask tokens or obtain the token distribution (ChatGPT, GPT-4)**. Simple constraints can still be enforced, as the LMQL runtime optimizes them to fit the OpenAI API. However, more complex constraints may not be enforceable. In these cases, LMQL will print a error message to the console. As a workaround users may then adjust their constraints to fit these API limitations or resort to post-processing and backtracking. Scripted prompting, intermediate instructions and simple constraints are still supported with Chat API models, nonetheless.
 
 ### Configuring OpenAI API Credentials
 
-If you want to use OpenAI models, you have to configure your API credentials. To do so you can either define the `OPENAI_API_KEY` enviornment variable or create a file `api.env` in the active working directory, with the following contents.
+If you want to use OpenAI models, you have to configure your API credentials. To do so you can either define the `OPENAI_API_KEY` environment variable or create a file `api.env` in the active working directory, with the following contents.
 
 ```
 openai-org: <org identifier>
 openai-secret: <api secret>
 ```
 
 For system-wide configuration, you can also create an `api.env` file at `$HOME/.lmql/api.env` or at the project root of your LMQL distribution (e.g. `src/` in a development copy).
@@ -79,9 +79,7 @@
 This exposes the LMQL inference API on port 8080. When serving a model remotely, make sure to tunnel/forward the port to your client machine.
 
 Now, when executing an LMQL query in the playground or via the CLI, you can simply specify e.g. `gpt2-medium`, and the runtime will automatically connect to the model server running on port 8080 to obtain model predictions.
 
 #### Running The Playground Remotely
 
 If you would like to run the LMQL Playground itself remotely (e.g. for latency reasons), you can do so using a similar port forwarding/tunnel setup as described above. For this, make sure you client browser has access to the Playground server ports `3000` and `3004`.
-
-
```

### Comparing `lmql-0.0.5/docs/source/language/overview.md` & `lmql-0.0.5.1/docs/source/language/overview.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Overview
 
 LMQL is a declarative, SQL-like programming language for language model interaction. As an example consider the following query, demonstrating the basic syntax of LMQL:
- 
+
 ```{lmql}
 
 name::overview-query
 argmax
    """Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.
    Q: What is the underlying sentiment of this review and why?
    A:[ANALYSIS]
    Based on this, the overall sentiment of the message can be considered to be[CLASSIFICATION]"""
-from 
+from
    "openai/text-davinci-003"
 where
    not "\n" in ANALYSIS and CLASSIFICATION in [" positive", " neutral", " negative"]
 
 model-output::
 Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.⏎
 Q: What is the underlying sentiment of this review and why?⏎
@@ -25,54 +25,59 @@
 In this program, we use the language model `openai/text-davinci-003` (GPT-3.5) to perform a sentiment analysis on a provided user review. We first ask the model to provide some basic analysis of the review, and then we ask the model to classify the overall sentiment as one of `positive`, `neutral`, or `negative`. The model is able to correctly identify the sentiment of the review as `positive`.
 
 Overall, the query consists of four main clauses:
 
 1. **Decoder Clause** First, we specify the decoding algorithm to use for text generation. In this case we use `argmax` decoding, however, LMQL also support branching decoding algorithms like beam search. See [Decoders](./decoders.md) to learn more about this.
 
 2. **Prompt Clause**
-    ```python
-    """Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.
+
+   ```python
+   """Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.
    Q: What is the underlying sentiment of this review and why?
    A:[ANALYSIS]
    Based on this, the overall sentiment of the message can be considered to be[CLASSIFICATION]"""
    ```
-    In this part of the program, you specify your prompt. Here, we include the user review, as well as the two questions we want to ask the model. Template variables like `[ANALYSIS]` are automatically completed by the model. Apart from simple textual prompts, LMQL also support multi-part and scripted prompts. To learn more, see [Scripted Prompting](./scripted_prompts.md).
+
+   In this part of the program, you specify your prompt. Here, we include the user review, as well as the two questions we want to ask the model. Template variables like `[ANALYSIS]` are automatically completed by the model. Apart from simple textual prompts, LMQL also support multi-part and scripted prompts. To learn more, see [Scripted Prompting](./scripted_prompts.md).
 
 3. **Model Clause**
+
     ```python
     from "openai/text-davinci-003"
     ```
+
     Next, we specify what model we want to use for text generation. In this case, we use the language model `openai/text-davinci-003`. To learn more about the different models available in LMQL, see [Models](./models.md).
 
 4. **Constraint Clause**
+
     ```python
     not "\n" in ANALYSIS and CLASSIFICATION in [" positive", " neutral", " negative"]
     ```
+
     In this part of the query, users can specify logical, high-level constraints on the generated text.<br>
     
     Here, we specify two constraints: For `ANALYSIS` we constrain the model to not output any newlines, which prevents the model from outputting multiple lines, which could potentially breaking the prompt. For `CLASSIFICATION` we constrain the model to output one of the three possible values. Using these constraints allows us to decode a fitting answer from the model, where both the analysis and the classification are well-formed and in an expected format.
 
+   Without constraints, the prompt above could produce different final classifications, such as `good`, `bad`, or `neutral`. To handle this in an automated way, one would again have to employ some model of language understanding to parse the model's CLASSIFICATION result.
 
-    Without constraints, the prompt above could produce different final classifications, such as `good`, `bad`, or `neutral`. To handle this in an automated way, one would again have to employ some model of language understanding to parse the model's CLASSIFICATION result.
-
-    To learn more about the different types of constraints available in LMQL, see [Constraints](./constraints.md).
+   To learn more about the different types of constraints available in LMQL, see [Constraints](./constraints.md).
 
 ### Extracting More Information With Distributions
 
 While the query above allows us to extract the sentiment of a review, we do not get any certainty information on the model's confidence in its classification. To obtain this information, we can additionally employ LMQL's `distribution` clause, to obtain the full distribution over the possible values for `CLASSIFICATION`:
 
 ```{lmql}
 
 name::sentiment-distribution
 argmax
    """Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.
    Q: What is the underlying sentiment of this review and why?
    A:[ANALYSIS]
    Based on this, the overall sentiment of the message can be considered to be[CLASSIFICATION]"""
-from 
+from
    "openai/text-davinci-003"
 where
    not "\n" in ANALYSIS
 distribution
    CLASSIFICATION in [" positive", " neutral", " negative"]
 
 model-output::
@@ -85,17 +90,17 @@
  -  positive (*) 0.9999244826658527
  -  neutral      7.513155848720942e-05
  -  negative     3.8577566019560874e-07
 ```
 
 **Distribution Clause**
 
-Instead of constraining `CLASSIFICATION` as part of the `where` clause, we now constrain in the `distribution` clause. In LMQL, the `distribution` clause is used to specify whether we want to additionally obtain the distribution over the possible values for a given variable. In this case, we want to obtain the distribution over the possible values for `CLASSIFICATION`. 
+Instead of constraining `CLASSIFICATION` as part of the `where` clause, we now constrain in the `distribution` clause. In LMQL, the `distribution` clause is used to specify whether we want to additionally obtain the distribution over the possible values for a given variable. In this case, we want to obtain the distribution over the possible values for `CLASSIFICATION`.
 
-In addition to using the model to perform the `ANALYSIS`, LMQL now also scores each of the individually provided values for `CLASSIFICATION` and normalizes the resulting sequence scores into a probability distribution `P(CLASSIFICATION)` (printed to the Terminal Ouput of the Playground or Standard Output of the CLI).
+In addition to using the model to perform the `ANALYSIS`, LMQL now also scores each of the individually provided values for `CLASSIFICATION` and normalizes the resulting sequence scores into a probability distribution `P(CLASSIFICATION)` (printed to the Terminal Output of the Playground or Standard Output of the CLI).
 
 Here, we can see that the model is indeed quite confident in its classification of the review as `positive`, with an overwhelming probability of `99.9%`.
 
 > Note that currently distribution variables like `CLASSIFICATION` can only occur at the end of a prompt.
 
 ### Dynamically Reacting To Model Output
 
@@ -126,10 +131,10 @@
 A: [ANALYSIS The underlying sentiment of this review is positive because the reviewer had a great stay, enjoyed the hiking and found the food to be good.]⏎
 Based on this, the overall sentiment of the message can be considered to be [CLASSIFICATION positive]⏎
 What is it that they liked about their stay?⏎
 ⏎
 [FURTHER_ANALYSIS The reviewer liked the hiking in the mountains and the food.]
 ```
 
-As shown here, we can use the `if` statement to dynamically react to the model's output. In this case, we ask the model to provide a more detailed analysis of the review, depending on the overally positive, neutral, or negative sentiment of the review. All intermediate variables like `ANALYSIS`, `CLASSIFICATION` or `FURTHER_ANALYSIS` can be considered the output of query, and may be processed by an surrounding automated system. 
+As shown here, we can use the `if` statement to dynamically react to the model's output. In this case, we ask the model to provide a more detailed analysis of the review, depending on the overall positive, neutral, or negative sentiment of the review. All intermediate variables like `ANALYSIS`, `CLASSIFICATION` or `FURTHER_ANALYSIS` can be considered the output of query, and may be processed by an surrounding automated system.
 
-To learn more about the capabilities of such control-flow-guided prompts, see [Scripted Prompting](./scripted_prompts.md).
+To learn more about the capabilities of such control-flow-guided prompts, see [Scripted Prompting](./scripted_prompts.md).
```

### Comparing `lmql-0.0.5/docs/source/language/scripted_prompts.md` & `lmql-0.0.5.1/docs/source/language/scripted_prompts.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Scripted Prompting
 
 In LMQL, prompts are not just static text, as they can also contain control flow (e.g. loops, conditions, function calls). This facilitates dynamic prompt construction and allows LMQL queries to respond dynamically to model output. This scripting mechanic is achieved by a combination of prompt templates, control flow and [output constraining](constraints.md).
 
 **Packing List** For instance, let's say we want to generate a packing list. One way to do this would be the following query:
 
 ```{lmql}
-  
+
 name::list
 sample(temperature=0.8)
    "A few things not to forget when going to the sea (not travelling): \n"
    "[LIST]"
 from
    'openai/text-ada-001'
 
@@ -69,18 +69,18 @@
    STOPS_AT(THING, "\n")
 
 model-output::
 A list of things not to forget when going to the sea (not travelling):
 -[THING A good pair of blue/gel saskaers]
 -[THING A good sun tanner]
 -[THING A good air freshener]
--[THING A good spot forwashing your hands]
+-[THING A good spot for washing your hands]
 -[THING A good spot for washing your feet]
 
-# print output: \['A good pair of blue/gel saskaers', 'A good sun tanner', 'A good air freshener', 'A good spot forwashing your hands', 'A good spot for washing your feet'\]
+# print output: \['A good pair of blue/gel saskaers', 'A good sun tanner', 'A good air freshener', 'A good spot for washing your hands', 'A good spot for washing your feet'\]
 ```
 
 Because we decode our list `THING` by `THING`, we can easily access the individual items, without having to think about parsing or validation. We just add them to a `backpack` list of things, which we then can process further.
 
 ## Python Compatibility
 
 Going beyond simple control flow, LMQL supports most valid Python constructs in the prompt clause of a query, where top-level strings like `"-[THING]"` are automatically interpreted as model input and template variables are assigned accordingly. For more advanced usage, also see the [External Functions](functions.md) chapter.
```

### Comparing `lmql-0.0.5/docs/source/lmql.svg` & `lmql-0.0.5.1/docs/source/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/source/logo.png` & `lmql-0.0.5.1/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/source/python/lmql.txt` & `lmql-0.0.5.1/docs/source/python/lmql.txt`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/docs/source/python/python.ipynb` & `lmql-0.0.5.1/docs/source/python/python.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9888847552910053%*

 * *Differences: {"'cells'": "{4: {'execution_count': 4, 'outputs': {0: {'execution_count': 4}}, 'source': {insert: "*

 * *            '[(4, "    \'\'\'lmql\\n"), (11, "    \'\'\'\\n")], delete: [11, 4]}}, 10: '*

 * *            "{'execution_count': 7, 'source': {insert: [(22, '        STOPS_AT(WHO, "*

 * *            '"\\\\n")\\n\')], delete: [22]}}, delete: [11]}'}*

```diff
@@ -47,41 +47,41 @@
                 "### LMQL as Decorated Python Functions\n",
                 "\n",
                 "To define and run LMQL queries within Python, you can simply decorate a Python function with the `lmql.query` decorator, and provide the query code as a multi-line string. The decorated function will then automatically be compiled into a LMQL query, and can be called with the same arguments as the original Python function. The return value of the decorated function will be the result of the LMQL query."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "'Hello everyone'"
                         ]
                     },
-                    "execution_count": 2,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import lmql\n",
                 "\n",
                 "@lmql.query\n",
                 "async def hello(): \n",
-                "    \"\"\"\n",
+                "    '''lmql\n",
                 "    argmax \n",
                 "        \"Hello[WHO]\" \n",
                 "    from \n",
                 "        \"openai/text-ada-001\" \n",
                 "    where \n",
                 "        len(WHO) < 10\n",
-                "    \"\"\"\n",
+                "    '''\n",
                 "\n",
                 "(await hello())[0].prompt"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -156,15 +156,15 @@
             "metadata": {},
             "source": [
                 "This also allows you to call utility functions, that query external information systems like Wikipedia, and incorporate the obtained information dynamically in your prompt:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Greet Earth (Earth is the third planet from the Sun and the only place known in the universe where life has originated and found habitability): \n",
@@ -192,33 +192,25 @@
                 "    argmax \n",
                 "        \"\"\"Greet {term} ({await look_up(term)}): \n",
                 "        Hello[WHO]\n",
                 "        \"\"\"\n",
                 "    from \n",
                 "        \"openai/text-davinci-003\" \n",
                 "    where \n",
-                "        STOPS_AT(WHO, \"\\\\n\")\n",
+                "        STOPS_AT(WHO, \"\\n\")\n",
                 "    '''\n",
                 "\n",
                 "print((await greet(\"Earth\"))[0].prompt)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "> **Escaping**: When embedding LMQL code in Python, make sure to always use double-escaped special characters like `\\\\n`. Single escaped characters (e.g. just `\\n`) will always be interpreted literally the query code and therefore lead to parser errors. "
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
                 "This capability of calling arbitrary program logic during query execution, enables powerful use cases like the integration of retrieval, as discussed in the [LangChain Integration](./langchain.ipynb) chapter."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `lmql-0.0.5/docs/source/quickstart.md` & `lmql-0.0.5.1/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/scripts/wheel.sh` & `lmql-0.0.5.1/scripts/wheel.sh`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/setup.cfg` & `lmql-0.0.5.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lmql
-version = 0.0.5
+version = 0.0.5.1
 author = Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 author_email = hello@lmql.ai
 description = A query language for language models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://lmql.ai
 project_urls =
```

### Comparing `lmql-0.0.5/src/lmql/__init__.py` & `lmql-0.0.5.1/src/lmql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import lmql.runtime.lmql_runtime as runtime_support
 from lmql.language.compiler import LMQLCompiler
 # re-export lmql runtime functions
 from lmql.runtime.lmql_runtime import (FunctionContext, LMQLInputVariableScope,
                                        LMQLQueryFunction, compiled_query, tag)
 from lmql.runtime.model_registry import LMQLModelRegistry
 from lmql.runtime.output_writer import headless, printing, silent, stream
+from lmql.runtime.interpreter import LMQLResult
 
 model_registry = LMQLModelRegistry
 
 def connect(server="http://localhost:8080", model_name="EleutherAI/gpt-j-6B"):
     from lmql.runtime.hf_integration import transformers_model
 
     Model = transformers_model(server, model_name)
@@ -130,31 +131,30 @@
         # get source code of the function
         source = source.splitlines()
 
         # remove common indent
         common_indent = None
         lines = []
         for line in source[start-1:end]:
-            if line.strip() == "":
+            if line.strip() == "" or line.strip() == '"""lmql' or line.strip() == "'''lmql":
                 lines.append(line)
                 continue
             if common_indent is None:
                 common_indent = len(line) - len(line.lstrip())
             else:
                 common_indent = min(common_indent, len(line) - len(line.lstrip()))
             lines.append(line[common_indent:])
-        
         lines[0] = lines[0][startcol - common_indent:]
         lines[-1] = lines[-1][:endcol]
 
         source = "\n".join(lines)
 
         quote_types = "'''" if source.endswith("'''") else '"""'
-        if source.startswith(quote_types):
-            source = source[len(quote_types):]
+        if source.lstrip().startswith(quote_types):
+            source = source.lstrip()[len(quote_types):]
         assert source.endswith(quote_types), f"Docstring of @lmql.query function {fct.__name__} must be on the first line of the function, but is:\n {source}"
         source = source[:-len(quote_types)].strip("\n")
     except:
         raise RuntimeError("Failed to parse docstring of query function as LMQL code:\n\n" + str(source))
 
     return source
 
@@ -164,15 +164,15 @@
 
     # support for lmql.query(<query string>)
     if type(fct) is str: return _query_from_string(fct)
     
     calling_frame = inspect.stack()[1]
     scope = LMQLInputVariableScope(fct, calling_frame)
     code = _get_decorated_function_code(fct)
-        
+
     temp_lmql_file = tempfile.mktemp(suffix=".lmql")
     with open(temp_lmql_file, "w") as f:
         f.write(code)
     module = load(temp_lmql_file, autoconnect=True, output_writer=silent)
     
     assert inspect.iscoroutinefunction(fct), f"@lmql.query {fct.__name__} must be declared async."
```

### Comparing `lmql-0.0.5/src/lmql/cli.py` & `lmql-0.0.5.1/src/lmql/cli.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/demo.py` & `lmql-0.0.5.1/src/lmql/demo.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/http.py` & `lmql-0.0.5.1/src/lmql/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/language/compiler.py` & `lmql-0.0.5.1/src/lmql/language/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,44 @@
 from io import StringIO
 from lmql.ops.ops import lmql_operation_registry
 
 from lmql.language.qstrings import qstring_to_stmts, TemplateVariable
 from lmql.language.validator import LMQLValidator, LMQLValidationError
 from lmql.language.fragment_parser import LMQLDecoderConfiguration, LMQLQuery, LanguageFragmentParser, FragmentParserError
 from lmql.runtime.model_registry import model_name_aliases
+import lmql.runtime.lmql_runtime as lmql_runtime
 
 OPS_NAMESPACE = "lmql.ops"
 
+class FreeVarCollector(ast.NodeVisitor):
+    def __init__(self, free_vars):
+        self.free_vars = free_vars
+
+    def visit_Name(self, node):
+        if type(node.ctx) is ast.Load:
+            self.free_vars.add(node.id)
+
 class PromptScope(ast.NodeVisitor):
     def scope(self, query: LMQLQuery):
         self.distribution_vars = set([query.distribution.variable_name]) if query.distribution is not None else set()    
         self.defined_vars = set()
 
         # collect set of global query template variables
         self.free_vars = set()
         self.written_vars = set()
 
         for p in query.prompt: self.visit(p)
+        
+        # also collect variable reads from where clause
+        if query.where is not None:
+            FreeVarCollector(self.free_vars).visit(query.where)
+        if query.from_ast is not None:
+            FreeVarCollector(self.free_vars).visit(query.from_ast)
+        if query.decode is not None:
+            FreeVarCollector(self.free_vars).visit(query.decode)
 
         query.scope = self
 
     def visit_Constant(self, node):
         if type(node.value) is not str: return super().visit_Constant(node)
         qstring = node.value
 
@@ -442,14 +459,17 @@
         self._code = None
         self.lmql_code = lmql_code
         self.output_variables = output_variables or []
 
     def load(self):
         sys.path.append(os.path.dirname(self.compiled_file))
         m = __import__(os.path.basename(self.compiled_file[:-3]))
+        for v in m.__dict__.values():
+            if type(v) is lmql_runtime.LMQLQueryFunction:
+                v.lmql_code = self.lmql_code
         setattr(m, "code", self.code)
         setattr(m, "lmql_code", self.lmql_code)
         return m
 
     def __str__(self):
         with open(self.compiled_file, "r") as f:
             return f.read()
```

### Comparing `lmql-0.0.5/src/lmql/language/fragment_parser.py` & `lmql-0.0.5.1/src/lmql/language/fragment_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/language/qstrings.py` & `lmql-0.0.5.1/src/lmql/language/qstrings.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/language/validator.py` & `lmql-0.0.5.1/src/lmql/language/validator.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/model/async_generation_utils.py` & `lmql-0.0.5.1/src/lmql/model/async_generation_utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/model/local_client.py` & `lmql-0.0.5.1/src/lmql/model/local_client.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/model/serve.py` & `lmql-0.0.5.1/src/lmql/model/serve.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/model/served_model.py` & `lmql-0.0.5.1/src/lmql/model/served_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ops/follow_map.py` & `lmql-0.0.5.1/src/lmql/ops/follow_map.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ops/ops.py` & `lmql-0.0.5.1/src/lmql/ops/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,16 +240,14 @@
             )
         
     def postprocess_var(self, var_name):
         return var_name == self.predecessors[0].name
 
     def postprocess(self, operands, raw):
         value = int(raw)
-        if raw.startswith(" "):
-            value = " " + str(value)
         return postprocessed_rewrite(str(value)), postprocessed_value(value)
 
     def postprocess_order(self, other, **kwargs):
         if isinstance(other, StopAtOp):
             return "after" # apply Int after StopAt
         else:
             return 0 # cannot be compared
@@ -947,14 +945,24 @@
             if matched_phrase_index < other_matched_phrase_index:
                 return "before"
             else:
                 return "after"
         
         return 0 # other constraints cannot be compared
 
+@LMQLOp(["STOPS_BEFORE", "stops_before"])
+class StopBeforeOp(StopAtOp):
+    def postprocess(self, operands, value):
+        op2 = operands[1]
+        matched_phrase_index = value.rfind(op2)
+        if matched_phrase_index != -1:
+            value = value[:matched_phrase_index]
+
+        return postprocessed_rewrite(value), postprocessed_value(value)
+
 class OpaqueLambdaOp(Node):
     def forward(self, *args, **kwargs):
         if any([a is None for a in args]): return None
         fct, *args = args
         return fct(*args)
     
     def follow(self, *v, **kwargs):
```

### Comparing `lmql-0.0.5/src/lmql/ops/token_set.py` & `lmql-0.0.5.1/src/lmql/ops/token_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from lmql.runtime.stats import Stats
 
 def get_vocab(tokenizer):
     if hasattr(tokenizer, "vocab"):
         return tokenizer.vocab
     elif hasattr(tokenizer, "get_vocab"):
         return tokenizer.get_vocab()
+    elif hasattr(tokenizer, "tokenizer_impl"):
+        return get_vocab(tokenizer.tokenizer_impl)
     else:
         assert False, "Could not obtain full vocabulary from unknown tokenizer type: {}".format(type(tokenizer))
 
 class VocabularyMatcher:
     """
     Generates sub-token level logit masks from provided tokens.
     """
```

### Comparing `lmql-0.0.5/src/lmql/runtime/bopenai/__init__.py` & `lmql-0.0.5.1/src/lmql/runtime/bopenai/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 organization = None
 api_key = None
 
 # mock OpenAI Completion API
 global _api
 _api = None
 
+def get_stats():
+    global _api
+    if _api is None:
+        _api = AsyncOpenAIAPI()
+    return _api.stats
+
 class AsyncConfiguration:
     @staticmethod
     def set_batch_size(bs):
         global _api
         if _api is None:
             _api = AsyncOpenAIAPI()
         _api.batch_size = bs
```

### Comparing `lmql-0.0.5/src/lmql/runtime/bopenai/batched_openai.py` & `lmql-0.0.5.1/src/lmql/runtime/bopenai/batched_openai.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/bopenai/openai_api.py` & `lmql-0.0.5.1/src/lmql/runtime/bopenai/openai_api.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/dclib/dclib_array.py` & `lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_array.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/dclib/dclib_global.py` & `lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_global.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/dclib/dclib_model.py` & `lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/dclib/dclib_seq.py` & `lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_seq.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/dclib/decoders.py` & `lmql-0.0.5.1/src/lmql/runtime/dclib/decoders.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/dclib/trie_cache.py` & `lmql-0.0.5.1/src/lmql/runtime/dclib/trie_cache.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/hf_integration.py` & `lmql-0.0.5.1/src/lmql/runtime/hf_integration.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/interpreter.py` & `lmql-0.0.5.1/src/lmql/runtime/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         self.interpreter.set_where_clause(where)
 
     async def get_context(self, *args):
         # prompt
         return self
 
     async def get_all_vars(self):
-        return self.program_state.variable_values.copy()
+        return self.program_state.variable_program_values.copy()
 
     async def set_distribution(self, distribution_variable, values):
         self.interpreter.distribution_variable = distribution_variable
         self.interpreter.distribution_values = values
 
     async def get_return_value(self, *args):
         return LMQLResult(self.state.prompt, await self.get_all_vars(),self.interpreter.distribution_variable, self.interpreter.distribution_values)
```

### Comparing `lmql-0.0.5/src/lmql/runtime/langchain.py` & `lmql-0.0.5.1/src/lmql/runtime/langchain.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/lmql_runtime.py` & `lmql-0.0.5.1/src/lmql/runtime/lmql_runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 
     output_writer: Optional[Any] = None
     args: Optional[List[str]] = None
     model: Optional[Any] = None
     function_context: Optional[FunctionContext] = None
 
     is_langchain_use: bool = False
+
+    lmql_code: str = None
     
     def __init__(self, fct, output_variables, postprocessors, scope, *args, **kwargs):
         # check for pydantic base class and do kw initialization then
         if hasattr(self, "schema_json"):
             super().__init__(fct=fct, output_variables=output_variables, postprocessors=postprocessors, scope=scope, *args, **kwargs)
         else:
             # otherwise, do standard initialization
```

### Comparing `lmql-0.0.5/src/lmql/runtime/maiohttp.py` & `lmql-0.0.5.1/src/lmql/runtime/maiohttp.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/model_registry.py` & `lmql-0.0.5.1/src/lmql/runtime/model_registry.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/multi_head_interpretation.py` & `lmql-0.0.5.1/src/lmql/runtime/multi_head_interpretation.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/openai_integration.py` & `lmql-0.0.5.1/src/lmql/runtime/openai_integration.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/openai_secret.py` & `lmql-0.0.5.1/src/lmql/runtime/openai_secret.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/output_writer.py` & `lmql-0.0.5.1/src/lmql/runtime/output_writer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/postprocessing/conditional_prob.py` & `lmql-0.0.5.1/src/lmql/runtime/postprocessing/conditional_prob.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/program_state.py` & `lmql-0.0.5.1/src/lmql/runtime/program_state.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/stats.py` & `lmql-0.0.5.1/src/lmql/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/runtime/tokenizer.py` & `lmql-0.0.5.1/src/lmql/runtime/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             tokens = [js.tokenize_gpt_toks(se).to_py() for se in s]
             
             if unpack:
                 return tokens[0]
             else:
                 return tokens
          
-        def decode(self, input_ids):
+        def decode(self, input_ids, clean_up_tokenization_spaces=None):
             # set typed array type of input_ids to int
             return str(js.detokenize_gpt(to_js([int(i) for i in input_ids])))
 
         def __call__(self, s: str):
             unpack = False
             if type(s) is not list:
                 s = [s]
@@ -106,26 +106,26 @@
             key = str(input_ids[:-1])
             if key in self.detokenizer_cache[n-1].keys():
                 global reverse_special_token_mappings
                 # print("secondary cache hit")
                 if input_ids[-1] >= self.tokenizer_impl.vocab_size:
                     extended = self.detokenizer_cache[n-1][key] + "<" + reverse_special_token_mappings[input_ids[-1]] + "/>"
                 else:
-                    extended = self.detokenizer_cache[n-1][key] + self.tokenizer_impl.decode([input_ids[-1]])
+                    extended = self.detokenizer_cache[n-1][key] + self.tokenizer_impl.decode([input_ids[-1]], clean_up_tokenization_spaces=False)
                 if not n in self.detokenizer_cache.keys():
                     self.detokenizer_cache[n] = {}
                 self.detokenizer_cache[n][str(input_ids)] = extended
                 return extended
 
         s = ""
         for chunk in self.chunk_out_by_special_ids(input_ids):
             if type(chunk) is str:
                 s += chunk
             else:
-                s += self.tokenizer_impl.decode(chunk)
+                s += self.tokenizer_impl.decode(chunk, clean_up_tokenization_spaces=False)
 
         if not n in self.detokenizer_cache.keys():
             self.detokenizer_cache[n] = {}
         self.detokenizer_cache[n][key] = s
 
         return s
```

### Comparing `lmql-0.0.5/src/lmql/tests/expr_test_utils.py` & `lmql-0.0.5.1/src/lmql/tests/expr_test_utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/tests/mask_product_test.py` & `lmql-0.0.5.1/src/lmql/tests/mask_product_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/tests/monotonicity.py` & `lmql-0.0.5.1/src/lmql/tests/monotonicity.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/tests/one_of_tests.py` & `lmql-0.0.5.1/src/lmql/tests/one_of_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/tests/sentences_op.py` & `lmql-0.0.5.1/src/lmql/tests/sentences_op.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/tests/starts_with_op_test.py` & `lmql-0.0.5.1/src/lmql/tests/starts_with_op_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/tests/stops_at.py` & `lmql-0.0.5.1/src/lmql/tests/stops_at.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/tests/str_in_str_tests.py` & `lmql-0.0.5.1/src/lmql/tests/str_in_str_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/tests/system/basic_use_cases.py` & `lmql-0.0.5.1/src/lmql/tests/system/basic_use_cases.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/tests/test_multi_head.py` & `lmql-0.0.5.1/src/lmql/tests/test_multi_head.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/tests/test_sample_queries.py` & `lmql-0.0.5.1/src/lmql/tests/test_sample_queries.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/tests/token_set_test.py` & `lmql-0.0.5.1/src/lmql/tests/token_set_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/live/live.js` & `lmql-0.0.5.1/src/lmql/ui/live/live.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/live/live.py` & `lmql-0.0.5.1/src/lmql/ui/live/live.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/live/livelib.py` & `lmql-0.0.5.1/src/lmql/ui/live/livelib.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/live/yarn.lock` & `lmql-0.0.5.1/src/lmql/ui/live/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/README.md` & `lmql-0.0.5.1/src/lmql/ui/playground/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/package.json` & `lmql-0.0.5.1/src/lmql/ui/playground/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/favicon.ico` & `lmql-0.0.5.1/src/lmql/ui/playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/index.html` & `lmql-0.0.5.1/src/lmql/ui/playground/public/index.html`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/lmql.svg` & `lmql-0.0.5.1/src/lmql/ui/playground/public/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/calc.json` & `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/calc.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/chat.json` & `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/chat.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/cot.json` & `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/cot.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/distribution.json` & `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/distribution.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/hello.json` & `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/hello.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/joke.json` & `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/joke.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/kv.json` & `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/kv.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/list.json` & `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/list.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/meta.json` & `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/meta.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/translation.json` & `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/translation.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/wiki.json` & `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/wiki.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/snippets/dynamic-cfg.json` & `lmql-0.0.5.1/src/lmql/ui/playground/public/snippets/dynamic-cfg.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/public/snippets/json-parsing.json` & `lmql-0.0.5.1/src/lmql/ui/playground/public/snippets/json-parsing.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/App.jsx` & `lmql-0.0.5.1/src/lmql/ui/playground/src/App.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/CodeScreenshot.jsx` & `lmql-0.0.5.1/src/lmql/ui/playground/src/CodeScreenshot.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/Configuration.js` & `lmql-0.0.5.1/src/lmql/ui/playground/src/Configuration.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/DataListView.js` & `lmql-0.0.5.1/src/lmql/ui/playground/src/DataListView.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/DecoderGraph.js` & `lmql-0.0.5.1/src/lmql/ui/playground/src/DecoderGraph.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/Explore.jsx` & `lmql-0.0.5.1/src/lmql/ui/playground/src/Explore.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/SharedState.js` & `lmql-0.0.5.1/src/lmql/ui/playground/src/SharedState.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/State.js` & `lmql-0.0.5.1/src/lmql/ui/playground/src/State.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/ValidationGraph.jsx` & `lmql-0.0.5.1/src/lmql/ui/playground/src/ValidationGraph.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/browser_process.js` & `lmql-0.0.5.1/src/lmql/ui/playground/src/browser_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/build_info.js` & `lmql-0.0.5.1/src/lmql/ui/playground/src/build_info.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/editor/lmql-monaco-language.js` & `lmql-0.0.5.1/src/lmql/ui/playground/src/editor/lmql-monaco-language.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/editor/theme.json` & `lmql-0.0.5.1/src/lmql/ui/playground/src/editor/theme.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/explore.svg` & `lmql-0.0.5.1/src/lmql/ui/playground/src/explore.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/graph-layout.css` & `lmql-0.0.5.1/src/lmql/ui/playground/src/graph-layout.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/index.css` & `lmql-0.0.5.1/src/lmql/ui/playground/src/index.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/logo.svg` & `lmql-0.0.5.1/src/lmql/ui/playground/src/logo.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/queries.js` & `lmql-0.0.5.1/src/lmql/ui/playground/src/queries.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/remote_process.js` & `lmql-0.0.5.1/src/lmql/ui/playground/src/remote_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/screenshot.css` & `lmql-0.0.5.1/src/lmql/ui/playground/src/screenshot.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/spinner.svg` & `lmql-0.0.5.1/src/lmql/ui/playground/src/spinner.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/src/tagged-model-result.js` & `lmql-0.0.5.1/src/lmql/ui/playground/src/tagged-model-result.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/playground/yarn.lock` & `lmql-0.0.5.1/src/lmql/ui/playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/vscode/.vscode/launch.json` & `lmql-0.0.5.1/src/lmql/ui/vscode/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/vscode/LICENSE` & `lmql-0.0.5.1/src/lmql/ui/vscode/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/vscode/language-configuration.json` & `lmql-0.0.5.1/src/lmql/ui/vscode/language-configuration.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/vscode/lmql-vscode.png` & `lmql-0.0.5.1/src/lmql/ui/vscode/lmql-vscode.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/vscode/package.json` & `lmql-0.0.5.1/src/lmql/ui/vscode/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/vscode/syntaxes/lmql.qstring.json` & `lmql-0.0.5.1/src/lmql/ui/vscode/syntaxes/lmql.qstring.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json` & `lmql-0.0.5.1/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/ui/vscode/syntaxes/pylmql.json` & `lmql-0.0.5.1/src/lmql/ui/vscode/syntaxes/pylmql.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/utils/graph.py` & `lmql-0.0.5.1/src/lmql/utils/graph.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql/utils/nputil.py` & `lmql-0.0.5.1/src/lmql/utils/nputil.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5/src/lmql.egg-info/PKG-INFO` & `lmql-0.0.5.1/src/lmql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.5
+Version: 0.0.5.1
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -34,36 +34,37 @@
     <br/>
   </p>
 </div>
 
 LMQL is a query language for large language models (LLMs). It facilitates LLM interaction by combining the benefits of natural language prompting with the expressiveness of Python. With only a few lines of LMQL code, users can express advanced, multi-part and tool-augmented LM queries, which then are optimized by the LMQL runtime to run efficiently as part of the LM decoding loop.
 
 ![lmql-overview](https://user-images.githubusercontent.com/17903049/222918379-84a00b9a-1ef0-45bf-9384-15a20f2874f0.png)
+
 <p align="center">Example of a simple LMQL program.</p>
 
 
 ## Getting Started
 
 To install the latest version of LMQL run the following command with Python >=3.10 installed.
 
 ```
 pip install lmql
 ```
 
-**Local GPU Support:** If you want to run models on a local GPU, make sure to install LMQL in an environment with a GPU-enabled installation of PyTorch >= 1.11 (cf. https://pytorch.org/get-started/locally/). 
+**Local GPU Support:** If you want to run models on a local GPU, make sure to install LMQL in an environment with a GPU-enabled installation of PyTorch >= 1.11 (cf. https://pytorch.org/get-started/locally/).
 
 ### Running LMQL Programs
 
 After installation, you can launch the LMQL playground IDE with the following command:
 
 ```
 lmql playground
 ```
 
-> Using the LMQL playground requires an installation of Node.js. If you are in a conda-managed environment you can install node.js via `conda install nodejs=14.20 -c conda-forge`. Otherwise, please see the offical Node.js website https://nodejs.org/en/download/ for instructions how to install it on your system.
+> Using the LMQL playground requires an installation of Node.js. If you are in a conda-managed environment you can install node.js via `conda install nodejs=14.20 -c conda-forge`. Otherwise, please see the official Node.js website https://nodejs.org/en/download/ for instructions how to install it on your system.
 
 This launches a browser-based playground IDE, including a showcase of many exemplary LMQL programs. If the IDE does not launch automatically, go to `http://localhost:3000`.
 
 Alternatively, `lmql run` can be used to execute local `.lmql` files. Note that when using local HuggingFace Transformers models in the Playground IDE or via `lmql run`, you have to first launch an instance of the LMQL Inference API for the corresponding model via the command `lmql serve-model`.
 
 ### Configuring OpenAI API Credentials
 
@@ -89,15 +90,15 @@
 source scripts/activate-dev.sh
 ```
 
 > **Operating System**: The GPU-enabled version of LMQL was tested to work on Ubuntu 22.04 with CUDA 12.0 and Windows 10 via WSL2 and CUDA 11.7. The no-GPU version (see below) was tested to work on Ubuntu 22.04 and macOS 13.2 Ventura or Windows 10 via WSL2.
 
 ### Development without GPU
 
-This section outlines how to setup an LMQL development environment without local GPU support. Note that LMQL without local GPU support only supports the use of API-integrated models like `openai/text-davinci-003`. Please see the OpenAI API documentation (https://platform.openai.com/docs/models/gpt-3-5) to learn more about the set of available models. 
+This section outlines how to setup an LMQL development environment without local GPU support. Note that LMQL without local GPU support only supports the use of API-integrated models like `openai/text-davinci-003`. Please see the OpenAI API documentation (https://platform.openai.com/docs/models/gpt-3-5) to learn more about the set of available models.
 
 To setup a `conda` environment for LMQL with GPU support, run the following commands:
 
 ```
 # prepare conda environment
 conda env create -f scripts/conda/requirements-no-gpu.yml -n lmql-no-gpu
 conda activate lmql-no-gpu
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.5 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.5.1 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
@@ -24,15 +24,15 @@
 Support:** If you want to run models on a local GPU, make sure to install LMQL
 in an environment with a GPU-enabled installation of PyTorch >= 1.11 (cf.
 https://pytorch.org/get-started/locally/). ### Running LMQL Programs After
 installation, you can launch the LMQL playground IDE with the following
 command: ``` lmql playground ``` > Using the LMQL playground requires an
 installation of Node.js. If you are in a conda-managed environment you can
 install node.js via `conda install nodejs=14.20 -c conda-forge`. Otherwise,
-please see the offical Node.js website https://nodejs.org/en/download/ for
+please see the official Node.js website https://nodejs.org/en/download/ for
 instructions how to install it on your system. This launches a browser-based
 playground IDE, including a showcase of many exemplary LMQL programs. If the
 IDE does not launch automatically, go to `http://localhost:3000`.
 Alternatively, `lmql run` can be used to execute local `.lmql` files. Note that
 when using local HuggingFace Transformers models in the Playground IDE or via
 `lmql run`, you have to first launch an instance of the LMQL Inference API for
 the corresponding model via the command `lmql serve-model`. ### Configuring
```

### Comparing `lmql-0.0.5/src/lmql.egg-info/SOURCES.txt` & `lmql-0.0.5.1/src/lmql.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 docs/source/language/models.md
 docs/source/language/overview.md
 docs/source/language/scripted_prompts.md
 docs/source/python/.gitignore
 docs/source/python/langchain.ipynb
 docs/source/python/lmql.txt
 docs/source/python/python.ipynb
+docs/source/releases/misc-snippets.md
 docs/source/releases/release-0.0.5.md
 scripts/activate-dev.sh
 scripts/pypi-release.sh
 scripts/wheel.sh
 scripts/conda/requirements-no-gpu.yml
 scripts/conda/requirements.yml
 src/lmql.svg
```

### Comparing `lmql-0.0.5/src/lmql.svg` & `lmql-0.0.5.1/src/lmql.svg`

 * *Files identical despite different names*

