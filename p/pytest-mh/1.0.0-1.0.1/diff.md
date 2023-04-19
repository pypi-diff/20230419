# Comparing `tmp/pytest_mh-1.0.0.tar.gz` & `tmp/pytest_mh-1.0.1.tar.gz`

## Comparing `pytest_mh-1.0.0.tar` & `pytest_mh-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/requirements.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/docs/requirements.txt
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/__init__.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/py.typed
--rw-r--r--   0        0        0    30978 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/ssh.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/_private/data.py
--rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/_private/fixtures.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/_private/logging.py
--rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/_private/marks.py
--rw-r--r--   0        0        0    16982 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/_private/multihost.py
--rw-r--r--   0        0        0    14927 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/_private/plugin.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/_private/topology.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/_private/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/utils/__init__.py
--rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/utils/fs.py
--rw-r--r--   0        0        0     7953 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pytest_mh/utils/services.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/LICENSE
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/readme.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 pytest_mh-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/requirements.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/docs/requirements.txt
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/__init__.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/py.typed
+-rw-r--r--   0        0        0    30978 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/ssh.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/data.py
+-rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/fixtures.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/logging.py
+-rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/marks.py
+-rw-r--r--   0        0        0    16982 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/multihost.py
+-rw-r--r--   0        0        0    14927 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/plugin.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/topology.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/utils/__init__.py
+-rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/utils/fs.py
+-rw-r--r--   0        0        0     7953 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/utils/services.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/readme.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/PKG-INFO
```

### Comparing `pytest_mh-1.0.0/pytest_mh/__init__.py` & `pytest_mh-1.0.1/pytest_mh/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/pytest_mh/cli.py` & `pytest_mh-1.0.1/pytest_mh/cli.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/pytest_mh/ssh.py` & `pytest_mh-1.0.1/pytest_mh/ssh.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/pytest_mh/_private/data.py` & `pytest_mh-1.0.1/pytest_mh/_private/data.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/pytest_mh/_private/fixtures.py` & `pytest_mh-1.0.1/pytest_mh/_private/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/pytest_mh/_private/logging.py` & `pytest_mh-1.0.1/pytest_mh/_private/logging.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/pytest_mh/_private/marks.py` & `pytest_mh-1.0.1/pytest_mh/_private/marks.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/pytest_mh/_private/multihost.py` & `pytest_mh-1.0.1/pytest_mh/_private/multihost.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/pytest_mh/_private/plugin.py` & `pytest_mh-1.0.1/pytest_mh/_private/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/pytest_mh/_private/topology.py` & `pytest_mh-1.0.1/pytest_mh/_private/topology.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/pytest_mh/_private/utils.py` & `pytest_mh-1.0.1/pytest_mh/_private/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/pytest_mh/utils/fs.py` & `pytest_mh-1.0.1/pytest_mh/utils/fs.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,24 +88,36 @@
             """,
             log_level=SSHLog.Error,
         )
 
         if result.stdout:
             self.__rollback.append(f"rm --force --recursive '{result.stdout}'")
 
-    def mktmp(self, *, mode: str | None = None, user: str | None = None, group: str | None = None) -> str:
+    def mktmp(
+        self,
+        contents: str | None = None,
+        *,
+        mode: str | None = None,
+        user: str | None = None,
+        group: str | None = None,
+        dedent: bool = True,
+    ) -> str:
         """
         Create temporary file on remote host.
 
+        :param contents: File contents to write.
+        :type contents: str | None
         :param mode: Access mode (chmod value), defaults to None
         :type mode: str | None, optional
         :param user: Owner, defaults to None
         :type user: str | None, optional
         :param group: Group, defaults to None
         :type group: str | None, optional
+        :param dedent: Automatically dedent and strip file contents, defaults to True
+        :type dedent: bool, optional
         :raises OSError: If the file can not be created.
         :return: Temporary file path.
         :rtype: str
         """
 
         self.logger.info(f"Creating temporary file on {self.host.hostname}")
         result = self.host.ssh.run(
@@ -119,14 +131,23 @@
 
         tmpfile = result.stdout.strip()
         if not tmpfile:
             raise OSError("Temporary file was not created")
 
         self.__rollback.append(f"rm --force '{tmpfile}'")
 
+        if contents is not None:
+            if dedent:
+                contents = textwrap.dedent(contents).strip()
+
+            self.logger.info(
+                f'Writing file "{tmpfile}" on {self.host.hostname}', extra={"data": {"Contents": contents}}
+            )
+            self.host.ssh.run(f"cat > '{tmpfile}'", input=contents, log_level=SSHLog.Error)
+
         attrs = self.__gen_chattrs(tmpfile, mode=mode, user=user, group=group)
         if attrs:
             self.host.ssh.run(attrs, log_level=SSHLog.Error)
 
         return tmpfile
 
     def read(self, path: str) -> str:
@@ -281,14 +302,46 @@
                 {self.__gen_chattrs(remote_path, mode=mode, user=user, group=group)}
             """,
             input=encoded,
             log_level=SSHLog.Error,
         )
         self.__rollback.append(f"rm --force '{remote_path}'")
 
+    def upload_to_tmp(
+        self,
+        local_path: str,
+        *,
+        mode: str | None = None,
+        user: str | None = None,
+        group: str | None = None,
+    ) -> str:
+        """
+        Upload local file to a new temporary file on remote host.
+
+        :param local_path: Source local path.
+        :type local_path: str
+        :param mode: Access mode (chmod value), defaults to None
+        :type mode: str | None, optional
+        :param user: Owner, defaults to None
+        :type user: str | None, optional
+        :param group: Group, defaults to None
+        :type group: str | None, optional
+        :return: Temporary file path.
+        :rtype: str
+        """
+        tmp_path = self.mktmp(mode=mode, user=user, group=group)
+
+        self.logger.info(f'Uploading file "{local_path}" to "{self.host.hostname}:{tmp_path}"')
+        with open(local_path, "rb") as f:
+            encoded = base64.b64encode(f.read()).decode("utf-8")
+
+        self.host.ssh.run(f"base64 --decode > '{tmp_path}'", input=encoded, log_level=SSHLog.Error)
+
+        return tmp_path
+
     def download(self, remote_path: str, local_path: str) -> None:
         """
         Download file from remote host to local machine.
 
         :param remote_path: Remote path.
         :type remote_path: str
         :param local_path: Local path.
```

### Comparing `pytest_mh-1.0.0/pytest_mh/utils/services.py` & `pytest_mh-1.0.1/pytest_mh/utils/services.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/LICENSE` & `pytest_mh-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/pyproject.toml` & `pytest_mh-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/readme.md` & `pytest_mh-1.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.0/PKG-INFO` & `pytest_mh-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mh
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pytest multihost plugin
 Project-URL: Homepage, https://github.com/next-actions/pytest-mh
 Project-URL: Bug Tracker, https://github.com/next-actions/pytest-mh/issues
 Author-email: Pavel Březina <pbrezina@redhat.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

