# Comparing `tmp/ezQpy-0.2.0.3-py3-none-any.whl.zip` & `tmp/ezQpy-0.2.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 20820 bytes, number of entries: 13
+Zip file size: 20752 bytes, number of entries: 13
 -rw-r--r--  2.0 unx    47866 b- defN 23-Apr-19 15:20 ezQpy.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 07:56 qasmtoqcis/__init__.py
 -rw-r--r--  2.0 unx     3973 b- defN 23-Apr-19 07:56 qasmtoqcis/const.py
 -rw-r--r--  2.0 unx     7400 b- defN 23-Apr-19 07:56 qasmtoqcis/qasm.py
 -rw-r--r--  2.0 unx    11185 b- defN 23-Apr-19 07:56 qasmtoqcis/qasm_to_qcis.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 07:56 qcistoqasm/__init__.py
 -rw-r--r--  2.0 unx      409 b- defN 23-Apr-19 07:56 qcistoqasm/const.py
 -rw-r--r--  2.0 unx     2612 b- defN 23-Apr-19 07:56 qcistoqasm/qcis.py
 -rw-r--r--  2.0 unx     2216 b- defN 23-Apr-19 07:56 qcistoqasm/qcis_to_qasm.py
--rw-r--r--  2.0 unx     2603 b- defN 23-Apr-19 15:56 ezQpy-0.2.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 15:56 ezQpy-0.2.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-19 15:56 ezQpy-0.2.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      984 b- defN 23-Apr-19 15:56 ezQpy-0.2.0.3.dist-info/RECORD
-13 files, 79368 bytes uncompressed, 19198 bytes compressed:  75.8%
+-rw-r--r--  2.0 unx     2474 b- defN 23-Apr-19 16:12 ezQpy-0.2.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 16:12 ezQpy-0.2.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-19 16:12 ezQpy-0.2.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      984 b- defN 23-Apr-19 16:12 ezQpy-0.2.0.4.dist-info/RECORD
+13 files, 79239 bytes uncompressed, 19130 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: qcistoqasm/qcis.py
 Comment: 
 
 Filename: qcistoqasm/qcis_to_qasm.py
 Comment: 
 
-Filename: ezQpy-0.2.0.3.dist-info/METADATA
+Filename: ezQpy-0.2.0.4.dist-info/METADATA
 Comment: 
 
-Filename: ezQpy-0.2.0.3.dist-info/WHEEL
+Filename: ezQpy-0.2.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: ezQpy-0.2.0.3.dist-info/top_level.txt
+Filename: ezQpy-0.2.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ezQpy-0.2.0.3.dist-info/RECORD
+Filename: ezQpy-0.2.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ezQpy-0.2.0.3.dist-info/METADATA` & `ezQpy-0.2.0.4.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezQpy
-Version: 0.2.0.3
+Version: 0.2.0.4
 Summary: A SDK to use Quantum Computer @ quantumcomputer.ac.cn with QCIS.
 Home-page: https://quantumcomputer.ac.cn
 Author: Code42
 Author-email: support@quantumcomputer.ac.cn
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -16,43 +16,41 @@
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4
 Requires-Dist: numpy
 Requires-Dist: requests
 Requires-Dist: isqmap
 Requires-Dist: sabreMapper
-Requires-Dist: base
-Requires-Dist: qiskit
 
 
-#中科院量子创新院量子计算云平台#
-#新机内测SDK使用说明#
+# 中科院量子创新院量子计算云平台 #
+# 新机内测SDK使用说明 #
 
 
-!!! note "把大象装冰箱里分三步:"
-    ### 1. 把冰箱门打开
-    ### 2. 把大象推进去
-    ### 3. 把冰箱门关上
+把大象装冰箱里分三步:  
+1. 把冰箱门打开
+2. 把大象推进去
+3. 把冰箱门关上
 
-!!! success "运行量子程序也只分三步:"
-    ### 1. 写量子程序(此处必须要省略好几万字)
-    ### 2. 使用Python调用量子计算云平台SDK，将量子线路提交到量子计算机。
-    ### 3. 等待并回读线路运行结果，进行自己的分析使用。
+运行量子程序也只分三步:
+1. 写量子程序(此处必须要省略好几万字)
+2. 使用Python调用量子计算云平台SDK，将量子线路提交到量子计算机。
+3. 等待并回读线路运行结果，进行自己的分析使用。
 
 
-!!! info "中科院量子创新院量子计算云平台, 2023年4月14日开放新机内测，官方网址：[https://quantumcomputer.ac.cn](https://quantumcomputer.ac.cn)"
+中科院量子创新院量子计算云平台, 2023年4月14日开放新机内测，官方网址：[https://quantumcomputer.ac.cn](https://quantumcomputer.ac.cn)
   
-!!! example "如需申请新量子计算机使用权限，可以[参考这里](https://quantumcomputer.ac.cn/Forum/reply/21a180c9fcdd43098303cac6b98adff4/9b6aa8fddaf64925a05f1764fdec011c.html)"
+如需申请新量子计算机使用权限，可以[参考这里](https://quantumcomputer.ac.cn/Forum/reply/21a180c9fcdd43098303cac6b98adff4/9b6aa8fddaf64925a05f1764fdec011c.html)
 
+本地快速安装SDK环境，请使用如下指令：
 ```python title='本地快速安装SDK环境，请使用如下指令：'
 pip install --upgrade ezQpy -i  https://pypi.tuna.tsinghua.edu.cn/simple
 ```
-!!! bug ""
-    因近期内测调整较快，如遇到原有程序运行报错，或无法提交线路等问题，请及时联系官方人员或用以下指令更新SDK库。  
-    同理，近期依赖关系有可能列的不全，用户可以根据报错提示来进行安装。  
-    如遇国内源暂未同步，请强行指定国外原进行更新安装-i  https://pypi.org/simple  
+
+因近期内测调整较快，如遇到原有程序运行报错，或无法提交线路等问题，请及时联系官方人员或用以下指令更新SDK库。  
+同理，近期依赖关系有可能列的不全，用户可以根据报错提示来进行安装。  
+如遇国内源暂未同步，请强行指定国外原进行更新安装-i  https://pypi.org/simple  
   
-!!! tip "在云平台网站提供的jupyternotebook环境Tutorial目录下，可以得到可互动执行的例子程序，复制到个人目录后，可以快速运行。" 
+在云平台网站提供的jupyternotebook环境Tutorial目录下，可以得到可互动执行的例子程序，复制到个人目录后，可以快速运行。
 
-!!! quote ""
-    [本文档](https://docs.quantumcomputer.ac.cn/)仅供2023年4月14日，中科院量子创新院量子计算云平台新量子计算内测，新SDK使用说明查询。  
+[本文档](https://docs.quantumcomputer.ac.cn/)仅供2023年4月14日，中科院量子创新院量子计算云平台新量子计算内测，新SDK使用说明查询。
```

