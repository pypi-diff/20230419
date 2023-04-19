# Comparing `tmp/pyftdc-0.3.2.tar.gz` & `tmp/pyftdc-0.3.4.macosx-12-arm64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyftdc-0.3.2.tar", last modified: Fri Dec  9 03:22:14 2022, max compression
+gzip compressed data, was "pyftdc-0.3.4.macosx-12-arm64.tar", last modified: Wed Apr 19 15:44:26 2023, max compression
```

## Comparing `pyftdc-0.3.2.tar` & `pyftdc-0.3.4.macosx-12-arm64.tar`

### file list

```diff
@@ -1,305 +1,39 @@
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.806460 pyftdc-0.3.2/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1224 2022-11-25 23:53:40.000000 pyftdc-0.3.2/CMakeLists.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2182 2022-11-25 22:23:11.000000 pyftdc-0.3.2/LICENSE
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      444 2022-11-26 00:11:52.000000 pyftdc-0.3.2/MANIFEST.in
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      310 2022-12-09 03:22:14.806323 pyftdc-0.3.2/PKG-INFO
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7595 2022-12-01 19:40:04.000000 pyftdc-0.3.2/README.md
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.762653 pyftdc-0.3.2/extern/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1386 2022-11-25 22:23:41.000000 pyftdc-0.3.2/extern/CMakeLists.txt
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.764526 pyftdc-0.3.2/pybind11/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1304 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/.appveyor.yml
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      996 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/.clang-format
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2210 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/.clang-tidy
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2196 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/.cmake-format.yaml
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      487 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/.gitignore
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3477 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       62 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/.readthedocs.yml
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    10999 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/CMakeLists.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1684 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/LICENSE
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      256 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/MANIFEST.in
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7656 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/README.rst
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.768144 pyftdc-0.3.2/pybind11/docs/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      653 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/docs/Doxyfile
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.768294 pyftdc-0.3.2/pybind11/docs/_static/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      254 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/_static/theme_overrides.css
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.769152 pyftdc-0.3.2/pybind11/docs/advanced/
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.770176 pyftdc-0.3.2/pybind11/docs/advanced/cast/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3937 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3409 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14283 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3889 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1556 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    12433 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9703 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9363 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    48319 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8453 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    17806 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    26827 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    12446 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.770708 pyftdc-0.3.2/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      278 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    17447 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9030 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5710 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     6367 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9368 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/docs/basics.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2962 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/docs/benchmark.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3168 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/docs/benchmark.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    99067 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/docs/changelog.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    16451 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/docs/classes.rst
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.770831 pyftdc-0.3.2/pybind11/docs/cmake/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      273 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/cmake/index.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    26267 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/docs/compiling.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    12082 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/docs/conf.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14599 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/docs/faq.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      613 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/index.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3277 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/installing.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3079 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/docs/limitations.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    58510 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    44653 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    87708 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    41121 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    85853 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2647 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/reference.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4414 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/docs/release.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      130 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/docs/requirements.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    23491 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.760147 pyftdc-0.3.2/pybind11/include/
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.773711 pyftdc-0.3.2/pybind11/include/pybind11/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    23920 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/include/pybind11/attr.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7069 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    64793 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/cast.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8907 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      120 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/common.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2096 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.774879 pyftdc-0.3.2/pybind11/include/pybind11/detail/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    28526 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    51655 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5491 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    17971 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    24196 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    44414 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1513 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    31441 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    12175 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/include/pybind11/embed.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5589 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/eval.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4755 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/functional.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     6848 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/gil.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8851 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    78036 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9781 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/operators.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2181 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/options.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)   125927 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    80901 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.775017 pyftdc-0.3.2/pybind11/include/pybind11/stl/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3551 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14438 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/stl.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    26992 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2575 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/noxfile.py
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.776062 pyftdc-0.3.2/pybind11/pybind11/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      216 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/pybind11/__init__.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1158 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/pybind11/__main__.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      202 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/pybind11/_version.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      137 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/pybind11/_version.pyi
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      662 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/pybind11/commands.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        0 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/pybind11/py.typed
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    17483 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2038 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/pybind11/setup_helpers.pyi
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      957 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/pyproject.toml
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1910 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/setup.cfg
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5057 2022-11-25 22:23:12.000000 pyftdc-0.3.2/pybind11/setup.py
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.793240 pyftdc-0.3.2/pybind11/tests/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    21095 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4841 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/conftest.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    11734 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/constructor_stats.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1781 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1022 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/env.py
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.793542 pyftdc-0.3.2/pybind11/tests/extra_python_package/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        0 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7578 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.793864 pyftdc-0.3.2/pybind11/tests/extra_setuptools/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        0 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4221 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2847 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/local_bindings.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5743 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/object.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     6264 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3686 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3018 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      693 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/pytest.ini
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      877 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/requirements.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      855 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_async.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      558 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_async.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8567 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5055 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_buffers.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    15872 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    18372 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4118 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     6573 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_call_policies.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9243 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     6044 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_callbacks.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3370 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5727 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_chrono.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    23812 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_class.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14508 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_class.py
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.794443 pyftdc-0.3.2/pybind11/tests/test_cmake_build/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2639 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      673 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.794589 pyftdc-0.3.2/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1171 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.794883 pyftdc-0.3.2/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1293 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.795089 pyftdc-0.3.2/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1685 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      152 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.795282 pyftdc-0.3.2/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1353 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.795463 pyftdc-0.3.2/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1163 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.795641 pyftdc-0.3.2/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1368 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      273 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4254 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_const_name.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      650 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_const_name.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5934 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1522 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    10718 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4646 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_copy_move.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7210 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4088 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1259 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/test_custom_type_setup.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1114 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2816 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1630 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    18169 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/test_eigen.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    28283 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_eigen.py
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.796657 pyftdc-0.3.2/pybind11/tests/test_embed/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1798 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      733 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      543 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14173 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      280 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      300 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_embed/test_trampoline.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5722 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_enum.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9132 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_enum.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3168 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/test_eval.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1183 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_eval.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      143 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_eval_call.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    10197 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      399 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_exceptions.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9038 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_exceptions.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    18419 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    16731 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1673 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3128 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4122 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7958 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_iostream.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9236 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    13998 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4401 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8101 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    21327 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    17804 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4021 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_modules.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2843 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_modules.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    12305 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    12034 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    19774 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    20339 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    20154 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14036 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4461 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9710 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2777 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1907 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9463 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4392 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     6646 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2286 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_pickling.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    20878 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    19010 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_pytypes.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    20580 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8059 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    19040 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9620 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    20722 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/test_stl.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    11662 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_stl.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4622 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8071 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4597 2022-11-25 22:58:21.000000 pyftdc-0.3.2/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      765 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1855 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/test_thread.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      875 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_thread.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      603 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/test_union.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      172 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/test_union.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    23102 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    13146 2022-11-25 22:58:20.000000 pyftdc-0.3.2/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3226 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2657 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.799001 pyftdc-0.3.2/pybind11/tools/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2350 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3105 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    10378 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 jorge.imperial   (502) staff       (20)     1423 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tools/check-style.sh
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      952 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1122 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tools/libsize.py
--rwxr-xr-x   0 jorge.imperial   (502) staff       (20)     1306 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tools/make_changelog.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14579 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7063 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9673 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7447 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       94 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tools/pyproject.toml
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1951 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tools/setup_global.py.in
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1089 2022-11-25 22:23:11.000000 pyftdc-0.3.2/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.800041 pyftdc-0.3.2/pyftdc.egg-info/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      310 2022-12-09 03:22:14.000000 pyftdc-0.3.2/pyftdc.egg-info/PKG-INFO
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9161 2022-12-09 03:22:14.000000 pyftdc-0.3.2/pyftdc.egg-info/SOURCES.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        1 2022-12-09 03:22:14.000000 pyftdc-0.3.2/pyftdc.egg-info/dependency_links.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        1 2022-11-25 23:54:31.000000 pyftdc-0.3.2/pyftdc.egg-info/not-zip-safe
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       20 2022-12-09 03:22:14.000000 pyftdc-0.3.2/pyftdc.egg-info/requires.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        7 2022-12-09 03:22:14.000000 pyftdc-0.3.2/pyftdc.egg-info/top_level.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      797 2022-12-09 03:21:39.000000 pyftdc-0.3.2/pyproject.toml
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       38 2022-12-09 03:22:14.806506 pyftdc-0.3.2/setup.cfg
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5492 2022-11-26 21:33:51.000000 pyftdc-0.3.2/setup.py
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.802550 pyftdc-0.3.2/src/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2247 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/CSVWriter.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14348 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/Chunk.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      344 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/ChunkMetric.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      177 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/ConstDataRangeCursor.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    12870 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/Dataset.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7905 2022-11-28 21:36:22.000000 pyftdc-0.3.2/src/FTDCParser.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       69 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/FileParsedData.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1911 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/JSONWriter.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2744 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/MetricsToWTMap.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       62 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/ParserTask.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2240 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/ParserTasksList.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       68 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/SampleLocation.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       65 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/WriterTask.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      643 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/WriterTaskList.cpp
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.805185 pyftdc-0.3.2/src/include/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      447 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/CSVWriter.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3012 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/Chunk.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      787 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/ChunkMetric.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      633 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/ConstDataRangeCursor.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2826 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/Dataset.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1474 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/FTDCParser.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      885 2022-11-28 21:34:49.000000 pyftdc-0.3.2/src/include/FileParsedData.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      444 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/JSONWriter.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      271 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/Metrics.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      976 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/MetricsToWTMap.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      593 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/ParserTask.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      625 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/ParserTasksList.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      468 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/SampleLocation.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      261 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/Timestamp.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      392 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/WriterTask.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      676 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/WriterTaskList.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1470 2022-11-25 22:23:12.000000 pyftdc-0.3.2/src/include/bson_value.h
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2022-12-09 03:22:14.806125 pyftdc-0.3.2/src/pyftdc.egg-info/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8130 2022-12-09 02:43:29.000000 pyftdc-0.3.2/src/pyftdc.egg-info/PKG-INFO
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8983 2022-12-09 02:43:29.000000 pyftdc-0.3.2/src/pyftdc.egg-info/SOURCES.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        1 2022-12-09 02:43:29.000000 pyftdc-0.3.2/src/pyftdc.egg-info/dependency_links.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        1 2022-11-28 20:14:23.000000 pyftdc-0.3.2/src/pyftdc.egg-info/not-zip-safe
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       20 2022-12-09 02:43:29.000000 pyftdc-0.3.2/src/pyftdc.egg-info/requires.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       15 2022-12-09 02:43:29.000000 pyftdc-0.3.2/src/pyftdc.egg-info/top_level.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    15791 2022-12-09 02:41:39.000000 pyftdc-0.3.2/src/python.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        6 2022-12-09 03:21:56.000000 pyftdc-0.3.2/version.txt
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 15:44:26.345949 ./
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 15:44:26.346003 ./Users/
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 15:44:26.346053 ./Users/jorge.imperial/
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 15:44:26.346102 ./Users/jorge.imperial/CLionProjects/
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 15:44:26.346153 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 15:44:26.346202 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 15:44:26.346252 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 15:44:26.346308 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 15:44:26.353621 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 15:44:26.350768 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      894 2023-04-11 21:35:43.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/BinaryBSON.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      447 2023-03-29 21:01:49.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/CSVWriter.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      813 2023-04-11 21:35:43.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/ChunkMetric.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      633 2023-03-29 21:01:49.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/ConstDataRangeCursor.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2131 2023-04-11 21:35:43.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/Dataset.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1158 2023-04-01 15:17:09.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/FTDCParser.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      753 2023-03-29 21:01:49.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/FileParsedData.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      444 2023-03-29 21:01:49.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/JSONWriter.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      271 2023-03-29 21:01:49.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/Metrics.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      976 2023-03-29 21:01:49.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/MetricsToWTMap.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1420 2023-03-31 02:42:43.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/ParserState.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      593 2023-03-29 21:01:49.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/ParserTask.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      625 2023-03-29 21:01:49.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/ParserTasksList.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      468 2023-03-29 21:01:49.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/SampleLocation.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      261 2023-03-29 21:01:49.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/Timestamp.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      392 2023-03-29 21:01:49.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/WriterTask.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      676 2023-03-29 21:01:49.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/WriterTaskList.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1470 2023-03-29 21:01:49.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/bson_value.h
+-rwxr-xr-x   0 jorge.imperial   (502) staff       (20)   237680 2023-04-19 15:44:22.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/libbson-1.0.0.0.0.dylib
+-rwxr-xr-x   0 jorge.imperial   (502) staff       (20)   237680 2023-04-19 15:44:22.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/libbson-1.0.0.dylib
+-rwxr-xr-x   0 jorge.imperial   (502) staff       (20)   237680 2023-04-19 15:44:22.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/libbson-1.0.dylib
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 15:44:26.355078 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/pyftdc-0.3.4-py3.10.egg-info/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8130 2023-04-19 15:41:00.351613 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/pyftdc-0.3.4-py3.10.egg-info/PKG-INFO
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9039 2023-04-19 15:41:00.361172 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/pyftdc-0.3.4-py3.10.egg-info/SOURCES.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)        1 2023-04-19 15:41:00.351809 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/pyftdc-0.3.4-py3.10.egg-info/dependency_links.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)        1 2023-04-19 15:22:46.383948 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/pyftdc-0.3.4-py3.10.egg-info/not-zip-safe
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       20 2023-04-19 15:41:00.351983 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/pyftdc-0.3.4-py3.10.egg-info/requires.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       15 2023-04-19 15:41:00.352067 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/pyftdc-0.3.4-py3.10.egg-info/top_level.txt
+-rwxr-xr-x   0 jorge.imperial   (502) staff       (20)   586192 2023-04-19 15:44:26.000000 ./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/pyftdc.cpython-310-darwin.so
```

### Comparing `pyftdc-0.3.2/README.md` & `./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/pyftdc-0.3.4-py3.10.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: pyftdc
+Version: 0.3.4
+Summary: A small example package
+Author: Jorge Imperial
+Author-email: Jorge Imperial <jlimperial@protonmail.com>
+Project-URL: Homepage, https://gitlab.com/jimper/mongo_ftdc
+Project-URL: Bug Tracker, https://gitlab.com/jimper/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 pyftdc
 ==============
 
 
 |            | Link | status |
 |--------------|------|------|
 | Conda builds | https://anaconda.org/jimper/pyftdc |      |
