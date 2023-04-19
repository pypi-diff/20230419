# Comparing `tmp/sara_compis1_tools-0.0.4.tar.gz` & `tmp/sara_compis1_tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sara_compis1_tools-0.0.4.tar", last modified: Sun Apr  9 04:39:15 2023, max compression
+gzip compressed data, was "sara_compis1_tools-0.0.5.tar", last modified: Wed Apr 19 20:42:32 2023, max compression
```

## Comparing `sara_compis1_tools-0.0.4.tar` & `sara_compis1_tools-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 04:39:15.327421 sara_compis1_tools-0.0.4/
--rw-rw-rw-   0        0        0       80 2023-04-09 04:37:57.000000 sara_compis1_tools-0.0.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1065 2023-04-08 22:44:28.000000 sara_compis1_tools-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-04-08 22:41:49.000000 sara_compis1_tools-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      681 2023-04-09 04:39:15.323040 sara_compis1_tools-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-04-08 22:40:09.000000 sara_compis1_tools-0.0.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-09 04:39:15.296522 sara_compis1_tools-0.0.4/sara_compis1_tools/
--rw-rw-rw-   0        0        0     6258 2023-04-09 04:22:00.000000 sara_compis1_tools-0.0.4/sara_compis1_tools/Format.py
--rw-rw-rw-   0        0        0      223 2023-03-07 18:50:14.000000 sara_compis1_tools-0.0.4/sara_compis1_tools/StateAFD.py
--rw-rw-rw-   0        0        0     1559 2023-03-06 05:32:15.000000 sara_compis1_tools-0.0.4/sara_compis1_tools/Syntax.py
--rw-rw-rw-   0        0        0        0 2023-04-08 21:45:17.000000 sara_compis1_tools-0.0.4/sara_compis1_tools/__init__.py
--rw-rw-rw-   0        0        0    19116 2023-04-09 00:32:31.000000 sara_compis1_tools-0.0.4/sara_compis1_tools/directAFD.py
--rw-rw-rw-   0        0        0      381 2023-04-09 03:01:32.000000 sara_compis1_tools-0.0.4/sara_compis1_tools/generated.py
--rw-rw-rw-   0        0        0    12081 2023-04-09 03:53:00.000000 sara_compis1_tools-0.0.4/sara_compis1_tools/lexGen.py
-drwxrwxrwx   0        0        0        0 2023-04-09 04:39:15.319291 sara_compis1_tools-0.0.4/sara_compis1_tools.egg-info/
--rw-rw-rw-   0        0        0      681 2023-04-09 04:39:14.000000 sara_compis1_tools-0.0.4/sara_compis1_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      479 2023-04-09 04:39:15.000000 sara_compis1_tools-0.0.4/sara_compis1_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 04:39:14.000000 sara_compis1_tools-0.0.4/sara_compis1_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-09 04:39:14.000000 sara_compis1_tools-0.0.4/sara_compis1_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-09 04:39:14.000000 sara_compis1_tools-0.0.4/sara_compis1_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 04:39:15.328337 sara_compis1_tools-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-04-09 04:38:08.000000 sara_compis1_tools-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:42:32.712366 sara_compis1_tools-0.0.5/
+-rw-rw-rw-   0        0        0      138 2023-04-19 20:39:04.000000 sara_compis1_tools-0.0.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1059 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      748 2023-04-19 20:42:32.709318 sara_compis1_tools-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 20:42:32.682981 sara_compis1_tools-0.0.5/sara_compis1_tools/
+-rw-rw-rw-   0        0        0     6072 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/Format.py
+-rw-rw-rw-   0        0        0      216 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/StateAFD.py
+-rw-rw-rw-   0        0        0     1502 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/Syntax.py
+-rw-rw-rw-   0        0        0     1167 2023-04-19 20:23:20.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/Visualizer.py
+-rw-rw-rw-   0        0        0        0 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/__init__.py
+-rw-rw-rw-   0        0        0    18584 2023-04-19 20:04:32.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/directAFD.py
+-rw-rw-rw-   0        0        0     1929 2023-04-19 20:29:35.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/generated.py
+-rw-rw-rw-   0        0        0    13324 2023-04-19 20:28:45.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/lexGen.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:42:32.705015 sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/
+-rw-rw-rw-   0        0        0      748 2023-04-19 20:42:32.000000 sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2023-04-19 20:42:32.000000 sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 20:42:32.000000 sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-19 20:42:32.000000 sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-19 20:42:32.000000 sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 20:42:32.713594 sara_compis1_tools-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      766 2023-04-19 20:39:31.000000 sara_compis1_tools-0.0.5/setup.py
+-rw-rw-rw-   0        0        0     1948 2023-04-19 18:13:23.000000 sara_compis1_tools-0.0.5/stateafd_objects.py
```

### Comparing `sara_compis1_tools-0.0.4/LICENSE.txt` & `sara_compis1_tools-0.0.5/LICENSE.txt`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2023 Sara Paguaga
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2023 Sara Paguaga
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `sara_compis1_tools-0.0.4/PKG-INFO` & `sara_compis1_tools-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sara_compis1_tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of tools for the Language Design course
-Home-page: https://github.com/MGonza20/Compis_Lab3
+Home-page: https://github.com/MGonza20/Compis_Lab4
 Author: Sara Paguaga
 Author-email: sara.paguaga@gmail.com
 License: MIT
 Keywords: Compiler
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,7 +17,11 @@
 
 Change Log
 ===========
 
 0.0.4 (08/04/2023)
 ------------------
 - More fixes.
