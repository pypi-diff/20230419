# Comparing `tmp/plone.event-1.4.2.tar.gz` & `tmp/plone.event-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.event-1.4.2.tar", last modified: Tue Jan 24 18:36:32 2023, max compression
+gzip compressed data, was "plone.event-2.0.0.tar", last modified: Wed Apr 19 07:16:30 2023, max compression
```

## Comparing `plone.event-1.4.2.tar` & `plone.event-2.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-24 18:36:32.000000 plone.event-1.4.2/
--rw-r--r--   0 maurits    (501) staff       (20)     7853 2023-01-24 18:36:32.000000 plone.event-1.4.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-01-24 18:36:31.000000 plone.event-1.4.2/CONTRIBUTING.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-24 18:36:32.000000 plone.event-1.4.2/plone.event.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     7853 2023-01-24 18:36:32.000000 plone.event-1.4.2/plone.event.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-01-24 18:36:32.000000 plone.event-1.4.2/plone.event.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-01-24 18:36:32.000000 plone.event-1.4.2/plone.event.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)      949 2023-01-24 18:36:32.000000 plone.event-1.4.2/plone.event.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)      103 2023-01-24 18:36:32.000000 plone.event-1.4.2/plone.event.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-01-24 18:36:32.000000 plone.event-1.4.2/plone.event.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-01-24 18:36:32.000000 plone.event-1.4.2/plone.event.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-01-24 18:36:31.000000 plone.event-1.4.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      166 2023-01-24 18:36:31.000000 plone.event-1.4.2/MANIFEST.in
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-24 18:36:32.000000 plone.event-1.4.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-01-24 18:36:31.000000 plone.event-1.4.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)     1181 2023-01-24 18:36:31.000000 plone.event-1.4.2/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)      726 2023-01-24 18:36:31.000000 plone.event-1.4.2/docs/contributors.rst
--rw-r--r--   0 maurits    (501) staff       (20)      743 2023-01-24 18:36:31.000000 plone.event-1.4.2/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1729 2023-01-24 18:36:31.000000 plone.event-1.4.2/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-24 18:36:32.000000 plone.event-1.4.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-24 18:36:32.000000 plone.event-1.4.2/plone/event/
--rw-r--r--   0 maurits    (501) staff       (20)     5734 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      151 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    20973 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/recurrence.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7601 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/recurrence.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-24 18:36:32.000000 plone.event-1.4.2/plone/event/tests/
--rw-r--r--   0 maurits    (501) staff       (20)     2835 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     6672 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/tests/test_recurrence_sequence_ical.py
--rw-r--r--   0 maurits    (501) staff       (20)     2526 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/tests/test_recurrence_sequence_timedelta.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      434 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/tests/test_recurrence_int_sequence.py
--rw-r--r--   0 maurits    (501) staff       (20)      933 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/tests/test_doctest.py
--rw-r--r--   0 maurits    (501) staff       (20)     1826 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/tests/test_adapters.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    20425 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     6557 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/recurrence_dateutil.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3186 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/utils.rst
--rw-r--r--   0 maurits    (501) staff       (20)      868 2023-01-24 18:36:31.000000 plone.event-1.4.2/plone/event/adapters.py
--rw-r--r--   0 maurits    (501) staff       (20)      140 2023-01-24 18:36:32.000000 plone.event-1.4.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      254 2023-01-24 18:36:31.000000 plone.event-1.4.2/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4704 2023-01-24 18:36:31.000000 plone.event-1.4.2/CHANGES.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:16:30.678099 plone.event-2.0.0/
+-rw-r--r--   0 gil       (1000) gil       (1000)     4890 2023-04-19 07:16:30.000000 plone.event-2.0.0/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-19 07:16:30.000000 plone.event-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      166 2023-04-19 07:16:30.000000 plone.event-2.0.0/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)     5982 2023-04-19 07:16:30.678099 plone.event-2.0.0/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      254 2023-04-19 07:16:30.000000 plone.event-2.0.0/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:16:30.676099 plone.event-2.0.0/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1181 2023-04-19 07:16:30.000000 plone.event-2.0.0/docs/INSTALL.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)    17987 2023-04-19 07:16:30.000000 plone.event-2.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      743 2023-04-19 07:16:30.000000 plone.event-2.0.0/docs/LICENSE.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)      726 2023-04-19 07:16:30.000000 plone.event-2.0.0/docs/contributors.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:16:30.676099 plone.event-2.0.0/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:16:30.677099 plone.event-2.0.0/plone/event/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      836 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/adapters.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      154 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     5624 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     7519 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/recurrence.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    20975 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/recurrence.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     6553 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/recurrence_dateutil.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:16:30.678099 plone.event-2.0.0/plone/event/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1796 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/tests/test_adapters.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      851 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/tests/test_doctest.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      426 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/tests/test_recurrence_int_sequence.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6641 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/tests/test_recurrence_sequence_ical.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2508 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/tests/test_recurrence_sequence_timedelta.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2836 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/tests/test_utils.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    20390 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/utils.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3187 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone/event/utils.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:16:30.677099 plone.event-2.0.0/plone.event.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)     5982 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone.event.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      949 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone.event.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone.event.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone.event.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone.event.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)       98 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone.event.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-19 07:16:30.000000 plone.event-2.0.0/plone.event.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2864 2023-04-19 07:16:30.000000 plone.event-2.0.0/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-19 07:16:30.679099 plone.event-2.0.0/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1429 2023-04-19 07:16:30.000000 plone.event-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plone.event-1.4.2/plone.event.egg-info/SOURCES.txt` & `plone.event-2.0.0/plone.event.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.event-1.4.2/docs/LICENSE.GPL` & `plone.event-2.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.event-1.4.2/docs/INSTALL.txt` & `plone.event-2.0.0/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.event-1.4.2/docs/contributors.rst` & `plone.event-2.0.0/docs/contributors.rst`

 * *Files identical despite different names*

### Comparing `plone.event-1.4.2/docs/LICENSE.txt` & `plone.event-2.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.event-1.4.2/setup.py` & `plone.event-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,47 @@
-# -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '1.4.2'
+version = "2.0.0"
 
 setup(
-    name='plone.event',
+    name="plone.event",
     version=version,
     description="Event and calendaring related tools not bound to Plone",
-    long_description=(
-        open("README.rst").read() + "\n" + open(("CHANGES.rst")).read()
-    ),
+    long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
-        "Framework :: Plone :: 5.1",
-        "Framework :: Plone :: 5.2",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    keywords='Plone calendar calendaring event recurring',
-    author='Plone Foundation',
-    author_email='plone-developers@lists.sourceforge.net',
-    url='https://github.com/plone/plone.event',
-    license='GPL',
+    keywords="Plone calendar calendaring event recurring",
+    author="Plone Foundation",
+    author_email="plone-developers@lists.sourceforge.net",
+    url="https://github.com/plone/plone.event",
+    license="GPL",
     packages=find_packages(),
-    namespace_packages=['plone'],
+    namespace_packages=["plone"],
     include_package_data=True,
     zip_safe=False,
-    python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*',
+    python_requires=">=3.8",
     install_requires=[
-        'setuptools',
-        'python-dateutil',  # >4.0.2
-        'pytz',
-        'zope.component',
-        'zope.interface',
+        "setuptools",
+        "python-dateutil",  # >4.0.2
+        "pytz",
+        "zope.component",
+        "zope.interface",
     ],
-    extras_require={'test': [
-        'DateTime',
-        'mock',
-        'zope.configuration',
-    ], },
+    extras_require={
+        "test": [
+            "DateTime",
+            "zope.configuration",
+        ],
+    },
 )
