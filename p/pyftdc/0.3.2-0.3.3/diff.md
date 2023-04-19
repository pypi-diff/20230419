# Comparing `tmp/pyftdc-0.3.2.tar.gz` & `tmp/pyftdc-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyftdc-0.3.2.tar", last modified: Fri Dec  9 03:22:14 2022, max compression
+gzip compressed data, was "pyftdc-0.3.3.tar", last modified: Wed Apr 19 17:19:26 2023, max compression
```

## Comparing `pyftdc-0.3.2.tar` & `pyftdc-0.3.3.tar`

### file list

```diff
@@ -1,305 +1,300 @@
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
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.630099 pyftdc-0.3.3/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1109 2023-04-19 15:22:46.000000 pyftdc-0.3.3/CMakeLists.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2182 2023-03-29 21:01:49.000000 pyftdc-0.3.3/LICENSE
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      444 2023-03-29 21:01:49.000000 pyftdc-0.3.3/MANIFEST.in
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8130 2023-04-19 17:19:26.629880 pyftdc-0.3.3/PKG-INFO
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7595 2023-03-29 21:01:49.000000 pyftdc-0.3.3/README.md
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.588911 pyftdc-0.3.3/extern/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1386 2023-03-29 21:01:49.000000 pyftdc-0.3.3/extern/CMakeLists.txt
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.591259 pyftdc-0.3.3/pybind11/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1304 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/.appveyor.yml
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      996 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/.clang-format
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2210 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/.clang-tidy
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2196 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/.cmake-format.yaml
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      487 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/.gitignore
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3477 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       62 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/.readthedocs.yml
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    10999 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/CMakeLists.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1684 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/LICENSE
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      256 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/MANIFEST.in
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7656 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/README.rst
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.594809 pyftdc-0.3.3/pybind11/docs/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      653 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/Doxyfile
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.594972 pyftdc-0.3.3/pybind11/docs/_static/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      254 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/_static/theme_overrides.css
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.595962 pyftdc-0.3.3/pybind11/docs/advanced/
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.597237 pyftdc-0.3.3/pybind11/docs/advanced/cast/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3937 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3409 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14283 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3889 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1556 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    12433 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9703 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9363 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    48319 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8453 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    17806 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    26827 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    12446 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.597914 pyftdc-0.3.3/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      278 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    17447 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9030 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5710 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     6367 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9368 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/basics.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2962 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/benchmark.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3168 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/benchmark.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    99067 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/changelog.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    16451 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/classes.rst
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.598150 pyftdc-0.3.3/pybind11/docs/cmake/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      273 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    26267 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/compiling.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    12082 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/conf.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14599 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/faq.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      613 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/index.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3277 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/installing.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3079 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/limitations.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    58510 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    44653 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    87708 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    41121 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    85853 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2647 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/reference.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4414 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/release.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      130 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/requirements.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    23491 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.586228 pyftdc-0.3.3/pybind11/include/
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.601153 pyftdc-0.3.3/pybind11/include/pybind11/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    23920 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7069 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    64793 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8907 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      120 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/common.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2096 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.602259 pyftdc-0.3.3/pybind11/include/pybind11/detail/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    28526 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    51655 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5491 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    17971 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    24196 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    44414 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1513 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    31441 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    12175 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5589 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4755 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     6848 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8851 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    78036 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9781 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2181 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/options.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)   125927 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    80901 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.602398 pyftdc-0.3.3/pybind11/include/pybind11/stl/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3551 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14438 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    26992 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2575 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/noxfile.py
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.603554 pyftdc-0.3.3/pybind11/pybind11/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      216 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/__init__.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1158 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/__main__.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      202 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/_version.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      137 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/_version.pyi
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      662 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/commands.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)        0 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/py.typed
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    17483 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2038 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/setup_helpers.pyi
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      957 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pyproject.toml
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1910 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/setup.cfg
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5057 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/setup.py
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.617337 pyftdc-0.3.3/pybind11/tests/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    21095 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4841 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/conftest.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    11734 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1781 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1022 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/env.py
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.617749 pyftdc-0.3.3/pybind11/tests/extra_python_package/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)        0 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7578 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.618053 pyftdc-0.3.3/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)        0 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4221 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2847 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/local_bindings.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5743 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/object.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     6264 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3686 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3018 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      693 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/pytest.ini
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      877 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/requirements.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      855 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_async.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      558 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_async.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8567 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5055 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_buffers.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    15872 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    18372 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4118 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     6573 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9243 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     6044 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3370 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5727 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_chrono.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    23812 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_class.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14508 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_class.py
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.618641 pyftdc-0.3.3/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2639 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      673 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.618809 pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1171 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.618952 pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1293 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.619096 pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1685 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      152 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.619258 pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1353 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.619439 pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1163 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.619600 pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1368 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      273 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4254 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      650 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_const_name.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5934 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1522 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    10718 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4646 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7210 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4088 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1259 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1114 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2816 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1630 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    18169 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_eigen.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    28283 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_eigen.py
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.620488 pyftdc-0.3.3/pybind11/tests/test_embed/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1798 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      733 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      543 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14173 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      280 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      300 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5722 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9132 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_enum.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3168 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1183 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_eval.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      143 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    10197 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      399 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_exceptions.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9038 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    18419 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    16731 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1673 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3128 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4122 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7958 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_iostream.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9236 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    13998 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4401 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8101 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    21327 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    17804 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4021 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2843 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_modules.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    12305 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    12034 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    19774 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    20339 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    20154 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14036 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4461 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9710 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2777 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1907 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9463 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4392 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     6646 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2286 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_pickling.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    20878 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    19010 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    20580 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8059 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    19040 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9620 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    20722 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    11662 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_stl.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4622 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8071 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4597 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      765 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1855 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_thread.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      875 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_thread.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      603 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_union.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      172 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_union.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    23102 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    13146 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3226 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2657 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.622988 pyftdc-0.3.3/pybind11/tools/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2350 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3105 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    10378 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 jorge.imperial   (502) staff       (20)     1423 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/check-style.sh
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      952 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1122 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/libsize.py
+-rwxr-xr-x   0 jorge.imperial   (502) staff       (20)     1306 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/make_changelog.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14579 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7063 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9673 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7447 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       94 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/pyproject.toml
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1951 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1089 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      679 2023-04-19 17:18:48.000000 pyftdc-0.3.3/pyproject.toml
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       38 2023-04-19 17:19:26.630141 pyftdc-0.3.3/setup.cfg
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5492 2023-04-19 15:22:46.000000 pyftdc-0.3.3/setup.py
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.625841 pyftdc-0.3.3/src/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    13508 2023-04-11 21:35:43.000000 pyftdc-0.3.3/src/BinaryBSON.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2236 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/CSVWriter.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      354 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/ChunkMetric.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      177 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/ConstDataRangeCursor.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5987 2023-04-11 21:35:43.000000 pyftdc-0.3.3/src/Dataset.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8622 2023-04-01 15:17:09.000000 pyftdc-0.3.3/src/FTDCParser.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      351 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/FileParsedData.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1911 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/JSONWriter.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2744 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/MetricsToWTMap.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2680 2023-03-31 02:42:43.000000 pyftdc-0.3.3/src/ParserState.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       62 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/ParserTask.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2240 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/ParserTasksList.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       68 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/SampleLocation.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       65 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/WriterTask.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      643 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/WriterTaskList.cpp
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.628738 pyftdc-0.3.3/src/include/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      894 2023-04-11 21:35:43.000000 pyftdc-0.3.3/src/include/BinaryBSON.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      447 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/CSVWriter.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      813 2023-04-11 21:35:43.000000 pyftdc-0.3.3/src/include/ChunkMetric.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      633 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/ConstDataRangeCursor.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2131 2023-04-11 21:35:43.000000 pyftdc-0.3.3/src/include/Dataset.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1158 2023-04-01 15:17:09.000000 pyftdc-0.3.3/src/include/FTDCParser.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      753 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/FileParsedData.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      444 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/JSONWriter.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      271 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/Metrics.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      976 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/MetricsToWTMap.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1420 2023-03-31 02:42:43.000000 pyftdc-0.3.3/src/include/ParserState.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      593 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/ParserTask.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      625 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/ParserTasksList.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      468 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/SampleLocation.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      261 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/Timestamp.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      392 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/WriterTask.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      676 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/WriterTaskList.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1470 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/bson_value.h
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.629679 pyftdc-0.3.3/src/pyftdc.egg-info/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8130 2023-04-19 17:19:26.000000 pyftdc-0.3.3/src/pyftdc.egg-info/PKG-INFO
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9039 2023-04-19 17:19:26.000000 pyftdc-0.3.3/src/pyftdc.egg-info/SOURCES.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)        1 2023-04-19 17:19:26.000000 pyftdc-0.3.3/src/pyftdc.egg-info/dependency_links.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)        1 2023-04-19 15:22:46.000000 pyftdc-0.3.3/src/pyftdc.egg-info/not-zip-safe
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       20 2023-04-19 17:19:26.000000 pyftdc-0.3.3/src/pyftdc.egg-info/requires.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       15 2023-04-19 17:19:26.000000 pyftdc-0.3.3/src/pyftdc.egg-info/top_level.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14741 2023-04-19 15:22:46.000000 pyftdc-0.3.3/src/python.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)        6 2023-04-19 17:18:36.000000 pyftdc-0.3.3/version.txt
```

### Comparing `pyftdc-0.3.2/CMakeLists.txt` & `pyftdc-0.3.3/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 cmake_minimum_required(VERSION 3.15)
-
-set(CMAKE_OSX_DEPLOYMENT_TARGET "12.0" CACHE STRING "Minimum OS X deployment version")
-
 project(pyftdc)
 
 set(CMAKE_CXX_STANDARD 17)
 
 # Get version from file
 file(READ "version.txt" file_version)
 
