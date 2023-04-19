# Comparing `tmp/sphinx-codeautolink-0.8.0.tar.gz` & `tmp/sphinx-codeautolink-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-codeautolink-0.8.0.tar", last modified: Thu Dec 16 17:08:32 2021, max compression
+gzip compressed data, was "sphinx-codeautolink-0.9.0.tar", last modified: Thu Jan 13 14:32:33 2022, max compression
```

## Comparing `sphinx-codeautolink-0.8.0.tar` & `sphinx-codeautolink-0.9.0.tar`

### file list

```diff
@@ -1,128 +1,135 @@
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.881180 sphinx-codeautolink-0.8.0/
--rw-rw-rw-   0        0        0     1091 2021-09-13 12:39:16.000000 sphinx-codeautolink-0.8.0/LICENSE
--rw-rw-rw-   0        0        0      142 2021-10-04 12:49:13.000000 sphinx-codeautolink-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3017 2021-12-16 17:08:32.880680 sphinx-codeautolink-0.8.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.752158 sphinx-codeautolink-0.8.0/docs/
--rw-rw-rw-   0        0        0      652 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.8.0/docs/Makefile
--rwxrwxrwx   0        0        0      796 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.8.0/docs/make.bat
--rw-rw-rw-   0        0        0       75 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.8.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.802666 sphinx-codeautolink-0.8.0/docs/src/
--rw-rw-rw-   0        0        0      260 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.8.0/docs/src/404.rst
--rw-rw-rw-   0        0        0     5464 2021-12-16 16:52:58.000000 sphinx-codeautolink-0.8.0/docs/src/about.rst
--rw-rw-rw-   0        0        0     1766 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.8.0/docs/src/conf.py
--rw-rw-rw-   0        0        0      297 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.8.0/docs/src/example_library.rst
--rw-rw-rw-   0        0        0     8834 2021-12-15 11:59:14.000000 sphinx-codeautolink-0.8.0/docs/src/examples.rst
--rw-rw-rw-   0        0        0     2997 2021-12-08 08:27:35.000000 sphinx-codeautolink-0.8.0/docs/src/index.rst
--rw-rw-rw-   0        0        0      758 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.8.0/docs/src/lib.py
--rw-rw-rw-   0        0        0     4844 2021-12-14 18:54:30.000000 sphinx-codeautolink-0.8.0/docs/src/reference.rst
--rw-rw-rw-   0        0        0     4071 2021-12-16 17:04:41.000000 sphinx-codeautolink-0.8.0/docs/src/release_notes.rst
--rw-rw-rw-   0        0        0      378 2021-09-19 14:12:58.000000 sphinx-codeautolink-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0     1648 2021-12-08 08:23:39.000000 sphinx-codeautolink-0.8.0/readme_pypi.rst
--rw-rw-rw-   0        0        0       42 2021-12-16 17:08:32.881180 sphinx-codeautolink-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     2076 2021-12-15 11:59:14.000000 sphinx-codeautolink-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.731154 sphinx-codeautolink-0.8.0/src/
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.805667 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/
--rw-rw-rw-   0        0        0        5 2021-12-16 17:04:41.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/VERSION
--rw-rw-rw-   0        0        0     2082 2021-12-16 16:52:58.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.815168 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/extension/
--rw-rw-rw-   0        0        0     8704 2021-12-16 16:52:58.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/extension/__init__.py
--rw-rw-rw-   0        0        0     3533 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/extension/backref.py
--rw-rw-rw-   0        0        0    13307 2021-12-14 18:54:30.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/extension/block.py
--rw-rw-rw-   0        0        0     1503 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/extension/cache.py
--rw-rw-rw-   0        0        0     3843 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/extension/directive.py
--rw-rw-rw-   0        0        0     4025 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/extension/resolve.py
--rw-rw-rw-   0        0        0    21031 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/parse.py
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.816169 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/static/
--rw-rw-rw-   0        0        0      343 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/static/sphinx-codeautolink.css
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.810168 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink.egg-info/
--rw-rw-rw-   0        0        0     3017 2021-12-16 17:08:32.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4124 2021-12-16 17:08:32.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-16 17:08:32.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2021-12-16 17:08:32.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2021-12-16 17:08:32.000000 sphinx-codeautolink-0.8.0/src/sphinx_codeautolink.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.817169 sphinx-codeautolink-0.8.0/tests/
--rw-rw-rw-   0        0        0      313 2021-12-14 18:54:30.000000 sphinx-codeautolink-0.8.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.818669 sphinx-codeautolink-0.8.0/tests/extension/
--rw-rw-rw-   0        0        0     7892 2021-12-16 16:52:58.000000 sphinx-codeautolink-0.8.0/tests/extension/__init__.py
--rw-rw-rw-   0        0        0     1546 2021-12-16 16:52:58.000000 sphinx-codeautolink-0.8.0/tests/extension/_check.py
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.823670 sphinx-codeautolink-0.8.0/tests/extension/fail/
--rw-rw-rw-   0        0        0      170 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/fail/concat_invalid.txt
--rw-rw-rw-   0        0        0      221 2021-12-06 21:15:51.000000 sphinx-codeautolink-0.8.0/tests/extension/fail/custom_block_import_invalid.txt
--rw-rw-rw-   0        0        0      146 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/fail/ref_invalid_block_type.txt
--rw-rw-rw-   0        0        0      145 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/fail/ref_invalid_syntax.txt
--rw-rw-rw-   0        0        0      283 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/fail/ref_invalid_syntax_complex.txt
--rw-rw-rw-   0        0        0      168 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/fail/skip_invalid.txt
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.867678 sphinx-codeautolink-0.8.0/tests/extension/ref/
--rw-rw-rw-   0        0        0      365 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/concat_default.txt
--rw-rw-rw-   0        0        0      272 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/concat_off.txt
--rw-rw-rw-   0        0        0      354 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/concat_on_across_sections.txt
--rw-rw-rw-   0        0        0      276 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/concat_on_breaks.txt
--rw-rw-rw-   0        0        0      343 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/concat_section_breaks.txt
--rw-rw-rw-   0        0        0      443 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/concat_section_returns_to_global.txt
--rw-rw-rw-   0        0        0      292 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/custom_block.txt
--rw-rw-rw-   0        0        0      253 2021-12-06 21:09:58.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/custom_block_imported.txt
--rw-rw-rw-   0        0        0       58 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/empty_project.txt
--rw-rw-rw-   0        0        0      117 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/no_module_docs.txt
--rw-rw-rw-   0        0        0      142 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/non_python_block.txt
--rw-rw-rw-   0        0        0      267 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/preface_concatenated.txt
--rw-rw-rw-   0        0        0      202 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/preface_consumed_non_python.txt
--rw-rw-rw-   0        0        0      233 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/preface_global.txt
--rw-rw-rw-   0        0        0      237 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/preface_global_multiline.txt
--rw-rw-rw-   0        0        0      262 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/preface_global_overwritten.txt
--rw-rw-rw-   0        0        0      243 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/preface_multiline.txt
--rw-rw-rw-   0        0        0      239 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/preface_multiline_and_arg.txt
--rw-rw-rw-   0        0        0      254 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/preface_multiple.txt
--rw-rw-rw-   0        0        0      184 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/preface_single.txt
--rw-rw-rw-   0        0        0      192 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_chain.txt
--rw-rw-rw-   0        0        0      342 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_class_attr.txt
--rw-rw-rw-   0        0        0      219 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_class_meth_returns_self.txt
--rw-rw-rw-   0        0        0      253 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_decorator.txt
--rw-rw-rw-   0        0        0      362 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_doctest.txt
--rw-rw-rw-   0        0        0      574 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_extdoctest_doctest.txt
--rw-rw-rw-   0        0        0      378 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_extdoctest_testcode.txt
--rw-rw-rw-   0        0        0      306 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_fluent_attrs.txt
--rw-rw-rw-   0        0        0      362 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_fluent_call.txt
--rw-rw-rw-   0        0        0      131 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_func_no_module.txt
--rw-rw-rw-   0        0        0      201 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_import_as.txt
--rw-rw-rw-   0        0        0      152 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_import_from.txt
--rw-rw-rw-   0        0        0      395 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_import_from_complex.txt
--rw-rw-rw-   0        0        0      234 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_import_multiple.txt
--rw-rw-rw-   0        0        0      145 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_import_star.txt
--rw-rw-rw-   0        0        0      246 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_import_submodule.txt
--rw-rw-rw-   0        0        0      192 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_imported_func.txt
--rw-rw-rw-   0        0        0      206 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_imported_func_relocated.txt
--rw-rw-rw-   0        0        0      387 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_inherited.txt
--rw-rw-rw-   0        0        0      279 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_intersphinx_only.txt
--rw-rw-rw-   0        0        0      196 2021-12-14 18:54:30.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_ipython.txt
--rw-rw-rw-   0        0        0      200 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_optional.txt
--rw-rw-rw-   0        0        0      210 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_optional_counter.txt
--rw-rw-rw-   0        0        0      200 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_optional_manual.txt
--rw-rw-rw-   0        0        0      175 2021-12-09 08:50:14.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_py.txt
--rw-rw-rw-   0        0        0      411 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_pycon.txt
--rw-rw-rw-   0        0        0      268 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_shadow_builtin.txt
--rw-rw-rw-   0        0        0      181 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/ref_simple.txt
--rw-rw-rw-   0        0        0      250 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/search_css_duplicates_removed.txt
--rw-rw-rw-   0        0        0      336 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/skip_file.txt
--rw-rw-rw-   0        0        0      268 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/skip_next.txt
--rw-rw-rw-   0        0        0      261 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/skip_next_consumed_non_python.txt
--rw-rw-rw-   0        0        0      426 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/skip_off.txt
--rw-rw-rw-   0        0        0      371 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/ref/skip_section.txt
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.868178 sphinx-codeautolink-0.8.0/tests/extension/src/
--rw-rw-rw-   0        0        0       84 2021-12-06 21:10:20.000000 sphinx-codeautolink-0.8.0/tests/extension/src/parser_func.py
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.869678 sphinx-codeautolink-0.8.0/tests/extension/src/test_project/
--rw-rw-rw-   0        0        0      812 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/src/test_project/__init__.py
--rw-rw-rw-   0        0        0       49 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/src/test_project/sub.py
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.875179 sphinx-codeautolink-0.8.0/tests/extension/table/
--rw-rw-rw-   0        0        0      166 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/table/tab_autodoc_empty.txt
--rw-rw-rw-   0        0        0      200 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/table/tab_autodoc_links.txt
--rw-rw-rw-   0        0        0      216 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/table/tab_manual_collapse.txt
--rw-rw-rw-   0        0        0      188 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/table/tab_manual_empty.txt
--rw-rw-rw-   0        0        0      219 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/table/tab_manual_links.txt
--rw-rw-rw-   0        0        0      276 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/table/tab_manual_links_subsection.txt
--rw-rw-rw-   0        0        0      147 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/extension/table/tab_no_table.txt
-drwxrwxrwx   0        0        0        0 2021-12-16 17:08:32.879180 sphinx-codeautolink-0.8.0/tests/parse/
--rw-rw-rw-   0        0        0     3811 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/parse/__init__.py
--rw-rw-rw-   0        0        0      697 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/parse/_util.py
--rw-rw-rw-   0        0        0     7205 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/parse/assign.py
--rw-rw-rw-   0        0        0      739 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/parse/chain.py
--rw-rw-rw-   0        0        0     9884 2021-12-03 15:20:11.000000 sphinx-codeautolink-0.8.0/tests/parse/scope.py
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.552946 sphinx-codeautolink-0.9.0/
+-rw-rw-rw-   0        0        0     1096 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      142 2021-10-04 12:49:13.000000 sphinx-codeautolink-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3017 2022-01-13 14:32:33.552446 sphinx-codeautolink-0.9.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.467931 sphinx-codeautolink-0.9.0/docs/
+-rw-rw-rw-   0        0        0      652 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.9.0/docs/Makefile
+-rwxrwxrwx   0        0        0      796 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.9.0/docs/make.bat
+-rw-rw-rw-   0        0        0      135 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.474933 sphinx-codeautolink-0.9.0/docs/src/
+-rw-rw-rw-   0        0        0      260 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.9.0/docs/src/404.rst
+-rw-rw-rw-   0        0        0     5464 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/docs/src/about.rst
+-rw-rw-rw-   0        0        0     1923 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/docs/src/conf.py
+-rw-rw-rw-   0        0        0      297 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.9.0/docs/src/example_library.rst
+-rw-rw-rw-   0        0        0     9215 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/docs/src/examples.rst
+-rw-rw-rw-   0        0        0     2997 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/docs/src/index.rst
+-rw-rw-rw-   0        0        0      758 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.9.0/docs/src/lib.py
+-rw-rw-rw-   0        0        0     5617 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/docs/src/reference.rst
+-rw-rw-rw-   0        0        0     4394 2022-01-13 14:24:23.000000 sphinx-codeautolink-0.9.0/docs/src/release_notes.rst
+-rw-rw-rw-   0        0        0      378 2021-09-19 14:12:58.000000 sphinx-codeautolink-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1648 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/readme_pypi.rst
+-rw-rw-rw-   0        0        0       42 2022-01-13 14:32:33.552946 sphinx-codeautolink-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2076 2022-01-13 14:21:20.000000 sphinx-codeautolink-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.459430 sphinx-codeautolink-0.9.0/src/
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.478433 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/
+-rw-rw-rw-   0        0        0        5 2022-01-13 14:21:50.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/VERSION
+-rw-rw-rw-   0        0        0     2082 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.487435 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/extension/
+-rw-rw-rw-   0        0        0     8599 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/extension/__init__.py
+-rw-rw-rw-   0        0        0     3533 2022-01-04 15:12:51.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/extension/backref.py
+-rw-rw-rw-   0        0        0    14289 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/extension/block.py
+-rw-rw-rw-   0        0        0     1503 2022-01-04 15:12:51.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/extension/cache.py
+-rw-rw-rw-   0        0        0     3843 2022-01-04 15:12:51.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/extension/directive.py
+-rw-rw-rw-   0        0        0     4025 2022-01-04 15:12:51.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/extension/resolve.py
+-rw-rw-rw-   0        0        0    21552 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/parse.py
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.488435 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/static/
+-rw-rw-rw-   0        0        0      343 2021-12-03 15:19:25.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/static/sphinx-codeautolink.css
+-rw-rw-rw-   0        0        0      144 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/warn.py
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.482934 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink.egg-info/
+-rw-rw-rw-   0        0        0     3017 2022-01-13 14:32:33.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4417 2022-01-13 14:32:33.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-13 14:32:33.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2022-01-13 14:32:33.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2022-01-13 14:32:33.000000 sphinx-codeautolink-0.9.0/src/sphinx_codeautolink.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.488935 sphinx-codeautolink-0.9.0/tests/
+-rw-rw-rw-   0        0        0      313 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.490435 sphinx-codeautolink-0.9.0/tests/extension/
+-rw-rw-rw-   0        0        0     7898 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/extension/__init__.py
+-rw-rw-rw-   0        0        0     1546 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/extension/_check.py
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.496936 sphinx-codeautolink-0.9.0/tests/extension/fail/
+-rw-rw-rw-   0        0        0      170 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/fail/concat_invalid.txt
+-rw-rw-rw-   0        0        0      221 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/extension/fail/custom_block_import_invalid.txt
+-rw-rw-rw-   0        0        0      134 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/extension/fail/ref_import_star_invalid.txt
+-rw-rw-rw-   0        0        0      146 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/fail/ref_invalid_block_type.txt
+-rw-rw-rw-   0        0        0      145 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/fail/ref_invalid_syntax.txt
+-rw-rw-rw-   0        0        0      283 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/fail/ref_invalid_syntax_complex.txt
+-rw-rw-rw-   0        0        0      270 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/extension/fail/ref_ipython_non-python.txt
+-rw-rw-rw-   0        0        0      570 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/extension/fail/ref_ipython_syntax.txt
+-rw-rw-rw-   0        0        0      168 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/fail/skip_invalid.txt
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.539444 sphinx-codeautolink-0.9.0/tests/extension/ref/
+-rw-rw-rw-   0        0        0      365 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/concat_default.txt
+-rw-rw-rw-   0        0        0      272 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/concat_off.txt
+-rw-rw-rw-   0        0        0      354 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/concat_on_across_sections.txt
+-rw-rw-rw-   0        0        0      276 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/concat_on_breaks.txt
+-rw-rw-rw-   0        0        0      343 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/concat_section_breaks.txt
+-rw-rw-rw-   0        0        0      443 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/concat_section_returns_to_global.txt
+-rw-rw-rw-   0        0        0      292 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/custom_block.txt
+-rw-rw-rw-   0        0        0      253 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/custom_block_imported.txt
+-rw-rw-rw-   0        0        0       58 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/empty_project.txt
+-rw-rw-rw-   0        0        0      117 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/no_module_docs.txt
+-rw-rw-rw-   0        0        0      142 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/non_python_block.txt
+-rw-rw-rw-   0        0        0      267 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/preface_concatenated.txt
+-rw-rw-rw-   0        0        0      202 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/preface_consumed_non_python.txt
+-rw-rw-rw-   0        0        0      233 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/preface_global.txt
+-rw-rw-rw-   0        0        0      237 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/preface_global_multiline.txt
+-rw-rw-rw-   0        0        0      262 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/preface_global_overwritten.txt
+-rw-rw-rw-   0        0        0      243 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/preface_multiline.txt
+-rw-rw-rw-   0        0        0      239 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/preface_multiline_and_arg.txt
+-rw-rw-rw-   0        0        0      254 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/preface_multiple.txt
+-rw-rw-rw-   0        0        0      184 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/preface_single.txt
+-rw-rw-rw-   0        0        0      285 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_builtins.txt
+-rw-rw-rw-   0        0        0      192 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_chain.txt
+-rw-rw-rw-   0        0        0      342 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_class_attr.txt
+-rw-rw-rw-   0        0        0      219 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_class_meth_returns_self.txt
+-rw-rw-rw-   0        0        0      253 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_decorator.txt
+-rw-rw-rw-   0        0        0      362 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_doctest.txt
+-rw-rw-rw-   0        0        0      574 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_extdoctest_doctest.txt
+-rw-rw-rw-   0        0        0      378 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_extdoctest_testcode.txt
+-rw-rw-rw-   0        0        0      306 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_fluent_attrs.txt
+-rw-rw-rw-   0        0        0      362 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_fluent_call.txt
+-rw-rw-rw-   0        0        0      131 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_func_no_module.txt
+-rw-rw-rw-   0        0        0      201 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_import_as.txt
+-rw-rw-rw-   0        0        0      152 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_import_from.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_import_from_complex.txt
+-rw-rw-rw-   0        0        0      234 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_import_multiple.txt
+-rw-rw-rw-   0        0        0      145 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_import_star.txt
+-rw-rw-rw-   0        0        0      246 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_import_submodule.txt
+-rw-rw-rw-   0        0        0      192 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_imported_func.txt
+-rw-rw-rw-   0        0        0      206 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_imported_func_relocated.txt
+-rw-rw-rw-   0        0        0      387 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_inherited.txt
+-rw-rw-rw-   0        0        0      279 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_intersphinx_only.txt
+-rw-rw-rw-   0        0        0      297 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_ipython.txt
+-rw-rw-rw-   0        0        0      196 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_ipython3.txt
+-rw-rw-rw-   0        0        0      333 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_ipython_directive.txt
+-rw-rw-rw-   0        0        0      200 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_optional.txt
+-rw-rw-rw-   0        0        0      210 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_optional_counter.txt
+-rw-rw-rw-   0        0        0      200 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_optional_manual.txt
+-rw-rw-rw-   0        0        0      175 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_py.txt
+-rw-rw-rw-   0        0        0      411 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_pycon.txt
+-rw-rw-rw-   0        0        0      268 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_shadow_builtin.txt
+-rw-rw-rw-   0        0        0      181 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/ref_simple.txt
+-rw-rw-rw-   0        0        0      250 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/search_css_duplicates_removed.txt
+-rw-rw-rw-   0        0        0      336 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/skip_file.txt
+-rw-rw-rw-   0        0        0      268 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/skip_next.txt
+-rw-rw-rw-   0        0        0      261 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/skip_next_consumed_non_python.txt
+-rw-rw-rw-   0        0        0      426 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/skip_off.txt
+-rw-rw-rw-   0        0        0      371 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/ref/skip_section.txt
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.540444 sphinx-codeautolink-0.9.0/tests/extension/src/
+-rw-rw-rw-   0        0        0       87 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/extension/src/parser_func.py
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.541944 sphinx-codeautolink-0.9.0/tests/extension/src/test_project/
+-rw-rw-rw-   0        0        0      812 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/src/test_project/__init__.py
+-rw-rw-rw-   0        0        0       49 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/src/test_project/sub.py
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.547445 sphinx-codeautolink-0.9.0/tests/extension/table/
+-rw-rw-rw-   0        0        0      166 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/table/tab_autodoc_empty.txt
+-rw-rw-rw-   0        0        0      200 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/table/tab_autodoc_links.txt
+-rw-rw-rw-   0        0        0      216 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/table/tab_manual_collapse.txt
+-rw-rw-rw-   0        0        0      188 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/table/tab_manual_empty.txt
+-rw-rw-rw-   0        0        0      219 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/table/tab_manual_links.txt
+-rw-rw-rw-   0        0        0      276 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/table/tab_manual_links_subsection.txt
+-rw-rw-rw-   0        0        0      147 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/extension/table/tab_no_table.txt
+drwxrwxrwx   0        0        0        0 2022-01-13 14:32:33.551446 sphinx-codeautolink-0.9.0/tests/parse/
+-rw-rw-rw-   0        0        0     3973 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/parse/__init__.py
+-rw-rw-rw-   0        0        0      716 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/parse/_util.py
+-rw-rw-rw-   0        0        0     7199 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/parse/assign.py
+-rw-rw-rw-   0        0        0      739 2022-01-11 08:20:09.000000 sphinx-codeautolink-0.9.0/tests/parse/chain.py
+-rw-rw-rw-   0        0        0     9813 2022-01-11 08:22:47.000000 sphinx-codeautolink-0.9.0/tests/parse/scope.py
```

### Comparing `sphinx-codeautolink-0.8.0/LICENSE` & `sphinx-codeautolink-0.9.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Felix Hildén
+Copyright (c) 2021-2022 Felix Hildén
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sphinx-codeautolink-0.8.0/PKG-INFO` & `sphinx-codeautolink-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-codeautolink
-Version: 0.8.0
+Version: 0.9.0
 Summary: Automatic links from code examples to reference documentation.
 Home-page: https://pypi.org/project/sphinx-codeautolink
 Author: Felix Hildén
 Author-email: felix.hilden@gmail.com
 Maintainer: Felix Hildén
 Maintainer-email: felix.hilden@gmail.com
 License: MIT