```

### Comparing `plone.event-1.4.2/plone/event/interfaces.py` & `plone.event-2.0.0/plone/event/interfaces.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,95 +1,90 @@
-# -*- coding: utf-8 -*-
 from zope.interface import Attribute
 from zope.interface import Interface
 
 
 class IEvent(Interface):
-    """Event type marker interface.
-
-    """
+    """Event type marker interface."""
 
 
 class IEventRecurrence(Interface):
     """Event type marker interface for events with an RFC5545 compatible
     recurrence definition.
 
     """
 
 
 class IOccurrence(Interface):
     """Marker interface for an occurrence item, which represents a single
     occurrence.
 
     """
-    start = Attribute(u'Occurrence start date')
-    end = Attribute(u'Occurrence end date')
+
+    start = Attribute("Occurrence start date")
+    end = Attribute("Occurrence end date")
 
 
 class ICalendarAccessor(Interface):
     """Generic calendar accessor adapter interface.
 
     A calendar is a collection of calendar components, like events.
 
     """
-    uid = Attribute(u'UID of the calendar. Autogenerated, read only.')
+
+    uid = Attribute("UID of the calendar. Autogenerated, read only.")
     # rw attributes
-    title = Attribute(u'Calendar title.')
-    description = Attribute(u'Calendar description text.')
-    timezone = Attribute(u'Default timezone of the calendar.')
+    title = Attribute("Calendar title.")
+    description = Attribute("Calendar description text.")
+    timezone = Attribute("Default timezone of the calendar.")
 
     def items(self):
-        """Return a list of calendar component items, like events.
-
-        """
+        """Return a list of calendar component items, like events."""
 
 
 class IEventAccessor(Interface):
     """Event type generic accessor adapter interface.
 
     A specific adapter implementation should be provided by the individual
     content type packages.
 
     """
 
     # ro attributes
-    uid = Attribute(u'UID of the event. Autogenerated, read only.')
-    created = Attribute(u'Python datetime of the event creation timestamp.')
-    duration = Attribute(u'Duration of the event. Computed attribute.')
+    uid = Attribute("UID of the event. Autogenerated, read only.")
+    created = Attribute("Python datetime of the event creation timestamp.")
+    duration = Attribute("Duration of the event. Computed attribute.")
 
     # reference
     url = Attribute(
-        u'Cannonical, unique url of the event. External events '
-        u'are referenced by the origin url unless explicitly set.'
+        "Canonical, unique url of the event. External events "
+        "are referenced by the origin url unless explicitly set."
     )
 
     # rw attributes
-    last_modified = Attribute(u'Last modified Python datetime.')
-    title = Attribute(u'Event title.')
-    description = Attribute(u'Event description text.')
-    start = Attribute(u'Event start date as Python datetime.')
-    end = Attribute(u'Event end date as Python datetime.')
-    whole_day = Attribute(u'Event lasts whole day.')
-    open_end = Attribute(u'Event has no defined end time.')
-    timezone = Attribute(u'Timezone of the event. A pytz timezone identifier.')
-    recurrence = Attribute(u'RFC5545 compatible recurrence definition.')
-    location = Attribute(u'Location of the event.')
-    attendees = Attribute(u'List of attendees.')
-    contact_name = Attribute(u'Contact name.')
-    contact_email = Attribute(u'Contact email.')
-    contact_phone = Attribute(u'Contact phone.')
-    event_url = Attribute(u'Website of the event.')
-    subjects = Attribute(u'Categories.')
-    text = Attribute(u'Body text of the event.')
+    last_modified = Attribute("Last modified Python datetime.")
+    title = Attribute("Event title.")
+    description = Attribute("Event description text.")
+    start = Attribute("Event start date as Python datetime.")
+    end = Attribute("Event end date as Python datetime.")
+    whole_day = Attribute("Event lasts whole day.")
+    open_end = Attribute("Event has no defined end time.")
+    timezone = Attribute("Timezone of the event. A pytz timezone identifier.")
+    recurrence = Attribute("RFC5545 compatible recurrence definition.")
+    location = Attribute("Location of the event.")
+    attendees = Attribute("List of attendees.")
+    contact_name = Attribute("Contact name.")
+    contact_email = Attribute("Contact email.")
+    contact_phone = Attribute("Contact phone.")
+    event_url = Attribute("Website of the event.")
+    subjects = Attribute("Categories.")
+    text = Attribute("Body text of the event.")
 
 
 class IRecurrenceSupport(Interface):
-    """Event type recurrence adatper.
-
-    """
+    """Event type recurrence adapter."""
 
     def occurrences(self, range_start, range_end):
         """Return a list of IOccurrence objects with custom attributes of the
         specific occurrence set.
 
         :param range_start: Search for occurrences after this date.
         :type range_start: Python datetime.
@@ -97,17 +92,15 @@
         :param range_end: Search for occurrences before this date.
         :type range_end: Python datetime.
 
         """
 
 
 class IICalendar(Interface):
-    """Adapter, which is used to construct an icalendar object.
-
-    """
+    """Adapter, which is used to construct an icalendar object."""
 
 
 class IICalendarEventComponent(Interface):
     """Adapter, which is used to construct an event component object for
     icalendar.
 
     """
