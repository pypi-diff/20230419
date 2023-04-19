# Comparing `tmp/wtfl-1.0.5.tar.gz` & `tmp/wtfl-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtfl-1.0.5.tar", max compression
+gzip compressed data, was "wtfl-1.1.0.tar", max compression
```

## Comparing `wtfl-1.0.5.tar` & `wtfl-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-04-18 11:53:10.252805 wtfl-1.0.5/LICENSE
--rw-r--r--   0        0        0     8724 2023-04-18 11:53:10.252805 wtfl-1.0.5/README.md
--rw-r--r--   0        0        0      578 2023-04-18 11:53:10.252805 wtfl-1.0.5/pyproject.toml
--rw-r--r--   0        0        0       98 2023-04-18 11:53:10.252805 wtfl-1.0.5/wtfl/__init__.py
--rw-r--r--   0        0        0     4606 2023-04-18 11:53:10.252805 wtfl-1.0.5/wtfl/grammar.py
--rw-r--r--   0        0        0     2720 2023-04-18 11:53:10.252805 wtfl-1.0.5/wtfl/internal_types.py
--rw-r--r--   0        0        0     4519 2023-04-18 11:53:10.252805 wtfl-1.0.5/wtfl/parser.py
--rw-r--r--   0        0        0     6099 2023-04-18 11:53:10.252805 wtfl-1.0.5/wtfl/reader.py
--rw-r--r--   0        0        0     1798 2023-04-18 11:53:10.252805 wtfl-1.0.5/wtfl/writer.py
--rw-r--r--   0        0        0     9563 1970-01-01 00:00:00.000000 wtfl-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-19 04:40:07.624410 wtfl-1.1.0/LICENSE
+-rw-r--r--   0        0        0     9891 2023-04-19 04:40:07.624410 wtfl-1.1.0/README.md
+-rw-r--r--   0        0        0      578 2023-04-19 04:40:07.624410 wtfl-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-04-19 04:40:07.624410 wtfl-1.1.0/wtfl/__init__.py
+-rw-r--r--   0        0        0     5035 2023-04-19 04:40:07.624410 wtfl-1.1.0/wtfl/grammar.py
+-rw-r--r--   0        0        0     2789 2023-04-19 04:40:07.624410 wtfl-1.1.0/wtfl/internal_types.py
+-rw-r--r--   0        0        0     6190 2023-04-19 04:40:07.624410 wtfl-1.1.0/wtfl/parser.py
+-rw-r--r--   0        0        0     6899 2023-04-19 04:40:07.624410 wtfl-1.1.0/wtfl/reader.py
+-rw-r--r--   0        0        0     4557 2023-04-19 04:40:07.624410 wtfl-1.1.0/wtfl/writer.py
+-rw-r--r--   0        0        0    10730 1970-01-01 00:00:00.000000 wtfl-1.1.0/PKG-INFO
```

### Comparing `wtfl-1.0.5/LICENSE` & `wtfl-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wtfl-1.0.5/README.md` & `wtfl-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# WTFL — Well-Designed Text-based Friendly Language
+# WTFL — Well-designed Text-based Friendly Language
 
 This is a spec for a very well-designed declarative language and a Python package to work with it.    
 Obviously, current solutions for config et al. (JSON, YAML, TOML) are very unsuitable as software development progress is going on, so here I propose a brand new format.   
 
 WTFL has all the features of its predecessors, and much more, with a very well-designed friendly syntax.
 
 It is case-insensitive, obvious and feature-rich language.
@@ -28,35 +28,67 @@
 }
 ```
 
 # Package
 
 Package's API is similar to built-in `json`:
 
-- `wtfl.loads(str)` reads an object from a string
-- `wtfl.load(file)` reads an object from a file
-- `wtfl.dumps(obj)` dumps an object into a string
-- `wtfl.dump(file, obj)` dumps an object into a file
+read an object from a string:
+```python
+def wtfl.loads(
+    s, # string to load
+    *,
+    parse_float, # function for float parsing, `float` used by default
+    parse_int, # function for integer parsing (only unprefixed decimal), `int` used by default
+    parse_roman, # function for roman numerals parsing, accepts whole literal as a string (0r...)
+    parse_numbers, # function for integer literals parsing (0b..., 0o..., and so on)
+) -> 
+```
+read an object from a file (same argument meaning as `.loads`):
+`wtfl.load(file, *, parse_float, parse_int, parse_roman, parse_numbers)` 
 
-Current reader and writer are fairly simple, later versions would probably improve configurability
+dump an object into a string:
+```python
+def wtfl.dumps(
+    obj: object, # object to dump
+    *,
+    # if True, non-serializable keys / values are skipped
+    skipkeys: bool = False, 
+    
+    # if True, encodes non-ASCII characters
+    ensure_ascii: bool = True, 
+    
+    # if a non-negative integer, used as indent size. if a string, used as indent character. If None, everything is inlined
+    indent: int | str | None = 2, 
+    
+    # a function that is used to recover from serialization errors. 
+    # if current value is not serializable and skipkeys=False, tries to serialize the result of default(value)
+    default: Callable[[object], str] | None = None, 
+    
+    # if True, sorts object keys
+    sort_keys: bool = False,
+)
+```
+dump an object into a file (same argument meaning as `.dumps()`):
+`wtfl.dump(file, obj, *, skipkeys, ensure_ascii, indent, default, sort_keys)`
 
 # Reserved keywords
 
 It is very important to know all the keywords of WTFL, since all those keywords are important.    
 
 Here's a list (keywords in the same list entry are equivalent and used interchangeably in the spec):
 
 - `is` / `are` / `'s` / `'re` / `do` / `does` / `be`
 - `isn't` / `aren't` / `'sn't` / `'ren't`
 - `of`
 - `also` / `and also` / `but also`
 - `that` / `this` / `these` / `those`
 - `there`
 - `have` / `has` / `'ve`