```

### Comparing `pyftdc-0.3.2/pyftdc.egg-info/SOURCES.txt` & `./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/pyftdc-0.3.4-py3.10.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -223,45 +223,41 @@
 pybind11/tools/pybind11Common.cmake
 pybind11/tools/pybind11Config.cmake.in
 pybind11/tools/pybind11NewTools.cmake
 pybind11/tools/pybind11Tools.cmake
 pybind11/tools/pyproject.toml
 pybind11/tools/setup_global.py.in
 pybind11/tools/setup_main.py.in
-pyftdc.egg-info/PKG-INFO
-pyftdc.egg-info/SOURCES.txt
-pyftdc.egg-info/dependency_links.txt
-pyftdc.egg-info/not-zip-safe
-pyftdc.egg-info/requires.txt
-pyftdc.egg-info/top_level.txt
+src/BinaryBSON.cpp
 src/CSVWriter.cpp
-src/Chunk.cpp
 src/ChunkMetric.cpp
 src/ConstDataRangeCursor.cpp
 src/Dataset.cpp
 src/FTDCParser.cpp
 src/FileParsedData.cpp
 src/JSONWriter.cpp
 src/MetricsToWTMap.cpp
+src/ParserState.cpp
 src/ParserTask.cpp
 src/ParserTasksList.cpp
 src/SampleLocation.cpp
 src/WriterTask.cpp
 src/WriterTaskList.cpp
 src/python.cpp
