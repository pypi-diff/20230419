# Comparing `tmp/py3_tts-3.0b0-py3-none-any.whl.zip` & `tmp/py3_tts-3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 38715 bytes, number of entries: 16
--rw-r--r--  2.0 unx      782 b- defN 23-Apr-03 04:07 pyttsx3/__init__.py
--rw-r--r--  2.0 unx     6621 b- defN 23-Apr-03 04:07 pyttsx3/driver.py
--rw-r--r--  2.0 unx     7004 b- defN 23-Apr-03 04:07 pyttsx3/engine.py
--rw-r--r--  2.0 unx    28688 b- defN 23-Apr-03 04:07 pyttsx3/six.py
--rw-r--r--  2.0 unx      417 b- defN 23-Apr-03 04:07 pyttsx3/voice.py
--rw-r--r--  2.0 unx      830 b- defN 23-Apr-03 04:07 pyttsx3/drivers/__init__.py
--rw-r--r--  2.0 unx    19000 b- defN 23-Apr-03 04:07 pyttsx3/drivers/_espeak.py
--rw-r--r--  2.0 unx     6008 b- defN 23-Apr-03 04:07 pyttsx3/drivers/dummy.py
--rw-r--r--  2.0 unx     6614 b- defN 23-Apr-03 04:07 pyttsx3/drivers/espeak.py
--rw-r--r--  2.0 unx     3623 b- defN 23-Apr-03 04:07 pyttsx3/drivers/nsss.py
--rw-r--r--  2.0 unx     5184 b- defN 23-Apr-03 04:07 pyttsx3/drivers/sapi5.py
--rw-r--r--  2.0 unx    16725 b- defN 23-Apr-03 04:08 py3_tts-3.0b0.dist-info/LICENSE
--rw-r--r--  2.0 unx    23754 b- defN 23-Apr-03 04:08 py3_tts-3.0b0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-03 04:08 py3_tts-3.0b0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-03 04:08 py3_tts-3.0b0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1245 b- defN 23-Apr-03 04:08 py3_tts-3.0b0.dist-info/RECORD
-16 files, 126595 bytes uncompressed, 36695 bytes compressed:  71.0%
+Zip file size: 38723 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      782 b- defN 23-Apr-19 03:10 pyttsx3/__init__.py
+-rw-r--r--  2.0 unx     6619 b- defN 23-Apr-19 03:10 pyttsx3/driver.py
+-rw-r--r--  2.0 unx     7005 b- defN 23-Apr-19 03:10 pyttsx3/engine.py
+-rw-r--r--  2.0 unx    28718 b- defN 23-Apr-19 03:10 pyttsx3/six.py
+-rw-r--r--  2.0 unx      417 b- defN 23-Apr-19 03:10 pyttsx3/voice.py
+-rw-r--r--  2.0 unx      831 b- defN 23-Apr-19 03:10 pyttsx3/drivers/__init__.py
+-rw-r--r--  2.0 unx    19148 b- defN 23-Apr-19 03:10 pyttsx3/drivers/_espeak.py
+-rw-r--r--  2.0 unx     6012 b- defN 23-Apr-19 03:10 pyttsx3/drivers/dummy.py
+-rw-r--r--  2.0 unx     6665 b- defN 23-Apr-19 03:10 pyttsx3/drivers/espeak.py
+-rw-r--r--  2.0 unx     3713 b- defN 23-Apr-19 03:10 pyttsx3/drivers/nsss.py
+-rw-r--r--  2.0 unx     5185 b- defN 23-Apr-19 03:10 pyttsx3/drivers/sapi5.py
+-rw-r--r--  2.0 unx    16725 b- defN 23-Apr-19 03:11 py3_tts-3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    23751 b- defN 23-Apr-19 03:11 py3_tts-3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 03:11 py3_tts-3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-19 03:11 py3_tts-3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1235 b- defN 23-Apr-19 03:11 py3_tts-3.1.dist-info/RECORD
+16 files, 126906 bytes uncompressed, 36723 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: pyttsx3/drivers/nsss.py
 Comment: 
 
 Filename: pyttsx3/drivers/sapi5.py
 Comment: 
 
-Filename: py3_tts-3.0b0.dist-info/LICENSE
+Filename: py3_tts-3.1.dist-info/LICENSE
 Comment: 
 
-Filename: py3_tts-3.0b0.dist-info/METADATA
+Filename: py3_tts-3.1.dist-info/METADATA
 Comment: 
 
-Filename: py3_tts-3.0b0.dist-info/WHEEL
+Filename: py3_tts-3.1.dist-info/WHEEL
 Comment: 
 
-Filename: py3_tts-3.0b0.dist-info/top_level.txt
+Filename: py3_tts-3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: py3_tts-3.0b0.dist-info/RECORD
+Filename: py3_tts-3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyttsx3/__init__.py

```diff
@@ -1,32 +1,32 @@
-from .engine import Engine
 import weakref
 
+from .engine import Engine
+
 _activeEngines = weakref.WeakValueDictionary()
 
+
 def init(driverName=None, debug=False):
-    '''
+    """
     Constructs a new TTS engine instance or reuses the existing instance for
     the driver name.
 
     @param driverName: Name of the platform specific driver to use. If
         None, selects the default driver for the operating system.
     @type: str
     @param debug: Debugging output enabled or not
     @type debug: bool
     @return: Engine instance
     @rtype: L{engine.Engine}
-    '''
+    """
     try:
         eng = _activeEngines[driverName]
     except KeyError:
         eng = Engine(driverName, debug)
         _activeEngines[driverName] = eng
     return eng
 
 
 def speak(text):
     engine = init()
     engine.say(text)
     engine.runAndWait()
-
-
```

## pyttsx3/driver.py

