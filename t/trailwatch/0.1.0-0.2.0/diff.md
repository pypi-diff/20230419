# Comparing `tmp/trailwatch-0.1.0.tar.gz` & `tmp/trailwatch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trailwatch-0.1.0.tar", max compression
+gzip compressed data, was "trailwatch-0.2.0.tar", max compression
```

## Comparing `trailwatch-0.1.0.tar` & `trailwatch-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1047 2023-03-28 23:02:21.055220 trailwatch-0.1.0/LICENSE
--rw-r--r--   0        0        0     1075 2023-03-28 23:02:21.055220 trailwatch-0.1.0/README.md
--rw-r--r--   0        0        0     1900 2023-03-28 23:02:21.055220 trailwatch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2250 2023-03-28 23:02:21.055220 trailwatch-0.1.0/src/trailwatch/__init__.py
--rw-r--r--   0        0        0     6010 2023-03-28 23:02:21.055220 trailwatch-0.1.0/src/trailwatch/config.py
--rw-r--r--   0        0        0       65 2023-03-28 23:02:21.055220 trailwatch-0.1.0/src/trailwatch/connectors/__init__.py
--rw-r--r--   0        0        0       71 2023-03-28 23:02:21.055220 trailwatch-0.1.0/src/trailwatch/connectors/aws/__init__.py
--rw-r--r--   0        0        0     4103 2023-03-28 23:02:21.055220 trailwatch-0.1.0/src/trailwatch/connectors/aws/api.py
--rw-r--r--   0        0        0     4370 2023-03-28 23:02:21.055220 trailwatch-0.1.0/src/trailwatch/connectors/aws/connector.py
--rw-r--r--   0        0        0      816 2023-03-28 23:02:21.055220 trailwatch-0.1.0/src/trailwatch/connectors/aws/handler.py
--rw-r--r--   0        0        0      866 2023-03-28 23:02:21.055220 trailwatch-0.1.0/src/trailwatch/connectors/base.py
--rw-r--r--   0        0        0     3074 2023-03-28 23:02:21.055220 trailwatch-0.1.0/src/trailwatch/context.py
--rw-r--r--   0        0        0      414 2023-03-28 23:02:21.059220 trailwatch-0.1.0/src/trailwatch/exceptions.py
--rw-r--r--   0        0        0     1729 1970-01-01 00:00:00.000000 trailwatch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-18 23:24:19.015464 trailwatch-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2988 2023-04-18 23:24:19.015464 trailwatch-0.2.0/README.md
+-rw-r--r--   0        0        0     2026 2023-04-18 23:24:19.015464 trailwatch-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2811 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/__init__.py
+-rw-r--r--   0        0        0     6071 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/config.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/connectors/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/connectors/aws/__init__.py
+-rw-r--r--   0        0        0     4103 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/connectors/aws/api.py
+-rw-r--r--   0        0        0     3453 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/connectors/aws/connector.py
+-rw-r--r--   0        0        0      809 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/connectors/aws/handler.py
+-rw-r--r--   0        0        0      930 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/connectors/base.py
+-rw-r--r--   0        0        0     3030 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/context.py
+-rw-r--r--   0        0        0      414 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/exceptions.py
+-rw-r--r--   0        0        0     3714 1970-01-01 00:00:00.000000 trailwatch-0.2.0/PKG-INFO
```

### Comparing `trailwatch-0.1.0/src/trailwatch/__init__.py` & `trailwatch-0.2.0/src/trailwatch/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,67 @@
 __all__ = [
     "configure",
-    "AwsConnector",
     "TrailwatchContext",
     "watch",
 ]
 
 import functools
+import signal
 
-from typing import Optional, Union
-
-from .config import NOTSET, configure
-from .connectors import AwsConnector
+from .config import DEFAULT, Default, configure
 from .context import TrailwatchContext