-- `haven't` / `hasn't` / `'ve'n't`
+- `haven't` / `hasn't` / `'ven't`
 - `can`
 - `cannot` / `can't`
 - `true` / `falsen't`
 - `false` / `truen't`
 - `and`
 - `return`
 - `skip`
```

### Comparing `wtfl-1.0.5/pyproject.toml` & `wtfl-1.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "wtfl"
-version = "1.0.5"
-description = "Well-Designed Text-based Friendly Language"
+version = "1.1.0"
+description = "Well-designed Text-based Friendly Language"
 authors = ["Dmitry Gritsenko <k01419q45@ya.ru>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/evtn/wtfl"
 homepage = "https://github.com/evtn/wtfl"
 keywords = ["markup", "config"]
```

### Comparing `wtfl-1.0.5/wtfl/internal_types.py` & `wtfl-1.1.0/wtfl/internal_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,16 @@
     def __init__(self, pairs: List[Assign]):
         self.pairs = pairs
 
     def __repr__(self):
         return f'[{",".join(map(repr, self.pairs))}]'
 
     def flatten_paths(self, prefix: KeyChain) -> List[Assign]:
+        if not self.pairs:
+            return [Assign(prefix, self)]
         new_pairs = []
         for pair in self.pairs:
             new_pairs.extend(pair.unwind(prefix))
         return new_pairs
 
 
 _T_co = TypeVar("_T_co", covariant=True)
```

### Comparing `wtfl-1.0.5/wtfl/reader.py` & `wtfl-1.1.0/wtfl/reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,21 +6,22 @@
     Constraint,
     KeyChain,
     Object,
     Operation,
     SupportsRead,
     Value,
 )
-from .parser import parse, Assign
 
 StateValue = Union[str, float, bool, None, "Store"]
 PythonValue = Union[
     str, float, bool, None, Dict[str, "PythonValue"], List["PythonValue"]
 ]
 
+from .parser import ParseFunc, ParseFuncs, parse, Assign
+
 
 class Store:
     def __init__(self) -> None:
         self.keys: Dict[str, StateValue] = {}
         self.is_array: bool = False
         self.can_be_array: bool = True
 
@@ -113,14 +114,19 @@
         return store
 
     def assign_path(self, path: KeyChain, value: Value):
         store: Store = self.create_path(path[:-1])
 
         last_key = path[-1]
 
+        if isinstance(value, Object):
+            if not value.pairs:
+                store[last_key] = Store()
+                return
+
         assert not isinstance(value, Object)
 
         store[last_key] = value
 
     def resolve_path(self, path: KeyChain) -> Store | None:
         store = self.keys
 
@@ -171,17 +177,21 @@
         self.assign_path(op.key, op.value)
 
     def to_dict(self) -> PythonValue:
         return self.keys.to_python_value()
 
 
 class Reader:
-    def read(self, s: str) -> ReadState:
+    def read(
+        self,
+        s: str,
+        parse_funcs: ParseFuncs,
+    ) -> ReadState:
         state = ReadState()
-        tree = parse(s.lower())
+        tree = parse(s, parse_funcs)
 
         statements: List[Tuple[Operation, int]] = []
 
         for i, operation in enumerate(tree):
             statements.extend((op, i) for op in self.process_operation(operation))
 
         def key_func(statement: Tuple[Operation, int]) -> float:
@@ -207,14 +217,36 @@
     def apply_operation(self, operation: Operation, state: ReadState):
         if isinstance(operation, Assign):
             state.assign(operation)
         if isinstance(operation, Constraint):
             state.add_constraint(operation)
 
 
