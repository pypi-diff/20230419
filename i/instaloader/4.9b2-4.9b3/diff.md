# Comparing `tmp/instaloader-4.9b2.tar.gz` & `tmp/instaloader-4.9b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/instaloader-4.9b2.tar", last modified: Sat Jan 15 16:40:29 2022, max compression
+gzip compressed data, was "instaloader-4.9b3.tar", last modified: Sat Mar 19 15:40:11 2022, max compression
```

## Comparing `instaloader-4.9b2.tar` & `instaloader-4.9b3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-15 16:40:29.000000 instaloader-4.9b2/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2221 2022-01-15 16:39:27.000000 instaloader-4.9b2/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5186 2022-01-15 16:39:27.000000 instaloader-4.9b2/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     6393 2022-01-15 16:40:29.000000 instaloader-4.9b2/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-15 16:40:29.000000 instaloader-4.9b2/instaloader.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2022-01-15 16:40:29.000000 instaloader-4.9b2/instaloader.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      553 2022-01-15 16:40:29.000000 instaloader-4.9b2/instaloader.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6393 2022-01-15 16:40:29.000000 instaloader-4.9b2/instaloader.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2022-01-15 16:40:29.000000 instaloader-4.9b2/instaloader.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2022-01-15 16:40:29.000000 instaloader-4.9b2/instaloader.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-01-15 16:40:29.000000 instaloader-4.9b2/instaloader.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-01-15 16:40:29.000000 instaloader-4.9b2/instaloader.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      219 2022-01-15 16:39:27.000000 instaloader-4.9b2/AUTHORS.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-01-15 16:40:29.000000 instaloader-4.9b2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2022-01-15 16:39:27.000000 instaloader-4.9b2/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-15 16:40:29.000000 instaloader-4.9b2/instaloader/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-01-15 16:39:27.000000 instaloader-4.9b2/instaloader/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)    31271 2022-01-15 16:39:27.000000 instaloader-4.9b2/instaloader/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1880 2022-01-15 16:39:27.000000 instaloader-4.9b2/instaloader/sectioniterator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13880 2022-01-15 16:39:27.000000 instaloader-4.9b2/instaloader/nodeiterator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79087 2022-01-15 16:39:27.000000 instaloader-4.9b2/instaloader/instaloader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4821 2022-01-15 16:39:27.000000 instaloader-4.9b2/instaloader/lateststamps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73992 2022-01-15 16:39:27.000000 instaloader-4.9b2/instaloader/structures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1531 2022-01-15 16:39:27.000000 instaloader-4.9b2/instaloader/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      831 2022-01-15 16:39:27.000000 instaloader-4.9b2/instaloader/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37599 2022-01-15 16:39:27.000000 instaloader-4.9b2/instaloader/instaloadercontext.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-19 15:40:11.793995 instaloader-4.9b3/
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-03-19 15:39:16.000000 instaloader-4.9b3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-03-19 15:39:16.000000 instaloader-4.9b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     7605 2022-03-19 15:40:11.793995 instaloader-4.9b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5186 2022-03-19 15:39:16.000000 instaloader-4.9b3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-19 15:40:11.793995 instaloader-4.9b3/instaloader/
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2022-03-19 15:39:16.000000 instaloader-4.9b3/instaloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31560 2022-03-19 15:39:16.000000 instaloader-4.9b3/instaloader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1531 2022-03-19 15:39:16.000000 instaloader-4.9b3/instaloader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    80826 2022-03-19 15:39:16.000000 instaloader-4.9b3/instaloader/instaloader.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37599 2022-03-19 15:39:16.000000 instaloader-4.9b3/instaloader/instaloadercontext.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4821 2022-03-19 15:39:16.000000 instaloader-4.9b3/instaloader/lateststamps.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13880 2022-03-19 15:39:16.000000 instaloader-4.9b3/instaloader/nodeiterator.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-19 15:39:16.000000 instaloader-4.9b3/instaloader/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-03-19 15:39:16.000000 instaloader-4.9b3/instaloader/sectioniterator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    74072 2022-03-19 15:39:16.000000 instaloader-4.9b3/instaloader/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-19 15:40:11.793995 instaloader-4.9b3/instaloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7605 2022-03-19 15:40:11.000000 instaloader-4.9b3/instaloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2022-03-19 15:40:11.000000 instaloader-4.9b3/instaloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-19 15:40:11.000000 instaloader-4.9b3/instaloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-03-19 15:40:11.000000 instaloader-4.9b3/instaloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-19 15:40:11.000000 instaloader-4.9b3/instaloader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-19 15:40:11.000000 instaloader-4.9b3/instaloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-19 15:40:11.000000 instaloader-4.9b3/instaloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-19 15:40:11.793995 instaloader-4.9b3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2221 2022-03-19 15:39:16.000000 instaloader-4.9b3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `instaloader-4.9b2/setup.py` & `instaloader-4.9b3/setup.py`

 * *Files identical despite different names*

### Comparing `instaloader-4.9b2/README.rst` & `instaloader-4.9b3/README.rst`

 * *Files identical despite different names*

### Comparing `instaloader-4.9b2/PKG-INFO` & `instaloader-4.9b3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,172 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: instaloader
-Version: 4.9b2
+Version: 4.9b3
 Summary: Download pictures (or videos) along with their captions and other metadata from Instagram.
 Home-page: https://instaloader.github.io/
 Author: Alexander Graf, André Koch-Kramer
 Author-email: mail@agraf.me, koch-kramer@web.de
 License: MIT
