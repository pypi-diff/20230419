# Comparing `tmp/django-cards-0.8.8.tar.gz` & `tmp/django-cards-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cards-0.8.8.tar", last modified: Tue Mar 14 15:27:47 2023, max compression
+gzip compressed data, was "django-cards-0.8.9.tar", last modified: Thu Mar 16 15:08:48 2023, max compression
```

## Comparing `django-cards-0.8.8.tar` & `django-cards-0.8.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.642893 django-cards-0.8.8/
--rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-16 09:53:41.000000 django-cards-0.8.8/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       55 2023-01-16 09:53:41.000000 django-cards-0.8.8/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)      588 2023-03-14 15:27:47.642724 django-cards-0.8.8/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      130 2023-01-16 09:53:41.000000 django-cards-0.8.8/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.607053 django-cards-0.8.8/cards/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      166 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/apps.py
--rw-r--r--   0 tom        (501) staff       (20)    25986 2023-03-14 15:25:24.000000 django-cards-0.8.8/cards/base.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.609109 django-cards-0.8.8/cards/card_list/
--rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/card_list/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     5753 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/card_list/base.py
--rw-r--r--   0 tom        (501) staff       (20)     3952 2023-02-20 18:38:25.000000 django-cards-0.8.8/cards/card_list/main.py
--rw-r--r--   0 tom        (501) staff       (20)     2468 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/card_list/tree.py
--rw-r--r--   0 tom        (501) staff       (20)      714 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/includes.py
--rw-r--r--   0 tom        (501) staff       (20)     5204 2023-02-21 09:19:57.000000 django-cards-0.8.8/cards/standard.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.598516 django-cards-0.8.8/cards/static/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.598644 django-cards-0.8.8/cards/static/cards/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.600171 django-cards-0.8.8/cards/static/cards/jstree/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.598907 django-cards-0.8.8/cards/static/cards/jstree/css/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.599498 django-cards-0.8.8/cards/static/cards/jstree/css/themes/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.611576 django-cards-0.8.8/cards/static/cards/jstree/css/themes/default/
--rw-r--r--   0 tom        (501) staff       (20)     5660 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/default/32px.png
--rw-r--r--   0 tom        (501) staff       (20)     2215 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/default/40px.png
--rw-r--r--   0 tom        (501) staff       (20)    31722 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/default/style.css
--rw-r--r--   0 tom        (501) staff       (20)    27353 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/default/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/default/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.615172 django-cards-0.8.8/cards/static/cards/jstree/css/themes/default-dark/
--rw-r--r--   0 tom        (501) staff       (20)     1525 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/default-dark/32px.png
--rw-r--r--   0 tom        (501) staff       (20)     6526 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/default-dark/40px.png
--rw-r--r--   0 tom        (501) staff       (20)    34459 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/default-dark/style.css
--rw-r--r--   0 tom        (501) staff       (20)    29959 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/default-dark/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/default-dark/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.619288 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/
--rw-r--r--   0 tom        (501) staff       (20)     6423 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/30px.png
--rw-r--r--   0 tom        (501) staff       (20)     3333 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/32px.png
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.599901 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.627386 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/
--rw-r--r--   0 tom        (501) staff       (20)    24108 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   134830 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    49936 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    27344 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    24056 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   140377 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    50224 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    27108 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    25059 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   150837 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    50788 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    28152 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    32574 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/style.css
--rw-r--r--   0 tom        (501) staff       (20)    27752 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1720 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.630057 django-cards-0.8.8/cards/static/cards/jstree/js/
--rw-r--r--   0 tom        (501) staff       (20)   307794 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/js/jstree.js
--rw-r--r--   0 tom        (501) staff       (20)   141222 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/static/cards/jstree/js/jstree.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.600622 django-cards-0.8.8/cards/templates/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.601277 django-cards-0.8.8/cards/templates/cards/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.632444 django-cards-0.8.8/cards/templates/cards/groups/
--rw-r--r--   0 tom        (501) staff       (20)      206 2023-01-18 12:35:38.000000 django-cards-0.8.8/cards/templates/cards/groups/groups.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.639993 django-cards-0.8.8/cards/templates/cards/standard/
--rw-r--r--   0 tom        (501) staff       (20)       69 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/templates/cards/standard/blank.html
--rw-r--r--   0 tom        (501) staff       (20)     1588 2023-01-26 20:53:02.000000 django-cards-0.8.8/cards/templates/cards/standard/card_group.html
--rw-r--r--   0 tom        (501) staff       (20)      980 2023-01-26 20:53:02.000000 django-cards-0.8.8/cards/templates/cards/standard/datatable.html
--rw-r--r--   0 tom        (501) staff       (20)      767 2023-01-26 20:53:02.000000 django-cards-0.8.8/cards/templates/cards/standard/default.html
--rw-r--r--   0 tom        (501) staff       (20)     1528 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/templates/cards/standard/default_body.html
--rw-r--r--   0 tom        (501) staff       (20)      917 2023-01-26 20:53:02.000000 django-cards-0.8.8/cards/templates/cards/standard/html.html
--rw-r--r--   0 tom        (501) staff       (20)     2541 2023-02-20 15:01:01.000000 django-cards-0.8.8/cards/templates/cards/standard/list_selection.html
--rw-r--r--   0 tom        (501) staff       (20)      565 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/templates/cards/standard/message.html
--rw-r--r--   0 tom        (501) staff       (20)      848 2023-01-26 20:53:02.000000 django-cards-0.8.8/cards/templates/cards/standard/table.html
--rw-r--r--   0 tom        (501) staff       (20)     1231 2023-03-14 15:05:03.000000 django-cards-0.8.8/cards/templates/cards/standard/table_body.html
--rw-r--r--   0 tom        (501) staff       (20)     2132 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/templates/cards/standard/tree_selection.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.640910 django-cards-0.8.8/cards/templatetags/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/templatetags/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      362 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/templatetags/django_cards_tags.py
--rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.8.8/cards/url_converters.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-14 15:27:47.642428 django-cards-0.8.8/django_cards.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      588 2023-03-14 15:27:47.000000 django-cards-0.8.8/django_cards.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     3065 2023-03-14 15:27:47.000000 django-cards-0.8.8/django_cards.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-14 15:27:47.000000 django-cards-0.8.8/django_cards.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2023-03-14 15:27:47.000000 django-cards-0.8.8/django_cards.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-03-14 15:27:47.642932 django-cards-0.8.8/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      645 2023-03-14 15:27:36.000000 django-cards-0.8.8/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.963661 django-cards-0.8.9/
+-rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-16 09:53:41.000000 django-cards-0.8.9/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       55 2023-01-16 09:53:41.000000 django-cards-0.8.9/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)      588 2023-03-16 15:08:48.963506 django-cards-0.8.9/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      130 2023-01-16 09:53:41.000000 django-cards-0.8.9/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.920722 django-cards-0.8.9/cards/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      166 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/apps.py
+-rw-r--r--   0 tom        (501) staff       (20)    25744 2023-03-16 15:07:28.000000 django-cards-0.8.9/cards/base.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.922731 django-cards-0.8.9/cards/card_list/
+-rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/card_list/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     5753 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/card_list/base.py
+-rw-r--r--   0 tom        (501) staff       (20)     3952 2023-02-20 18:38:25.000000 django-cards-0.8.9/cards/card_list/main.py
+-rw-r--r--   0 tom        (501) staff       (20)     2468 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/card_list/tree.py
+-rw-r--r--   0 tom        (501) staff       (20)      714 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/includes.py
+-rw-r--r--   0 tom        (501) staff       (20)     5204 2023-02-21 09:19:57.000000 django-cards-0.8.9/cards/standard.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.912636 django-cards-0.8.9/cards/static/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.912796 django-cards-0.8.9/cards/static/cards/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.914224 django-cards-0.8.9/cards/static/cards/jstree/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.913134 django-cards-0.8.9/cards/static/cards/jstree/css/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.913660 django-cards-0.8.9/cards/static/cards/jstree/css/themes/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.925265 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/
+-rw-r--r--   0 tom        (501) staff       (20)     5660 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/32px.png
+-rw-r--r--   0 tom        (501) staff       (20)     2215 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/40px.png
+-rw-r--r--   0 tom        (501) staff       (20)    31722 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    27353 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.927591 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/
+-rw-r--r--   0 tom        (501) staff       (20)     1525 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/32px.png
+-rw-r--r--   0 tom        (501) staff       (20)     6526 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/40px.png
+-rw-r--r--   0 tom        (501) staff       (20)    34459 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    29959 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.930275 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/
+-rw-r--r--   0 tom        (501) staff       (20)     6423 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/30px.png
+-rw-r--r--   0 tom        (501) staff       (20)     3333 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/32px.png
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.913998 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.948120 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/
+-rw-r--r--   0 tom        (501) staff       (20)    24108 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   134830 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    49936 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    27344 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    24056 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   140377 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    50224 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    27108 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    25059 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   150837 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    50788 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    28152 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    32574 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    27752 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1720 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.955730 django-cards-0.8.9/cards/static/cards/jstree/js/
+-rw-r--r--   0 tom        (501) staff       (20)   307794 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/js/jstree.js
+-rw-r--r--   0 tom        (501) staff       (20)   141222 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/js/jstree.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.914737 django-cards-0.8.9/cards/templates/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.915494 django-cards-0.8.9/cards/templates/cards/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.958148 django-cards-0.8.9/cards/templates/cards/groups/
+-rw-r--r--   0 tom        (501) staff       (20)      206 2023-01-18 12:35:38.000000 django-cards-0.8.9/cards/templates/cards/groups/groups.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.961840 django-cards-0.8.9/cards/templates/cards/standard/
+-rw-r--r--   0 tom        (501) staff       (20)       69 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/templates/cards/standard/blank.html
+-rw-r--r--   0 tom        (501) staff       (20)     1588 2023-01-26 20:53:02.000000 django-cards-0.8.9/cards/templates/cards/standard/card_group.html
+-rw-r--r--   0 tom        (501) staff       (20)      980 2023-01-26 20:53:02.000000 django-cards-0.8.9/cards/templates/cards/standard/datatable.html
+-rw-r--r--   0 tom        (501) staff       (20)      767 2023-01-26 20:53:02.000000 django-cards-0.8.9/cards/templates/cards/standard/default.html
+-rw-r--r--   0 tom        (501) staff       (20)     1528 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/templates/cards/standard/default_body.html
+-rw-r--r--   0 tom        (501) staff       (20)      917 2023-01-26 20:53:02.000000 django-cards-0.8.9/cards/templates/cards/standard/html.html
+-rw-r--r--   0 tom        (501) staff       (20)     2541 2023-02-20 15:01:01.000000 django-cards-0.8.9/cards/templates/cards/standard/list_selection.html
+-rw-r--r--   0 tom        (501) staff       (20)      565 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/templates/cards/standard/message.html
+-rw-r--r--   0 tom        (501) staff       (20)      848 2023-01-26 20:53:02.000000 django-cards-0.8.9/cards/templates/cards/standard/table.html
+-rw-r--r--   0 tom        (501) staff       (20)     1231 2023-03-14 15:05:03.000000 django-cards-0.8.9/cards/templates/cards/standard/table_body.html
+-rw-r--r--   0 tom        (501) staff       (20)     2132 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/templates/cards/standard/tree_selection.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.962333 django-cards-0.8.9/cards/templatetags/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/templatetags/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      362 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/templatetags/django_cards_tags.py
+-rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/url_converters.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.963251 django-cards-0.8.9/django_cards.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      588 2023-03-16 15:08:48.000000 django-cards-0.8.9/django_cards.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     3065 2023-03-16 15:08:48.000000 django-cards-0.8.9/django_cards.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-16 15:08:48.000000 django-cards-0.8.9/django_cards.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-03-16 15:08:48.000000 django-cards-0.8.9/django_cards.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-03-16 15:08:48.963702 django-cards-0.8.9/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      645 2023-03-16 15:08:06.000000 django-cards-0.8.9/setup.py
```

### Comparing `django-cards-0.8.8/LICENSE` & `django-cards-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/PKG-INFO` & `django-cards-0.8.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cards
-Version: 0.8.8
+Version: 0.8.9
 Summary: Django app that allows you make cards
 Home-page: https://github.com/django-advance-utils/django-cards
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-cards-0.8.8/cards/base.py` & `django-cards-0.8.9/cards/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,16 +245,16 @@
                     if not hasattr(value, 'through') and callable(value):
                         value = value()
 
                     if label is None:
                         label = self.label_from_field(field=field, field_type=field_type)
         return value, label, field_type
 