@@ -152,41 +145,42 @@
     ; and MAY occur more than once.
     ;
     attach / attendee / categories / comment /
     contact / exdate / rstatus / related /
     resources / rdate / x-prop / iana-prop
 
     """
-    dtstart = Attribute(u'Start Date/Time')
-    dtend = Attribute(u'End Date/Time')
-    duration = Attribute(u'Duration')
-    rrule = Attribute(u'Recurrence Rule')
-    description = Attribute(u'Description')
-    location = Attribute(u'Location')
-    summary = Attribute(u'Summary')
-    url = Attribute(u'Url')
-    attendee = Attribute(u'Attendee')
-    categories = Attribute(u'Categories')
-    contact = Attribute(u'Contact')
-
-    exdate = Attribute(u'Exdate')
-    rdate = Attribute(u'Rdate')
-
-    dtstamp = Attribute(u'Timestamp')
-    uid = Attribute(u'Unique identifier')
-    klass = Attribute(u'Class')  # class
-    created = Attribute(u'Created')
-    geo = Attribute(u'Geo')
-    last_mod = Attribute(u'Last Modified')  # last-mod
-    organizer = Attribute(u'Organizer')
-    priority = Attribute(u'Priority')
-    seq = Attribute(u'Seq')
-    status = Attribute(u'Status')
-    transp = Attribute(u'Transp')
-    recurid = Attribute(u'Recurid')
-    attach = Attribute(u'Attach')
-    comment = Attribute(u'Comment')
-    rstatus = Attribute(u'Rstatus')
-    related = Attribute(u'Related')
-    resources = Attribute(u'Resources')
-    x_prop = Attribute(u'X Prop')  # x-prop
-    iana_prop = Attribute(u'Iana Prop')  # iana-prop
+
+    dtstart = Attribute("Start Date/Time")
+    dtend = Attribute("End Date/Time")
+    duration = Attribute("Duration")
+    rrule = Attribute("Recurrence Rule")
+    description = Attribute("Description")
+    location = Attribute("Location")
+    summary = Attribute("Summary")
+    url = Attribute("Url")
+    attendee = Attribute("Attendee")
+    categories = Attribute("Categories")
+    contact = Attribute("Contact")
+
+    exdate = Attribute("Exdate")
+    rdate = Attribute("Rdate")
+
+    dtstamp = Attribute("Timestamp")
+    uid = Attribute("Unique identifier")
+    klass = Attribute("Class")  # class
+    created = Attribute("Created")
+    geo = Attribute("Geo")
+    last_mod = Attribute("Last Modified")  # last-mod
+    organizer = Attribute("Organizer")
+    priority = Attribute("Priority")
+    seq = Attribute("Seq")
+    status = Attribute("Status")
+    transp = Attribute("Transp")
+    recurid = Attribute("Recurid")
+    attach = Attribute("Attach")
+    comment = Attribute("Comment")
+    rstatus = Attribute("Rstatus")
+    related = Attribute("Related")
+    resources = Attribute("Resources")
+    x_prop = Attribute("X Prop")  # x-prop
+    iana_prop = Attribute("Iana Prop")  # iana-prop
```

### Comparing `plone.event-1.4.2/plone/event/recurrence.rst` & `plone.event-2.0.0/plone/event/recurrence.rst`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     [datetime.datetime(2010, 10, 28, 9, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CEST+2:00:00 DST>),
         datetime.datetime(2010, 10, 29, 9, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CEST+2:00:00 DST>),
         datetime.datetime(2010, 10, 30, 9, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CEST+2:00:00 DST>),
         datetime.datetime(2010, 10, 31, 9, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CET+1:00:00 STD>),
         datetime.datetime(2010, 11, 1, 9, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CET+1:00:00 STD>)]
 
 
-Note, that recurrence_sequence_ical calculates occurences timezone naively and
+Note, that recurrence_sequence_ical calculates occurrences timezone naively and
 applies timezones afterwards. This leads into a problem in corner cases:
     >>> list(recurrence_sequence_ical(
     ...      start=at.localize(datetime(2010,10,30,23,0,0,0)),
     ...      recrule="""RRULE:FREQ=HOURLY;INTERVAL=1;COUNT=7"""
     ...      ))
     [datetime.datetime(2010, 10, 30, 23, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CEST+2:00:00 DST>),
         datetime.datetime(2010, 10, 31, 0, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CEST+2:00:00 DST>),
@@ -105,18 +105,18 @@
     [datetime.datetime(2010, 1, 4, 0, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CET+1:00:00 STD>),
         datetime.datetime(2010, 1, 6, 0, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CET+1:00:00 STD>),
         datetime.datetime(2010, 1, 8, 0, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CET+1:00:00 STD>),
         datetime.datetime(2010, 1, 10, 0, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CET+1:00:00 STD>),
         datetime.datetime(2010, 1, 20, 0, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CET+1:00:00 STD>)]
 
 
-Limiting number of occurences
+Limiting number of occurrences
 -----------------------------
 
-Until (date until recurrence happens) and count (Number of occurences) can also
+Until (date until recurrence happens) and count (Number of occurrences) can also
 be given in recurrence_sequence_ical, instead of defining it in the rrule.
 But defining it in a rrule gives more flexibility since you can set it for each
 rrule individually.
 If MAXCOUNT is exceeded, recurrence generation will stop regardless of any other
 setting.
 
 ...init
@@ -297,33 +297,33 @@
         datetime.datetime(2008, 3, 30, 15, 0, tzinfo=<DstTzInfo 'CET' CEST+2:00:00 DST>),
         datetime.datetime(2008, 3, 30, 16, 0, tzinfo=<DstTzInfo 'CET' CEST+2:00:00 DST>),
         datetime.datetime(2008, 3, 30, 17, 0, tzinfo=<DstTzInfo 'CET' CEST+2:00:00 DST>),
         datetime.datetime(2008, 3, 30, 18, 0, tzinfo=<DstTzInfo 'CET' CEST+2:00:00 DST>),
         datetime.datetime(2008, 3, 30, 19, 0, tzinfo=<DstTzInfo 'CET' CEST+2:00:00 DST>),
         datetime.datetime(2008, 3, 30, 20, 0, tzinfo=<DstTzInfo 'CET' CEST+2:00:00 DST>)]
 
-Usally we want an clever behaviour, dependend on delta. This is implemented
+Usually we want a clever behaviour, dependent on delta. This is implemented
 with DSTAUTO, which is the default behaviour.
 
-Here the correct behaviour on day level or above: DSTADJUST is choosen.
+Here the correct behaviour on day level or above: DSTADJUST is chosen.
 
     >>> start = datetime(2008, 3, 29, 11, 0, 0, 0, pytz.timezone('CET'))
     >>> until = datetime(2008, 3, 31, 11, 0, 0, 0, pytz.timezone('CET'))
     >>> until = utcoffset_normalize(until, dstmode=DSTADJUST)
     >>> until
     datetime.datetime(2008, 3, 31, 11, 0, tzinfo=<DstTzInfo 'CET' CEST+2:00:00 DST>)
 
     >>> dates = recurrence_sequence_timedelta(start, delta=24*60, until=until)
     >>> list(dates)
     [datetime.datetime(2008, 3, 29, 11, 0, tzinfo=<DstTzInfo 'CET' CET+1:00:00 STD>),
         datetime.datetime(2008, 3, 30, 11, 0, tzinfo=<DstTzInfo 'CET' CEST+2:00:00 DST>),
         datetime.datetime(2008, 3, 31, 11, 0, tzinfo=<DstTzInfo 'CET' CEST+2:00:00 DST>)]
 
 
-The correct behaviour on below day level: DSTKEEP is choosen.
+The correct behaviour on below day level: DSTKEEP is chosen.
 
     >>> start = datetime(2008, 3, 29, 21, 0, 0, 0, pytz.timezone('CET'))
     >>> until = datetime(2008, 3, 30, 21, 0, 0, 0, pytz.timezone('CET')) - timedelta(microseconds=1)
     >>> until = utcoffset_normalize(until, dstmode=DSTADJUST)
     >>> dates = recurrence_sequence_timedelta(start, delta=60, until=until)
     >>> len(list(dates))
     23
@@ -394,15 +394,15 @@
     [datetime.datetime(2008, 8, 26, 23, 59, tzinfo=<DstTzInfo 'CET' CEST+2:00:00 DST>)]
 
 Comparison of two datetime with same time related to UTC but in different
 timezones works.
     >>> seqDT[0] == seqdt[0]
     True
 
-Does integer represenation work?
+Does integer representation work?
     >>> seqDT = list(recurrence_int_sequence(recurrence_sequence_timedelta(DT, 0, None)))
     >>> seqdt = list(recurrence_int_sequence(recurrence_sequence_timedelta(dt, 0, None)))
 
 Integer sequences are the same anyways, because dates are converted to UTC first.
     >>> seqDT[0] == seqdt[0]
     True
```

### Comparing `plone.event-1.4.2/plone/event/recurrence.py` & `plone.event-2.0.0/plone/event/recurrence.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from dateutil import rrule
 from plone.event.utils import DSTAUTO
 from plone.event.utils import dt2int
 from plone.event.utils import pydt
 from plone.event.utils import tzdel
 from plone.event.utils import utc
 from plone.event.utils import utcoffset_normalize
@@ -12,20 +11,20 @@
 
 
 # TODO: make me configurable
 MAXCOUNT = 1000  # Maximum number of occurrences
 
 
 def recurrence_sequence_ical(
-        start,
-        recrule=None,
-        from_=None,
-        until=None,
-        count=None,
-        duration=None,
+    start,
+    recrule=None,
+    from_=None,
+    until=None,
+    count=None,
+    duration=None,
 ):
     """Calculates a sequence of datetime objects from a recurrence rule
     following the RFC2445 specification, using python-dateutil recurrence
     rules.  The resolution of the resulting datetime objects is one second,
     since python-dateutil rrulestr doesn't support microseconds.
 
     :param start:   datetime or DateTime instance of the date from which the