@@ -13,28 +10,27 @@
 
 add_subdirectory(extern)
 add_subdirectory(pybind11)
 #add_subdirectory(Boost_tests)
 
 pybind11_add_module(${PROJECT_NAME}
         src/python.cpp
-        src/Chunk.cpp
         src/ConstDataRangeCursor.cpp
         src/Dataset.cpp
         src/FTDCParser.cpp
         src/MetricsToWTMap.cpp
-        src/ParserTasksList.cpp
         src/SampleLocation.cpp
         src/WriterTaskList.cpp
         src/ChunkMetric.cpp
         src/CSVWriter.cpp
         src/FileParsedData.cpp
         src/JSONWriter.cpp
-        src/ParserTask.cpp
         src/WriterTask.cpp
+        src/ParserState.cpp
+        src/BinaryBSON.cpp
         )
 
 target_link_libraries(${PROJECT_NAME} PRIVATE bson_static)
 
 target_include_directories(${PROJECT_NAME} PUBLIC
         ${CMAKE_BINARY_DIR}/_deps/spdlog-src/include
         ${CMAKE_SOURCE_DIR}/src/include
```

### Comparing `pyftdc-0.3.2/LICENSE` & `pyftdc-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/README.md` & `pyftdc-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/extern/CMakeLists.txt` & `pyftdc-0.3.3/extern/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 set(CMAKE_INSTALL_PREFIX "${CMAKE_BINARY_DIR}/artifacts" CACHE STRING "" FORCE)
 
 include(FetchContent)
 
 message("Fetching mongo-c-driver...")
 FetchContent_Declare(mongocdriver
         GIT_REPOSITORY  "https://github.com/mongodb/mongo-c-driver.git"
-        GIT_TAG         "1.22.1"
+        GIT_TAG         "1.23.2"
         )
 FetchContent_GetProperties(mongocdriver)
 
 if(NOT mongocdriver_POPULATED)
     set(ENABLE_MONGOC OFF CACHE BOOL "" FORCE)
     set(ENABLE_AUTOMATIC_INIT_AND_CLEANUP OFF CACHE BOOL "" FORCE)
     set(ENABLE_TESTS OFF CACHE BOOL "" FORCE)
```

### Comparing `pyftdc-0.3.2/pybind11/.appveyor.yml` & `pyftdc-0.3.3/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/.clang-format` & `pyftdc-0.3.3/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/.clang-tidy` & `pyftdc-0.3.3/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/.cmake-format.yaml` & `pyftdc-0.3.3/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/.pre-commit-config.yaml` & `pyftdc-0.3.3/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/CMakeLists.txt` & `pyftdc-0.3.3/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/LICENSE` & `pyftdc-0.3.3/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/README.rst` & `pyftdc-0.3.3/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/Doxyfile` & `pyftdc-0.3.3/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/cast/chrono.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/cast/custom.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/cast/eigen.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/cast/functional.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/cast/index.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/cast/overview.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/cast/stl.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/cast/strings.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/classes.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/embedding.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/exceptions.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/functions.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/misc.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/pycpp/numpy.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/pycpp/object.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/pycpp/utilities.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/advanced/smart_ptrs.rst` & `pyftdc-0.3.3/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/basics.rst` & `pyftdc-0.3.3/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/benchmark.py` & `pyftdc-0.3.3/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/benchmark.rst` & `pyftdc-0.3.3/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/changelog.rst` & `pyftdc-0.3.3/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/classes.rst` & `pyftdc-0.3.3/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/compiling.rst` & `pyftdc-0.3.3/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/conf.py` & `pyftdc-0.3.3/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/faq.rst` & `pyftdc-0.3.3/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/index.rst` & `pyftdc-0.3.3/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/installing.rst` & `pyftdc-0.3.3/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/limitations.rst` & `pyftdc-0.3.3/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/pybind11-logo.png` & `pyftdc-0.3.3/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/pybind11_vs_boost_python1.png` & `pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/pybind11_vs_boost_python1.svg` & `pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/pybind11_vs_boost_python2.png` & `pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/pybind11_vs_boost_python2.svg` & `pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/reference.rst` & `pyftdc-0.3.3/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/release.rst` & `pyftdc-0.3.3/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/docs/upgrade.rst` & `pyftdc-0.3.3/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/attr.h` & `pyftdc-0.3.3/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/buffer_info.h` & `pyftdc-0.3.3/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/cast.h` & `pyftdc-0.3.3/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/chrono.h` & `pyftdc-0.3.3/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/complex.h` & `pyftdc-0.3.3/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/detail/class.h` & `pyftdc-0.3.3/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/detail/common.h` & `pyftdc-0.3.3/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/detail/descr.h` & `pyftdc-0.3.3/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/detail/init.h` & `pyftdc-0.3.3/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/detail/internals.h` & `pyftdc-0.3.3/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/detail/type_caster_base.h` & `pyftdc-0.3.3/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/detail/typeid.h` & `pyftdc-0.3.3/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/eigen.h` & `pyftdc-0.3.3/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/embed.h` & `pyftdc-0.3.3/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/eval.h` & `pyftdc-0.3.3/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/functional.h` & `pyftdc-0.3.3/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/gil.h` & `pyftdc-0.3.3/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/iostream.h` & `pyftdc-0.3.3/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/numpy.h` & `pyftdc-0.3.3/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/operators.h` & `pyftdc-0.3.3/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/options.h` & `pyftdc-0.3.3/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/pybind11.h` & `pyftdc-0.3.3/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/pytypes.h` & `pyftdc-0.3.3/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/stl/filesystem.h` & `pyftdc-0.3.3/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/stl.h` & `pyftdc-0.3.3/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/include/pybind11/stl_bind.h` & `pyftdc-0.3.3/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/noxfile.py` & `pyftdc-0.3.3/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/pybind11/__main__.py` & `pyftdc-0.3.3/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/pybind11/commands.py` & `pyftdc-0.3.3/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/pybind11/setup_helpers.py` & `pyftdc-0.3.3/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/pybind11/setup_helpers.pyi` & `pyftdc-0.3.3/pybind11/pybind11/setup_helpers.pyi`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/pyproject.toml` & `pyftdc-0.3.3/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/setup.cfg` & `pyftdc-0.3.3/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/setup.py` & `pyftdc-0.3.3/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/CMakeLists.txt` & `pyftdc-0.3.3/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/conftest.py` & `pyftdc-0.3.3/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/constructor_stats.h` & `pyftdc-0.3.3/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/cross_module_gil_utils.cpp` & `pyftdc-0.3.3/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/env.py` & `pyftdc-0.3.3/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/extra_python_package/test_files.py` & `pyftdc-0.3.3/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/extra_setuptools/test_setuphelper.py` & `pyftdc-0.3.3/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/local_bindings.h` & `pyftdc-0.3.3/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/object.h` & `pyftdc-0.3.3/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/pybind11_cross_module_tests.cpp` & `pyftdc-0.3.3/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/pybind11_tests.cpp` & `pyftdc-0.3.3/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/pybind11_tests.h` & `pyftdc-0.3.3/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/pytest.ini` & `pyftdc-0.3.3/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/requirements.txt` & `pyftdc-0.3.3/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_async.cpp` & `pyftdc-0.3.3/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_async.py` & `pyftdc-0.3.3/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_buffers.cpp` & `pyftdc-0.3.3/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_buffers.py` & `pyftdc-0.3.3/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_builtin_casters.cpp` & `pyftdc-0.3.3/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_builtin_casters.py` & `pyftdc-0.3.3/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_call_policies.cpp` & `pyftdc-0.3.3/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_call_policies.py` & `pyftdc-0.3.3/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_callbacks.cpp` & `pyftdc-0.3.3/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_callbacks.py` & `pyftdc-0.3.3/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_chrono.cpp` & `pyftdc-0.3.3/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_chrono.py` & `pyftdc-0.3.3/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_class.cpp` & `pyftdc-0.3.3/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_class.py` & `pyftdc-0.3.3/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pyftdc-0.3.3/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_cmake_build/embed.cpp` & `pyftdc-0.3.3/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_const_name.cpp` & `pyftdc-0.3.3/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_const_name.py` & `pyftdc-0.3.3/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_constants_and_functions.cpp` & `pyftdc-0.3.3/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_constants_and_functions.py` & `pyftdc-0.3.3/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_copy_move.cpp` & `pyftdc-0.3.3/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_copy_move.py` & `pyftdc-0.3.3/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_custom_type_casters.cpp` & `pyftdc-0.3.3/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_custom_type_casters.py` & `pyftdc-0.3.3/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_custom_type_setup.cpp` & `pyftdc-0.3.3/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_custom_type_setup.py` & `pyftdc-0.3.3/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_docstring_options.cpp` & `pyftdc-0.3.3/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_docstring_options.py` & `pyftdc-0.3.3/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_eigen.cpp` & `pyftdc-0.3.3/pybind11/tests/test_eigen.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_eigen.py` & `pyftdc-0.3.3/pybind11/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_embed/CMakeLists.txt` & `pyftdc-0.3.3/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_embed/catch.cpp` & `pyftdc-0.3.3/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_embed/external_module.cpp` & `pyftdc-0.3.3/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_embed/test_interpreter.cpp` & `pyftdc-0.3.3/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_enum.cpp` & `pyftdc-0.3.3/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_enum.py` & `pyftdc-0.3.3/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_eval.cpp` & `pyftdc-0.3.3/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_eval.py` & `pyftdc-0.3.3/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_exceptions.cpp` & `pyftdc-0.3.3/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_exceptions.py` & `pyftdc-0.3.3/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_factory_constructors.cpp` & `pyftdc-0.3.3/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_factory_constructors.py` & `pyftdc-0.3.3/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_gil_scoped.cpp` & `pyftdc-0.3.3/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_gil_scoped.py` & `pyftdc-0.3.3/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_iostream.cpp` & `pyftdc-0.3.3/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_iostream.py` & `pyftdc-0.3.3/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_kwargs_and_defaults.cpp` & `pyftdc-0.3.3/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_kwargs_and_defaults.py` & `pyftdc-0.3.3/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_local_bindings.cpp` & `pyftdc-0.3.3/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_local_bindings.py` & `pyftdc-0.3.3/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_methods_and_attributes.cpp` & `pyftdc-0.3.3/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_methods_and_attributes.py` & `pyftdc-0.3.3/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_modules.cpp` & `pyftdc-0.3.3/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_modules.py` & `pyftdc-0.3.3/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_multiple_inheritance.cpp` & `pyftdc-0.3.3/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_multiple_inheritance.py` & `pyftdc-0.3.3/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_numpy_array.cpp` & `pyftdc-0.3.3/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_numpy_array.py` & `pyftdc-0.3.3/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_numpy_dtypes.cpp` & `pyftdc-0.3.3/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_numpy_dtypes.py` & `pyftdc-0.3.3/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_numpy_vectorize.cpp` & `pyftdc-0.3.3/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_numpy_vectorize.py` & `pyftdc-0.3.3/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_opaque_types.cpp` & `pyftdc-0.3.3/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_opaque_types.py` & `pyftdc-0.3.3/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_operator_overloading.cpp` & `pyftdc-0.3.3/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_operator_overloading.py` & `pyftdc-0.3.3/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_pickling.cpp` & `pyftdc-0.3.3/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_pickling.py` & `pyftdc-0.3.3/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_pytypes.cpp` & `pyftdc-0.3.3/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_pytypes.py` & `pyftdc-0.3.3/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_sequences_and_iterators.cpp` & `pyftdc-0.3.3/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_sequences_and_iterators.py` & `pyftdc-0.3.3/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_smart_ptr.cpp` & `pyftdc-0.3.3/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_smart_ptr.py` & `pyftdc-0.3.3/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_stl.cpp` & `pyftdc-0.3.3/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_stl.py` & `pyftdc-0.3.3/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_stl_binders.cpp` & `pyftdc-0.3.3/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_stl_binders.py` & `pyftdc-0.3.3/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_tagbased_polymorphic.cpp` & `pyftdc-0.3.3/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_tagbased_polymorphic.py` & `pyftdc-0.3.3/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_thread.cpp` & `pyftdc-0.3.3/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_thread.py` & `pyftdc-0.3.3/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_union.cpp` & `pyftdc-0.3.3/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_virtual_functions.cpp` & `pyftdc-0.3.3/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/test_virtual_functions.py` & `pyftdc-0.3.3/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/valgrind-numpy-scipy.supp` & `pyftdc-0.3.3/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tests/valgrind-python.supp` & `pyftdc-0.3.3/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tools/FindCatch.cmake` & `pyftdc-0.3.3/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tools/FindEigen3.cmake` & `pyftdc-0.3.3/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tools/FindPythonLibsNew.cmake` & `pyftdc-0.3.3/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tools/check-style.sh` & `pyftdc-0.3.3/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tools/cmake_uninstall.cmake.in` & `pyftdc-0.3.3/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tools/libsize.py` & `pyftdc-0.3.3/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tools/make_changelog.py` & `pyftdc-0.3.3/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tools/pybind11Common.cmake` & `pyftdc-0.3.3/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tools/pybind11Config.cmake.in` & `pyftdc-0.3.3/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tools/pybind11NewTools.cmake` & `pyftdc-0.3.3/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tools/pybind11Tools.cmake` & `pyftdc-0.3.3/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tools/setup_global.py.in` & `pyftdc-0.3.3/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pybind11/tools/setup_main.py.in` & `pyftdc-0.3.3/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/pyftdc.egg-info/SOURCES.txt` & `pyftdc-0.3.3/src/pyftdc.egg-info/SOURCES.txt`

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

### Comparing `pyftdc-0.3.2/pyproject.toml` & `pyftdc-0.3.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -4,29 +4,29 @@
     "wheel",
     "ninja",
     "pybind11>=2.8.0",
     "cmake>=3.21",
     "scikit-build>=0.12",
 ]
 build-backend = "setuptools.build_meta"