+Description: .. image:: https://raw.githubusercontent.com/instaloader/instaloader/master/docs/logo_heading.png
+        
+        .. badges-start
+        
+        |travis| |pypi| |pyversion| |license| |aur| |contributors| |downloads|
+        
+        .. |travis| image:: https://img.shields.io/travis/instaloader/instaloader/master.svg
+           :alt: Travis-CI Build Status
+           :target: https://travis-ci.org/instaloader/instaloader
+        
+        .. |pypi| image:: https://img.shields.io/pypi/v/instaloader.svg
+           :alt: Instaloader PyPI Project Page
+           :target: https://pypi.org/project/instaloader/
+        
+        .. |license| image:: https://img.shields.io/github/license/instaloader/instaloader.svg
+           :alt: MIT License
+           :target: https://github.com/instaloader/instaloader/blob/master/LICENSE
+        
+        .. |pyversion| image:: https://img.shields.io/pypi/pyversions/instaloader.svg
+           :alt: Supported Python Versions
+        
+        .. |contributors| image:: https://img.shields.io/github/contributors/instaloader/instaloader.svg
+           :alt: Contributor Count
+           :target: https://github.com/instaloader/instaloader/graphs/contributors
+        
+        .. |aur| image:: https://img.shields.io/aur/version/instaloader.svg
+           :alt: Arch User Repository Package
+           :target: https://aur.archlinux.org/packages/instaloader/
+        
+        .. |downloads| image:: https://pepy.tech/badge/instaloader/month
+           :alt: PyPI Download Count
+           :target: https://pepy.tech/project/instaloader
+        
+        .. badges-end
+        
+        ::
+        
+            $ pip3 install instaloader
+        
+            $ instaloader profile [profile ...]
+        
+        **Instaloader**
+        
+        - downloads **public and private profiles, hashtags, user stories,
+          feeds and saved media**,
+        
+        - downloads **comments, geotags and captions** of each post,
+        
+        - automatically **detects profile name changes** and renames the target
+          directory accordingly,
+        
+        - allows **fine-grained customization** of filters and where to store
+          downloaded media,
+        
+        - automatically **resumes previously-interrupted** download iterations.
+        
+        ::
+        
+            instaloader [--comments] [--geotags]
+                        [--stories] [--highlights] [--tagged] [--igtv]
+                        [--login YOUR-USERNAME] [--fast-update]
+                        profile | "#hashtag" | :stories | :feed | :saved
+        
+        `Instaloader Documentation <https://instaloader.github.io/>`__
+        
+        
+        How to Automatically Download Pictures from Instagram
+        -----------------------------------------------------
+        
+        To **download all pictures and videos of a profile**, as well as the
+        **profile picture**, do
+        
+        ::
+        
+            instaloader profile [profile ...]
+        
+        where ``profile`` is the name of a profile you want to download. Instead
+        of only one profile, you may also specify a list of profiles.
+        
+        To later **update your local copy** of that profiles, you may run
+        
+        ::
+        
+            instaloader --fast-update profile [profile ...]
+        
+        If ``--fast-update`` is given, Instaloader stops when arriving at the
+        first already-downloaded picture.
+        
+        Alternatively, you can use ``--latest-stamps`` to have Instaloader store
+        the time each profile was last downloaded and only download newer media:
+        
+        ::
+        
+            instaloader --latest-stamps -- profile [profile ...]
+        
+        With this option it's possible to move or delete downloaded media and still keep
+        the archive updated.
+        
+        When updating profiles, Instaloader
+        automatically **detects profile name changes** and renames the target directory
+        accordingly.
+        
+        Instaloader can also be used to **download private profiles**. To do so,
+        invoke it with
+        
+        ::
+        
+            instaloader --login=your_username profile [profile ...]
+        
+        When logging in, Instaloader **stores the session cookies** in a file in your
+        temporary directory, which will be reused later the next time ``--login``
+        is given.  So you can download private profiles **non-interactively** when you
+        already have a valid session cookie file.
+        
+        `Instaloader Documentation <https://instaloader.github.io/basic-usage.html>`__
+        
+        Contributing
+        ------------
+        
+        As an open source project, Instaloader heavily depends on the contributions from
+        its community. See
+        `contributing <https://instaloader.github.io/contributing.html>`__
+        for how you may help Instaloader to become an even greater tool.
+        
+        Supporters
+        ----------
+        
+        .. current-sponsors-start
+        
+        See `Alex' GitHub Sponsors <https://github.com/sponsors/aandergr>`__ page for
+        how you can sponsor the development of Instaloader!
+        
+        .. current-sponsors-end
+        
+        It is a pleasure for us to share our Instaloader to the world, and we are proud
+        to have attracted such an active and motivating community, with so many users
+        who share their suggestions and ideas with us. Buying a community-sponsored beer
+        or coffee from time to time is very likely to further raise our passion for the
+        development of Instaloader.
+        
+        | For Donations, we provide GitHub Sponsors page, a PayPal.Me link and a Bitcoin address.
+        |  GitHub Sponsors: `Sponsor @aandergr on GitHub Sponsors <https://github.com/sponsors/aandergr>`__
+        |  PayPal: `PayPal.me/aandergr <https://www.paypal.me/aandergr>`__
+        |  BTC: 1Nst4LoadeYzrKjJ1DX9CpbLXBYE9RKLwY
+        
+        Disclaimer
+        ----------
+        
+        .. disclaimer-start
+        
+        Instaloader is in no way affiliated with, authorized, maintained or endorsed by Instagram or any of its affiliates or
+        subsidiaries. This is an independent and unofficial project. Use at your own risk.
+        
+        Instaloader is licensed under an MIT license. Refer to ``LICENSE`` file for more information.
+        
+        .. disclaimer-end
+        
 Keywords: instagram,instagram-scraper,instagram-client,instagram-feed,downloader,videos,photos,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-stories
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,168 +175,7 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.6
-License-File: LICENSE
-License-File: AUTHORS.md
-
-.. image:: https://raw.githubusercontent.com/instaloader/instaloader/master/docs/logo_heading.png
-
-.. badges-start
-
-|travis| |pypi| |pyversion| |license| |aur| |contributors| |downloads|
-
-.. |travis| image:: https://img.shields.io/travis/instaloader/instaloader/master.svg
-   :alt: Travis-CI Build Status
-   :target: https://travis-ci.org/instaloader/instaloader
-
-.. |pypi| image:: https://img.shields.io/pypi/v/instaloader.svg
-   :alt: Instaloader PyPI Project Page
-   :target: https://pypi.org/project/instaloader/
-
-.. |license| image:: https://img.shields.io/github/license/instaloader/instaloader.svg
-   :alt: MIT License
-   :target: https://github.com/instaloader/instaloader/blob/master/LICENSE
-
-.. |pyversion| image:: https://img.shields.io/pypi/pyversions/instaloader.svg
-   :alt: Supported Python Versions
-
-.. |contributors| image:: https://img.shields.io/github/contributors/instaloader/instaloader.svg
-   :alt: Contributor Count
-   :target: https://github.com/instaloader/instaloader/graphs/contributors
-
-.. |aur| image:: https://img.shields.io/aur/version/instaloader.svg
-   :alt: Arch User Repository Package
-   :target: https://aur.archlinux.org/packages/instaloader/
-
-.. |downloads| image:: https://pepy.tech/badge/instaloader/month
-   :alt: PyPI Download Count
-   :target: https://pepy.tech/project/instaloader
-
-.. badges-end
-
-::
-
-    $ pip3 install instaloader
-
-    $ instaloader profile [profile ...]
-
-**Instaloader**
-
-- downloads **public and private profiles, hashtags, user stories,
-  feeds and saved media**,
-
-- downloads **comments, geotags and captions** of each post,
-
-- automatically **detects profile name changes** and renames the target
-  directory accordingly,
-
-- allows **fine-grained customization** of filters and where to store
-  downloaded media,
-
-- automatically **resumes previously-interrupted** download iterations.
-
-::
-
-    instaloader [--comments] [--geotags]
-                [--stories] [--highlights] [--tagged] [--igtv]
-                [--login YOUR-USERNAME] [--fast-update]
-                profile | "#hashtag" | :stories | :feed | :saved
-
-`Instaloader Documentation <https://instaloader.github.io/>`__
-
-
-How to Automatically Download Pictures from Instagram
------------------------------------------------------
-
-To **download all pictures and videos of a profile**, as well as the
-**profile picture**, do
-
-::
-
-    instaloader profile [profile ...]
-
-where ``profile`` is the name of a profile you want to download. Instead
-of only one profile, you may also specify a list of profiles.
-
-To later **update your local copy** of that profiles, you may run
-
-::
-
-    instaloader --fast-update profile [profile ...]
-
-If ``--fast-update`` is given, Instaloader stops when arriving at the
-first already-downloaded picture.
-
-Alternatively, you can use ``--latest-stamps`` to have Instaloader store
-the time each profile was last downloaded and only download newer media:
-
-::
-
-    instaloader --latest-stamps -- profile [profile ...]
-
-With this option it's possible to move or delete downloaded media and still keep
-the archive updated.
-
-When updating profiles, Instaloader
-automatically **detects profile name changes** and renames the target directory
-accordingly.
-
-Instaloader can also be used to **download private profiles**. To do so,
-invoke it with
-
-::
-
-    instaloader --login=your_username profile [profile ...]
-
-When logging in, Instaloader **stores the session cookies** in a file in your
-temporary directory, which will be reused later the next time ``--login``
-is given.  So you can download private profiles **non-interactively** when you
-already have a valid session cookie file.
-
-`Instaloader Documentation <https://instaloader.github.io/basic-usage.html>`__
-
-Contributing
-------------
-
-As an open source project, Instaloader heavily depends on the contributions from
-its community. See
-`contributing <https://instaloader.github.io/contributing.html>`__
-for how you may help Instaloader to become an even greater tool.
-
-Supporters
-----------
-
-.. current-sponsors-start
-
-See `Alex' GitHub Sponsors <https://github.com/sponsors/aandergr>`__ page for
-how you can sponsor the development of Instaloader!
-
-.. current-sponsors-end
-
-It is a pleasure for us to share our Instaloader to the world, and we are proud
-to have attracted such an active and motivating community, with so many users
-who share their suggestions and ideas with us. Buying a community-sponsored beer
-or coffee from time to time is very likely to further raise our passion for the
-development of Instaloader.
-
-| For Donations, we provide GitHub Sponsors page, a PayPal.Me link and a Bitcoin address.
-|  GitHub Sponsors: `Sponsor @aandergr on GitHub Sponsors <https://github.com/sponsors/aandergr>`__
-|  PayPal: `PayPal.me/aandergr <https://www.paypal.me/aandergr>`__
-|  BTC: 1Nst4LoadeYzrKjJ1DX9CpbLXBYE9RKLwY
-
-Disclaimer
-----------
-
-.. disclaimer-start
-
-Instaloader is in no way affiliated with, authorized, maintained or endorsed by Instagram or any of its affiliates or
-subsidiaries. This is an independent and unofficial project. Use at your own risk.
-
-Instaloader is licensed under an MIT license. Refer to ``LICENSE`` file for more information.
-
-.. disclaimer-end
-
-
```

### Comparing `instaloader-4.9b2/instaloader.egg-info/SOURCES.txt` & `instaloader-4.9b3/instaloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `instaloader-4.9b2/instaloader.egg-info/PKG-INFO` & `instaloader-4.9b3/instaloader.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,172 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: instaloader
-Version: 4.9b2
+Version: 4.9b3
 Summary: Download pictures (or videos) along with their captions and other metadata from Instagram.
 Home-page: https://instaloader.github.io/
 Author: Alexander Graf, André Koch-Kramer
 Author-email: mail@agraf.me, koch-kramer@web.de
 License: MIT
+Description: .. image:: https://raw.githubusercontent.com/instaloader/instaloader/master/docs/logo_heading.png
+        
+        .. badges-start
+        
+        |travis| |pypi| |pyversion| |license| |aur| |contributors| |downloads|
+        
+        .. |travis| image:: https://img.shields.io/travis/instaloader/instaloader/master.svg
+           :alt: Travis-CI Build Status
+           :target: https://travis-ci.org/instaloader/instaloader
+        
+        .. |pypi| image:: https://img.shields.io/pypi/v/instaloader.svg
+           :alt: Instaloader PyPI Project Page
+           :target: https://pypi.org/project/instaloader/
+        
+        .. |license| image:: https://img.shields.io/github/license/instaloader/instaloader.svg
+           :alt: MIT License
+           :target: https://github.com/instaloader/instaloader/blob/master/LICENSE
+        
+        .. |pyversion| image:: https://img.shields.io/pypi/pyversions/instaloader.svg
+           :alt: Supported Python Versions
+        
+        .. |contributors| image:: https://img.shields.io/github/contributors/instaloader/instaloader.svg
+           :alt: Contributor Count
+           :target: https://github.com/instaloader/instaloader/graphs/contributors
+        
+        .. |aur| image:: https://img.shields.io/aur/version/instaloader.svg
+           :alt: Arch User Repository Package
+           :target: https://aur.archlinux.org/packages/instaloader/
+        
+        .. |downloads| image:: https://pepy.tech/badge/instaloader/month
+           :alt: PyPI Download Count
+           :target: https://pepy.tech/project/instaloader
+        
+        .. badges-end
+        
+        ::
+        
+            $ pip3 install instaloader
+        
+            $ instaloader profile [profile ...]
+        
+        **Instaloader**
+        
+        - downloads **public and private profiles, hashtags, user stories,
+          feeds and saved media**,
+        
+        - downloads **comments, geotags and captions** of each post,
+        
+        - automatically **detects profile name changes** and renames the target
+          directory accordingly,
+        
+        - allows **fine-grained customization** of filters and where to store
+          downloaded media,
+        
+        - automatically **resumes previously-interrupted** download iterations.
+        
+        ::
+        
+            instaloader [--comments] [--geotags]
+                        [--stories] [--highlights] [--tagged] [--igtv]
+                        [--login YOUR-USERNAME] [--fast-update]
+                        profile | "#hashtag" | :stories | :feed | :saved
+        
+        `Instaloader Documentation <https://instaloader.github.io/>`__
+        
+        
+        How to Automatically Download Pictures from Instagram
+        -----------------------------------------------------
+        
+        To **download all pictures and videos of a profile**, as well as the
+        **profile picture**, do
+        
+        ::
+        
+            instaloader profile [profile ...]
+        
+        where ``profile`` is the name of a profile you want to download. Instead
+        of only one profile, you may also specify a list of profiles.
+        
+        To later **update your local copy** of that profiles, you may run
+        
+        ::
+        
+            instaloader --fast-update profile [profile ...]
+        
+        If ``--fast-update`` is given, Instaloader stops when arriving at the
+        first already-downloaded picture.
+        
+        Alternatively, you can use ``--latest-stamps`` to have Instaloader store
+        the time each profile was last downloaded and only download newer media:
+        
+        ::
+        
+            instaloader --latest-stamps -- profile [profile ...]
+        
+        With this option it's possible to move or delete downloaded media and still keep
+        the archive updated.
+        
+        When updating profiles, Instaloader
+        automatically **detects profile name changes** and renames the target directory
+        accordingly.
+        
+        Instaloader can also be used to **download private profiles**. To do so,
+        invoke it with
+        
+        ::
+        
+            instaloader --login=your_username profile [profile ...]
+        
+        When logging in, Instaloader **stores the session cookies** in a file in your
+        temporary directory, which will be reused later the next time ``--login``
+        is given.  So you can download private profiles **non-interactively** when you
+        already have a valid session cookie file.
+        
+        `Instaloader Documentation <https://instaloader.github.io/basic-usage.html>`__
+        
+        Contributing
+        ------------
+        
+        As an open source project, Instaloader heavily depends on the contributions from
+        its community. See
+        `contributing <https://instaloader.github.io/contributing.html>`__
+        for how you may help Instaloader to become an even greater tool.
+        
+        Supporters
+        ----------
+        
+        .. current-sponsors-start
+        
+        See `Alex' GitHub Sponsors <https://github.com/sponsors/aandergr>`__ page for
+        how you can sponsor the development of Instaloader!
+        
+        .. current-sponsors-end
+        
+        It is a pleasure for us to share our Instaloader to the world, and we are proud
+        to have attracted such an active and motivating community, with so many users
+        who share their suggestions and ideas with us. Buying a community-sponsored beer
+        or coffee from time to time is very likely to further raise our passion for the
+        development of Instaloader.
+        
+        | For Donations, we provide GitHub Sponsors page, a PayPal.Me link and a Bitcoin address.
+        |  GitHub Sponsors: `Sponsor @aandergr on GitHub Sponsors <https://github.com/sponsors/aandergr>`__
+        |  PayPal: `PayPal.me/aandergr <https://www.paypal.me/aandergr>`__
+        |  BTC: 1Nst4LoadeYzrKjJ1DX9CpbLXBYE9RKLwY
+        
+        Disclaimer
+        ----------
+        
+        .. disclaimer-start
+        
+        Instaloader is in no way affiliated with, authorized, maintained or endorsed by Instagram or any of its affiliates or
+        subsidiaries. This is an independent and unofficial project. Use at your own risk.
+        
+        Instaloader is licensed under an MIT license. Refer to ``LICENSE`` file for more information.
+        
+        .. disclaimer-end
+        
 Keywords: instagram,instagram-scraper,instagram-client,instagram-feed,downloader,videos,photos,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-stories
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,168 +175,7 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.6
-License-File: LICENSE
-License-File: AUTHORS.md
-
-.. image:: https://raw.githubusercontent.com/instaloader/instaloader/master/docs/logo_heading.png
-
-.. badges-start
-
-|travis| |pypi| |pyversion| |license| |aur| |contributors| |downloads|
-
-.. |travis| image:: https://img.shields.io/travis/instaloader/instaloader/master.svg
-   :alt: Travis-CI Build Status
-   :target: https://travis-ci.org/instaloader/instaloader
-
-.. |pypi| image:: https://img.shields.io/pypi/v/instaloader.svg
-   :alt: Instaloader PyPI Project Page
-   :target: https://pypi.org/project/instaloader/
-
-.. |license| image:: https://img.shields.io/github/license/instaloader/instaloader.svg
-   :alt: MIT License
-   :target: https://github.com/instaloader/instaloader/blob/master/LICENSE
-
-.. |pyversion| image:: https://img.shields.io/pypi/pyversions/instaloader.svg
-   :alt: Supported Python Versions
-
-.. |contributors| image:: https://img.shields.io/github/contributors/instaloader/instaloader.svg
-   :alt: Contributor Count
-   :target: https://github.com/instaloader/instaloader/graphs/contributors
-
-.. |aur| image:: https://img.shields.io/aur/version/instaloader.svg
-   :alt: Arch User Repository Package
-   :target: https://aur.archlinux.org/packages/instaloader/
-
-.. |downloads| image:: https://pepy.tech/badge/instaloader/month
-   :alt: PyPI Download Count
-   :target: https://pepy.tech/project/instaloader
-
-.. badges-end
-
-::
-
-    $ pip3 install instaloader
-
-    $ instaloader profile [profile ...]
-
-**Instaloader**
-
-- downloads **public and private profiles, hashtags, user stories,
-  feeds and saved media**,
-
-- downloads **comments, geotags and captions** of each post,
-
-- automatically **detects profile name changes** and renames the target
-  directory accordingly,
-
-- allows **fine-grained customization** of filters and where to store
-  downloaded media,
-
-- automatically **resumes previously-interrupted** download iterations.
-
-::
-
-    instaloader [--comments] [--geotags]
-                [--stories] [--highlights] [--tagged] [--igtv]
-                [--login YOUR-USERNAME] [--fast-update]
-                profile | "#hashtag" | :stories | :feed | :saved
-
-`Instaloader Documentation <https://instaloader.github.io/>`__
-
-
-How to Automatically Download Pictures from Instagram
------------------------------------------------------
-
-To **download all pictures and videos of a profile**, as well as the
-**profile picture**, do
-
-::
-
-    instaloader profile [profile ...]
-
-where ``profile`` is the name of a profile you want to download. Instead
-of only one profile, you may also specify a list of profiles.
-
-To later **update your local copy** of that profiles, you may run
-
-::
-
-    instaloader --fast-update profile [profile ...]
-
-If ``--fast-update`` is given, Instaloader stops when arriving at the
-first already-downloaded picture.
-
-Alternatively, you can use ``--latest-stamps`` to have Instaloader store
-the time each profile was last downloaded and only download newer media:
-
-::
-
-    instaloader --latest-stamps -- profile [profile ...]
-
-With this option it's possible to move or delete downloaded media and still keep
-the archive updated.
-
-When updating profiles, Instaloader
-automatically **detects profile name changes** and renames the target directory
-accordingly.
-
-Instaloader can also be used to **download private profiles**. To do so,
-invoke it with
-
-::
-
-    instaloader --login=your_username profile [profile ...]
-
-When logging in, Instaloader **stores the session cookies** in a file in your
-temporary directory, which will be reused later the next time ``--login``
-is given.  So you can download private profiles **non-interactively** when you
-already have a valid session cookie file.
-
-`Instaloader Documentation <https://instaloader.github.io/basic-usage.html>`__
-
-Contributing
-------------
-
-As an open source project, Instaloader heavily depends on the contributions from
-its community. See
-`contributing <https://instaloader.github.io/contributing.html>`__
-for how you may help Instaloader to become an even greater tool.
-
-Supporters
-----------
-
-.. current-sponsors-start
-
-See `Alex' GitHub Sponsors <https://github.com/sponsors/aandergr>`__ page for
-how you can sponsor the development of Instaloader!
-
-.. current-sponsors-end
-
-It is a pleasure for us to share our Instaloader to the world, and we are proud
-to have attracted such an active and motivating community, with so many users
-who share their suggestions and ideas with us. Buying a community-sponsored beer
-or coffee from time to time is very likely to further raise our passion for the
-development of Instaloader.
-
-| For Donations, we provide GitHub Sponsors page, a PayPal.Me link and a Bitcoin address.
-|  GitHub Sponsors: `Sponsor @aandergr on GitHub Sponsors <https://github.com/sponsors/aandergr>`__
-|  PayPal: `PayPal.me/aandergr <https://www.paypal.me/aandergr>`__
-|  BTC: 1Nst4LoadeYzrKjJ1DX9CpbLXBYE9RKLwY
-
-Disclaimer
-----------
-
-.. disclaimer-start
-
-Instaloader is in no way affiliated with, authorized, maintained or endorsed by Instagram or any of its affiliates or
-subsidiaries. This is an independent and unofficial project. Use at your own risk.
-
-Instaloader is licensed under an MIT license. Refer to ``LICENSE`` file for more information.
-
-.. disclaimer-end
-
-
```

### Comparing `instaloader-4.9b2/LICENSE` & `instaloader-4.9b3/LICENSE`

 * *Files identical despite different names*

### Comparing `instaloader-4.9b2/instaloader/__main__.py` & `instaloader-4.9b3/instaloader/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,14 +379,17 @@
                        help='Prefix of filenames for profile pics, hashtag profile pics, and highlight covers. '
                             'Defaults to \'{date_utc}_UTC_{typename}\' if --dirname-pattern contains \'{target}\' '
                             'or \'{dirname}\', or if --dirname-pattern is not specified. Otherwise defaults to '
                             '\'{target}_{date_utc}_UTC_{typename}\'.')
     g_how.add_argument('--resume-prefix', metavar='PREFIX',
                        help='Prefix for filenames that are used to save the information to resume an interrupted '
                             'download.')
