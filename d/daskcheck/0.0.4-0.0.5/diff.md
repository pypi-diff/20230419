# Comparing `tmp/daskcheck-0.0.4.tar.gz` & `tmp/daskcheck-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daskcheck-0.0.4.tar", last modified: Fri Apr 14 12:43:18 2023, max compression
+gzip compressed data, was "daskcheck-0.0.5.tar", last modified: Wed Apr 19 07:18:56 2023, max compression
```

## Comparing `daskcheck-0.0.4.tar` & `daskcheck-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-14 12:43:18.034442 daskcheck-0.0.4/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2802 2023-04-14 12:43:18.034442 daskcheck-0.0.4/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2524 2023-04-14 12:43:15.000000 daskcheck-0.0.4/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-14 12:43:18.030442 daskcheck-0.0.4/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      680 2023-01-13 14:22:42.000000 daskcheck-0.0.4/bin/daskcheck
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-14 12:43:18.030442 daskcheck-0.0.4/daskcheck/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2023-01-13 14:22:42.000000 daskcheck-0.0.4/daskcheck/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6840 2023-01-13 14:22:42.000000 daskcheck-0.0.4/daskcheck/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6892 2023-01-13 14:22:42.000000 daskcheck-0.0.4/daskcheck/daskcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1090 2023-01-13 14:22:42.000000 daskcheck-0.0.4/daskcheck/unitname.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-04-14 12:43:17.000000 daskcheck-0.0.4/daskcheck/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-14 12:43:18.030442 daskcheck-0.0.4/daskcheck.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2802 2023-04-14 12:43:18.000000 daskcheck-0.0.4/daskcheck.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      304 2023-04-14 12:43:18.000000 daskcheck-0.0.4/daskcheck.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-14 12:43:18.000000 daskcheck-0.0.4/daskcheck.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        5 2023-04-14 12:43:18.000000 daskcheck-0.0.4/daskcheck.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-04-14 12:43:18.000000 daskcheck-0.0.4/daskcheck.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-14 12:43:18.034442 daskcheck-0.0.4/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1151 2023-04-14 12:41:57.000000 daskcheck-0.0.4/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-19 07:18:56.333319 daskcheck-0.0.5/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     3799 2023-04-19 07:18:56.333319 daskcheck-0.0.5/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     3511 2023-04-19 07:18:53.000000 daskcheck-0.0.5/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-19 07:18:56.329319 daskcheck-0.0.5/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      853 2023-04-19 07:18:06.000000 daskcheck-0.0.5/bin/daskcheck
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-19 07:18:56.333319 daskcheck-0.0.5/daskcheck/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2023-01-13 14:22:42.000000 daskcheck-0.0.5/daskcheck/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6840 2023-01-13 14:22:42.000000 daskcheck-0.0.5/daskcheck/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6892 2023-01-13 14:22:42.000000 daskcheck-0.0.5/daskcheck/daskcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1090 2023-01-13 14:22:42.000000 daskcheck-0.0.5/daskcheck/unitname.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-04-19 07:18:56.000000 daskcheck-0.0.5/daskcheck/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-19 07:18:56.333319 daskcheck-0.0.5/daskcheck.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     3799 2023-04-19 07:18:56.000000 daskcheck-0.0.5/daskcheck.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      304 2023-04-19 07:18:56.000000 daskcheck-0.0.5/daskcheck.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-19 07:18:56.000000 daskcheck-0.0.5/daskcheck.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-04-19 07:18:56.000000 daskcheck-0.0.5/daskcheck.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-04-19 07:18:56.000000 daskcheck-0.0.5/daskcheck.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-19 07:18:56.333319 daskcheck-0.0.5/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1168 2023-04-19 07:18:41.000000 daskcheck-0.0.5/setup.py
```

### Comparing `daskcheck-0.0.4/PKG-INFO` & `daskcheck-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: daskcheck
-Version: 0.0.4
-Summary: Automatically created environment for python package
-Home-page: http://gitlab.com/jaromrax/daskcheck
-Author: me
-Author-email: mail@gmail.com
-License: GPL2
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 Project daskcheck
 =================
 
 Help with a simple use of the **dask**
 
 The idea
 --------
@@ -42,20 +31,60 @@
 Launching dask scheduler/workers
 --------------------------------
 
 *Pay attention to correct/compatible libraries on different workers*
 
 ### Environment needed
 
-    to be done
+    export PATH=$PATH:$HOME/.local/bin
+
+    export PYTHONPATH=$HOME/root/lib/
+    export ROOTSYS=$HOME/root
+    export PATH=$ROOTSYS/bin:~/bin:$PATH
+    export LD_LIBRARY_PATH=$ROOTSYS/lib:$ROOTSYS/lib/root:$LD_LIBRARY_PATH
+
+    source $HOME/root/bin/thisroot.sh
+
+    export DISPLAY=:0
+    export DS=$HOME/.dask_server
+    export DSER=`cat $DS`
+    export HOST=`hostname`
+
+    cd /tmp
+
+    if [ -f  "$DS" ]; then
+        echo ... OK $DS exists
+    else
+        echo ... NO $DS exists
+        sleep 5
+        echo ...
+        exit 1
+    fi
+
+    export workers=2
+
+    echo ... I am on $HOST and trying to connect to /$DSER/ one thread per worker
+    dask worker ${DSER}:8786      --nworkers $workers --nthreads 1
 
 ### Launching scheduler
 
 ``` {.bash org-language="sh"}
-dask scheduler --port 8786
+#dask scheduler --port 8786
+export PATH=$PATH:$HOME/.local/bin
+
+export HOST=`hostname`
+
+cd /tmp
+
+if [ "$HOST" = "core6a" ]; then
+    echo ... starting scheduler
+    dask scheduler   --port 8786 #  --bokeh-port 8787
+fi
+sleep 5
+exit 0
 ```
 
 ### Launching worker
 
 ``` {.bash org-language="sh"}
 dask     worker 127.0.0.1:8786 --nworkers 5 --nthreads 1
 ```