+src/include/BinaryBSON.h
 src/include/CSVWriter.h
-src/include/Chunk.h
 src/include/ChunkMetric.h
 src/include/ConstDataRangeCursor.h
 src/include/Dataset.h
 src/include/FTDCParser.h
 src/include/FileParsedData.h
 src/include/JSONWriter.h
 src/include/Metrics.h
 src/include/MetricsToWTMap.h
+src/include/ParserState.h
 src/include/ParserTask.h
 src/include/ParserTasksList.h
 src/include/SampleLocation.h
 src/include/Timestamp.h
 src/include/WriterTask.h
 src/include/WriterTaskList.h
 src/include/bson_value.h
```

### Comparing `pyftdc-0.3.2/src/include/ChunkMetric.h` & `./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/ChunkMetric.h`

 * *Files 12% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 public:
 
     ChunkMetric(std::string name, bson_type_t param, int64_t init_value);
     ChunkMetric(std::string name);
 
     static const int MAX_SAMPLES = 300;
 
-    int getSampleCount() { return nSamples; }
+    [[nodiscard]] size_t getSampleCount() const { return nSamples; }
     std::string getName() { return name; }
     uint64_t *getValues() { return values; }
     uint64_t  getValue(unsigned long n) { return values[n]; }
 
     void setSampleCount(int samples) { nSamples = samples; }
 
 private:
-    int nSamples{};
+    size_t nSamples{};
     std::string name;
     bson_type_t  type{};
     uint64_t  values[MAX_SAMPLES];  // All metrics fit in a 64 bit integer so....
 };
 
 
 #endif //FTDCPARSER_METRIC_H
```