```diff
@@ -1,15 +1,15 @@
+import importlib
 import sys
 import traceback
 import weakref
-import importlib
 
 
 class DriverProxy(object):
-    '''
+    """
     Proxy to a driver implementation.
 
     @ivar _module: Module containing the driver implementation
     @type _module: module
     @ivar _engine: Reference to the engine that owns the driver
     @type _engine: L{engine.Engine}
     @ivar _queue: Queue of commands outstanding for the driver
@@ -19,28 +19,28 @@
     @type _busy: bool
     @ivar _name: Name associated with the current utterance
     @type _name: str
     @ivar _debug: Debugging output enabled or not
     @type _debug: bool
     @ivar _iterator: Driver iterator to invoke when in an external run loop
     @type _iterator: iterator
-    '''
+    """
 
     def __init__(self, engine, driverName, debug):
-        '''
+        """
         Constructor.
 
         @param engine: Reference to the engine that owns the driver
         @type engine: L{engine.Engine}
         @param driverName: Name of the driver module to use under drivers/ or
             None to select the default for the platform
         @type driverName: str
         @param debug: Debugging output enabled or not
         @type debug: bool
-        '''
+        """
         if driverName is None:
             # pick default driver for common platforms
             if sys.platform == 'darwin':
                 driverName = 'nsss'
             elif sys.platform == 'win32':
                 driverName = 'sapi5'
             else:
@@ -61,163 +61,163 @@
     def __del__(self):
         try:
             self._driver.destroy()
         except (AttributeError, TypeError):
             pass
 
     def _push(self, mtd, args, name=None):
-        '''
+        """
         Adds a command to the queue.
 
         @param mtd: Method to invoke to process the command
         @type mtd: method
         @param args: Arguments to apply when invoking the method
         @type args: tuple
         @param name: Name associated with the command
         @type name: str
-        '''
+        """
         self._queue.append((mtd, args, name))
         self._pump()
 
     def _pump(self):
-        '''
+        """
         Attempts to process the next command in the queue if one exists and the
         driver is not currently busy.
-        '''
+        """
         while (not self._busy) and len(self._queue):
             cmd = self._queue.pop(0)
             self._name = cmd[2]
             try:
                 cmd[0](*cmd[1])
             except Exception as e:
                 self.notify('error', exception=e)
                 if self._debug:
                     traceback.print_exc()
 
     def notify(self, topic, **kwargs):
-        '''
+        """
         Sends a notification to the engine from the driver.
 
         @param topic: Notification topic
         @type topic: str
         @param kwargs: Arbitrary keyword arguments
         @type kwargs: dict
-        '''
+        """
         kwargs['name'] = self._name
         self._engine._notify(topic, **kwargs)
 
     def setBusy(self, busy):
-        '''
+        """
         Called by the driver to indicate it is busy.
 
         @param busy: True when busy, false when idle
         @type busy: bool
-        '''
+        """
         self._busy = busy
         if not self._busy:
             self._pump()
 
     def isBusy(self):
-        '''
+        """
         @return: True if the driver is busy, false if not
         @rtype: bool
-        '''
+        """
         return self._busy
 
     def say(self, text, name):
-        '''
+        """
         Called by the engine to push a say command onto the queue.
 
         @param text: Text to speak
         @type text: unicode
         @param name: Name to associate with the utterance
         @type name: str
-        '''
+        """
         self._push(self._driver.say, (text,), name)
 
     def stop(self):
-        '''
+        """
         Called by the engine to stop the current utterance and clear the queue
         of commands.
-        '''
+        """
         # clear queue up to first end loop command
-        while(True):
+        while True:
             try:
                 mtd, args, name = self._queue[0]
             except IndexError:
                 break
-            if(mtd == self._engine.endLoop):
+            if mtd == self._engine.endLoop:
                 break
             self._queue.pop(0)
         self._driver.stop()
 
     def save_to_file(self, text, filename, name):
-        '''
+        """
         Called by the engine to push a say command onto the queue.
 
         @param text: Text to speak
         @type text: unicode
         @param name: Name to associate with the utterance
         @type name: str
-        '''
+        """
         self._push(self._driver.save_to_file, (text, filename), name)
 
     def getProperty(self, name):
-        '''
+        """
         Called by the engine to get a driver property value.
 
         @param name: Name of the property
         @type name: str
         @return: Property value
         @rtype: object
-        '''
+        """
         return self._driver.getProperty(name)
 
     def setProperty(self, name, value):
-        '''
+        """
         Called by the engine to set a driver property value.
 
         @param name: Name of the property
         @type name: str
         @param value: Property value
         @type value: object
-        '''
+        """
         self._push(self._driver.setProperty, (name, value))
 
     def runAndWait(self):
-        '''
+        """
         Called by the engine to start an event loop, process all commands in
         the queue at the start of the loop, and then exit the loop.
-        '''
+        """
         self._push(self._engine.endLoop, tuple())
         self._driver.startLoop()
 
     def startLoop(self, useDriverLoop):
-        '''
+        """
         Called by the engine to start an event loop.
-        '''
+        """
         if useDriverLoop:
             self._driver.startLoop()
         else:
             self._iterator = self._driver.iterate()
 
     def endLoop(self, useDriverLoop):
-        '''
+        """
         Called by the engine to stop an event loop.
-        '''
+        """
         self._queue = []
         self._driver.stop()
         if useDriverLoop:
             self._driver.endLoop()
         else:
             self._iterator = None
         self.setBusy(True)
 
     def iterate(self):
-        '''
+        """
         Called by the engine to iterate driver commands and notifications from
         within an external event loop.
-        '''
+        """
         try:
             next(self._iterator)
         except StopIteration:
             pass
```

## pyttsx3/engine.py

```diff
@@ -1,11 +1,12 @@
-from . import driver
 import traceback
 import weakref
 
+from . import driver
+
 
 class Engine(object):
     """
     @ivar proxy: Proxy to a driver implementation
     @type proxy: L{DriverProxy}
     @ivar _connects: Array of subscriptions
     @type _connects: list
@@ -87,42 +88,42 @@
         if len(arr) == 0:
             del self._connects[topic]
 
     def say(self, text, name=None):
         """
         Adds an utterance to speak to the event queue.
 
-        @param text: Text to sepak
+        @param text: Text to speak
         @type text: unicode
         @param name: Name to associate with this utterance. Included in
             notifications about this utterance.
         @type name: str
         """
-        if text == None:
+        if text is None:
             return "Argument value can't be none or empty"
         else:
             self.proxy.say(text, name)
 
     def stop(self):
         """
         Stops the current utterance and clears the event queue.
         """
         self.proxy.stop()
 
     def save_to_file(self, text, filename, name=None):
-        '''
+        """
         Adds an utterance to speak to the event queue.
 
-        @param text: Text to sepak
+        @param text: Text to speak
         @type text: unicode
         @param filename: the name of file to save.
         @param name: Name to associate with this utterance. Included in
             notifications about this utterance.
         @type name: str
-        '''
+        """
         self.proxy.save_to_file(text, filename, name)
 
     def isBusy(self):
         """
         @return: True if an utterance is currently being spoken, false if not
         @rtype: bool
         """
```

## pyttsx3/six.py