```

### Comparing `sphinx-codeautolink-0.8.0/docs/Makefile` & `sphinx-codeautolink-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/docs/make.bat` & `sphinx-codeautolink-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/docs/src/about.rst` & `sphinx-codeautolink-0.9.0/docs/src/about.rst`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/docs/src/conf.py` & `sphinx-codeautolink-0.9.0/docs/src/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 _src_dir = Path(os.path.realpath(__file__)).parent
 _package_root = _src_dir.parent.parent / "src"
 sys.path.insert(0, str(_package_root))
 sys.path.insert(0, str(_src_dir))
 
 project = "sphinx-codeautolink"
 author = "Felix Hildén"
-copyright = "2021, Felix Hildén"
+copyright = "2021-2022, Felix Hildén"
 version = Path(_package_root, "sphinx_codeautolink", "VERSION").read_text().strip()
 release = version
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
     "sphinx.ext.intersphinx",
     "sphinx.ext.extlinks",
     "sphinx_rtd_theme",
     "sphinx_codeautolink",
     "matplotlib.sphinxext.plot_directive",
     "sphinx.ext.doctest",
+    "IPython.sphinxext.ipython_directive",
+    "IPython.sphinxext.ipython_console_highlighting",
 ]
 
 # Builtin options
 html_theme = "sphinx_rtd_theme"
 python_use_unqualified_type_names = True
 
 # Extension options
@@ -37,14 +39,15 @@
 
 autodoc_default_options = {
     "members": True,
     "undoc-members": True,
 }
 autodoc_typehints = "description"
 intersphinx_mapping = {
+    "python": ('https://docs.python.org/3/', None),
     "numpy": ("https://numpy.org/doc/stable/", None),
     "matplotlib": ("https://matplotlib.org/stable/", None),
 }
 extlinks = {
     'issue': ('https://github.com/felix-hilden/sphinx-codeautolink/issues/%s', '#'),
 }
 # Copy plot directive options from Seaborn
```

