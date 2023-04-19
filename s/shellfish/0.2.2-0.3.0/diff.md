# Comparing `tmp/shellfish-0.2.2.tar.gz` & `tmp/shellfish-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellfish-0.2.2.tar", max compression
+gzip compressed data, was "shellfish-0.3.0.tar", max compression
```

## Comparing `shellfish-0.2.2.tar` & `shellfish-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,35 @@
--rw-r--r--   0        0        0     1905 2023-03-22 17:14:54.990699 shellfish-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1003 2022-12-12 16:24:11.606024 shellfish-0.2.2/README.md
--rw-r--r--   0        0        0      409 2022-09-28 19:37:06.789210 shellfish-0.2.2/shellfish/__init__.py
--rw-r--r--   0        0        0      239 2022-02-01 20:37:20.196356 shellfish-0.2.2/shellfish/__main__.py
--rw-r--r--   0        0        0      218 2023-03-22 17:15:17.135877 shellfish-0.2.2/shellfish/_meta.py
--rw-r--r--   0        0        0      681 2023-03-08 23:03:45.973046 shellfish-0.2.2/shellfish/aios/__init__.py
--rw-r--r--   0        0        0      624 2022-02-11 23:27:58.166196 shellfish-0.2.2/shellfish/aios/_path.py
--rw-r--r--   0        0        0     6468 2022-06-02 17:33:59.763392 shellfish-0.2.2/shellfish/batman.py
--rw-r--r--   0        0        0      295 2022-02-11 23:27:58.166196 shellfish-0.2.2/shellfish/const.py
--rw-r--r--   0        0        0       49 2022-02-01 20:37:20.197354 shellfish-0.2.2/shellfish/dev/__init__.py
--rw-r--r--   0        0        0     2446 2022-06-02 17:33:59.763392 shellfish-0.2.2/shellfish/dev/popen_gen.py
--rw-r--r--   0        0        0     3487 2023-03-08 23:03:45.973046 shellfish-0.2.2/shellfish/dotenv.py
--rw-r--r--   0        0        0      554 2023-03-08 23:03:45.974275 shellfish-0.2.2/shellfish/echo.py
--rw-r--r--   0        0        0     7846 2023-03-08 23:03:45.974275 shellfish-0.2.2/shellfish/exe.py
--rw-r--r--   0        0        0    52521 2023-03-08 23:03:45.974275 shellfish-0.2.2/shellfish/fs/__init__.py
--rw-r--r--   0        0        0    14257 2023-03-08 23:03:45.975280 shellfish-0.2.2/shellfish/fs/_async.py
--rw-r--r--   0        0        0     1534 2023-03-08 23:03:45.975777 shellfish-0.2.2/shellfish/fs/promises.py
--rw-r--r--   0        0        0       50 2023-03-08 23:03:45.975777 shellfish-0.2.2/shellfish/libsh/__init__.py
--rw-r--r--   0        0        0     3653 2023-03-08 23:03:45.976783 shellfish-0.2.2/shellfish/libsh/_dirtree.py
--rw-r--r--   0        0        0    10602 2022-06-02 17:33:59.763392 shellfish-0.2.2/shellfish/osfs.py
--rw-r--r--   0        0        0     5257 2023-03-22 17:14:38.828805 shellfish-0.2.2/shellfish/process.py
--rw-r--r--   0        0        0      288 2022-06-02 17:33:59.763392 shellfish-0.2.2/shellfish/psu.py
--rw-r--r--   0        0        0        0 2022-02-01 20:37:20.199984 shellfish-0.2.2/shellfish/py.typed
--rw-r--r--   0        0        0    64238 2023-03-22 17:14:38.829793 shellfish-0.2.2/shellfish/sh.py
--rw-r--r--   0        0        0     5504 2023-03-08 23:03:45.977781 shellfish-0.2.2/shellfish/sp.py
--rw-r--r--   0        0        0     2361 2023-03-08 23:03:45.977781 shellfish-0.2.2/shellfish/testing.py
--rw-r--r--   0        0        0     1974 1970-01-01 00:00:00.000000 shellfish-0.2.2/setup.py
--rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 shellfish-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2246 2023-04-19 19:17:33.731684 shellfish-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1003 2022-09-19 18:35:16.987296 shellfish-0.3.0/README.md
+-rw-r--r--   0        0        0     1144 2023-04-19 19:17:33.732684 shellfish-0.3.0/shellfish/__init__.py
+-rw-r--r--   0        0        0      479 2023-04-18 11:41:47.355881 shellfish-0.3.0/shellfish/__main__.py
+-rw-r--r--   0        0        0      218 2023-04-19 19:17:33.733686 shellfish-0.3.0/shellfish/_meta.py
+-rw-r--r--   0        0        0      866 2023-04-19 19:17:33.733686 shellfish-0.3.0/shellfish/_types.py
+-rw-r--r--   0        0        0     3278 2023-04-19 19:17:33.734686 shellfish-0.3.0/shellfish/aios/__init__.py
+-rw-r--r--   0        0        0      640 2023-04-19 19:16:52.950595 shellfish-0.3.0/shellfish/aios/_path.py
+-rw-r--r--   0        0        0     7251 2023-04-19 19:17:33.734686 shellfish-0.3.0/shellfish/batman.py
+-rw-r--r--   0        0        0      295 2022-02-17 22:17:07.429546 shellfish-0.3.0/shellfish/const.py
+-rw-r--r--   0        0        0       49 2022-02-04 21:32:32.211842 shellfish-0.3.0/shellfish/dev/__init__.py
+-rw-r--r--   0        0        0     1439 2023-04-19 19:17:33.735685 shellfish-0.3.0/shellfish/dev/do.py
+-rw-r--r--   0        0        0     3456 2023-04-19 19:17:33.735685 shellfish-0.3.0/shellfish/dev/popen_gen.py
+-rw-r--r--   0        0        0     7941 2023-04-19 19:17:33.736685 shellfish-0.3.0/shellfish/dev/run_async.py
+-rw-r--r--   0        0        0     4265 2023-04-11 22:29:27.086800 shellfish-0.3.0/shellfish/dotenv.py
+-rw-r--r--   0        0        0      664 2023-03-31 17:46:06.868732 shellfish-0.3.0/shellfish/echo.py
+-rw-r--r--   0        0        0     7924 2023-04-19 19:17:33.736685 shellfish-0.3.0/shellfish/exe.py
+-rw-r--r--   0        0        0    54260 2023-04-19 19:17:33.737715 shellfish-0.3.0/shellfish/fs/__init__.py
+-rw-r--r--   0        0        0    15169 2023-04-19 19:17:33.738722 shellfish-0.3.0/shellfish/fs/_async.py
+-rw-r--r--   0        0        0     1534 2023-02-24 22:45:12.450622 shellfish-0.3.0/shellfish/fs/promises.py
+-rw-r--r--   0        0        0     1917 2023-04-19 19:17:33.738722 shellfish-0.3.0/shellfish/libhash.py
+-rw-r--r--   0        0        0       50 2023-02-09 22:42:06.315587 shellfish-0.3.0/shellfish/libsh/__init__.py
+-rw-r--r--   0        0        0     3655 2023-04-19 19:17:33.739722 shellfish-0.3.0/shellfish/libsh/_dirtree.py
+-rw-r--r--   0        0        0     1872 2023-04-19 19:17:33.739722 shellfish-0.3.0/shellfish/libsh/args.py
+-rw-r--r--   0        0        0    10653 2023-04-19 19:17:33.739722 shellfish-0.3.0/shellfish/osfs.py
+-rw-r--r--   0        0        0     7266 2023-04-19 19:17:33.740721 shellfish-0.3.0/shellfish/process.py
+-rw-r--r--   0        0        0      308 2023-03-24 22:14:11.926875 shellfish-0.3.0/shellfish/psu.py
+-rw-r--r--   0        0        0        0 2022-02-01 22:06:04.844951 shellfish-0.3.0/shellfish/py.typed
+-rw-r--r--   0        0        0    63204 2023-04-19 19:17:33.740721 shellfish-0.3.0/shellfish/sh.py
+-rw-r--r--   0        0        0     8275 2023-04-19 19:17:33.741721 shellfish-0.3.0/shellfish/sp.py
+-rw-r--r--   0        0        0      228 2023-04-19 19:17:33.741721 shellfish-0.3.0/shellfish/stdio.py
+-rw-r--r--   0        0        0     2617 2023-04-11 22:29:27.086800 shellfish-0.3.0/shellfish/testing.py
+-rw-r--r--   0        0        0       27 2023-04-19 19:17:33.742721 shellfish-0.3.0/shellfish/tests/__init__.py
+-rw-r--r--   0        0        0     2814 2023-04-19 19:17:33.742721 shellfish-0.3.0/shellfish/tests/test_fs.py
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 shellfish-0.3.0/PKG-INFO
```

### Comparing `shellfish-0.2.2/pyproject.toml` & `shellfish-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shellfish"
-version = "0.2.2"
+version = "0.3.0"
 description = "shellfish ~ shell & file-system utils"
 license = "MIT"
 authors = ["jesse <jesse@dgi.com>"]
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 homepage = "https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/shellfish"
 readme = 'README.md'
 packages = [
@@ -36,15 +36,15 @@
 asyncify = ">=0.9.1"
 funkify = ">=0.4.0"
 jsonbourne = ">=0.24.0"
 listless = ">=0.1.0"
 xtyping = ">=0.6.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
@@ -69,9 +69,29 @@
 markers = [
   "slow: marks tests as slow (deselect with '-m \"not slow\"')",
   "timeout",
   "aio",
   "asyncio",
 ]
 
+[tool.coverage.run]
+source = ['shellfish']
+branch = true
+context = '${CONTEXT}'
+omit = ["**/__main__.py"]
+
+[tool.coverage.report]
+precision = 2
+show_missing = true
+exclude_lines = [
+  'pragma: nocov',
+  'pragma: no cover',
+  'raise NotImplementedError',
+  'if TYPE_CHECKING:',
+  '@overload',
+  '\(Protocol\):$',
+  'if 0:',
+  'if False:',
+]
+
 [tool.ruff]
 extend = "../../pyproject.toml"
```

### Comparing `shellfish-0.2.2/README.md` & `shellfish-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `shellfish-0.2.2/shellfish/aios/_path.py` & `shellfish-0.3.0/shellfish/aios/_path.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "getsize",
     "isdir",
     "isfile",
     "islink",
     "samefile",
     "sameopenfile",
 )
-
+join = path.join
 exists = asyncify(path.exists)
 getatime = asyncify(path.getatime)
 getctime = asyncify(path.getctime)
 getmtime = asyncify(path.getmtime)
 getsize = asyncify(path.getsize)
 isdir = asyncify(path.isdir)
 isfile = asyncify(path.isfile)
```

### Comparing `shellfish-0.2.2/shellfish/batman.py` & `shellfish-0.3.0/shellfish/batman.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,18 +29,16 @@
     bat_filepath = which(fspath)
     if bat_filepath is None:
         fspath_obj = Path(fspath)
         if not fspath_obj.exists():
             raise FileNotFoundError(fspath)
     else:
         fspath_obj = Path(bat_filepath)
-
-    _args = [str(fspath)] if shell else ["cmd", "/c", _fspath(fspath_obj)]
     return run(
-        args=_args,
+        args=[str(fspath)] if shell else ["cmd", "/c", _fspath(fspath_obj)],
         capture_output=True,
         shell=shell,
         text=text,
         check=check,
         cwd=fspath_obj.parent,
     )
 
@@ -72,14 +70,38 @@
         with bat_filepath.open(mode="w", newline="\r\n") as f:
             bat_file_str = "\r\n".join(_commands)
             f.write(bat_file_str)
         return bat(bat_filepath, text=text)
 
 
 def MKLINK_OPT(D: bool = False, H: bool = False, J: bool = False) -> Union[str, None]:
+    """Return the appropriate /D, /H, or /J option for windows mklink
+
+    Args:
+        D (bool): `mklink /D` creates a directory symbolic link.
+        H (bool): `mklink /H` creates a hard link instead of a symbolic link.
+        J (bool): `mklink /J` creates a directory junction.
+
+    Returns:
+        Union[str, None]: The appropriate /D, /H, or /J option for windows mklink
+
+    Examples:
+        >>> MKLINK_OPT(D=True)
+        '/D'
+        >>> MKLINK_OPT(H=True)
+        '/H'
+        >>> MKLINK_OPT(J=True)
+        '/J'
+        >>> MKLINK_OPT()
+        >>> MKLINK_OPT(D=True, H=True)
+        Traceback (most recent call last):
+        ...
+        ValueError: Only one of D, H, J can be True.  Got True, True, False
+
+    """
     # Check that only one of D, H, J is True
     if sum((D, H, J)) > 1:
         raise ValueError(f"Only one of D, H, J can be True.  Got {D}, {H}, {J}")
     if D:
         return "/D"
     if H:
         return "/H"
@@ -231,7 +253,13 @@
     return run(
         args=("DEL", _fspath(Path(fspath))),
         check=check,
         capture_output=True,
         text=True,
         shell=True,
     )
+
+
+if __name__ == "__main__":
+    import doctest
+
+    doctest.testmod()
```

### Comparing `shellfish-0.2.2/shellfish/dev/popen_gen.py` & `shellfish-0.3.0/shellfish/dev/popen_gen.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,92 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from concurrent.futures.thread import ThreadPoolExecutor
 from queue import Empty, Queue
-from subprocess import PIPE, Popen
+from subprocess import PIPE, Popen, TimeoutExpired
+from time import time
 
 from shellfish.fs import Stdio
-from xtyping import IO, Any, AnyStr, Iterable, Tuple
+from xtyping import IO, Any, AnyStr, Iterable, Optional, Tuple
 
-__all__ = ("popen_gen",)
+__all__ = ("popen_gen", "popen_pipes_gen")
 
 
-def _enqueue_output(fileio: IO[AnyStr], queue: Queue[AnyStr]) -> None:
+def _enqueue_output(
+    fileio: IO[AnyStr],
+    queue: Queue[AnyStr],
+    block: bool = True,
+) -> None:
+    while True:
+        line = fileio.readline()
+        if line:
+            queue.put(line, block=block)
+        else:
+            break
+
+
+def _enqueue_output_iter_readline(
+    fileio: IO[AnyStr], queue: Queue[AnyStr], block: bool = True
+) -> None:
     for line in iter(fileio.readline, ""):
-        queue.put(line)
+        queue.put(line, block=block)
     fileio.close()
 
 
-def _popen_pipes_gen(proc: Popen[AnyStr]) -> Iterable[Tuple[Stdio, str]]:
+def popen_pipes_gen(
+    proc: Popen[AnyStr], timeout: Optional[float] = None
+) -> Iterable[Tuple[Stdio, str]]:
     """Yield stdout and stderr lines from a subprocess
 
     Args:
         proc (Popen): Popen process
+        timeout (Optional[float], optional): Timeout in seconds. Defaults to None.
 
     Yields:
         Tuple[Stdio, str]: Tuples with stdio enum marker followed by a string
 
     Raises:
         ValueError: if proc is not Popen or proc.stdout or proc.stderr is None
 
     """
     if not isinstance(proc, Popen):
         raise ValueError("proc must be a Popen object")
+    _raise_err = False
     if proc.stdout is not None and proc.stderr is not None:
+        ti = time()
         with ThreadPoolExecutor(2) as pool:
             q_stdout: Queue[AnyStr] = Queue()
             q_stderr: Queue[AnyStr] = Queue()
-            pool.submit(_enqueue_output, proc.stdout, q_stdout)  # type: ignore[arg-type]
-            pool.submit(_enqueue_output, proc.stderr, q_stderr)  # type: ignore[arg-type]
-            while True:
-                if proc.poll() is not None and q_stdout.empty() and q_stderr.empty():
-                    break
-
+            _block = True
+            stdout_future = pool.submit(
+                _enqueue_output_iter_readline, proc.stdout, q_stdout, _block  # type: ignore[arg-type]
+            )
+            stderr_future = pool.submit(
+                _enqueue_output_iter_readline, proc.stderr, q_stderr, _block  # type: ignore[arg-type]
+            )
+            while proc.poll() is None:
                 try:
                     yield Stdio.stdout, q_stdout.get_nowait()
                 except Empty:
                     pass
-
                 try:
                     yield Stdio.stderr, q_stderr.get_nowait()
                 except Empty:
                     pass
+                if timeout is not None and time() - ti > timeout:
+                    _raise_err = True
+                    stdout_future.cancel()
+                    stderr_future.cancel()
+                    pool.shutdown(wait=False)
+                    break
+        if _raise_err and timeout is not None:
+            proc.terminate()
+            raise TimeoutExpired(proc.args, timeout, output=None, stderr=None)
+
     else:
         raise ValueError("proc.stdout and proc.stderr must be not None")
 
 
 def popen_gen(*popenargs: Any, **popenkwargs: Any) -> Iterable[Tuple[Stdio, str]]:
     """Create and open a subprocess and yield tuples with stdout/stderr lines
 
@@ -67,8 +99,8 @@
             or ('stderr', stderr_line) for the stdout and stderr lines for
             the subprocess created.
 
     """
     with Popen(
         *popenargs, **popenkwargs, stdout=PIPE, stderr=PIPE, text=True
     ) as proc:  # type: ignore[call-overload]
-        yield from _popen_pipes_gen(proc)
+        yield from popen_pipes_gen(proc)
```

### Comparing `shellfish-0.2.2/shellfish/echo.py` & `shellfish-0.3.0/shellfish/echo.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,19 @@
     end: str = "\n",
     file: Optional[IO[str]] = None,
     flush: bool = False,
 ) -> None:
     """Print/echo function
 
     Args:
-        *args: Item(s) to print/echo
+        *objects: Item(s) to print/echo
         sep: Separator to print with
         end: End of print suffix; defaults to `\n`
         file: File like object to write to if not stdout
+        flush: Flush the file after writing
+
+    Examples:
+        >>> echo("shellfish")
+        shellfish
 
     """
     print(*objects, sep=sep, end=end, file=file, flush=flush)  # ruff: noqa: T201