@@ -41,21 +40,21 @@
     :type from_: datetime.datetime
 
     :param until:   Optional datetime or DateTime instance of the date, until
                     the recurrence is calculated. If not given, count or
                     MAXDATE limit the recurrence calculation.
     :type until: datetime.datetime
 
-    :param count:   Optional integer which defines the number of occurences.
+    :param count:   Optional integer which defines the number of occurrences.
                     If not given, until or MAXDATE limits the recurrence
                     calculation.
     :type count: integer
 
     :param duration: Optional timedelta instance, which is used to calculate
-                     if a occurence datetime plus duration is within the
+                     if a occurrence datetime plus duration is within the
                      queried timerange.
     :type duration:  datetime.timedelta
 
     :returns: A generator which generates a sequence of datetime instances.
     :rtype: generator
 
     """
@@ -64,15 +63,15 @@
     from_ = pydt(from_, exact=False)
     until = pydt(until, exact=False)
     tz = start.tzinfo
     start = tzdel(start)  # tznaive | start defines tz
     _from = tzdel(from_)
     _until = tzdel(until)
     if duration:
-        assert (isinstance(duration, datetime.timedelta))
+        assert isinstance(duration, datetime.timedelta)
     else:
         duration = datetime.timedelta(0)
 
     if recrule:
         # TODO BUGFIX WRONG TIME DEFINITIONS
         # THIS HACK ensures, that UNTIL, RDATE and EXDATE definitions with
         # incorrect time (currently always set to 0:00 by the recurrence
@@ -84,24 +83,24 @@
         # - RDATE definitions should have the same time as the start date.
         # - EXDATE definitions should exclude occurrences on the specific date
         #   only the same time as the start date.
         # In the long term ,the recurrence widget should be able to set the
         # time for UNTIL, RDATE and EXDATE.
         t0 = start.time()  # set initial time information.
         # First, replace all times in the recurring rule with starttime
-        t0str = 'T{0:02d}{1:02d}{2:02d}'.format(t0.hour, t0.minute, t0.second)
+        t0str = f"T{t0.hour:02d}{t0.minute:02d}{t0.second:02d}"
         # Replace any times set to 000000 with start time, not all
         # rrules are set by a specific broken widget.  Don't waste time
         # subbing if the start time is already 000000.
-        if t0str != 'T000000':
-            recrule = re.sub(r'T000000', t0str, recrule)
+        if t0str != "T000000":
+            recrule = re.sub(r"T000000", t0str, recrule)
         # Then, replace incorrect until times with the end of the day
         recrule = re.sub(
-            r'(UNTIL[^T]*[0-9]{8})T(000000)',
-            r'\1T235959',
+            r"(UNTIL[^T]*[0-9]{8})T(000000)",
+            r"\1T235959",
             recrule,
         )
 
         # RFC2445 string
         # forceset: always return a rruleset
         # dtstart: optional used when no dtstart is in RFC2445 string
         #          dtstart is given as timezone naive time. timezones are
@@ -137,37 +136,37 @@
             break
 
         yield date
     return
 
 
 def recurrence_sequence_timedelta(
-        start,
-        delta=None,
-        until=None,
-        count=None,
-        dst=DSTAUTO,
+    start,
+    delta=None,
+    until=None,
+    count=None,
+    dst=DSTAUTO,
 ):
-    """ Calculates a sequence of datetime objects from a timedelta integer,
-    which defines the minutes between each occurence.
+    """Calculates a sequence of datetime objects from a timedelta integer,
+    which defines the minutes between each occurrence.
 
     :param start: datetime or DateTime instance of the date from which the
                   recurrence sequence is calculated.
     :type start: datetime
 
     :param delta: Integer which defines the minutes
-                  between each date occurence.
+                  between each date occurrence.
     :type delta: integer
 
     :param until: datetime or DateTime instance of the date, until the
                   recurrence is calculated. If not given,
                   count or MAXDATE limit the recurrence calculation.
     :type until: datetime
 
-    :param count: Integer which defines the number of occurences. If not given,
+    :param count: Integer which defines the number of occurrences. If not given,
                   until or MAXDATE limits the recurrence calculation.
     :param count: integer
 
     :param dst:   Daylight Saving Time crossing behavior. DSTAUTO, DSTADJUST or
                   DSTKEEP. For more information, see
                   plone.event.utils.utcoffset_normalize.
     :param dst: string
@@ -201,15 +200,15 @@
         cnt += 1
 
         yield after
         before = after
 
 
 def recurrence_int_sequence(sequence):
-    """ Generates a sequence of integer representations from a sequence of
+    """Generates a sequence of integer representations from a sequence of
     dateime instances.
 
     :param sequence: An iterable sequence of datetime instances.
     :type sequence: iterable
     :returns: Generator of integer representations of datetime instances.
     :rtype: generator
```

### Comparing `plone.event-1.4.2/plone/event/tests/test_recurrence_sequence_ical.py` & `plone.event-2.0.0/plone/event/tests/test_recurrence_sequence_ical.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,172 +1,182 @@
-# -*- coding: utf-8 -*-
 import unittest
 
 
 class TestRecurrenceSequenceIcal(unittest.TestCase):
     def test_start(self):
-        from plone.event.recurrence import recurrence_sequence_ical
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_ical
+
         start = datetime(2011, 11, 23)
         seq = recurrence_sequence_ical(start)
         results = [res for res in seq]
         self.assertEqual(len(results), 1)
 
     def test_recrule_str(self):
-        from plone.event.recurrence import recurrence_sequence_ical
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_ical
+
         start = datetime(2011, 11, 23)
-        recrule = 'FREQ=DAILY;INTERVAL=10;COUNT=5'
+        recrule = "FREQ=DAILY;INTERVAL=10;COUNT=5"
         seq = recurrence_sequence_ical(start, recrule=recrule)
         results = [res for res in seq]
         self.assertEqual(len(results), 5)
 
     def test_recrule_str_rdate(self):
         """Test, if an RDATE date has the correct time set.
