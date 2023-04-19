# Comparing `tmp/olallieberry-0.1.0.tar.gz` & `tmp/olallieberry-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olallieberry-0.1.0.tar", max compression
+gzip compressed data, was "olallieberry-1.0.0.tar", max compression
```

## Comparing `olallieberry-0.1.0.tar` & `olallieberry-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-04-19 07:51:00.956525 olallieberry-0.1.0/LICENSE
--rw-r--r--   0        0        0       86 2023-04-19 18:05:20.631492 olallieberry-0.1.0/README.md
--rw-r--r--   0        0        0      369 2023-04-19 18:06:32.156134 olallieberry-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      704 2023-04-19 18:06:22.048049 olallieberry-0.1.0/src/olallieberry/__init__.py
--rw-r--r--   0        0        0     1919 2023-04-19 18:05:33.119610 olallieberry-0.1.0/src/olallieberry/lexer.py
--rw-r--r--   0        0        0     1013 2023-04-19 18:05:37.319650 olallieberry-0.1.0/src/olallieberry/rule.py
--rw-r--r--   0        0        0     1491 2023-04-19 18:05:39.319668 olallieberry-0.1.0/src/olallieberry/token.py
--rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 olallieberry-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-19 07:51:00.956525 olallieberry-1.0.0/LICENSE
+-rw-r--r--   0        0        0       86 2023-04-19 18:16:20.303086 olallieberry-1.0.0/README.md
+-rw-r--r--   0        0        0      369 2023-04-19 18:16:29.767112 olallieberry-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      704 2023-04-19 18:09:02.493228 olallieberry-1.0.0/src/olallieberry/__init__.py
+-rw-r--r--   0        0        0     2052 2023-04-19 18:12:35.254324 olallieberry-1.0.0/src/olallieberry/lexer.py
+-rw-r--r--   0        0        0      993 2023-04-19 18:12:12.718227 olallieberry-1.0.0/src/olallieberry/rule.py
+-rw-r--r--   0        0        0     1478 2023-04-19 18:12:30.426303 olallieberry-1.0.0/src/olallieberry/token.py
+-rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 olallieberry-1.0.0/PKG-INFO
```

### Comparing `olallieberry-0.1.0/LICENSE` & `olallieberry-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `olallieberry-0.1.0/src/olallieberry/__init__.py` & `olallieberry-1.0.0/src/olallieberry/__init__.py`

 * *Files identical despite different names*

### Comparing `olallieberry-0.1.0/src/olallieberry/rule.py` & `olallieberry-1.0.0/src/olallieberry/rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 # limitations under the License.
 """olallieberry Rule"""
 
 from re import Pattern
 
 
 class Rule:
-    """Lexical Rule"""
+    """
+    Lexical Rule
 
-    def __init__(self, __name: str, __pattern: str | Pattern[str]) -> None:
-        """
+    Attributes:
         __name (str): rule name
         __pattern (str | Pattern[str]): rule pattern
-        """
-        self.name = __name
-        self.pattern = __pattern
+    """
+
+    def __init__(self, name: str, pattern: str | Pattern[str]) -> None:
+        self.name = name
+        self.pattern = pattern
 
     def __repr__(self) -> str:
-        """"""
         return f"Rule(name={self.name}, pattern={self.pattern})"
```

### Comparing `olallieberry-0.1.0/src/olallieberry/token.py` & `olallieberry-1.0.0/src/olallieberry/token.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,41 +11,42 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """olallieberry Token"""
 
 
 class Token:
-    """Lexical Token"""
+    """
+    Lexical Token
+
+    Attributes:
+        __name (str): token name
+        __idx (int): token identifier
+        __line (int): token line
+        __column (int): token column
+        __value (str): token value
+    """
 
     def __init__(
         self,
         # fmt: off
         __name: str,
         __idx: int,
         __line: int,
         __column: int,
         __value: str
         # fmt: on
     ) -> None:
-        """
-        __name (str): token name
-        __idx (int): token identifier
-        __line (int): token line 
-        __column (int): token column
-        __value (str): token value
-        """
         self.name = __name
         self.idx = __idx
         self.line = __line
         self.column = __column
         self.value = __value
 
     def __repr__(self) -> str:
-        """"""
         return "Token({name}, {idx}, {line}, {column}, {value})".format(
             name=f"name={self.name}",
             idx=f"idx={self.idx}",
             line=f"line={self.line}",
             column=f"column={self.column}",
             value=f"value={self.value}",
         )
```