### Comparing `pyftdc-0.3.2/src/include/ConstDataRangeCursor.h` & `./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/ConstDataRangeCursor.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/include/Dataset.h` & `./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/Dataset.h`

 * *Files 16% similar despite different names*

```diff
@@ -7,75 +7,58 @@
 
 #include <string>
 #include <vector>
 #include <map>
 #include <mutex>
 
 #include "SampleLocation.h"
-#include "Chunk.h"
 #include "FileParsedData.h"
 #include "Timestamp.h"
 #include "Metrics.h"
 #include "MetricsToWTMap.h"
 
+using namespace ftdcparser;
 
 class Dataset {
 
 public:
-    Dataset() : samplesInDataset(0),  metricNames(0), lazyParsing(0) {};
-    Dataset(std::string csvFileName);
+    static const int INVALID_TIMESTAMP_POS = INT_MAX;
 
-    void addChunk(Chunk *pChunk);
-    size_t getChunkCount() { return chunkVector.size(); }
-    Chunk *getChunk(size_t n) { return (n < chunkVector.size()) ? chunkVector[n] : nullptr; }
-    std::vector<Chunk *> getChunkVector() { return chunkVector; }
-    // TODO: merge to have only one signature
-    size_t getMetricsNames(std::vector< std::string> & metricNames);
-    std::vector<std::string> getMetricsNames();
-
-    MetricsPtr getMetric(std::string   metricName, Timestamp start=Chunk::INVALID_TIMESTAMP_POS, Timestamp end=Chunk::INVALID_TIMESTAMP_POS, bool ratedMetric=false);
-    uint64_t getMetricValue(std::string metricName, size_t pos);
-
-    size_t getMetricNamesCount() { return metricNames.size(); }
-    void sortChunks();
-    void finishedParsingFile(std::string path, uint64_t start, uint64_t end, size_t samplesInFile);
-    bool IsMetricInDataset(const std::string& metric);
-    std::vector<FileParsedData*> getParsedFileInfo() {  return this->filesParsed; }
-    size_t LoadMetricsNamesFromChunk();
-    void setLazyParsingFlag(bool lazy) { lazyParsing = lazy; }
-    bool getLazyParsing() const { return lazyParsing; }
-    std::vector<MetricsPtr> getMetrics( std::vector<std::string> metricNames,
+    Dataset() :  samplesInDataset(0), start(INVALID_TIMESTAMP), end(INVALID_TIMESTAMP), metricNames(0){};
+    explicit Dataset(const std::string& csvFileName);
+    explicit Dataset(ParserState *pState, FileParsedData* fileParsedData);
+
+    std::vector< std::string> const *getMetricsNames();
+    MetricsPtr getMetric(std::string   metricName,
+                         Timestamp start = INVALID_TIMESTAMP,
+                         Timestamp end = INVALID_TIMESTAMP,
+                         bool ratedMetric=false);
+    int getIndexInMetrics(const std::string& metric);
+    FileParsedData*  getParsedFileInfo() {  return this->fileParsed; }
+    std::vector<MetricsPtr> getMetrics( std::vector<std::string> metricNamesIn,
                                                  size_t start,  size_t end,
                                                  bool ratedMetrics);
-    MetricsPtr getMetricMatrix( std::vector<std::string> metricNames, size_t *stride, Timestamp start,  Timestamp end,
-                     bool ratedMetrics);
-    Timestamp getStartTimestamp();
-    Timestamp getEndTimestamp();
-    std::string getJsonFromTimestamp(Timestamp ts);
-    std::string getCsvFromTimestamp(Timestamp ts);
-    std::string getJsonAtPosition(int pos);
-    SampleLocation getLocationInMetric(Timestamp ts, bool fromStart);
-    int releaseChunks();
-    void SetMetadata(std::string metadata);
-    std::string getMetadata() { return metadata; }
-
-private:
-    std::vector<FileParsedData *> filesParsed;
-    MetricsPtr assembleMetricFromChunks(std::string name,  SampleLocation startLocation, SampleLocation endLocation);
-    bool ConvertToRatedMetric(MetricsPtr pVector);
+    MetricsPtr getMetricMatrix(const std::vector<std::string>& metricNamesToReturn, size_t *stride,
+                               Timestamp startLimit, Timestamp endLimit,
+                               bool ratedMetrics);
+    [[nodiscard]] Timestamp getStartTimestamp() const;
+    [[nodiscard]] Timestamp getEndTimestamp() const;
+    static std::string getJsonFromTimestamp(Timestamp ts);
+    static std::string getCsvFromTimestamp(Timestamp ts);
+    std::string getMetadata() { return parserState->getJSONMetadata();  }
 
+    void buildFromFTDC();
+    void buildFromFTDCThreaded();
 
 private:
-    std::vector<Chunk*> chunkVector;
-    size_t samplesInDataset;
-    std::mutex mu;
+    FileParsedData *fileParsed{};
+    bool ConvertToRatedMetric(MetricsPtr pVector);
     std::vector<std::string> metricNames;
-    std::string metadata;
-
-    bool lazyParsing;
 
+    ParserState *parserState{};
+    size_t samplesInDataset{};
 
+    Timestamp start;
+    Timestamp end;
 };
 
-
-
 #endif //FTDCPARSER_DATASET_H
```

### Comparing `pyftdc-0.3.2/src/include/MetricsToWTMap.h` & `./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/MetricsToWTMap.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/include/ParserTask.h` & `./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/ParserTask.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/include/ParserTasksList.h` & `./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/ParserTasksList.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/include/WriterTaskList.h` & `./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/WriterTaskList.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/include/bson_value.h` & `./Users/jorge.imperial/CLionProjects/mongo_ftdc/venv/lib/python3.10/site-packages/include/bson_value.h`

 * *Files identical despite different names*