```diff
@@ -1,21 +1,18 @@
-
-
 from __future__ import absolute_import
 
 import functools
 import itertools
 import operator
 import sys
 import types
 
 __author__ = "Benjamin Peterson <benjamin@python.org>"
 __version__ = "1.9.0"
 
-
 # Useful for very coarse version differentiation.
 PY2 = sys.version_info[0] == 2
 PY3 = sys.version_info[0] == 3
 
 if PY3:
     string_types = str,
     integer_types = int,
@@ -35,14 +32,16 @@
         # Jython always uses 32 bits.
         MAXSIZE = int((1 << 31) - 1)
     else:
         # It's possible to have sizeof(long) != sizeof(Py_ssize_t).
         class X(object):
             def __len__(self):
                 return 1 << 31
+
+
         try:
             len(X())
         except OverflowError:
             # 32-bit
             MAXSIZE = int((1 << 31) - 1)
         else:
             # 64-bit
@@ -194,14 +193,15 @@
 
     def get_code(self, fullname):
         """Return None
 
         Required, if is_package is implemented"""
         self.__get_module(fullname)  # eventually raises ImportError
         return None
+
     get_source = get_code  # same as get_code
 
 
 _importer = _SixMetaPathImporter(__name__)
 
 
 class _MovedItems(_LazyModule):
@@ -488,146 +488,165 @@
     _meth_self = "im_self"
 
     _func_closure = "func_closure"
     _func_code = "func_code"
     _func_defaults = "func_defaults"
     _func_globals = "func_globals"
 
-
 try:
     advance_iterator = next
 except NameError:
     def advance_iterator(it):
         return it.next()
 next = advance_iterator
 
-
 try:
     callable = callable
 except NameError:
     def callable(obj):
         return any("__call__" in klass.__dict__ for klass in type(obj).__mro__)
 
-
 if PY3:
     def get_unbound_function(unbound):
         return unbound
 
+
     create_bound_method = types.MethodType
 
     Iterator = object
 else:
     def get_unbound_function(unbound):
         return unbound.im_func
 
+
     def create_bound_method(func, obj):
         return types.MethodType(func, obj, obj.__class__)
 
+
     class Iterator(object):
 
         def next(self):
             return type(self).__next__(self)
 
+
     callable = callable
 _add_doc(get_unbound_function,
          """Get the function out of a possibly unbound function""")
 
-
 get_method_function = operator.attrgetter(_meth_func)
 get_method_self = operator.attrgetter(_meth_self)
 get_function_closure = operator.attrgetter(_func_closure)
 get_function_code = operator.attrgetter(_func_code)
 get_function_defaults = operator.attrgetter(_func_defaults)
 get_function_globals = operator.attrgetter(_func_globals)
 
-
 if PY3:
     def iterkeys(d, **kw):
         return iter(d.keys(**kw))
 
+
     def itervalues(d, **kw):
         return iter(d.values(**kw))
 
+
     def iteritems(d, **kw):
         return iter(d.items(**kw))
 
+
     def iterlists(d, **kw):
         return iter(d.lists(**kw))
 
+
     viewkeys = operator.methodcaller("keys")
 
     viewvalues = operator.methodcaller("values")
 
     viewitems = operator.methodcaller("items")
 else:
     def iterkeys(d, **kw):
         return iter(d.iterkeys(**kw))
 
+
     def itervalues(d, **kw):
         return iter(d.itervalues(**kw))
 
+
     def iteritems(d, **kw):
         return iter(d.iteritems(**kw))
 
+
     def iterlists(d, **kw):
         return iter(d.iterlists(**kw))
 
+
     viewkeys = operator.methodcaller("viewkeys")
 
     viewvalues = operator.methodcaller("viewvalues")
 
     viewitems = operator.methodcaller("viewitems")
 
 _add_doc(iterkeys, "Return an iterator over the keys of a dictionary.")
 _add_doc(itervalues, "Return an iterator over the values of a dictionary.")
 _add_doc(iteritems,
          "Return an iterator over the (key, value) pairs of a dictionary.")
 _add_doc(iterlists,
          "Return an iterator over the (key, [values]) pairs of a dictionary.")
 
-
 if PY3:
     def b(s):
         return s.encode("latin-1")
 
+
     def u(s):
         return s
+
+
     unichr = chr
     if sys.version_info[1] <= 1:
         def int2byte(i):
             return bytes((i,))
     else:
         # This is about 2x faster than the implementation above on 3.2+
         int2byte = operator.methodcaller("to_bytes", 1, "big")
     byte2int = operator.itemgetter(0)
     indexbytes = operator.getitem
     iterbytes = iter
     import io
+
     StringIO = io.StringIO
     BytesIO = io.BytesIO
     _assertCountEqual = "assertCountEqual"
     _assertRaisesRegex = "assertRaisesRegex"
     _assertRegex = "assertRegex"
 else:
     def b(s):
         return s
+
+
     # Workaround for standalone backslash
 
     def u(s):
         return unicode(s.replace(r'\\', r'\\\\'), "unicode_escape")
+
+
     unichr = unichr
     int2byte = chr
 
+
     def byte2int(bs):
         return ord(bs[0])
 
+
     def indexbytes(buf, i):
         return ord(buf[i])
+
+
     iterbytes = functools.partial(itertools.imap, ord)
     import StringIO
+
     StringIO = BytesIO = StringIO.StringIO
     _assertCountEqual = "assertItemsEqual"
     _assertRaisesRegex = "assertRaisesRegexp"
     _assertRegex = "assertRegexpMatches"
 _add_doc(b, """Byte literal""")
 _add_doc(u, """Text literal""")
 
@@ -643,14 +662,15 @@
 def assertRegex(self, *args, **kwargs):
     return getattr(self, _assertRegex)(*args, **kwargs)
 
 
 if PY3:
     exec_ = getattr(moves.builtins, "exec")
 
+
     def reraise(tp, value, tb=None):
         if value is None:
             value = tp()
         if value.__traceback__ is not tb:
             raise value.with_traceback(tb)
         raise value
 
@@ -663,54 +683,54 @@
             if _locs_ is None:
                 _locs_ = frame.f_locals
             del frame
         elif _locs_ is None:
             _locs_ = _globs_
         exec("""exec _code_ in _globs_, _locs_""")
 
+
     exec_("""def reraise(tp, value, tb=None):
     raise tp, value, tb
 """)
 
-
 if sys.version_info[:2] == (3, 2):
     exec_("""def raise_from(value, from_value):
     if from_value is None:
         raise value
     raise value from from_value
 """)
 elif sys.version_info[:2] > (3, 2):
     exec_("""def raise_from(value, from_value):
     raise value from from_value
 """)
 else:
     def raise_from(value, from_value):
         raise value
 
-
 print_ = getattr(moves.builtins, "print", None)
 if print_ is None:
     def print_(*args, **kwargs):
         """The new-style print function for Python 2.4 and 2.5."""
         fp = kwargs.pop("file", sys.stdout)
         if fp is None:
             return
 
         def write(data):
             if not isinstance(data, basestring):
                 data = str(data)
             # If the file has an encoding, encode unicode with it.
             if (isinstance(fp, file) and
-                isinstance(data, unicode) and
+                    isinstance(data, unicode) and
                     fp.encoding is not None):
                 errors = getattr(fp, "errors", None)
                 if errors is None:
                     errors = "strict"
                 data = data.encode(fp.encoding, errors)
             fp.write(data)
+
         want_unicode = False
         sep = kwargs.pop("sep", None)
         if sep is not None:
             if isinstance(sep, unicode):
                 want_unicode = True
             elif not isinstance(sep, str):
                 raise TypeError("sep must be None or a string")
@@ -741,14 +761,15 @@
             if i:
                 write(sep)
             write(arg)
         write(end)
 if sys.version_info[:2] < (3, 3):
     _print = print_
 
+
     def print_(*args, **kwargs):
         fp = kwargs.get("file", sys.stdout)
         flush = kwargs.pop("flush", False)
         _print(*args, **kwargs)
         if flush and fp is not None:
             fp.flush()
 
@@ -757,43 +778,48 @@
 if sys.version_info[0:2] < (3, 4):
     def wraps(wrapped, assigned=functools.WRAPPER_ASSIGNMENTS,
               updated=functools.WRAPPER_UPDATES):
         def wrapper(f):
             f = functools.wraps(wrapped, assigned, updated)(f)
             f.__wrapped__ = wrapped
             return f
+
         return wrapper
 else:
     wraps = functools.wraps
 
 
 def with_metaclass(meta, *bases):
     """Create a base class with a metaclass."""
+
     # This requires a bit of explanation: the basic idea is to make a dummy
     # metaclass for one level of class instantiation that replaces itself with
     # the actual metaclass.
     class metaclass(meta):
         def __new__(cls, name, this_bases, d):
             return meta(name, bases, d)
+
     return type.__new__(metaclass, 'temporary_class', (), {})
 
 
 def add_metaclass(metaclass):
     """Class decorator for creating a class with a metaclass."""
+
     def wrapper(cls):
         orig_vars = cls.__dict__.copy()
         slots = orig_vars.get('__slots__')
         if slots is not None:
             if isinstance(slots, str):
                 slots = [slots]
             for slots_var in slots:
                 orig_vars.pop(slots_var)
         orig_vars.pop('__dict__', None)
         orig_vars.pop('__weakref__', None)
         return metaclass(cls.__name__, cls.__bases__, orig_vars)
+
     return wrapper
 
 
 def python_2_unicode_compatible(klass):
     """
     A decorator that defines __unicode__ and __str__ methods under Python 2.
     Under Python 3 it does nothing.
```

## pyttsx3/drivers/__init__.py

```diff
@@ -1,23 +1,24 @@
-
-'''
+"""
 Utility functions to help with Python 2/3 compatibility
-'''
+"""
 from .. import six
 
+
 def toUtf8(value):
-    '''
+    """
     Takes in a value and converts it to a text (unicode) type.  Then decodes that
     type to a byte array encoded in utf-8.  In 2.X the resulting object will be a
     str and in 3.X the resulting object will be bytes.  In both 2.X and 3.X any
     object can be passed in and the object's __str__ will be used (or __repr__ if
     __str__ is not defined) if the object is not already a text type.
-    '''
+    """
     return six.text_type(value).encode('utf-8')
 
+
 def fromUtf8(value):
-    '''
+    """
     Takes in a byte array encoded as utf-8 and returns a text (unicode) type.  In
     2.X we expect a str type and return a unicde type.  In 3.X we expect a bytes
     type and return a str type.
-    '''
+    """
     return value.decode('utf-8')
```

## pyttsx3/drivers/_espeak.py