+
+0.0.5 (19/04/2023)
+------------------
+- Rearranging packages.
```

### Comparing `sara_compis1_tools-0.0.4/sara_compis1_tools/Format.py` & `sara_compis1_tools-0.0.5/sara_compis1_tools/Format.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-
-class Format:
-    def __init__(self, regex):
-        self.regex = regex
-        self.sims = {'(': 1, '|': 2, '.': 3, '*': 4, '+': 4, '?': 4}
-
-
-    def prec(self, value):
-        return 5 if value.isalnum() else self.sims[value]
-
-
-    def idempotenciesApp(self):
-        regexStr = self.regex
-        i = 0
-        while i < len(regexStr)-1:
-            if regexStr[i] == regexStr[i+1] and regexStr[i] in "+?":
-                regexStr = regexStr[:i] + regexStr[i+1:]
-            else:
-                i += 1
-        self.regex = regexStr
-
-
-    def positiveId(self, regexx):
-        expression = regexx
-        count_plus = expression.count('+')
-        count_plus_lit = expression.count("'+'")
-        count_t = count_plus - count_plus_lit
-        while count_t > 0:
-
-            count_plus = expression.count('+')
-            count_plus_lit = expression.count("'+'")
-            count_t = count_plus - count_plus_lit
-            
-            for i in range(len(expression)):
-                if expression[i] == '+':
-                    if expression[i-1] == ')':
-                        j = i-2
-                        continuee = True
-                        closeParen = 1
-                        while continuee:
-                            if expression[j] == ')':
-                                closeParen += 1
-                            elif expression[j] == '(':
-                                closeParen -= 1
-                            j -= 1
-                            if closeParen == 0:
-                                continuee = False
-                        expression = f'{expression[:j+1]}{expression[j+1:i]*2}*{expression[i+1:]}'
-
-                    elif expression[i-1].isalnum():
-                        before = expression[:i-1]
-                        after = expression[i+1:]
-                        middle = expression[i-1]*2
-                        expression = f'{before}{middle}*{after}'    
-        return expression
-
-    
-    def zeroOrOneId(self, regexx):
-        expression = regexx
-        count_q = expression.count('?')
-        count_q_lit = expression.count("'?'")
-        count_t = count_q - count_q_lit
-        while count_t > 0:
-
-            count_q = expression.count('?')
-            count_q_lit = expression.count("'?'")
-            count_t = count_q - count_q_lit
-
-            for i in range(len(expression)):
-
-                
-
-                if expression[i] == '?':
-                    if expression[i-1] == ')':
-                        j = i-2
-                        continuee = True
-                        closeParen = 1
-                        while continuee:
-                            if expression[j] == ')':
-                                closeParen += 1
-                            elif expression[j] == '(':
-                                closeParen -= 1
-                            j -= 1
-                            if closeParen == 0:
-                                continuee = False
-                        expression = f'{expression[:j+1]}({expression[j+1:i]}|ε){expression[i+1:]}'
-
-                    elif expression[i-1].isalnum():
-                        before = expression[:i-1]
-                        after = expression[i+1:]
-                        middle = expression[i-1]
-                        expression = f'{before}({middle}|ε){after}' 
-                    elif i-2 >= 0:
-                        ck = expression[i-3:i]
-                        if ck[0] == "'" and ck[-1] == "'":
-                            expression = f'{expression[:i-3]}({ck}|ε){expression[i+1:]}'
-
-                               
-
-                    
-        return expression
-
-
-    def concat(self, regexx):
-        newRegex, ops = "", list(self.sims.keys())
-        ops.remove('(')
-
-        i = 0
-        while i < len(regexx):
-            val = regexx[i]
-            if i + 2 < len(regexx):
-                if regexx[i] == "'" and regexx[i + 2] == "'":
-                    val = regexx[i + 1]
-                    val = str(ord(val))
-                    if len(val) == 2:
-                        val = '0' + val
-                    elif len(val) == 1:
-                        val = '00' + val
-                    i += 2
-                elif val.isalnum() or val in ["#", '_']:
-                    val = str(ord(val))
-                    if len(val) == 2:
-                        val = '0' + val
-                    elif len(val) == 1:
-                        val = '00' + val
-
-            elif regexx[i].isalnum() or regexx[i] in ['#', '_']:
-                val = str(ord(val)) 
-                if len(val) == 2:
-                    val = '0' + val
-                elif len(val) == 1:
-                    val = '00' + val
-                    
-            if i + 1 < len(regexx):
-                val_p1 = regexx[i + 1]
-                newRegex += val
-
-                if val != '(' and val_p1 != ')' and val != '|' and val_p1 not in ops:
-                    newRegex += '.'
-
-            i += 1
-
-        if regexx[-1] == ')' or regexx[-1] in ops:
-            newRegex += regexx[-1]
-        else:
-            if len(str(ord(regexx[-1]))) == 1:
-                newRegex += '00' + str(ord(regexx[-1]))
-            elif len(str(ord(regexx[-1]))) == 2:
-                newRegex += '0' + str(ord(regexx[-1]))
-
-        return newRegex
-
-
-    def infixPostfix(self):
-        postfix, stack = '', []
-        concatRegex = self.concat()
-
-        for value in concatRegex:
-            if value == '(':
-                stack.append(value)
-
-            elif value == ')':
-                while stack[-1] != '(':
-                    postfix += stack.pop()
-                stack.pop()
-
-            else:
-                while stack and self.prec(value) <= self.prec(stack[-1]):
-                    postfix += stack.pop()
-                stack.append(value)
-
-        while stack:
-            postfix += stack.pop()
-        return postfix
-
-
-
-# a = Format("12c++(d|q)??e")
-# a.zeroOrOneSus()
-# a.positiveSus()
-# print(a.regex)
-# a.idempotenciesApp()
-# a.zeroOrOneId()
-# a.positiveId()
-# print(a.infixPostfix())
-# print(a.regex)
+
+class Format:
+    def __init__(self, regex):
+        self.regex = regex
+        self.sims = {'(': 1, '|': 2, '.': 3, '*': 4, '+': 4, '?': 4}
+
+
+    def prec(self, value):
+        return 5 if value.isalnum() else self.sims[value]
+
+
+    def idempotenciesApp(self):
+        regexStr = self.regex
+        i = 0
+        while i < len(regexStr)-1:
+            if regexStr[i] == regexStr[i+1] and regexStr[i] in "+?":
+                regexStr = regexStr[:i] + regexStr[i+1:]
+            else:
+                i += 1
+        self.regex = regexStr
+
+
+    def positiveId(self, regexx):
+        expression = regexx
+        count_plus = expression.count('+')
+        count_plus_lit = expression.count("'+'")
+        count_t = count_plus - count_plus_lit
+        while count_t > 0:
+
+            count_plus = expression.count('+')
+            count_plus_lit = expression.count("'+'")
+            count_t = count_plus - count_plus_lit
+            
+            for i in range(len(expression)):
+                if expression[i] == '+':
+                    if expression[i-1] == ')':
+                        j = i-2
+                        continuee = True
+                        closeParen = 1
+                        while continuee:
+                            if expression[j] == ')':
+                                closeParen += 1
+                            elif expression[j] == '(':
+                                closeParen -= 1
+                            j -= 1
+                            if closeParen == 0:
+                                continuee = False
+                        expression = f'{expression[:j+1]}{expression[j+1:i]*2}*{expression[i+1:]}'
+
+                    elif expression[i-1].isalnum():
+                        before = expression[:i-1]
+                        after = expression[i+1:]
+                        middle = expression[i-1]*2
+                        expression = f'{before}{middle}*{after}'    
+        return expression
+
+    
+    def zeroOrOneId(self, regexx):
+        expression = regexx
+        count_q = expression.count('?')
+        count_q_lit = expression.count("'?'")
+        count_t = count_q - count_q_lit
+        while count_t > 0:
+
+            count_q = expression.count('?')
+            count_q_lit = expression.count("'?'")
+            count_t = count_q - count_q_lit
+
+            for i in range(len(expression)):
+
+                
+
+                if expression[i] == '?':
+                    if expression[i-1] == ')':
+                        j = i-2
+                        continuee = True
+                        closeParen = 1
+                        while continuee:
+                            if expression[j] == ')':
+                                closeParen += 1
+                            elif expression[j] == '(':
+                                closeParen -= 1
+                            j -= 1
+                            if closeParen == 0:
+                                continuee = False
+                        expression = f'{expression[:j+1]}({expression[j+1:i]}|ε){expression[i+1:]}'
+
+                    elif expression[i-1].isalnum():
+                        before = expression[:i-1]
+                        after = expression[i+1:]
+                        middle = expression[i-1]
+                        expression = f'{before}({middle}|ε){after}' 
+                    elif i-2 >= 0:
+                        ck = expression[i-3:i]
+                        if ck[0] == "'" and ck[-1] == "'":
+                            expression = f'{expression[:i-3]}({ck}|ε){expression[i+1:]}'
+
+                               
+
+                    
+        return expression
+
+
+    def concat(self, regexx):
+        newRegex, ops = "", list(self.sims.keys())
+        ops.remove('(')
+
+        i = 0
+        while i < len(regexx):
+            val = regexx[i]
+            if i + 2 < len(regexx):
+                if regexx[i] == "'" and regexx[i + 2] == "'":
+                    val = regexx[i + 1]
+                    val = str(ord(val))
+                    if len(val) == 2:
+                        val = '0' + val
+                    elif len(val) == 1:
+                        val = '00' + val
+                    i += 2
+                elif val.isalnum() or val in ["#", '_']:
+                    val = str(ord(val))
+                    if len(val) == 2:
+                        val = '0' + val
+                    elif len(val) == 1:
+                        val = '00' + val
+
+            elif regexx[i].isalnum() or regexx[i] in ['#', '_']:
+                val = str(ord(val)) 
+                if len(val) == 2:
+                    val = '0' + val
+                elif len(val) == 1:
+                    val = '00' + val
+                    
+            if i + 1 < len(regexx):
+                val_p1 = regexx[i + 1]
+                newRegex += val
+
+                if val != '(' and val_p1 != ')' and val != '|' and val_p1 not in ops:
+                    newRegex += '.'
+
+            i += 1
+
+        if regexx[-1] == ')' or regexx[-1] in ops:
+            newRegex += regexx[-1]
+        else:
+            if len(str(ord(regexx[-1]))) == 1:
+                newRegex += '00' + str(ord(regexx[-1]))
+            elif len(str(ord(regexx[-1]))) == 2:
+                newRegex += '0' + str(ord(regexx[-1]))
+
+        return newRegex
+
+
+    def infixPostfix(self):
+        postfix, stack = '', []
+        concatRegex = self.concat()
+
+        for value in concatRegex:
+            if value == '(':
+                stack.append(value)
+
+            elif value == ')':
+                while stack[-1] != '(':
+                    postfix += stack.pop()
+                stack.pop()
+
+            else:
+                while stack and self.prec(value) <= self.prec(stack[-1]):
+                    postfix += stack.pop()
+                stack.append(value)
+
+        while stack:
+            postfix += stack.pop()
+        return postfix
+
+
+
+# a = Format("12c++(d|q)??e")
+# a.zeroOrOneSus()
+# a.positiveSus()
+# print(a.regex)
+# a.idempotenciesApp()
+# a.zeroOrOneId()
+# a.positiveId()
+# print(a.infixPostfix())
+# print(a.regex)
```

### Comparing `sara_compis1_tools-0.0.4/sara_compis1_tools/directAFD.py` & `sara_compis1_tools-0.0.5/sara_compis1_tools/directAFD.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,533 +1,533 @@
-import os
-import networkx as nx
-from graphviz import Digraph
-
-from Format import Format
-os.environ["PATH"] += os.pathsep + 'C:/Program Files (x86)/Graphviz/bin'    
-from StateAFD import StateAFD
-
-
-class Node:
-    def __init__(self, symbol, parent = None, left = None, right = None, no = None, anulable = False, firstpos = [], lastpos = []):
-        self.symbol = symbol
-        self.parent = parent
-        self.left = left
-        self.right = right
-        self.no = no  
-        self.anulable = anulable
-        self.firstpos = firstpos
-        self.lastpos = lastpos
-
-class npObj:
-    def __init__(self, treeNo, symbol, nextpos = []):
-        self.symbol = symbol
-        self.nextpos = nextpos        
-        self.treeNo = treeNo
-
-
-class AFD:
-    def __init__(self, regex):
-        self.regex = regex
-        self.tree = None
-        self.table = {}
-        self.tableSet = set()
-        self.transitions = {}
-
-    def augmentRegex(self):
-        hashRegex = Format(self.regex + '#')
-        # hashRegex.idempotenciesApp()
-        a = hashRegex.positiveId(self.regex)
-        b = hashRegex.zeroOrOneId(a)
-        return hashRegex.concat(b)
-    
-    def syntaxTree(self):
-        tree = []
-        toDo = []
-        enum = 1
-        regex = self.regex.regex
-        subexpr_stack = [] 
-
-        i = 0
-        while i < len(regex):
-            rrrr = regex[i]
-            if len(toDo) > 0:
-                if toDo[-1] == '|':
-                    if len(tree) > 1:
-                        l = tree.pop(0)
-                        r = tree.pop(0)
-                        newSymU = Node(toDo.pop(), left=l, right=r)
-                        l.parent = newSymU
-                        r.parent = newSymU
-                        tree.append(newSymU)
-                elif toDo[-1] == '.':
-                    if len(tree) > 1:
-                        l = tree.pop(0)
-                        r = tree.pop(0)
-                        newSymC = Node(toDo.pop(), left=l, right=r)
-                        l.parent = newSymC
-                        r.parent = newSymC
-                        tree.append(newSymC)
-            if regex[i].isalnum() or regex[i:i+3] == '035':
-                if i+2+1 < len(regex) and regex[i+2+1] == '*':
-                    if regex[i:i+3] != '949':
-                        alnumNode = Node(regex[i:i+3], no=enum)
-                        kleeneNode = Node(regex[i+2+1], left=alnumNode)
-                        alnumNode.parent = kleeneNode
-                        tree.append(kleeneNode)
-                        enum += 1
-                        i += 2
-                    else:
-                        alnumNode = Node(regex[i:i+3])
-                        kleeneNode = Node(regex[i+2+1], left=alnumNode)
-                        alnumNode.parent = kleeneNode
-                        tree.append(kleeneNode)
-                        i += 2
-                else:
-                    ehh = regex[i:i+3]
-                    if regex[i:i+3] != '949':
-                        alnumNode = Node(regex[i:i+3], no=enum)
-                        tree.append(alnumNode)
-                        enum += 1
-                        i += 2
-                    else:
-                        alnumNode = Node(regex[i:i+3])
-                        tree.append(alnumNode)
-                        i += 2
-            elif regex[i] == '(':
-                subexpr_stack.append(tree)  
-                tree = []  
-            elif regex[i] == ')':
-                if len(subexpr_stack) > 0:
-                    parent_tree = subexpr_stack.pop()  
-                    if len(tree) > 0:
-                        if regex[i+1] == '*':
-                            parent_tree.append(Node(regex[i+1], left=tree[0]))
-                            i += 1
-                        else:
-                            parent_tree.append(tree[0])  
-                    tree = parent_tree  
-            elif regex[i] == '|' or regex[i] == '.':
-                if len(tree) < 2:
-                    toDo.append(regex[i])
-            i += 1
-
-        while toDo and tree:
-            if toDo[-1] == '|':
-                if len(tree) > 1:
-                    l = tree.pop(0)
-                    r = tree.pop(0)
-                    newSymU = Node(toDo.pop(), left=l, right=r)
-                    l.parent = newSymU
-                    r.parent = newSymU
-                    tree.append(newSymU)
-            elif toDo[-1] == '.':
-                if len(tree) > 1:
-                    l = tree.pop(0)
-                    r = tree.pop(0)
-                    newSymC = Node(toDo.pop(), left=l, right=r)
-                    l.parent = newSymC
-                    r.parent = newSymC
-                    tree.append(newSymC)
-        return tree
-    
-
-    def anulable(self, tree):
-        if tree:
-            self.anulable(tree.left)
-            self.anulable(tree.right)
-            if tree.symbol == '949':
-                tree.anulable = True
-            elif tree.symbol.isalnum():
-                tree.anulable = False
-            elif tree.symbol == '|':
-                    tree.anulable = tree.left.anulable or tree.right.anulable
-            elif tree.symbol == '.':
-                    tree.anulable = tree.left.anulable and tree.right.anulable
-            elif tree.symbol == '*':
-                tree.anulable = True
-        return tree
-
-
-    def firstPosMethod(self, tree):
-        if tree:
-            self.firstPosMethod(tree.left)
-            self.firstPosMethod(tree.right)
-            if tree.symbol.isalnum() and tree.no or tree.no == 0 or tree.symbol == '035':
-                tree.firstpos = [tree.no]
-            if tree.symbol == '|':
-                tree.firstpos = tree.left.firstpos + tree.right.firstpos
-            if tree.symbol == '.':
-                if tree.left.anulable:
-                    tree.firstpos = tree.left.firstpos + tree.right.firstpos
-                else:
-                    tree.firstpos = tree.left.firstpos
-            if tree.symbol == '*':
-                tree.firstpos = tree.left.firstpos
-        return tree
-
-
-    def lastPosMethod(self, tree):
-        if tree:
-            self.lastPosMethod(tree.left)
-            self.lastPosMethod(tree.right)
-            if tree.symbol.isalnum() and tree.no or tree.no == 0 or tree.symbol == '035':
-                tree.lastpos = [tree.no]
-            if tree.symbol == '|':
-                tree.lastpos = tree.left.lastpos + tree.right.lastpos
-            if tree.symbol == '.':
-                if tree.right.anulable:
-                    tree.lastpos = tree.left.lastpos + tree.right.lastpos
-                else:
-                    tree.lastpos = tree.right.lastpos
-            if tree.symbol == '*':
-                tree.lastpos = tree.left.lastpos
-        return tree
-    
-
-    def genNextPosDict(self, tree):
-        if tree:
-            self.genNextPosDict(tree.left)
-            self.genNextPosDict(tree.right)
-            if tree.no or tree.no == 0:
-                self.table[tree.no] = {tree.symbol: []}
-
-
-    def genNextPos(self, tree):
-        if tree:
-            self.genNextPos(tree.left)
-            self.genNextPos(tree.right)
-            if tree.symbol == '.':
-                for i in tree.left.lastpos:
-                    for key in self.table[i]:
-                        if tree.right.firstpos not in self.table[i][key]:
-                            self.table[i][key] += tree.right.firstpos
-            if tree.symbol == '*':
-                for i in tree.lastpos:
-                    for key in self.table[i]:
-                        if tree.firstpos not in self.table[i][key]:
-                            self.table[i][key] += tree.firstpos
-        
-
-    def tableToObj(self):
-        for key in self.table:
-            for key2 in self.table[key]:
-                s = key2
-                nP = self.table[key][key2]
-                self.tableSet.add(npObj(treeNo=key, symbol=s, nextpos=nP))
-        return self.tableSet
-        
-
-    def genAFD(self, count_states = 0):
-        table = self.tableSet
-        states = [self.tree.firstpos]
-        toDo = [self.tree.firstpos]
-        newAFD = []
-        acceptState = None
-
-        count = 0
-        while toDo:
-            toDoState = toDo.pop(0)
-            symbols = {} 
-            for elem in toDoState:
-                for elem2 in table:
-                    if elem == elem2.treeNo:
-                        if elem2.symbol != '035':
-                            if elem2.symbol not in symbols:
-                                symbols[elem2.symbol] = set(elem2.nextpos)
-                            else:
-                                symbols[elem2.symbol].update(elem2.nextpos)
-                            if list(symbols[elem2.symbol]) not in states:
-                                states.append(list(symbols[elem2.symbol]))
-                                toDo.append(list(symbols[elem2.symbol]))
-                        else:
-                            acceptState = elem2.treeNo
-            newState = StateAFD(name=toDoState, transitions=symbols)
-            if not count:
-                newState.start = True
-                count += 1
-            newAFD.append(newState)
-
-        for elem in newAFD:
-            if acceptState in elem.name:
-                elem.accepting = True
-        
-        # Changing the name of the states
-        count = count_states
-        for state in newAFD:
-            for st in newAFD:
-                for key, transition in st.transitions.items():
-                    if transition == set(state.name):
-                        st.transitions[key] = chr(65+count)
-            
-            state.name = chr(65+count)
-            count += 1
-
-        return newAFD
-    
-
-    def minimizationAFD(self):
-        # Creando copia del AFD
-        afd = self.genAFD()
-
-        # Unir estados de aceptacion y que no son de aceptacion
-        accepting_states = set(state for state in afd if state.accepting)
-        non_accepting_states = set(state for state in afd if not state.accepting)
-        state_groups = [accepting_states, non_accepting_states]
-
-        # Repetir hasta que no se puedan unir mas estados
-        while True:
-            new_state_groups = []
-            for group in state_groups:
-                # Por cada grupo de estados, agrupar por transiciones
-                transition_groups = {}
-                for state in group:
-                    transition = tuple(sorted(state.transitions.values()))
-                    if transition not in transition_groups:
-                        transition_groups[transition] = set()
-                    transition_groups[transition].add(state)
-
-                # Por cada grupo de transiciones, unir estados
-                for transition_group in transition_groups.values():
-                    if len(transition_group) > 1:
-                        new_state_groups.append(transition_group)
-                    else:
-                        new_state_groups.append({transition_group.pop()})
-
-            # Si ya no se pueden unir mas estados, terminar
-            if len(new_state_groups) == len(state_groups):
-                break
-            state_groups = new_state_groups
-
-        # Crear nuevo AFD
-        statesI = sum(len(group) for group in state_groups)
-        reps = {}
-        for group in state_groups:
-            if len(group) > 1:
-                same = []
-                for element in group:
-                    same.append(element)
-                reps[chr(65+statesI)] = tuple(same)
-                statesI += 1
-
-
-        for replacement, same in reps.items():
-            check = tuple([obj.name for obj in same])
-            checkAccepting = tuple([obj.accepting for obj in same])
-            checkStart = tuple([obj.start for obj in same])
-            for key, state in afd.items():
-                for k, v in state.transitions.items():
-                    if v in check:
-                        state.transitions[k] = replacement
-                if  checkAccepting.count(True) > 0:
-                    if state.name in check:
-                        state.accepting = True
-                if checkStart.count(True) > 0:
-                    if state.name in check:
-                        state.start = True
-                if state.name in check:
-                    state.name = replacement
-
-        miniAFD = {}
-        index = 0
-        for state in afd:
-            if state.name not in [obj.name for obj in miniAFD.values()]:
-                miniAFD[index] = state
-                index += 1
-
-        return miniAFD
-
-
-
-    def draw_afd(self, afd):
-
-        G = nx.MultiDiGraph()
-        for state in afd:
-            node_attrs = {'shape': 'circle'}
-            if state.start:
-                node_attrs.update({'color': 'green', 'style': 'filled'})
-            if state.accepting:
-                node_attrs.update({'peripheries': '2'})
-            G.add_node(str(state.name), **node_attrs)
-
-            for transition, final_dest in state.transitions.items():
-                G.add_node(str(final_dest))
-                G.add_edge(str(state.name), str(final_dest), label=str(chr(int(transition))), dir='forward')
-
-        dot = Digraph()
-        for u, v, data in G.edges(data=True):
-            dot.edge(u, v, label=data['label'], dir=data['dir'])
-        for node in G.nodes:
-            attrs = G.nodes[node]
-            dot.node(node, **attrs)
-
-        dot.attr(rankdir='LR')
-        dot.render('directAFD/directAFD', format='png')
-
-
-    def draw_mini_afd(self):
-        afd = self.minimizationAFD()
-
-        G = nx.MultiGraph()
-        for state in afd.values():
-            if state.start:
-                G.add_node(state.name, color='green', style='filled', shape='circle')
-            if state.accepting:
-                G.add_node(state.name, shape='doublecircle')
-            for k, v in state.transitions.items():
-                if state.start:
-                    G.add_node(state.name, color='green', style='filled', shape='circle')
-                if state.accepting:
-                    G.add_node(state.name, shape='doublecircle')
-                else:
-                    if v != 'estado muerto':
-                        G.add_node(v)
-                if v != 'estado muerto':
-                    G.add_edge(state.name, v, label=k, dir='forward')
-                   
-        dot = Digraph()
-        for u, v, data in G.edges(data=True):
-            dot.edge(u, v, label=data['label'], dir=data['dir'])
-        for node in G.nodes:
-            attrs = G.nodes[node]
-            dot.node(node, **attrs)
-
-        dot.attr(rankdir='LR')
-        dot.render('directAFD/miniDirectAFD', format='png')
-
-
-    
-    def simulateDirectAFD(self, string, afd):
-        current_state = afd[0]
-        for symbol in string:
-            if symbol not in current_state.transitions:
-                return False
-            current_state = [afd[i] for i in range(len(afd)) if afd[i].name == current_state.transitions[symbol]]
-            if not current_state:
-                return False
-            else:
-                current_state = current_state[0]
-        return current_state.accepting
-    
-
-    def simulateMiniAFD(self, string):
-        afd = self.minimizationAFD()
-        current_state = afd[0]
-        for symbol in string:
-            if symbol not in current_state.transitions:
-                return False
-            current_state = [state for key, state in afd.items() if state.name == current_state.transitions[symbol]]
-            if not current_state:
-                return False
-            else:
-                current_state = current_state[0]
-        return current_state.accepting
-
-
-    
-    def generateAFD(self, count_states):
-        st = self.syntaxTree()
-        anulable = self.anulable(st[0])
-        fP = self.firstPosMethod(anulable)
-        lP = self.lastPosMethod(fP)
-        self.tree = lP
-        treeVar = self.tree
-        self.genNextPosDict(treeVar)
-        self.genNextPos(treeVar)
-        self.tableToObj()
-        return self.genAFD(count_states)
-        # self.draw_afd(data)
-
-    
-    def generateMiniAFD(self):
-        st = self.syntaxTree()
-        anulable = self.anulable(st[0])
-        fP = self.firstPosMethod(anulable)
-        lP = self.lastPosMethod(fP)
-        self.tree = lP
-        treeVar = self.tree
-        self.genNextPosDict(treeVar)
-        self.genNextPos(treeVar)
-        self.tableToObj()
-        self.draw_mini_afd()
-
-
-    def simulateDirectAFD_General(self, miniString):
-        st = self.syntaxTree()
-        anulable = self.anulable(st[0])
-        fP = self.firstPosMethod(anulable)
-        lP = self.lastPosMethod(fP)
-        self.tree = lP
-        treeVar = self.tree
-        self.genNextPosDict(treeVar)
-        self.genNextPos(treeVar)
-        self.tableToObj()
-        data = self.genAFD()
-        if self.simulateDirectAFD(miniString, data):
-            print('Simulacion AFD Directo: Cadena aceptada')
-        else:
-            print('Simulacion AFD Directo: Cadena no aceptada')
-
-
-    def simulateMiniAFD_General(self, miniString):
-        st = self.syntaxTree()
-        anulable = self.anulable(st[0])
-        fP = self.firstPosMethod(anulable)
-        lP = self.lastPosMethod(fP)
-        self.tree = lP
-        treeVar = self.tree
-        self.genNextPosDict(treeVar)
-        self.genNextPos(treeVar)
-        self.tableToObj()
-        data = self.genAFD()
-        if self.simulateMiniAFD(miniString):
-            print('Simulacion AFD Minimizado: Cadena aceptada')
-        else:
-            print('Simulacion AFD Minimizado: Cadena no aceptada')
-
-
-        
-        
-    
-
-    def generatelP(self):
-        st = self.syntaxTree()
-        anulable = self.anulable(st[0])
-        fP = self.firstPosMethod(anulable)
-        lP = self.lastPosMethod(fP)
-        return lP
-    
-
-    def defineInitialAndAceptting(self, table, initial, aceptting):
-        for k, v in table.items():
-            if v.positions == initial:
-                v.initial = True
-            if v.positions in aceptting:
-                v.aceptting = True
-        return table
-
-
-
-
-
-    def printVisualTree(self, tree, level=0):
-        if tree:
-            self.printVisualTree(tree.right, level+1)
-            if tree.no or tree.no == 0:
-                print('  '*(level*3) + str(tree.symbol))
-            else:
-                print('  '*(level*3) + str((tree.symbol)))
-            self.printVisualTree(tree.left, level+1)
-
-
-def printPostOrder(tree):
-    if tree:
-        printPostOrder(tree.left)
-        printPostOrder(tree.right)
-        print(tree.symbol)
-
-
-
-# string = '(0|1|2)#'
-# afdd = AFD(string)
-# tree = afdd.syntaxTree()[0]
+import os
+import networkx as nx
+from graphviz import Digraph
+
+from Format import Format
+os.environ["PATH"] += os.pathsep + 'C:/Program Files (x86)/Graphviz/bin'    
+from StateAFD import StateAFD
+
+
+class Node:
+    def __init__(self, symbol, parent = None, left = None, right = None, no = None, anulable = False, firstpos = [], lastpos = []):
+        self.symbol = symbol
+        self.parent = parent
+        self.left = left
+        self.right = right
+        self.no = no  
+        self.anulable = anulable
+        self.firstpos = firstpos
+        self.lastpos = lastpos
+
+class npObj:
+    def __init__(self, treeNo, symbol, nextpos = []):
+        self.symbol = symbol
+        self.nextpos = nextpos        
+        self.treeNo = treeNo
+
+
+class AFD:
+    def __init__(self, regex):
+        self.regex = regex
+        self.tree = None
+        self.table = {}
+        self.tableSet = set()
+        self.transitions = {}
+
+    def augmentRegex(self):
+        hashRegex = Format(self.regex + '#')
+        # hashRegex.idempotenciesApp()
+        a = hashRegex.positiveId(self.regex)
+        b = hashRegex.zeroOrOneId(a)
+        return hashRegex.concat(b)
+    
+    def syntaxTree(self):
+        tree = []
+        toDo = []
+        enum = 1
+        regex = self.regex.regex
+        subexpr_stack = [] 
+
+        i = 0
+        while i < len(regex):
+            rrrr = regex[i]
+            if len(toDo) > 0:
+                if toDo[-1] == '|':
+                    if len(tree) > 1:
+                        l = tree.pop(0)
+                        r = tree.pop(0)
+                        newSymU = Node(toDo.pop(), left=l, right=r)
+                        l.parent = newSymU
+                        r.parent = newSymU
+                        tree.append(newSymU)
+                elif toDo[-1] == '.':
+                    if len(tree) > 1:
+                        l = tree.pop(0)
+                        r = tree.pop(0)
+                        newSymC = Node(toDo.pop(), left=l, right=r)
+                        l.parent = newSymC
+                        r.parent = newSymC
+                        tree.append(newSymC)
+            if regex[i].isalnum() or regex[i:i+3] == '035':
+                if i+2+1 < len(regex) and regex[i+2+1] == '*':
+                    if regex[i:i+3] != '949':
+                        alnumNode = Node(regex[i:i+3], no=enum)
+                        kleeneNode = Node(regex[i+2+1], left=alnumNode)
+                        alnumNode.parent = kleeneNode
+                        tree.append(kleeneNode)
+                        enum += 1
+                        i += 2
+                    else:
+                        alnumNode = Node(regex[i:i+3])
+                        kleeneNode = Node(regex[i+2+1], left=alnumNode)
+                        alnumNode.parent = kleeneNode
+                        tree.append(kleeneNode)
+                        i += 2
+                else:
+                    ehh = regex[i:i+3]
+                    if regex[i:i+3] != '949':
+                        alnumNode = Node(regex[i:i+3], no=enum)
+                        tree.append(alnumNode)
+                        enum += 1
+                        i += 2
+                    else:
+                        alnumNode = Node(regex[i:i+3])
+                        tree.append(alnumNode)
+                        i += 2
+            elif regex[i] == '(':
+                subexpr_stack.append(tree)  
+                tree = []  
+            elif regex[i] == ')':
+                if len(subexpr_stack) > 0:
+                    parent_tree = subexpr_stack.pop()  
+                    if len(tree) > 0:
+                        if regex[i+1] == '*':
+                            parent_tree.append(Node(regex[i+1], left=tree[0]))
+                            i += 1
+                        else:
+                            parent_tree.append(tree[0])  
+                    tree = parent_tree  
+            elif regex[i] == '|' or regex[i] == '.':
+                if len(tree) < 2:
+                    toDo.append(regex[i])
+            i += 1
+
+        while toDo and tree:
+            if toDo[-1] == '|':
+                if len(tree) > 1:
+                    l = tree.pop(0)
+                    r = tree.pop(0)
+                    newSymU = Node(toDo.pop(), left=l, right=r)
+                    l.parent = newSymU
+                    r.parent = newSymU
+                    tree.append(newSymU)
+            elif toDo[-1] == '.':
+                if len(tree) > 1:
+                    l = tree.pop(0)
+                    r = tree.pop(0)
+                    newSymC = Node(toDo.pop(), left=l, right=r)
+                    l.parent = newSymC
+                    r.parent = newSymC
+                    tree.append(newSymC)
+        return tree
+    
+
+    def anulable(self, tree):
+        if tree:
+            self.anulable(tree.left)
+            self.anulable(tree.right)
+            if tree.symbol == '949':
+                tree.anulable = True
+            elif tree.symbol.isalnum():
+                tree.anulable = False
+            elif tree.symbol == '|':
+                    tree.anulable = tree.left.anulable or tree.right.anulable
+            elif tree.symbol == '.':
+                    tree.anulable = tree.left.anulable and tree.right.anulable
+            elif tree.symbol == '*':
+                tree.anulable = True
+        return tree
+
+
+    def firstPosMethod(self, tree):
+        if tree:
+            self.firstPosMethod(tree.left)
+            self.firstPosMethod(tree.right)
+            if tree.symbol.isalnum() and tree.no or tree.no == 0 or tree.symbol == '035':
+                tree.firstpos = [tree.no]
+            if tree.symbol == '|':
+                tree.firstpos = tree.left.firstpos + tree.right.firstpos
+            if tree.symbol == '.':
+                if tree.left.anulable:
+                    tree.firstpos = tree.left.firstpos + tree.right.firstpos
+                else:
+                    tree.firstpos = tree.left.firstpos
+            if tree.symbol == '*':
+                tree.firstpos = tree.left.firstpos
+        return tree
+
+
+    def lastPosMethod(self, tree):
+        if tree:
+            self.lastPosMethod(tree.left)
+            self.lastPosMethod(tree.right)
+            if tree.symbol.isalnum() and tree.no or tree.no == 0 or tree.symbol == '035':
+                tree.lastpos = [tree.no]
+            if tree.symbol == '|':
+                tree.lastpos = tree.left.lastpos + tree.right.lastpos
+            if tree.symbol == '.':
+                if tree.right.anulable:
+                    tree.lastpos = tree.left.lastpos + tree.right.lastpos
+                else:
+                    tree.lastpos = tree.right.lastpos
+            if tree.symbol == '*':
+                tree.lastpos = tree.left.lastpos
+        return tree
+    
+
+    def genNextPosDict(self, tree):
+        if tree:
+            self.genNextPosDict(tree.left)
+            self.genNextPosDict(tree.right)
+            if tree.no or tree.no == 0:
+                self.table[tree.no] = {tree.symbol: []}
+
+
+    def genNextPos(self, tree):
+        if tree:
+            self.genNextPos(tree.left)
+            self.genNextPos(tree.right)
+            if tree.symbol == '.':
+                for i in tree.left.lastpos:
+                    for key in self.table[i]:
+                        if tree.right.firstpos not in self.table[i][key]:
+                            self.table[i][key] += tree.right.firstpos
+            if tree.symbol == '*':
+                for i in tree.lastpos:
+                    for key in self.table[i]:
+                        if tree.firstpos not in self.table[i][key]:
+                            self.table[i][key] += tree.firstpos
+        
+
+    def tableToObj(self):
+        for key in self.table:
+            for key2 in self.table[key]:
+                s = key2
+                nP = self.table[key][key2]
+                self.tableSet.add(npObj(treeNo=key, symbol=s, nextpos=nP))
+        return self.tableSet
+        
+
+    def genAFD(self, count_states = 0):
+        table = self.tableSet
+        states = [self.tree.firstpos]
+        toDo = [self.tree.firstpos]
+        newAFD = []
+        acceptState = None
+
+        count = 0
+        while toDo:
+            toDoState = toDo.pop(0)
+            symbols = {} 
+            for elem in toDoState:
+                for elem2 in table:
+                    if elem == elem2.treeNo:
+                        if elem2.symbol != '035':
+                            if elem2.symbol not in symbols:
+                                symbols[elem2.symbol] = set(elem2.nextpos)
+                            else:
+                                symbols[elem2.symbol].update(elem2.nextpos)
+                            if list(symbols[elem2.symbol]) not in states:
+                                states.append(list(symbols[elem2.symbol]))
+                                toDo.append(list(symbols[elem2.symbol]))
+                        else:
+                            acceptState = elem2.treeNo
+            newState = StateAFD(name=toDoState, transitions=symbols)
+            if not count:
+                newState.start = True
+                count += 1
+            newAFD.append(newState)
+
+        for elem in newAFD:
+            if acceptState in elem.name:
+                elem.accepting = True
+        
+        # Changing the name of the states
+        count = count_states
+        for state in newAFD:
+            for st in newAFD:
+                for key, transition in st.transitions.items():
+                    if transition == set(state.name):
+                        st.transitions[key] = chr(65+count)
+            
+            state.name = chr(65+count)
+            count += 1
+
+        return newAFD
+    
+
+    def minimizationAFD(self):
+        # Creando copia del AFD
+        afd = self.genAFD()
+
+        # Unir estados de aceptacion y que no son de aceptacion
+        accepting_states = set(state for state in afd if state.accepting)
+        non_accepting_states = set(state for state in afd if not state.accepting)
+        state_groups = [accepting_states, non_accepting_states]
+
+        # Repetir hasta que no se puedan unir mas estados
+        while True:
+            new_state_groups = []
+            for group in state_groups:
+                # Por cada grupo de estados, agrupar por transiciones
+                transition_groups = {}
+                for state in group:
+                    transition = tuple(sorted(state.transitions.values()))
+                    if transition not in transition_groups:
+                        transition_groups[transition] = set()
+                    transition_groups[transition].add(state)
+
+                # Por cada grupo de transiciones, unir estados
+                for transition_group in transition_groups.values():
+                    if len(transition_group) > 1:
+                        new_state_groups.append(transition_group)
+                    else:
+                        new_state_groups.append({transition_group.pop()})
+
+            # Si ya no se pueden unir mas estados, terminar
+            if len(new_state_groups) == len(state_groups):
+                break
+            state_groups = new_state_groups
+
+        # Crear nuevo AFD
+        statesI = sum(len(group) for group in state_groups)
+        reps = {}
+        for group in state_groups:
+            if len(group) > 1:
+                same = []
+                for element in group:
+                    same.append(element)
+                reps[chr(65+statesI)] = tuple(same)
+                statesI += 1
+
+
+        for replacement, same in reps.items():
+            check = tuple([obj.name for obj in same])
+            checkAccepting = tuple([obj.accepting for obj in same])
+            checkStart = tuple([obj.start for obj in same])
+            for key, state in afd.items():
+                for k, v in state.transitions.items():
+                    if v in check:
+                        state.transitions[k] = replacement
+                if  checkAccepting.count(True) > 0:
+                    if state.name in check:
+                        state.accepting = True
+                if checkStart.count(True) > 0:
+                    if state.name in check:
+                        state.start = True
+                if state.name in check:
+                    state.name = replacement
+
+        miniAFD = {}
+        index = 0
+        for state in afd:
+            if state.name not in [obj.name for obj in miniAFD.values()]:
+                miniAFD[index] = state
+                index += 1
+
+        return miniAFD
+
+
+
+    def draw_afd(self, afd):
+
+        G = nx.MultiDiGraph()
+        for state in afd:
+            node_attrs = {'shape': 'circle'}
+            if state.start:
+                node_attrs.update({'color': 'green', 'style': 'filled'})
+            if state.accepting:
+                node_attrs.update({'peripheries': '2'})
+            G.add_node(str(state.name), **node_attrs)
+
+            for transition, final_dest in state.transitions.items():
+                G.add_node(str(final_dest))
+                G.add_edge(str(state.name), str(final_dest), label=str(chr(int(transition))), dir='forward')
+
+        dot = Digraph()
+        for u, v, data in G.edges(data=True):
+            dot.edge(u, v, label=data['label'], dir=data['dir'])
+        for node in G.nodes:
+            attrs = G.nodes[node]
+            dot.node(node, **attrs)
+
+        dot.attr(rankdir='LR')
+        dot.render('directAFD/directAFD', format='png')
+
+
+    def draw_mini_afd(self):
+        afd = self.minimizationAFD()
+
+        G = nx.MultiGraph()
+        for state in afd.values():
+            if state.start:
+                G.add_node(state.name, color='green', style='filled', shape='circle')
+            if state.accepting:
+                G.add_node(state.name, shape='doublecircle')
+            for k, v in state.transitions.items():
+                if state.start:
+                    G.add_node(state.name, color='green', style='filled', shape='circle')
+                if state.accepting:
+                    G.add_node(state.name, shape='doublecircle')
+                else:
+                    if v != 'estado muerto':
+                        G.add_node(v)
+                if v != 'estado muerto':
+                    G.add_edge(state.name, v, label=k, dir='forward')
+                   
+        dot = Digraph()
+        for u, v, data in G.edges(data=True):
+            dot.edge(u, v, label=data['label'], dir=data['dir'])
+        for node in G.nodes:
+            attrs = G.nodes[node]
+            dot.node(node, **attrs)
+
+        dot.attr(rankdir='LR')
+        dot.render('directAFD/miniDirectAFD', format='png')
+
+
+    
+    def simulateDirectAFD(self, string, afd):
+        current_state = afd[0]
+        for symbol in string:
+            if symbol not in current_state.transitions:
+                return False
+            current_state = [afd[i] for i in range(len(afd)) if afd[i].name == current_state.transitions[symbol]]
+            if not current_state:
+                return False
+            else:
+                current_state = current_state[0]
+        return current_state.accepting
+    
+
+    def simulateMiniAFD(self, string):
+        afd = self.minimizationAFD()
+        current_state = afd[0]
+        for symbol in string:
+            if symbol not in current_state.transitions:
+                return False
+            current_state = [state for key, state in afd.items() if state.name == current_state.transitions[symbol]]
+            if not current_state:
+                return False
+            else:
+                current_state = current_state[0]
+        return current_state.accepting
+
+
+    
+    def generateAFD(self, count_states):
+        st = self.syntaxTree()
+        anulable = self.anulable(st[0])
+        fP = self.firstPosMethod(anulable)
+        lP = self.lastPosMethod(fP)
+        self.tree = lP
+        treeVar = self.tree
+        self.genNextPosDict(treeVar)
+        self.genNextPos(treeVar)
+        self.tableToObj()
+        return self.genAFD(count_states)
+        # self.draw_afd(data)
+
+    
+    def generateMiniAFD(self):
+        st = self.syntaxTree()
+        anulable = self.anulable(st[0])
+        fP = self.firstPosMethod(anulable)
+        lP = self.lastPosMethod(fP)
+        self.tree = lP
+        treeVar = self.tree
+        self.genNextPosDict(treeVar)
+        self.genNextPos(treeVar)
+        self.tableToObj()
+        self.draw_mini_afd()
+
+
+    def simulateDirectAFD_General(self, miniString):
+        st = self.syntaxTree()
+        anulable = self.anulable(st[0])
+        fP = self.firstPosMethod(anulable)
+        lP = self.lastPosMethod(fP)
+        self.tree = lP
+        treeVar = self.tree
+        self.genNextPosDict(treeVar)
+        self.genNextPos(treeVar)
+        self.tableToObj()
+        data = self.genAFD()
+        if self.simulateDirectAFD(miniString, data):
+            print('Simulacion AFD Directo: Cadena aceptada')
+        else:
+            print('Simulacion AFD Directo: Cadena no aceptada')
+
+
+    def simulateMiniAFD_General(self, miniString):
+        st = self.syntaxTree()
+        anulable = self.anulable(st[0])
+        fP = self.firstPosMethod(anulable)
+        lP = self.lastPosMethod(fP)
+        self.tree = lP
+        treeVar = self.tree
+        self.genNextPosDict(treeVar)
+        self.genNextPos(treeVar)
+        self.tableToObj()
+        data = self.genAFD()
+        if self.simulateMiniAFD(miniString):
+            print('Simulacion AFD Minimizado: Cadena aceptada')
+        else:
+            print('Simulacion AFD Minimizado: Cadena no aceptada')
+
+
+        
+        
+    
+
+    def generatelP(self):
+        st = self.syntaxTree()
+        anulable = self.anulable(st[0])
+        fP = self.firstPosMethod(anulable)
+        lP = self.lastPosMethod(fP)
+        return lP
+    
+
+    def defineInitialAndAceptting(self, table, initial, aceptting):
+        for k, v in table.items():
+            if v.positions == initial:
+                v.initial = True
+            if v.positions in aceptting:
+                v.aceptting = True
+        return table
+
+
+
+
+
+    def printVisualTree(self, tree, level=0):
+        if tree:
+            self.printVisualTree(tree.right, level+1)
+            if tree.no or tree.no == 0:
+                print('  '*(level*3) + str(tree.symbol))
+            else:
+                print('  '*(level*3) + str((tree.symbol)))
+            self.printVisualTree(tree.left, level+1)
+
+
+def printPostOrder(tree):
+    if tree:
+        printPostOrder(tree.left)
+        printPostOrder(tree.right)
+        print(tree.symbol)
+
+
+
+# string = '(0|1|2)#'
+# afdd = AFD(string)
+# tree = afdd.syntaxTree()[0]
 # afdd.generateAFD()