-            See: "BUGFIX WRONG RDATE TIME" in recurrence.py
+        See: "BUGFIX WRONG RDATE TIME" in recurrence.py
         """
-        from plone.event.recurrence import recurrence_sequence_ical
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_ical
+
         start = datetime(2011, 11, 23, 10, 10)
         recrule = """FREQ=DAILY;INTERVAL=1;COUNT=3
 RDATE:20111129T000000"""
         seq = recurrence_sequence_ical(start, recrule=recrule)
         results = [res for res in seq]
         self.assertEqual(len(results), 4)
         self.assertEqual(results[0].time(), results[-1].time())
 
     def test_recrule_str_exdate(self):
-        """Test, if an EXDATE date are not in the resulting recurrence set.
-        """
-        from plone.event.recurrence import recurrence_sequence_ical
+        """Test, if an EXDATE date are not in the resulting recurrence set."""
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_ical
+
         import pytz
-        at = pytz.timezone('Europe/Vienna')
+
+        at = pytz.timezone("Europe/Vienna")
         start = at.localize(datetime(2013, 6, 29, 10, 10))
-        recrule = 'RRULE:FREQ=DAILY;COUNT=4\r\nEXDATE:20130630T000000,20130701T000000\r\nRDATE:20130706T000000,20130809T000000'  # noqa
+        recrule = "RRULE:FREQ=DAILY;COUNT=4\r\nEXDATE:20130630T000000,20130701T000000\r\nRDATE:20130706T000000,20130809T000000"  # noqa
         seq = recurrence_sequence_ical(start, recrule=recrule)
         res = [res for res in seq]
         res_test = [
             at.localize(datetime(2013, 6, 29, 10, 10)),
             at.localize(datetime(2013, 7, 2, 10, 10)),
             at.localize(datetime(2013, 7, 6, 10, 10)),
-            at.localize(datetime(2013, 8, 9, 10, 10))
+            at.localize(datetime(2013, 8, 9, 10, 10)),
         ]
         self.assertEqual(len(res), 4)
         self.assertEqual(res, res_test)
 
     def test_recrule_str_until(self):
         """Test, if UNTIL stops the sequence at the end of the day, even if
         it's set to 0:00 by the recurrence widget.
         """
-        from plone.event.recurrence import recurrence_sequence_ical
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_ical
+
         import pytz
-        at = pytz.timezone('Europe/Vienna')
+
+        at = pytz.timezone("Europe/Vienna")
         start = at.localize(datetime(2013, 6, 29, 10, 10))
-        recrule = 'RRULE:FREQ=DAILY;UNTIL=20130702T000000'
+        recrule = "RRULE:FREQ=DAILY;UNTIL=20130702T000000"
         seq = recurrence_sequence_ical(start, recrule=recrule)
         res = [res for res in seq]
         res_test = [
             at.localize(datetime(2013, 6, 29, 10, 10)),
             at.localize(datetime(2013, 6, 30, 10, 10)),
             at.localize(datetime(2013, 7, 1, 10, 10)),
-            at.localize(datetime(2013, 7, 2, 10, 10))
+            at.localize(datetime(2013, 7, 2, 10, 10)),
         ]
         self.assertEqual(len(res), 4)
         self.assertEqual(res, res_test)
 
     def test_recrule_from_until(self):
-        from plone.event.recurrence import recurrence_sequence_ical
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_ical
+
         start = datetime(2011, 11, 23)
         recrule = None
         from_ = datetime(2011, 11, 1)
         until = datetime(2011, 12, 31)
         seq = recurrence_sequence_ical(
             start,
             recrule=recrule,
             from_=from_,
             until=until,
         )
         results = [res for res in seq]
         self.assertEqual(len(results), 1)
 
     def test_recrule_str_more_than_MAXCOUNT(self):
-        from plone.event.recurrence import recurrence_sequence_ical
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_ical
+
         start = datetime(2011, 11, 23)
-        recrule = 'FREQ=DAILY;INTERVAL=10;COUNT=1001'
+        recrule = "FREQ=DAILY;INTERVAL=10;COUNT=1001"
         seq = recurrence_sequence_ical(start, recrule=recrule)
         results = [res for res in seq]
         self.assertEqual(len(results), 1000)
 
     def test_recrule_str_more_than_count(self):
-        from plone.event.recurrence import recurrence_sequence_ical
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_ical
+
         start = datetime(2011, 11, 23)
-        recrule = 'FREQ=DAILY;INTERVAL=10;COUNT=10'
+        recrule = "FREQ=DAILY;INTERVAL=10;COUNT=10"
         count = 5
         seq = recurrence_sequence_ical(start, recrule=recrule, count=count)
         results = [res for res in seq]
         self.assertEqual(len(results), 5)
 
     def test_recrule_from(self):
-        from plone.event.recurrence import recurrence_sequence_ical
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_ical
+
         start = datetime(2011, 11, 23)
-        recrule = 'FREQ=DAILY;INTERVAL=1;COUNT=5'
+        recrule = "FREQ=DAILY;INTERVAL=1;COUNT=5"
         from_ = datetime(2011, 11, 25)
         until = datetime(2011, 11, 27)
         seq = recurrence_sequence_ical(
             start,
             recrule=recrule,
             from_=from_,
             until=until,
         )
         results = [res for res in seq]
         self.assertEqual(len(results), 3)
 
     def test_recrule_until(self):
-        from plone.event.recurrence import recurrence_sequence_ical
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_ical
+
         start = datetime(2011, 11, 24)
-        recrule = 'FREQ=DAILY;INTERVAL=1;COUNT=5'
+        recrule = "FREQ=DAILY;INTERVAL=1;COUNT=5"
         from_ = datetime(2011, 11, 23)
         until = datetime(2011, 11, 27)
         seq = recurrence_sequence_ical(
             start,
             recrule=recrule,
             from_=from_,
             until=until,
         )
         results = [res for res in seq]
         self.assertEqual(len(results), 4)
 
     def test_recrule_from_until_with_duration(self):
-        """Should include events ranging into the queried timerange.
-        """
-        from plone.event.recurrence import recurrence_sequence_ical
+        """Should include events ranging into the queried timerange."""
         from datetime import datetime
         from datetime import timedelta
+        from plone.event.recurrence import recurrence_sequence_ical
+
         start = datetime(2011, 11, 23)
-        recrule = 'FREQ=DAILY;INTERVAL=1;COUNT=5'
+        recrule = "FREQ=DAILY;INTERVAL=1;COUNT=5"
         from_ = datetime(2011, 11, 26)
         until = datetime(2011, 11, 27)
         seq = recurrence_sequence_ical(
             start,
             recrule=recrule,
             from_=from_,
             until=until,
             duration=timedelta(days=2),
         )
         results = [res for res in seq]
         self.assertEqual(len(results), 4)
 
     def test_recrule_until_with_timezone(self):
-        from plone.event.recurrence import recurrence_sequence_ical
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_ical
 
         start = datetime(2011, 11, 24)
-        recrule = 'RRULE:FREQ=DAILY;UNTIL=20111130T000000Z'
+        recrule = "RRULE:FREQ=DAILY;UNTIL=20111130T000000Z"
         seq = list(recurrence_sequence_ical(start, recrule=recrule))
         self.assertEqual(len(seq), 7)
```

### Comparing `plone.event-1.4.2/plone/event/tests/test_recurrence_sequence_timedelta.py` & `plone.event-2.0.0/plone/event/tests/test_recurrence_sequence_timedelta.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,68 @@
-# -*- coding: utf-8 -*-
 import unittest
 
 
 class TestRecurrenceSequenceTimedelta(unittest.TestCase):
     def test_delta_None(self):
-        from plone.event.recurrence import recurrence_sequence_timedelta
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_timedelta
+
         start = datetime(2011, 11, 23)
         until = datetime(2011, 11, 24)
         td = recurrence_sequence_timedelta(start, until=until)
         results = [res for res in td]
         self.assertEqual(len(results), 1)
 
     def test_delta_zero(self):
-        from plone.event.recurrence import recurrence_sequence_timedelta
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_timedelta
+
         start = datetime(2011, 11, 23)
         delta = 0
         until = datetime(2011, 11, 24)
         td = recurrence_sequence_timedelta(start, delta=delta, until=until)
         results = [res for res in td]
         self.assertEqual(len(results), 1)
 
     def test_until_None(self):
-        from plone.event.recurrence import recurrence_sequence_timedelta
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_timedelta
+
         start = datetime(2011, 11, 23)
         delta = 1
         td = recurrence_sequence_timedelta(start, delta=delta)
         results = [res for res in td]
         self.assertEqual(len(results), 1)
 
     def test_delta_an_hour_until_next_day(self):
-        from plone.event.recurrence import recurrence_sequence_timedelta
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_timedelta
+
         start = datetime(2011, 11, 23)
         delta = 60
         until = datetime(2011, 11, 24)
         td = recurrence_sequence_timedelta(start, delta=delta, until=until)
         results = [res for res in td]
         self.assertEqual(len(results), 25)
 
     def test_recur_more_than_MAXCOUNT(self):
-        from plone.event.recurrence import recurrence_sequence_timedelta
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_timedelta
+
         start = datetime(2011, 11, 23)
         delta = 1
         until = datetime(2012, 11, 23)
         td = recurrence_sequence_timedelta(start, delta=delta, until=until)
         results = [res for res in td]
         self.assertEqual(len(results), 1001)
 
     def test_recur_more_than_count(self):
-        from plone.event.recurrence import recurrence_sequence_timedelta
         from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_timedelta
+
         start = datetime(2011, 11, 23)
         delta = 1
         until = datetime(2011, 11, 24)
         count = 20
         td = recurrence_sequence_timedelta(
             start,
             delta=delta,
```

### Comparing `plone.event-1.4.2/plone/event/tests/test_adapters.py` & `plone.event-2.0.0/plone/event/tests/test_adapters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-# -*- coding: utf-8 -*-
 from datetime import datetime
 from plone.event.interfaces import IEvent
 from plone.event.interfaces import IEventAccessor
 from zope.configuration import xmlconfig
 
 import pytz
 import unittest
 import zope.interface
 
 
-class MockObject(object):
+class MockObject:
     """Mock object"""
 
 
 class TestAdapters(unittest.TestCase):
     def setUp(self):
         import zope.component
-        context = xmlconfig.file('meta.zcml', zope.component)
-        xmlconfig.file('configure.zcml', zope.component, context=context)
+
+        context = xmlconfig.file("meta.zcml", zope.component)
+        xmlconfig.file("configure.zcml", zope.component, context=context)
 
         import plone.event
-        xmlconfig.file('configure.zcml', plone.event, context=context)
+
+        xmlconfig.file("configure.zcml", plone.event, context=context)
 
     def test_event_accessor(self):
         obj = MockObject()
-        tz = pytz.timezone('Europe/Vienna')
+        tz = pytz.timezone("Europe/Vienna")
         obj.start = datetime(2012, 12, 12, 10, 0, tzinfo=tz)
         obj.end = datetime(2012, 12, 12, 12, 0, tzinfo=tz)
         zope.interface.alsoProvides(obj, IEvent)
 
         # Create accessor
         acc = IEventAccessor(obj)
 
@@ -45,13 +46,13 @@
         self.assertTrue(acc.start == obj.start == start)
         self.assertTrue(acc.end == obj.end == end)
 
         # Accessor deletor
         acc.something = True
         self.assertTrue(acc.something == obj.something is True)
         del acc.something
-        self.assertTrue(hasattr(acc, 'something') is False)
-        self.assertTrue(hasattr(obj, 'something') is False)
+        self.assertTrue(hasattr(acc, "something") is False)
+        self.assertTrue(hasattr(obj, "something") is False)
 
         del acc.start
-        self.assertTrue(hasattr(acc, 'start') is False)
-        self.assertTrue(hasattr(obj, 'start') is False)
+        self.assertTrue(hasattr(acc, "start") is False)
+        self.assertTrue(hasattr(obj, "start") is False)
```

### Comparing `plone.event-1.4.2/plone/event/utils.py` & `plone.event-2.0.0/plone/event/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from datetime import date
 from datetime import datetime
 from datetime import timedelta
 
 import logging
 import os
 import pytz
@@ -55,24 +54,24 @@
     """
     try:
         # following statement ensures, that timezone is a valid pytz/Olson zone
         return pytz.timezone(timezone).zone
     except Exception:
         if fallback:
             logger.warn(
-                "The timezone {0} is not a valid timezone from the "
-                "Olson database or pytz. Falling back to {1}.".format(
+                "The timezone {} is not a valid timezone from the "
+                "Olson database or pytz. Falling back to {}.".format(
                     timezone,
                     fallback,
                 )
             )
             return fallback
         else:
             raise ValueError(
-                "The timezone {0} is not a valid timezone from "
+                "The timezone {} is not a valid timezone from "
                 "the Olson database or pytz.".format(timezone)
             )
 
 
 def default_timezone(fallback="UTC"):
     """Retrieve the timezone from the server.
     Default Fallback: UTC
@@ -146,15 +145,15 @@
     :type end: Python datetime or Zope DateTime
     :param exact: If True, the resolution goes down to microseconds. If False,
                   the resolution are seconds. Default is False.
     :type exact: Boolean
     :returns: True, if start and end have the same time, otherwise False.
     :rtype: Boolean.
 
-    >>> from plone.event.utils import is_same_time, pydt
+    >>> from plone.event.utils import is_same_time
     >>> from datetime import datetime, timedelta
 
     >>> is_same_time(datetime.now(), datetime.now()+timedelta(hours=1))
     False
 
     >>> is_same_time(datetime.now(), datetime.now()+timedelta(days=1))
     True
@@ -269,15 +268,15 @@
                   This is what humans might expect when recurring rules are
                   defined.
                   Mode DSTKEEP: When crossing daylight saving time changes, the
                   start time of the date before and after DST change will be
                   the same relative to UTC.  So, 8:00 GMT+1 before will result
                   in 7:00 GMT+2 afterwards. This behavior might be what
                   machines expect, when recurrence rules are defined.
-                  Mode DSTAUTO: If the relative delta between two occurences of
+                  Mode DSTAUTO: If the relative delta between two occurrences of
                   a reucurrence sequence is less than a day, DSTKEEP will be
                   used - otherwise DSTADJUST. This behavior is the default.
     """
     try:
         assert bool(date.tzinfo)
     except Exception:
         raise TypeError("Cannot normalize timezone naive dates")
@@ -505,33 +504,33 @@
 
     return ret
 
 
 def guesstz(DT):
     """'Guess' pytz from a zope DateTime.
 
-    !!! theres no real good method to guess the timezone.
+    !!! there is no real good method to guess the timezone.
     DateTime was build somewhere in 1998 long before python had a working
     datetime implementation available and still stucks with this incomplete
     implementation.
 
     >>> from DateTime import DateTime
     >>> from plone.event.utils import guesstz
 
     Timezones with the same name as in the Olson DB can easily be guessed.
     >>> guesstz(DateTime('2010-01-01 Europe/Vienna')).zone
     'Europe/Vienna'
 
     GMT timezones which are popular with DateTime cannot be guessed,
-    unfortunatly
+    unfortunately
     >>> guesstz(DateTime('2010-01-01 GMT+1'))
     """
     tzname = DT.timezone()
 
-    # Please note, the GMT offset based timezone informations in DateTime are
+    # Please note, the GMT offset based timezone information in DateTime are
     # not compatible with Etc/GMT based from pytz. They have different offsets.
     try:
         tz = pytz.timezone(tzname)
         return tz
     except KeyError:
         pass
     return None
@@ -554,15 +553,15 @@
     dt = utc(dt)
     value = (((dt.year * 12 + dt.month) * 31 + dt.day) * 24 + dt.hour) * 60 + dt.minute
 
     # TODO: unit test me
     if value > MAX32:
         # value must be integer fitting in the 32bit range
         raise OverflowError(
-            """{0} is not within the range of indexable dates,<<
+            """{} is not within the range of indexable dates,<<
             exceeding 32bit range.""".format(
                 dt
             )
         )
     return value
 
 
@@ -659,15 +658,15 @@
 
     """
     # TODO: rfc2445dt might not be necessary. drop me then.
 
     dt = pydt(dt)
     if mode == "utc":
         dt = utc(dt)
-    date = "{0}{1}{2}{3}".format(
+    date = "{}{}{}{}".format(
         date and dt.strftime("%Y%m%d") or "",
         date and time and "T" or "",
         time and dt.strftime("%H%M%S") or "",
         mode == "utc" and "Z" or "",
     )
     if mode == "local":
         return date, dt.tzinfo.zone
```

### Comparing `plone.event-1.4.2/plone/event/recurrence_dateutil.rst` & `plone.event-2.0.0/plone/event/recurrence_dateutil.rst`

 * *Files 3% similar despite different names*

```diff
@@ -45,39 +45,39 @@
     >>> list(recurrence_sequence_ical(start, recrule=recrule))
     [datetime.datetime(2010, 10, 30, 0, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CEST+2:00:00 DST>),
         datetime.datetime(2010, 10, 31, 0, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CEST+2:00:00 DST>),
         datetime.datetime(2010, 11, 1, 0, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CET+1:00:00 STD>)]
 
 
 It's safer to let rrule calculate timezone naive dates and localizing them
-afterwards than letting rrule substracting (EXDATE) timezone correct dates from
+afterwards than letting rrule subtracting (EXDATE) timezone correct dates from
 a possibly timezone incorrect recurrence sequence. This issue will be gone, if
 rrule does TZ normalizing itself before applying EXDATE to the recurrence
 sequence.
 
-See here... This is our recurrence rule. We want to substract from the sequence
+See here... This is our recurrence rule. We want to subtract from the sequence
 the date 2010-10-31, 23:30 in UTC, which is 2010-11-01, 0:30 in Austria, UTC+1
 
 ::
 
     >>> recrule = """RRULE:FREQ=DAILY;INTERVAL=1;COUNT=3
     ...              EXDATE:20101031T233000Z"""
 
 If we let the sequence start from 1st November, the 1st November is correctly
-substracted, since the sequence has all correct timezones.
+subtracted, since the sequence has all correct timezones.
 
 ::
 
     >>> start = at.localize(datetime(2010, 11, 1, 0, 30))
     >>> list(rrule.rrulestr(recrule, dtstart=start, forceset=True))
     [datetime.datetime(2010, 11, 2, 0, 30, tzinfo=<DstTzInfo 'Europe/Vienna' CET+1:00:00 STD>),
         datetime.datetime(2010, 11, 3, 0, 30, tzinfo=<DstTzInfo 'Europe/Vienna' CET+1:00:00 STD>)]
 
 But if we start from 30th October, where UTC+2 offset is still active, the
-sequence has incorrect timezones and substracting does not work as expected
+sequence has incorrect timezones and subtracting does not work as expected
 anymore.
 
 ::
 
     >>> start = at.localize(datetime(2010,10,30,0,30))
     >>> list(rrule.rrulestr(recrule, dtstart=start, forceset=True))
     [datetime.datetime(2010, 10, 30, 0, 30, tzinfo=<DstTzInfo 'Europe/Vienna' CEST+2:00:00 DST>),
```

### Comparing `plone.event-1.4.2/plone/event/utils.rst` & `plone.event-2.0.0/plone/event/utils.rst`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 boundaries and has to be normalized - see below.
 
 Normalizing it with DSTADJUST should correct the UTC offset and adjusting the
 time in a way, that it's value will be the same as before normalizing.
     >>> utcoffset_normalize(date2, dstmode=DSTADJUST)
     datetime.datetime(2010, 11, 10, 0, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CET+1:00:00 STD>)
 
-With DSTKEEP, normalizing will also keep the time as originaly set by UTC
+With DSTKEEP, normalizing will also keep the time as originally set by UTC
 offset - time's value will change.
     >>> utcoffset_normalize(date2, dstmode=DSTKEEP)
     datetime.datetime(2010, 11, 9, 23, 0, tzinfo=<DstTzInfo 'Europe/Vienna' CET+1:00:00 STD>)
 
 This should have explained the difference between DSTADJUST and DSTKEEP.
 Please note, that the naming of those two daylight saving time modes are a bit
 confusing. DSTKEEP will keep the time as set by UTC offset, so it's value will
```

### Comparing `plone.event-1.4.2/plone/event/adapters.py` & `plone.event-2.0.0/plone/event/adapters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# -*- coding: utf-8 -*-
 from plone.event.interfaces import IEvent
 from plone.event.interfaces import IEventAccessor
 from zope.component import adapter
 from zope.interface import implementer
 
 
 @implementer(IEventAccessor)
 @adapter(IEvent)
-class EventAccessor(object):
+class EventAccessor:
     """Simple event accessor adapter implementation for generic events, which
     follow the IEvent interface closely.
 
     Concrete implementations adapt a content type to the IEvent specification.
     """
 
     def __init__(self, context):
-        object.__setattr__(self, 'context', context)
+        object.__setattr__(self, "context", context)
 
     def __getattr__(self, name):
         return getattr(self.context, name)
 
     def __setattr__(self, name, value):
         setattr(self.context, name, value)
```

### Comparing `plone.event-1.4.2/CHANGES.rst` & `plone.event-2.0.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.0 (2023-04-19)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7 compatibility.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5cc689e5)
+
+
 1.4.2 (2023-01-24)
 ------------------
 
 Bug fixes:
 
 
 - Fix AttributeError: 'NoneType' object has no attribute 'astimezone'.
@@ -104,18 +121,18 @@
   [maurits]
 
 
 1.1 (2014-02-11)
 ----------------
 
 - Fix tests, where they broke with unicode recurrence strings and unicode date
-  formating strings.
+  formatting strings.
   [thet]
 
-- Make rrule munging hack only apply to RDATEs, EXDATEs and UNTILs which have
+- Make rrule munging hack only apply to `RDATE`, `EXDATE` and `UNTIL` which have
   null times, otherwise the DateRecurrenceIndex is broken for those who are
   generating RRULES using a non-broken widget. This will still result in broken
   RRULEs for some edge cases (where an RDATE is explicitly set for midnight on
   a RRULE with a DTSTART which is not), but that's better than breaking valid
   RRULES which are not generated improperly.
   This code should go into the broken widget itself or its DataManager/Field.
   [alecpm]
```