-    def _add_many_to_many_field(self, label, query, query_filter, m2m_field,
-                                html_barge, default='N/A', html_override=None,
+    def _add_many_to_many_field(self, label, query, query_filter=None, m2m_field=None,
+                                html_barge=None, default='N/A', html_override=None,
                                 entry_css_class=None, css_class=None, menu=None, default_if=None, **kwargs):
         if html_barge is None:
             html_barge = '<span class="small badge badge-pill badge-primary"> %1% </span> '
 
         if query_filter is None:
             results = query.all()
         else:
@@ -308,17 +308,14 @@
                                        html_override=html_override,
                                        menu=menu,
                                        default_if=default_if,
                                        **kwargs)
         elif hasattr(value, 'through'):
             return self._add_many_to_many_field(label=label,
                                                 query=value,
-                                                query_filter=kwargs.get('query_filter'),
-                                                html_barge=kwargs.get('html_barge'),
-                                                m2m_field=kwargs.get('m2m_field'),
                                                 default=default,
                                                 html_override=html_override,
                                                 entry_css_class=entry_css_class,
                                                 css_class=entry_css_class,
                                                 menu=menu,
                                                 default_if=default_if,
                                                 **kwargs)
```

### Comparing `django-cards-0.8.8/cards/card_list/base.py` & `django-cards-0.8.9/cards/card_list/base.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/card_list/main.py` & `django-cards-0.8.9/cards/card_list/main.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/card_list/tree.py` & `django-cards-0.8.9/cards/card_list/tree.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/includes.py` & `django-cards-0.8.9/cards/includes.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/standard.py` & `django-cards-0.8.9/cards/standard.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/default/32px.png` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/default/40px.png` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/40px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/default/style.css` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/default/style.min.css` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/default/throbber.gif` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/default-dark/32px.png` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/default-dark/40px.png` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/40px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/default-dark/style.css` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/default-dark/style.min.css` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/default-dark/throbber.gif` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/30px.png` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/30px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/32px.png` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/style.css` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/style.min.css` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/css/themes/proton/throbber.gif` & `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/js/jstree.js` & `django-cards-0.8.9/cards/static/cards/jstree/js/jstree.js`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/static/cards/jstree/js/jstree.min.js` & `django-cards-0.8.9/cards/static/cards/jstree/js/jstree.min.js`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/templates/cards/standard/card_group.html` & `django-cards-0.8.9/cards/templates/cards/standard/card_group.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/templates/cards/standard/datatable.html` & `django-cards-0.8.9/cards/templates/cards/standard/datatable.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/templates/cards/standard/default.html` & `django-cards-0.8.9/cards/templates/cards/standard/default.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/templates/cards/standard/default_body.html` & `django-cards-0.8.9/cards/templates/cards/standard/default_body.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/templates/cards/standard/html.html` & `django-cards-0.8.9/cards/templates/cards/standard/html.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/templates/cards/standard/list_selection.html` & `django-cards-0.8.9/cards/templates/cards/standard/list_selection.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/templates/cards/standard/message.html` & `django-cards-0.8.9/cards/templates/cards/standard/message.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/templates/cards/standard/table.html` & `django-cards-0.8.9/cards/templates/cards/standard/table.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/templates/cards/standard/table_body.html` & `django-cards-0.8.9/cards/templates/cards/standard/table_body.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/cards/templates/cards/standard/tree_selection.html` & `django-cards-0.8.9/cards/templates/cards/standard/tree_selection.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/django_cards.egg-info/PKG-INFO` & `django-cards-0.8.9/django_cards.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cards
-Version: 0.8.8
+Version: 0.8.9
 Summary: Django app that allows you make cards
 Home-page: https://github.com/django-advance-utils/django-cards
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-cards-0.8.8/django_cards.egg-info/SOURCES.txt` & `django-cards-0.8.9/django_cards.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.8/setup.py` & `django-cards-0.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-cards",
-    version="0.8.8",
+    version="0.8.9",
     author="Thomas Turner",
     description="Django app that allows you make cards",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/django-cards",
     include_package_data=True,
     packages=['cards'],
```