### Comparing `sphinx-codeautolink-0.8.0/docs/src/examples.rst` & `sphinx-codeautolink-0.9.0/docs/src/examples.rst`

 * *Files 7% similar despite different names*

```diff
@@ -154,19 +154,26 @@
        lines.append("   :collapse:")
 
    def setup(app):
        app.connect("autodoc-process-docstring", process_docstring)
 
 Intersphinx integration
 -----------------------
-When writing documentation that references other libraries, `intersphinx
+When writing code examples that use builtins or other libraries, `intersphinx
 <https://www.sphinx-doc.org/en/master/usage/extensions/intersphinx.html>`_
-is a great extension to use. It enables links to documentation on other sites.
-sphinx-codeautolink integrates this functionality seamlessly,
-linking objects as long as the correct ``intersphinx_mapping`` is defined.
+can be used to enable links to documentation on other Sphinx-generated sites.
+Intersphinx is integrated seamlessly, linking objects as long as the correct
+``intersphinx_mapping`` is defined.
+
+.. code:: python
+
+   if __debug__:
+       print(...)
+   else:
+       raise RuntimeError(f"Could not debug!")
 
 .. code:: python
 
    import numpy as np
    from matplotlib import pyplot as plt
 
    x = np.linspace(0, 2 * np.pi, 100)