```

### Comparing `shellfish-0.2.2/shellfish/exe.py` & `shellfish-0.3.0/shellfish/exe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,19 @@
 # -*- coding: utf-8 -*-
 """Exes/commands"""
 from __future__ import annotations
 
 from shlex import split as _shplit
+from typing import Any, Dict, List, Optional, Set, Tuple, Type, TypeVar, Union
 
 from jsonbourne.pydantic import JsonBaseModel
 from shellfish import sh
+from shellfish._types import PopenArgs, PopenArgv
 from shellfish.sh import Done, flatten_args
-from shellfish.sp import PopenArgs, PopenArgv
-from xtyping import (
-    STDIN,
-    Any,
-    Dict,
-    FsPath,
-    List,
-    Optional,
-    Sequence,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-)
+from xtyping import STDIN, FsPath
 
 __all__ = (
     "Exe",
     "ExeAsync",
 )
 
 TExe = TypeVar("TExe", bound="ExeABC")
@@ -35,40 +24,40 @@
     subcmd: Optional[Tuple[str, ...]] = None
     abspath: Optional[str] = None
     env: Optional[Dict[str, str]] = None
     cwd: Optional[str] = None
     shell: bool = False
     verbose: bool = False
     timeout: Optional[int] = None
-    ok_code: Sequence[int] = (0,)
+    ok_code: Union[int, Set[int]] = {0}
     check: bool = False
 
 
 class ExeABC:
     cmd: str
     subcmd: Optional[Tuple[str, ...]] = None
 
     abspath: Optional[str] = None
     env: Optional[Dict[str, str]] = None
     cwd: Optional[FsPath] = None
     shell: bool = False
     verbose: bool = False
     timeout: Optional[int] = None
-    ok_code: Sequence[int] = (0,)
+    ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = (0,)
     check: bool = False
 
     def __init__(
         self,
         cmd: str,
         subcmd: Optional[Union[Tuple[str, ...], List[str], str]] = None,
         abspath: Optional[str] = None,
         check: bool = False,
         cwd: Optional[FsPath] = None,
         env: Optional[Dict[str, str]] = None,
-        ok_code: Union[int, Sequence[int]] = 0,
+        ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
         shell: bool = False,
         timeout: Optional[int] = None,
         verbose: bool = False,
     ):
         self.cmd = cmd
         if subcmd is not None:
             self.subcmd = (subcmd,) if isinstance(subcmd, str) else tuple(subcmd)
