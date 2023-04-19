# Comparing `tmp/plone.indexer-1.0rc2.tar.gz` & `tmp/plone.indexer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.indexer-1.0rc2.tar", last modified: Sun Apr  5 10:16:07 2009, max compression, from Unix
+gzip compressed data, was "plone.indexer-2.0.0.tar", last modified: Wed Apr 19 07:15:29 2023, max compression
```

## Comparing `plone.indexer-1.0rc2.tar` & `plone.indexer-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 optilude   (501) staff       (20)        0 2009-04-05 10:16:07.000000 plone.indexer-1.0rc2/
-drwxr-xr-x   0 optilude   (501) staff       (20)        0 2009-04-05 10:16:07.000000 plone.indexer-1.0rc2/docs/
--rw-r--r--   0 optilude   (501) staff       (20)      674 2009-04-05 10:12:37.000000 plone.indexer-1.0rc2/docs/HISTORY.txt
--rw-r--r--   0 optilude   (501) staff       (20)     1244 2009-04-05 10:03:21.000000 plone.indexer-1.0rc2/docs/INSTALL.txt
--rw-r--r--   0 optilude   (501) staff       (20)    15712 2009-04-05 10:16:07.000000 plone.indexer-1.0rc2/PKG-INFO
-drwxr-xr-x   0 optilude   (501) staff       (20)        0 2009-04-05 10:16:07.000000 plone.indexer-1.0rc2/plone/
--rw-r--r--   0 optilude   (501) staff       (20)      244 2009-04-05 10:03:21.000000 plone.indexer-1.0rc2/plone/__init__.py
-drwxr-xr-x   0 optilude   (501) staff       (20)        0 2009-04-05 10:16:07.000000 plone.indexer-1.0rc2/plone/indexer/
--rw-r--r--   0 optilude   (501) staff       (20)       43 2009-04-05 10:03:21.000000 plone.indexer-1.0rc2/plone/indexer/__init__.py
--rw-r--r--   0 optilude   (501) staff       (20)      152 2009-04-05 10:03:21.000000 plone.indexer-1.0rc2/plone/indexer/configure.zcml
--rw-r--r--   0 optilude   (501) staff       (20)     1608 2009-04-05 10:03:21.000000 plone.indexer-1.0rc2/plone/indexer/decorator.py
--rw-r--r--   0 optilude   (501) staff       (20)      903 2009-04-05 10:03:21.000000 plone.indexer-1.0rc2/plone/indexer/delegate.py
--rw-r--r--   0 optilude   (501) staff       (20)     1874 2009-04-05 10:13:12.000000 plone.indexer-1.0rc2/plone/indexer/interfaces.py
--rw-r--r--   0 optilude   (501) staff       (20)    12400 2009-04-05 10:12:40.000000 plone.indexer-1.0rc2/plone/indexer/README.txt
--rw-r--r--   0 optilude   (501) staff       (20)      369 2009-04-05 10:03:21.000000 plone.indexer-1.0rc2/plone/indexer/tests.py
--rw-r--r--   0 optilude   (501) staff       (20)     2382 2009-04-05 10:12:25.000000 plone.indexer-1.0rc2/plone/indexer/wrapper.py
-drwxr-xr-x   0 optilude   (501) staff       (20)        0 2009-04-05 10:16:07.000000 plone.indexer-1.0rc2/plone.indexer.egg-info/
--rw-r--r--   0 optilude   (501) staff       (20)        1 2009-04-05 10:16:07.000000 plone.indexer-1.0rc2/plone.indexer.egg-info/dependency_links.txt
--rw-r--r--   0 optilude   (501) staff       (20)        7 2009-04-05 10:16:07.000000 plone.indexer-1.0rc2/plone.indexer.egg-info/entry_points.txt
--rw-r--r--   0 optilude   (501) staff       (20)        6 2009-04-05 10:16:07.000000 plone.indexer-1.0rc2/plone.indexer.egg-info/namespace_packages.txt
--rw-r--r--   0 optilude   (501) staff       (20)        1 2009-04-05 10:03:37.000000 plone.indexer-1.0rc2/plone.indexer.egg-info/not-zip-safe
--rw-r--r--   0 optilude   (501) staff       (20)    15712 2009-04-05 10:16:07.000000 plone.indexer-1.0rc2/plone.indexer.egg-info/PKG-INFO
--rw-r--r--   0 optilude   (501) staff       (20)       57 2009-04-05 10:16:07.000000 plone.indexer-1.0rc2/plone.indexer.egg-info/requires.txt
--rw-r--r--   0 optilude   (501) staff       (20)      575 2009-04-05 10:16:07.000000 plone.indexer-1.0rc2/plone.indexer.egg-info/SOURCES.txt
--rw-r--r--   0 optilude   (501) staff       (20)        6 2009-04-05 10:16:07.000000 plone.indexer-1.0rc2/plone.indexer.egg-info/top_level.txt
--rw-r--r--   0 optilude   (501) staff       (20)       59 2009-04-05 10:16:07.000000 plone.indexer-1.0rc2/setup.cfg
--rw-r--r--   0 optilude   (501) staff       (20)     1171 2009-04-05 10:15:59.000000 plone.indexer-1.0rc2/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:15:29.332512 plone.indexer-2.0.0/
+-rw-r--r--   0 gil       (1000) gil       (1000)     2688 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      149 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    16131 2023-04-19 07:15:29.332512 plone.indexer-2.0.0/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      308 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:15:29.330512 plone.indexer-2.0.0/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1495 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/docs/LICENSE.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:15:29.331512 plone.indexer-2.0.0/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:15:29.332512 plone.indexer-2.0.0/plone/indexer/
+-rw-r--r--   0 gil       (1000) gil       (1000)    12200 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/plone/indexer/README.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       52 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/plone/indexer/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      142 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/plone/indexer/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1753 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/plone/indexer/decorator.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      975 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/plone/indexer/delegate.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1843 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/plone/indexer/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      949 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/plone/indexer/tests.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3254 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/plone/indexer/wrapper.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:15:29.331512 plone.indexer-2.0.0/plone.indexer.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    16131 2023-04-19 07:15:29.000000 plone.indexer-2.0.0/plone.indexer.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      595 2023-04-19 07:15:29.000000 plone.indexer-2.0.0/plone.indexer.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-19 07:15:29.000000 plone.indexer-2.0.0/plone.indexer.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-19 07:15:29.000000 plone.indexer-2.0.0/plone.indexer.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-19 07:15:29.000000 plone.indexer-2.0.0/plone.indexer.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)       28 2023-04-19 07:15:29.000000 plone.indexer-2.0.0/plone.indexer.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-19 07:15:29.000000 plone.indexer-2.0.0/plone.indexer.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2864 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-19 07:15:29.333512 plone.indexer-2.0.0/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1534 2023-04-19 07:15:28.000000 plone.indexer-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plone.indexer-1.0rc2/PKG-INFO` & `plone.indexer-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,368 +1,475 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: plone.indexer
-Version: 1.0rc2
+Version: 2.0.0
 Summary: Hooks to facilitate managing custom index values in Zope 2/CMF applications