@@ -208,31 +215,41 @@
 However, any test setup and teardown code is not taken into account.
 
 .. doctest::
 
    >>> import lib
    >>> lib.Knight()
 
-IPython code blocks
--------------------
-Code blocks using the language setting ``ipython3`` are supported by default.
+IPython blocks and notebooks
+----------------------------
+Code blocks using ``ipython`` or ``ipython3`` lexers are supported by default.
 The function :func:`~sphinx_codeautolink.clean_ipython` is used to handle
-IPython-specific syntax like so-called `magic functions`_.
+IPython-specific syntax like `magic functions`_ and console prefixes.
 
 .. _magic functions: https://ipython.readthedocs.io/en/stable/
    interactive/tutorial.html#magic-functions
 
 .. code:: ipython3
 
    %reset
    import lib
    lib.Knight().taunt()
 
-This is useful for integrating Jupyter notebooks, which is possible with
-separate Sphinx extensions like nbsphinx_ or MyST-NB_.
+IPython's ``.. ipython::`` `directive <https://ipython.readthedocs.io/en/
+stable/sphinxext.html#>`_ is also supported:
+
+.. ipython::
+
+   In [1]: import lib
+
+   In [2]: lib.Knight().taunt()
+   Out[2]: -taunt here-
+
+They are also useful for integrating Jupyter notebooks and similar source code,
+which is possible with separate Sphinx extensions like nbsphinx_ or MyST-NB_.
 IPython processing is enabled if the ``ipython`` library is installed.
 It is also included in the ``ipython`` extra of sphinx-codeautolink.
 
 .. code:: sh
 
    pip install sphinx-codeautolink[ipython]
```

### Comparing `sphinx-codeautolink-0.8.0/docs/src/index.rst` & `sphinx-codeautolink-0.9.0/docs/src/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/docs/src/lib.py` & `sphinx-codeautolink-0.9.0/docs/src/lib.py`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/docs/src/reference.rst` & `sphinx-codeautolink-0.9.0/docs/src/reference.rst`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,16 @@
    They are registered as a dict mapping a block lexer name to a function
    possibly cleaning up the block content to valid Python syntax.
    If none is specified, no transformations are applied.
    A string is interpreted as an importable transformer function.
    The transformer must return two strings: the code appearing in documentation
    (often just the original source) and the cleaned Python source code.
    The transformer must preserve line numbers for correct matching.
+   The transformer may raise a syntax error, which is caught automatically and
+   a corresponding Sphinx warning using subtype "parsing_error" is issued.
 
 .. confval:: codeautolink_search_css_classes
 
    Type: ``List[str]``. Extra CSS classes used to search for code examples
    when matching the final HTML. May contain multiple values separated by
    spaces as they would be passed to :code:`bs4.BeautifulSoup.find_all`.
 
@@ -116,7 +118,20 @@
 The functions below are usable for cleaning
 ``pycon`` and ``ipython`` code blocks.
 They are intended to be used with :confval:`codeautolink_custom_blocks`.
 
 .. autofunction:: sphinx_codeautolink.clean_pycon
 
 .. autofunction:: sphinx_codeautolink.clean_ipython
+
+Warning types
+-------------
+Sphinx logging machinery is used to issue warnings during documentation builds.
+All warning subtypes below are in the ``codeautolink.*`` namespace
+and can be ignored with configuring ``suppress_warnings``.
+
+- ``invalid_argument``: issued when a directive is used incorrectly
+- ``parse_block``: issued when parsing a code block fails
+- ``import_star``: issued when a library cannot be imported to determine
+  the names that an ``import *`` would introduce
+- ``match_block``: issued when a block cannot be matched
+- ``match_name``: issued when a code snippet cannot be matched
```

### Comparing `sphinx-codeautolink-0.8.0/docs/src/release_notes.rst` & `sphinx-codeautolink-0.9.0/docs/src/release_notes.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 =============
 
 These release notes are based on
 `Keep a Changelog <https://keepachangelog.com>`_.
 sphinx-codeautolink adheres to
 `Semantic Versioning <https://semver.org>`_.
 