-
+ 
 
 # Project
 [project]
 name = "pyftdc"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
     { name="Jorge Imperial", email="jlimperial@protonmail.com" },
 ]
-description = "A MongoDB FTDC files parser written in C++ that provides Python bindings using [pybind11](https://github.com/pybind/pybind11) and scikit-build."
+description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/jimper/mongo_ftdc"
-"Bug Tracker" = "https://gitlab.com/jimper/issues"
+"Bug Tracker" = "https://gitlab.com/jimper/issues"
```

### Comparing `pyftdc-0.3.2/setup.py` & `pyftdc-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,9 +130,9 @@
     author_email="jorgeluis.imperial@gmail.com",
     long_description="",
 
     ext_modules=[CMakeExtension("pyftdc")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     extras_require={"test": ["pytest>=6.0"]},
-    python_requires=">=3.6",
+    python_requires=">=3.8",
 )
```

### Comparing `pyftdc-0.3.2/src/CSVWriter.cpp` & `pyftdc-0.3.3/src/CSVWriter.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     size_t i = 0;
     for (auto t : *ts)
         csvTasks.setTimestamp(i++, t);
 
 
     // Write metric names in first row
     std::vector<std::string> metricNames ;
-    auto n = pDataset->getMetricsNames(metricNames);
+    auto n = pDataset->getMetricsNames();
     csvFileStream << "#line,";
     for (size_t i=0;i<metricNames.size();++i)
         csvFileStream << "\"" << metricNames[i] << "\",";
     spdlog::debug("WriterTasks: From {} to {}. Metrics size {}", start, end, ts->size());
     /*
     // Thread pool
     size_t numThreads = boost::thread::hardware_concurrency() - 1;
```

### Comparing `pyftdc-0.3.2/src/Chunk.cpp` & `pyftdc-0.3.3/src/BinaryBSON.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,151 +1,135 @@
 //
-// Created by jorge on 11/14/20.
+// Created by Jorge Imperial-Sosa on 3/22/23.
 //
-
-#include "Chunk.h"
-
-// Zlib decompressor
 #include <zlib.h>
-#include <bson.h>
+#include "BinaryBSON.h"
+#include "ConstDataRangeCursor.h"
+#include "spdlog/spdlog.h"
+#include "ParserState.h"
+#include "bson/bson.h"
+#include <vector>
 #include <sstream>
-#include <map>
-#include <spdlog/spdlog.h>
 
-#include "ChunkMetric.h"
-#include "ConstDataRangeCursor.h"
+uint64_t unpack(ConstDataRangeCursor *cdc) ;
+std::string fullname (const char *key, std::vector<std::string> & docs) ;
 
-static
-void
-write_log(const std::vector<std::string>  pref, const char *key, const bson_t *document) {
-#if DEBUG_VISIT
-    size_t documentLength = 0;
-    char *str = bson_as_canonical_extended_json (document, &documentLength);
-    BOOST_LOG_TRIVIAL(info) << "LOG-JSON " << key << " " << str;
-    bson_free (str);
-#endif
-}
 
-Chunk::Chunk (const uint8_t *data, size_t size, int64_t id=-1) : deltasInChunk(0), metricsInChunk(0) {
-    compressed = new uint8_t[size];
-    compressed_size = size;
-
-    this->id = id;  //TODO: Why divide by 1000 ?
-
-    // We know where this chunk starts, but not where it ends
-    this->start = id;
-    this->end = INVALID_TIMESTAMP;
 
-    if (!memcpy(compressed, data, size)) {
-        spdlog::critical( "Could not allocate {}  bytes while parsing chunkVector.", size);
+uint64_t
+unpack(ConstDataRangeCursor *cdc) {
+    uint64_t i = 0;
+    uint8_t b;
+    uint s = 0;
 
+    while(true) {
+        b   = cdc->ReadByte();
+        i |= uint64_t(b & 0x7f) << s;
+        s += 7;
+        if ((b & 0x80) == 0) {
+            return i;
+        }
     }
 }
 
-size_t
-Chunk::getMetricNames(std::vector<std::string> & metricNames) {
-
-    for (auto &m : metrics) {
-        metricNames.emplace_back(m->getName());
-    }
-    return metricNames.size();
-}
 
 std::string
 fullname (const char *key, std::vector<std::string> & docs) {
     std::ostringstream s;
     for (auto & doc : docs)
         s << doc << ".";
 
     s << key;
     return s.str();
 }
 
+
 //
 // From StackOverflow https://stackoverflow.com/questions/4901842/in-memory-decompression-with-zlib
 //
+
 int
-Chunk::inflate(const void *src, int srcLen, void *dst, int dstLen) {
+BinaryBSON::unCompress() { // const void *src, int srcLen, void *dst, int dstLen) {
+
+    auto src = static_cast<void *>(blob.data()+4);
+    auto srcLen = blob.size();
+    auto buffer = new char[BIN_BSON_MAX_SIZE];
+    auto dst = static_cast<void*>(buffer);
+    int dstLen = BIN_BSON_MAX_SIZE;
+
     z_stream strm = {nullptr};
     strm.total_in = strm.avail_in = srcLen;
     strm.total_out = strm.avail_out = dstLen;
     strm.next_in = (Bytef *) src;
     strm.next_out = (Bytef *) dst;
 
     strm.zalloc = Z_NULL;
     strm.zfree = Z_NULL;
     strm.opaque = Z_NULL;
 
     int err;
     int ret = -1;
 
+    // Returned errors from zlib
+    // Z_OK            0
+    // Z_STREAM_END    1
+    // Z_NEED_DICT     2
+    // Z_ERRNO        (-1)
+    // Z_STREAM_ERROR (-2)
+    // Z_DATA_ERROR   (-3)
+    // Z_MEM_ERROR    (-4)
+    // Z_BUF_ERROR    (-5)
+    // Z_VERSION_ERROR (-6)
+
     err = inflateInit2(&strm, (15 + 32)); //15 window bits, and the +32 tells zlib to to detect if using gzip or zlib
     if (err == Z_OK) {
         err = ::inflate(&strm, Z_FINISH);
         if (err == Z_STREAM_END) {
             ret = strm.total_out;
         } else {
             inflateEnd(&strm);
             return err;
         }
     } else {
         inflateEnd(&strm);
         return err;
     }
+    auto x = inflateEnd(&strm);
+    // Copy to uncompressed structure.
+    uncompressed.reserve(ret);
+    uncompressed.assign(buffer, buffer+strm.total_out);
 
-    inflateEnd(&strm);
-    return ret;
-}
+    std::destroy(blob.begin(), blob.end());
 
-uint64_t
-unpack(ConstDataRangeCursor *cdc) {
-    uint64_t i = 0;
-    uint8_t b;
-    uint s = 0;
-
-    while(true) {
-        b   = cdc->ReadByte();
-        i |= uint64_t(b & 0x7f) << s;
-        s += 7;
-        if ((b & 0x80) == 0) {
-            return i;
-        }
-    }
+    return Z_OK;
 }
 
 int
-Chunk::ReadVariableSizedInts() {
+BinaryBSON::UnpackVariableInts() {
     int count = 0;
 
-    const uint8_t *p = this->decompressed; // data;
-    auto docSize = *(uint32_t*) this->decompressed;
-
-    auto metricsSize = metrics.size();
-    if (metricsSize != metricsInChunk) {
-        spdlog::debug(  "Different metrics counts in chunk {} != {}",  metrics.size(), metricsInChunk);
-        //return -1;
-    }
-
+    const uint8_t *p = uncompressed.data();
+    auto docSize = *(uint32_t*) uncompressed.data();
     auto offset = docSize + 8;
     const uint8_t *q = p +  offset;
 
-    auto dataRangeSize = this->decompressed_size-offset;
+    auto dataRangeSize = uncompressed.size()-offset;
 
     //if (dataRangeSize <= 0) return 0;
 
     ConstDataRangeCursor dataRangeCursor(q,dataRangeSize);
 
     uint64_t nZeroes = 0;
 
     for (int m=0; m < metrics.size(); ++m) {
 
         auto values = metrics[m]->getValues(); //
         auto value = values[0];
 
-        for (int s = 0; s < deltasInChunk; ++s) {
+        for (int s = 0; s < deltaCountFromHeader; ++s) {
 
             uint64_t delta;
 
             if (nZeroes!=0) {
                 delta = 0;
                 --nZeroes;
             } else {
@@ -153,39 +137,53 @@
                 if (delta == 0) {
                     nZeroes = unpack(&dataRangeCursor);
                 }
             }
             value += delta;
             values[s + 1] = value;
         }
-        metrics[m]->setSampleCount(deltasInChunk);
+        metrics[m]->setSampleCount(deltaCountFromHeader);
     }
     return count;
 }
 
-int
-Chunk::Decompress() {
-    decompressed = new uint8_t[CHUNK_MAX_SIZE];
-    decompressed_size = inflate(compressed+4, compressed_size, decompressed, CHUNK_MAX_SIZE);
-    return decompressed_size;
+static
+void
+write_log(const std::vector<std::string>  pref, const char *key, const bson_t *document) {
+#if DEBUG_VISIT
+    size_t documentLength = 0;
+    char *str = bson_as_canonical_extended_json (document, &documentLength);
+    BOOST_LOG_TRIVIAL(info) << "LOG-JSON " << key << " " << str;
+    bson_free (str);
+#endif
 }
 
 typedef struct {
     int visited;
+
     bson_visitor_t *visit_table;
     std::vector<std::string> name_stack;
     std::vector<ChunkMetric *> *metrics;
     bool logNames;
+
+    bson_type_metrics_t bson_type_metrics[MAX_METRICS];
 } visitResults;
 
 static bool
 visit_before (const bson_iter_t *iter, const char *key, void *data)
 {
     auto *v = (visitResults *) data;
     v->visited++;
+
+    auto btype = bson_iter_type (iter);
+    ++v->bson_type_metrics[btype].count;
+    if (btype > 15) {
+        spdlog::debug("Type {}: key: {}", btype, key);
+    }
+
     return false;// returning true stops further iteration of the document
 }
 
 static bool
 visit_array(const bson_iter_t *, const char *key, const bson_t *v_array, void *data) {
     auto *v = (visitResults *) data;
 
@@ -200,39 +198,38 @@
 
 static bool
 visit_document(const bson_iter_t *, const char *key, const bson_t *v_document, void *data){
     auto *v = (visitResults *) data;
     bson_iter_t child;
     if (bson_iter_init(&child, v_document)) {
 
-        ::write_log(v->name_stack, key, v_document);
-
+        //::write_log(v->name_stack, key, v_document);
         v->name_stack.emplace_back(key);
         ::bson_iter_visit_all(&child, v->visit_table, data);
         v->name_stack.pop_back();
     }
     return false;
 }
 
 static bool
 visit_int32(const bson_iter_t *, const char *key, int32_t v_int32, void *data) {
     auto *v = (visitResults *) data;
     v->metrics->emplace_back( new ChunkMetric(fullname(key, v->name_stack),  BSON_TYPE_INT32, v_int32));
 
     if (v->logNames)
-       spdlog::debug("Metric: {} = {}", fullname(key, v->name_stack), v_int32);
+        spdlog::debug("Metric: {} = {}", fullname(key, v->name_stack), v_int32);
     return false;
 }
 
 static bool
 visit_int64(const bson_iter_t *, const char *key, int64_t v_int64, void *data) {
     auto *v = (visitResults *) data;
     v->metrics->emplace_back( new ChunkMetric(fullname(key, v->name_stack),  BSON_TYPE_INT64, v_int64));
     if (v->logNames)
-       spdlog::debug("Metric: {} = {}", fullname(key, v->name_stack), v_int64);
+        spdlog::debug("Metric: {} = {}", fullname(key, v->name_stack), v_int64);
     return false;
 }
 
 static bool
 visit_bool(const bson_iter_t *, const char *key, bool v_bool, void *data) {
     auto *v = (visitResults *) data;
     v->metrics->emplace_back( new ChunkMetric(fullname(key, v->name_stack),  BSON_TYPE_BOOL, v_bool));
@@ -299,209 +296,136 @@
 
 static bool
 visit_binary(const bson_iter_t *, const char *key, bson_subtype_t subtype, size_t , const uint8_t *, void *data){
     spdlog::error("Discarding binary {}", key);
     return false;
 }
 
-int
-Chunk::ConstructMetrics(const uint8_t* data ) {
 
+int
+BinaryBSON::parseUncompressedBinary() {
+    const uint8_t* data = uncompressed.data();
     bson_iter_t iter;
     auto *dataSize = (int32_t*) data;
 
     // Keys are variable between chunks and so are deltas.
     // Assume makes an ass of u and me.
     auto pp = data+(*dataSize);
-    metricsInChunk = *(uint32_t*)pp;
-    deltasInChunk = *(uint32_t*)(pp + 4);
+    metricCountFromHeader = *(uint32_t*)pp;
+    deltaCountFromHeader = *(uint32_t*)(pp + 4);
+
+    if (deltaCountFromHeader!=299) {
+        spdlog::debug("Deltas count is not default {}, it is {}.",
+                      ChunkMetric::MAX_SAMPLES-1,
+                      deltaCountFromHeader);
+        //deltaCountFromHeader = ChunkMetric::MAX_SAMPLES-1;
+    }
+    //spdlog::set_level(spdlog::level::debug);
 
     // This is the number of structures needed
-    spdlog::debug( "Metrics in chunk to reserve: {}", metricsInChunk);
-    metrics.reserve(metricsInChunk);
+    spdlog::debug("Reserve space for {} metrics.", metricCountFromHeader);
+    metrics.reserve(metricCountFromHeader);
 
+    bson_t *bsonStruct;
     if ((bsonStruct = bson_new_from_data (data, (size_t)(*dataSize)))) {
         if (bson_iter_init (&iter, bsonStruct)) {
 
             bson_visitor_t vt{};
             visitResults results{};
+            for (int i=0;i<MAX_METRICS;++i) results.bson_type_metrics[i].count = 0;
 
-            vt.visit_before = visit_before;
-            vt.visit_array = visit_array;
-            vt.visit_document = visit_document;
-            vt.visit_int32 = visit_int32;
-            vt.visit_int64 = visit_int64;
-            vt.visit_bool = visit_bool;
-            vt.visit_double = visit_double;
+            results.bson_type_metrics[BSON_TYPE_EOD] = {0, "End of document"};
+            results.bson_type_metrics[BSON_TYPE_DOUBLE] = {0, "Floating point"};
+            results.bson_type_metrics[BSON_TYPE_UTF8] = {0, "UTF-8 string"};
+            results.bson_type_metrics[BSON_TYPE_DOCUMENT] = {0, "Embedded document"};
+            results.bson_type_metrics[BSON_TYPE_ARRAY] = {0, "Array"};
+            results.bson_type_metrics[BSON_TYPE_BINARY] = {0, "Binary"};
+            results.bson_type_metrics[BSON_TYPE_UNDEFINED] = {0, "Undefined"};
+            results.bson_type_metrics[BSON_TYPE_OID] = {0, "Object ID"};
+            results.bson_type_metrics[BSON_TYPE_BOOL] = {0, "Boolean"};
+            results.bson_type_metrics[BSON_TYPE_DATE_TIME] = {0, "Datetime"};
+            results.bson_type_metrics[BSON_TYPE_NULL] = {0, "Null"};
+            results.bson_type_metrics[BSON_TYPE_REGEX] = {0, "Regexp"};
+            results.bson_type_metrics[BSON_TYPE_DBPOINTER] = {0, "DB Pointer"};
+            results.bson_type_metrics[BSON_TYPE_CODE] = {0, "Code"};
+            results.bson_type_metrics[BSON_TYPE_SYMBOL] = {0, "Symbol"};
+            results.bson_type_metrics[BSON_TYPE_CODEWSCOPE] = {0, "JavaScript code w/ scope"};
+            results.bson_type_metrics[BSON_TYPE_INT32] = {0, "32-bit Integer"};
+            results.bson_type_metrics[BSON_TYPE_TIMESTAMP] = {0, "Timestamp"};
+            results.bson_type_metrics[BSON_TYPE_INT64] = {0, "64-bit Integer"};
+            results.bson_type_metrics[BSON_TYPE_DECIMAL128] = {0, "Decimal 128"};
+            results.bson_type_metrics[BSON_TYPE_MAXKEY] = {0, "Max Key"};
+            results.bson_type_metrics[BSON_TYPE_MINKEY] = {0, "Min Key"};
+
+            vt.visit_before    = visit_before;
+            vt.visit_array     = visit_array;
+            vt.visit_document  = visit_document;
+            vt.visit_int32     = visit_int32;
+            vt.visit_int64     = visit_int64;
+            vt.visit_bool      = visit_bool;
+            vt.visit_double    = visit_double;
             vt.visit_date_time = visit_date_time;
             vt.visit_timestamp = visit_timestamp;
 
-            vt.visit_oid = visit_oid;
-            vt.visit_binary = visit_binary;
-            vt.visit_null = visit_null;
+            vt.visit_oid       = visit_oid;
+            vt.visit_binary    = visit_binary;
+            vt.visit_null      = visit_null;
 
             // Only for display
-            vt.visit_utf8 = visit_utf8;
-
-            //results.logNames = true;
-            //spdlog::set_level(spdlog::level::debug);
+            vt.visit_utf8      = visit_utf8;
 
             results.visit_table = &vt;
             results.metrics = &metrics;
 
             ::bson_iter_visit_all(&iter, &vt, &results);
 
             spdlog::debug("Visited: {} Metrics: {}", results.visited, results.metrics->size());
-            if (metricsInChunk != metrics.size())
-                spdlog::debug("Different metric names counts: {} != {}", results.metrics->size(), metricsInChunk);
+            if (metricCountFromHeader != metrics.size())
+                spdlog::debug("Metrics visited {} are different than header {}.", results.metrics->size(), metricCountFromHeader);
+            // Get values of metrics from deltas+.
+            UnpackVariableInts();
+
+            return (int) metrics.size();
+        }
+        else {
+            spdlog::error("Could not initialize BSON iterator. Not parsing.");
+            return -1;
         }
     }
-
-    // Get actual values
-    ReadVariableSizedInts();
-    setTimestampLimits();
-
-    return metrics.size();
-}
-
-void
-Chunk::setTimestampLimits() {
-    start = metrics[0]->getValue(0);
-    end = metrics[0]->getValue( getSamplesCount()-1);
-}
-
-bool Chunk::Consume() {
-
-    if (Decompress() > 0) {
-        auto data = getUncompressedData();
-
-        // We construct the metrics. These are name and first value only since deltasInChunk have not been read.
-        ConstructMetrics(data);
-
-        // Get actual values
-        ReadVariableSizedInts();
-        setTimestampLimits();
-        return true;
+    else {
+        spdlog::error("Could not convert unzipped blob to bson.");
+        return -2;
     }
-    else
-        return false;
 }
 
 
 
-typedef struct {
-
-    bson_t *parent;
-    bson_t *doc;
-    std::string name;
-} SubDocs;
-
-std::string
-Chunk::getJsonAtPosition(size_t position) {
-
-    bson_iter_t iter;
-    bson_iter_t baz;
-
-    bson_t* newBson = bson_copy(bsonStruct);
-
-    if (bson_iter_init (&iter, newBson)) {
-
-        for (int i=0;i<metrics.size(); ++i) {
-            if (bson_iter_find_descendant(&iter, metrics[i]->getName().c_str(), &baz)) {
+std::vector<std::string>
+BinaryBSON::getMetricsNames() {
 
-                auto t = bson_iter_type(&baz);
-
-                switch (t) {
-                    case BSON_TYPE_INT64:
-                        bson_iter_overwrite_int64(&baz, metrics[i]->getValue(position));
-                        break;
-                    case BSON_TYPE_INT32:
-                        bson_iter_overwrite_int32(&baz, metrics[i]->getValue( position ));
-                        break;
-                    case BSON_TYPE_DATE_TIME:
-                        bson_iter_overwrite_date_time(&baz, metrics[i]->getValue( position));
-                        break;
-                    case BSON_TYPE_DOUBLE:
-                        bson_iter_overwrite_double(&baz, metrics[i]->getValue( position));
-                        break;
-                    case BSON_TYPE_BOOL:
-                        bson_iter_overwrite_bool(&baz, metrics[i]->getValue( position));
-                        break;
-                    case BSON_TYPE_UTF8:
-                    case  BSON_TYPE_EOD:
-                    case BSON_TYPE_DOCUMENT:
-                    case BSON_TYPE_ARRAY:
-                    case BSON_TYPE_DECIMAL128:
-                    case BSON_TYPE_MAXKEY:
-                    case BSON_TYPE_MINKEY :
-                    case BSON_TYPE_BINARY:
-                    case BSON_TYPE_UNDEFINED:
-                    case BSON_TYPE_OID:
-                    case BSON_TYPE_NULL:
-                    case BSON_TYPE_REGEX:
-                    case BSON_TYPE_TIMESTAMP:
-                    case BSON_TYPE_DBPOINTER:
-
-                    default:
-                        break;
-                }
-            }
-        }
+    auto metricList = new std::vector<std::string>();
+    for (auto m : metrics) {
+        metricList->emplace_back(m->getName());
     }
-    auto jsonStr = bson_as_json(newBson, NULL);
-    std::string ret = std::string(jsonStr);
-    bson_free(jsonStr);
-    bson_destroy(newBson);
-
-    return ret;
-
+    return *metricList;
 }
 
+ChunkMetric *
+BinaryBSON::getMetric(std::string name) {
 
-std::string
-Chunk::getJsonFromTimestamp(Timestamp ts) {
-
-    for (size_t i=0;i<metrics.size(); ++i) {
-        if (metrics[0]->getValue(i) == ts) {
-            return getJsonAtPosition(i);
-        }
-    }
-
-    return "{}";
-}
-
-std::string
-Chunk::getCsvAtPosition(size_t pos) {
+    for(auto m : metrics)
+        if (name == m->getName())
+            return m;
 
-    std::string ret;
-    for (auto m : metrics) {
-        ret += std::to_string(m->getValue(pos));
-        ret += ",";
-    }
-    return ret;
+    return nullptr;
 }
 
-size_t Chunk::getRawValuesAtPosition(uint64_t *values, size_t pos) {
-    size_t count = 0;
-    for (auto m : metrics)
-        values[count++] = m->getValue(pos);
-
-    return count;
+ChunkMetric *
+BinaryBSON::getMetric(unsigned int index) {
+    return metrics[index];
 }
 
-int Chunk::AddMetric(std::string metricName, std::vector<uint64_t> *data)   {
-    ChunkMetric *chunkMetric = new ChunkMetric(metricName);
-
-    auto metricValues = chunkMetric->getValues();
-
-    assert(data->size() <= ChunkMetric::MAX_SAMPLES);
-
-    for (auto & v : *data) *metricValues++ = v;
-    chunkMetric->setSampleCount(data->size());
-
-    metrics.emplace_back(chunkMetric);
-
-    ++metricsInChunk;
-
-    return 0;
+size_t
+BinaryBSON::getSampleCount() const {
+    return 1+deltaCountFromHeader;
 }
```

### Comparing `pyftdc-0.3.2/src/JSONWriter.cpp` & `pyftdc-0.3.3/src/JSONWriter.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/MetricsToWTMap.cpp` & `pyftdc-0.3.3/src/MetricsToWTMap.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/ParserTasksList.cpp` & `pyftdc-0.3.3/src/ParserTasksList.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/WriterTaskList.cpp` & `pyftdc-0.3.3/src/WriterTaskList.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/include/ChunkMetric.h` & `pyftdc-0.3.3/src/include/ChunkMetric.h`

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

### Comparing `pyftdc-0.3.2/src/include/ConstDataRangeCursor.h` & `pyftdc-0.3.3/src/include/ConstDataRangeCursor.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/include/Dataset.h` & `pyftdc-0.3.3/src/include/Dataset.h`

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

### Comparing `pyftdc-0.3.2/src/include/MetricsToWTMap.h` & `pyftdc-0.3.3/src/include/MetricsToWTMap.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/include/ParserTask.h` & `pyftdc-0.3.3/src/include/ParserTask.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/include/ParserTasksList.h` & `pyftdc-0.3.3/src/include/ParserTasksList.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/include/WriterTaskList.h` & `pyftdc-0.3.3/src/include/WriterTaskList.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/include/bson_value.h` & `pyftdc-0.3.3/src/include/bson_value.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.2/src/pyftdc.egg-info/PKG-INFO` & `pyftdc-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pyftdc
-Version: 0.3.1
+Version: 0.3.3
 Summary: A small example package
 Author: Jorge Imperial
 Author-email: Jorge Imperial <jlimperial@protonmail.com>
 Project-URL: Homepage, https://gitlab.com/jimper/mongo_ftdc
 Project-URL: Bug Tracker, https://gitlab.com/jimper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 pyftdc
 ==============
```

### Comparing `pyftdc-0.3.2/src/python.cpp` & `pyftdc-0.3.3/src/python.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,308 +1,320 @@
 #include <pybind11/pybind11.h>
 #include <pybind11/stl_bind.h>
 #include <pybind11/stl.h>
 #include <pybind11/numpy.h>
 
 #include "FTDCParser.h"
+#include <utility>
 #include <vector>
 #include <filesystem>
 
-
 namespace py = pybind11;
 
 using namespace py::literals;
 using namespace ftdcparser;
 namespace fs = std::filesystem;
 
 typedef std::vector<std::string> MetricNames;
 
 
 #define FALSE 0
 
 #define STRINGIFY(x) #x
 #define MACRO_STRINGIFY(x) STRINGIFY(x)
 
-//TODO: Check for memory leaks.
-
+//std::vector<uint64_t> *emptyArray;
 
+//TODO: Check for memory leaks.
 
 // helper function to avoid making a copy when returning a py::array_t
 // author: https://github.com/YannickJadoul
 // source: https://github.com/pybind/pybind11/issues/1042#issuecomment-642215028
 template <typename Sequence>
+
+[[maybe_unused]]
 inline py::array_t<typename Sequence::value_type>
 as_pyarray(Sequence &&seq) {
     auto size = seq.size();
     auto data = seq.data();
-    std::unique_ptr<Sequence> seq_ptr = std::make_unique<Sequence>(std::move(seq));
+    std::unique_ptr<Sequence> seq_ptr = std::make_unique<Sequence>(std::forward<Sequence>(seq));
     auto capsule = py::capsule(seq_ptr.get(), [](void *p) { std::unique_ptr<Sequence>(reinterpret_cast<Sequence*>(p)); });
     seq_ptr.release();
     return py::array(size, data, capsule);
 }
 
+
 inline py::array_t<uint64_t >
 as_pyarray(MetricsPtr m) {
     auto size = m->size();
     auto data = m->data();
     std::unique_ptr<MetricsPtr> seq_ptr = std::make_unique<MetricsPtr>(std::move(m));
     auto capsule = py::capsule(seq_ptr.get(),
                                [](void *p) { std::unique_ptr<Metrics>(reinterpret_cast<Metrics *>(p)); });
     seq_ptr.release();
     return py::array(size, data, capsule);
 }
 
+
+
+/** @brief Helper function that returns a vector of given size and type
+ *
+ * @tparam T The type of element
+ * @param size The size of the vector to return
+ * @returns a vector of given size and type
+ */
+template <typename T> std::vector<T>
+make_vector(std::size_t size) {
+    std::vector<T> v(size, 0);
+    std::iota(v.begin(), v.end(), 0);
+    return v;
+}
+
 //-----------------------------------------------------------------------------------
 // DatasetClass
 
 struct DatasetClass {
-    Dataset *dataSet;
+    Dataset *dataSet{};
     std::string filePath;
     std::string file;
     std::string metadata;
     MetricNames metricsNames;
-    bool interim;
+    bool interim{};
     std::vector<MetricsPtr> dataSetMetrics;
 
-    DatasetClass() {
-    }
+    DatasetClass() = default;
 
-    explicit DatasetClass(Dataset *ds, std::string path) {
+    explicit DatasetClass(Dataset *ds, const std::string& path) {
         dataSet = ds;
         filePath = path;
         file = fs::path(path).filename();
-        metricsNames = dataSet->getMetricsNames();
+        metricsNames = *dataSet->getMetricsNames();
         metadata = dataSet->getMetadata();
         if (file == "metrics.interim")
             interim = true;
         else {
             interim = false;
         }
     };
 
+    [[nodiscard]]
     MetricsPtr
-    getMetric(std::string metric_name,
-                          size_t start = INVALID_TIMESTAMP, size_t end =INVALID_TIMESTAMP,
-                          bool rated_metric = false) {
-
-        auto m = dataSet->getMetric(metric_name, start, end, rated_metric);
-        if (!m) {
-            auto *mp = new MetricsPtr();
-            return *mp;
-        }
-        else
-            return m;
-    }
-
-    std::vector<MetricsPtr>
-    getMetricsList(std::vector<std::string> metric_names,
-              size_t start = INVALID_TIMESTAMP, size_t end =INVALID_TIMESTAMP,
-              bool rated_metric = false) {
-
-        std::vector<MetricsPtr> metricList;
-        for (auto &name : metric_names) {
-            auto m = this->getMetric(name, start, end, rated_metric);
-            metricList.emplace_back(m);
-        }
-        return metricList;
+    getMetric(std::string &metric_name,
+                          size_t start = INVALID_TIMESTAMP, size_t end = INVALID_TIMESTAMP,
+                          bool rated_metric = false) const  {
+        return dataSet->getMetric(metric_name, start, end, rated_metric);
     }
 
 
+    [[nodiscard]]
     py::array_t<unsigned long>
-    getMetricAsNumpyArray(std::string metric_name,
+    getMetricAsNumpyArray(std::string &metric_name,
                           size_t start = INVALID_TIMESTAMP,
                           size_t end = INVALID_TIMESTAMP,
-                          bool rated_metric = false) {
+                          bool rated_metric = false) const {
         auto m = getMetric(metric_name, start, end, rated_metric);
 
-        if (m) return as_pyarray(m);
+        if (m) {
+            return as_pyarray(m);
+        }
         else {
-            auto  *empty = new py::array_t<unsigned long>;
-            return *empty;
+            return as_pyarray( make_vector<uint64_t >(0));
         }
     }
 
+    [[nodiscard]]
     std::vector<py::array_t<unsigned long>>
-    getMetricListAsNumpyArray(std::vector<std::string> metric_names,
+    getMetricListAsNumpyArray(std::vector<std::string>& metric_names,
                               size_t start = INVALID_TIMESTAMP,
                               size_t end = INVALID_TIMESTAMP,
-                              bool rated_metric = false) {
+                              bool rated_metric = false) const {
 
         std::vector<py::array_t<unsigned long>> metricList;
         for (auto &name : metric_names) {
             auto m = this->getMetricAsNumpyArray(name, start, end, rated_metric);
             metricList.emplace_back(m);
         }
+
         return metricList;
     }
 };
 
 //-----------------------------------------------------------------------------------
 //
 
 struct ParserClass {
     FTDCParser *pParser;
     Dataset *dataSet = nullptr;
     std::string metadata;
     std::vector<std::string> fileList;
     MetricNames metricNames;
 
-    MetricsPtr emptyMetrics;
+    MetricsPtr emptyMetrics{};
 
     explicit ParserClass() {
         pParser = new FTDCParser();
     };
 
-    DatasetClass *parseFile(std::string file, bool only_metadata=false, bool only_metrics_names=false, bool lazy=false) {
+    std::variant<DatasetClass *, bool>
+    parseFile(const std::string& file) {
         if (dataSet != nullptr) {
             delete dataSet;
             dataSet = nullptr;
         }
-        dataSet = pParser->parseFile(file, only_metadata, only_metrics_names, false);
+        dataSet = pParser->parseFile(file);
         if (dataSet) {
             // Timestamps, metric names, and metadata as fields in python
-            metricNames = dataSet->getMetricsNames();
+            metricNames = *dataSet->getMetricsNames();
             metadata = dataSet->getMetadata();
+            return new DatasetClass(dataSet, file);
+        }
+        else {
+            return false;
         }
-        return new DatasetClass(dataSet, file);
     }
 
-    void setVerbose(bool verbose) {
+    void
+    setVerbose(bool verbose) const {
         pParser->setVerbose(verbose);
     }
 
+    [[nodiscard]]
     std::vector<DatasetClass*>
-    parseDir(std::string dir, bool only_metadata=false, bool only_metrics_names=false, bool lazy=false) {
-
+    parseDir(const std::string& dir) const {
 
-        std::vector<DatasetClass*> *r = new std::vector<DatasetClass*>;
+        auto *r = new std::vector<DatasetClass*>;
         for (const auto &entry : fs::directory_iterator(dir)) {
             if (entry.is_regular_file()) {
 
-                //printf("******** parsing %s\n", entry.path().c_str());
-                auto ds = pParser->parseFile(entry.path(),
-                                             only_metadata, only_metrics_names, false);
+                auto ds = pParser->parseFile(entry.path());
                 if (ds) {
-                    DatasetClass *dsc = new DatasetClass(ds, entry.path());
+                    auto *dsc = new DatasetClass(ds, entry.path());
                     r->emplace_back(dsc);
                 }
             }
         }
-
         return *r;
     }
 
-    int dumpFileAsJson(std::string input, std::string output) {
+    [[nodiscard]]
+    size_t
+    dumpFileAsJson(std::string &input, std::string &output) const {
         return pParser->dumpDocsAsJsonTimestamps(input, output, INVALID_TIMESTAMP, INVALID_TIMESTAMP);
     }
 
-    int dumpFileAsCsv(std::string input, std::string output) {
+    [[nodiscard]]
+    size_t
+    dumpFileAsCsv(std::string &input, std::string &output) const {
         return pParser->dumpDocsAsCsvTimestamps(input, output, INVALID_TIMESTAMP, INVALID_TIMESTAMP);
     }
 
-    py::list
-    getParsedFileInfo() {
+    [[nodiscard]] py::list
+    getParsedFileInfo() const {
         auto fi = dataSet->getParsedFileInfo();
         py::list parsedFiles;
-        for (auto f : fi) {
-            auto fileInfo = py::dict("abs_path"_a=f->getFileAbsolute(),
-                                     "samples"_a=f->getSamplesCount(),
-                                     "start"_a=f->getStart(),
-                                     "end"_a=f->getEnd()
-            );
-            parsedFiles.append(fileInfo);
-        }
+
+        auto fileInfo = py::dict("abs_path"_a=fi->getFileAbsolute(),
+                                 "samples"_a=fi->getSamplesCount(),
+                                 "start"_a=fi->getStart(),
+                                 "end"_a=fi->getEnd()
+        );
+        parsedFiles.append(fileInfo);
+
         return parsedFiles;
     }
 
+    [[nodiscard]]
     MetricsPtr
-    get_timestamps(size_t start =INVALID_TIMESTAMP, size_t end = INVALID_TIMESTAMP) {
+    get_timestamps(size_t start =INVALID_TIMESTAMP, size_t end = INVALID_TIMESTAMP) const {
         return dataSet->getMetric( "start", start, end);
     }
 
+    [[nodiscard]]
     MetricsPtr
     getMetric(std::string metric_name,
                           size_t start = INVALID_TIMESTAMP, size_t end =INVALID_TIMESTAMP,
-                          bool rated_metric = false) {
-        return dataSet->getMetric(metric_name, start, end, rated_metric);
+                          bool rated_metric = false) const {
+        return dataSet->getMetric(std::move(metric_name), start, end, rated_metric);
     }
 
     std::vector<MetricsPtr>
-    getMetricList(const std::vector<std::string> metric_names,
+    getMetricList(const std::vector<std::string>& metric_names,
                                           size_t start = INVALID_TIMESTAMP,
                                           size_t end = INVALID_TIMESTAMP,
                                           bool rated_metric = false) {
 
-        auto m = dataSet->getMetrics(metric_names, start, end, rated_metric);
+        auto metricPtrList = dataSet->getMetrics(metric_names, start, end, rated_metric);
 
         std::vector<MetricsPtr> metricList;
-        for(size_t i=0;i<m.size();++i) {
+        for(auto & m : metricPtrList) {
 
             // How to handle metric names that are not found?
-            if (m[i] != nullptr) {
-
-                metricList.emplace_back(m[i]);
-            }
+            if (m != nullptr)
+                metricList.emplace_back(m);
             else
                 metricList.emplace_back(emptyMetrics);
         }
         return metricList;
     }
 
 
+    [[nodiscard]]
     py::array_t<unsigned long>
     getMetricAsNumpyArray(std::string metric_name,
                           size_t start = INVALID_TIMESTAMP,
                           size_t end = INVALID_TIMESTAMP,
-                          bool rated_metric = false) {
-        auto m = dataSet->getMetric(metric_name, start, end, rated_metric);
+                          bool rated_metric = false) const {
+        auto m = dataSet->getMetric(std::move(metric_name), start, end, rated_metric);
         return as_pyarray(m);
     }
 
+    /**
+    [[nodiscard]]
     std::vector<py::array_t<unsigned long>>
     getMetricListAsNumpyArray(std::vector<std::string> metric_names,
             size_t start = INVALID_TIMESTAMP,
             size_t end = INVALID_TIMESTAMP,
-            bool rated_metric = false) {
+            bool rated_metric = false) const {
 
-        auto m = dataSet->getMetrics(metric_names, start, end, rated_metric);
+        auto m = dataSet->getMetrics(std::move(metric_names), start, end, rated_metric);
 
         std::vector<py::array_t<unsigned long>> metricList;
         for(size_t i=0;i<m.size();++i) {
 
             // How to handle metric names that are not found?
             if (m[i] != nullptr) {
                 auto element = as_pyarray(m[i]);
                 metricList.emplace_back(element);
             }
-            else {
-                auto  *empty = new py::array_t<unsigned long>;
-                metricList.emplace_back(*empty);
-            }
+            else
+                metricList.emplace_back(as_pyarray(emptyArray));
+
         }
         return metricList;
     }
+     ***/
 
+    [[nodiscard]]
     py::array_t<uint64_t>
-    getMetricListAsNumpyMatrix(const std::vector<std::string> metric_names,
+    getMetricListAsNumpyMatrix(const std::vector<std::string>& metric_names,
                                                       size_t start = INVALID_TIMESTAMP,
                                                       size_t end = INVALID_TIMESTAMP,
                                                       bool rated_metric = false,
-                                                      bool transpose = false)  {
+                                                      bool transpose = false) const  {
         size_t stride = 0;
         auto m = dataSet->getMetricMatrix( metric_names, &stride, start, end, rated_metric);
 
         if (stride !=0) {
 
-            int metricNamesSize = metric_names.size();
+            auto metricNamesSize = metric_names.size();
             if (!transpose) {
-                return py::array_t<uint64_t>({ metricNamesSize, (int)stride}, m->data());
+                return py::array_t<uint64_t>({ (int)metricNamesSize, (int)stride}, m->data());
             }
             else {
-                py::array_t<uint64_t> a = py::array_t<uint64_t>( {(int)stride, metricNamesSize});
+                py::array_t<uint64_t> a = py::array_t<uint64_t>( {(int)stride, (int)metricNamesSize});
 
                 uint64_t   *p   = m->data();
 
                 auto r =  a.mutable_unchecked();
 
                 //printf("dimensions %zd x %zd\n", r.shape(0), r.shape(1));
                 //printf("Element (0,0)=%ld\nElement (%ld,0)=%ld\n", p[0], r.shape(0),  p[r.shape(0)]);
@@ -334,61 +346,49 @@
 
         .. autosummary::
            :toctree: _generate
     )pbdoc";
 
 py::class_<DatasetClass>(m, "Dataset")
     .def(py::init<>())
+    .def("get_metrics", &DatasetClass::getMetric,
+        "Returns a list of values from the metrics, using starting and ending timestamps if specified",
+        py::arg("metric_name"),
+        py::arg("start") = ::INVALID_TIMESTAMP,
+        py::arg("end") = ::INVALID_TIMESTAMP,
+        py::arg("rated_metric") = false)
     .def_readonly("interim", &DatasetClass::interim)
     .def_readonly("metadata", &DatasetClass::metadata)
     .def_readonly("metrics_names", &DatasetClass::metricsNames)
     .def_readonly("file", &DatasetClass::file)
     .def_readonly("path", &DatasetClass::filePath)
     .def_readonly("metrics", &DatasetClass::dataSetMetrics)
-    .def("get_metric", &DatasetClass::getMetric,
-        "Returns a list of values from the metrics, using starting and ending timestamps if specified",
-        py::arg("metric_name"),
-        py::arg("start") = ::INVALID_TIMESTAMP,
-        py::arg("end") = ::INVALID_TIMESTAMP,
-        py::arg("rated_metric") = false)
-    .def("get_metric_list", &DatasetClass::getMetricsList,
-             "Returns a list of lists of values from the metrics, using starting and ending timestamps if specified",
-             py::arg("metric_name"),
-             py::arg("start") = ::INVALID_TIMESTAMP,
-             py::arg("end") = ::INVALID_TIMESTAMP,
-             py::arg("rated_metric") = false)
-    .def("get_metric_numpy", &DatasetClass::getMetricAsNumpyArray,
+        .def("get_metrics_numpy", &DatasetClass::getMetricAsNumpyArray,
              "Returns a metric as a numpy array.",
              py::arg("metric_name"),
              py::arg("start") = ::INVALID_TIMESTAMP,
              py::arg("end") = ::INVALID_TIMESTAMP,
              py::arg("rated_metric") = false)
-    .def("get_metric_list_numpy", &DatasetClass::getMetricListAsNumpyArray,
+        .def("get_metrics_list_numpy", &DatasetClass::getMetricListAsNumpyArray,
              "Returns a list of metrics as numpy arrays.",
              py::arg("testMetricNames"),
              py::arg("start") = ::INVALID_TIMESTAMP,
              py::arg("end") = ::INVALID_TIMESTAMP,
              py::arg("rated_metric") = false);
 
 py::class_<ParserClass>(m, "FTDCParser")
     .def(py::init<>())
     .def("set_verbose", &ParserClass::setVerbose,
          "Set verbose flag", py::arg("verbose"))
     .def("parse_dir", &ParserClass::parseDir,
         "Parses all files in a directory",
-        py::arg("dir"),
-        py::arg("only_metadata") = false,
-        py::arg("only_metrics_names") = false,
-        py::arg("lazy") = true)
+        py::arg("dir"))
     .def("parse_file", &ParserClass::parseFile,
         "Parses one file",
-        py::arg("file"),
-        py::arg("only_metadata") = false,
-        py::arg("only_metrics_names") = false,
-        py::arg("lazy") = true)
+        py::arg("file"))
     .def("get_parsed_file_info", &ParserClass::getParsedFileInfo,
         "Returns information on parsed files")
     .def("dump_file_as_json", &ParserClass::dumpFileAsJson,
         "Dumps a file contents to a file as JSON structures.",
         py::arg("input"),
         py::arg("output"))
     .def("dump_file_as_csv", &ParserClass::dumpFileAsCsv,
@@ -416,20 +416,14 @@
     .def_readonly("metadata", &ParserClass::metadata)
     .def("get_metric_numpy", &ParserClass::getMetricAsNumpyArray,
         "Returns a metric as a numpy array.",
         py::arg("metric_name"),
         py::arg("start") = ::INVALID_TIMESTAMP,
         py::arg("end") = ::INVALID_TIMESTAMP,
         py::arg("rated_metric") = false)
-    .def("get_metrics_list_numpy", &ParserClass::getMetricListAsNumpyArray,
-        "Returns a list of metrics as numpy arrays.",
-        py::arg("testMetricNames"),
-        py::arg("start") = ::INVALID_TIMESTAMP,
-        py::arg("end") = ::INVALID_TIMESTAMP,
-        py::arg("rated_metric") = false)
     .def("get_metrics_list_numpy_matrix", &ParserClass::getMetricListAsNumpyMatrix,
         "Returns a matrix of metrics.",
         py::arg("testMetricNames"),
         py::arg("start") = ::INVALID_TIMESTAMP,
         py::arg("end") = ::INVALID_TIMESTAMP,
         py::arg("rated_metric") = false,
         py::arg("transpose") = false);
```