```

### Comparing `sara_compis1_tools-0.0.4/sara_compis1_tools/lexGen.py` & `sara_compis1_tools-0.0.5/sara_compis1_tools/lexGen.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from Format import Format
 from directAFD import AFD
 from StateAFD import StateAFD
 
-import networkx as nx
-from graphviz import Digraph
 import sys
 
 
 class Token:
         def __init__(self, name):
             self.name = name
             self.regex = None
@@ -49,35 +47,115 @@
 
         lines = [line.encode('utf-8').decode('unicode_escape') for line in lines]
 
         lines_with_n = [n[:-1] for n in lines]
         check_comments = [lll.split(' ') for lll in lines_with_n]  
 
         joined = [' '.join(line) for line in check_comments]
-        for lj in joined:
-            if '(*' in lj and '*)' not in lj:
-                raise Exception("Error en comentario, linea "+ str(joined.index(lj)+1))
-            elif '(*' not in lj and '*)' in lj:
-                raise Exception("Error en comentario, linea "+ str(joined.index(lj)+1))
-
-        for i in range(len(check_comments)):
-            if 'let' in check_comments[i] and len(check_comments[i]) > 4:
-                if check_comments[i][3][-1] == ']' or check_comments[i][3][-1] == ')': 
-                    if check_comments[i][4] == '(*' and check_comments[i][-1] == '*)':
-                        left_idx = check_comments[i].index('(*')
-                        right_idx = check_comments[i].index('*)')
-                        check_comments[i] = check_comments[i][:left_idx] + check_comments[i][right_idx + 1:]
+        # Revision de errores en comentarios
+        for line_no, lj in enumerate(joined, start=1):
+            comments_stack = []
+            for i in range(len(lj) - 1):
+
+                current_next = lj[i:i+2]
+                if current_next == '(*':
+                    comments_stack.append(current_next)
+                elif current_next == '*)':
+                    if comments_stack and comments_stack[-1] == '(*':
+                        comments_stack.pop()
+                    else:
+                        raise Exception(f"Error en comentario, linea {line_no}")
+            if comments_stack:
+                raise Exception(f"Error en comentario, linea {line_no}")
+
+
+        for index, line in enumerate(joined):
+            line_wo_comment = ''
+            i = 0
+            while i < len(line):
+                if i < len(line) - 1 and line[i] == '(' and line[i + 1] == '*':
+                    while i < len(line) - 1 and (line[i] != '*' or line[i + 1] != ')'):
+                        i += 1
+                    i += 2
+                else:
+                    line_wo_comment += line[i]
+                    i += 1
+            joined[index] = line_wo_comment
             