+0.9.0 (2022-01-13)
+------------------
+- Use Sphinx logging instead of raising exceptions (:issue:`86`)
+- Link builtins if visible to intersphinx (:issue:`87`)
+- Use Sphinx logging instead of the builtin ``warnings`` to warn
+  (:issue:`89`, :issue:`94`)
+- Support IPython's ``.. ipython::`` directive (:issue:`91`)
+
 0.8.0 (2021-12-16)
 ------------------
 - Correctly test for optional types in annotations (:issue:`72`)
 - Don't check for ``notranslate`` CSS class, allowing for additional classes
   (:issue:`75`)
 - Allow to specify block parsers as importable references (:issue:`76`)
 - Allow parallel builds (:issue:`77`)
```

### Comparing `sphinx-codeautolink-0.8.0/readme_pypi.rst` & `sphinx-codeautolink-0.9.0/readme_pypi.rst`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/setup.py` & `sphinx-codeautolink-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/__init__.py` & `sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/extension/__init__.py` & `sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/extension/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 from traceback import print_exc
 from pathlib import Path
 
 from sphinx.util import import_object
 from sphinx.ext.intersphinx import InventoryAdapter
 
 from .backref import CodeRefsVisitor, CodeExample
-from .block import (
-    CodeBlockAnalyser, SourceTransform, link_html, UserError, ParsingError
-)
+from .block import CodeBlockAnalyser, SourceTransform, link_html
 from .directive import RemoveExtensionVisitor
 from .cache import DataCache
 from .resolve import resolve_location
 
 
 @dataclass
 class DocumentedObject:
@@ -36,16 +34,14 @@
     is pulled from the second argument named "doctree" and added to the message.
     """
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
-            except (UserError, ParsingError):
-                raise
             except Exception as e:
                 print_exc()
                 if append_source:
                     doctree = args[2] if len(args) > 1 else kwargs['doctree']
                     source = doctree['source']
                     msg = f'in document `{source}`'
                     if e.args:
```

### Comparing `sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/extension/backref.py` & `sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/extension/backref.py`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/extension/block.py` & `sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/extension/block.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Code block processing."""
 import re
 
 from typing import List, Union, Optional, Dict, Callable, Tuple
 from pathlib import Path
-from warnings import warn
 from dataclasses import dataclass
 
 from bs4 import BeautifulSoup
 from docutils import nodes
 
 from ..parse import parse_names, Name, LinkContext
 from .backref import CodeExample
 from .directive import ConcatMarker, PrefaceMarker, SkipMarker
-
+from ..warn import logger, warn_type
 
 BUILTIN_BLOCKS = {
     'python': None,
     'py': None,
 }
 
 
@@ -25,22 +24,14 @@
     """Transforms on source code."""
 
     source: str
     names: List[Name]
     example: CodeExample
 
 
-class ParsingError(Exception):
-    """Error in sphinx-autocodelink parsing."""
-
-
-class UserError(Exception):
-    """Error in sphinx-autocodelink usage."""
-
-
 def clean_pycon(source: str) -> Tuple[str, str]:
     """Clean up Python console syntax to pure Python."""
     in_statement = False
     source = re.sub(r'^\s*<BLANKLINE>', '', source, flags=re.MULTILINE)
     clean_lines = []
     for line in source.split('\n'):
         if line.startswith('>>> '):
@@ -54,25 +45,36 @@
     return source, '\n'.join(clean_lines)
 
 
 BUILTIN_BLOCKS['pycon'] = clean_pycon
 
 
 def clean_ipython(source: str) -> Tuple[str, str]:
-    """Clean up IPython syntax to pure Python."""
+    """Clean up IPython magics and console syntax to pure Python."""
     from IPython.core.inputtransformer2 import TransformerManager
-    return source, TransformerManager().transform_cell(source)
+
+    in_statement = True
+    clean_lines = []
+    for line in source.split('\n'):
+        if re.match(r'^In \[[0-9]+\]: ', line):
+            in_statement = True
+        elif re.match(r'^Out\[[0-9]+\]: ', line):
+            in_statement = False
+        clean_lines.append(line * in_statement)
+
+    return source, TransformerManager().transform_cell('\n'.join(clean_lines))
 
 
 try:
     import IPython
 except ImportError:
     pass
 else:
     del IPython