+    g_how.add_argument('--sanitize-paths', action='store_true',
+                       help='Sanitize paths so that the resulting file and directory names are valid on both '
+                            'Windows and Unix.')
     g_how.add_argument('--no-resume', action='store_true',
                        help='Do not resume a previously-aborted download iteration, and do not save such information '
                             'when interrupted.')
     g_how.add_argument('--use-aged-resume-files', action='store_true', help=SUPPRESS)
     g_how.add_argument('--user-agent',
                        help='User Agent to use for HTTP requests. Defaults to \'{}\'.'.format(default_user_agent()))
     g_how.add_argument('-S', '--no-sleep', action='store_true', help=SUPPRESS)
@@ -459,15 +462,16 @@
                              max_connection_attempts=args.max_connection_attempts,
                              request_timeout=args.request_timeout,
                              resume_prefix=resume_prefix,
                              check_resume_bbd=not args.use_aged_resume_files,
                              slide=args.slide,
                              fatal_status_codes=args.abort_on,
                              iphone_support=not args.no_iphone,
-                             title_pattern=args.title_pattern)
+                             title_pattern=args.title_pattern,
+                             sanitize_paths=args.sanitize_paths)
         _main(loader,
               args.profile,
               username=args.login.lower() if args.login is not None else None,
               password=args.password,
               sessionfile=args.sessionfile,
               download_profile_pic=download_profile_pic,
               download_posts=download_posts,
```

### Comparing `instaloader-4.9b2/instaloader/sectioniterator.py` & `instaloader-4.9b3/instaloader/sectioniterator.py`

 * *Files identical despite different names*

### Comparing `instaloader-4.9b2/instaloader/nodeiterator.py` & `instaloader-4.9b3/instaloader/nodeiterator.py`

 * *Files identical despite different names*

### Comparing `instaloader-4.9b2/instaloader/instaloader.py` & `instaloader-4.9b3/instaloader/instaloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,32 +133,46 @@
             return super().format_field(value, '%Y-%m-%d_%H-%M-%S')
         if value is None:
             return ''
         return super().format_field(value, format_spec)
 
 
 class _PostPathFormatter(_ArbitraryItemFormatter):
+    RESERVED: set = {'CON', 'PRN', 'AUX', 'NUL',
+                     'COM1', 'COM2', 'COM3', 'COM4', 'COM5', 'COM6', 'COM7', 'COM8', 'COM9',
+                     'LPT1', 'LPT2', 'LPT3', 'LPT4', 'LPT5', 'LPT6', 'LPT7', 'LPT8', 'LPT9'}
+
+    def __init__(self, item: Any, force_windows_path: bool = False):
+        super().__init__(item)
+        self.force_windows_path = force_windows_path
+
     def get_value(self, key, args, kwargs):
         ret = super().get_value(key, args, kwargs)
         if not isinstance(ret, str):
             return ret
-        return self.sanitize_path(ret)
+        return self.sanitize_path(ret, self.force_windows_path)
 
     @staticmethod
-    def sanitize_path(ret: str) -> str:
+    def sanitize_path(ret: str, force_windows_path: bool = False) -> str:
         """Replaces '/' with similar looking Division Slash and some other illegal filename characters on Windows."""
         ret = ret.replace('/', '\u2215')
 
         if ret.startswith('.'):
             ret = ret.replace('.', '\u2024', 1)
 
-        if platform.system() == 'Windows':
+        if force_windows_path or platform.system() == 'Windows':
             ret = ret.replace(':', '\uff1a').replace('<', '\ufe64').replace('>', '\ufe65').replace('\"', '\uff02')
             ret = ret.replace('\\', '\ufe68').replace('|', '\uff5c').replace('?', '\ufe16').replace('*', '\uff0a')
             ret = ret.replace('\n', ' ').replace('\r', ' ')
+            root, ext = os.path.splitext(ret)
+            if root.upper() in _PostPathFormatter.RESERVED:
+                root += '_'
+            if ext == '.':
+                ext = '\u2024'
+            ret = root + ext
         return ret
 
 
 class Instaloader:
     """Instaloader Class.
 
     :param quiet: :option:`--quiet`
@@ -183,14 +197,15 @@
     :param request_timeout: :option:`--request-timeout`, set per-request timeout (seconds)
     :param rate_controller: Generator for a :class:`RateController` to override rate controlling behavior
     :param resume_prefix: :option:`--resume-prefix`, or None for :option:`--no-resume`.
     :param check_resume_bbd: Whether to check the date of expiry of resume files and reject them if expired.
     :param slide: :option:`--slide`
     :param fatal_status_codes: :option:`--abort-on`
     :param iphone_support: not :option:`--no-iphone`
+    :param sanitize_paths: :option:`--sanitize-paths`
 
     .. attribute:: context
 
        The associated :class:`InstaloaderContext` with low-level communication functions and logging.
     """
 
     def __init__(self,
@@ -212,15 +227,16 @@
                  request_timeout: float = 300.0,
                  rate_controller: Optional[Callable[[InstaloaderContext], RateController]] = None,
                  resume_prefix: Optional[str] = "iterator",
                  check_resume_bbd: bool = True,
                  slide: Optional[str] = None,
                  fatal_status_codes: Optional[List[int]] = None,
                  iphone_support: bool = True,
-                 title_pattern: Optional[str] = None):
+                 title_pattern: Optional[str] = None,
+                 sanitize_paths: bool = False):
 
         self.context = InstaloaderContext(sleep, quiet, user_agent, max_connection_attempts,
                                           request_timeout, rate_controller, fatal_status_codes,
                                           iphone_support)
 
         # configuration parameters
         self.dirname_pattern = dirname_pattern or "{target}"