```diff
@@ -1,97 +1,127 @@
-
-
 from __future__ import print_function
-from ctypes import cdll, c_int, c_char_p, c_wchar_p, POINTER, c_short, c_uint, c_long, c_void_p
-from ctypes import CFUNCTYPE, Structure, Union, c_wchar, c_ubyte, c_ulong, byref
+
 import time
+from ctypes import CFUNCTYPE, Structure, Union, c_wchar, c_ubyte, c_ulong
+from ctypes import cdll, c_int, c_char_p, POINTER, c_short, c_uint, c_long, c_void_p
+
 
 def cfunc(name, dll, result, *args):
-    '''build and apply a ctypes prototype complete with parameter flags'''
+    """build and apply a ctypes prototype complete with parameter flags"""
     atypes = []
     aflags = []
     for arg in args:
         atypes.append(arg[1])
         aflags.append((arg[2], arg[0]) + arg[3:])
     return CFUNCTYPE(result, *atypes)((name, dll), tuple(aflags))
 
+
 dll = None
 
+
 def load_linux_ep():
-   global dll
-   try: dll = cdll.LoadLibrary('libespeak.so.1')
-   except Exception as e: return False
-   else: return True
+    global dll
+    try:
+        dll = cdll.LoadLibrary('libespeak.so.1')
+    except Exception:
+        return False
+    else:
+        return True
+
 
 def load_linux_epng():
-   global dll
-   try: dll = cdll.LoadLibrary('libespeak-ng.so.1')
-   except Exception as e: return False
-   else: return True
+    global dll
+    try:
+        dll = cdll.LoadLibrary('libespeak-ng.so.1')
+    except Exception:
+        return False
+    else:
+        return True
+
 
 def load_linux_epng2():
-   global dll
-   try: dll = cdll.LoadLibrary('/usr/local/lib/libespeak-ng.so.1')
-   except Exception as e: return False
-   else: return True
+    global dll
+    try:
+        dll = cdll.LoadLibrary('/usr/local/lib/libespeak-ng.so.1')
+    except Exception:
+        return False
+    else:
+        return True
+
 
 def load_windows_epng1():
-   global dll
-   try: dll = cdll.LoadLibrary('libespeak-ng.dll')
-   except Exception as e: return False
-   else: return True
+    global dll
+    try:
+        dll = cdll.LoadLibrary('libespeak-ng.dll')
+    except Exception:
+        return False
+    else:
+        return True
+
 
 def load_windows_epng2():
-   global dll
-   try: dll = cdll.LoadLibrary('C:\\Program Files\\eSpeak NG\\libespeak-ng.dll')
-   except Exception as e: return False
-   else: return True
+    global dll
+    try:
+        dll = cdll.LoadLibrary('C:\\Program Files\\eSpeak NG\\libespeak-ng.dll')
+    except Exception:
+        return False
+    else:
+        return True
+
 
 def load_windows_epng3():
-   global dll
-   try: dll = cdll.LoadLibrary('C:\\Program Files (x86)\\eSpeak NG\\libespeak-ng.dll')
-   except Exception as e: return False
-   else: return True
+    global dll
+    try:
+        dll = cdll.LoadLibrary('C:\\Program Files (x86)\\eSpeak NG\\libespeak-ng.dll')
+    except Exception:
+        return False
+    else:
+        return True
+
 
 try:
-   load_linux_ep() or load_linux_epng() or load_linux_epng2() or load_windows_epng1() or load_windows_epng2() or load_windows_epng3()
+    load_linux_ep() or load_linux_epng() or load_linux_epng2() or load_windows_epng1() or load_windows_epng2() or load_windows_epng3()
 except Exception as exp:
     print("Exception: " + str(exp) + "\n")
     print("This means you probably do not have eSpeak or eSpeak-ng installed!")
     import sys
+
     sys.exit()
 
 # constants and such from speak_lib.h
 
 EVENT_LIST_TERMINATED = 0
 EVENT_WORD = 1
 EVENT_SENTENCE = 2
 EVENT_MARK = 3
 EVENT_PLAY = 4
 EVENT_END = 5
 EVENT_MSG_TERMINATED = 6
 
+
 class numberORname(Union):
     _fields_ = [
         ('number', c_int),
         ('name', c_char_p)
-        ]
-    
+    ]
+
+
 class EVENT(Structure):
     _fields_ = [
         ('type', c_int),
         ('unique_identifier', c_uint),
         ('text_position', c_int),
         ('length', c_int),
         ('audio_position', c_int),
         ('sample', c_int),
         ('user_data', c_void_p),
         ('id', numberORname)
-        ]
-    
+    ]
+
+
 AUDIO_OUTPUT_PLAYBACK = 0
 AUDIO_OUTPUT_RETRIEVAL = 1
 AUDIO_OUTPUT_SYNCHRONOUS = 2
 AUDIO_OUTPUT_SYNCH_PLAYBACK = 3
 
 EE_OK = 0
 EE_INTERNAL_ERROR = -1
@@ -99,33 +129,36 @@
 EE_NOT_FOUND = 2
 
 Initialize = cfunc('espeak_Initialize', dll, c_int,
                    ('output', c_int, 1, AUDIO_OUTPUT_PLAYBACK),
                    ('bufflength', c_int, 1, 100),
                    ('path', c_char_p, 1, None),
                    ('option', c_int, 1, 0))
-Initialize.__doc__ = '''Must be called before any synthesis functions are called.
+Initialize.__doc__ = """Must be called before any synthesis functions are called.
   output: the audio data can either be played by eSpeak or passed back by the SynthCallback function. 
   buflength:  The length in mS of sound buffers passed to the SynthCallback function.
   path: The directory which contains the espeak-data directory, or NULL for the default location.
   options: bit 0: 1=allow espeakEVENT_PHONEME events.
 
-  Returns: sample rate in Hz, or -1 (EE_INTERNAL_ERROR).'''
+  Returns: sample rate in Hz, or -1 (EE_INTERNAL_ERROR)."""
 
 t_espeak_callback = CFUNCTYPE(c_int, POINTER(c_short), c_int, POINTER(EVENT))
 
 cSetSynthCallback = cfunc('espeak_SetSynthCallback', dll, None,
-                        ('SynthCallback', t_espeak_callback, 1))
+                          ('SynthCallback', t_espeak_callback, 1))
 SynthCallback = None
+
+
 def SetSynthCallback(cb):
     global SynthCallback
     SynthCallback = t_espeak_callback(cb)
     cSetSynthCallback(SynthCallback)
 
-SetSynthCallback.__doc__ = '''Must be called before any synthesis functions are called.
+
+SetSynthCallback.__doc__ = """Must be called before any synthesis functions are called.
    This specifies a function in the calling program which is called when a buffer of
    speech sound data has been produced. 
 
 
    The callback function is of the form:
 
 int SynthCallback(short *wav, int numsamples, espeak_EVENT *events);
@@ -137,27 +170,30 @@
       the value implied by the buflength parameter given in espeak_Initialize, and may
       sometimes be zero (which does NOT indicate end of synthesis).
 
    events: an array of espeak_EVENT items which indicate word and sentence events, and
       also the occurance if <mark> and <audio> elements within the text.
 
 
-   Callback returns: 0=continue synthesis,  1=abort synthesis.'''
+   Callback returns: 0=continue synthesis,  1=abort synthesis."""
 
 t_UriCallback = CFUNCTYPE(c_int, c_int, c_char_p, c_char_p)
 
 cSetUriCallback = cfunc('espeak_SetUriCallback', dll, None,
-                       ('UriCallback', t_UriCallback, 1))
+                        ('UriCallback', t_UriCallback, 1))
 UriCallback = None
+
+
 def SetUriCallback(cb):
     global UriCallback
     UriCallback = t_UriCallback(UriCallback)
     cSetUriCallback(UriCallback)
 
-SetUriCallback.__doc__ = '''This function must be called before synthesis functions are used, in order to deal with
+
+SetUriCallback.__doc__ = """This function must be called before synthesis functions are used, in order to deal with
    <audio> tags.  It specifies a callback function which is called when an <audio> element is
    encountered and allows the calling program to indicate whether the sound file which
    is specified in the <audio> element is available and is to be played.
 
    The callback function is of the form:
 
 int UriCallback(int type, const char *uri, const char *base);
@@ -166,45 +202,46 @@
 
    uri:   the "src" attribute from the <audio> element
 
    base:  the "xml:base" attribute (if any) from the <speak> element
 
    Return: 1=don't play the sound, but speak the text alternative.
            0=place a PLAY event in the event list at the point where the <audio> element
-             occurs.  The calling program can then play the sound at that point.'''
-
+             occurs.  The calling program can then play the sound at that point."""
 
 # a few manifest constants
-CHARS_AUTO =  0
-CHARS_UTF8 =  1
-CHARS_8BIT =  2
+CHARS_AUTO = 0
+CHARS_UTF8 = 1
+CHARS_8BIT = 2
 CHARS_WCHAR = 3
 
-SSML          = 0x10
-PHONEMES      = 0x100
-ENDPAUSE      = 0x1000
+SSML = 0x10
+PHONEMES = 0x100
+ENDPAUSE = 0x1000
 KEEP_NAMEDATA = 0x2000
 
 POS_CHARACTER = 1
-POS_WORD      = 2
-POS_SENTENCE  = 3
+POS_WORD = 2
+POS_SENTENCE = 3
+
 
 def Synth(text, position=0, position_type=POS_CHARACTER, end_position=0, flags=0, user_data=None):
-    return cSynth(text, len(text)*10, position, position_type, end_position, flags, None, user_data)
+    return cSynth(text, len(text) * 10, position, position_type, end_position, flags, None, user_data)
+
 
 cSynth = cfunc('espeak_Synth', dll, c_int,
-              ('text', c_char_p, 1),
-              ('size', c_long, 1),
-              ('position', c_uint, 1, 0),
-              ('position_type', c_int, 1, POS_CHARACTER),
-              ('end_position', c_uint, 1, 0),
-              ('flags', c_uint, 1, CHARS_AUTO),
-              ('unique_identifier', POINTER(c_uint), 1, None),
-              ('user_data', c_void_p, 1, None))
-Synth.__doc__ = '''Synthesize speech for the specified text.  The speech sound data is passed to the calling
+               ('text', c_char_p, 1),
+               ('size', c_long, 1),
+               ('position', c_uint, 1, 0),
+               ('position_type', c_int, 1, POS_CHARACTER),
+               ('end_position', c_uint, 1, 0),
+               ('flags', c_uint, 1, CHARS_AUTO),
+               ('unique_identifier', POINTER(c_uint), 1, None),
+               ('user_data', c_void_p, 1, None))
+Synth.__doc__ = """Synthesize speech for the specified text.  The speech sound data is passed to the calling
    program in buffers by means of the callback function specified by espeak_SetSynthCallback(). The command is asynchronous: it is internally buffered and returns as soon as possible. If espeak_Initialize was previously called with AUDIO_OUTPUT_PLAYBACK as argument, the sound data are played by eSpeak.
 
    text: The text to be spoken, terminated by a zero character. It may be either 8-bit characters,
       wide characters (wchar_t), or UTF8 encoding.  Which of these is determined by the "flags"
       parameter.
 
    size: Equal to (or greater than) the size of the text data, in bytes.  This is used in order
@@ -238,258 +275,264 @@
      data supplied to the callback.
 
    user_data: pointer which will be passed to the callback function.
 
    Return: EE_OK: operation achieved 
            EE_BUFFER_FULL: the command can not be buffered; 
              you may try after a while to call the function again.
-	   EE_INTERNAL_ERROR.'''
+	   EE_INTERNAL_ERROR."""
+
 
 def Synth_Mark(text, index_mark, end_position=0, flags=CHARS_AUTO):
-    cSynth_Mark(text, len(text)+1, index_mark, end_position, flags)
+    cSynth_Mark(text, len(text) + 1, index_mark, end_position, flags)
+
 
 cSynth_Mark = cfunc('espeak_Synth_Mark', dll, c_int,
-                   ('text', c_char_p, 1),
-                   ('size', c_ulong, 1),
-                   ('index_mark', c_char_p, 1),
-                   ('end_position', c_uint, 1, 0),
-                   ('flags', c_uint, 1, CHARS_AUTO),
-                   ('unique_identifier', POINTER(c_uint), 1, None),
-                   ('user_data', c_void_p, 1, None))
-Synth_Mark.__doc__ = '''Synthesize speech for the specified text.  Similar to espeak_Synth() but the start position is
+                    ('text', c_char_p, 1),
+                    ('size', c_ulong, 1),
+                    ('index_mark', c_char_p, 1),
+                    ('end_position', c_uint, 1, 0),
+                    ('flags', c_uint, 1, CHARS_AUTO),
+                    ('unique_identifier', POINTER(c_uint), 1, None),
+                    ('user_data', c_void_p, 1, None))
+Synth_Mark.__doc__ = """Synthesize speech for the specified text.  Similar to espeak_Synth() but the start position is
    specified by the name of a <mark> element in the text.
 
    index_mark:  The "name" attribute of a <mark> element within the text which specified the
       point at which synthesis starts.  UTF8 string.
 
    For the other parameters, see espeak_Synth()
 
-   Return: EE_OK: operation achieved 
-           EE_BUFFER_FULL: the command can not be buffered; 
+   Return:  EE_OK: operation achieved 
+            EE_BUFFER_FULL: the command can not be buffered; 
              you may try after a while to call the function again.
-	   EE_INTERNAL_ERROR.'''
+	        EE_INTERNAL_ERROR."""
 
 Key = cfunc('espeak_Key', dll, c_int,
             ('key_name', c_char_p, 1))
-Key.__doc__ = '''Speak the name of a keyboard key.
+Key.__doc__ = """Speak the name of a keyboard key.
    Currently this just speaks the "key_name" as given 
 
    Return: EE_OK: operation achieved 
            EE_BUFFER_FULL: the command can not be buffered; 
              you may try after a while to call the function again.
-	   EE_INTERNAL_ERROR.'''
+	   EE_INTERNAL_ERROR."""
 
 Char = cfunc('espeak_Char', dll, c_int,
              ('character', c_wchar, 1))
-Char.__doc__ = '''Speak the name of the given character 
+Char.__doc__ = """Speak the name of the given character 
 
    Return: EE_OK: operation achieved 
            EE_BUFFER_FULL: the command can not be buffered; 
              you may try after a while to call the function again.
-	   EE_INTERNAL_ERROR.'''
+	   EE_INTERNAL_ERROR."""
 
 # Speech Parameters
-SILENCE=0  #internal use
-RATE=1
-VOLUME=2
-PITCH=3
-RANGE=4
-PUNCTUATION=5
-CAPITALS=6
-EMPHASIS=7   # internal use
-LINELENGTH=8 # internal use
-
-PUNCT_NONE=0
-PUNCT_ALL=1
-PUNCT_SOME=2
+SILENCE = 0  # internal use
+RATE = 1
+VOLUME = 2
+PITCH = 3
+RANGE = 4
+PUNCTUATION = 5
+CAPITALS = 6
+EMPHASIS = 7  # internal use
+LINELENGTH = 8  # internal use
+
+PUNCT_NONE = 0
+PUNCT_ALL = 1
+PUNCT_SOME = 2
 
 SetParameter = cfunc('espeak_SetParameter', dll, c_int,
                      ('parameter', c_int, 1),
                      ('value', c_int, 1),
                      ('relative', c_int, 1, 0))
-SetParameter.__doc__ = '''Sets the value of the specified parameter.
+SetParameter.__doc__ = """Sets the value of the specified parameter.
    relative=0   Sets the absolute value of the parameter.
    relative=1   Sets a relative value of the parameter.
 
    parameter:
       espeak.RATE:    speaking speed in word per minute.
 
       espeak.VOLUME:  volume in range 0-100    0=silence
 
       espeak.PITCH:   base pitch, range 0-100.  50=normal
 
       espeak.RANGE:   pitch range, range 0-100. 0-monotone, 50=normal
 
       espeak.PUNCTUATION:  which punctuation characters to announce:
          value in espeak_PUNCT_TYPE (none, all, some), 
-	 see espeak_GetParameter() to specify which characters are announced.
+         see espeak_GetParameter() to specify which characters are announced.
 
       espeak.CAPITALS: announce capital letters by:
          0=none,
          1=sound icon,
          2=spelling,
          3 or higher, by raising pitch.  This values gives the amount in Hz by which the pitch
             of a word raised to indicate it has a capital letter.
 
    Return: EE_OK: operation achieved 
            EE_BUFFER_FULL: the command can not be buffered; 
              you may try after a while to call the function again.
-	   EE_INTERNAL_ERROR.'''
+           EE_INTERNAL_ERROR."""
 
 GetParameter = cfunc('espeak_GetParameter', dll, c_int,
                      ('parameter', c_int, 1))
-GetParameter.__doc__ = '''current=0  Returns the default value of the specified parameter.
-   current=1  Returns the current value of the specified parameter, as set by SetParameter()'''
+GetParameter.__doc__ = """current=0  Returns the default value of the specified parameter.
+   current=1  Returns the current value of the specified parameter, as set by SetParameter()"""
 
 SetPunctuationList = cfunc('espeak_SetPunctuationList', dll, c_int,
                            ('punctlist', c_wchar, 1))
-SetPunctuationList.__doc__ = '''Specified a list of punctuation characters whose names are to be spoken when the value of the Punctuation parameter is set to "some".
+SetPunctuationList.__doc__ = """Specified a list of punctuation characters whose names are 
+to be spoken when the value of the Punctuation parameter is set to "some".
 
    punctlist:  A list of character codes, terminated by a zero character.
 
-   Return: EE_OK: operation achieved 
-           EE_BUFFER_FULL: the command can not be buffered; 
+   Return:  EE_OK: operation achieved 
+            EE_BUFFER_FULL: the command can not be buffered; 
              you may try after a while to call the function again.
-	   EE_INTERNAL_ERROR.'''
-                           
+            EE_INTERNAL_ERROR."""
+
 SetPhonemeTrace = cfunc('espeak_SetPhonemeTrace', dll, None,
                         ('value', c_int, 1),
                         ('stream', c_void_p, 1))
-SetPhonemeTrace.__doc__ = '''Controls the output of phoneme symbols for the text
+SetPhonemeTrace.__doc__ = """Controls the output of phoneme symbols for the text
    value=0  No phoneme output (default)
    value=1  Output the translated phoneme symbols for the text
    value=2  as (1), but also output a trace of how the translation was done (matching rules and list entries)
 
-   stream   output stream for the phoneme symbols (and trace).  If stream=NULL then it uses stdout.'''
+   stream   output stream for the phoneme symbols (and trace).  If stream=NULL then it uses stdout."""
 
 CompileDictionary = cfunc('espeak_CompileDictionary', dll, None,
                           ('path', c_char_p, 1),
                           ('log', c_void_p, 1))
-CompileDictionary.__doc__ = '''Compile pronunciation dictionary for a language which corresponds to the currently
+CompileDictionary.__doc__ = """Compile pronunciation dictionary for a language which corresponds to the currently
    selected voice.  The required voice should be selected before calling this function.
 
    path:  The directory which contains the language's '_rules' and '_list' files.
           'path' should end with a path separator character ('/').
-   log:   Stream for error reports and statistics information. If log=NULL then stderr will be used.'''
+   log:   Stream for error reports and statistics information. If log=NULL then stderr will be used."""
+
 
 class VOICE(Structure):
     _fields_ = [
         ('name', c_char_p),
         ('languages', c_char_p),
         ('identifier', c_char_p),
         ('gender', c_ubyte),
         ('age', c_ubyte),
         ('variant', c_ubyte),
         ('xx1', c_ubyte),
         ('score', c_int),
         ('spare', c_void_p),
-        ]
+    ]
+
     def __repr__(self):
-        '''Print the fields'''
+        """Print the fields"""
         res = []
         for field in self._fields_:
             res.append('%s=%s' % (field[0], repr(getattr(self, field[0]))))
         return self.__class__.__name__ + '(' + ','.join(res) + ')'
-        
+
 
 cListVoices = cfunc('espeak_ListVoices', dll, POINTER(POINTER(VOICE)),
                     ('voice_spec', POINTER(VOICE), 1))
-cListVoices.__doc__ = '''Reads the voice files from espeak-data/voices and creates an array of espeak_VOICE pointers.
+cListVoices.__doc__ = """Reads the voice files from espeak-data/voices and creates an array of espeak_VOICE pointers.
    The list is terminated by a NULL pointer
 
    If voice_spec is NULL then all voices are listed.
    If voice spec is given, then only the voices which are compatible with the voice_spec
-   are listed, and they are listed in preference order.'''
+   are listed, and they are listed in preference order."""
+
 
 def ListVoices(voice_spec=None):
-    '''Reads the voice files from espeak-data/voices and returns a list of VOICE objects.
+    """Reads the voice files from espeak-data/voices and returns a list of VOICE objects.
 
    If voice_spec is None then all voices are listed.
    If voice spec is given, then only the voices which are compatible with the voice_spec
-   are listed, and they are listed in preference order.'''
+   are listed, and they are listed in preference order."""
     ppv = cListVoices(voice_spec)
     res = []
     i = 0
     while ppv[i]:
         res.append(ppv[i][0])
         i += 1
     return res
 
+
 SetVoiceByName = cfunc('espeak_SetVoiceByName', dll, c_int,
                        ('name', c_char_p, 1))
-SetVoiceByName.__doc__ = '''Searches for a voice with a matching "name" field.  Language is not considered.
+SetVoiceByName.__doc__ = """Searches for a voice with a matching "name" field.  Language is not considered.
    "name" is a UTF8 string.
 
-   Return: EE_OK: operation achieved 
-           EE_BUFFER_FULL: the command can not be buffered; 
+   Return:   EE_OK: operation achieved 
+             EE_BUFFER_FULL: the command can not be buffered; 
              you may try after a while to call the function again.
-	   EE_INTERNAL_ERROR.'''
+             EE_INTERNAL_ERROR."""
 
 SetVoiceByProperties = cfunc('espeak_SetVoiceByProperties', dll, c_int,
                              ('voice_spec', POINTER(VOICE), 1))
-SetVoiceByProperties.__doc__ = '''An espeak_VOICE structure is used to pass criteria to select a voice.  Any of the following
+SetVoiceByProperties.__doc__ = """An espeak_VOICE structure is used to pass criteria to select a voice.  Any of the following
    fields may be set:
 
    name     NULL, or a voice name
 
    languages  NULL, or a single language string (with optional dialect), eg. "en-uk", or "en"
 
    gender   0=not specified, 1=male, 2=female
 
    age      0=not specified, or an age in years
 
    variant  After a list of candidates is produced, scored and sorted, "variant" is used to index
             that list and choose a voice.
-            variant=0 takes the top voice (i.e. best match). variant=1 takes the next voice, etc'''
+            variant=0 takes the top voice (i.e. best match). variant=1 takes the next voice, etc"""
 
 GetCurrentVoice = cfunc('espeak_GetCurrentVoice', dll, POINTER(VOICE),
                         )
-GetCurrentVoice.__doc__ = '''Returns the espeak_VOICE data for the currently selected voice.
-   This is not affected by temporary voice changes caused by SSML elements such as <voice> and <s>'''
+GetCurrentVoice.__doc__ = """Returns the espeak_VOICE data for the currently selected voice.
+   This is not affected by temporary voice changes caused by SSML elements such as <voice> and <s>"""
 
 Cancel = cfunc('espeak_Cancel', dll, c_int)
-Cancel.__doc__ = '''Stop immediately synthesis and audio output of the current text. When this
+Cancel.__doc__ = """Stop immediately synthesis and audio output of the current text. When this
    function returns, the audio output is fully stopped and the synthesizer is ready to
    synthesize a new message.
 
-   Return: EE_OK: operation achieved 
-	   EE_INTERNAL_ERROR.'''
+   Return:  EE_OK: operation achieved 
+            EE_INTERNAL_ERROR."""
 
 IsPlaying = cfunc('espeak_IsPlaying', dll, c_int)
-IsPlaying.__doc__ = '''Returns 1 if audio is played, 0 otherwise.'''
+IsPlaying.__doc__ = """Returns 1 if audio is played, 0 otherwise."""
 
 Synchronize = cfunc('espeak_Synchronize', dll, c_int)
-Synchronize.__doc__ = '''This function returns when all data have been spoken.
-   Return: EE_OK: operation achieved 
-	   EE_INTERNAL_ERROR.'''
+Synchronize.__doc__ = """This function returns when all data have been spoken.
+   Return:  EE_OK: operation achieved 
+	        EE_INTERNAL_ERROR."""
 
 Terminate = cfunc('espeak_Terminate', dll, c_int)
-Terminate.__doc__ = '''last function to be called.
-   Return: EE_OK: operation achieved 
-	   EE_INTERNAL_ERROR.'''
-
-Info = cfunc('espeak_Info', dll, c_char_p,
-             ('ptr', c_void_p, 1, 0))
-Info.__doc__ = '''Returns the version number string.
-   The parameter is for future use, and should be set to NULL'''
+Terminate.__doc__ = """last function to be called.
+   Return:  EE_OK: operation achieved 
+	        EE_INTERNAL_ERROR."""
+
+Info = cfunc('espeak_Info', dll, c_char_p, ('ptr', c_void_p, 1, 0))
+Info.__doc__ = """Returns the version number string.
+The parameter is for future use, and should be set to NULL"""
 
 if __name__ == '__main__':
     def synth_cb(wav, numsample, events):
         print(numsample, end="")
         i = 0
         while True:
             if events[i].type == EVENT_LIST_TERMINATED:
                 break
-            print (events[i].type, end="")
+            print(events[i].type, end="")
             i += 1
-        print
         return 0
 
+
     samplerate = Initialize(output=AUDIO_OUTPUT_PLAYBACK)
     SetSynthCallback(synth_cb)
     s = 'This is a test, only a test. '
     uid = c_uint(0)
-    #print 'pitch=',GetParameter(PITCH)
-    #SetParameter(PITCH, 50, 0)
+    # print 'pitch=',GetParameter(PITCH)
+    # SetParameter(PITCH, 50, 0)
     print(Synth(s))
     while IsPlaying():
         time.sleep(0.1)
```