@@ -161,15 +150,15 @@
         extenv: bool = True,
         cwd: Optional[FsPath] = None,
         shell: bool = False,
         check: bool = False,
         verbose: bool = False,
         input: STDIN = None,
         timeout: Optional[int] = None,
-        ok_code: Union[int, Sequence[int]] = 0,
+        ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
         dryrun: bool = False,
     ) -> Done:
         _args = self._cmdargs(popenargs, args)
         return sh.do(
             args=_args,
             env=env or self.env,
             extenv=extenv,
@@ -190,29 +179,28 @@
         check: bool = False,
         cwd: Optional[str] = None,
         dryrun: bool = False,
         env: Optional[Dict[str, str]] = None,
         extenv: bool = True,
         input: STDIN = None,
         loop: Optional[Any] = None,
-        ok_code: Union[int, Sequence[int]] = 0,
+        ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
         shell: bool = False,
         timeout: Optional[int] = None,
         verbose: bool = False,
     ) -> Done:
         _args = self._cmdargs(popenargs, args)
         return await sh.do_async(
             args=_args,
             check=check,
             cwd=cwd or str(self.cwd),
             dryrun=dryrun,
             env=env or self.env,
             extenv=extenv,
             input=input,
-            loop=loop,
             ok_code=ok_code or self.ok_code,
             shell=shell or self.shell,
             timeout=timeout or self.timeout,
             verbose=verbose or self.verbose,
         )
 
     # aliases
@@ -230,15 +218,15 @@
         extenv: bool = True,
         cwd: Optional[FsPath] = None,
         shell: bool = False,
         check: bool = False,
         verbose: bool = False,
         input: STDIN = None,
         timeout: Optional[int] = None,