@@ -229,14 +245,15 @@
             self.title_pattern = title_pattern
         else:
             if (format_string_contains_key(self.dirname_pattern, 'profile') or
                 format_string_contains_key(self.dirname_pattern, 'target')):
                 self.title_pattern = '{date_utc}_UTC_{typename}'
             else:
                 self.title_pattern = '{target}_{date_utc}_UTC_{typename}'
+        self.sanitize_paths = sanitize_paths
         self.download_pictures = download_pictures
         self.download_videos = download_videos
         self.download_video_thumbnails = download_video_thumbnails
         self.download_geotags = download_geotags
         self.download_comments = download_comments
         self.save_metadata = save_metadata
         self.compress_json = compress_json
@@ -292,15 +309,16 @@
             storyitem_metadata_txt_pattern=self.storyitem_metadata_txt_pattern,
             max_connection_attempts=self.context.max_connection_attempts,
             request_timeout=self.context.request_timeout,
             resume_prefix=self.resume_prefix,
             check_resume_bbd=self.check_resume_bbd,
             slide=self.slide,
             fatal_status_codes=self.context.fatal_status_codes,
-            iphone_support=self.context.iphone_support)
+            iphone_support=self.context.iphone_support,
+            sanitize_paths=self.sanitize_paths)
         yield new_loader
         self.context.error_log.extend(new_loader.context.error_log)
         new_loader.context.error_log = []  # avoid double-printing of errors
         new_loader.close()
 
     def close(self):
         """Close associated session objects and repeat error log."""