-        lines_c = [' '.join(line) for line in check_comments]
-        return self.remove_spaces(lines_c)  
+
+        return (self.remove_spaces(joined), joined)
+    
+
+    def special_split(self, text, delimiter):
+        result = []
+        start = 0
+        open_curly_b = 0
+
+        for index, char in enumerate(text):
+            if char == '{':
+                open_curly_b += 1
+            elif char == '}':
+                open_curly_b -= 1
+
+            elif char == delimiter and not open_curly_b:
+                result.append(text[start:index])
+                start = index + 1
+
+        result.append(text[start:])
+        return result
+    
+
+    def remove_spaces_list(self, lines):
+        for line in lines:
+            if not all(element == '' for element in line):
+                while '' in line:
+                    for element in line:
+                        if element == '':
+                            line.pop(line.index(element))
         return lines
+    
+
+    def assign_values(self):
+        splits = [self.special_split(line, ' ') for line in self.getLines()[1]]
+        splits = self.remove_spaces_list(splits)
+        
+        start = 0
+        for indx, line in enumerate(splits):
+            if line[0] == 'rule':
+                start = indx + 1
+        
+        if start:
+            rules = ''.join([''.join([word.replace('\t', '') for word in line]) for line in splits[start:]]).split('|')
+            rules_dict = {}
+            for rule in rules:
+                name = ''
+                value = ''
+                inside = False
+
+                for i in range(len(rule)):
+                    if rule[i] == '{':
+                        inside = True
+                        continue
+
+                    if rule[i] == '}':
+                        inside = False
+                        continue
+
+                    if not inside:
+                        name += rule[i]
+                    else:
+                        value += rule[i]
+
+                if name:
+                    name = name[1:-1] if name[0] == "'" and name[-1] == "'" else name 
+                    rules_dict[name] = value.strip()
 
 
     def getTokens(self):