## pyttsx3/drivers/dummy.py

```diff
@@ -1,98 +1,101 @@
+import time
 
 from ..voice import Voice
-import time
+
 
 def buildDriver(proxy):
-    '''
+    """
     Builds a new instance of a driver and returns it for use by the driver
     proxy.
 
     @param proxy: Proxy creating the driver
     @type proxy: L{driver.DriverProxy}
-    '''
+    """
     return DummyDriver(proxy)
 
+
 class DummyDriver(object):
-    '''
+    """
     Dummy speech engine implementation. Documents the interface, notifications,
     properties, and sequencing responsibilities of a driver implementation.
 
     @ivar _proxy: Driver proxy that manages this instance
     @type _proxy: L{driver.DriverProxy}
     @ivar _config: Dummy configuration
     @type _config: dict
     @ivar _looping: True when in the dummy event loop, False when not
     @ivar _looping: bool
-    '''
+    """
+
     def __init__(self, proxy):
-        '''
+        """
         Constructs the driver.
 
         @param proxy: Proxy creating the driver
         @type proxy: L{driver.DriverProxy}
-        '''
+        """
         self._proxy = proxy
         self._looping = False
         # hold config values as if we had a real tts implementation that
         # supported them
         voices = [
             Voice('dummy.voice1', 'John Doe', ['en-US', 'en-GB'], 'male', 'adult'),
             Voice('dummy.voice2', 'Jane Doe', ['en-US', 'en-GB'], 'female', 'adult'),
             Voice('dummy.voice3', 'Jimmy Doe', ['en-US', 'en-GB'], 'male', 10)
         ]
         self._config = {
-            'rate' : 200,
-            'volume' : 1.0,
-            'voice' : voices[0],
-            'voices' : voices
+            'rate': 200,
+            'volume': 1.0,
+            'voice': voices[0],
+            'voices': voices
         }
 
     def destroy(self):
-        '''
+        """
         Optional method that will be called when the driver proxy is being
         destroyed. Can cleanup any resources to make sure the engine terminates
         properly.
-        '''
+        """
         pass
 
     def startLoop(self):
-        '''
+        """
         Starts a blocking run loop in which driver callbacks are properly
         invoked.
 
         @precondition: There was no previous successful call to L{startLoop}
             without an intervening call to L{stopLoop}.
-        '''
+        """
         first = True
         self._looping = True
         while self._looping:
             if first:
                 self._proxy.setBusy(False)
                 first = False
             time.sleep(0.5)
 
     def endLoop(self):
-        '''
+        """
         Stops a previously started run loop.
 
         @precondition: A previous call to L{startLoop} suceeded and there was
             no intervening call to L{endLoop}.
-        '''
+        """
         self._looping = False
 
     def iterate(self):
-        '''
+        """
         Iterates from within an external run loop.
-        '''
+        """
         self._proxy.setBusy(False)
         yield
 
     def say(self, text):
-        '''
+        """
         Speaks the given text. Generates the following notifications during
         output:
 
         started-utterance: When speech output has started
         started-word: When a word is about to be spoken. Includes the character
             "location" of the start of the word in the original utterance text
             and the "length" of the word in characters.
@@ -106,70 +109,70 @@
         that it is busy by invoking L{driver.DriverProxy.setBusy} with a flag
         of True. When the utterance completes or is interrupted, the driver
         inform the proxy that it is no longer busy by invoking
         L{driver.DriverProxy.setBusy} with a flag of False.
 
         @param text: Unicode text to speak
         @type text: unicode
-        '''
+        """
         self._proxy.setBusy(True)
         self._proxy.notify('started-utterance')
         i = 0
         for word in text.split(' '):
             self._proxy.notify('started-word', location=i, length=len(word))
             try:
-                i = text.index(' ', i+1)+1
+                i = text.index(' ', i + 1) + 1
             except Exception:
                 pass
         self._proxy.notify('finished-utterance', completed=True)
         self._proxy.setBusy(False)
 
     def stop(self):
-        '''
+        """
         Stops any current output. If an utterance was being spoken, the driver
         is still responsible for sending the closing finished-utterance
         notification documented above and resetting the busy state of the
         proxy.
-        '''
+        """
         pass
 
     def getProperty(self, name):
-        '''
+        """
         Gets a property value of the speech engine. The suppoted properties
         and their values are:
 
         voices: List of L{voice.Voice} objects supported by the driver
         voice: String ID of the current voice
         rate: Integer speech rate in words per minute
         volume: Floating point volume of speech in the range [0.0, 1.0]
 
         @param name: Property name
         @type name: str
         @raise KeyError: When the property name is unknown
-        '''
+        """
         try:
             return self._config[name]
         except KeyError:
             raise KeyError('unknown property %s' % name)
 
     def setProperty(self, name, value):
-        '''
+        """
         Sets one of the supported property values of the speech engine listed
         above. If a value is invalid, attempts to clip it / coerce so it is
         valid before giving up and firing an exception.
 
         @param name: Property name
         @type name: str
         @param value: Property value
         @type value: object
         @raise KeyError: When the property name is unknown
         @raise ValueError: When the value cannot be coerced to fit the property
-        '''
+        """
         if name == 'voice':
             v = filter(lambda v: v.id == value, self._config['voices'])
             self._config['voice'] = v[0]
         elif name == 'rate':
             self._config['rate'] = value
         elif name == 'volume':
             self._config['volume'] = value
         else:
-            raise KeyError('unknown property %s' % name)
+            raise KeyError('unknown property %s' % name)
```