@@ -313,23 +331,33 @@
         self.close()
 
     @_retry_on_connection_error
     def download_pic(self, filename: str, url: str, mtime: datetime,
                      filename_suffix: Optional[str] = None, _attempt: int = 1) -> bool:
         """Downloads and saves picture with given url under given directory with given timestamp.
         Returns true, if file was actually downloaded, i.e. updated."""
-        urlmatch = re.search('\\.[a-z0-9]*\\?', url)
-        file_extension = url[-3:] if urlmatch is None else urlmatch.group(0)[1:-1]
         if filename_suffix is not None:
             filename += '_' + filename_suffix
-        filename += '.' + file_extension
-        if os.path.isfile(filename):
+        urlmatch = re.search('\\.[a-z0-9]*\\?', url)
+        file_extension = url[-3:] if urlmatch is None else urlmatch.group(0)[1:-1]
+        nominal_filename = filename + '.' + file_extension
+        if os.path.isfile(nominal_filename):
+            self.context.log(nominal_filename + ' exists', end=' ', flush=True)
+            return False
+        resp = self.context.get_raw(url)
+        if 'Content-Type' in resp.headers and resp.headers['Content-Type']:
+            header_extension = '.' + resp.headers['Content-Type'].split(';')[0].split('/')[-1]
+            header_extension = header_extension.lower().replace('jpeg', 'jpg')
+            filename += header_extension
+        else:
+            filename = nominal_filename
+        if filename != nominal_filename and os.path.isfile(filename):
             self.context.log(filename + ' exists', end=' ', flush=True)
             return False