+    BUILTIN_BLOCKS['ipython'] = clean_ipython
     BUILTIN_BLOCKS['ipython3'] = clean_ipython
 
 
 class CodeBlockAnalyser(nodes.SparseNodeVisitor):
     """Transform literal blocks of Python with links to reference documentation."""
 
     def __init__(
@@ -100,34 +102,34 @@
         self.concat_sources = []
         self.skip = None
 
     def unknown_visit(self, node):
         """Handle and delete custom directives, ignore others."""
         if isinstance(node, ConcatMarker):
             if node.mode not in ('off', 'section', 'on'):
-                raise UserError(
-                    f'Invalid concatenation argument: `{node.mode}` '
-                    f'in document "{self.current_document}"'
+                msg = f'Invalid concatenation argument: `{node.mode}`'
+                logger.error(
+                    msg, type=warn_type, subtype='invalid_argument', location=node
                 )
 
             self.concat_sources = []
             if node.mode == 'section':
                 self.concat_section = True
             else:
                 self.concat_section = False
                 self.concat_global = (node.mode == 'on')
             node.parent.remove(node)
         elif isinstance(node, PrefaceMarker):
             self.prefaces.extend(node.content.split('\n'))
             node.parent.remove(node)
         elif isinstance(node, SkipMarker):
             if node.level not in ('next', 'section', 'file', 'off'):
-                raise UserError(
-                    f'Invalid skipping argument: `{node.level}` '
-                    f'in document "{self.current_document}"'
+                msg = f'Invalid skipping argument: `{node.level}`'
+                logger.error(
+                    msg, type=warn_type, subtype='invalid_argument', location=node
                 )
             self.skip = node.level if node.level != 'off' else None
             node.parent.remove(node)
 
     def unknown_departure(self, node):
         """Ignore unknown nodes."""
 
@@ -176,15 +178,23 @@
             or language not in self.valid_blocks
         ):
             return
 
         source = node.children[0].astext()
         transformer = self.transformers[language]
         if transformer:
-            source, clean_source = transformer(source)
+            try:
+                source, clean_source = transformer(source)
+            except SyntaxError as e:
+                show_source = self._format_source_for_error(source, prefaces)
+                msg = self._parsing_error_msg(e, language, show_source)
+                logger.warning(
+                    msg, type=warn_type, subtype='parse_block', location=node
+                )
+                return
         else:
             clean_source = source
         example = CodeExample(
             self.current_document, self.current_refid, list(self.title_stack)
         )
         transform = SourceTransform(source, [], example)
         self.source_transforms.append(transform)
@@ -192,39 +202,20 @@
         modified_source = '\n'.join(
             self.global_preface
             + self.concat_sources
             + prefaces
             + [clean_source]
         )
         try:
-            names = parse_names(modified_source)
+            names = parse_names(modified_source, node)
         except SyntaxError as e:
-            guides = [''] * len(modified_source)
-            ix = 0
-            if self.global_preface:
-                guides[0] = 'global preface:'
-                ix += len(self.global_preface)
-            if self.concat_sources:
-                guides[ix] = 'concatenations:'
-                ix += len(self.concat_sources)
-            if prefaces:
-                guides[ix] = 'local preface:'
-                ix += len(prefaces)
-            guides[ix] = 'block source:'
-            pad = max(len(i) + 1 for i in guides)
-            guides = [g.ljust(pad) for g in guides]
-            split_source = modified_source.split('\n')
-            show_source = '\n'.join([g + s for g, s in zip(guides, split_source)])
-
-            msg = '\n'.join([
-                str(e) + f' in document "{self.current_document}"',
-                f'Parsed source in `{language}` block:',
-                show_source,
-            ])
-            raise ParsingError(msg + '\n') from e
+            show_source = self._format_source_for_error(source, prefaces)
+            msg = self._parsing_error_msg(e, language, show_source)
+            logger.warning(msg, type=warn_type, subtype='parse_block', location=node)
+            return
 
         if prefaces or self.concat_sources or self.global_preface:
             concat_lens = [s.count('\n') + 1 for s in self.concat_sources]
             hidden_len = (
                 len(prefaces) + sum(concat_lens) + len(self.global_preface)
             )
             for name in names:
@@ -233,14 +224,39 @@
 
         if self.concat_section or self.concat_global:
             self.concat_sources.extend(prefaces + [clean_source])
 
         # Remove transforms from concatenated sources
         transform.names.extend([n for n in names if n.lineno > 0])
 
+    def _format_source_for_error(self, source: str, prefaces: List[str]) -> str:
+        split_source = source.split('\n')
+        guides = [''] * len(split_source)
+        ix = 0
+        if self.global_preface:
+            guides[0] = 'global preface:'
+            ix += len(self.global_preface)
+        if self.concat_sources:
+            guides[ix] = 'concatenations:'
+            ix += len(self.concat_sources)
+        if prefaces:
+            guides[ix] = 'local preface:'
+            ix += len(prefaces)
+        guides[ix] = 'block source:'
+        pad = max(len(i) + 1 for i in guides)
+        guides = [g.ljust(pad) for g in guides]
+        return '\n'.join([g + s for g, s in zip(guides, split_source)])
+
+    def _parsing_error_msg(self, error: Exception, language: str, source: str) -> str:
+        return '\n'.join([
+            str(error) + f' in document "{self.current_document}"',
+            f'Parsed source in `{language}` block:',
+            source,
+        ])
+
 
 def link_html(
     document: Path,
     out_dir: str,
     transforms: List[SourceTransform],
     inventory: dict,
     custom_blocks: dict,
@@ -269,37 +285,38 @@
 
     for trans in transforms:
         for ix in range(len(inners)):
             if trans.source.rstrip() == ''.join(inners[ix].strings).rstrip():
                 inner = inners.pop(ix)
                 break
         else:
-            msg = (
-                f'Could not match a code example to HTML in document "{document}", '
-                f'source:\n{trans.source}'
+            msg = f'Could not match a code example to HTML, source:\n{trans.source}'
+            logger.warning(
+                msg, type=warn_type, subtype='match_block', location=str(document)
             )
-            warn(msg, RuntimeWarning)
             continue
 
         lines = str(inner).split('\n')
 
         for name in trans.names:
             begin_line = name.lineno - 1
             end_line = name.end_lineno - 1
             selection = '\n'.join(lines[begin_line:end_line + 1])
 
             # Reverse because a.b = a.b should replace from the right
             matches = list(re.finditer(construct_name_pattern(name), selection))[::-1]
             if not matches:
                 msg = (
                     f'Could not match transformation of `{name.code_str}` '
-                    f'on source lines {name.lineno}-{name.end_lineno} '
-                    f'in document "{document}", source:\n{trans.source}'
+                    f'on source lines {name.lineno}-{name.end_lineno}, '
+                    f'source:\n{trans.source}'
+                )
+                logger.warning(
+                    msg, type=warn_type, subtype='match_name', location=str(document)
                 )
-                warn(msg, RuntimeWarning)
                 continue
 
             start, end = matches[0].span()
             start += len(matches[0].group(1))
             location = inventory[name.resolved_location]
             if not any(location.startswith(s) for s in ('http://', 'https://')):
                 location = local_prefix + location
@@ -317,18 +334,18 @@
 
 
 # ---------------------------------------------------------------
 # Patterns for different types of name access in highlighted HTML
 # ---------------------------------------------------------------
 period = r'\s*<span class="o">.</span>\s*'
 name_pattern = '<span class="n">{name}</span>'
-# Pygments has special classes for decorators (nd) and builtins (nb),
+# Pygments has special classes for different types of nouns
 # which are also highlighted in import statements
-first_name_pattern = '<span class="n[bd]?">@?{name}</span>'
-import_target_pattern = '<span class="n[nb]?">{name}</span>'
+first_name_pattern = '<span class="[a-z]+">@?{name}</span>'
+import_target_pattern = '<span class="[a-z]+">{name}</span>'
 import_from_pattern = '<span class="nn">{name}</span>'
 
 # The builtin re doesn't support variable-width lookbehind,
 # so instead we use a match groups in all pre patterns to remove the non-content.
 no_dot_prere = r'(?<!<span class="o">\.</span>)()'
 # Potentially instead assert an initial closing parenthesis followed by a dot.
 call_dot_prere = r'(\)</span>\s*<span class="o">\.</span>\s*)'
```

### Comparing `sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/extension/cache.py` & `sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/extension/cache.py`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/extension/directive.py` & `sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/extension/directive.py`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/extension/resolve.py` & `sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/extension/resolve.py`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/src/sphinx_codeautolink/parse.py` & `sphinx-codeautolink-0.9.0/src/sphinx_codeautolink/parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Analyse AST of code blocks to determine used names and their sources."""
 import ast
 import sys
+import builtins
 
 from contextlib import contextmanager
 from enum import Enum
 from functools import wraps
 from importlib import import_module
 from typing import Dict, Union, List, Optional, Tuple
-from warnings import warn
 from dataclasses import dataclass, field
 
+from .warn import logger, warn_type
 
-def parse_names(source: str) -> List['Name']:
+
+def parse_names(source: str, doctree_node) -> List['Name']:
     """Parse names from source."""
     tree = ast.parse(source)
-    visitor = ImportTrackerVisitor()
+    visitor = ImportTrackerVisitor(doctree_node)
     visitor.visit(tree)
     return sum([split_access(a) for a in visitor.accessed], [])
 
 
 @dataclass
 class PendingAccess:
     """Pending name access."""
@@ -197,27 +199,35 @@
                 self._resolve_assignment(r)
             elif isinstance(r, PendingAccess):
                 self._access(r)
         return r
     return wrapper
 
 
+builtin_components: Dict[str, List[Component]] = {
+    b: [Component(b, -1, -1, LinkContext.none)] for b in dir(builtins)
+}
+
+
 class ImportTrackerVisitor(ast.NodeVisitor):
     """Track imports and their use through source code."""
 
-    def __init__(self):
+    def __init__(self, doctree_node):
         super().__init__()
         self.accessed: List[Access] = []
         self.in_augassign = False
         self._parents = 0
+        self.doctree_node = doctree_node
 
         # Stack for dealing with class body pseudo scopes
         # which are completely bypassed by inner scopes (func, lambda).
         # Current values are copied to the next class body level.
-        self.pseudo_scopes_stack: List[Dict[str, List[Component]]] = [{}]
+        self.pseudo_scopes_stack: List[Dict[str, List[Component]]] = [
+            builtin_components.copy()
+        ]
         # Stack for dealing with nested scopes.
         # Holds references to the values of previous nesting levels.
         self.outer_scopes_stack: List[Dict[str, List[Component]]] = []
 
     @contextmanager
     def reset_parents(self):
         """Reset parents state for the duration of the context."""
@@ -344,15 +354,20 @@
             try:
                 mod = import_module(node.module)
                 import_names = [
                     name for name in mod.__dict__ if not name.startswith('_')
                 ]
                 aliases = [None] * len(import_names)
             except ImportError:
-                warn(f'Could not import module `{node.module}` for parsing!')
+                logger.warning(
+                    f'Could not import module `{node.module}` for parsing!',
+                    type=warn_type,
+                    subtype='import_star',
+                    location=self.doctree_node,
+                )
                 import_names = []
                 aliases = []
         else:
             import_names = [name.name for name in node.names]
             aliases = [name.asname for name in node.names]
 
         end_lineno = getattr(node, 'end_lineno', node.lineno)
@@ -522,15 +537,15 @@
         args = self._get_args(node.args)
         args += [node.args.vararg, node.args.kwarg]
         for arg in args:
             if arg is None or arg.annotation is None:
                 continue
             self.visit(arg.annotation)
 
-        inner = self.__class__()
+        inner = self.__class__(self.doctree_node)
         inner.pseudo_scopes_stack[0] = self.pseudo_scopes_stack[0].copy()
         inner.outer_scopes_stack = list(self.outer_scopes_stack)
         inner.outer_scopes_stack.append(self.pseudo_scopes_stack[0])
         for arg in args:
             if arg is None:
                 continue
             inner._overwrite(arg.arg)
@@ -543,15 +558,15 @@
         for d in node.args.defaults + node.args.kw_defaults:
             if d is None:
                 continue
             self.visit(d)
         args = self._get_args(node.args)
         args += [node.args.vararg, node.args.kwarg]
 
-        inner = self.__class__()
+        inner = self.__class__(self.doctree_node)
         inner.pseudo_scopes_stack[0] = self.pseudo_scopes_stack[0].copy()
         for arg in args:
             if arg is None:
                 continue
             inner._overwrite(arg.arg)
         inner.visit(node.body)
         self.accessed.extend(inner.accessed)
@@ -579,14 +594,14 @@
         for f in node.ifs:
             self.visit(f)
 
     def visit_generic_comp(
         self, values: List[ast.AST], generators: List[ast.comprehension]
     ):
         """Separate inner scope, respects class body scope."""
-        inner = self.__class__()
+        inner = self.__class__(self.doctree_node)
         inner.pseudo_scopes_stack[0] = self.pseudo_scopes_stack[-1].copy()
         for gen in generators:
             inner.visit(gen)
         for value in values:
             inner.visit(value)
         self.accessed.extend(inner.accessed)
```

### Comparing `sphinx-codeautolink-0.8.0/src/sphinx_codeautolink.egg-info/PKG-INFO` & `sphinx-codeautolink-0.9.0/src/sphinx_codeautolink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-codeautolink
-Version: 0.8.0
+Version: 0.9.0
 Summary: Automatic links from code examples to reference documentation.
 Home-page: https://pypi.org/project/sphinx-codeautolink
 Author: Felix Hildén
 Author-email: felix.hilden@gmail.com
 Maintainer: Felix Hildén
 Maintainer-email: felix.hilden@gmail.com
 License: MIT
```

### Comparing `sphinx-codeautolink-0.8.0/src/sphinx_codeautolink.egg-info/SOURCES.txt` & `sphinx-codeautolink-0.9.0/src/sphinx_codeautolink.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 docs/src/index.rst
 docs/src/lib.py
 docs/src/reference.rst
 docs/src/release_notes.rst
 src/sphinx_codeautolink/VERSION
 src/sphinx_codeautolink/__init__.py
 src/sphinx_codeautolink/parse.py
+src/sphinx_codeautolink/warn.py
 src/sphinx_codeautolink.egg-info/PKG-INFO
 src/sphinx_codeautolink.egg-info/SOURCES.txt
 src/sphinx_codeautolink.egg-info/dependency_links.txt
 src/sphinx_codeautolink.egg-info/requires.txt
 src/sphinx_codeautolink.egg-info/top_level.txt
 src/sphinx_codeautolink/extension/__init__.py
 src/sphinx_codeautolink/extension/backref.py
@@ -31,17 +32,20 @@
 src/sphinx_codeautolink/extension/resolve.py
 src/sphinx_codeautolink/static/sphinx-codeautolink.css
 tests/__init__.py
 tests/extension/__init__.py
 tests/extension/_check.py
 tests/extension/fail/concat_invalid.txt
 tests/extension/fail/custom_block_import_invalid.txt
+tests/extension/fail/ref_import_star_invalid.txt
 tests/extension/fail/ref_invalid_block_type.txt
 tests/extension/fail/ref_invalid_syntax.txt
 tests/extension/fail/ref_invalid_syntax_complex.txt
+tests/extension/fail/ref_ipython_non-python.txt
+tests/extension/fail/ref_ipython_syntax.txt
 tests/extension/fail/skip_invalid.txt
 tests/extension/ref/concat_default.txt
 tests/extension/ref/concat_off.txt
 tests/extension/ref/concat_on_across_sections.txt
 tests/extension/ref/concat_on_breaks.txt
 tests/extension/ref/concat_section_breaks.txt
 tests/extension/ref/concat_section_returns_to_global.txt
@@ -55,14 +59,15 @@
 tests/extension/ref/preface_global.txt
 tests/extension/ref/preface_global_multiline.txt
 tests/extension/ref/preface_global_overwritten.txt
 tests/extension/ref/preface_multiline.txt
 tests/extension/ref/preface_multiline_and_arg.txt
 tests/extension/ref/preface_multiple.txt
 tests/extension/ref/preface_single.txt
+tests/extension/ref/ref_builtins.txt
 tests/extension/ref/ref_chain.txt
 tests/extension/ref/ref_class_attr.txt
 tests/extension/ref/ref_class_meth_returns_self.txt
 tests/extension/ref/ref_decorator.txt
 tests/extension/ref/ref_doctest.txt
 tests/extension/ref/ref_extdoctest_doctest.txt
 tests/extension/ref/ref_extdoctest_testcode.txt
@@ -76,14 +81,16 @@
 tests/extension/ref/ref_import_star.txt
 tests/extension/ref/ref_import_submodule.txt
 tests/extension/ref/ref_imported_func.txt
 tests/extension/ref/ref_imported_func_relocated.txt
 tests/extension/ref/ref_inherited.txt
 tests/extension/ref/ref_intersphinx_only.txt
 tests/extension/ref/ref_ipython.txt
+tests/extension/ref/ref_ipython3.txt
+tests/extension/ref/ref_ipython_directive.txt
 tests/extension/ref/ref_optional.txt
 tests/extension/ref/ref_optional_counter.txt
 tests/extension/ref/ref_optional_manual.txt
 tests/extension/ref/ref_py.txt
 tests/extension/ref/ref_pycon.txt
 tests/extension/ref/ref_shadow_builtin.txt
 tests/extension/ref/ref_simple.txt
```

### Comparing `sphinx-codeautolink-0.8.0/tests/extension/__init__.py` & `sphinx-codeautolink-0.9.0/tests/extension/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,14 +282,14 @@
     """Build Sphinx documentation and return result folder."""
     src_dir = folder / 'src'
     src_dir.mkdir(exist_ok=True)
     for name, content in files.items():
         (src_dir / name).write_text(content, 'utf-8')
 
     build_dir = folder / 'build'
-    args = ['-M', builder, str(src_dir), str(build_dir)]
+    args = ['-M', builder, str(src_dir), str(build_dir), '-W']
     if n_processes:
         args.extend(['-j', str(n_processes)])
     ret_val = sphinx_main(args)
     if ret_val:
         raise RuntimeError('Sphinx build failed!')
     return build_dir / builder
```

### Comparing `sphinx-codeautolink-0.8.0/tests/extension/_check.py` & `sphinx-codeautolink-0.9.0/tests/extension/_check.py`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/tests/extension/ref/ref_extdoctest_doctest.txt` & `sphinx-codeautolink-0.9.0/tests/extension/ref/ref_extdoctest_doctest.txt`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/tests/extension/src/test_project/__init__.py` & `sphinx-codeautolink-0.9.0/tests/extension/src/test_project/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/tests/parse/__init__.py` & `sphinx-codeautolink-0.9.0/tests/parse/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,27 @@
         return '', []
 
     @refs_equal
     def test_no_imports(self):
         return '1\na = 2\nb()', []
 
     @refs_equal
+    def test_builtins(self):
+        s = 'print()'
+        refs = [('print', 'print')]
+        return s, refs
+
+    @pytest.mark.xfail(reason='Magics are currently not tracked.')
+    @refs_equal
+    def test_magics(self):
+        s = '__file__'
+        refs = [('__file__', '__file__')]
+        return s, refs
+
+    @refs_equal
     def test_import_from(self):
         s = 'from lib import a'
         refs = [('lib', 'lib'), ('lib.a', 'a')]
         return s, refs
 
     @refs_equal
     def test_import_from_as(self):
@@ -119,13 +132,7 @@
     def test_import_star(self):
         s = 'from sphinx_codeautolink import *\nsetup'
         refs = [
             ('sphinx_codeautolink', 'sphinx_codeautolink'),
             ('sphinx_codeautolink.setup', 'setup')
         ]
         return s, refs
-
-    @refs_equal
-    def test_import_star_invalid(self):
-        s = 'from not_a_module import *'
-        refs = [('not_a_module', 'not_a_module')]
-        return s, refs
```

### Comparing `sphinx-codeautolink-0.8.0/tests/parse/assign.py` & `sphinx-codeautolink-0.9.0/tests/parse/assign.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,33 +75,33 @@
     def test_augassign_uses_and_assigns_imported(self):
         s = 'import a\na += a\na'
         refs = [('a', 'a'), ('a', 'a'), ('a', 'a'), ('a', 'a')]
         return s, refs
 
     @refs_equal
     def test_annassign_uses_imported(self):
-        s = 'import a\na: str = 1\na'
+        s = 'import a\na: b = 1\na'
         refs = [('a', 'a')]
         return s, refs
 
     @refs_equal
     def test_annassign_uses_and_assigns_imported(self):
-        s = 'import a\na: str = a\na'
+        s = 'import a\na: b = a\na'
         refs = [('a', 'a'), ('a', 'a'), ('a', 'a')]
         return s, refs
 
     @refs_equal
     def test_annassign_why_would_anyone_do_this(self):
         s = 'import a\na: a = a\na'
         refs = [('a', 'a'), ('a', 'a'), ('a', 'a'), ('a', 'a')]
         return s, refs
 
     @refs_equal
     def test_annassign_without_value_overrides_annotation_but_not_linked(self):
-        s = 'import a\na: str\na'
+        s = 'import a\na: b\na'
         refs = [('a', 'a'), ('a', 'a')]
         return s, refs
 
     @pytest.mark.skipif(
         sys.version_info < (3, 8), reason='Walrus introduced in Python 3.8.'
     )
     @refs_equal
```

### Comparing `sphinx-codeautolink-0.8.0/tests/parse/chain.py` & `sphinx-codeautolink-0.9.0/tests/parse/chain.py`

 * *Files identical despite different names*

### Comparing `sphinx-codeautolink-0.8.0/tests/parse/scope.py` & `sphinx-codeautolink-0.9.0/tests/parse/scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,79 +171,79 @@
         refs = [('a', 'a'), ('a', 'a'), ('a', 'a')]  # refs in global and del
         return s, refs
 
 
 class TestComprehension:
     @refs_equal
     def test_comp_uses_in_value(self):
-        s = 'import a\n[a for _ in range(2)]'
+        s = 'import a\n[a for b in c]'
         refs = [('a', 'a'), ('a', 'a')]
         return s, refs
 
     @refs_equal
     def test_setcomp_uses_in_value(self):
-        s = 'import a\n{a for _ in range(2)}'
+        s = 'import a\n{a for b in c}'
         refs = [('a', 'a'), ('a', 'a')]
         return s, refs
 
     @refs_equal
     def test_dictcomp_uses_in_value(self):
-        s = 'import a\n{a: a for _ in range(2)}'
+        s = 'import a\n{a: a for b in c}'
         refs = [('a', 'a'), ('a', 'a'), ('a', 'a')]
         return s, refs
 
     @refs_equal
     def test_generator_uses_in_value(self):
-        s = 'import a\n(a for _ in range(2))'
+        s = 'import a\n(a for b in c)'
         refs = [('a', 'a'), ('a', 'a')]
         return s, refs
 
     @refs_equal
     def test_comp_uses_in_ifs(self):
-        s = 'import a\n[_ for _ in range(2) if a]'
+        s = 'import a\n[_ for _ in b if a]'
         refs = [('a', 'a'), ('a', 'a')]
         return s, refs
 
     @refs_equal
     def test_comp_uses_in_iter(self):
-        s = 'import a\n[_ for _ in range(a)]'
+        s = 'import a\n[_ for _ in b(a)]'
         refs = [('a', 'a'), ('a', 'a')]
         return s, refs
 
     @refs_equal
     def test_comp_overrides(self):
-        s = 'import a\n[a for a in range(2) if a]'
+        s = 'import a\n[a for a in b if a]'
         refs = [('a', 'a')]
         return s, refs
 
     @refs_equal
     def test_comp_overrides_used_after(self):
-        s = 'import a\n[a for a in range(2)]\na'
+        s = 'import a\n[a for a in b]\na'
         refs = [('a', 'a'), ('a', 'a')]
         return s, refs
 
     @refs_equal
     def test_multicomp_overrides(self):
-        s = 'import a\n[a for a in range(2) for b in a]'
+        s = 'import a\n[a for a in b for b in a]'
         refs = [('a', 'a')]
         return s, refs
 
     @refs_equal
     def test_multicomp_uses_then_overrides(self):
-        s = 'import a\n[a for b in range(a) for a in b]'
+        s = 'import a\n[a for b in c(a) for a in b]'
         refs = [('a', 'a'), ('a', 'a')]
         return s, refs
 
     @pytest.mark.skipif(
         sys.version_info < (3, 8), reason='Walrus introduced in Python 3.8.'
     )
     @pytest.mark.xfail(reason='Assignments are not tracked.')
     @refs_equal
     def test_comp_leaks_walrus(self):
-        s = 'import a\n[a := i for i in range(2)]\na'
+        s = 'import a\n[a := i for i in b]\na'
         refs = [('a', 'a')]
         return s, refs
 
 
 class TestClass:
     @refs_equal
     def test_class_name_shadows(self):
```