## pyttsx3/drivers/espeak.py

```diff
@@ -1,16 +1,15 @@
-
-import time
 import ctypes
-import io
-import wave
 import os
+import time
+import wave
 from tempfile import NamedTemporaryFile
-from ..voice import Voice
+
 from . import _espeak, toUtf8, fromUtf8
+from ..voice import Voice
 
 
 def buildDriver(proxy):
     return EspeakDriver(proxy)
 
 
 class EspeakDriver(object):
@@ -48,15 +47,15 @@
     def destroy(self):
         _espeak.SetSynthCallback(None)
 
     def say(self, text):
         self._proxy.setBusy(True)
         self._proxy.notify('started-utterance')
         _espeak.Synth(toUtf8(text), flags=_espeak.ENDPAUSE |
-                      _espeak.CHARS_UTF8)
+                                          _espeak.CHARS_UTF8)
 
     def stop(self):
         if _espeak.IsPlaying():
             self._stopping = True
 
     def getProperty(self, name):
         if name == 'voices':
@@ -131,15 +130,15 @@
                 self._proxy.notify('finished-utterance', completed=False)
                 self._proxy.setBusy(False)
             time.sleep(0.01)
 
     def save_to_file(self, text, filename):
         code = self.numerise(filename)
         _espeak.Synth(toUtf8(text), flags=_espeak.ENDPAUSE |
-                    _espeak.CHARS_UTF8, user_data=code)
+                                          _espeak.CHARS_UTF8, user_data=code)
 
     def endLoop(self):
         self._looping = False
 
     def iterate(self):
         self._proxy.setBusy(False)
         while 1:
@@ -168,20 +167,21 @@
                 with wave.open(stream, 'wb') as f:
                     f.setnchannels(1)
                     f.setsampwidth(2)
                     f.setframerate(22050.0)
                     f.writeframes(self._data_buffer)
 
                 if event.user_data:
-                    os.system('ffmpeg -y -i {} {} -loglevel quiet'.format(stream.name, self.decode_numeric(event.user_data)))
+                    os.system(
+                        'ffmpeg -y -i {} {} -loglevel quiet'.format(stream.name, self.decode_numeric(event.user_data)))
                 else:
                     os.system('aplay {} -q'.format(stream.name))  # -q for quiet
 
                 self._data_buffer = b''
                 self._proxy.notify('finished-utterance', completed=True)
                 self._proxy.setBusy(False)
             i += 1
-        
+
         if numsamples > 0:
             self._data_buffer += ctypes.string_at(wav, numsamples *
-                                                ctypes.sizeof(ctypes.c_short))
+                                                  ctypes.sizeof(ctypes.c_short))
         return 0
```

