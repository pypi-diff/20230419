# Comparing `tmp/python_rdma_qe-0.0.3.tar.gz` & `tmp/python_rdma_qe-0.0.4.tar.gz`

## Comparing `python_rdma_qe-0.0.3.tar` & `python_rdma_qe-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,35 @@
--rwxr-xr-x   0        0        0     4101 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe_test.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/requirements-stable.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/__init__.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdmaqe_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/common/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/common/cli.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/common/file_libs.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/common/fmf_tools.py
--rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/common/tc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/__init__.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/general.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/opa.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/roce.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/sriov.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/sriov/__init__.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/sriov/abc_sriov.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/sriov/sriov.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/__init__.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/.fmf/version
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/opa-fm/__init__.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/opa-fm/functional.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/opa-fm/init_mem.txt
--rw-r--r--   0        0        0    23939 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/opa-fm/init_top.txt
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/opa-fm/main.fmf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/sriov/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0    35079 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/LICENSE
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/README.md
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     4101 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe_test.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/requirements-stable.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/rdmaqe_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/common/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/common/cli.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/common/file_libs.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/common/fmf_tools.py
+-rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/common/tc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/rdma/__init__.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/rdma/general.py
+-rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/rdma/opa.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/rdma/roce.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/rdma/sriov.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/rdma/sriov/__init__.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/rdma/sriov/abc_sriov.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/rdma/sriov/sriov.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/tests/__init__.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/tests/.fmf/version
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/tests/opa-fm/1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/tests/opa-fm/__init__.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/tests/opa-fm/functional.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/tests/opa-fm/functional.py_backup
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/tests/opa-fm/init_mem.txt
+-rw-r--r--   0        0        0    24100 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/tests/opa-fm/init_top.txt
+-rw-r--r--   0        0        0    16908 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/tests/opa-fm/log
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/tests/opa-fm/main.fmf
+-rw-r--r--   0        0        0  7730117 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/tests/opa-fm/mycapture.tgz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/rdmaqe/tests/sriov/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0    35079 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/LICENSE
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/README.md
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.4/PKG-INFO
```

### Comparing `python_rdma_qe-0.0.3/rdmaqe_test.py` & `python_rdma_qe-0.0.4/rdmaqe_test.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.3/requirements-stable.txt` & `python_rdma_qe-0.0.4/requirements-stable.txt`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.3/rdmaqe/common/cli.py` & `python_rdma_qe-0.0.4/rdmaqe/common/cli.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.3/rdmaqe/common/file_libs.py` & `python_rdma_qe-0.0.4/rdmaqe/common/file_libs.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,9 +37,7 @@
             if p not in lines:
                 with open(conf_file, 'a+') as wf:
                     wf.write(p)
                     wf.write('\n')
             else:
                 print("INFO: It's all set already.")
 
-
-
```