-Home-page: http://pypi.python.org/pypi/plone.indexer
-Author: Martin Aspeli
-Author-email: optilude@gmail.com
-License: LGPL
-Description: Introduction
-        ============
-        
-        This package provides primitives to help delegate ZCatalog indexing operations
-        to adapters. It doesn't do very much on its own, but can be used by catalog
-        implementations that want to allow individual index values to be provided
-        not by the object itself, but by separate adapters.
-        
-        Writing indexers
-        ================
-        
-        An indexer is a named adapter that adapts the type of an object and provides
-        a value to be indexed when the catalog attempts to index the attribute with
-        that name.
-        
-        For example, let's say we have two types, page and news item:
-        
-        >>> from zope.interface import implements, Interface
-        >>> from zope import schema
-        
-        >>> class IPage(Interface):
-        ...     text = schema.Text(title=u"Body text")
-        >>> class Page(object):
-        ...     implements(IPage)
-        ...     def __init__(self, text):
-        ...         self.text = text
-        
-        >>> class INewsItem(Interface):
-        ...     summary = schema.TextLine(title=u"Short summary")
-        ...     story = schema.Text(title=u"Body text")
-        ...     audience = schema.TextLine(title=u"Audience")
-        
-        >>> class NewsItem(object):
-        ...     implements(INewsItem)
-        ...     def __init__(self, summary, story, audience):
-        ...         self.summary = summary
-        ...         self.story = story
-        ...         self.audience = audience
-        
-        Now, pretend that our catalog had an index 'description', which for a page
-        should contain the first 10 characters from the body text, and for a news
-        item should contain the contents of the 'summary' field. Furthermore, there
-        is an index 'audience' that should contain the value of the corresponding
-        field for news items, in all uppercase. It should do nothing for pages.
-        
-        We could write indexers for all of these like this
-        
-        >>> from plone.indexer import indexer
-        
-        >>> @indexer(IPage)
-        ... def page_description(object):
-        ...     return object.text[:10]
-        
-        >>> @indexer(INewsItem)
-        ... def newsitem_description(object):
-        ...     return object.summary
-        
-        >>> @indexer(INewsItem)
-        ... def newsitem_audience(object):
-        ...     return object.audience.upper()
-        
-        These need to be registered as named adapters, where the name corresponds to
-        the index name. In ZCML, that may be::
-        
-        <adapter name="description" factory=".indexers.page_description" />
-        <adapter name="description" factory=".indexers.newsitem_description" />
-        <adapter name="audience" factory=".indexers.newsitem_audience" />
-        
-        We can omit the 'for' attribute because we passed this to the @indexer
-        decorator, and we can omit the 'provides' attribute because the thing
-        returned by the decorator is actually a class providing the required IIndexer
-        interface.
-        
-        For the purposes of the ensuing tests, we'll register these directly.
-        
-        >>> from zope.component import provideAdapter
-        >>> provideAdapter(page_description, name='description')
-        >>> provideAdapter(newsitem_description, name='description')
-        >>> provideAdapter(newsitem_audience, name='audience')
-        
-        Testing your indexers (or calling them directly)
-        ------------------------------------------------
-        
-        If you are writing tests for your indexers (as you should!), then you should
-        be aware of the following:
-        
-        When the @indexer decorator returns, it turns your function into an instance
-        of type DelegatingIndexerFactory. This is an adapter factory that can create
-        a DelegatingIndexer, which in turn will call your function when asked to
-        perform indexing operations.
-        
-        This means that you can't just call your function to test the indexer.
-        Instead, you need to instantiate the adapter and then call the delegating
-        indexer with the portal root as the first argument. For example:
-        
-        >>> test_page = Page(text=u"My page with some text")
-        >>> page_description(test_page)()
-        u'My page wi'
-        
-        This will suffice in most cases. Note that there is actually a second
-        parameter, catalog, which defaults to None. If you need to write an indexer
-        that acts on catalog, you'll need to register a conventional adapter, as
-        described in the next section.
-        
-        Other means of registering indexers
-        -----------------------------------
-        
-        At the end of the day, an indexer is just a named multi-adapter from the
-        indexable object (e.g. INewsItem or IPage above) and the catalog (usually
-        portal_catalog in a CMF application) to IIndexer, where the name is the name
-        of the indexed attribute in the catalog. Thus, you could register your
-        indexers as more conventional adapters:
-        
-        >>> from plone.indexer.interfaces import IIndexer
-        >>> from Products.ZCatalog.interfaces import IZCatalog
-        
-        >>> from zope.interface import implements
-        >>> from zope.component import adapts
-        >>> class LengthIndexer(object):
-        ...     """Index the length of the body text
-        ...     """
-        ...     implements(IIndexer)
-        ...     adapts(IPage, IZCatalog)
-        ...
-        ...     def __init__(self, context, catalog):
-        ...         self.context = context
-        ...         self.catalog = catalog
-        ...
-        ...     def __call__(self):
-        ...         return len(self.context.text)
-        
-        We normally just use IZCatalog for the catalog adaptation, to apply to any
-        catalog. However, if you want different indexers for different types of
-        catalogs, there is an example later in this test.
-        
-        You'd register this with ZCML like so::
-        
-        <adapter factory=".indexers.LengthIndexer" name="length" />
-        
-        Or in a test:
-        
-        >>> provideAdapter(LengthIndexer, name="length")
-        
-        If you're only curious about how to write indexers, you can probably stop
-        here. If you want to know more about how they work and how they are wired into
-        a framework, read on.
-        
-        Hooking up indexers to the framework
-        =====================================
-        
-        Here is a mock implementation of a ZCatalog.catalog_object() override, based
-        on the one in Plone. We'll use this for testing. We won't bother with the full
-        ZCatalog interface, only catalog_object(), and we'll stub out a few things.
-        This really is for illustration purposes only, to show the intended usage
-        pattern.
-        
-        In CMF 2.2, there is an IIndexableObject marker interface defined in
-        Products.CMFCore.interfaces. We have a compatibility alias in this package
-        for use with CMF 2.1.
-        
-        >>> from Products.ZCatalog.interfaces import IZCatalog
-        >>> from plone.indexer.interfaces import IIndexableObject
-        >>> from zope.component import queryMultiAdapter
-        
-        >>> class FauxCatalog(object):
-        ...     implements(IZCatalog)
-        ...
-        ...     def catalog_object(self, object, uid, idxs=[]):
-        ...         """Pretend to index 'object' under the key 'uid'. We'll
-        ...         print the results of the indexing operation to the screen .
-        ...         """
-        ...
-        ...         if not IIndexableObject.providedBy(object):
-        ...             wrapper = queryMultiAdapter((object, self,), IIndexableObject)
-        ...             if wrapper is not None:
-        ...                 object = wrapper
-        ...
-        ...         # Perform the actual indexing of attributes in the idxs list
-        ...         for idx in idxs:
-        ...             try:
-        ...                 indexed_value = getattr(object, idx)
-        ...                 if callable(indexed_value):
-        ...                     indexed_value = indexed_value()
-        ...                 print idx, "=", indexed_value
-        ...             except (AttributeError, TypeError,):
-        ...                 pass
-        
-        The important things here are:
-        
-        - We attempt to obtain an IIndexableObject for the object to be indexed.
-        This is just a way to get hold of an implementation of this interface
-        (we'll register one in a moment) and allow some coarse-grained overrides.
-        
-        - Cataloging involves looking up attributes on the indexable object
-        wrapper matching the names of indexes (in the real ZCatalog, this is
-        actually decoupled, but let's not get carried away). If they are
-        callable, they should be called. This is just mimicking what ZCatalog's
-        implementation does.
-        
-        This package comes with an implementation of an IIndexableObject adapter that
-        knows how to delegate to an IIndexer. Let's now register that as the default
-        IIndexableObject wrapper adapter so that the code above will find it.
-        
-        >>> from plone.indexer.wrapper import IndexableObjectWrapper
-        >>> from plone.indexer.interfaces import IIndexableObject
-        >>> provideAdapter(factory=IndexableObjectWrapper, adapts=(Interface, IZCatalog,), provides=IIndexableObject)
-        
-        Seeing it in action
-        ===================
-        
-        Now for the testing. First, we need a faux catalog:
-        
-        >>> catalog = FauxCatalog()
-        
-        Finally, let's create some objects to index.
-        
-        >>> page = Page(u"The page body text here")
-        >>> news = NewsItem(u"News summary", u"News body text", u"Audience")
-        
-        First of all, let's demonstrate that our indexers work and apply only to
-        the types for which they are registered.
-        
-        >>> catalog.catalog_object(page, 'p1', idxs=['description', 'audience', 'length'])
-        description = The page b
-        length = 23
-        
-        >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
-        description = News summary
-        audience = AUDIENCE
-        
-        Our custom indexable object wrapper is capable of looking up workflow
-        variables if the portal_workflow tool is available. For testing purposes,
-        we'll create a fake minimal workflow tool and stash it onto the fake catalog
-        so that it can be found by getToolByName. In real life, it would of course be
-        acquirable as normal.
-        
-        >>> class FauxWorkflowTool(object):
-        ...     def getCatalogVariablesFor(self, object):
-        ...         return dict(review_state='published', audience='Somebody')
-        >>> catalog.portal_workflow = FauxWorkflowTool()
-        
-        If we now index 'review_state', it will be obtained from the workflow
-        variables. However, a custom indexer still overrides workflow variables.
-        
-        >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'review_state'])
-        description = News summary
-        audience = AUDIENCE
-        review_state = published
-        
-        Finally, if not adapter can be found, we fall back on getattr() on the object.
-        
-        >>> catalog.catalog_object(page, 'p3', idxs=['description', 'text'])
-        description = The page b
-        text = The page body text here
-        
-        Customising indexers based on the catalog type
-        ==============================================
-        
-        It is possible to provide a custom indexer for a different type of catalog.
-        To test that, let's create a secondary catalog and mark it with a marker
-        interface.
-        
-        >>> from zope.interface import Interface
-        >>> class IAlternateCatalog(Interface):
-        ...     pass
-        >>> from zope.interface import alsoProvides
-        >>> catalog2 = FauxCatalog()
-        >>> alsoProvides(catalog2, IAlternateCatalog)
-        
-        Let's say that we did not want the news item audience uppercased here. We
-        could provide a custom indexer for just this catalog:
-        
-        >>> @indexer(INewsItem, IAlternateCatalog)
-        ... def alternate_newsitem_audience(object):
-        ...     return object.audience.lower()
-        >>> provideAdapter(alternate_newsitem_audience, name='audience')
-        
-        This does not affect the first catalog:
-        
-        >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
-        description = News summary
-        audience = AUDIENCE
-        
-        However, the second catalog gets the audience in lowercase.
-        
-        >>> catalog2.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
-        description = News summary
-        audience = audience
-        
-        Interfaces provided by the wrapper
-        ==================================
-        
-        The indexable object wrapper has one particular feature: instances of the
-        wrapper will provide the same interfaces as instances of the wrapped object.
-        For example:
-        
-        >>> from plone.indexer.interfaces import IIndexableObjectWrapper, IIndexableObject
-        >>> wrapper = IndexableObjectWrapper(page, catalog)
-        >>> IIndexableObjectWrapper.providedBy(wrapper)
-        True
-        >>> IIndexableObject.providedBy(wrapper)
-        True
-        >>> IPage.providedBy(wrapper)
-        True
-        >>> INewsItem.providedBy(wrapper)
-        False
-        
-        >>> wrapper = IndexableObjectWrapper(news, catalog)
-        >>> IIndexableObjectWrapper.providedBy(wrapper)
-        True
-        >>> IPage.providedBy(wrapper)
-        False
-        >>> INewsItem.providedBy(wrapper)
-        True
-        
-        Unboxing
-        ========
-        
-        It is possible to obtain the wrapped object from the wrapper:
-        
-        >>> wrapper = IndexableObjectWrapper(page, catalog)
-        >>> wrapper._getWrappedObject() is page
-        True
-        
-        
-        Changelog
-        =========
-        
-        1.0rc2 - unreleased
-        ------------------
-        
-        * Added _getWrappedObject() method to get hold of the underlying object.
-        Note that this means you can't have an index/metadata column with this name.
-        [optilude]
-        
-        * Corrected IZCatalog import location to point to the interfaces module.
-        [hannosch]
-        
-        
-        1.0rc1 - 2009-03-26
-        ------------------
-        
-        * Updated the interface to match the developments of similar functionality
-        on CMF trunk. This means that indexers are now multi-adapters on
-        (object, catalog), and the keyword arguments (including the implicit
-        'portal' parameter) are gone.
-        [optilude]
-        
-        
-        1.0a1 - 2009-03-05
-        ------------------
-        
-        * Initial release
-        
-        
+Home-page: https://pypi.org/project/plone.indexer
+Author: Plone Foundation
+Author-email: plone-developers@lists.sourceforge.net
+License: BSD
 Keywords: plone cmf zope catalog index
-Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
+Classifier: Framework :: Plone :: 6.0
+Classifier: Framework :: Plone :: Core
+Classifier: Framework :: Zope :: 5
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+
+Introduction
+============
+
+This package provides primitives to help delegate ZCatalog indexing operations
+to adapters. It doesn't do very much on its own, but can be used by catalog
+implementations that want to allow individual index values to be provided
+not by the object itself, but by separate adapters.
+
+
+Changelog
+=========
+
+.. You should *NOT* be adding new change log entries to this file.
+   You should create a file in the news directory instead.
+   For helpful instructions, please see:
+   https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
+
+.. towncrier release notes start
+
+2.0.0 (2023-04-19)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7 support.
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
+1.0.7 (2020-04-20)
+------------------
+
+Bug fixes:
+
+
+- Minor packaging updates. (#1)
+
+
+1.0.6 (2019-04-29)
+------------------
+
+Bug fixes:
+
+
+- Fixed: doctests on Python 2 were not correctly checked.  [maurits] (#7)
+
+
+1.0.5 (2018-09-26)
+------------------
+
+Fixes:
+
+- fix https://github.com/plone/Products.CMFPlone/issues/2469:
+  "Subobjects are indexing attributes of parent".
+  Allow only direct attributes and acquired PythonScripts,
+  but not acquired attributes.
+  Indexers and PythonScripts are able to handle this explicitly,
+  because they get the acquisition-wrapped object.
+  [jensens]
+
+- Fix tests to work in Python 3
+  [pbauer]
+
+
+1.0.4 (2016-02-25)
+------------------
+
+Fixes:
+
+- Replace deprecated ``zope.testing.doctestunit`` import with ``doctest``
+  module from stdlib.
+  [thet]
+
+- Reformat according to the Plone styleguide.
+  [thet]
+
+
+1.0.3 (2015-05-05)
+------------------
+
+- Add missing dependency on Products.ZCatalog.
+  [gforcada]
+
+
+1.0.2 (2013-01-13)
+------------------
+
+- Changed the @indexer decorator to maintain the information about the wrapped
+  function (__doc__, __module__, __name__, etc).
+  [dokai]
+
+
+1.0.1 (2012-12-14)
+------------------
+
+- Relicense under modified BSD license; per Plone Foundation board
+  approval on 2012-05-31.
+  See: http://plone.org/foundation/materials/foundation-resolutions/plone-framework-components-relicensing-policy
+  [supton]
+
+- Add MANIFEST.in.
+  [WouterVH]
+
+
+1.0 - 2010-07-18
+----------------
+
+- Fixed reSt markup in the changelog.
+  [hannosch]
+
+- Update license to GPL version 2 only.
+  [hannosch]
+
+
+1.0rc2 - 2009-04-05
+-------------------
+
+- Added _getWrappedObject() method to get hold of the underlying object.
+  Note that this means you can't have an index/metadata column with this name.
+  [optilude]
+
+- Corrected IZCatalog import location to point to the interfaces module.
+  [hannosch]
+
+
+1.0rc1 - 2009-03-26
+-------------------
+
+- Updated the interface to match the developments of similar functionality
+  on CMF trunk. This means that indexers are now multi-adapters on
+  (object, catalog), and the keyword arguments (including the implicit
+  'portal' parameter) are gone.
+  [optilude]
+
+
+1.0a1 - 2009-03-05
+------------------
+
+- Initial release
+
+
+Writing indexers
+================
+
+An indexer is a named adapter that adapts the type of an object and provides a value to be indexed when the catalog attempts to index the attribute with that name.
+
+For example, let's say we have two types, page and news item::
+
+    >>> from zope.interface import Interface
+    >>> from zope.interface import implementer
+    >>> from zope import schema
+
+    >>> class IPage(Interface):
+    ...     text = schema.Text(title=u"Body text")
+
+    >>> @implementer(IPage)
+    ... class Page(object):
+    ...     def __init__(self, text):
+    ...         self.text = text
+
+    >>> class INewsItem(Interface):
+    ...     summary = schema.TextLine(title=u"Short summary")
+    ...     story = schema.Text(title=u"Body text")
+    ...     audience = schema.TextLine(title=u"Audience")
+
+    >>> @implementer(INewsItem)
+    ... class NewsItem(object):
+    ...     def __init__(self, summary, story, audience):
+    ...         self.summary = summary
+    ...         self.story = story
+    ...         self.audience = audience
+
+Now, pretend that our catalog had an index 'description', which for a page should contain the first 10 characters from the body text, and for a news item should contain the contents of the 'summary' field.
+Furthermore, there is an index 'audience' that should contain the value of the corresponding field for news items, in all uppercase.
+It should do nothing for pages.
+
+We could write indexers for all of these like this::
+
+    >>> from plone.indexer import indexer
+
+    >>> @indexer(IPage)
+    ... def page_description(object):
+    ...     return object.text[:10]
+
+    >>> @indexer(INewsItem)
+    ... def newsitem_description(object):
+    ...     return object.summary
+
+    >>> @indexer(INewsItem)
+    ... def newsitem_audience(object):
+    ...     return object.audience.upper()
+
+These need to be registered as named adapters, where the name corresponds to the index name.
+In ZCML, that may be::
+
+    <adapter name="description" factory=".indexers.page_description" />
+    <adapter name="description" factory=".indexers.newsitem_description" />
+    <adapter name="audience" factory=".indexers.newsitem_audience" />
+
+We can omit the 'for' attribute because we passed this to the @indexer decorator, and we can omit the 'provides' attribute because the thing returned by the decorator is actually a class providing the required IIndexer interface.
+
+For the purposes of the ensuing tests, we'll register these directly::
+
+    >>> from zope.component import provideAdapter
+    >>> provideAdapter(page_description, name='description')
+    >>> provideAdapter(newsitem_description, name='description')
+    >>> provideAdapter(newsitem_audience, name='audience')
+
+
+Testing your indexers (or calling them directly)
+------------------------------------------------
+
+If you are writing tests for your indexers (as you should!), then you should be aware of the following:
+
+When the @indexer decorator returns, it turns your function into an instance of type DelegatingIndexerFactory.
+This is an adapter factory that can create a DelegatingIndexer, which in turn will call your function when asked to perform indexing operations.
+
+This means that you can't just call your function to test the indexer.
+Instead, you need to instantiate the adapter and then call the delegating indexer with the portal root as the first argument.
+For example::
+
+    >>> test_page = Page(text=u"My page with some text")
+    >>> page_description(test_page)()
+    'My page wi'
+
+This will suffice in most cases.
+Note that there is actually a second parameter, catalog, which defaults to None.
+If you need to write an indexer that acts on catalog, you'll need to register a conventional adapter, as described in the next section.
+
+
+Other means of registering indexers
+-----------------------------------
+
+At the end of the day, an indexer is just a named multi-adapter from the indexable object (e.g.
+INewsItem or IPage above) and the catalog (usually portal_catalog in a CMF application) to IIndexer, where the name is the name of the indexed attribute in the catalog.
+Thus, you could register your indexers as more conventional adapters::
+
+    >>> from plone.indexer.interfaces import IIndexer
+    >>> from Products.ZCatalog.interfaces import IZCatalog
+    >>> from zope.component import adapter
+    >>> from zope.interface import implementer
+
+    >>> @implementer(IIndexer)
+    ... @adapter(IPage, IZCatalog)
+    ... class LengthIndexer(object):
+    ...     """Index the length of the body text
+    ...     """
+    ...     def __init__(self, context, catalog):
+    ...         self.context = context
+    ...         self.catalog = catalog
+    ...
+    ...     def __call__(self):
+    ...         return len(self.context.text)
+
+We normally just use IZCatalog for the catalog adaptation, to apply to any catalog.
+However, if you want different indexers for different types of catalogs, there is an example later in this test.
+
+You'd register this with ZCML like so::
+
+    <adapter factory=".indexers.LengthIndexer" name="length" />
+
+Or in a test::
+
+    >>> provideAdapter(LengthIndexer, name="length")
+
+If you're only curious about how to write indexers, you can probably stop here.
+If you want to know more about how they work and how they are wired into a framework, read on.
+
+
+Hooking up indexers to the framework
+=====================================
+
+Here is a mock implementation of a ZCatalog.catalog_object() override, based on the one in Plone.
+We'll use this for testing.
+We won't bother with the full ZCatalog interface, only catalog_object(), and we'll stub out a few things.
+This really is for illustration purposes only, to show the intended usage pattern.
+
+In CMF 2.2, there is an IIndexableObject marker interface defined in Products.CMFCore.interfaces.
+We have a compatibility alias in this package for use with CMF 2.1.
+
+::
+
+    >>> from OFS.interfaces import IItem
+    >>> from plone.indexer.interfaces import IIndexableObject
+    >>> from Products.ZCatalog.interfaces import IZCatalog
+    >>> from zope.component import queryMultiAdapter
+
+    >>> @implementer(IZCatalog, IItem)
+    ... class FauxCatalog(object):
+    ...
+    ...     def catalog_object(self, object, uid, idxs=[]):
+    ...         """Pretend to index 'object' under the key 'uid'. We'll
+    ...         print the results of the indexing operation to the screen .
+    ...         """
+    ...
+    ...         if not IIndexableObject.providedBy(object):
+    ...             wrapper = queryMultiAdapter((object, self,), IIndexableObject)
+    ...             if wrapper is not None:
+    ...                 object = wrapper
+    ...
+    ...         # Perform the actual indexing of attributes in the idxs list
+    ...         for idx in idxs:
+    ...             try:
+    ...                 indexed_value = getattr(object, idx)
+    ...                 if callable(indexed_value):
+    ...                     indexed_value = indexed_value()
+    ...                 print("{0} = {1}".format(idx, indexed_value))
+    ...             except (AttributeError, TypeError,):
+    ...                 pass
+
+The important things here are:
+
+    - We attempt to obtain an IIndexableObject for the object to be indexed.
+      This is just a way to get hold of an implementation of this interface (we'll register one in a moment) and allow some coarse-grained overrides.
+
+    - Cataloging involves looking up attributes on the indexable object wrapper matching the names of indexes (in the real ZCatalog, this is actually decoupled, but let's not get carried away).
+      If they are callable, they should be called.
+      This is just mimicking what ZCatalog's implementation does.
+
+This package comes with an implementation of an IIndexableObject adapter that knows how to delegate to an IIndexer.
+Let's now register that as the default IIndexableObject wrapper adapter so that the code above will find it::
+
+    >>> from plone.indexer.interfaces import IIndexableObject
+    >>> from plone.indexer.wrapper import IndexableObjectWrapper
+    >>> provideAdapter(factory=IndexableObjectWrapper, adapts=(Interface, IZCatalog,), provides=IIndexableObject)
+
+Seeing it in action
+===================
+
+Now for the testing. First, we need a faux catalog::
+
+    >>> catalog = FauxCatalog()
+
+Finally, let's create some objects to index::
+
+    >>> page = Page(u"The page body text here")
+    >>> news = NewsItem(u"News summary", u"News body text", u"Audience")
+
+First of all, let's demonstrate that our indexers work and apply only to the types for which they are registered::
+
+    >>> catalog.catalog_object(page, 'p1', idxs=['description', 'audience', 'length'])
+    description = The page b
+    length = 23
+
+    >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
+    description = News summary
+    audience = AUDIENCE
+
+Our custom indexable object wrapper is capable of looking up workflow variables if the portal_workflow tool is available.
+For testing purposes, we'll create a fake minimal workflow tool and stash it onto the fake catalog so that it can be found by getToolByName.
+In real life, it would of course be acquirable as normal::
+
+    >>> @implementer(IItem)
+    ... class FauxWorkflowTool(object):
+    ...     def getCatalogVariablesFor(self, object):
+    ...         return dict(review_state='published', audience='Somebody')
+    >>> catalog.portal_workflow = FauxWorkflowTool()
+
+If we now index 'review_state', it will be obtained from the workflow variables.
+However, a custom indexer still overrides workflow variables::
+
+    >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'review_state'])
+    description = News summary
+    audience = AUDIENCE
+    review_state = published
+
+Finally, if not adapter can be found, we fall back on getattr() on the object::
+
+    >>> catalog.catalog_object(page, 'p3', idxs=['description', 'text'])
+    description = The page b
+    text = The page body text here
+
+
+Customising indexers based on the catalog type
+==============================================
+
+It is possible to provide a custom indexer for a different type of catalog.
+To test that, let's create a secondary catalog and mark it with a marker interface::
+
+    >>> from zope.interface import Interface
+    >>> class IAlternateCatalog(Interface):
+    ...     pass
+    >>> from zope.interface import alsoProvides
+    >>> catalog2 = FauxCatalog()
+    >>> alsoProvides(catalog2, IAlternateCatalog)
+
+Let's say that we did not want the news item audience uppercased here.
+We could provide a custom indexer for just this catalog::
+
+    >>> @indexer(INewsItem, IAlternateCatalog)
+    ... def alternate_newsitem_audience(object):
+    ...     return object.audience.lower()
+    >>> provideAdapter(alternate_newsitem_audience, name='audience')
+
+This does not affect the first catalog::
+
+    >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
+    description = News summary
+    audience = AUDIENCE
+
+However, the second catalog gets the audience in lowercase::
+
+    >>> catalog2.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
+    description = News summary
+    audience = audience
+
+
+Interfaces provided by the wrapper
+==================================
+
+The indexable object wrapper has one particular feature: instances of the wrapper will provide the same interfaces as instances of the wrapped object.
+For example::
+
+    >>> from plone.indexer.interfaces import IIndexableObject
+    >>> from plone.indexer.interfaces import IIndexableObjectWrapper
+
+    >>> wrapper = IndexableObjectWrapper(page, catalog)
+    >>> IIndexableObjectWrapper.providedBy(wrapper)
+    True
+    >>> IIndexableObject.providedBy(wrapper)
+    True
+    >>> IPage.providedBy(wrapper)
+    True
+    >>> INewsItem.providedBy(wrapper)
+    False
+
+    >>> wrapper = IndexableObjectWrapper(news, catalog)
+    >>> IIndexableObjectWrapper.providedBy(wrapper)
+    True
+    >>> IPage.providedBy(wrapper)
+    False
+    >>> INewsItem.providedBy(wrapper)
+    True
+
+
+Unboxing
+========
+
+It is possible to obtain the wrapped object from the wrapper::
+
+    >>> wrapper = IndexableObjectWrapper(page, catalog)
+    >>> wrapper._getWrappedObject() is page
+    True
+
```

### Comparing `plone.indexer-1.0rc2/plone/indexer/decorator.py` & `plone.indexer-2.0.0/plone/indexer/decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,51 @@
-"""This module defines a decorator that 
+"""This module defines a decorator that
 """
 
-from zope.component import adapter
 from plone.indexer.delegate import DelegatingIndexerFactory
 from Products.ZCatalog.interfaces import IZCatalog
+from zope.component import adapter
+
 
 class indexer(adapter):
     """The @indexer decorator can be used like this:
 
+        >>> from zope.interface import Interface
         >>> from plone.indexer.decorator import indexer
+        >>> class IMyType(Interface): ...
+        >>> class IMyCatalog(Interface): ...
         >>> @indexer(IMyType)
         ... def some_attribute(object):
-        ...     return "some indexable value"
-    
+        ...     return 'some indexable value'
+
     Note that the @indexer decorator is a superset of the @adapter decorator
     from zope.component.
-    
+
     To register an indexer for a special type of catalog, use:
-    
+
         >>> from plone.indexer.decorator import indexer
         >>> @indexer(IMyType, IMyCatalog)
-        ... def some_attribute(object):
-        ...     return "some indexable value"
-    
+        ... def another_attribute(object):
+        ...     return 'some indexable value'
+
     The default is to register the indexer for all IZCatalog catalogs.
-    
+
     Once you've created an indexer, you can register the adapter in ZCML:
 
         <adapter factory=".myindexers.some_attribute" name="some_attribute" />
-    
+
     At this point, the indexable object wrapper will ensure that when
     some_attribute is indexed on an object providing IMyType
     """
 
     def __init__(self, *interfaces):
         if len(interfaces) == 1:
             interfaces += (IZCatalog,)
         elif len(interfaces) > 2:
-            raise ValueError(u"The @indexer decorator takes at most two interfaces as arguments")
+            raise ValueError(
+                "The @indexer decorator takes at most two interfaces as arguments.",
+            )
         adapter.__init__(self, *interfaces)
 
     def __call__(self, callable):
-        factory =  DelegatingIndexerFactory(callable)
+        factory = DelegatingIndexerFactory(callable)
         return adapter.__call__(self, factory)
```

### Comparing `plone.indexer-1.0rc2/plone/indexer/delegate.py` & `plone.indexer-2.0.0/plone/indexer/delegate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-from zope.interface import implements
-from zope.interface.declarations import Implements, implementedBy
+from functools import update_wrapper
 from plone.indexer.interfaces import IIndexer
+from zope.interface import implementer
+from zope.interface.declarations import implementedBy
+from zope.interface.declarations import Implements
+
+
+@implementer(IIndexer)
+class DelegatingIndexer:
+    """An indexer that delegates to a given callable"""
 
-class DelegatingIndexer(object):
-    """An indexer that delegates to a given callable
-    """
-    implements(IIndexer)
-    
     def __init__(self, context, catalog, callable):
         self.context = context
         self.catalog = catalog
         self.callable = callable
-        
+
     def __call__(self):
         return self.callable(self.context)
 
-class DelegatingIndexerFactory(object):
+
+class DelegatingIndexerFactory:
     """An adapter factory for an IIndexer that works by calling a
     DelegatingIndexer.
     """
-    
+
     def __init__(self, callable):
         self.callable = callable
         self.__implemented__ = Implements(implementedBy(DelegatingIndexer))
-        
+        update_wrapper(self, callable)
+
     def __call__(self, object, catalog=None):
-        return DelegatingIndexer(object, catalog, self.callable)
+        return DelegatingIndexer(object, catalog, self.callable)
```

### Comparing `plone.indexer-1.0rc2/plone/indexer/interfaces.py` & `plone.indexer-2.0.0/plone/indexer/interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 from zope.interface import Interface
 
+
 # NOTE: CMF 2.2 provides standard interfaces for indexing. We provide
 # compatibility aliases here for CMF 2.1
 
 try:
     from Products.CMFCore.interfaces import IIndexableObjectWrapper
 except ImportError:
+
     class IIndexableObjectWrapper(Interface):
         pass
+
+
 try:
     from Products.CMFCore.interfaces import IIndexableObject
 except ImportError:
+
     class IIndexableObject(Interface):
         """An object being indexed in the catalog. The indexable object
         wrapper will be looked up as a multi-adapter of (object, catalog)
         to this interface if the object being indexed in the catalog does
         not already provide this interface.
         """
 
+
 class IIndexer(Interface):
     """A component that can provide the value for an catalog index.
-    
+
     Register a named adapter from an indexable object type (e.g. a content
     object) and the catalog to this interface.
-    
+
     The name of the adapter should be the same as the name of the indexable
     attribute in the catalog.
-    
+
     See also decorator.py, for a simpler indexer based on a function
     decorator.
     """
-    
+
     def __call__(self):
-        """Return the value to index.
-        """
+        """Return the value to index."""
+
 
 class IDelegatingIndexableObjectWrapper(IIndexableObjectWrapper):
-    """An adapter of a (object, catalog) where object is to be indexed in 
+    """An adapter of a (object, catalog) where object is to be indexed in
     the catalog and catalog is the portal_catalog or similar ZCatalog instance.
 
     The catalog will call getattr() on the wrapper for each attribute to be
     indexed. The wrapper may either implement these directly (as methods
     taking no parameters) or implement __getattr__() appropriately.
     """
-    
+
     def _getWrappedObject():
         """Return the object that was wrapped.
-        
+
         This has a leading underscore to reduce the risk of clashing with
         an index or metadata column.
         """
```

### Comparing `plone.indexer-1.0rc2/plone/indexer/README.txt` & `plone.indexer-2.0.0/plone/indexer/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,304 +1,282 @@
-Introduction
-============
-
-This package provides primitives to help delegate ZCatalog indexing operations
-to adapters. It doesn't do very much on its own, but can be used by catalog
-implementations that want to allow individual index values to be provided
-not by the object itself, but by separate adapters.
-
 Writing indexers
 ================
 
-An indexer is a named adapter that adapts the type of an object and provides
-a value to be indexed when the catalog attempts to index the attribute with
-that name.
+An indexer is a named adapter that adapts the type of an object and provides a value to be indexed when the catalog attempts to index the attribute with that name.
 
-For example, let's say we have two types, page and news item:
+For example, let's say we have two types, page and news item::
 
-    >>> from zope.interface import implements, Interface
+    >>> from zope.interface import Interface
+    >>> from zope.interface import implementer
     >>> from zope import schema
 
     >>> class IPage(Interface):
     ...     text = schema.Text(title=u"Body text")
-    >>> class Page(object):
-    ...     implements(IPage)
+
+    >>> @implementer(IPage)
+    ... class Page(object):
     ...     def __init__(self, text):
     ...         self.text = text
 
     >>> class INewsItem(Interface):
     ...     summary = schema.TextLine(title=u"Short summary")
     ...     story = schema.Text(title=u"Body text")
     ...     audience = schema.TextLine(title=u"Audience")
 
-    >>> class NewsItem(object):
-    ...     implements(INewsItem)
+    >>> @implementer(INewsItem)
+    ... class NewsItem(object):
     ...     def __init__(self, summary, story, audience):
     ...         self.summary = summary
     ...         self.story = story
     ...         self.audience = audience
 
-Now, pretend that our catalog had an index 'description', which for a page
-should contain the first 10 characters from the body text, and for a news
-item should contain the contents of the 'summary' field. Furthermore, there
-is an index 'audience' that should contain the value of the corresponding
-field for news items, in all uppercase. It should do nothing for pages.
+Now, pretend that our catalog had an index 'description', which for a page should contain the first 10 characters from the body text, and for a news item should contain the contents of the 'summary' field.
+Furthermore, there is an index 'audience' that should contain the value of the corresponding field for news items, in all uppercase.
+It should do nothing for pages.
 
-We could write indexers for all of these like this
+We could write indexers for all of these like this::
 
     >>> from plone.indexer import indexer
-    
+
     >>> @indexer(IPage)
     ... def page_description(object):
     ...     return object.text[:10]
 
     >>> @indexer(INewsItem)
     ... def newsitem_description(object):
     ...     return object.summary
 
     >>> @indexer(INewsItem)
     ... def newsitem_audience(object):
     ...     return object.audience.upper()
 
-These need to be registered as named adapters, where the name corresponds to
-the index name. In ZCML, that may be::
+These need to be registered as named adapters, where the name corresponds to the index name.
+In ZCML, that may be::
 
     <adapter name="description" factory=".indexers.page_description" />
     <adapter name="description" factory=".indexers.newsitem_description" />
     <adapter name="audience" factory=".indexers.newsitem_audience" />
 
-We can omit the 'for' attribute because we passed this to the @indexer
-decorator, and we can omit the 'provides' attribute because the thing 
-returned by the decorator is actually a class providing the required IIndexer
-interface.
+We can omit the 'for' attribute because we passed this to the @indexer decorator, and we can omit the 'provides' attribute because the thing returned by the decorator is actually a class providing the required IIndexer interface.
 
-For the purposes of the ensuing tests, we'll register these directly.
+For the purposes of the ensuing tests, we'll register these directly::
 
     >>> from zope.component import provideAdapter
     >>> provideAdapter(page_description, name='description')
     >>> provideAdapter(newsitem_description, name='description')
     >>> provideAdapter(newsitem_audience, name='audience')
 
+
 Testing your indexers (or calling them directly)
 ------------------------------------------------
 
-If you are writing tests for your indexers (as you should!), then you should
-be aware of the following:
+If you are writing tests for your indexers (as you should!), then you should be aware of the following:
+
+When the @indexer decorator returns, it turns your function into an instance of type DelegatingIndexerFactory.
+This is an adapter factory that can create a DelegatingIndexer, which in turn will call your function when asked to perform indexing operations.
 
-When the @indexer decorator returns, it turns your function into an instance
-of type DelegatingIndexerFactory. This is an adapter factory that can create
-a DelegatingIndexer, which in turn will call your function when asked to
-perform indexing operations.
-   
 This means that you can't just call your function to test the indexer.
-Instead, you need to instantiate the adapter and then call the delegating
-indexer with the portal root as the first argument. For example:
- 
+Instead, you need to instantiate the adapter and then call the delegating indexer with the portal root as the first argument.
+For example::
+
     >>> test_page = Page(text=u"My page with some text")
     >>> page_description(test_page)()
-    u'My page wi'
+    'My page wi'
+
+This will suffice in most cases.
+Note that there is actually a second parameter, catalog, which defaults to None.
+If you need to write an indexer that acts on catalog, you'll need to register a conventional adapter, as described in the next section.
 
-This will suffice in most cases. Note that there is actually a second
-parameter, catalog, which defaults to None. If you need to write an indexer
-that acts on catalog, you'll need to register a conventional adapter, as
-described in the next section.
 
 Other means of registering indexers
 -----------------------------------
 
-At the end of the day, an indexer is just a named multi-adapter from the
-indexable object (e.g. INewsItem or IPage above) and the catalog (usually
-portal_catalog in a CMF application) to IIndexer, where the name is the name
-of the indexed attribute in the catalog. Thus, you could register your
-indexers as more conventional adapters:
+At the end of the day, an indexer is just a named multi-adapter from the indexable object (e.g.
+INewsItem or IPage above) and the catalog (usually portal_catalog in a CMF application) to IIndexer, where the name is the name of the indexed attribute in the catalog.
+Thus, you could register your indexers as more conventional adapters::
 
     >>> from plone.indexer.interfaces import IIndexer
     >>> from Products.ZCatalog.interfaces import IZCatalog
+    >>> from zope.component import adapter
+    >>> from zope.interface import implementer
 
-    >>> from zope.interface import implements
-    >>> from zope.component import adapts
-    >>> class LengthIndexer(object):
+    >>> @implementer(IIndexer)
+    ... @adapter(IPage, IZCatalog)
+    ... class LengthIndexer(object):
     ...     """Index the length of the body text
     ...     """
-    ...     implements(IIndexer)
-    ...     adapts(IPage, IZCatalog)
-    ...     
     ...     def __init__(self, context, catalog):
     ...         self.context = context
     ...         self.catalog = catalog
-    ...         
+    ...
     ...     def __call__(self):
     ...         return len(self.context.text)
 
-We normally just use IZCatalog for the catalog adaptation, to apply to any
-catalog. However, if you want different indexers for different types of
-catalogs, there is an example later in this test.
+We normally just use IZCatalog for the catalog adaptation, to apply to any catalog.
+However, if you want different indexers for different types of catalogs, there is an example later in this test.
 
 You'd register this with ZCML like so::
 
     <adapter factory=".indexers.LengthIndexer" name="length" />
-    
-Or in a test:
+
+Or in a test::
 
     >>> provideAdapter(LengthIndexer, name="length")
 
-If you're only curious about how to write indexers, you can probably stop
-here. If you want to know more about how they work and how they are wired into
-a framework, read on.
+If you're only curious about how to write indexers, you can probably stop here.
+If you want to know more about how they work and how they are wired into a framework, read on.
+
 
 Hooking up indexers to the framework
 =====================================
 
-Here is a mock implementation of a ZCatalog.catalog_object() override, based
-on the one in Plone. We'll use this for testing. We won't bother with the full
-ZCatalog interface, only catalog_object(), and we'll stub out a few things.
-This really is for illustration purposes only, to show the intended usage
-pattern.
-
-In CMF 2.2, there is an IIndexableObject marker interface defined in 
-Products.CMFCore.interfaces. We have a compatibility alias in this package
-for use with CMF 2.1.
+Here is a mock implementation of a ZCatalog.catalog_object() override, based on the one in Plone.
+We'll use this for testing.
+We won't bother with the full ZCatalog interface, only catalog_object(), and we'll stub out a few things.
+This really is for illustration purposes only, to show the intended usage pattern.
 
-    >>> from Products.ZCatalog.interfaces import IZCatalog
+In CMF 2.2, there is an IIndexableObject marker interface defined in Products.CMFCore.interfaces.
+We have a compatibility alias in this package for use with CMF 2.1.
+
+::
+
+    >>> from OFS.interfaces import IItem
     >>> from plone.indexer.interfaces import IIndexableObject
+    >>> from Products.ZCatalog.interfaces import IZCatalog
     >>> from zope.component import queryMultiAdapter
 
-    >>> class FauxCatalog(object):
-    ...     implements(IZCatalog)
+    >>> @implementer(IZCatalog, IItem)
+    ... class FauxCatalog(object):
     ...
     ...     def catalog_object(self, object, uid, idxs=[]):
     ...         """Pretend to index 'object' under the key 'uid'. We'll
     ...         print the results of the indexing operation to the screen .
     ...         """
-    ...         
+    ...
     ...         if not IIndexableObject.providedBy(object):
     ...             wrapper = queryMultiAdapter((object, self,), IIndexableObject)
     ...             if wrapper is not None:
     ...                 object = wrapper
-    ...         
+    ...
     ...         # Perform the actual indexing of attributes in the idxs list
     ...         for idx in idxs:
     ...             try:
     ...                 indexed_value = getattr(object, idx)
     ...                 if callable(indexed_value):
     ...                     indexed_value = indexed_value()
-    ...                 print idx, "=", indexed_value
+    ...                 print("{0} = {1}".format(idx, indexed_value))
     ...             except (AttributeError, TypeError,):
     ...                 pass
 
 The important things here are:
 
     - We attempt to obtain an IIndexableObject for the object to be indexed.
-      This is just a way to get hold of an implementation of this interface
-      (we'll register one in a moment) and allow some coarse-grained overrides.
-      
-    - Cataloging involves looking up attributes on the indexable object 
-      wrapper matching the names of indexes (in the real ZCatalog, this is
-      actually decoupled, but let's not get carried away). If they are
-      callable, they should be called. This is just mimicking what ZCatalog's
-      implementation does.
-      
-This package comes with an implementation of an IIndexableObject adapter that
-knows how to delegate to an IIndexer. Let's now register that as the default
-IIndexableObject wrapper adapter so that the code above will find it.
+      This is just a way to get hold of an implementation of this interface (we'll register one in a moment) and allow some coarse-grained overrides.
+
+    - Cataloging involves looking up attributes on the indexable object wrapper matching the names of indexes (in the real ZCatalog, this is actually decoupled, but let's not get carried away).
+      If they are callable, they should be called.
+      This is just mimicking what ZCatalog's implementation does.
+
+This package comes with an implementation of an IIndexableObject adapter that knows how to delegate to an IIndexer.
+Let's now register that as the default IIndexableObject wrapper adapter so that the code above will find it::
 
-    >>> from plone.indexer.wrapper import IndexableObjectWrapper
     >>> from plone.indexer.interfaces import IIndexableObject
+    >>> from plone.indexer.wrapper import IndexableObjectWrapper
     >>> provideAdapter(factory=IndexableObjectWrapper, adapts=(Interface, IZCatalog,), provides=IIndexableObject)
 
 Seeing it in action
 ===================
 
-Now for the testing. First, we need a faux catalog:
+Now for the testing. First, we need a faux catalog::
 
     >>> catalog = FauxCatalog()
 
-Finally, let's create some objects to index.
+Finally, let's create some objects to index::
 
     >>> page = Page(u"The page body text here")
     >>> news = NewsItem(u"News summary", u"News body text", u"Audience")
 
-First of all, let's demonstrate that our indexers work and apply only to
-the types for which they are registered.
+First of all, let's demonstrate that our indexers work and apply only to the types for which they are registered::
 
     >>> catalog.catalog_object(page, 'p1', idxs=['description', 'audience', 'length'])
     description = The page b
     length = 23
 
     >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
     description = News summary
     audience = AUDIENCE
 
-Our custom indexable object wrapper is capable of looking up workflow
-variables if the portal_workflow tool is available. For testing purposes,
-we'll create a fake minimal workflow tool and stash it onto the fake catalog
-so that it can be found by getToolByName. In real life, it would of course be
-acquirable as normal.
+Our custom indexable object wrapper is capable of looking up workflow variables if the portal_workflow tool is available.
+For testing purposes, we'll create a fake minimal workflow tool and stash it onto the fake catalog so that it can be found by getToolByName.
+In real life, it would of course be acquirable as normal::
 
-    >>> class FauxWorkflowTool(object):
+    >>> @implementer(IItem)
+    ... class FauxWorkflowTool(object):
     ...     def getCatalogVariablesFor(self, object):
     ...         return dict(review_state='published', audience='Somebody')
     >>> catalog.portal_workflow = FauxWorkflowTool()
 
-If we now index 'review_state', it will be obtained from the workflow
-variables. However, a custom indexer still overrides workflow variables.
+If we now index 'review_state', it will be obtained from the workflow variables.
+However, a custom indexer still overrides workflow variables::
 
     >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'review_state'])
     description = News summary
     audience = AUDIENCE
     review_state = published
 
-Finally, if not adapter can be found, we fall back on getattr() on the object.
+Finally, if not adapter can be found, we fall back on getattr() on the object::
 
     >>> catalog.catalog_object(page, 'p3', idxs=['description', 'text'])
     description = The page b
     text = The page body text here
 
+
 Customising indexers based on the catalog type
 ==============================================
 
 It is possible to provide a custom indexer for a different type of catalog.
-To test that, let's create a secondary catalog and mark it with a marker
-interface.
+To test that, let's create a secondary catalog and mark it with a marker interface::
 
     >>> from zope.interface import Interface
     >>> class IAlternateCatalog(Interface):
     ...     pass
     >>> from zope.interface import alsoProvides
     >>> catalog2 = FauxCatalog()
     >>> alsoProvides(catalog2, IAlternateCatalog)
 
-Let's say that we did not want the news item audience uppercased here. We
-could provide a custom indexer for just this catalog:
+Let's say that we did not want the news item audience uppercased here.
+We could provide a custom indexer for just this catalog::
 
     >>> @indexer(INewsItem, IAlternateCatalog)
     ... def alternate_newsitem_audience(object):
     ...     return object.audience.lower()
     >>> provideAdapter(alternate_newsitem_audience, name='audience')
 
-This does not affect the first catalog:
+This does not affect the first catalog::
 
     >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
     description = News summary
     audience = AUDIENCE
 
-However, the second catalog gets the audience in lowercase.
+However, the second catalog gets the audience in lowercase::
 
     >>> catalog2.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
     description = News summary
     audience = audience
 
+
 Interfaces provided by the wrapper
 ==================================
 
-The indexable object wrapper has one particular feature: instances of the
-wrapper will provide the same interfaces as instances of the wrapped object.
-For example:
+The indexable object wrapper has one particular feature: instances of the wrapper will provide the same interfaces as instances of the wrapped object.
+For example::
+
+    >>> from plone.indexer.interfaces import IIndexableObject
+    >>> from plone.indexer.interfaces import IIndexableObjectWrapper
 
-    >>> from plone.indexer.interfaces import IIndexableObjectWrapper, IIndexableObject
     >>> wrapper = IndexableObjectWrapper(page, catalog)
     >>> IIndexableObjectWrapper.providedBy(wrapper)
     True
     >>> IIndexableObject.providedBy(wrapper)
     True
     >>> IPage.providedBy(wrapper)
     True
@@ -309,16 +287,17 @@
     >>> IIndexableObjectWrapper.providedBy(wrapper)
     True
     >>> IPage.providedBy(wrapper)
     False
     >>> INewsItem.providedBy(wrapper)
     True
 
+
 Unboxing
 ========
 
-It is possible to obtain the wrapped object from the wrapper:
+It is possible to obtain the wrapped object from the wrapper::
 
     >>> wrapper = IndexableObjectWrapper(page, catalog)
     >>> wrapper._getWrappedObject() is page
     True
```

### Comparing `plone.indexer-1.0rc2/plone.indexer.egg-info/PKG-INFO` & `plone.indexer-2.0.0/plone.indexer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,368 +1,475 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: plone.indexer
-Version: 1.0rc2
+Version: 2.0.0
 Summary: Hooks to facilitate managing custom index values in Zope 2/CMF applications
-Home-page: http://pypi.python.org/pypi/plone.indexer
-Author: Martin Aspeli
-Author-email: optilude@gmail.com
-License: LGPL
-Description: Introduction
-        ============
-        
-        This package provides primitives to help delegate ZCatalog indexing operations
-        to adapters. It doesn't do very much on its own, but can be used by catalog
-        implementations that want to allow individual index values to be provided
-        not by the object itself, but by separate adapters.
-        
-        Writing indexers
-        ================
-        
-        An indexer is a named adapter that adapts the type of an object and provides
-        a value to be indexed when the catalog attempts to index the attribute with
-        that name.
-        
-        For example, let's say we have two types, page and news item:
-        
-        >>> from zope.interface import implements, Interface
-        >>> from zope import schema
-        
-        >>> class IPage(Interface):
-        ...     text = schema.Text(title=u"Body text")
-        >>> class Page(object):
-        ...     implements(IPage)
-        ...     def __init__(self, text):
-        ...         self.text = text
-        
-        >>> class INewsItem(Interface):
-        ...     summary = schema.TextLine(title=u"Short summary")
-        ...     story = schema.Text(title=u"Body text")
-        ...     audience = schema.TextLine(title=u"Audience")
-        
-        >>> class NewsItem(object):
-        ...     implements(INewsItem)
-        ...     def __init__(self, summary, story, audience):
-        ...         self.summary = summary
-        ...         self.story = story
-        ...         self.audience = audience
-        
-        Now, pretend that our catalog had an index 'description', which for a page
-        should contain the first 10 characters from the body text, and for a news
-        item should contain the contents of the 'summary' field. Furthermore, there
-        is an index 'audience' that should contain the value of the corresponding
-        field for news items, in all uppercase. It should do nothing for pages.
-        
-        We could write indexers for all of these like this
-        
-        >>> from plone.indexer import indexer
-        
-        >>> @indexer(IPage)
-        ... def page_description(object):
-        ...     return object.text[:10]
-        
-        >>> @indexer(INewsItem)
-        ... def newsitem_description(object):
-        ...     return object.summary
-        
-        >>> @indexer(INewsItem)
-        ... def newsitem_audience(object):
-        ...     return object.audience.upper()
-        
-        These need to be registered as named adapters, where the name corresponds to
-        the index name. In ZCML, that may be::
-        
-        <adapter name="description" factory=".indexers.page_description" />
-        <adapter name="description" factory=".indexers.newsitem_description" />
-        <adapter name="audience" factory=".indexers.newsitem_audience" />
-        
-        We can omit the 'for' attribute because we passed this to the @indexer
-        decorator, and we can omit the 'provides' attribute because the thing
-        returned by the decorator is actually a class providing the required IIndexer
-        interface.
-        
-        For the purposes of the ensuing tests, we'll register these directly.
-        
-        >>> from zope.component import provideAdapter
-        >>> provideAdapter(page_description, name='description')
-        >>> provideAdapter(newsitem_description, name='description')
-        >>> provideAdapter(newsitem_audience, name='audience')
-        
-        Testing your indexers (or calling them directly)
-        ------------------------------------------------
-        
-        If you are writing tests for your indexers (as you should!), then you should
-        be aware of the following:
-        
-        When the @indexer decorator returns, it turns your function into an instance
-        of type DelegatingIndexerFactory. This is an adapter factory that can create
-        a DelegatingIndexer, which in turn will call your function when asked to
-        perform indexing operations.
-        
-        This means that you can't just call your function to test the indexer.
-        Instead, you need to instantiate the adapter and then call the delegating
-        indexer with the portal root as the first argument. For example:
-        
-        >>> test_page = Page(text=u"My page with some text")
-        >>> page_description(test_page)()
-        u'My page wi'
-        
-        This will suffice in most cases. Note that there is actually a second
-        parameter, catalog, which defaults to None. If you need to write an indexer
-        that acts on catalog, you'll need to register a conventional adapter, as
-        described in the next section.
-        
-        Other means of registering indexers
-        -----------------------------------
-        
-        At the end of the day, an indexer is just a named multi-adapter from the
-        indexable object (e.g. INewsItem or IPage above) and the catalog (usually
-        portal_catalog in a CMF application) to IIndexer, where the name is the name
-        of the indexed attribute in the catalog. Thus, you could register your
-        indexers as more conventional adapters:
-        
-        >>> from plone.indexer.interfaces import IIndexer
-        >>> from Products.ZCatalog.interfaces import IZCatalog
-        
-        >>> from zope.interface import implements
-        >>> from zope.component import adapts
-        >>> class LengthIndexer(object):
-        ...     """Index the length of the body text
-        ...     """
-        ...     implements(IIndexer)
-        ...     adapts(IPage, IZCatalog)
-        ...
-        ...     def __init__(self, context, catalog):
-        ...         self.context = context
-        ...         self.catalog = catalog
-        ...
-        ...     def __call__(self):
-        ...         return len(self.context.text)
-        
-        We normally just use IZCatalog for the catalog adaptation, to apply to any
-        catalog. However, if you want different indexers for different types of
-        catalogs, there is an example later in this test.
-        
-        You'd register this with ZCML like so::
-        
-        <adapter factory=".indexers.LengthIndexer" name="length" />
-        
-        Or in a test:
-        
-        >>> provideAdapter(LengthIndexer, name="length")
-        
-        If you're only curious about how to write indexers, you can probably stop
-        here. If you want to know more about how they work and how they are wired into
-        a framework, read on.
-        
-        Hooking up indexers to the framework
-        =====================================
-        
-        Here is a mock implementation of a ZCatalog.catalog_object() override, based
-        on the one in Plone. We'll use this for testing. We won't bother with the full
-        ZCatalog interface, only catalog_object(), and we'll stub out a few things.
-        This really is for illustration purposes only, to show the intended usage
-        pattern.
-        
-        In CMF 2.2, there is an IIndexableObject marker interface defined in
-        Products.CMFCore.interfaces. We have a compatibility alias in this package
-        for use with CMF 2.1.
-        
-        >>> from Products.ZCatalog.interfaces import IZCatalog
-        >>> from plone.indexer.interfaces import IIndexableObject
-        >>> from zope.component import queryMultiAdapter
-        
-        >>> class FauxCatalog(object):
-        ...     implements(IZCatalog)
-        ...
-        ...     def catalog_object(self, object, uid, idxs=[]):
-        ...         """Pretend to index 'object' under the key 'uid'. We'll
-        ...         print the results of the indexing operation to the screen .
-        ...         """
-        ...
-        ...         if not IIndexableObject.providedBy(object):
-        ...             wrapper = queryMultiAdapter((object, self,), IIndexableObject)
-        ...             if wrapper is not None:
-        ...                 object = wrapper
-        ...
-        ...         # Perform the actual indexing of attributes in the idxs list
-        ...         for idx in idxs:
-        ...             try:
-        ...                 indexed_value = getattr(object, idx)
-        ...                 if callable(indexed_value):
-        ...                     indexed_value = indexed_value()
-        ...                 print idx, "=", indexed_value
-        ...             except (AttributeError, TypeError,):
-        ...                 pass
-        
-        The important things here are:
-        
-        - We attempt to obtain an IIndexableObject for the object to be indexed.
-        This is just a way to get hold of an implementation of this interface
-        (we'll register one in a moment) and allow some coarse-grained overrides.
-        
-        - Cataloging involves looking up attributes on the indexable object
-        wrapper matching the names of indexes (in the real ZCatalog, this is
-        actually decoupled, but let's not get carried away). If they are
-        callable, they should be called. This is just mimicking what ZCatalog's
-        implementation does.
-        
-        This package comes with an implementation of an IIndexableObject adapter that
-        knows how to delegate to an IIndexer. Let's now register that as the default
-        IIndexableObject wrapper adapter so that the code above will find it.
-        
-        >>> from plone.indexer.wrapper import IndexableObjectWrapper
-        >>> from plone.indexer.interfaces import IIndexableObject
-        >>> provideAdapter(factory=IndexableObjectWrapper, adapts=(Interface, IZCatalog,), provides=IIndexableObject)
-        
-        Seeing it in action
-        ===================
-        
-        Now for the testing. First, we need a faux catalog:
-        
-        >>> catalog = FauxCatalog()
-        
-        Finally, let's create some objects to index.
-        
-        >>> page = Page(u"The page body text here")
-        >>> news = NewsItem(u"News summary", u"News body text", u"Audience")
-        
-        First of all, let's demonstrate that our indexers work and apply only to
-        the types for which they are registered.
-        
-        >>> catalog.catalog_object(page, 'p1', idxs=['description', 'audience', 'length'])
-        description = The page b
-        length = 23
-        
-        >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
-        description = News summary
-        audience = AUDIENCE
-        
-        Our custom indexable object wrapper is capable of looking up workflow
-        variables if the portal_workflow tool is available. For testing purposes,
-        we'll create a fake minimal workflow tool and stash it onto the fake catalog
-        so that it can be found by getToolByName. In real life, it would of course be
-        acquirable as normal.
-        
-        >>> class FauxWorkflowTool(object):
-        ...     def getCatalogVariablesFor(self, object):
-        ...         return dict(review_state='published', audience='Somebody')
-        >>> catalog.portal_workflow = FauxWorkflowTool()
-        
-        If we now index 'review_state', it will be obtained from the workflow
-        variables. However, a custom indexer still overrides workflow variables.
-        
-        >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'review_state'])
-        description = News summary
-        audience = AUDIENCE
-        review_state = published
-        
-        Finally, if not adapter can be found, we fall back on getattr() on the object.
-        
-        >>> catalog.catalog_object(page, 'p3', idxs=['description', 'text'])
-        description = The page b
-        text = The page body text here
-        
-        Customising indexers based on the catalog type
-        ==============================================
-        
-        It is possible to provide a custom indexer for a different type of catalog.
-        To test that, let's create a secondary catalog and mark it with a marker
-        interface.
-        
-        >>> from zope.interface import Interface
-        >>> class IAlternateCatalog(Interface):
-        ...     pass
-        >>> from zope.interface import alsoProvides
-        >>> catalog2 = FauxCatalog()
-        >>> alsoProvides(catalog2, IAlternateCatalog)
-        
-        Let's say that we did not want the news item audience uppercased here. We
-        could provide a custom indexer for just this catalog:
-        
-        >>> @indexer(INewsItem, IAlternateCatalog)
-        ... def alternate_newsitem_audience(object):
-        ...     return object.audience.lower()
-        >>> provideAdapter(alternate_newsitem_audience, name='audience')
-        
-        This does not affect the first catalog:
-        
-        >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
-        description = News summary
-        audience = AUDIENCE
-        
-        However, the second catalog gets the audience in lowercase.
-        
-        >>> catalog2.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
-        description = News summary
-        audience = audience
-        
-        Interfaces provided by the wrapper
-        ==================================
-        
-        The indexable object wrapper has one particular feature: instances of the
-        wrapper will provide the same interfaces as instances of the wrapped object.
-        For example:
-        
-        >>> from plone.indexer.interfaces import IIndexableObjectWrapper, IIndexableObject
-        >>> wrapper = IndexableObjectWrapper(page, catalog)
-        >>> IIndexableObjectWrapper.providedBy(wrapper)
-        True
-        >>> IIndexableObject.providedBy(wrapper)
-        True
-        >>> IPage.providedBy(wrapper)
-        True
-        >>> INewsItem.providedBy(wrapper)
-        False
-        
-        >>> wrapper = IndexableObjectWrapper(news, catalog)
-        >>> IIndexableObjectWrapper.providedBy(wrapper)
-        True
-        >>> IPage.providedBy(wrapper)
-        False
-        >>> INewsItem.providedBy(wrapper)
-        True
-        
-        Unboxing
-        ========
-        
-        It is possible to obtain the wrapped object from the wrapper:
-        
-        >>> wrapper = IndexableObjectWrapper(page, catalog)
-        >>> wrapper._getWrappedObject() is page
-        True
-        
-        
-        Changelog
-        =========
-        
-        1.0rc2 - unreleased
-        ------------------
-        
-        * Added _getWrappedObject() method to get hold of the underlying object.
-        Note that this means you can't have an index/metadata column with this name.
-        [optilude]
-        
-        * Corrected IZCatalog import location to point to the interfaces module.
-        [hannosch]
-        
-        
-        1.0rc1 - 2009-03-26
-        ------------------
-        
-        * Updated the interface to match the developments of similar functionality
-        on CMF trunk. This means that indexers are now multi-adapters on
-        (object, catalog), and the keyword arguments (including the implicit
-        'portal' parameter) are gone.
-        [optilude]
-        
-        
-        1.0a1 - 2009-03-05
-        ------------------
-        
-        * Initial release
-        
-        
+Home-page: https://pypi.org/project/plone.indexer
+Author: Plone Foundation
+Author-email: plone-developers@lists.sourceforge.net
+License: BSD
 Keywords: plone cmf zope catalog index
-Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
+Classifier: Framework :: Plone :: 6.0
+Classifier: Framework :: Plone :: Core
+Classifier: Framework :: Zope :: 5
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+
+Introduction
+============
+
+This package provides primitives to help delegate ZCatalog indexing operations
+to adapters. It doesn't do very much on its own, but can be used by catalog
+implementations that want to allow individual index values to be provided
+not by the object itself, but by separate adapters.
+
+
+Changelog
+=========
+
+.. You should *NOT* be adding new change log entries to this file.
+   You should create a file in the news directory instead.
+   For helpful instructions, please see:
+   https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
+
+.. towncrier release notes start
+
+2.0.0 (2023-04-19)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7 support.
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
+1.0.7 (2020-04-20)
+------------------
+
+Bug fixes:
+
+
+- Minor packaging updates. (#1)
+
+
+1.0.6 (2019-04-29)
+------------------
+
+Bug fixes:
+
+
+- Fixed: doctests on Python 2 were not correctly checked.  [maurits] (#7)
+
+
+1.0.5 (2018-09-26)
+------------------
+
+Fixes:
+
+- fix https://github.com/plone/Products.CMFPlone/issues/2469:
+  "Subobjects are indexing attributes of parent".
+  Allow only direct attributes and acquired PythonScripts,
+  but not acquired attributes.
+  Indexers and PythonScripts are able to handle this explicitly,
+  because they get the acquisition-wrapped object.
+  [jensens]
+
+- Fix tests to work in Python 3
+  [pbauer]
+
+
+1.0.4 (2016-02-25)
+------------------
+
+Fixes:
+
+- Replace deprecated ``zope.testing.doctestunit`` import with ``doctest``
+  module from stdlib.
+  [thet]
+
+- Reformat according to the Plone styleguide.
+  [thet]
+
+
+1.0.3 (2015-05-05)
+------------------
+
+- Add missing dependency on Products.ZCatalog.
+  [gforcada]
+
+
+1.0.2 (2013-01-13)
+------------------
+
+- Changed the @indexer decorator to maintain the information about the wrapped
+  function (__doc__, __module__, __name__, etc).
+  [dokai]
+
+
+1.0.1 (2012-12-14)
+------------------
+
+- Relicense under modified BSD license; per Plone Foundation board
+  approval on 2012-05-31.
+  See: http://plone.org/foundation/materials/foundation-resolutions/plone-framework-components-relicensing-policy
+  [supton]
+
+- Add MANIFEST.in.
+  [WouterVH]
+
+
+1.0 - 2010-07-18
+----------------
+
+- Fixed reSt markup in the changelog.
+  [hannosch]
+
+- Update license to GPL version 2 only.
+  [hannosch]
+
+
+1.0rc2 - 2009-04-05
+-------------------
+
+- Added _getWrappedObject() method to get hold of the underlying object.
+  Note that this means you can't have an index/metadata column with this name.
+  [optilude]
+
+- Corrected IZCatalog import location to point to the interfaces module.
+  [hannosch]
+
+
+1.0rc1 - 2009-03-26
+-------------------
+
+- Updated the interface to match the developments of similar functionality
+  on CMF trunk. This means that indexers are now multi-adapters on
+  (object, catalog), and the keyword arguments (including the implicit
+  'portal' parameter) are gone.
+  [optilude]
+
+
+1.0a1 - 2009-03-05
+------------------
+
+- Initial release
+
+
+Writing indexers
+================
+
+An indexer is a named adapter that adapts the type of an object and provides a value to be indexed when the catalog attempts to index the attribute with that name.
+
+For example, let's say we have two types, page and news item::
+
+    >>> from zope.interface import Interface
+    >>> from zope.interface import implementer
+    >>> from zope import schema
+
+    >>> class IPage(Interface):
+    ...     text = schema.Text(title=u"Body text")
+
+    >>> @implementer(IPage)
+    ... class Page(object):
+    ...     def __init__(self, text):
+    ...         self.text = text
+
+    >>> class INewsItem(Interface):
+    ...     summary = schema.TextLine(title=u"Short summary")
+    ...     story = schema.Text(title=u"Body text")
+    ...     audience = schema.TextLine(title=u"Audience")
+
+    >>> @implementer(INewsItem)
+    ... class NewsItem(object):
+    ...     def __init__(self, summary, story, audience):
+    ...         self.summary = summary
+    ...         self.story = story
+    ...         self.audience = audience
+
+Now, pretend that our catalog had an index 'description', which for a page should contain the first 10 characters from the body text, and for a news item should contain the contents of the 'summary' field.
+Furthermore, there is an index 'audience' that should contain the value of the corresponding field for news items, in all uppercase.
+It should do nothing for pages.
+
+We could write indexers for all of these like this::
+
+    >>> from plone.indexer import indexer
+
+    >>> @indexer(IPage)
+    ... def page_description(object):
+    ...     return object.text[:10]
+
+    >>> @indexer(INewsItem)
+    ... def newsitem_description(object):
+    ...     return object.summary
+
+    >>> @indexer(INewsItem)
+    ... def newsitem_audience(object):
+    ...     return object.audience.upper()
+
+These need to be registered as named adapters, where the name corresponds to the index name.
+In ZCML, that may be::
+
+    <adapter name="description" factory=".indexers.page_description" />
+    <adapter name="description" factory=".indexers.newsitem_description" />
+    <adapter name="audience" factory=".indexers.newsitem_audience" />
+
+We can omit the 'for' attribute because we passed this to the @indexer decorator, and we can omit the 'provides' attribute because the thing returned by the decorator is actually a class providing the required IIndexer interface.
+
+For the purposes of the ensuing tests, we'll register these directly::
+
+    >>> from zope.component import provideAdapter
+    >>> provideAdapter(page_description, name='description')
+    >>> provideAdapter(newsitem_description, name='description')
+    >>> provideAdapter(newsitem_audience, name='audience')
+
+
+Testing your indexers (or calling them directly)
+------------------------------------------------
+
+If you are writing tests for your indexers (as you should!), then you should be aware of the following:
+
+When the @indexer decorator returns, it turns your function into an instance of type DelegatingIndexerFactory.
+This is an adapter factory that can create a DelegatingIndexer, which in turn will call your function when asked to perform indexing operations.
+
+This means that you can't just call your function to test the indexer.
+Instead, you need to instantiate the adapter and then call the delegating indexer with the portal root as the first argument.
+For example::
+
+    >>> test_page = Page(text=u"My page with some text")
+    >>> page_description(test_page)()
+    'My page wi'
+
+This will suffice in most cases.
+Note that there is actually a second parameter, catalog, which defaults to None.
+If you need to write an indexer that acts on catalog, you'll need to register a conventional adapter, as described in the next section.
+
+
+Other means of registering indexers
+-----------------------------------
+
+At the end of the day, an indexer is just a named multi-adapter from the indexable object (e.g.
+INewsItem or IPage above) and the catalog (usually portal_catalog in a CMF application) to IIndexer, where the name is the name of the indexed attribute in the catalog.
+Thus, you could register your indexers as more conventional adapters::
+
+    >>> from plone.indexer.interfaces import IIndexer
+    >>> from Products.ZCatalog.interfaces import IZCatalog
+    >>> from zope.component import adapter
+    >>> from zope.interface import implementer
+
+    >>> @implementer(IIndexer)
+    ... @adapter(IPage, IZCatalog)
+    ... class LengthIndexer(object):
+    ...     """Index the length of the body text
+    ...     """
+    ...     def __init__(self, context, catalog):
+    ...         self.context = context
+    ...         self.catalog = catalog
+    ...
+    ...     def __call__(self):
+    ...         return len(self.context.text)
+
+We normally just use IZCatalog for the catalog adaptation, to apply to any catalog.
+However, if you want different indexers for different types of catalogs, there is an example later in this test.
+
+You'd register this with ZCML like so::
+
+    <adapter factory=".indexers.LengthIndexer" name="length" />
+
+Or in a test::
+
+    >>> provideAdapter(LengthIndexer, name="length")
+
+If you're only curious about how to write indexers, you can probably stop here.
+If you want to know more about how they work and how they are wired into a framework, read on.
+
+
+Hooking up indexers to the framework
+=====================================
+
+Here is a mock implementation of a ZCatalog.catalog_object() override, based on the one in Plone.
+We'll use this for testing.
+We won't bother with the full ZCatalog interface, only catalog_object(), and we'll stub out a few things.
+This really is for illustration purposes only, to show the intended usage pattern.
+
+In CMF 2.2, there is an IIndexableObject marker interface defined in Products.CMFCore.interfaces.
+We have a compatibility alias in this package for use with CMF 2.1.
+
+::
+
+    >>> from OFS.interfaces import IItem
+    >>> from plone.indexer.interfaces import IIndexableObject
+    >>> from Products.ZCatalog.interfaces import IZCatalog
+    >>> from zope.component import queryMultiAdapter
+
+    >>> @implementer(IZCatalog, IItem)
+    ... class FauxCatalog(object):
+    ...
+    ...     def catalog_object(self, object, uid, idxs=[]):
+    ...         """Pretend to index 'object' under the key 'uid'. We'll
+    ...         print the results of the indexing operation to the screen .
+    ...         """
+    ...
+    ...         if not IIndexableObject.providedBy(object):
+    ...             wrapper = queryMultiAdapter((object, self,), IIndexableObject)
+    ...             if wrapper is not None:
+    ...                 object = wrapper
+    ...
+    ...         # Perform the actual indexing of attributes in the idxs list
+    ...         for idx in idxs:
+    ...             try:
+    ...                 indexed_value = getattr(object, idx)
+    ...                 if callable(indexed_value):
+    ...                     indexed_value = indexed_value()
+    ...                 print("{0} = {1}".format(idx, indexed_value))
+    ...             except (AttributeError, TypeError,):
+    ...                 pass
+
+The important things here are:
+
+    - We attempt to obtain an IIndexableObject for the object to be indexed.
+      This is just a way to get hold of an implementation of this interface (we'll register one in a moment) and allow some coarse-grained overrides.
+
+    - Cataloging involves looking up attributes on the indexable object wrapper matching the names of indexes (in the real ZCatalog, this is actually decoupled, but let's not get carried away).
+      If they are callable, they should be called.
+      This is just mimicking what ZCatalog's implementation does.
+
+This package comes with an implementation of an IIndexableObject adapter that knows how to delegate to an IIndexer.
+Let's now register that as the default IIndexableObject wrapper adapter so that the code above will find it::
+
+    >>> from plone.indexer.interfaces import IIndexableObject
+    >>> from plone.indexer.wrapper import IndexableObjectWrapper
+    >>> provideAdapter(factory=IndexableObjectWrapper, adapts=(Interface, IZCatalog,), provides=IIndexableObject)
+
+Seeing it in action
+===================
+
+Now for the testing. First, we need a faux catalog::
+
+    >>> catalog = FauxCatalog()
+
+Finally, let's create some objects to index::
+
+    >>> page = Page(u"The page body text here")
+    >>> news = NewsItem(u"News summary", u"News body text", u"Audience")
+
+First of all, let's demonstrate that our indexers work and apply only to the types for which they are registered::
+
+    >>> catalog.catalog_object(page, 'p1', idxs=['description', 'audience', 'length'])
+    description = The page b
+    length = 23
+
+    >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
+    description = News summary
+    audience = AUDIENCE
+
+Our custom indexable object wrapper is capable of looking up workflow variables if the portal_workflow tool is available.
+For testing purposes, we'll create a fake minimal workflow tool and stash it onto the fake catalog so that it can be found by getToolByName.
+In real life, it would of course be acquirable as normal::
+
+    >>> @implementer(IItem)
+    ... class FauxWorkflowTool(object):
+    ...     def getCatalogVariablesFor(self, object):
+    ...         return dict(review_state='published', audience='Somebody')
+    >>> catalog.portal_workflow = FauxWorkflowTool()
+
+If we now index 'review_state', it will be obtained from the workflow variables.
+However, a custom indexer still overrides workflow variables::
+
+    >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'review_state'])
+    description = News summary
+    audience = AUDIENCE
+    review_state = published
+
+Finally, if not adapter can be found, we fall back on getattr() on the object::
+
+    >>> catalog.catalog_object(page, 'p3', idxs=['description', 'text'])
+    description = The page b
+    text = The page body text here
+
+
+Customising indexers based on the catalog type
+==============================================
+
+It is possible to provide a custom indexer for a different type of catalog.
+To test that, let's create a secondary catalog and mark it with a marker interface::
+
+    >>> from zope.interface import Interface
+    >>> class IAlternateCatalog(Interface):
+    ...     pass
+    >>> from zope.interface import alsoProvides
+    >>> catalog2 = FauxCatalog()
+    >>> alsoProvides(catalog2, IAlternateCatalog)
+
+Let's say that we did not want the news item audience uppercased here.
+We could provide a custom indexer for just this catalog::
+
+    >>> @indexer(INewsItem, IAlternateCatalog)
+    ... def alternate_newsitem_audience(object):
+    ...     return object.audience.lower()
+    >>> provideAdapter(alternate_newsitem_audience, name='audience')
+
+This does not affect the first catalog::
+
+    >>> catalog.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
+    description = News summary
+    audience = AUDIENCE
+
+However, the second catalog gets the audience in lowercase::
+
+    >>> catalog2.catalog_object(news, 'n1', idxs=['description', 'audience', 'length'])
+    description = News summary
+    audience = audience
+
+
+Interfaces provided by the wrapper
+==================================
+
+The indexable object wrapper has one particular feature: instances of the wrapper will provide the same interfaces as instances of the wrapped object.
+For example::
+
+    >>> from plone.indexer.interfaces import IIndexableObject
+    >>> from plone.indexer.interfaces import IIndexableObjectWrapper
+
+    >>> wrapper = IndexableObjectWrapper(page, catalog)
+    >>> IIndexableObjectWrapper.providedBy(wrapper)
+    True
+    >>> IIndexableObject.providedBy(wrapper)
+    True
+    >>> IPage.providedBy(wrapper)
+    True
+    >>> INewsItem.providedBy(wrapper)
+    False
+
+    >>> wrapper = IndexableObjectWrapper(news, catalog)
+    >>> IIndexableObjectWrapper.providedBy(wrapper)
+    True
+    >>> IPage.providedBy(wrapper)
+    False
+    >>> INewsItem.providedBy(wrapper)
+    True
+
+
+Unboxing
+========
+
+It is possible to obtain the wrapped object from the wrapper::
+
+    >>> wrapper = IndexableObjectWrapper(page, catalog)
+    >>> wrapper._getWrappedObject() is page
+    True
+
```

### Comparing `plone.indexer-1.0rc2/plone.indexer.egg-info/SOURCES.txt` & `plone.indexer-2.0.0/plone.indexer.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+CHANGES.rst
+CONTRIBUTING.rst
+MANIFEST.in
+README.rst
+pyproject.toml
+setup.cfg
 setup.py
-docs/HISTORY.txt
-docs/INSTALL.txt
+docs/LICENSE.txt
 plone/__init__.py
 plone.indexer.egg-info/PKG-INFO
 plone.indexer.egg-info/SOURCES.txt
 plone.indexer.egg-info/dependency_links.txt
-plone.indexer.egg-info/entry_points.txt
 plone.indexer.egg-info/namespace_packages.txt
 plone.indexer.egg-info/not-zip-safe
 plone.indexer.egg-info/requires.txt
 plone.indexer.egg-info/top_level.txt
-plone/indexer/README.txt
+plone/indexer/README.rst
 plone/indexer/__init__.py
 plone/indexer/configure.zcml
 plone/indexer/decorator.py
 plone/indexer/delegate.py
 plone/indexer/interfaces.py
 plone/indexer/tests.py
 plone/indexer/wrapper.py
```