-        lines = self.getLines()
+        lines = self.getLines()[0]
         for line_no, line in enumerate(lines, start=1):
             # generando tokens
             if line[:3] == 'let':
                 name, regex = line[3:].split('=')
                 token = Token(name)
                 token.regex = regex
                 token.line_no = line_no
@@ -228,42 +306,14 @@
                     output += content
                 
             else:
                 output += token[i]
                 i += 1
         return output
 
-    def draw_mega_afd(self, afd):
-
-        G = nx.MultiDiGraph()
-        for state in afd:
-            node_attrs = {'shape': 'circle'}
-            if state.start:
-                node_attrs.update({'color': 'green', 'style': 'filled'})
-            if state.accepting:
-                node_attrs.update({'peripheries': '2'})
-            G.add_node(str(state.name), **node_attrs)
-
-            for transition, final_dest in state.transitions.items():
-                G.add_node(str(final_dest))
-                
-                if int(transition) not in [el for el in range(0, 35)]:
-                    transition = str(chr(int(transition)))
-
-                G.add_edge(str(state.name), str(final_dest), label=transition, dir='forward')    
-
-        dot = Digraph()
-        for u, v, data in G.edges(data=True):
-            dot.edge(u, v, label=data['label'], dir=data['dir'])
-        for node in G.nodes:
-            attrs = G.nodes[node]
-            dot.node(node, **attrs)
-
-        dot.render('mega/megaautomata', format='png')
-
     
     def generate_automatas(self):
         mega_content = []
         count = 0
         for token in self.tokens:
             ff = Format(token.regex)
             token.regex = ff.positiveId(token.regex + '#')