### Comparing `python_rdma_qe-0.0.3/rdmaqe/common/fmf_tools.py` & `python_rdma_qe-0.0.4/rdmaqe/common/fmf_tools.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.3/rdmaqe/common/tc.py` & `python_rdma_qe-0.0.4/rdmaqe/common/tc.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.3/rdmaqe/rdma/general.py` & `python_rdma_qe-0.0.4/rdmaqe/rdma/general.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.3/rdmaqe/rdma/opa.py` & `python_rdma_qe-0.0.4/rdmaqe/rdma/opa.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,8 +125,21 @@
     """
     cmd = "/usr/sbin/opasaquery"
     retcode, output = run(cmd, return_output=True, verbose=True)
     if retcode != 0:
         _print("FAIL: Could not run opasaquery")
         return None
 
-    return output
+    return output
+
+
+def is_port_active():
+    """
+    @return: True, if the port is active; Otherwise, return False.
+    """
+    cmd = "opainfo | grep Active -C 50"
+    retcode, output = run(cmd, return_output=True, verbose=True)
+    if retcode != 0:
+        _print("FAIL: No active port")
+        return False
+
+    return True
```

### Comparing `python_rdma_qe-0.0.3/rdmaqe/rdma/roce.py` & `python_rdma_qe-0.0.4/rdmaqe/rdma/roce.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.3/rdmaqe/rdma/sriov/abc_sriov.py` & `python_rdma_qe-0.0.4/rdmaqe/rdma/sriov/abc_sriov.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.3/rdmaqe/rdma/sriov/sriov.py` & `python_rdma_qe-0.0.4/rdmaqe/rdma/sriov/sriov.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.3/rdmaqe/tests/opa-fm/functional.py` & `python_rdma_qe-0.0.4/rdmaqe/tests/opa-fm/functional.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.3/rdmaqe/tests/opa-fm/init_top.txt` & `python_rdma_qe-0.0.4/rdmaqe/tests/opa-fm/init_top.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,189 +1,186 @@
-top - 03:22:04 up 6 days,  5:02,  1 user,  load average: 0.00, 0.00, 0.00
-Tasks: 295 total,   1 running, 294 sleeping,   0 stopped,   0 zombie
-%Cpu(s):  0.5 us,  0.8 sy,  0.0 ni, 98.7 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st
-MiB Mem :  47972.4 total,  43900.5 free,   2967.1 used,   2643.2 buff/cache
-MiB Swap:  24180.0 total,  24180.0 free,      0.0 used.  45005.3 avail Mem 
+top - 06:19:05 up 21 days,  7:59,  1 user,  load average: 0.02, 0.03, 0.01
+Tasks: 297 total,   1 running, 296 sleeping,   0 stopped,   0 zombie
+%Cpu(s):  1.1 us,  0.8 sy,  0.0 ni, 98.1 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st
+MiB Mem :  47972.4 total,  43767.6 free,   2858.4 used,   2881.5 buff/cache
+MiB Swap:  24180.0 total,  24180.0 free,      0.0 used.  45114.0 avail Mem 
 
     PID USER      PR  NI    VIRT    RES    SHR S  %CPU  %MEM     TIME+ COMMAND
- 380714 root      20   0   10700   4212   3400 R  11.8   0.0   0:00.04 top
-     18 root      20   0       0      0      0 I   5.9   0.0   3:14.30 rcu_pre+
-      1 root      20   0  173836  18412  11052 S   0.0   0.0   0:20.42 systemd
-      2 root      20   0       0      0      0 S   0.0   0.0   0:00.13 kthreadd
+   1041 root      20   0  626460  36416  34740 S  23.5   0.1  24:45.05 rsyslogd
+1222339 root      20   0   10700   4280   3468 R   5.9   0.0   0:00.03 top
+      1 root      20   0  173836  18412  11052 S   0.0   0.0   0:32.94 systemd
+      2 root      20   0       0      0      0 S   0.0   0.0   0:00.62 kthreadd
       3 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 rcu_gp
       4 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 rcu_par+
       5 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 slub_fl+
       6 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 netns
       8 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-     10 root       0 -20       0      0      0 I   0.0   0.0   0:00.08 kworker+
+     10 root       0 -20       0      0      0 I   0.0   0.0   0:00.14 kworker+
      12 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mm_perc+
      14 root      20   0       0      0      0 I   0.0   0.0   0:00.00 rcu_tas+
      15 root      20   0       0      0      0 I   0.0   0.0   0:00.00 rcu_tas+
      16 root      20   0       0      0      0 I   0.0   0.0   0:00.00 rcu_tas+
-     17 root      20   0       0      0      0 S   0.0   0.0   0:00.07 ksoftir+
-     19 root      rt   0       0      0      0 S   0.0   0.0   0:00.75 migrati+
+     17 root      20   0       0      0      0 S   0.0   0.0   0:00.28 ksoftir+
+     18 root      20   0       0      0      0 I   0.0   0.0  11:03.38 rcu_pre+
+     19 root      rt   0       0      0      0 S   0.0   0.0   0:02.59 migrati+
      21 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/0
      22 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/1
-     23 root      rt   0       0      0      0 S   0.0   0.0   0:00.93 migrati+
-     24 root      20   0       0      0      0 S   0.0   0.0   0:00.05 ksoftir+
+     23 root      rt   0       0      0      0 S   0.0   0.0   0:02.66 migrati+
+     24 root      20   0       0      0      0 S   0.0   0.0   0:00.14 ksoftir+
      26 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      27 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/2
-     28 root      rt   0       0      0      0 S   0.0   0.0   0:00.98 migrati+
-     29 root      20   0       0      0      0 S   0.0   0.0   0:00.01 ksoftir+
+     28 root      rt   0       0      0      0 S   0.0   0.0   0:02.80 migrati+
+     29 root      20   0       0      0      0 S   0.0   0.0   0:00.03 ksoftir+
      31 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      32 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/3
-     33 root      rt   0       0      0      0 S   0.0   0.0   0:00.88 migrati+
-     34 root      20   0       0      0      0 S   0.0   0.0   0:00.20 ksoftir+
+     33 root      rt   0       0      0      0 S   0.0   0.0   0:02.48 migrati+
+     34 root      20   0       0      0      0 S   0.0   0.0   0:00.59 ksoftir+
      36 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      37 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/4
-     38 root      rt   0       0      0      0 S   0.0   0.0   0:00.93 migrati+
-     39 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     38 root      rt   0       0      0      0 S   0.0   0.0   0:02.60 migrati+
+     39 root      20   0       0      0      0 S   0.0   0.0   0:00.02 ksoftir+
      41 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      42 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/5
-     43 root      rt   0       0      0      0 S   0.0   0.0   0:00.94 migrati+
-     44 root      20   0       0      0      0 S   0.0   0.0   0:00.01 ksoftir+
+     43 root      rt   0       0      0      0 S   0.0   0.0   0:02.64 migrati+
+     44 root      20   0       0      0      0 S   0.0   0.0   0:00.04 ksoftir+
      46 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      47 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/6
-     48 root      rt   0       0      0      0 S   0.0   0.0   0:00.95 migrati+
-     49 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     48 root      rt   0       0      0      0 S   0.0   0.0   0:02.69 migrati+
+     49 root      20   0       0      0      0 S   0.0   0.0   0:00.02 ksoftir+
      51 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      52 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/7
-     53 root      rt   0       0      0      0 S   0.0   0.0   0:00.97 migrati+
-     54 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     53 root      rt   0       0      0      0 S   0.0   0.0   0:02.76 migrati+
+     54 root      20   0       0      0      0 S   0.0   0.0   0:00.03 ksoftir+
      56 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      57 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/8
-     58 root      rt   0       0      0      0 S   0.0   0.0   0:00.95 migrati+
-     59 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     58 root      rt   0       0      0      0 S   0.0   0.0   0:02.65 migrati+
+     59 root      20   0       0      0      0 S   0.0   0.0   0:00.02 ksoftir+
      61 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      62 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/9
-     63 root      rt   0       0      0      0 S   0.0   0.0   0:00.99 migrati+
-     64 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     63 root      rt   0       0      0      0 S   0.0   0.0   0:02.80 migrati+
+     64 root      20   0       0      0      0 S   0.0   0.0   0:00.03 ksoftir+
      66 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      67 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/10
-     68 root      rt   0       0      0      0 S   0.0   0.0   0:01.04 migrati+
-     69 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     68 root      rt   0       0      0      0 S   0.0   0.0   0:02.79 migrati+
+     69 root      20   0       0      0      0 S   0.0   0.0   0:00.01 ksoftir+
      71 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      74 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/11
-     75 root      rt   0       0      0      0 S   0.0   0.0   0:01.01 migrati+
-     76 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     75 root      rt   0       0      0      0 S   0.0   0.0   0:02.66 migrati+
+     76 root      20   0       0      0      0 S   0.0   0.0   0:00.01 ksoftir+
      78 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      79 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/12
-     80 root      rt   0       0      0      0 S   0.0   0.0   0:01.04 migrati+
-     81 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     80 root      rt   0       0      0      0 S   0.0   0.0   0:02.76 migrati+
+     81 root      20   0       0      0      0 S   0.0   0.0   0:00.01 ksoftir+
      83 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      84 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/13
-     85 root      rt   0       0      0      0 S   0.0   0.0   0:01.03 migrati+
+     85 root      rt   0       0      0      0 S   0.0   0.0   0:02.69 migrati+
      86 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
      88 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      89 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/14
-     90 root      rt   0       0      0      0 S   0.0   0.0   0:01.01 migrati+
+     90 root      rt   0       0      0      0 S   0.0   0.0   0:02.64 migrati+
      91 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
      93 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      94 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/15
-     95 root      rt   0       0      0      0 S   0.0   0.0   0:01.03 migrati+
-     96 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
-     98 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
+     95 root      rt   0       0      0      0 S   0.0   0.0   0:02.67 migrati+
+     96 root      20   0       0      0      0 S   0.0   0.0   0:00.03 ksoftir+
+     98 root       0 -20       0      0      0 I   0.0   0.0   0:00.47 kworker+
      99 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/16
-    100 root      rt   0       0      0      0 S   0.0   0.0   0:01.04 migrati+
+    100 root      rt   0       0      0      0 S   0.0   0.0   0:02.70 migrati+
     101 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
     103 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
     104 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/17
-    105 root      rt   0       0      0      0 S   0.0   0.0   0:01.04 migrati+
+    105 root      rt   0       0      0      0 S   0.0   0.0   0:02.67 migrati+
     106 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
     108 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
     109 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/18
-    110 root      rt   0       0      0      0 S   0.0   0.0   0:01.04 migrati+
+    110 root      rt   0       0      0      0 S   0.0   0.0   0:02.68 migrati+
     111 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
     113 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
     114 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/19
-    115 root      rt   0       0      0      0 S   0.0   0.0   0:01.04 migrati+
+    115 root      rt   0       0      0      0 S   0.0   0.0   0:02.68 migrati+
     116 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
     118 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
     139 root      20   0       0      0      0 S   0.0   0.0   0:00.00 kdevtmp+
     140 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 inet_fr+
-    141 root      20   0       0      0      0 S   0.0   0.0   0:00.01 kauditd
-    143 root      20   0       0      0      0 I   0.0   0.0   0:00.63 kworker+
-    145 root      20   0       0      0      0 S   0.0   0.0   0:00.12 khungta+
+    141 root      20   0       0      0      0 S   0.0   0.0   0:00.03 kauditd
+    145 root      20   0       0      0      0 S   0.0   0.0   0:00.44 khungta+
     146 root      20   0       0      0      0 S   0.0   0.0   0:00.00 oom_rea+
     147 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 writeba+
-    148 root      20   0       0      0      0 S   0.0   0.0   0:04.76 kcompac+
-    149 root      20   0       0      0      0 S   0.0   0.0   0:04.08 kcompac+
+    148 root      20   0       0      0      0 S   0.0   0.0   0:16.50 kcompac+
+    149 root      20   0       0      0      0 S   0.0   0.0   0:14.28 kcompac+
     150 root      25   5       0      0      0 S   0.0   0.0   0:00.00 ksmd
-    151 root      39  19       0      0      0 S   0.0   0.0   0:02.40 khugepa+
+    151 root      39  19       0      0      0 S   0.0   0.0   0:06.89 khugepa+
     152 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 cryptd
     153 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kintegr+
     154 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kblockd
     155 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 blkcg_p+
-    160 root      20   0       0      0      0 I   0.0   0.0   0:00.26 kworker+
-    164 root      20   0       0      0      0 I   0.0   0.0   2:24.82 kworker+
     174 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 tpm_dev+
     175 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 md
     176 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 edac-po+
     177 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 watchdo+
-    178 root       0 -20       0      0      0 I   0.0   0.0   0:00.06 kworker+
+    178 root       0 -20       0      0      0 I   0.0   0.0   0:10.45 kworker+
     179 root      20   0       0      0      0 S   0.0   0.0   0:00.00 kswapd0
     180 root      20   0       0      0      0 S   0.0   0.0   0:00.00 kswapd1
     186 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kthrotld
-    189 root      20   0       0      0      0 I   0.0   0.0   0:00.86 kworker+
     195 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 acpi_th+
     196 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kmpath_+
     197 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kaluad
-    198 root       0 -20       0      0      0 I   0.0   0.0   0:00.05 kworker+
-    200 root       0 -20       0      0      0 I   0.0   0.0   0:04.16 kworker+
-    201 root       0 -20       0      0      0 I   0.0   0.0   0:00.10 kworker+
-    203 root       0 -20       0      0      0 I   0.0   0.0   0:00.04 kworker+
-    204 root       0 -20       0      0      0 I   0.0   0.0   0:00.08 kworker+
+    198 root       0 -20       0      0      0 I   0.0   0.0   0:00.33 kworker+
+    200 root       0 -20       0      0      0 I   0.0   0.0   0:14.17 kworker+
+    201 root       0 -20       0      0      0 I   0.0   0.0   0:00.31 kworker+
+    203 root       0 -20       0      0      0 I   0.0   0.0   0:00.15 kworker+
+    204 root       0 -20       0      0      0 I   0.0   0.0   0:00.37 kworker+
     205 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mld
-    206 root       0 -20       0      0      0 I   0.0   0.0   0:00.10 kworker+
+    206 root       0 -20       0      0      0 I   0.0   0.0   0:00.33 kworker+
     207 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ipv6_ad+
     208 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kstrp
     220 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 zswap-s+
     333 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
     334 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    336 root       0 -20       0      0      0 I   0.0   0.0   0:00.03 kworker+
-    402 root       0 -20       0      0      0 I   0.0   0.0   0:00.05 kworker+
-    508 root       0 -20       0      0      0 I   0.0   0.0   0:00.04 kworker+
-    542 root       0 -20       0      0      0 I   0.0   0.0   0:00.06 kworker+
+    336 root       0 -20       0      0      0 I   0.0   0.0   0:00.15 kworker+
+    402 root       0 -20       0      0      0 I   0.0   0.0   0:00.07 kworker+
+    508 root       0 -20       0      0      0 I   0.0   0.0   0:00.08 kworker+
+    542 root       0 -20       0      0      0 I   0.0   0.0   0:00.14 kworker+
     577 root      20   0       0      0      0 S   0.0   0.0   0:00.00 scsi_eh+
     578 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 scsi_tm+
     592 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 tls-strp
     598 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ata_sff
-    600 root       0 -20       0      0      0 I   0.0   0.0   0:00.13 kworker+
+    600 root       0 -20       0      0      0 I   0.0   0.0   0:00.30 kworker+
     605 root      20   0       0      0      0 S   0.0   0.0   0:00.01 scsi_eh+
     606 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 scsi_tm+
     607 root      20   0       0      0      0 S   0.0   0.0   0:00.02 scsi_eh+
     608 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 scsi_tm+
-    609 root       0 -20       0      0      0 I   0.0   0.0   0:00.02 kworker+
-    610 root       0 -20       0      0      0 I   0.0   0.0   0:01.02 kworker+
+    609 root       0 -20       0      0      0 I   0.0   0.0   0:00.05 kworker+
+    610 root       0 -20       0      0      0 I   0.0   0.0   0:04.18 kworker+
     612 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mlx5_he+
     613 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mlx5_pa+
     616 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mlx5_cm+
     643 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mlx5_ev+
     644 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mlx5_fw+
     645 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mlx5_fc
     646 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mlx5_hv+
-    686 root       0 -20       0      0      0 I   0.0   0.0   0:00.02 kworker+
+    686 root       0 -20       0      0      0 I   0.0   0.0   0:00.07 kworker+
     689 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kdmflus+
     696 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kdmflus+
-    702 root       0 -20       0      0      0 I   0.0   0.0   0:00.03 kworker+
-    714 root       0 -20       0      0      0 I   0.0   0.0   0:00.02 kworker+
+    702 root       0 -20       0      0      0 I   0.0   0.0   0:00.08 kworker+
+    714 root       0 -20       0      0      0 I   0.0   0.0   0:00.06 kworker+
     716 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfsalloc
     717 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs_mru+
     718 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-buf+
     719 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-con+
     720 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-rec+
     721 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-blo+
     722 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-ino+
     723 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-log+
     724 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-cil+
-    725 root      20   0       0      0      0 S   0.0   0.0   0:35.81 xfsaild+
-    772 root       0 -20       0      0      0 I   0.0   0.0   0:02.00 kworker+
-    773 root       0 -20       0      0      0 I   0.0   0.0   0:00.04 kworker+
-    790 root      20   0  313056 180940 179652 S   0.0   0.4   3:16.57 systemd+
-    806 root      20   0   36388  14452   9012 S   0.0   0.0   0:01.12 systemd+
+    725 root      20   0       0      0      0 S   0.0   0.0   2:19.99 xfsaild+
+    772 root       0 -20       0      0      0 I   0.0   0.0   0:11.17 kworker+
+    773 root       0 -20       0      0      0 I   0.0   0.0   0:00.09 kworker+
+    790 root      20   0  279660 157672 156364 S   0.0   0.3  14:26.30 systemd+
+    806 root      20   0   36388  14720   9280 S   0.0   0.0   0:02.86 systemd+
     887 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ipmi-ms+
     890 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-buf+
     891 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-con+
     892 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-rec+
     893 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-blo+
     894 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-ino+
     895 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-log+
@@ -198,15 +195,14 @@
     905 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ib_mad1
     906 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ib_mad2
     907 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mkey_ca+
     916 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 hfi_opfn
     923 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ipoib_wq
     925 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ipoib_wq
     929 root      20   0    6464   1544   1312 S   0.0   0.0   0:00.01 rdma-ndd
-    931 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
     934 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-buf+
     935 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-con+
     936 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-rec+
     937 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-blo+
     938 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-ino+
     939 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 rdma_cm
     940 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-log+
@@ -217,86 +213,92 @@
     949 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 target_+
     950 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xcopy_wq
     974 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 rpciod
     975 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xprtiod
     983 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 irq/196+
     984 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 irq/197+
     985 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 irq/198+
-    989 root      16  -4   18144   4456   1688 S   0.0   0.0   0:00.32 auditd
-   1025 root      20   0  257396  19796  16716 S   0.0   0.0  18:00.62 Network+
-   1034 chrony    20   0   10440   3120   2616 S   0.0   0.0   0:00.75 chronyd
-   1038 root      20   0   79360   5348   2820 S   0.0   0.0   2:35.57 irqbala+
-   1041 root      20   0  628824  46888  45236 S   0.0   0.1   4:47.18 rsyslogd
+    989 root      16  -4   18144   4456   1688 S   0.0   0.0   0:00.99 auditd
+   1025 root      20   0  257396  19796  16716 S   0.0   0.0  59:14.32 Network+
+   1034 chrony    20   0   10440   3120   2616 S   0.0   0.0   0:02.50 chronyd
+   1038 root      20   0   79360   5348   2820 S   0.0   0.0   8:53.29 irqbala+
    1056 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 hfi1_up+
    1057 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 hfi0_0
    1058 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 hfi_lin+
-   1064 root      20   0   21772  12948   9100 S   0.0   0.0   0:01.07 systemd+
-   1083 dbus      20   0   11068   5028   4060 S   0.0   0.0   0:00.14 dbus-br+
-   1109 dbus      20   0    5424   3364   2500 S   0.0   0.0   0:00.58 dbus-br+
+   1064 root      20   0   21772  12948   9100 S   0.0   0.0   0:03.10 systemd+
+   1083 dbus      20   0   11068   5028   4060 S   0.0   0.0   0:00.15 dbus-br+
+   1109 dbus      20   0    5424   3364   2500 S   0.0   0.0   0:01.31 dbus-br+
    1118 root      20   0    3044   1100   1008 S   0.0   0.0   0:00.03 agetty
    1119 root      20   0    5612   1096   1008 S   0.0   0.0   0:00.00 agetty
-   1120 root      20   0   81052   4312   2076 S   0.0   0.0   0:00.02 rhsmcer+
+   1120 root      20   0   81052   4312   2076 S   0.0   0.0   0:00.10 rhsmcer+
    1147 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ib_mad1
    1148 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ipoib_wq
-   2652 root      20   0    8636   3852   2932 S   0.0   0.0   0:00.76 crond
-   2657 root      20   0  231528   8448   5584 S   0.0   0.0   0:10.86 restrai+
-   5685 root      20   0   23440  15108  10844 S   0.0   0.0   0:00.35 systemd
+   2652 root      20   0    8636   3852   2932 S   0.0   0.0   0:02.51 crond
+   2657 root      20   0  231528   8448   5584 S   0.0   0.0   0:33.61 restrai+
+   5685 root      20   0   23440  15108  10844 S   0.0   0.0   0:00.66 systemd
    5698 root      20   0  173224   5656      0 S   0.0   0.0   0:00.00 (sd-pam)
-   6633 root      20   0   15836   9324   8020 S   0.0   0.0   0:00.04 sshd
+   6633 root      20   0   15836   9324   8020 S   0.0   0.0   0:00.06 sshd
   17519 root      20   0    7276   3704   3344 S   0.0   0.0   0:00.01 10_bash+
-  17546 root      20   0    7308   3768   3328 S   0.0   0.0   1:40.16 runtest+
-  17643 root      20   0   38160   4580   4100 S   0.0   0.0   0:02.41 master
-  17645 postfix   20   0   45296   8400   7416 S   0.0   0.0   0:00.44 qmgr
-  17660 postfix   20   0   46380  10800   9500 S   0.0   0.0   0:00.23 tlsmgr
-  24868 root      20   0       0      0      0 I   0.0   0.0   0:00.93 kworker+
-  68805 root      20   0       0      0      0 I   0.0   0.0   0:00.56 kworker+
-  91596 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 133670 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
- 137051 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 138083 root      20   0       0      0      0 I   0.0   0.0   0:00.36 kworker+
- 138293 root      20   0   13516   7736   3900 S   0.0   0.0   0:00.13 opafmd
- 138306 root      20   0 2325560 404492   9300 S   0.0   0.8  17:13.82 sm
- 138934 root      20   0       0      0      0 I   0.0   0.0   0:00.15 kworker+
- 161022 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 163727 root      20   0       0      0      0 I   0.0   0.0   0:00.64 kworker+
- 165261 root      20   0       0      0      0 I   0.0   0.0   0:00.66 kworker+
- 168567 root      20   0       0      0      0 I   0.0   0.0   0:00.09 kworker+
- 193969 root      20   0       0      0      0 I   0.0   0.0   0:00.83 kworker+
- 198788 root      20   0       0      0      0 I   0.0   0.0   0:00.13 kworker+
- 252358 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 254441 root      20   0       0      0      0 I   0.0   0.0   0:00.17 kworker+
- 255728 root      20   0       0      0      0 I   0.0   0.0   0:00.20 kworker+
- 255729 root      20   0       0      0      0 I   0.0   0.0   0:00.09 kworker+
- 310696 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 312786 root      20   0   18928  11444   9548 S   0.0   0.0   0:00.05 sshd
- 312792 root      20   0   18784   7120   5228 S   0.0   0.0   0:00.62 sshd
- 312793 root      20   0    7568   4496   3700 S   0.0   0.0   0:00.32 bash
- 312799 root      20   0       0      0      0 I   0.0   0.0   0:00.15 kworker+
- 312800 root      20   0       0      0      0 I   0.0   0.0   0:00.37 kworker+
- 312857 root      20   0       0      0      0 I   0.0   0.0   0:00.03 kworker+
- 314087 root      20   0       0      0      0 I   0.0   0.0   0:00.10 kworker+
- 314088 root      20   0       0      0      0 I   0.0   0.0   0:00.09 kworker+
- 316652 root      20   0       0      0      0 I   0.0   0.0   0:00.07 kworker+
- 319980 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 327781 root      20   0       0      0      0 I   0.0   0.0   0:00.04 kworker+
- 362654 root      20   0       0      0      0 I   0.0   0.0   0:00.03 kworker+
- 363787 root      20   0       0      0      0 I   0.0   0.0   0:00.18 kworker+
- 366804 root      20   0       0      0      0 I   0.0   0.0   0:00.13 kworker+
- 368869 root      20   0       0      0      0 I   0.0   0.0   0:00.09 kworker+
- 369161 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 369162 root      20   0       0      0      0 I   0.0   0.0   0:00.04 kworker+
- 372508 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
- 372509 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
- 374102 root      20   0       0      0      0 I   0.0   0.0   0:00.13 kworker+
- 374848 root       0 -20       0      0      0 I   0.0   0.0   0:00.06 kworker+
- 376269 root      20   0       0      0      0 I   0.0   0.0   0:00.17 kworker+
- 377127 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 377130 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 377549 root       0 -20       0      0      0 I   0.0   0.0   0:00.04 kworker+
- 378497 root      20   0       0      0      0 I   0.0   0.0   0:00.09 kworker+
- 378592 root      20   0       0      0      0 I   0.0   0.0   0:00.07 kworker+
- 379283 postfix   20   0   45252   8328   7356 S   0.0   0.0   0:00.01 pickup
- 379804 root      20   0    5648   2416   2176 S   0.0   0.0   0:00.00 anacron
- 380421 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 380671 root      20   0    5584   1032    940 S   0.0   0.0   0:00.00 sleep
- 380672 root      20   0   35388  30660  10300 S   0.0   0.1   0:00.50 python3
- 380713 root      20   0    7120   3264   3008 S   0.0   0.0   0:00.00 sh
+  17546 root      20   0    7308   3768   3328 S   0.0   0.0   5:44.27 runtest+
+  17643 root      20   0   38160   4580   4100 S   0.0   0.0   0:08.19 master
+  17645 postfix   20   0   45296   8400   7416 S   0.0   0.0   0:01.50 qmgr
+  17660 postfix   20   0   46380  10800   9500 S   0.0   0.0   0:00.76 tlsmgr
+  24868 root      20   0       0      0      0 I   0.0   0.0   0:01.39 kworker+
+ 165261 root      20   0       0      0      0 I   0.0   0.0   0:01.39 kworker+
+ 434483 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 500847 root      20   0       0      0      0 I   0.0   0.0   0:01.00 kworker+
+ 501175 root      20   0   10584   4356   3988 S   0.0   0.0   0:00.01 dbus-br+
+ 501176 root      20   0    4864   1400   1252 S   0.0   0.0   0:00.02 dbus-br+
+ 894516 root      20   0       0      0      0 I   0.0   0.0   0:00.77 kworker+
+ 958070 root      20   0       0      0      0 I   0.0   0.0   0:00.22 kworker+
+ 958071 root      20   0       0      0      0 I   0.0   0.0   0:00.43 kworker+
+1001027 root       0 -20       0      0      0 I   0.0   0.0   0:01.93 kworker+
+1017177 root       0 -20       0      0      0 I   0.0   0.0   0:01.74 kworker+
+1133738 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
+1133739 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
+1137217 root      20   0       0      0      0 I   0.0   0.0   0:00.05 kworker+
+1137218 root      20   0       0      0      0 I   0.0   0.0   0:00.21 kworker+
+1139698 root      20   0       0      0      0 I   0.0   0.0   0:00.38 kworker+
+1139699 root      20   0       0      0      0 I   0.0   0.0   0:00.27 kworker+
+1140261 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+1140339 root      20   0   13516   7748   3912 S   0.0   0.0   0:00.13 opafmd
+1140340 root      20   0  912452 266496   8764 S   0.0   0.5   6:42.49 sm
+1144219 root      20   0       0      0      0 I   0.0   0.0   0:00.18 kworker+
+1153134 root      20   0       0      0      0 I   0.0   0.0   0:00.09 kworker+
+1164411 root      20   0       0      0      0 I   0.0   0.0   0:00.52 kworker+
+1172190 root      20   0       0      0      0 I   0.0   0.0   0:00.29 kworker+
+1172507 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+1189074 root      20   0       0      0      0 I   0.0   0.0   0:00.49 kworker+
+1194140 root      20   0       0      0      0 I   0.0   0.0   0:00.74 kworker+
+1202015 root      20   0       0      0      0 I   0.0   0.0   0:01.38 kworker+
+1203964 root      20   0       0      0      0 I   0.0   0.0   0:11.72 kworker+
+1204994 root      20   0       0      0      0 I   0.0   0.0   0:00.09 kworker+
+1205789 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
+1205824 root      20   0       0      0      0 I   0.0   0.0   0:00.06 kworker+
+1207627 root      20   0       0      0      0 I   0.0   0.0   0:00.93 kworker+
+1207631 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+1207704 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+1209404 root      20   0       0      0      0 I   0.0   0.0   0:00.14 kworker+
+1210019 root      20   0       0      0      0 I   0.0   0.0   0:00.15 kworker+
+1211747 root      20   0       0      0      0 I   0.0   0.0   0:00.16 kworker+
+1213580 root      20   0       0      0      0 I   0.0   0.0   0:00.29 kworker+
+1213845 root      20   0       0      0      0 I   0.0   0.0   0:00.25 kworker+
+1213881 root      20   0   18920  11452   9564 S   0.0   0.0   0:00.05 sshd
+1213887 root      20   0   18784   7164   5280 S   0.0   0.0   0:01.30 sshd
+1213888 root      20   0    7568   4456   3632 S   0.0   0.0   0:00.17 bash
+1213931 root      20   0       0      0      0 I   0.0   0.0   0:00.03 kworker+
+1213932 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+1214679 postfix   20   0   45252   8340   7372 S   0.0   0.0   0:00.02 pickup
+1216221 root      20   0       0      0      0 I   0.0   0.0   0:00.08 kworker+
+1216579 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+1217023 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+1217920 root      20   0       0      0      0 I   0.0   0.0   0:00.15 kworker+
+1219263 root      20   0       0      0      0 I   0.0   0.0   0:00.11 kworker+
+1219495 root      20   0       0      0      0 I   0.0   0.0   0:00.24 kworker+
+1220149 root      20   0       0      0      0 I   0.0   0.0   0:00.04 kworker+
+1220903 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
+1222069 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+1222106 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
+1222203 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+1222296 root      20   0    5584   1028    940 S   0.0   0.0   0:00.00 sleep
+1222297 root      20   0   35228  30668  10236 S   0.0   0.1   0:00.98 python
+1222338 root      20   0    7120   3268   3020 S   0.0   0.0   0:00.00 sh
```

### Comparing `python_rdma_qe-0.0.3/LICENSE` & `python_rdma_qe-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.3/pyproject.toml` & `python_rdma_qe-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.3/PKG-INFO` & `python_rdma_qe-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-rdma-qe
-Version: 0.0.3
+Version: 0.0.4
 Summary: Redhat Kernel RDMA QE Python libs and tests
 Project-URL: Documentation, https://gitlab.com/rh-rdma-qe/python-rdma-qe#README.md
 Project-URL: Issues, https://gitlab.com/rh-rdma-qe/python-rdma-qe/issues
 Project-URL: Source, https://gitlab.com/rh-rdma-qe/python-rdma-qe
 Author-email: Zhaojuan Guo <zguo@redhat.com>
 Maintainer-email: Zhaojuan Guo <zguo@redhat.com>
 License-Expression: GPL-3.0-or-later
```

