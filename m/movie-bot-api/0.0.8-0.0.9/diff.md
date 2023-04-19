# Comparing `tmp/movie-bot-api-0.0.8.tar.gz` & `tmp/movie-bot-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movie-bot-api-0.0.8.tar", last modified: Fri Nov 11 12:35:04 2022, max compression
+gzip compressed data, was "movie-bot-api-0.0.9.tar", last modified: Fri Nov 11 14:03:44 2022, max compression
```

## Comparing `movie-bot-api-0.0.8.tar` & `movie-bot-api-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 yee        (501) staff       (20)        0 2022-11-11 12:35:04.750544 movie-bot-api-0.0.8/
--rw-r--r--   0 yee        (501) staff       (20)     1066 2022-11-11 01:25:56.000000 movie-bot-api-0.0.8/LICENSE
--rw-r--r--   0 yee        (501) staff       (20)       40 2022-11-11 12:12:15.000000 movie-bot-api-0.0.8/MANIFEST.in
--rw-r--r--   0 yee        (501) staff       (20)      404 2022-11-11 12:35:04.750411 movie-bot-api-0.0.8/PKG-INFO
--rw-r--r--   0 yee        (501) staff       (20)       42 2022-11-11 01:25:56.000000 movie-bot-api-0.0.8/README.md
-drwxr-xr-x   0 yee        (501) staff       (20)        0 2022-11-11 12:35:04.747280 movie-bot-api-0.0.8/movie_bot_api.egg-info/
--rw-r--r--   0 yee        (501) staff       (20)      404 2022-11-11 12:35:04.000000 movie-bot-api-0.0.8/movie_bot_api.egg-info/PKG-INFO
--rw-r--r--   0 yee        (501) staff       (20)      604 2022-11-11 12:35:04.000000 movie-bot-api-0.0.8/movie_bot_api.egg-info/SOURCES.txt
--rw-r--r--   0 yee        (501) staff       (20)        1 2022-11-11 12:35:04.000000 movie-bot-api-0.0.8/movie_bot_api.egg-info/dependency_links.txt
--rw-r--r--   0 yee        (501) staff       (20)       36 2022-11-11 12:35:04.000000 movie-bot-api-0.0.8/movie_bot_api.egg-info/requires.txt
--rw-r--r--   0 yee        (501) staff       (20)       12 2022-11-11 12:35:04.000000 movie-bot-api-0.0.8/movie_bot_api.egg-info/top_level.txt
-drwxr-xr-x   0 yee        (501) staff       (20)        0 2022-11-11 12:35:04.748743 movie-bot-api-0.0.8/moviebotapi/
--rw-r--r--   0 yee        (501) staff       (20)      835 2022-11-11 12:12:15.000000 movie-bot-api-0.0.8/moviebotapi/__init__.py
-drwxr-xr-x   0 yee        (501) staff       (20)        0 2022-11-11 12:35:04.750119 movie-bot-api-0.0.8/moviebotapi/core/
--rw-r--r--   0 yee        (501) staff       (20)        0 2022-11-11 01:25:56.000000 movie-bot-api-0.0.8/moviebotapi/core/__init__.py
--rw-r--r--   0 yee        (501) staff       (20)     2545 2022-11-11 12:12:15.000000 movie-bot-api-0.0.8/moviebotapi/core/country_mapping.txt
--rw-r--r--   0 yee        (501) staff       (20)      343 2022-11-11 12:16:46.000000 movie-bot-api-0.0.8/moviebotapi/core/decorators.py
--rw-r--r--   0 yee        (501) staff       (20)      226 2022-11-11 01:25:56.000000 movie-bot-api-0.0.8/moviebotapi/core/exceptions.py
--rw-r--r--   0 yee        (501) staff       (20)      282 2022-11-11 12:12:15.000000 movie-bot-api-0.0.8/moviebotapi/core/models.py
--rw-r--r--   0 yee        (501) staff       (20)     2546 2022-11-11 12:34:49.000000 movie-bot-api-0.0.8/moviebotapi/core/session.py
--rw-r--r--   0 yee        (501) staff       (20)     8298 2022-11-11 12:12:15.000000 movie-bot-api-0.0.8/moviebotapi/core/utils.py
--rw-r--r--   0 yee        (501) staff       (20)     2505 2022-11-11 01:25:56.000000 movie-bot-api-0.0.8/moviebotapi/douban.py
--rw-r--r--   0 yee        (501) staff       (20)     4521 2022-11-11 12:34:49.000000 movie-bot-api-0.0.8/moviebotapi/ext.py
--rw-r--r--   0 yee        (501) staff       (20)     1061 2022-11-11 01:25:56.000000 movie-bot-api-0.0.8/moviebotapi/scraper.py
--rw-r--r--   0 yee        (501) staff       (20)     1222 2022-11-11 01:25:56.000000 movie-bot-api-0.0.8/moviebotapi/site.py
--rw-r--r--   0 yee        (501) staff       (20)     2982 2022-11-11 01:25:56.000000 movie-bot-api-0.0.8/moviebotapi/subscribe.py
--rw-r--r--   0 yee        (501) staff       (20)     3599 2022-11-11 12:16:46.000000 movie-bot-api-0.0.8/moviebotapi/tmdb.py
--rw-r--r--   0 yee        (501) staff       (20)     2139 2022-11-11 12:12:15.000000 movie-bot-api-0.0.8/moviebotapi/user.py
--rw-r--r--   0 yee        (501) staff       (20)       38 2022-11-11 12:35:04.750595 movie-bot-api-0.0.8/setup.cfg
--rw-r--r--   0 yee        (501) staff       (20)      874 2022-11-11 12:34:49.000000 movie-bot-api-0.0.8/setup.py
+drwxr-xr-x   0 yee        (501) staff       (20)        0 2022-11-11 14:03:44.960880 movie-bot-api-0.0.9/
+-rw-r--r--   0 yee        (501) staff       (20)     1066 2022-11-11 01:25:56.000000 movie-bot-api-0.0.9/LICENSE
+-rw-r--r--   0 yee        (501) staff       (20)       40 2022-11-11 12:12:15.000000 movie-bot-api-0.0.9/MANIFEST.in
+-rw-r--r--   0 yee        (501) staff       (20)      404 2022-11-11 14:03:44.960714 movie-bot-api-0.0.9/PKG-INFO
+-rw-r--r--   0 yee        (501) staff       (20)       42 2022-11-11 01:25:56.000000 movie-bot-api-0.0.9/README.md
+drwxr-xr-x   0 yee        (501) staff       (20)        0 2022-11-11 14:03:44.957126 movie-bot-api-0.0.9/movie_bot_api.egg-info/
+-rw-r--r--   0 yee        (501) staff       (20)      404 2022-11-11 14:03:44.000000 movie-bot-api-0.0.9/movie_bot_api.egg-info/PKG-INFO
+-rw-r--r--   0 yee        (501) staff       (20)      626 2022-11-11 14:03:44.000000 movie-bot-api-0.0.9/movie_bot_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yee        (501) staff       (20)        1 2022-11-11 14:03:44.000000 movie-bot-api-0.0.9/movie_bot_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yee        (501) staff       (20)       36 2022-11-11 14:03:44.000000 movie-bot-api-0.0.9/movie_bot_api.egg-info/requires.txt
+-rw-r--r--   0 yee        (501) staff       (20)       12 2022-11-11 14:03:44.000000 movie-bot-api-0.0.9/movie_bot_api.egg-info/top_level.txt
+drwxr-xr-x   0 yee        (501) staff       (20)        0 2022-11-11 14:03:44.958943 movie-bot-api-0.0.9/moviebotapi/
+-rw-r--r--   0 yee        (501) staff       (20)      939 2022-11-11 13:41:01.000000 movie-bot-api-0.0.9/moviebotapi/__init__.py
+drwxr-xr-x   0 yee        (501) staff       (20)        0 2022-11-11 14:03:44.960461 movie-bot-api-0.0.9/moviebotapi/core/
+-rw-r--r--   0 yee        (501) staff       (20)        0 2022-11-11 01:25:56.000000 movie-bot-api-0.0.9/moviebotapi/core/__init__.py
+-rw-r--r--   0 yee        (501) staff       (20)     2545 2022-11-11 12:12:15.000000 movie-bot-api-0.0.9/moviebotapi/core/country_mapping.txt
+-rw-r--r--   0 yee        (501) staff       (20)      343 2022-11-11 12:16:46.000000 movie-bot-api-0.0.9/moviebotapi/core/decorators.py
+-rw-r--r--   0 yee        (501) staff       (20)      226 2022-11-11 01:25:56.000000 movie-bot-api-0.0.9/moviebotapi/core/exceptions.py
+-rw-r--r--   0 yee        (501) staff       (20)      282 2022-11-11 12:12:15.000000 movie-bot-api-0.0.9/moviebotapi/core/models.py
+-rw-r--r--   0 yee        (501) staff       (20)     2546 2022-11-11 12:34:49.000000 movie-bot-api-0.0.9/moviebotapi/core/session.py
+-rw-r--r--   0 yee        (501) staff       (20)     8298 2022-11-11 12:12:15.000000 movie-bot-api-0.0.9/moviebotapi/core/utils.py
+-rw-r--r--   0 yee        (501) staff       (20)     2505 2022-11-11 01:25:56.000000 movie-bot-api-0.0.9/moviebotapi/douban.py
+-rw-r--r--   0 yee        (501) staff       (20)     4521 2022-11-11 12:34:49.000000 movie-bot-api-0.0.9/moviebotapi/ext.py
+-rw-r--r--   0 yee        (501) staff       (20)     1765 2022-11-11 13:38:51.000000 movie-bot-api-0.0.9/moviebotapi/notify.py
+-rw-r--r--   0 yee        (501) staff       (20)     1061 2022-11-11 01:25:56.000000 movie-bot-api-0.0.9/moviebotapi/scraper.py
+-rw-r--r--   0 yee        (501) staff       (20)     1222 2022-11-11 01:25:56.000000 movie-bot-api-0.0.9/moviebotapi/site.py
+-rw-r--r--   0 yee        (501) staff       (20)     2982 2022-11-11 01:25:56.000000 movie-bot-api-0.0.9/moviebotapi/subscribe.py
+-rw-r--r--   0 yee        (501) staff       (20)     3599 2022-11-11 12:16:46.000000 movie-bot-api-0.0.9/moviebotapi/tmdb.py
+-rw-r--r--   0 yee        (501) staff       (20)     2139 2022-11-11 12:12:15.000000 movie-bot-api-0.0.9/moviebotapi/user.py
+-rw-r--r--   0 yee        (501) staff       (20)       38 2022-11-11 14:03:44.960941 movie-bot-api-0.0.9/setup.cfg
+-rw-r--r--   0 yee        (501) staff       (20)      874 2022-11-11 14:03:42.000000 movie-bot-api-0.0.9/setup.py
```

### Comparing `movie-bot-api-0.0.8/LICENSE` & `movie-bot-api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `movie-bot-api-0.0.8/movie_bot_api.egg-info/SOURCES.txt` & `movie-bot-api-0.0.9/movie_bot_api.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 movie_bot_api.egg-info/SOURCES.txt
 movie_bot_api.egg-info/dependency_links.txt
 movie_bot_api.egg-info/requires.txt
 movie_bot_api.egg-info/top_level.txt
 moviebotapi/__init__.py
 moviebotapi/douban.py
 moviebotapi/ext.py
+moviebotapi/notify.py
 moviebotapi/scraper.py
 moviebotapi/site.py
 moviebotapi/subscribe.py
 moviebotapi/tmdb.py
 moviebotapi/user.py
 moviebotapi/core/__init__.py
 moviebotapi/core/country_mapping.txt
```