-        self.context.get_and_write_raw(url, filename)
+        self.context.write_raw(resp, filename)
         os.utime(filename, (datetime.now().timestamp(), mtime.timestamp()))
         return True
 
     def save_metadata_json(self, filename: str, structure: JsonExportable) -> None:
         """Saves metadata JSON file of a structure."""
         if self.compress_json:
             filename += '.json.xz'
@@ -502,17 +530,18 @@
             date_object = datetime.strptime(http_response.headers["Last-Modified"], '%a, %d %b %Y %H:%M:%S GMT')
             date_object = date_object.replace(tzinfo=timezone.utc)
             pic_bytes = None
         else:
             pic_bytes = http_response.content
         ig_filename = url.split('/')[-1].split('?')[0]
         pic_data = TitlePic(owner_profile, target, name_suffix, ig_filename, date_object)
-        dirname = _PostPathFormatter(pic_data).format(self.dirname_pattern, target=target)
-        filename_template = os.path.join(dirname,
-                                         _PostPathFormatter(pic_data).format(self.title_pattern, target=target))
+        dirname = _PostPathFormatter(pic_data, self.sanitize_paths).format(self.dirname_pattern, target=target)
+        filename_template = os.path.join(
+                dirname,
+                _PostPathFormatter(pic_data, self.sanitize_paths).format(self.title_pattern, target=target))
         filename = self.__prepare_filename(filename_template, lambda: url) + ".jpg"
         content_length = http_response.headers.get('Content-Length', None)
         if os.path.isfile(filename) and (not self.context.is_logged_in or
                                          (content_length is not None and
                                           os.path.getsize(filename) >= int(content_length))):
             self.context.log(filename + ' already exists')
             return