+from .exceptions import ExecutionTimeoutError
+
+
+def throw_timeout_on_alarm(signum, frame):
+    raise ExecutionTimeoutError
 
 
-# TODO - add timeout configuration; add support for uploading files
+signal.signal(signal.SIGALRM, throw_timeout_on_alarm)
+
+
+# TODO - add support for uploading files (use locals() to get execution context)
 def watch(
-    job: Optional[str] = None,
-    job_description: Optional[str] = None,
-    loggers: Union[Optional[list[str]], object] = NOTSET,
-    execution_ttl: Union[Optional[int], object] = NOTSET,
-    log_ttl: Union[Optional[int], object] = NOTSET,
-    error_ttl: Union[Optional[int], object] = NOTSET,
+    job: str | None = None,
+    job_description: str | None = None,
+    loggers: list[str] | Default | None = DEFAULT,
+    execution_ttl: int | Default | None = DEFAULT,
+    log_ttl: int | Default | None = DEFAULT,
+    error_ttl: int | Default | None = DEFAULT,
+    timeout: int | None = None,
 ):
     """
-    Initialize a TrailwatchContext instance for a job.
+    Watch a callable (function or method).
+
+    This is a decorator that can be used to wrap a callable (function or method)
+    and send execution statistics (start, end, name, logs, exceptions, etc.)
+    to configured connectors.
 
     Parameters
     ----------
     job : str
         Job name. E.g., 'Upsert appointments'.
     job_description : str
         Job description. E.g., 'Upsert appointments from ModMed to Salesforce'.
-    loggers : Optional[list[str]], optional
-        List of loggers logs from which are sent to Trailwatch.
+    loggers : list[str], optional
+        List of loggers logs from which are sent to TrailWatch.
         By default, no logs are sent.
-    execution_ttl : Optional[int], optional
+    execution_ttl : int, optional
         Time to live for the execution record in seconds.
         By default, global configuration is used.
-    log_ttl : Optional[int], optional
+    log_ttl : int, optional
         Time to live for the log records in seconds.
         By default, global configuration is used.
-    error_ttl : Optional[int], optional
+    error_ttl : int, optional
         Time to live for the error records in seconds.
         By default, global configuration is used.
+    timeout : int, optional
+        Timeout in seconds. If the callable takes longer than this to execute,
+        an execution timeout error is raised and execution is marked as timed out.
+        By default, no timeout is set.
 
     """
 
     def wrapper(func):
         decorator_kwargs = {
             "job": job or func.__name__,
             "job_description": job_description or func.__doc__,
@@ -60,13 +74,15 @@
             raise ValueError(
                 "Job description must either be provided explicitly or "
                 "via the docstring of the decorated function"
             )
 
         @functools.wraps(func)
         def inner(*args, **kwargs):
+            if timeout is not None:
+                signal.alarm(timeout)
             with TrailwatchContext(**decorator_kwargs):
                 return func(*args, **kwargs)
 
         return inner
 
     return wrapper
```

### Comparing `trailwatch-0.1.0/src/trailwatch/config.py` & `trailwatch-0.2.0/src/trailwatch/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,88 @@
 from dataclasses import dataclass, field
-from typing import Optional, Union
 
-from trailwatch.connectors.base import ConnectorBase
+from trailwatch.connectors.base import ConnectorFactory
 
 from .exceptions import NotConfiguredError
 
-NOTSET = object()
+
+class Default:
+    """
+    Sentinel value to indicate that user did not set a value.
+
+    Used to distinguish between None and using globally configured value.
+
+    """
+
+
+DEFAULT = Default()
 
 
 @dataclass(frozen=True)
 class SharedConfiguration:
     is_configured: bool = False
-    connectors: list[ConnectorBase] = field(default_factory=list)
+    connectors: list[ConnectorFactory] = field(default_factory=list)
 
     project: str = ""
     project_description: str = ""
     environment: str = ""
     loggers: list[str] = field(default_factory=list)
-    execution_ttl: Optional[int] = None
-    log_ttl: Optional[int] = None
-    error_ttl: Optional[int] = None
+    execution_ttl: int | None = None
+    log_ttl: int | None = None
+    error_ttl: int | None = None
 
 
 class TrailwatchConfig:
     shared_configuration: SharedConfiguration = SharedConfiguration()
 
     # Job-specific properties
     job: str
     job_description: str
 
     # Shared properties which can be overridden for each job
-    _loggers: Union[Optional[list[str]], object]
-    _execution_ttl: Union[Optional[int], object]
-    _log_ttl: Union[Optional[int], object]
-    _error_ttl: Union[Optional[int], object]
+    _loggers: list[str] | Default | None
+    _execution_ttl: int | Default | None
+    _log_ttl: int | Default | None
+    _error_ttl: int | Default | None
 
     def __init__(
         self,
         job: str,
         job_description: str,
-        loggers: Union[Optional[list[str]], object] = NOTSET,
-        execution_ttl: Union[Optional[int], object] = NOTSET,
-        log_ttl: Union[Optional[int], object] = NOTSET,
-        error_ttl: Union[Optional[int], object] = NOTSET,
+        loggers: list[str] | Default | None = DEFAULT,
+        execution_ttl: int | Default | None = DEFAULT,
+        log_ttl: int | Default | None = DEFAULT,
+        error_ttl: int | Default | None = DEFAULT,
     ) -> None:
         """
         Initialize a TrailwatchConfig instance for a job.
 
         Parameters
         ----------
         job : str
             Job name. E.g., 'Upsert appointments'.
         job_description : str
             Job description. E.g., 'Upsert appointments from ModMed to Salesforce'.
-        loggers : Optional[list[str]], optional
-            List of loggers logs from which are sent to Trailwatch.
+        loggers : list[str], optional
+            List of loggers logs from which are sent to TrailWatch.
             By default, no logs are sent.
-        execution_ttl : Optional[int], optional
+        execution_ttl : int, optional
             Time to live for the execution record in seconds.
             By default, global configuration is used.
-        log_ttl : Optional[int], optional
+        log_ttl : int, optional
             Time to live for the log records in seconds.
             By default, global configuration is used.
-        error_ttl : Optional[int], optional
+        error_ttl : int, optional
             Time to live for the error records in seconds.
             By default, global configuration is used.
 
         """
         if not self.shared_configuration.is_configured:
             raise NotConfiguredError(
-                "Trailwatch must be configured with trailwatch.configure() before using"
+                "TrailWatch must be configured with trailwatch.configure() before using"
             )
         self.job = job
         self.job_description = job_description
         self._loggers = loggers or []
         self._execution_ttl = execution_ttl
         self._log_ttl = log_ttl
         self._error_ttl = error_ttl
@@ -88,53 +97,53 @@
 
     @property
     def environment(self) -> str:
         return self.shared_configuration.environment
 
     @property
     def loggers(self) -> list[str]:
-        if self._loggers is not NOTSET:
+        if self._loggers is not DEFAULT:
             assert isinstance(self._loggers, (list, type(None)))
             return self._loggers or []
         return self.shared_configuration.loggers
 
     @property
-    def execution_ttl(self) -> Optional[int]:
-        if self._execution_ttl is not NOTSET:
+    def execution_ttl(self) -> int | None:
+        if self._execution_ttl is not DEFAULT:
             assert isinstance(self._execution_ttl, (int, type(None)))
             return self._execution_ttl
         return self.shared_configuration.execution_ttl
 
     @property
-    def log_ttl(self) -> Optional[int]:
-        if self._log_ttl is not NOTSET:
+    def log_ttl(self) -> int | None:
+        if self._log_ttl is not DEFAULT:
             assert isinstance(self._log_ttl, (int, type(None)))
             return self._log_ttl
         return self.shared_configuration.log_ttl
 
     @property
-    def error_ttl(self) -> Optional[int]:
-        if self._error_ttl is not NOTSET:
+    def error_ttl(self) -> int | None:
+        if self._error_ttl is not DEFAULT:
             assert isinstance(self._error_ttl, (int, type(None)))
             return self._error_ttl
         return self.shared_configuration.error_ttl
 
 
 def configure(
     project: str,
     project_description: str,
     environment: str,
-    connectors: list[ConnectorBase],
-    loggers: Optional[list[str]] = None,
-    execution_ttl: Optional[int] = None,
-    log_ttl: Optional[int] = None,
-    error_ttl: Optional[int] = None,
+    connectors: list[ConnectorFactory],
+    loggers: list[str] | None = None,
+    execution_ttl: int | None = None,
+    log_ttl: int | None = None,
+    error_ttl: int | None = None,
 ):
     """
-    Configure Trailwatch.
+    Configure TrailWatch.
 
     This function configures global settings shared across all executions unless
     explicitly overridden for a specific job.
     This function must be called once per process.
 
     Parameters
     ----------
@@ -143,24 +152,26 @@
         E.g., 'companyname-middleware'.
     project_description : str
         User-friendly description of the project.
         E.g., 'Synchronize appointment data from ModMed with companyname's Salesforce'.
     environment : str
         Environment in which all jobs are executed.
         E.g., 'production', 'staging', 'development'.
-    loggers : Optional[list[str]], optional
-        List of loggers logs from which are sent to Trailwatch.
+    connectors : list[ConnectorFactoryBase]
+        List of connectors to use.
+    loggers : list[str], optional
+        List of loggers logs from which are sent to TrailWatch.
         By default, no logs are sent.
-    execution_ttl : Optional[int], optional
+    execution_ttl : int, optional
         Time to live for the execution record in seconds.
         By default, the execution record is kept indefinitely.
-    log_ttl : Optional[int], optional
+    log_ttl : int, optional
         Time to live for the log records in seconds.
         By default, the log records are kept indefinitely.
-    error_ttl : Optional[int], optional
+    error_ttl : int, optional
         Time to live for the error records in seconds.
         By default, the error records are kept indefinitely.
 
     """
     if len(connectors) == 0:
         raise ValueError("At least one connector must be configured")
     TrailwatchConfig.shared_configuration = SharedConfiguration(
```

### Comparing `trailwatch-0.1.0/src/trailwatch/connectors/aws/api.py` & `trailwatch-0.2.0/src/trailwatch/connectors/aws/api.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.1.0/src/trailwatch/connectors/base.py` & `trailwatch-0.2.0/src/trailwatch/connectors/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,38 +4,31 @@
 from types import TracebackType
 from typing import TYPE_CHECKING, Type
 
 if TYPE_CHECKING:
     from trailwatch.config import TrailwatchConfig
 
 
-class ConnectorBase(ABC):
-    @abstractmethod
-    def reset(self) -> None:
-        ...
-
-    @property
-    @abstractmethod
-    def is_configured(self) -> bool:
-        ...
-
-    @abstractmethod
-    def configure(self, config: "TrailwatchConfig") -> None:
-        ...
-
+class Connector(ABC):
     @abstractmethod
     def start_execution(self) -> None:
-        ...
+        """Create execution record, attach handlers, etc."""
 
     @abstractmethod
     def finalize_execution(self, status: str, end: datetime.datetime) -> None:
-        ...
+        """Update execution record, detach handlers, etc."""
 
     @abstractmethod
     def handle_exception(
         self,
         timestamp: datetime.datetime,
         exc_type: Type[Exception],
         exc_value: Exception,
         exc_traceback: TracebackType,
     ):
-        ...
+        """Add exception to execution record (or do nothing)."""
+
+
+class ConnectorFactory(ABC):
+    @abstractmethod
+    def __call__(self, config: "TrailwatchConfig") -> Connector:
+        """Create connector instance."""
```

### Comparing `trailwatch-0.1.0/src/trailwatch/context.py` & `trailwatch-0.2.0/src/trailwatch/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,87 @@
-from __future__ import annotations
-
 import datetime
 
 from types import TracebackType
-from typing import Optional, Type, Union
+from typing import Type
 
-from .config import NOTSET, TrailwatchConfig
+from .config import DEFAULT, Default, TrailwatchConfig
+from .connectors.base import Connector
 from .exceptions import ExecutionTimeoutError, PartialSuccessError, TrailwatchError
 
 
 class TrailwatchContext:
     def __init__(
         self,
         job: str,
         job_description: str,
-        loggers: Union[Optional[list[str]], object] = NOTSET,
-        execution_ttl: Union[Optional[int], object] = NOTSET,
-        log_ttl: Union[Optional[int], object] = NOTSET,
-        error_ttl: Union[Optional[int], object] = NOTSET,
+        loggers: list[str] | Default | None = DEFAULT,
+        execution_ttl: int | Default | None = DEFAULT,
+        log_ttl: int | Default | None = DEFAULT,
+        error_ttl: int | Default | None = DEFAULT,
     ) -> None:
         """
         Initialize a TrailwatchContext instance for a job.
 
         Parameters
         ----------
         job : str
             Job name. E.g., 'Upsert appointments'.
         job_description : str
             Job description. E.g., 'Upsert appointments from ModMed to Salesforce'.
-        loggers : Optional[list[str]], optional
-            List of loggers logs from which are sent to Trailwatch.
+        loggers : list[str], optional
+            List of loggers logs from which are sent to TrailWatch.
             By default, no logs are sent.
-        execution_ttl : Optional[int], optional
+        execution_ttl : int, optional
             Time to live for the execution record in seconds.
-        log_ttl : Optional[int], optional
+        log_ttl : int, optional
             Time to live for the log records in seconds.
-        error_ttl : Optional[int], optional
+        error_ttl : int, optional
             Time to live for the error records in seconds.
 
         """
         self.config = TrailwatchConfig(
             job=job,
             job_description=job_description,
             loggers=loggers,
             execution_ttl=execution_ttl,
             log_ttl=log_ttl,
             error_ttl=error_ttl,
         )
+        self.connectors: list[Connector] = []
 
-    def __enter__(self) -> TrailwatchContext:
-        for connector in self.config.shared_configuration.connectors:
-            connector.reset()
-            connector.configure(self.config)
+    def __enter__(self) -> "TrailwatchContext":
+        for connector_factory in self.config.shared_configuration.connectors:
+            connector = connector_factory(self.config)
             connector.start_execution()
+            self.connectors.append(connector)
         return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[Exception]],
-        exc_value: Optional[Exception],
-        exc_traceback: Optional[TracebackType],
+        exc_type: Type[Exception] | None,
+        exc_value: Exception | None,
+        exc_traceback: TracebackType | None,
     ) -> bool:
         end = datetime.datetime.utcnow()
         if exc_type is None:
             status = "success"
         else:
             if issubclass(exc_type, ExecutionTimeoutError):
                 status = "timeout"
             elif issubclass(exc_type, PartialSuccessError):
                 status = "partial"
             else:
                 status = "failure"
-        for connector in self.config.shared_configuration.connectors:
+        for connector in self.connectors:
             connector.finalize_execution(status, end)
             if exc_type is not None and not issubclass(exc_type, TrailwatchError):
                 assert exc_value is not None
                 assert exc_traceback is not None
                 connector.handle_exception(
                     timestamp=end,
                     exc_type=exc_type,
                     exc_value=exc_value,
                     exc_traceback=exc_traceback,
                 )
-
-        if exc_type is None or issubclass(exc_type, TrailwatchError):
+        if isinstance(exc_type, PartialSuccessError):
             return True
         return False
```