## pyttsx3/drivers/nsss.py

```diff
@@ -8,16 +8,19 @@
 def buildDriver(proxy):
     return NSSpeechDriver.alloc().initWithProxy(proxy)
 
 
 class NSSpeechDriver(NSObject):
     @objc.python_method
     def initWithProxy(self, proxy):
-        self = super(NSSpeechDriver, self).init()
-        if self:
+        try:
+            proxy_attr = super(NSSpeechDriver, self).init()
+        except AttributeError:
+            proxy_attr = self
+        if proxy_attr:
             self._proxy = proxy
             self._tts = NSSpeechSynthesizer.alloc().initWithVoice_(None)
             self._tts.setDelegate_(self)
             # default rate
             self._tts.setRate_(200)
             self._completed = True
         return self
```

## pyttsx3/drivers/sapi5.py

```diff
@@ -1,8 +1,9 @@
 import comtypes.client  # Importing comtypes.client will make the gen subpackage
+
 try:
     from comtypes.gen import SpeechLib  # comtypes
 except ImportError:
     # Generate the SpeechLib lib and any associated files
     engine = comtypes.client.CreateObject("SAPI.SpVoice")
     stream = comtypes.client.CreateObject("SAPI.SpFileStream")
     from comtypes.gen import SpeechLib
```

