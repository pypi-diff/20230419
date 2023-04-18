# Comparing `tmp/transparentlogs_pymerkle-0.0.1.tar.gz` & `tmp/transparentlogs_pymerkle-0.0.2.tar.gz`

## Comparing `transparentlogs_pymerkle-0.0.1.tar` & `transparentlogs_pymerkle-0.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/.travis.yml
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/__init__.py
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/benchmark.sh
--rwxr-xr-x   0        0        0     2339 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/build-docs.sh
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/demo.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/requirements-dev.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/requirements-doc.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/requirements.txt
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/setup.py
--rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/test.sh
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/docs/index.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/docs/menu.rst
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/docs/proof.rst
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/docs/tree.rst
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/docs/target/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/docs/target/make.bat
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/docs/target/source/conf.py
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/docs/target/source/index.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/docs/target/source/menu.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/docs/target/source/modules.rst
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/docs/target/source/proof.rst
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/docs/target/source/pymerkle.rst
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/docs/target/source/pymerkle.tree.rst
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/docs/target/source/tree.rst
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/src/transparentlogs_pymerkle/__init__.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/src/transparentlogs_pymerkle/constants.py
--rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/src/transparentlogs_pymerkle/hashing.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/src/transparentlogs_pymerkle/proof.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/src/transparentlogs_pymerkle/utils.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/src/transparentlogs_pymerkle/tree/__init__.py
--rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/src/transparentlogs_pymerkle/tree/base.py
--rw-r--r--   0        0        0    13308 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/src/transparentlogs_pymerkle/tree/sakura.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/tests/pytest.ini
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/tests/test_base.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/tests/test_defense.py
--rw-r--r--   0        0        0    12300 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/tests/test_hashing.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/tests/test_proof.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/tests/test_utils.py
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/tests/test_verification.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/tests/sakura/__init__.py
--rw-r--r--   0        0        0    13915 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/tests/sakura/test_path_consistency.py
--rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/tests/sakura/test_path_inclusion.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/tests/sakura/test_previous_state.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/tests/sakura/test_structure.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/.gitignore
--rw-r--r--   0        0        0    35147 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/LICENSE
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/README.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/.travis.yml
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/__init__.py
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/benchmark.sh
+-rwxr-xr-x   0        0        0     2339 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/build-docs.sh
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/demo.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/requirements-doc.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/setup.py
+-rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/test.sh
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/docs/index.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/docs/menu.rst
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/docs/proof.rst
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/docs/tree.rst
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/docs/target/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/docs/target/make.bat
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/docs/target/source/conf.py
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/docs/target/source/index.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/docs/target/source/menu.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/docs/target/source/modules.rst
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/docs/target/source/proof.rst
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/docs/target/source/pymerkle.rst
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/docs/target/source/pymerkle.tree.rst
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/docs/target/source/tree.rst
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/src/transparentlogs_pymerkle/__init__.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/src/transparentlogs_pymerkle/constants.py
+-rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/src/transparentlogs_pymerkle/hashing.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/src/transparentlogs_pymerkle/proof.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/src/transparentlogs_pymerkle/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/src/transparentlogs_pymerkle/tree/__init__.py
+-rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/src/transparentlogs_pymerkle/tree/base.py
+-rw-r--r--   0        0        0    13201 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/src/transparentlogs_pymerkle/tree/sakura.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/tests/pytest.ini
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/tests/test_base.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/tests/test_defense.py
+-rw-r--r--   0        0        0    12300 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/tests/test_hashing.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/tests/test_proof.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/tests/test_utils.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/tests/test_verification.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/tests/sakura/__init__.py
+-rw-r--r--   0        0        0    13915 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/tests/sakura/test_path_consistency.py
+-rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/tests/sakura/test_path_inclusion.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/tests/sakura/test_previous_state.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/tests/sakura/test_structure.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35147 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/README.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 transparentlogs_pymerkle-0.0.2/PKG-INFO
```

### Comparing `transparentlogs_pymerkle-0.0.1/.gitlab-ci.yml` & `transparentlogs_pymerkle-0.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/CHANGELOG.md` & `transparentlogs_pymerkle-0.0.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/build-docs.sh` & `transparentlogs_pymerkle-0.0.2/build-docs.sh`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/demo.py` & `transparentlogs_pymerkle-0.0.2/demo.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/setup.py` & `transparentlogs_pymerkle-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/test.sh` & `transparentlogs_pymerkle-0.0.2/test.sh`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/docs/index.rst` & `transparentlogs_pymerkle-0.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/docs/proof.rst` & `transparentlogs_pymerkle-0.0.2/docs/proof.rst`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/docs/tree.rst` & `transparentlogs_pymerkle-0.0.2/docs/tree.rst`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/docs/target/Makefile` & `transparentlogs_pymerkle-0.0.2/docs/target/Makefile`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/docs/target/make.bat` & `transparentlogs_pymerkle-0.0.2/docs/target/make.bat`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/docs/target/source/conf.py` & `transparentlogs_pymerkle-0.0.2/docs/target/source/conf.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/docs/target/source/index.rst` & `transparentlogs_pymerkle-0.0.2/docs/target/source/index.rst`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/docs/target/source/proof.rst` & `transparentlogs_pymerkle-0.0.2/docs/target/source/proof.rst`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/docs/target/source/pymerkle.rst` & `transparentlogs_pymerkle-0.0.2/docs/target/source/pymerkle.rst`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/docs/target/source/tree.rst` & `transparentlogs_pymerkle-0.0.2/docs/target/source/tree.rst`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/src/transparentlogs_pymerkle/constants.py` & `transparentlogs_pymerkle-0.0.2/src/transparentlogs_pymerkle/constants.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/src/transparentlogs_pymerkle/hashing.py` & `transparentlogs_pymerkle-0.0.2/src/transparentlogs_pymerkle/hashing.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/src/transparentlogs_pymerkle/proof.py` & `transparentlogs_pymerkle-0.0.2/src/transparentlogs_pymerkle/proof.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/src/transparentlogs_pymerkle/utils.py` & `transparentlogs_pymerkle-0.0.2/src/transparentlogs_pymerkle/utils.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/src/transparentlogs_pymerkle/tree/base.py` & `transparentlogs_pymerkle-0.0.2/src/transparentlogs_pymerkle/tree/base.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/src/transparentlogs_pymerkle/tree/sakura.py` & `transparentlogs_pymerkle-0.0.2/src/transparentlogs_pymerkle/tree/sakura.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,16 +262,14 @@
         :type data: str or bytes
         :returns: hash stored by new leaf
         :rtype: bytes
         """
         if encoding:
             new_leaf = Leaf(self.hash_entry(data))
         else:
-            if not isinstance(data, str) or not isinstance(data, bytes):
-                data = str(data) 
             new_leaf = Leaf(bytes(data))
 
         if not self:
             self.root_node = self.update_tail(new_leaf)
             return self.root_node.value
 
         node = self.get_last_maximal_perfect()
```

### Comparing `transparentlogs_pymerkle-0.0.1/tests/conftest.py` & `transparentlogs_pymerkle-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/tests/test_base.py` & `transparentlogs_pymerkle-0.0.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/tests/test_defense.py` & `transparentlogs_pymerkle-0.0.2/tests/test_defense.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/tests/test_hashing.py` & `transparentlogs_pymerkle-0.0.2/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/tests/test_proof.py` & `transparentlogs_pymerkle-0.0.2/tests/test_proof.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/tests/test_utils.py` & `transparentlogs_pymerkle-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/tests/test_verification.py` & `transparentlogs_pymerkle-0.0.2/tests/test_verification.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/tests/sakura/test_path_consistency.py` & `transparentlogs_pymerkle-0.0.2/tests/sakura/test_path_consistency.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/tests/sakura/test_path_inclusion.py` & `transparentlogs_pymerkle-0.0.2/tests/sakura/test_path_inclusion.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/tests/sakura/test_previous_state.py` & `transparentlogs_pymerkle-0.0.2/tests/sakura/test_previous_state.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/tests/sakura/test_structure.py` & `transparentlogs_pymerkle-0.0.2/tests/sakura/test_structure.py`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/LICENSE` & `transparentlogs_pymerkle-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/README.md` & `transparentlogs_pymerkle-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `transparentlogs_pymerkle-0.0.1/pyproject.toml` & `transparentlogs_pymerkle-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "transparentlogs-pymerkle"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Guilherme Fumagali", email="guilhermefumarques@gmail.com" },
 ]
 
 description = "A Python implementation of Merkle Tree"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `transparentlogs_pymerkle-0.0.1/PKG-INFO` & `transparentlogs_pymerkle-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transparentlogs-pymerkle
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python implementation of Merkle Tree
 Project-URL: Homepage, https://github.com/Guilherme-Fumagali/pymerkle
 Project-URL: Bug Tracker, https://github.com/Guilherme-Fumagali/pymerkle/issues
 Author-email: Guilherme Fumagali <guilhermefumarques@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