@@ -629,15 +658,15 @@
         return filename
 
     def format_filename(self, item: Union[Post, StoryItem, PostSidecarNode, TitlePic],
                         target: Optional[Union[str, Path]] = None):
         """Format filename of a :class:`Post` or :class:`StoryItem` according to ``filename-pattern`` parameter.
 
         .. versionadded:: 4.1"""
-        return _PostPathFormatter(item).format(self.filename_pattern, target=target)
+        return _PostPathFormatter(item, self.sanitize_paths).format(self.filename_pattern, target=target)
 
     def download_post(self, post: Post, target: Union[str, Path]) -> bool:
         """
         Download everything associated with one instagram post node, i.e. picture, caption and video.
 
         :param post: Post to download.
         :param target: Target name, i.e. profile name, #hashtag, :feed; for filename.
@@ -661,15 +690,15 @@
                     if not _already_downloaded("{0}_{1}.jpg".format(path_base, idx)):
                         return False
                 if is_video and self.download_videos:
                     if not _already_downloaded("{0}_{1}.mp4".format(path_base, idx)):
                         return False
             return True
 
-        dirname = _PostPathFormatter(post).format(self.dirname_pattern, target=target)
+        dirname = _PostPathFormatter(post, self.sanitize_paths).format(self.dirname_pattern, target=target)
         filename_template = os.path.join(dirname, self.format_filename(post, target=target))
         filename = self.__prepare_filename(filename_template, lambda: post.url)
 
         # Download the image(s) / video thumbnail and videos within sidecars if desired
         downloaded = True
         if post.typename == 'GraphSidecar':
             if self.download_pictures or self.download_videos:
@@ -842,15 +871,15 @@
             if not os.path.isfile(path):
                 return False
             else:
                 self.context.log(path + ' exists', end=' ', flush=True)
                 return True
 
         date_local = item.date_local
-        dirname = _PostPathFormatter(item).format(self.dirname_pattern, target=target)
+        dirname = _PostPathFormatter(item, self.sanitize_paths).format(self.dirname_pattern, target=target)
         filename_template = os.path.join(dirname, self.format_filename(item, target=target))
         filename = self.__prepare_filename(filename_template, lambda: item.url)
         downloaded = False
         if not item.is_video or self.download_video_thumbnails is True:
             downloaded = (not _already_downloaded(filename + ".jpg") and
                           self.download_pic(filename=filename, url=item.url, mtime=date_local))
         if item.is_video and self.download_videos is True:
@@ -910,16 +939,17 @@
         :param storyitem_filter: function(storyitem), which returns True if given StoryItem should be downloaded
         :raises LoginRequiredException: If called without being logged in.
         """
         for user_highlight in self.get_highlights(user):
             name = user_highlight.owner_username
             highlight_target = (filename_target
                                 if filename_target
-                                else (Path(_PostPathFormatter.sanitize_path(name)) /
-                                      _PostPathFormatter.sanitize_path(user_highlight.title)))  # type: Union[str, Path]
+                                else (Path(_PostPathFormatter.sanitize_path(name, self.sanitize_paths)) /
+                                      _PostPathFormatter.sanitize_path(user_highlight.title,
+                                                                       self.sanitize_paths)))  # type: Union[str, Path]
             self.context.log("Retrieving highlights \"{}\" from profile {}".format(user_highlight.title, name))
             self.download_highlight_cover(user_highlight, highlight_target)
             totalcount = user_highlight.itemcount
             count = 1
             for item in user_highlight.get_items():
                 if storyitem_filter is not None and not storyitem_filter(item):
                     self.context.log("<{} skipped>".format(item), flush=True)