-def loads(s: str) -> PythonValue:
-    state: ReadState = Reader().read(s)
+def loads(
+    s: str,
+    *,
+    parse_float: ParseFunc | None = None,
+    parse_int: ParseFunc | None = None,
+    parse_roman: ParseFunc | None = None,
+    parse_numbers: ParseFunc | None = None,
+) -> PythonValue:
+    state: ReadState = Reader().read(
+        s, (parse_float, parse_int, parse_roman, parse_numbers)
+    )
     return state.to_dict()
 
 
-def load(file: SupportsRead[str]) -> PythonValue:
-    return loads(file.read())
+def load(
+    file: SupportsRead[str],
+    *,
+    parse_float: ParseFunc | None = None,
+    parse_int: ParseFunc | None = None,
+    parse_roman: ParseFunc | None = None,
+    parse_numbers: ParseFunc | None = None,
+) -> PythonValue:
+    return loads(
+        file.read(),
+        parse_float=parse_float,
+        parse_int=parse_int,
+        parse_roman=parse_roman,
+        parse_numbers=parse_numbers,
+    )
```

### Comparing `wtfl-1.0.5/PKG-INFO` & `wtfl-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wtfl
-Version: 1.0.5
-Summary: Well-Designed Text-based Friendly Language
+Version: 1.1.0
+Summary: Well-designed Text-based Friendly Language
 Home-page: https://github.com/evtn/wtfl
 License: MIT
 Keywords: markup,config
 Author: Dmitry Gritsenko
 Author-email: k01419q45@ya.ru
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lark (>=1.1.5,<2.0.0)
 Requires-Dist: lark-dynamic (>=1.0.4,<2.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/evtn/wtfl
 Description-Content-Type: text/markdown
 
-# WTFL — Well-Designed Text-based Friendly Language
+# WTFL — Well-designed Text-based Friendly Language
 
 This is a spec for a very well-designed declarative language and a Python package to work with it.    
 Obviously, current solutions for config et al. (JSON, YAML, TOML) are very unsuitable as software development progress is going on, so here I propose a brand new format.   
 
 WTFL has all the features of its predecessors, and much more, with a very well-designed friendly syntax.
 
 It is case-insensitive, obvious and feature-rich language.
@@ -51,35 +51,67 @@
 }
 ```
 
 # Package
 
 Package's API is similar to built-in `json`:
 
-- `wtfl.loads(str)` reads an object from a string
-- `wtfl.load(file)` reads an object from a file
-- `wtfl.dumps(obj)` dumps an object into a string
-- `wtfl.dump(file, obj)` dumps an object into a file
+read an object from a string:
+```python
+def wtfl.loads(
+    s, # string to load
+    *,
+    parse_float, # function for float parsing, `float` used by default
+    parse_int, # function for integer parsing (only unprefixed decimal), `int` used by default
+    parse_roman, # function for roman numerals parsing, accepts whole literal as a string (0r...)
+    parse_numbers, # function for integer literals parsing (0b..., 0o..., and so on)
+) -> 
+```
+read an object from a file (same argument meaning as `.loads`):
+`wtfl.load(file, *, parse_float, parse_int, parse_roman, parse_numbers)` 
 
-Current reader and writer are fairly simple, later versions would probably improve configurability
+dump an object into a string:
+```python
+def wtfl.dumps(
+    obj: object, # object to dump
+    *,
+    # if True, non-serializable keys / values are skipped
+    skipkeys: bool = False, 
+    
+    # if True, encodes non-ASCII characters
+    ensure_ascii: bool = True, 
+    
+    # if a non-negative integer, used as indent size. if a string, used as indent character. If None, everything is inlined
+    indent: int | str | None = 2, 
+    
+    # a function that is used to recover from serialization errors. 
+    # if current value is not serializable and skipkeys=False, tries to serialize the result of default(value)
+    default: Callable[[object], str] | None = None, 
+    
+    # if True, sorts object keys
+    sort_keys: bool = False,
+)
+```
+dump an object into a file (same argument meaning as `.dumps()`):
+`wtfl.dump(file, obj, *, skipkeys, ensure_ascii, indent, default, sort_keys)`
 
 # Reserved keywords
 
 It is very important to know all the keywords of WTFL, since all those keywords are important.    
 
 Here's a list (keywords in the same list entry are equivalent and used interchangeably in the spec):
 
 - `is` / `are` / `'s` / `'re` / `do` / `does` / `be`
 - `isn't` / `aren't` / `'sn't` / `'ren't`
 - `of`
 - `also` / `and also` / `but also`
 - `that` / `this` / `these` / `those`
 - `there`
 - `have` / `has` / `'ve`
-- `haven't` / `hasn't` / `'ve'n't`
+- `haven't` / `hasn't` / `'ven't`
 - `can`
 - `cannot` / `can't`
 - `true` / `falsen't`
 - `false` / `truen't`
 - `and`
 - `return`
 - `skip`
```