@@ -288,49 +338,43 @@
                     init_state.transitions['949'] = state.name
                     stack.append(init_state)
                 stack.append(state)
         return stack
     
 
     def read(self):
+        self.assign_values()
         self.getTokens()
         self.change_range_format()
         self.surround_dot()
         self.replace_tokens()
     
 
 
     
 if __name__ == '__main__':
 
-    # if len(sys.argv) < 2:
-    #     print("Por favor ingrese el archivo .yal")
-    #     sys.exit(1)
+    if len(sys.argv) < 2:
+        print("Por favor ingrese el archivo .yal")
+        sys.exit(1)
 
-    yal_file = 'sara_compis1_tools/lexer.yal'
-    # yal_file = sys.argv[1]
+    yal_file = sys.argv[1]
     lexer = Lexer(yal_file)
     
     lexer.read()
     mega_content = lexer.generate_automatas()
     mega_automata = lexer.unify(mega_content)
-    lexer.draw_mega_afd(mega_automata)
-
-#     script_content = '''
-# import sys
-# import sara_compis1_tools.readLex as tool
-
-# if len(sys.argv) < 2:
-#     print("Por favor ingrese el archivo .yal")
-#     sys.exit(1)
-
-# yal_file = sys.argv[1]
-# lex_var = tool.Lexer(yal_file)
-# lex_var.read()
-# mega_content = lex_var.generate_automatas()
-# mega_automata = lex_var.unify(mega_content)
-# lex_var.draw_mega_afd(mega_automata)
-#     '''
 