### Comparing `movie-bot-api-0.0.8/moviebotapi/core/country_mapping.txt` & `movie-bot-api-0.0.9/moviebotapi/core/country_mapping.txt`

 * *Files identical despite different names*

### Comparing `movie-bot-api-0.0.8/moviebotapi/core/session.py` & `movie-bot-api-0.0.9/moviebotapi/core/session.py`

 * *Files identical despite different names*

### Comparing `movie-bot-api-0.0.8/moviebotapi/core/utils.py` & `movie-bot-api-0.0.9/moviebotapi/core/utils.py`

 * *Files identical despite different names*

### Comparing `movie-bot-api-0.0.8/moviebotapi/douban.py` & `movie-bot-api-0.0.9/moviebotapi/douban.py`

 * *Files identical despite different names*

### Comparing `movie-bot-api-0.0.8/moviebotapi/ext.py` & `movie-bot-api-0.0.9/moviebotapi/ext.py`

 * *Files identical despite different names*

### Comparing `movie-bot-api-0.0.8/moviebotapi/scraper.py` & `movie-bot-api-0.0.9/moviebotapi/scraper.py`

 * *Files identical despite different names*

### Comparing `movie-bot-api-0.0.8/moviebotapi/site.py` & `movie-bot-api-0.0.9/moviebotapi/site.py`

 * *Files identical despite different names*

### Comparing `movie-bot-api-0.0.8/moviebotapi/subscribe.py` & `movie-bot-api-0.0.9/moviebotapi/subscribe.py`

 * *Files identical despite different names*

### Comparing `movie-bot-api-0.0.8/moviebotapi/tmdb.py` & `movie-bot-api-0.0.9/moviebotapi/tmdb.py`

 * *Files identical despite different names*

### Comparing `movie-bot-api-0.0.8/moviebotapi/user.py` & `movie-bot-api-0.0.9/moviebotapi/user.py`

 * *Files identical despite different names*

### Comparing `movie-bot-api-0.0.8/setup.py` & `movie-bot-api-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open('requirements.txt') as handle:
     for line in handle.readlines():
         if not line.startswith('#'):
             package = line.strip().split('=', 1)[0]
             requirements.append(package)
 setup(
     name='movie-bot-api',
-    version='0.0.8',
+    version='0.0.9',
     author='yee',
     author_email='yipengfei329@gmail.com',
     url='https://github.com/pofey/movie-bot-api',
     description='智能影音机器人MovieBot的接口SDK',
     python_requires='>=3.8',
     long_description=readme,
     long_description_content_type="text/markdown",
```