@@ -67,14 +96,17 @@
 
 This runs (sched and workers are ON) 40x get~cpuinfo~
 
 ``` {.bash org-language="sh"}
 ./daskcheck.py test
 ```
 
+**In progress ... this worked only inside git project folder with actual
+files...**
+
 This is solved .... possible to load (unload first). See `tesmod.py`
 
 ``` {.bash org-language="sh"}
 ./daskcheck.py dask py_file_with_main  1,3
 ./daskcheck.py dask py_file_with_main  11..33
 ```
 
@@ -124,9 +156,7 @@
     return order, [platform.node(),  f"{time.perf_counter() - start_time:.1f} s" , ni]
 
 
 if __name__=="__main__":
     Fire(main)
 
 ```
-
-
```

### Comparing `daskcheck-0.0.4/daskcheck/config.py` & `daskcheck-0.0.5/daskcheck/config.py`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.4/daskcheck/daskcheck.py` & `daskcheck-0.0.5/daskcheck/daskcheck.py`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.4/daskcheck/unitname.py` & `daskcheck-0.0.5/daskcheck/unitname.py`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.4/daskcheck.egg-info/PKG-INFO` & `daskcheck-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: daskcheck
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automatically created environment for python package
 Home-page: http://gitlab.com/jaromrax/daskcheck
-Author: me
-Author-email: mail@gmail.com
+Author: jaromrax
+Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Project daskcheck
 =================
 
@@ -42,20 +42,60 @@
 Launching dask scheduler/workers
 --------------------------------
 
 *Pay attention to correct/compatible libraries on different workers*
 
 ### Environment needed
 
-    to be done
+    export PATH=$PATH:$HOME/.local/bin
+
+    export PYTHONPATH=$HOME/root/lib/
+    export ROOTSYS=$HOME/root
+    export PATH=$ROOTSYS/bin:~/bin:$PATH
+    export LD_LIBRARY_PATH=$ROOTSYS/lib:$ROOTSYS/lib/root:$LD_LIBRARY_PATH
+
+    source $HOME/root/bin/thisroot.sh
+
+    export DISPLAY=:0
+    export DS=$HOME/.dask_server
+    export DSER=`cat $DS`
+    export HOST=`hostname`
+
+    cd /tmp
+
+    if [ -f  "$DS" ]; then
+        echo ... OK $DS exists
+    else
+        echo ... NO $DS exists
+        sleep 5
+        echo ...
+        exit 1
+    fi
+
+    export workers=2
+
+    echo ... I am on $HOST and trying to connect to /$DSER/ one thread per worker
+    dask worker ${DSER}:8786      --nworkers $workers --nthreads 1
 
 ### Launching scheduler
 
 ``` {.bash org-language="sh"}
-dask scheduler --port 8786
+#dask scheduler --port 8786
+export PATH=$PATH:$HOME/.local/bin
+
+export HOST=`hostname`
+
+cd /tmp
+
+if [ "$HOST" = "core6a" ]; then
+    echo ... starting scheduler
+    dask scheduler   --port 8786 #  --bokeh-port 8787
+fi
+sleep 5
+exit 0
 ```
 
 ### Launching worker
 
 ``` {.bash org-language="sh"}
 dask     worker 127.0.0.1:8786 --nworkers 5 --nthreads 1
 ```
@@ -67,14 +107,17 @@
 
 This runs (sched and workers are ON) 40x get~cpuinfo~
 
 ``` {.bash org-language="sh"}
 ./daskcheck.py test
 ```
 
+**In progress ... this worked only inside git project folder with actual
+files...**
+
 This is solved .... possible to load (unload first). See `tesmod.py`
 
 ``` {.bash org-language="sh"}
 ./daskcheck.py dask py_file_with_main  1,3
 ./daskcheck.py dask py_file_with_main  11..33
 ```
```

### Comparing `daskcheck-0.0.4/setup.py` & `daskcheck-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,19 +20,19 @@
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
 setup(
     name="daskcheck",
     description="Automatically created environment for python package",
-    author="me",
+    author="jaromrax",
     url="http://gitlab.com/jaromrax/daskcheck",
-    author_email="mail@gmail.com",
+    author_email="jaromrax@gmail.com",
     license="GPL2",
     version=get_version("daskcheck/version.py"),
     packages=['daskcheck'],
     package_data={'daskcheck': ['data/*']},
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     scripts = ['bin/daskcheck'],
-    install_requires = ['fire'],
+    install_requires = ['fire','dask'],
 )
```