-        ok_code: Union[int, Sequence[int]] = 0,
+        ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
         dryrun: bool = False,
     ) -> Done:
         return self._do(
             *popenargs,
             args=args,
             check=check,
             cwd=cwd,
```

### Comparing `shellfish-0.2.2/shellfish/fs/__init__.py` & `shellfish-0.3.0/shellfish/fs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 """file-system utils"""
 from __future__ import annotations
 
-from enum import IntEnum
 from glob import has_magic, iglob
 from itertools import chain, count
 from os import (
     DirEntry,
     chmod as _chmod,
     fspath as _fspath,
     makedirs as _makedirs,
@@ -19,21 +18,22 @@
     stat as _stat,
     stat_result as os_stat_result,
     symlink as _symlink,
     utime,
     walk,
 )
 from pathlib import Path
-from shutil import copytree, move as _move, rmtree
+from shutil import copystat as _copystat, copytree, move as _move, rmtree
 from time import time
 
 from jsonbourne import JSON
 from listless import exhaust
 from shellfish import const
 from shellfish._meta import __version__
+from shellfish._types import FsPath, SymlinkType
 from shellfish.fs._async import (
     dir_exists_async as dir_exists_async,
     exists_async as exists_async,
     file_exists_async as file_exists_async,
     filesize_async as filesize_async,
     is_dir_async as is_dir_async,
     is_file_async as is_file_async,
@@ -66,42 +66,33 @@
     wbin_gen_async as wbin_gen_async,
     wbytes_async as wbytes_async,
     wbytes_gen_async as wbytes_gen_async,
     wjson_async as wjson_async,
     wstr_async as wstr_async,
     wstring_async as wstring_async,
 )
-from shellfish.process import is_win
+from shellfish.process import is_win as is_win
+from shellfish.stdio import Stdio as Stdio
 from xtyping import (
     Any,
     AnyStr,
     Callable,
-    FsPath,
     Generator,
     Iterable,
     Iterator,
     List,
-    Literal,
     Optional,
     Tuple,
     Union,
     cast,
 )
 
 # END-IMPORTS
 
 
-class Stdio(IntEnum):
-    """Standard-io enum object"""
-
-    stdin = 0
-    stdout = 1
-    stderr = 2
-
-
 def fspath(fspath: FsPath) -> str:
     """Alias for os._fspath; returns fspath string for any type of path"""
     return _fspath(fspath)
 
 
 def isfile(fspath: FsPath) -> bool:
     """Return True if the given path is a file; False otherwise"""
@@ -120,26 +111,36 @@
 
 def exists(fspath: FsPath) -> bool:
     """Return True if the given path exists; False otherwise"""
     return path.exists(_fspath(fspath))
 
 
 def file_exists(fspath: FsPath) -> bool:
-    """Return True if the given path exists; False otherwise"""
+    """Return True if the given path exists; False otherwise; alias for isfile"""
     return isfile(fspath)
 
 
 def dir_exists(fspath: FsPath) -> bool:
-    """Return True if the given path exists; False otherwise"""
+    """Return True if the given path exists; False otherwise; alias for isdir"""
     return isdir(fspath)
 
 
-is_dir = isdir
-is_file = isfile
-is_link = islink
+def is_dir(fspath: FsPath) -> bool:
+    """Return True if the given path is a directory; alias for isdir"""
+    return isdir(fspath)
+
+
+def is_file(fspath: FsPath) -> bool:
+    """Return True if the given path is a file; alias for isfile"""
+    return isfile(fspath)
+
+
+def is_link(fspath: FsPath) -> bool:
+    """Return True if the given path is a link; alias for islink"""
+    return islink(fspath)
 
 
 def safepath(fspath: FsPath) -> str:
     """Check if a file/dir path is save/unused; returns an unused path.
 
     Args:
         fspath: file-system path; file or directory path string or Path obj
@@ -233,18 +234,22 @@
     dirs_only: bool = False,
     symlinks_only: bool = False,
 ) -> Iterator[DirEntry[str]]:
     r"""Return an iterator of os.DirEntry objects
 
     Args:
         fspath: (FsPath): dirpath to look through
+        recursive (bool): recursively scan the directory
+        follow_symlinks (bool): follow symlinks when checking for dirs and files
         files (bool): include files
         dirs (bool): include directories
         symlinks (bool): include symlinks
-        follow_symlinks (bool): follow symlinks when checking for dirs and files
+        dirs_only (bool): only include directories
+        files_only (bool): only include files
+        symlinks_only (bool): only include symlinks
 
     Returns:
         Iterator[DirEntry]: Iterator of os.DirEntry objects
 
     Raises:
         ValueError: if any of the kwargs (`dirs`, `files` and `symlinks`) are not True
 
@@ -306,14 +311,15 @@
 
     Examples
         >>> tmpdir = 'listdir_gen.doctest'
         >>> from shellfish import sh
         >>> from os import makedirs, path, chdir
         >>> from shutil import rmtree
         >>> _makedirs(tmpdir, exist_ok=True)
+        >>> pwd = sh.pwd()
         >>> sh.cd(tmpdir)
         >>> filepath_parts = [
         ...     ("dir", "file1.txt"),
         ...     ("dir", "file2.txt"),
         ...     ("dir", "file3.txt"),
         ...     ("dir", "data1.json"),
         ...     ("dir", "dir2", "file1.txt"),
@@ -340,15 +346,20 @@
         >>> abspaths = sorted(listdir_gen(dirpath, abspath=True, dirs=False, symlinks=False))
         >>> for abspath in [p.replace("\\", "/") for p in abspaths]:
         ...    print(abspath)
         listdir_gen.doctest/dir/data1.json
         listdir_gen.doctest/dir/file1.txt
         listdir_gen.doctest/dir/file2.txt
         listdir_gen.doctest/dir/file3.txt
-        >>> rmtree(tmpdir)
+        >>> sh.cd(pwd)
+        >>> import os
+        >>> if path.exists(tmpdir):
+        ...     rmtree(tmpdir)
+        >>> path.isdir(tmpdir)
+        False
 
     """
     _attr = "path" if abspath else "name"
     return (
         getattr(el, _attr)
         for el in scandir_gen(
             fspath,
@@ -364,23 +375,27 @@
 
 
 def filepath_mtimedelta_sec(filepath: FsPath) -> float:
     """Return the seconds since the file(path) was last modified"""
     return time() - path.getmtime(_fspath(filepath))
 
 
-def touch(fspath: FsPath) -> None:
+def touch(fspath: FsPath, *, mkdirp: bool = True) -> None:
     """Create an empty file given a fspath
 
     Args:
         fspath (FsPath): File-system path for where to make an empty file
+        mkdirp (bool): Make parent directories if they don't exist
 
     """
     if not path.exists(str(fspath)):
-        _makedirs(path.dirname(str(fspath)), exist_ok=True)
+        if mkdirp:
+            parent_dir = path.dirname(str(fspath))
+            if parent_dir:
+                _makedirs(parent_dir, exist_ok=True)
         with open(fspath, "a"):
             utime(fspath, None)
 
 
 def files_gen(
     dirpath: FsPath = ".",
     *,
@@ -497,14 +512,15 @@
 
     Args:
         dirpath: Directory path to walk down/through.
         abspath (bool): Yield the absolute path
         onerror: Function called on OSError
         topdown: Not applicable
         followlinks: Follow links
+        check: Check that dir exists
 
     Returns:
         Generator object that yields directory paths (absolute or relative)
 
     Examples:
         >>> tmpdir = 'dirs_gen.doctest'
         >>> from os import makedirs; _makedirs(tmpdir, exist_ok=True)
@@ -617,14 +633,15 @@
 
     Args:
         dirpath: Directory path to walk down/through.
         abspath (bool): Yield the absolute path
         onerror: Function called on OSError
         topdown: Not applicable
         followlinks: Follow links
+        check: Check if dirpath is a directory
 
     Returns:
         A tuple of two generators (files_gen(), dirs_gen())
 
 
     Examples:
         >>> tmpdir = 'files_dirs_gen.doctest'
@@ -740,14 +757,15 @@
 
     Args:
         dirpath: Directory path to walk down/through.
         abspath (bool): Yield the absolute path
         onerror: Function called on OSError
         topdown: Not applicable
         followlinks: Follow links
+        check: Check if dirpath exists
 
     Returns:
         Generator object that yields directory paths (absolute or relative)
 
     Examples:
         >>> tmpdir = 'walk_gen.doctest'
         >>> from os import makedirs; _makedirs(tmpdir, exist_ok=True)
@@ -1173,16 +1191,18 @@
 
     Args:
         filepath: fspath to write to
         data (Any): json-serial-ize-able data
         fmt (bool): Indented (2 spaces) or minify data (default=False)
         pretty (bool): Indented (2 spaces) or minify data (default=False)
         sort_keys (bool): Sort the data keys if the data is a dictionary.
-        append_newline (bool): Sort the data keys if the data is a dictionary.
+        append_newline (bool): Append a newline to the end of the file
         default: default function hook
+        chmod (Optional[int]): Optional chmod to set on file
+        append (bool): Append to the file if True, overwrite otherwise; default
         **kwargs: Additional keyword arguments to pass to jsonbourne.JSON.dumpb
 
     Returns:
         int: Number of bytes written
 
     Examples:
         Imports:
@@ -1267,16 +1287,29 @@
         [['a', 1], ['b', 2], ['c', 3]]
         >>> os.remove(fspath)
 
     """
     return JSON.loads(lstring(filepath=filepath))
 
 
-def extension(fspath: str) -> str:
-    """Return the extension for a fspath"""
+def extension(fspath: str, *, period: bool = False) -> str:
+    """Return the extension for a fspath
+
+    Examples:
+        >>> from shellfish.fs import extension
+        >>> extension("foo.bar")
+        'bar'
+        >>> extension("foo.tar.gz")
+        'tar.gz'
+        >>> extension("foo.tar.gz", period=True)
+        '.tar.gz'
+
+    """
+    if period:
+        return "".join(Path(fspath).suffixes)
     return "".join(Path(fspath).suffixes).lstrip(".")
 
 
 def sep_split(fspath: FsPath) -> Tuple[str, ...]:
     """Split a string on the current platform os.path.sep value"""
     return tuple(el for el in str(fspath).split(sep) if el != sep and el != "")
 
@@ -1402,15 +1435,15 @@
     return mkdir(fspath=fspath, parents=True)
 
 
 def glob(pattern: str, *, recursive: bool = False, r: bool = False) -> Iterator[str]:
     """Return an iterator of fspaths matching the given glob pattern
 
     Args:
-        fspath: Glob pattern
+        pattern: Glob pattern
         recursive: Recursively search directories if True
         r: Recursively search directories if True (Alias for recursive)
 
     Returns:
         Iterator[str]: Iterator of fspaths matching the glob pattern
 
     """
@@ -1453,14 +1486,15 @@
 
 
 def rmdir(fspath: FsPath, *, force: bool = False, recursive: bool = False) -> None:
     """Remove directory at given fspath
 
     Args:
         fspath (FsPath): Directory path to remove
+        force (bool): Force removal of files and directories
         recursive (bool): Recursively remove all contents if True
 
     Returns:
         None
 
     """
     if force:
@@ -1556,39 +1590,41 @@
     Returns:
         os.stat_result: stat_result object
 
     """
     return _stat(_fspath(fspath))
 
 
-SymlinkType = Union[Literal["dir"], Literal["file"], Literal["junction"], str]
-
-
 def symlink(link: FsPath, target: FsPath, *, _type: SymlinkType = "file") -> None:
     if is_win():
         raise NotImplementedError("TODO")
     _symlink(str(link), str(target))
 
 
 def copy_file(
     src: FsPath, dest: FsPath, *, dryrun: bool = False, mkdirp: bool = False
-) -> None:
+) -> Tuple[str, str]:
     """Copy a file given a source-path and a destination-path
 
     Args:
         src (str): Source fspath
         dest (str): Destination fspath
+        dryrun (bool): Do not copy file if True just return the src and dest
+        mkdirp (bool): Create parent directories if they do not exist
 
     """
     _dest = Path(dest)
-    if mkdirp:
+    if not dryrun and mkdirp:
         _dest.parent.mkdir(parents=mkdirp, exist_ok=True)
     elif not _dest.parent.exists() or not _dest.parent.is_dir():
         raise FileNotFoundError(f"Destination directory {_dest.parent} does not exist")
-    wbytes_gen(dest, lbytes_gen(src, blocksize=2**18))
+    if not dryrun:
+        wbytes_gen(dest, lbytes_gen(src, blocksize=2**18))
+        _copystat(src, dest, follow_symlinks=True)
+    return (str(src), str(dest))
 
 
 def cp(
     src: FsPath,
     dest: FsPath,
     *,
     force: bool = True,
```

### Comparing `shellfish-0.2.2/shellfish/fs/_async.py` & `shellfish-0.3.0/shellfish/fs/_async.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,24 +52,39 @@
 
 
 async def isfile_async(fspath: FsPath) -> bool:
     """Return True if the given path is a file; False otherwise"""
     return await aios.path.isfile(_fspath(fspath))
 
 
+async def is_file_async(fspath: FsPath) -> bool:
+    """Return True if the given path is a file; False otherwise"""
+    return await isfile_async(fspath)
+
+
 async def isdir_async(fspath: FsPath) -> bool:
     """Return True if the given path is a file; False otherwise"""
-    return await aios.path.isfile(_fspath(fspath))
+    return await aios.path.isdir(_fspath(fspath))
+
+
+async def is_dir_async(fspath: FsPath) -> bool:
+    """Return True if the given path is a file; False otherwise"""
+    return await isdir_async(fspath)
 
 
 async def islink_async(fspath: FsPath) -> bool:
     """Return True if the given path is a link; False otherwise"""
     return await aios.path.islink(_fspath(fspath))
 
 
+async def is_link_async(fspath: FsPath) -> bool:
+    """Return True if the given path is a link; False otherwise"""
+    return await islink_async(fspath)
+
+
 async def exists_async(fspath: FsPath) -> bool:
     return await aios.path.exists(_fspath(fspath))
 
 
 async def stat_async(fspath: FsPath) -> os.stat_result:
     """Async version of `os.lstat`"""
     return await aios.stat(str(fspath))
@@ -77,34 +92,42 @@
 
 async def lstat_async(fspath: FsPath) -> os.stat_result:
     """Async version of `os.lstat`"""
     return await aios.lstat(str(fspath))
 
 
 async def filesize_async(fspath: FsPath) -> int:
-    """Return the size of the file at the given fspath"""
+    """Return the size of the file at the given fspath
+
+    Examples:
+        >>> from asyncio import run as aiorun
+        >>> from pathlib import Path
+        >>> from tempfile import TemporaryDirectory
+        >>> with TemporaryDirectory() as tmpdir:
+        ...     tmpdir = Path(tmpdir)
+        ...     fpath = tmpdir / "test.txt"
+        ...     written = fpath.write_text("hello world")
+        ...     aiorun(filesize_async(fpath))
+        11
+
+    """
     _stat_res = await aios.stat(str(fspath))
     return _stat_res.st_size
 
 
 async def file_exists_async(fspath: FsPath) -> bool:
     """Return True if the file exists; False otherwise"""
     return await aios.path.isfile(_fspath(fspath))
 
 
 async def dir_exists_async(fspath: FsPath) -> bool:
     """Return True if the directory exists; False otherwise"""
     return await aios.path.isdir(_fspath(fspath))
 
 
-is_dir_async = isdir_async
-is_file_async = isfile_async
-is_link_async = islink_async
-
-
 async def listdir_async(fspath: FsPath) -> List[str]:
     """Async version of `os.listdir`"""
     return await aios.listdir(_fspath(fspath))
 
 
 # IO # IO # IO # IO # IO # IO # IO # IO # IO # IO # IO # IO # IO # IO # IO #
 async def wbytes_async(
@@ -119,14 +142,15 @@
     The parameter 'bites' is used instead of 'bytes' so as to not redefine
     the built-in python bytes object.
 
     Args:
         append (bool): Append to the fspath if True; otherwise overwrite
         filepath: fspath to write to
         bites: Bytes to be written
+        chmod: chmod the fspath to this mode after writing
 
     Returns:
         None
 
     Examples:
         >>> from shellfish.fs._async import rbytes_async, wbytes_async
         >>> from asyncio import run as aiorun
@@ -339,24 +363,25 @@
                 _bytes_written += await f.write(b)
         elif isinstance(bytes_gen, AsyncIterable):
             async for b in bytes_gen.__aiter__():
                 _bytes_written += await f.write(b)
         else:
             for b in bytes_gen:
                 _bytes_written += await f.write(b)
-    if chmod is not None:
+    if chmod is not None:  # pragma: nocov
         await aios.chmod(filepath, chmod)
     return _bytes_written
 
 
 async def rstring_async(filepath: FsPath, encoding: str = "utf-8") -> str:
     r"""(ASYNC) Load/Read a string given a fspath
 
     Args:
         filepath: Filepath for file to read
+        encoding (str): File encoding (Default='utf-8')
 
     Returns:
         str: String read from given fspath
 
     """
     return (await rbytes_async(filepath)).decode(encoding=encoding)
```

### Comparing `shellfish-0.2.2/shellfish/fs/promises.py` & `shellfish-0.3.0/shellfish/fs/promises.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.2.2/shellfish/libsh/_dirtree.py` & `shellfish-0.3.0/shellfish/libsh/_dirtree.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         is_last: bool,
     ) -> None:
         """Construct a DirTree object
 
         Args:
             path: Path-string to start the directory tree at
             parent_path: The parent path to start the directory tree at
-            is_last: Is the current tree the last diretory in the tree
+            is_last: Is the current tree the last directory in the tree
 
         """
         self.path = Path(str(path))
         self.parent = parent_path
         self.is_last = is_last
         self.depth: int = self.parent.depth + 1 if self.parent else 0
 
@@ -88,15 +88,15 @@
         ignore_strings = (".pyc", "__pycache__")
         return not any(
             ignored in str(path_string).lower() for ignored in ignore_strings
         )
 
     @property
     def displayname(self) -> str:
-        """Diplay name for DirTree root path name
+        """Display name for DirTree root path name
 
         Returns:
             str: root path name as a string
 
         """
         if self.path.is_dir():
             return self.path.name + "/"
```

### Comparing `shellfish-0.2.2/shellfish/osfs.py` & `shellfish-0.3.0/shellfish/osfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from abc import ABC, abstractmethod
 from os import makedirs, path, symlink, unlink
 
 from shellfish import batman
 from xtyping import IterableStr, List, Tuple
 
 
-class OsFsAbc(ABC):
+class OsFsAbc(ABC):  # pragma: nocov
     """Abstract base class for OS-specific fns"""
 
     @staticmethod
     @abstractmethod
     def link_dir(linkpath: str, targetpath: str, *, exist_ok: bool = False) -> None:
         ...
 
@@ -63,15 +63,15 @@
 #  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\
 # /  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \
 # =============================================================================
 # \/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\
 # =============================================================================
 
 
-class LIN(OsFsAbc):
+class LIN(OsFsAbc):  # pragma: nocov
     """Linux (and Mac) shell commands/methods container"""
 
     @staticmethod
     def link_dir(linkpath: str, targetpath: str, *, exist_ok: bool = False) -> None:
         """Make a directory symlink
 
         Args:
@@ -174,15 +174,15 @@
             links: Iterable of paths to links
 
         """
         for link in links:
             LIN.unlink_file(link)
 
 
-class WIN(OsFsAbc):
+class WIN(OsFsAbc):  # pragma: nocov
     """Windows shell commands/methods container"""
 
     _MAX_CMD_LENGTH: int = 8192
 
     @staticmethod
     def link_dir(linkpath: str, targetpath: str, *, exist_ok: bool = False) -> None:
         """Make a directory symlink
```

### Comparing `shellfish-0.2.2/shellfish/process.py` & `shellfish-0.3.0/shellfish/process.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,31 @@
 """Current running process info"""
 from __future__ import annotations
 
 import os
 import platform
 import sys
 
+from contextlib import contextmanager
 from os import environ
-from typing import Callable, Dict, Iterator, List, Optional, Union, cast
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generator,
+    ItemsView,
+    Iterator,
+    KeysView,
+    List,
+    Optional,
+    Type,
+    Union,
+    ValuesView,
+    cast,
+)
 
 IS_WIN = os.name == "nt"
 PYTHON_IMPLEMENTATION = platform.python_implementation()
 SYS_PATH_SEP: str = os.pathsep
 
 __all__ = (
     "ENV",
@@ -28,18 +43,30 @@
     "is_wsl",
     "ismac",
     "iswin",
     "iswsl",
     "opsys",
     "sys_path_sep",
 )
-
 _OS_ENVIRON_ATTRS = set(dir(os.environ))
 
 
+@contextmanager
+def tmpenv(**kwargs: str) -> Generator[Type[Env], Any, None]:
+    """Context manager for Env"""
+    old_env = dict(environ)
+    if kwargs:
+        env.update(kwargs)
+    try:
+        yield env
+    finally:
+        environ.clear()
+        environ.update(old_env)
+
+
 class _EnvObjMeta(type):
     def __contains__(cls, key: str) -> bool:
         return key in environ
 
     def __delitem__(cls, key: str) -> None:
         return environ.__delitem__(key)
 
@@ -72,20 +99,39 @@
         return cls.__getitem__(item)
 
     def __setattr__(cls, key: str, value: str) -> None:
         if hasattr(environ, key):
             raise ValueError(f"Key ({key}) is protected; set with __setitem__")
         return cls.__setitem__(key, value)
 
-    update = environ.update
-    get = environ.get
-    setdefault = environ.setdefault
-    clear = environ.clear
-    items = environ.items
-    keys = environ.keys
+    def update(self, d: Dict[str, str]) -> None:
+        return environ.update(d)
+
+    def update_from_dict(self, d: Dict[str, str]) -> None:
+        return self.update(d)
+
+    def get(self, key: str, default: Optional[str] = None) -> str:
+        if default is None:
+            return environ[key]
+        return environ.get(key, default)
+
+    def setdefault(self, key: str, default: str) -> str:
+        return environ.setdefault(key, default)
+
+    def clear(self) -> None:
+        return environ.clear()
+
+    def keys(self) -> KeysView[str]:
+        return environ.keys()
+
+    def values(self) -> ValuesView[str]:
+        return environ.values()
+
+    def items(self) -> ItemsView[str, str]:
+        return environ.items()
 
     def asdict(cls) -> Dict[str, str]:
         return dict(environ.items())
 
 
 class Env(metaclass=_EnvObjMeta):
     """Env with attr access
@@ -99,51 +145,64 @@
         >>> Env.SOMEENVVARIABLE = 'value'
         >>> Env.SOMEENVVARIABLE
         'value'
         >>> environ.get('SOMEENVVARIABLE')
         'value'
         >>> environ['SOMEENVVARIABLE']
         'value'
+        >>> 'SOMEENVVARIABLE' in Env
+        True
         >>> {k: v for k, v in Env.items() if k == 'SOMEENVVARIABLE'}
         {'SOMEENVVARIABLE': 'value'}
+        >>> del Env['SOMEENVVARIABLE']
+        >>> 'SOMEENVVARIABLE' in Env
+        False
 
     """
 
-    ...
-
 
 env = ENV = Env
 
 
 def env_dict() -> Dict[str, str]:
-    """Return the current enviroment as a dictionary"""
+    """Return the current environment-variables as a dictionary"""
     return env.asdict()
 
 
 def is_mac() -> bool:
     """Determine if current operating system is macos/osx
 
     Returns:
         True if on a mac; False otherwise
 
     """
     return "darwin" in platform.system().lower()
 
 
+def ismac() -> bool:
+    """Alias for is_mac()"""
+    return is_mac()
+
+
 def is_win() -> bool:
     """Determine if current operating system is windows
 
     Returns:
         True if on a windows machine; False otherwise
 
     """
     return IS_WIN
 
 
-def is_wsl() -> bool:
+def iswin() -> bool:
+    """Alias for is_win()"""
+    return is_win()
+
+
+def is_wsl() -> bool:  # pragma: nocov
     """Return True if python is running under (WSL); Return False otherwise"""
     if sys.platform in {"win32", "cygwin", "darwin"}:
         return False
 
     if "microsoft" in platform.release().lower():
         return True
 
@@ -153,15 +212,20 @@
                 return True
     except FileNotFoundError:
         pass
 
     return False
 
 
-def is_notebook() -> bool:
+def iswsl() -> bool:
+    """Alias for is_wsl()"""
+    return is_wsl()
+
+
+def is_notebook() -> bool:  # pragma: nocov
     """Determine if running in ipython/jupyter notebook; returns True/False"""
     try:
         shell = get_ipython().__class__.__name__  # type: ignore[name-defined]
         if shell == "ZMQInteractiveShell":
             return True  # Jupyter notebook or qtconsole
         elif shell == "TerminalInteractiveShell":
             return False  # Terminal running IPython
@@ -189,26 +253,53 @@
         return "wsl"
     if is_mac():
         return "mac"
     return "lin"
 
 
 def hostname() -> str:
-    """Return the current computer's hostname"""
+    """Return the current computer's hostname
+
+    Returns:
+        str: hostname
+
+    Examples:
+        >>> hn = hostname()
+        >>> isinstance(hn, str)
+        True
+
+    """
     return platform.node()
 
 
 def sys_path_sep() -> str:
-    """Return the system path separator string (; on windows -- : otherwise)"""
+    """Return the system path separator string (; on windows -- : otherwise)
+
+    Examples:
+        >>> sep = sys_path_sep()
+        >>> isinstance(sep, str)
+        True
+        >>> os.pathsep == sep
+        True
+
+    """
     return os.pathsep
 
 
 def syspath_paths(syspath: Optional[str] = None) -> List[str]:
-    """Return the current sys.path as a list"""
+    """Return the current sys.path as a list
+
+    Examples:
+        >>> sys_paths = syspath_paths()
+        >>> isinstance(sys_paths, list)
+        True
+        >>> sys_path_arg = 'path1;path2;path3' if is_win() else 'path1:path2:path3'
+        >>> sys_paths_w_args = syspath_paths(syspath=sys_path_arg)
+        >>> isinstance(sys_paths_w_args, list)
+        True
+        >>> sys_paths_w_args == ['path1', 'path2', 'path3']
+        True
+
+    """
     if syspath is None:
         return list(filter(None, sys.path))
     return list(filter(None, syspath.split(os.pathsep)))
-
-
-ismac = is_mac
-iswin = is_win
-iswsl = is_wsl
```

### Comparing `shellfish-0.2.2/shellfish/sh.py` & `shellfish-0.3.0/shellfish/sh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,46 @@
 # -*- coding: utf-8 -*-
 """shell utils"""
 from __future__ import annotations
 
-import asyncio
 import signal
 import sys
 
-from abc import ABC, abstractmethod
-from asyncio import TimeoutError
-from functools import lru_cache, reduce
-from operator import iconcat
+from functools import lru_cache
 from os import chdir, environ, fspath as _fspath, getcwd, listdir, makedirs, path
 from pathlib import Path
 from platform import system
 from shlex import quote as _quote, split as _shplit
 from shutil import which as _which
-from subprocess import (
-    DEVNULL,
-    PIPE,
-    CalledProcessError,
-    CompletedProcess,
-    SubprocessError,
-    run,
-)
+from subprocess import PIPE, CompletedProcess, SubprocessError, run
 from time import time
 from typing import (
     IO,
     Any,
     Callable,
     Dict,
     Iterable,
     List,
     Optional,
-    Sequence,
+    Set,
     Tuple,
     Type,
     Union,
 )
 
 from asyncify import asyncify
 from jsonbourne import JSON
 from jsonbourne.pydantic import JsonBaseModel
-from shellfish import fs
+from listless import flatten_strings as _flatten_strings
+from shellfish import fs, sp
 from shellfish._meta import __version__
+from shellfish._types import FsPath as FsPath, PopenArgs as PopenArgs
+from shellfish.dev import run_async as __run_async
 from shellfish.echo import echo as echo
 from shellfish.fs import (
-    Stdio as Stdio,
     SymlinkType as SymlinkType,
     chmod as chmod,
     copy_file as copy_file,
     cp as cp,
     dir_exists as dir_exists,
     dir_exists_async as dir_exists_async,
     dirpath_gen as dirpath_gen,
@@ -157,16 +148,16 @@
     wstr_async as wstr_async,
     wstring as wstring,
     wstring_async as wstring_async,
 )
 from shellfish.libsh._dirtree import _DirTree
 from shellfish.osfs import LIN as _LIN, WIN as _WIN
 from shellfish.process import is_win
-from shellfish.sp import PopenArgs
-from xtyping import STDIN, AnyStr, FsPath, IterableStr, TypedDict
+from shellfish.stdio import Stdio as Stdio
+from xtyping import STDIN, AnyStr, IterableStr, TypedDict
 
 __all__ = (
     "Done",
     "DoneError",
     "DoneObj",
     "Flag",
     "FlagMeta",
@@ -197,14 +188,15 @@
     "pstdout",
     "pstdout_pstderr",
     "pwd",
     "q",
     "quote",
     "run",
     "setenv",
+    "shell",
     "shplit",
     "shx",
     "source",
     "sync",
     "tree",
     "unlink_dir",
     "unlink_dirs",
@@ -377,21 +369,28 @@
         Tuple[int, int]: (seconds, nanoseconds)
 
     """
     _sec, _ns = divmod(int(seconds * 1_000_000_000), 1_000_000_000)
     return _sec, _ns
 
 
-class HrTimeObj(TypedDict):
+class HrTimeDict(TypedDict):
     """High resolution time"""
 
     sec: int
     ns: int
 
 
+class HrTimeObj(TypedDict):
+    """TODO: deprecate this in favor of HrTimeDict"""
+
+    sec: int
+    ns: int
+
+
 class HrTime(JsonBaseModel):
     """High resolution time"""
 
     sec: int
     ns: int
 
     @classmethod
@@ -404,14 +403,20 @@
         Returns:
             HrTime object
 
         """
         _sec, _ns = seconds2hrtime(seconds)
         return cls(sec=_sec, ns=_ns)
 
+    def hrdt_dict(self) -> HrTimeDict:
+        return {
+            "sec": self.sec,
+            "ns": self.ns,
+        }
+
     def hrdt_obj(self) -> HrTimeObj:
         return {
             "sec": self.sec,
             "ns": self.ns,
         }
 
 
@@ -447,15 +452,31 @@
             f"Command '{self.cmd}' returned non-zero exit status {self.returncode:d}."
         )
 
     def __str__(self) -> str:
         return f"{self.error_msg()}\n{self.done}"
 
 
+class DoneDict(TypedDict):
+    args: List[str]
+    returncode: int
+    stdout: str
+    stderr: str
+    ti: float
+    tf: float
+    dt: float
+    hrdt: Optional[HrTimeDict]
+    stdin: Optional[str]
+    async_proc: bool
+    verbose: bool
+
+
 class DoneObj(TypedDict):
+    """TODO: deprecate this in favor of DoneDict"""
+
     args: List[str]
     returncode: int
     stdout: str
     stderr: str
     ti: float
     tf: float
     dt: float
@@ -482,14 +503,19 @@
     dryrun: bool = False
 
     def __post_init__(self) -> None:
         """Write the stdout/stdout to sys.stdout/sys.stderr post object init"""
         if self.verbose:
             self.sys_print()
 
+    def hrdt_dict(self) -> HrTimeDict:
+        if self.hrdt:
+            return self.hrdt.hrdt_dict()
+        return HrTime.from_seconds(seconds=self.dt).hrdt_dict()
+
     def hrdt_obj(self) -> HrTimeObj:
         if self.hrdt:
             return self.hrdt.hrdt_obj()
         return HrTime.from_seconds(seconds=self.dt).hrdt_obj()
 
     def stdout_lines(self, keepends: bool = False) -> List[str]:
         return self.stdout.splitlines(keepends=keepends)
@@ -497,14 +523,30 @@
     def stderr_lines(self, keepends: bool = False) -> List[str]:
         return self.stderr.splitlines(keepends=keepends)
 
     @property
     def lines(self) -> List[str]:
         return self.stdout_lines(keepends=False)
 
+    def done_dict(self) -> DoneDict:
+        """Return Done object as typed-dict"""
+        return DoneDict(
+            args=self.args,
+            returncode=self.returncode,
+            stdout=self.stdout,
+            stderr=self.stderr,
+            ti=self.ti,
+            tf=self.tf,
+            dt=self.dt,
+            hrdt=self.hrdt_dict(),
+            stdin=self.stdin,
+            async_proc=self.async_proc,
+            verbose=self.verbose,
+        )
+
     def done_obj(self) -> DoneObj:
         """Return Done object typed dict"""
         return DoneObj(
             args=self.args,
             returncode=self.returncode,
             stdout=self.stdout,
             stderr=self.stderr,
@@ -517,15 +559,18 @@
             verbose=self.verbose,
         )
 
     def _error(self) -> DoneError:
         """Returns a CalledProcessError object"""
         return DoneError(done=self)
 
-    def check(self, ok_code: Union[int, Sequence[int]] = 0) -> None:
+    def check(
+        self,
+        ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
+    ) -> None:
         """Check returncode and stderr
 
         Raises:
             DoneError: If return code is non-zero and stderr is not None
 
         """
         if isinstance(ok_code, int):
@@ -747,27 +792,15 @@
     Examples:
         >>> list(flatten_args("cmd", ["uno", "dos", "tres"]))
         ['cmd', 'uno', 'dos', 'tres']
         >>> list(flatten_args("cmd", ["uno", "dos", "tres", ["4444", "five"]]))
         ['cmd', 'uno', 'dos', 'tres', '4444', 'five']
 
     """
-    return list(
-        map(
-            utf8_string,
-            reduce(
-                iconcat,
-                [
-                    flatten_args(*arg) if isinstance(arg, (list, tuple)) else (arg,)
-                    for arg in args
-                ],
-                [],
-            ),
-        )
-    )
+    return list(_flatten_strings(*args))
 
 
 def validate_popen_args(args: Union[PopenArgs, Tuple[PopenArgs, ...]]) -> List[str]:
     if len(args) == 0:
         raise ValueError("args must be a non-empty sequence")
     if len(args) == 1:
         _args = args[0]
@@ -794,43 +827,69 @@
         if fspath.lower().endswith(".cmd"):
             args[0] = str(fspath_obj.absolute())
         elif fspath.lower().endswith(".bat"):
             args[0] = str(fspath_obj.absolute())
     return args
 
 
+def _do_tee(
+    args: PopenArgs,
+    input: Optional[STDIN],
+    cwd: Optional[FsPath],
+    env: Optional[Dict[str, str]],
+    timeout: Optional[float],
+    shell: bool = False,
+) -> Done:
+    completed, pdt = sp.run_dtee(
+        args, input=input, cwd=cwd, env=env, timeout=timeout, shell=shell
+    )
+    return Done(
+        args=completed.args,
+        stdout=completed.stdout,
+        stderr=completed.stderr,
+        returncode=completed.returncode,
+        ti=pdt.ti,
+        tf=pdt.tf,
+        dt=pdt.dt,
+    )
+
+
 def _do(
     args: PopenArgs,
     *,
     env: Optional[Dict[str, str]] = None,
     extenv: bool = True,
     cwd: Optional[FsPath] = None,
     shell: bool = False,
     check: bool = False,
     verbose: bool = False,
     input: STDIN = None,
     timeout: Optional[int] = None,
     text: bool = False,
-    ok_code: Union[int, Sequence[int]] = 0,
+    tee: bool = False,
+    ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess synchronously
 
     Args:
         args: Args as strings for the subprocess
         env: Environment variables as a dictionary (Default value = None)
         extenv: Extend the environment with current environment (Default value = True)
         cwd: Current working directory (Default value = None)
         shell: Run in shell or sub-shell
         check: Check the outputs (generally useless)
         input: Stdin to give to the subprocess
         verbose (bool): Flag to write the subprocess stdout and stderr to
             sys.stdout and sys.stderr
+        tee (bool): Flag to tee the subprocess stdout and stderr to sys.stdout/stderr
         text: Flag to decode the output as text
         timeout (Optional[int]): Timeout in seconds for the process if not None
+        ok_code (Union[int, Sequence[int]]): Code(s) to consider as OK
+        dryrun (bool): Flag to not run the subprocess and return faux Done
 
     Returns:
         Finished PRun object which is a dictionary, so a dictionary
 
     Raises:
         ValueError: If args has pipe character (`|`)
 
@@ -862,14 +921,24 @@
             dt=0,
             hrdt=HrTime(sec=0, ns=0),
             verbose=verbose,
             stdin=_input if not isinstance(_input, bytes) else _input.decode(),
             dryrun=True,
         )
 
+    if tee:
+        return _do_tee(
+            args=args,
+            input=_input,
+            cwd=cwd,
+            env=_env,
+            timeout=timeout,
+            shell=shell,
+        )
+
     ti = time()
     proc = run(
         args=_args if IS_WIN or not shell else args_str,
         stdout=PIPE,
         stderr=PIPE,
         env=_env,
         cwd=cwd,
@@ -905,28 +974,29 @@
     extenv: bool = True,
     cwd: Optional[FsPath] = None,
     shell: bool = False,
     check: bool = False,
     verbose: bool = False,
     input: STDIN = None,
     timeout: Optional[int] = None,
-    ok_code: Union[int, Sequence[int]] = 0,
+    ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess synchronously
 
     Args:
         *popenargs: Args given as `*args`; Cannot use both *popenargs and args
         args: Args as strings for the subprocess
         env: Environment variables as a dictionary (Default value = None)
         extenv: Extend the environment with the current environment (Default value = True)
         cwd: Current working directory (Default value = None)
         shell: Run in shell or sub-shell
         check: Check the outputs (generally useless)
         input: Stdin to give to the subprocess
+        tee (bool): Flag to tee the subprocess stdout and stderr to sys.stdout/stderr
         verbose (bool): Flag to write the subprocess stdout and stderr to
             sys.stdout and sys.stderr
         timeout (Optional[int]): Timeout in seconds for the process if not None
         ok_code: Return code(s) to check against
         dryrun: Don't run the subprocess
 
     Returns:
@@ -953,26 +1023,26 @@
         input=_input,
         timeout=timeout,
         ok_code=ok_code,
         dryrun=dryrun,
     )
 
 
-def shx(
+def shell(
     *popenargs: PopenArgs,
     args: Optional[PopenArgs] = None,
     env: Optional[Dict[str, str]] = None,
     shell: bool = True,
     extenv: bool = True,
     cwd: Optional[FsPath] = None,
     check: bool = False,
     verbose: bool = False,
     input: STDIN = None,
     timeout: Optional[int] = None,
-    ok_code: Union[int, Sequence[int]] = 0,
+    ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess synchronously in current shell
 
     Args:
         *popenargs: Args given as `*args`; Cannot use both *popenargs and args
         args: Args as strings for the subprocess
@@ -981,14 +1051,17 @@
         extenv: Extend the environment with the current environment (Default value = True)
         cwd: Current working directory (Default value = None)
         check: Check the outputs (generally useless)
         input: Stdin to give to the subprocess
         verbose (bool): Flag to write the subprocess stdout and stderr to
             sys.stdout and sys.stderr
         timeout (Optional[int]): Timeout in seconds for the process if not None
+        ok_code: Return code(s) to check if ok
+        dryrun: Don't run the subprocess
+
 
     Returns:
         Finished PRun object which is a dictionary, so a dictionary
 
     """
     return do(
         *popenargs,
@@ -1002,23 +1075,16 @@
         input=input,
         timeout=timeout,
         ok_code=ok_code,
         dryrun=dryrun,
     )
 
 
-x = shx
-
-
-def args2cmd(args: PopenArgs) -> Union[str, bytes]:
-    """Return single command string from given popenargs"""
-    if isinstance(args, (str, bytes)):
-        return args
-    return " ".join(map(str, args))
-
+shx = shell
+x = shell
 
 _run_async = asyncify(run)
 _do_asyncify = asyncify(do)
 
 
 async def run_async(
     args: PopenArgs,
@@ -1036,15 +1102,15 @@
     errors: Optional[str] = None,
     text: bool = False,
     env: Optional[Dict[str, str]] = None,
     universal_newlines: bool = False,
     **other_popen_kwargs: Any,
 ) -> CompletedProcess[Any]:
     args = validate_popen_args(args)
-    complete_subprocess = await _run_async(
+    return await _run_async(
         args=args,
         input=input,
         stdin=stdin,
         stdout=stdout,
         stderr=stderr,
         shell=shell,
         cwd=cwd,
@@ -1053,43 +1119,41 @@
         errors=errors,
         env=env,
         capture_output=capture_output,
         universal_newlines=universal_newlines | text,
         encoding=encoding,
         **other_popen_kwargs,
     )
-    return complete_subprocess
 
 
 async def do_asyncify(
-    args: PopenArgs,
-    *,
+    *popenargs: PopenArgs,
+    args: Optional[PopenArgs] = None,
     env: Optional[Dict[str, str]] = None,
     extenv: bool = True,
     cwd: Optional[str] = None,
     shell: bool = False,
     verbose: bool = False,
     input: STDIN = None,
     check: bool = False,
-    loop: Optional[Any] = None,
     timeout: Optional[int] = None,
-    ok_code: Union[int, Sequence[int]] = 0,
+    ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess asynchronously using asyncified version of do"""
-    done = await _do_asyncify(  # type: ignore[call-arg]
+    done = await _do_asyncify(
+        *popenargs,
         args=args,
         env=env,
         extenv=extenv,
         cwd=cwd,
         shell=shell,
         verbose=verbose,
         input=input,
         check=check,
-        loop=loop,
         timeout=timeout,
         ok_code=ok_code,
         dryrun=dryrun,
     )
     done.async_proc = True
     return done
 
@@ -1100,17 +1164,16 @@
     env: Optional[Dict[str, str]] = None,
     extenv: bool = True,
     cwd: Optional[str] = None,
     shell: bool = False,
     verbose: bool = False,
     input: STDIN = None,
     check: bool = False,
-    loop: Optional[Any] = None,
     timeout: Optional[int] = None,
-    ok_code: Union[int, Sequence[int]] = 0,
+    ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess and await completion
 
     Args:
         args: Args as strings for the subprocess
         check (bool): Check the result returncode
@@ -1118,15 +1181,16 @@
         extenv: Extend environment with the current environment (Default value = True)
         cwd: Current working directory (Default value = None)
         shell: Run in shell or sub-shell
         input: Stdin to give to the subprocess
         verbose (bool): Flag to write the subprocess stdout and stderr to
             sys.stdout and sys.stderr
         timeout (Optional[int]): Timeout in seconds for the process if not None
-        loop: Event loop to use if have you use asyncified version (`do_asyncify`)
+        ok_code: Return code(s) to check if ok
+        dryrun: Don't run the subprocess
 
     Returns:
         Finished PRun object which is a dictionary, so a dictionary
 
     Raises:
         CalledProcessError: If check is True and the returncode is not 0
         TimeoutError: If the process takes longer than timeout if given
@@ -1138,45 +1202,39 @@
             args=args,
             env=env,
             cwd=cwd,
             shell=shell,
             verbose=verbose,
             input=input,
             check=check,
-            loop=loop,
             timeout=timeout,
             ok_code=ok_code,
             dryrun=dryrun,
         )
         done.async_proc = True
         return done
 
-    _default_asyncio_stream_limit = 2**16
-
     if input:
         input = validate_stdin(input)
     if isinstance(args, str):
         _args = [args]
-    if isinstance(args, bytes):
+    elif isinstance(args, bytes):
         _args = [utf8_string(args)]
     elif isinstance(args, (list, tuple)):
         _args = flatten_args(args)
     else:
         _args = list(map(str, args))
 
-    # stdin kwarg is DEVNULL if input is None else aio.PIPE
-    _stdin = DEVNULL if input is None else asyncio.subprocess.PIPE
     # input is None or bytes
     _input = input if not isinstance(input, str) else input.encode()
 
     _env = None if env is None else mkenv(env, extenv=extenv)
     _cwd = pwd()
     if cwd and path.exists(cwd) and path.isdir(cwd):
         _cwd = cwd
-
     if is_win():
         _syspath = None
         if env:
             _syspath = env.get("PATH", environ["PATH"])
 
         exe_path = which_lru(_args[0], path=_syspath)
         if exe_path:
@@ -1196,88 +1254,42 @@
                 ns=0,
             ),
             verbose=verbose,
             stdin=_input if not isinstance(_input, bytes) else _input.decode(),
             dryrun=True,
             async_proc=True,
         )
+    _proc, _pdt = await __run_async.run_dtee_async(
+        *_args,
+        env=_env,
+        cwd=_cwd,
+        shell=shell,
+        ok_code=ok_code if isinstance(ok_code, (list, tuple, set)) else {ok_code},
+        check=check,
+        capture_output=True,
+        timeout=timeout,
+        input=_input,
+        universal_newlines=True,
+    )
 
-    if shell:
-        _cmd = args2cmd(_args)
-        ti = time()
-        _proc = await asyncio.create_subprocess_shell(
-            cmd=_cmd,
-            stdin=_stdin,
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
-            env=_env,
-            shell=True,
-            limit=_default_asyncio_stream_limit,
-            cwd=_cwd,
-        )
-    else:
-        ti = time()
-        _proc = await asyncio.create_subprocess_exec(
-            *_args,
-            stdin=_stdin,
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
-            env=_env,
-            limit=_default_asyncio_stream_limit,
-            cwd=_cwd,
-        )
-
-    if timeout:
-        try:
-            (stdout, stderr) = await asyncio.wait_for(
-                _proc.communicate(input=_input),  # wait for subprocess to finish
-                timeout=timeout,
-            )
-            tf = time()
-        except TimeoutError as te:
-            _proc.terminate()
-            raise TimeoutError(
-                str(
-                    {
-                        "args": args,
-                        "input": input,
-                        "env": env,
-                        "cwd": cwd,
-                        "shell": shell,
-                        "asyncio.TimeoutError": str(te),
-                    }
-                )
-            )
-
-    else:
-        (stdout, stderr) = await _proc.communicate(input=_input)  # wait fo
-        tf = time()
-
-    if check or ok_code != 0:
-        _ok_codes = {ok_code} if isinstance(ok_code, int) else set(ok_code)
-        if _proc.returncode and _proc.returncode not in _ok_codes:
-            raise CalledProcessError(
-                returncode=_proc.returncode,
-                output=stdout,
-                stderr=stderr,
-                cmd=str(args),
-            )
     _args_array = (
         list(map(str, args)) if isinstance(args, (list, tuple)) else [str(args)]
     )
     return Done(
         args=_args_array,
         returncode=_proc.returncode or -1,
-        stdout=decode_stdio_bytes(stdout),
-        stderr=decode_stdio_bytes(stderr),
+        stdout=decode_stdio_bytes(_proc.stdout),
+        stderr=decode_stdio_bytes(_proc.stderr),
         stdin=input.decode(encoding="utf-8") if isinstance(input, bytes) else None,
-        ti=ti,
-        tf=tf,
-        dt=tf - ti,
-        hrdt=HrTime.from_seconds(tf - ti),
+        ti=_pdt.ti,
+        tf=_pdt.tf,
+        dt=_pdt.dt,
+        hrdt=HrTime.from_seconds(
+            _pdt.dt,
+        ),
         verbose=verbose,
         async_proc=True,
     )
 
 
 async def do_async(
     *popenargs: PopenArgs,
@@ -1285,17 +1297,16 @@
     env: Optional[Dict[str, str]] = None,
     extenv: bool = True,
     cwd: Optional[str] = None,
     shell: bool = False,
     verbose: bool = False,
     input: STDIN = None,
     check: bool = False,
-    loop: Optional[Any] = None,
     timeout: Optional[int] = None,
-    ok_code: Union[Sequence[int], int] = 0,
+    ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess and await its completion
 
     Args:
         *popenargs: Args given as `*args`; Cannot use both *popenargs and args
         args: Args as strings for the subprocess
@@ -1304,15 +1315,16 @@
         extenv: Extend environment with the current environment (Default value = True)
         cwd: Current working directory (Default value = None)
         shell: Run in shell or sub-shell
         input: Stdin to give to the subprocess
         verbose (bool): Flag to write the subprocess stdout and stderr to
             sys.stdout and sys.stderr
         timeout (Optional[int]): Timeout in seconds for the process if not None
-        loop: Optional event loop to run subprocess in
+        ok_code: Return code(s) that are considered OK (Default value = 0)
+        dryrun (bool): Flag to not run the subprocess but return a Done object
 
     Returns:
         Finished PRun object which is a dictionary, so a dictionary
 
     Raises:
         ValueError: If both *popenargs and args are given
 
@@ -1326,15 +1338,14 @@
             env=env,
             extenv=extenv,
             cwd=cwd,
             shell=shell,
             verbose=verbose,
             input=input,
             check=check,
-            loop=loop,
             timeout=timeout,
             ok_code=ok_code,
             dryrun=dryrun,
         )
         done.async_proc = True
         return done
     if not shell and is_win():
@@ -1344,15 +1355,14 @@
         env=env,
         extenv=extenv,
         cwd=cwd,
         shell=shell,
         verbose=verbose,
         input=input,
         check=check,
-        loop=loop,
         timeout=timeout,
         ok_code=ok_code,
         dryrun=dryrun,
     )
 
 
 do_ = do_async
@@ -1364,17 +1374,16 @@
     env: Optional[Dict[str, str]] = None,
     extenv: bool = True,
     cwd: Optional[str] = None,
     shell: bool = False,
     verbose: bool = False,
     input: STDIN = None,
     check: bool = False,
-    loop: Optional[Any] = None,
     timeout: Optional[int] = None,
-    ok_code: Union[int, Sequence[int]] = 0,
+    ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess and await its completion
 
     Alias for sh.do_async
 
     Args:
@@ -1384,15 +1393,17 @@
         env: Environment variables as a dictionary (Default value = None)
         cwd: Current working directory (Default value = None)
         shell: Run in shell or sub-shell
         input: Stdin to give to the subprocess
         verbose (bool): Flag to write the subprocess stdout and stderr to
             sys.stdout and sys.stderr
         timeout (Optional[int]): Timeout in seconds for the process if not None
-        loop: Optional event loop to run subprocess in
+        ok_code: Return code(s) that are considered OK (Default value = 0)
+        dryrun (bool): Flag to not run the subprocess but return a Done object
+        extenv: Extend environment with the current environment (Default value = True)
 
     Returns:
         Finished PRun object which is a dictionary, so a dictionary
 
     """
     return await do_async(
         *popenargs,
@@ -1400,15 +1411,14 @@
         env=env,
         extenv=extenv,
         cwd=cwd,
         shell=shell,
         verbose=verbose,
         input=input,
         check=check,
-        loop=loop,
         timeout=timeout,
         ok_code=ok_code,
         dryrun=dryrun,
     )
 
 
 # =============================================================================
@@ -1417,86 +1427,14 @@
 #  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\
 # /  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \
 # =============================================================================
 # \/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\
 # =============================================================================
 
 
-class OSABC(ABC):
-    """Abstract base class for OS-specific fns"""
-
-    @staticmethod
-    @abstractmethod
-    def sync(
-        src: str,
-        dest: str,
-        *,
-        delete: bool = False,
-        mkdirs: bool = False,
-        dry_run: bool = False,
-        exclude: Optional[IterableStr] = None,
-        include: Optional[IterableStr] = None,
-    ) -> Done:
-        ...
-
-    @staticmethod
-    @abstractmethod
-    def link_dir(linkpath: str, targetpath: str, *, exist_ok: bool = False) -> None:
-        ...
-
-    @staticmethod
-    @abstractmethod
-    def link_dirs(
-        link_target_tuples: List[Tuple[str, str]], *, exist_ok: bool = False
-    ) -> None:
-        ...
-
-    @staticmethod
-    @abstractmethod
-    def link_file(linkpath: str, targetpath: str, *, exist_ok: bool = False) -> None:
-        ...
-
-    @staticmethod
-    @abstractmethod
-    def link_files(
-        link_target_tuples: List[Tuple[str, str]], *, exist_ok: bool = False
-    ) -> None:
-        ...
-
-    @staticmethod
-    @abstractmethod
-    def unlink_dir(link: str) -> None:
-        ...
-
-    @staticmethod
-    @abstractmethod
-    def unlink_dirs(links: IterableStr) -> None:
-        ...
-
-    @staticmethod
-    @abstractmethod
-    def unlink_file(link: str) -> None:
-        ...
-
-    @staticmethod
-    @abstractmethod
-    def unlink_files(links: IterableStr) -> None:
-        ...
-
-
-# =============================================================================
-# /\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/
-# =============================================================================
-#  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\
-# /  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \
-# =============================================================================
-# \/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\
-# =============================================================================
-
-
 class LIN(_LIN):
     """Linux (and Mac) shell commands/methods container"""
 
     @staticmethod
     def rsync_args(
         src: str,
         dest: str,
@@ -1745,15 +1683,15 @@
         dest: str,
         *,
         mkdirs: bool = True,
         delete: bool = False,
         exclude_files: Optional[Iterable[str]] = None,
         exclude_dirs: Optional[Iterable[str]] = None,
         dry_run: bool = False,
-    ) -> Done:
+    ) -> Done:  # pragma: nocov
         """Robocopy wrapper function (crude in that it opens a subprocess)
 
         Args:
             src (str): path to source directory
             dest (str): path to destination directory
             delete (bool): Delete files in the destination directory if they do
                 not exist in the source directory
@@ -1807,15 +1745,15 @@
         dest: str,
         *,
         delete: bool = False,
         mkdirs: bool = False,
         dry_run: bool = False,
         exclude: Optional[IterableStr] = None,
         include: Optional[IterableStr] = None,
-    ) -> Done:
+    ) -> Done:  # pragma: nocov
         return WIN.robocopy(
             src=src,
             dest=dest,
             mkdirs=mkdirs,
             delete=delete,
             exclude_files=exclude,
             exclude_dirs=include,
@@ -1951,20 +1889,48 @@
 
 def shplit(string: str, comments: bool = False, posix: bool = True) -> List[str]:
     """Typed alias for shlex.split"""
     return _shplit(string, comments=comments, posix=posix)
 
 
 def quote(string: str) -> str:
-    """Typed alias for shlex.quote"""
+    """Typed alias for shlex.quote
+
+    Args:
+        string (str): string to quote
+
+    Returns:
+        str: quoted string
+
+    Examples:
+        >>> quote("hello world")
+        "'hello world'"
+        >>> quote("hello 'world'")
+        '\\'hello \\'"\\'"\\'world\\'"\\'"\\'\\''
+
+    """
     return _quote(string)
 
 
 def q(string: str) -> str:
-    """Typed alias for shlex.quote"""
+    """Typed alias for shlex.quote
+
+    Args:
+        string (str): string to quote
+
+    Returns:
+        str: quoted string
+
+    Examples:
+        >>> q("hello world")
+        "'hello world'"
+        >>> q("hello 'world'")
+        '\\'hello \\'"\\'"\\'world\\'"\\'"\\'\\''
+
+    """
     return _quote(string)
 
 
 def which(cmd: str, path: Optional[str] = None) -> Optional[str]:
     """Return the result of `shutil.which`
 
     Args:
@@ -2153,18 +2119,18 @@
         dirpath (FsPath): path-string to directory to list
         abspath (bool): Give absolute paths
 
     Returns:
         List of the directory items
 
     """
+    items = await listdir_async(dirpath)
     if abspath:
-        items = await listdir_async(dirpath)
         return [path.join(dirpath, el) for el in items]
-    return await listdir_async(dirpath)
+    return items
 
 
 def rm(
     fspath: FsPath,
     *,
     force: bool = False,
     recursive: bool = False,
@@ -2207,15 +2173,15 @@
         src (FsPath): source file(s)
         dest (FsPath): destination path
 
     """
     fs.move(src, dest)
 
 
-def source(filepath: FsPath, _globals: bool = True) -> None:
+def source(filepath: FsPath, _globals: bool = True) -> None:  # pragma: nocov
     """Execute/run a python file given a fspath and put globals in globasl
 
     Args:
         filepath (FsPath): Path to python file
         _globals (bool): Exec using globals
 
     """
```

### Comparing `shellfish-0.2.2/shellfish/testing.py` & `shellfish-0.3.0/shellfish/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,22 +30,37 @@
         return True
     except AssertionError:
         ...
     return False
 
 
 def random_string(length: int = 10) -> str:
-    """Return a random string of a given length (defaults to 10)"""
+    """Return a random string of a given length (defaults to 10)
+
+    Examples:
+        >>> string = random_string(10)
+        >>> len(string) == 10
+        True
+
+    """
     return "".join(
         rand_choice(string.ascii_letters + string.digits) for _ in range(length)
     )
 
 
 def random_directory_path(depth: int = 4) -> str:
-    """Return a random directory path with a given depth (defaults to 4)"""
+    """Return a random directory path with a given depth (defaults to 4)
+
+    Examples:
+        >>> from os import sep
+        >>> dirpath = random_directory_path(4)
+        >>> len(dirpath.split(sep)) == 4
+        True
+
+    """
     return str(path.join(*(random_string(randint(1, 5)) for s in range(depth))))
 
 
 def mk_random_dirtree(
     dest: Optional[str] = None,
     n_subdirectories: int = 8,
     max_subdirectory_files: int = 4,
```

### Comparing `shellfish-0.2.2/PKG-INFO` & `shellfish-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellfish
-Version: 0.2.2
+Version: 0.3.0
 Summary: shellfish ~ shell & file-system utils
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/shellfish
 License: MIT
 Keywords: dgpy,shell,fs,filesystem,typed
 Author: jesse
 Author-email: jesse@dgi.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shellfish Version: 0.2.2 Summary: shellfish ~ shell
+Metadata-Version: 2.1 Name: shellfish Version: 0.3.0 Summary: shellfish ~ shell
 & file-system utils Home-page: https://github.com/dynamic-graphics-inc/dgpy-
 libs/tree/main/libs/shellfish License: MIT Keywords:
 dgpy,shell,fs,filesystem,typed Author: jesse Author-email: jesse@dgi.com
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