## Comparing `py3_tts-3.0b0.dist-info/LICENSE` & `py3_tts-3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `py3_tts-3.0b0.dist-info/METADATA` & `py3_tts-3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3-tts
-Version: 3.0b0
+Version: 3.1
 Summary: Text to Speech (TTS) library for Python 3. Works without internet connection or delay. Supports multiple TTS engines, including Sapi5, nsss, and espeak.
 Author-email: Vignesh Sivanandha Rao <svignesh1793@gmail.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -374,15 +374,15 @@
         Exhibit B - "Incompatible With Secondary Licenses" Notice
         ---------------------------------------------------------
         
           This Source Code Form is "Incompatible With Secondary Licenses", as
           defined by the Mozilla Public License, v. 2.0.
         
 Project-URL: Homepage, https://github.com/thevickypedia/pyttsx3
-Project-URL: Docs, https://thevickypedia.github.io/pyttsx3
+Project-URL: Docs, https://pyttsx3.readthedocs.org/
 Project-URL: Source, https://github.com/thevickypedia/pyttsx3
 Keywords: pyttsx,ivona,pyttsx for python3,TTS for python3,pyttsx3,text to speech for python,tts,text to speech,speech,speech synthesis,offline text to speech,offline tts,gtts
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: MacOS :: MacOS X
@@ -410,23 +410,23 @@
 Installation
 ************
 ::
 
 	pip install py3-tts
 
 
-> If you get installation errors , make sure you first upgrade your wheel version using :  
+> If you get installation errors, make sure you first upgrade your wheel version using :
 `pip install --upgrade wheel`
 
 **Linux installation requirements :**
 #####################################
 
-+ If you are on a linux system and if the voice output is not working , then  : 
++ If you are on a Linux system and if the voice output is not working , then  :
 
-Install espeak , ffmpeg and libespeak1 as shown below: 
+Install espeak, ffmpeg, and libespeak1 as shown below:
 
 ::
 
 	sudo apt update && sudo apt install espeak ffmpeg libespeak1
 
 
 Usage :
@@ -435,44 +435,44 @@
 
 	import pyttsx3
 	engine = pyttsx3.init()
 	engine.say("I will speak this text")
 	engine.runAndWait()
 	
 	
-**Changing Voice , Rate and Volume :**
+**Changing Voice, Rate and Volume :**
 
 ::
 
 	import pyttsx3
 	engine = pyttsx3.init() # object creation
 
 	""" RATE"""
 	rate = engine.getProperty('rate')   # getting details of current speaking rate
-	print (rate)                        #printing current voice rate
+	print (rate)                        # printing current voice rate
 	engine.setProperty('rate', 125)     # setting up new voice rate
 
 
 	"""VOLUME"""
-	volume = engine.getProperty('volume')   #getting to know current volume level (min=0 and max=1)
-	print (volume)                          #printing current volume level
-	engine.setProperty('volume',1.0)    # setting up volume level  between 0 and 1
+	volume = engine.getProperty('volume')   # getting to know current volume level (min=0 and max=1)
+	print (volume)                          # printing current volume level
+	engine.setProperty('volume',1.0)        # setting up volume level  between 0 and 1
 
 	"""VOICE"""
-	voices = engine.getProperty('voices')       #getting details of current voice
-	#engine.setProperty('voice', voices[0].id)  #changing index, changes voices. o for male
-	engine.setProperty('voice', voices[1].id)   #changing index, changes voices. 1 for female
+	voices = engine.getProperty('voices')       # getting details of current voice
+	#engine.setProperty('voice', voices[0].id)  # changing index, changes voices. o for male
+	engine.setProperty('voice', voices[1].id)   # changing index, changes voices. 1 for female
 
 	engine.say("Hello World!")
 	engine.say('My current speaking rate is ' + str(rate))
 	engine.runAndWait()
 	engine.stop()
 
 	"""Saving Voice to a file"""
-	# On linux make sure that 'espeak' and 'ffmpeg' are installed
+	# On Linux make sure that 'espeak' and 'ffmpeg' are installed
 	engine.save_to_file('Hello World', 'test.mp3')
 	engine.runAndWait()
 
 
 **Full documentation of the Library**
 #####################################
 
@@ -487,9 +487,9 @@
 
 Feel free to wrap another text-to-speech engine for use with ``pyttsx3``.
 
 Project Links:
 **************
 
 * PyPI (https://pypi.python.org)
-* GitHub (https://github.com/nateshmbhat/pyttsx3)
+* GitHub (https://github.com/thevickypedia/pyttsx3)
 * Full Documentation (https://pyttsx3.readthedocs.org)
```