@@ -961,15 +991,15 @@
         :param owner_profile: Associated profile, if any.
         :param takewhile: Expression evaluated for each post. Once it returns false, downloading stops.
         """
         displayed_count = (max_count if total_count is None or max_count is not None and max_count < total_count
                            else total_count)
         sanitized_target = target
         if isinstance(target, str):
-            sanitized_target = _PostPathFormatter.sanitize_path(target)
+            sanitized_target = _PostPathFormatter.sanitize_path(target, self.sanitize_paths)
         if takewhile is None:
             takewhile = lambda _: True
         with resumable_iteration(
                 context=self.context,
                 iterator=posts,
                 load=load_structure_from_file,
                 save=save_structure_to_file,
@@ -1205,16 +1235,16 @@
         posts_takewhile: Optional[Callable[[Post], bool]] = None
         if latest_stamps is not None:
             last_scraped = latest_stamps.get_last_tagged_timestamp(profile.username)
             posts_takewhile = lambda p: p.date_local > last_scraped
         tagged_posts = profile.get_tagged_posts()
         self.posts_download_loop(tagged_posts,
                                  target if target
-                                 else (Path(_PostPathFormatter.sanitize_path(profile.username)) /
-                                       _PostPathFormatter.sanitize_path(':tagged')),
+                                 else (Path(_PostPathFormatter.sanitize_path(profile.username, self.sanitize_paths)) /
+                                       _PostPathFormatter.sanitize_path(':tagged', self.sanitize_paths)),
                                  fast_update, post_filter, takewhile=posts_takewhile)
         if latest_stamps is not None and tagged_posts.first_item is not None:
             latest_stamps.set_last_tagged_timestamp(profile.username, tagged_posts.first_item.date_local)
 
     def download_igtv(self, profile: Profile, fast_update: bool = False,
                       post_filter: Optional[Callable[[Post], bool]] = None,
                       latest_stamps: Optional[LatestStamps] = None) -> None:
```

### Comparing `instaloader-4.9b2/instaloader/lateststamps.py` & `instaloader-4.9b3/instaloader/lateststamps.py`

 * *Files identical despite different names*

### Comparing `instaloader-4.9b2/instaloader/structures.py` & `instaloader-4.9b3/instaloader/structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from base64 import b64decode, b64encode
 from collections import namedtuple
 from contextlib import suppress
 from datetime import datetime
 from itertools import islice
 from pathlib import Path
 from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple, Union
+from unicodedata import normalize
 
 from . import __version__
 from .exceptions import *
 from .instaloadercontext import InstaloaderContext
 from .nodeiterator import FrozenNodeIterator, NodeIterator
 from .sectioniterator import SectionIterator
 
@@ -361,17 +362,17 @@
                     yield PostSidecarNode(is_video=is_video, display_url=display_url,
                                           video_url=node['video_url'] if is_video else None)
 
     @property
     def caption(self) -> Optional[str]:
         """Caption."""
         if "edge_media_to_caption" in self._node and self._node["edge_media_to_caption"]["edges"]:
-            return self._node["edge_media_to_caption"]["edges"][0]["node"]["text"]
+            return normalize("NFC", self._node["edge_media_to_caption"]["edges"][0]["node"]["text"])
         elif "caption" in self._node:
-            return self._node["caption"]
+            return normalize("NFC", self._node["caption"])
         return None
 
     @property
     def caption_hashtags(self) -> List[str]:
         """List of all lowercased hashtags (without preceeding #) that occur in the Post's caption."""
         if not self.caption:
             return []
@@ -385,15 +386,15 @@
         """List of all lowercased profiles that are mentioned in the Post's caption, without preceeding @."""
         if not self.caption:
             return []
         # This regular expression is modified from jStassen, adjusted to use Python's \w to
         # support Unicode and a word/beginning of string delimiter at the beginning to ensure
         # that no email addresses join the list of mentions.
         # http://blog.jstassen.com/2016/03/code-regex-for-instagram-username-and-hashtags/
-        mention_regex = re.compile(r"(?:^|\W|_)(?:@)(\w(?:(?:\w|(?:\.(?!\.))){0,28}(?:\w))?)")
+        mention_regex = re.compile(r"(?:^|\W|_)(?:@)(\w(?:(?:\w|(?:\.(?!\.))){0,28}(?:\w))?)", re.ASCII)
         return re.findall(mention_regex, self.caption.lower())
 
     @property
     def pcaption(self) -> str:
         """Printable caption, useful as a format specifier for --filename-pattern.
 
         .. versionadded:: 4.2.6"""
```

### Comparing `instaloader-4.9b2/instaloader/exceptions.py` & `instaloader-4.9b3/instaloader/exceptions.py`

 * *Files identical despite different names*

### Comparing `instaloader-4.9b2/instaloader/__init__.py` & `instaloader-4.9b3/instaloader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Download pictures (or videos) along with their captions and other metadata from Instagram."""
 
 
-__version__ = '4.9b2'
+__version__ = '4.9b3'
 
 
 try:
     # pylint:disable=wrong-import-position
     import win_unicode_console  # type: ignore
 except ImportError:
     pass
```

### Comparing `instaloader-4.9b2/instaloader/instaloadercontext.py` & `instaloader-4.9b3/instaloader/instaloadercontext.py`

 * *Files identical despite different names*