-#     with open('generated.py', 'w') as script_file:
-#         script_file.write(script_content)
+    with open('generated.py', 'w') as file:
+        file.write("from StateAFD import StateAFD\n")
+        file.write("from Visualizer import Visualizer\n\n")
+        file.write("mega = [")
+        for i, obj in enumerate(mega_automata):
+            file.write(f"StateAFD(name='{obj.name}',transitions={obj.transitions},accepting={obj.accepting},start={obj.start})")
+            if i != len(mega_automata) - 1:
+                file.write(",") 
+        file.write("]\n\n")
+
+        file.write("visual = Visualizer()\n")
+        file.write("visual.draw_mega_afd(mega)")
+
```

### Comparing `sara_compis1_tools-0.0.4/sara_compis1_tools.egg-info/PKG-INFO` & `sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sara-compis1-tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of tools for the Language Design course
-Home-page: https://github.com/MGonza20/Compis_Lab3
+Home-page: https://github.com/MGonza20/Compis_Lab4
 Author: Sara Paguaga
 Author-email: sara.paguaga@gmail.com
 License: MIT
 Keywords: Compiler
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,7 +17,11 @@
 
 Change Log
 ===========
 
 0.0.4 (08/04/2023)
 ------------------
 - More fixes.
+
+0.0.5 (19/04/2023)
+------------------
+- Rearranging packages.
```

### Comparing `sara_compis1_tools-0.0.4/setup.py` & `sara_compis1_tools-0.0.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='sara_compis1_tools',
-    version='0.0.4',
-    description='A collection of tools for the Language Design course',
-    long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
-    url='https://github.com/MGonza20/Compis_Lab3',
-    author='Sara Paguaga',
-    author_email='sara.paguaga@gmail.com',
-    license='MIT',
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3'
-    ],
-    keywords='Compiler',
-    packages=find_packages(),
-    include_package_data=True,
-    install_requires=[
-        'networkx',
-        'graphviz'
-    ]
+from setuptools import setup, find_packages
+
+setup(
+    name='sara_compis1_tools',
+    version='0.0.5',
+    description='A collection of tools for the Language Design course',
+    long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
+    url='https://github.com/MGonza20/Compis_Lab4',
+    author='Sara Paguaga',
+    author_email='sara.paguaga@gmail.com',
+    license='MIT',
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3'
+    ],
+    keywords='Compiler',
+    packages=find_packages(),
+    include_package_data=True,
+    install_requires=[
+        'networkx',
+        'graphviz'
+    ]
 )
```

