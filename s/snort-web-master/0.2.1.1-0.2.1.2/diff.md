# Comparing `tmp/snort_web_master-0.2.1.1.tar.gz` & `tmp/snort_web_master-0.2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\snort_web_master-0.2.1.1.tar", last modified: Wed Mar 15 09:11:29 2023, max compression
+gzip compressed data, was "dist\snort_web_master-0.2.1.2.tar", last modified: Wed Apr 19 11:29:37 2023, max compression
```

## Comparing `snort_web_master-0.2.1.1.tar` & `snort_web_master-0.2.1.2.tar`

### file list

```diff
@@ -1,86 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:29.385730 snort_web_master-0.2.1.1/
--rw-rw-rw-   0        0        0       54 2022-11-21 06:29:02.000000 snort_web_master-0.2.1.1/LICENSE.rst
--rw-rw-rw-   0        0        0       24 2022-11-24 17:54:23.000000 snort_web_master-0.2.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      251 2023-03-15 09:11:29.385730 snort_web_master-0.2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      716 2022-11-21 06:20:44.000000 snort_web_master-0.2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:28.870109 snort_web_master-0.2.1.1/data/
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:28.682604 snort_web_master-0.2.1.1/data/admin/
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:28.901394 snort_web_master-0.2.1.1/data/admin/image/
--rw-rw-rw-   0        0        0     7972 2023-01-16 16:49:34.000000 snort_web_master-0.2.1.1/data/admin/image/images.png
--rw-rw-rw-   0        0        0   241664 2023-01-07 17:05:37.000000 snort_web_master-0.2.1.1/data/db.sqlite3
--rw-rw-rw-   0        0        0    39363 2022-10-13 12:31:39.000000 snort_web_master-0.2.1.1/data/dicts.py
--rw-rw-rw-   0        0        0      690 2023-01-23 09:10:03.000000 snort_web_master-0.2.1.1/data/dockercompose
--rw-rw-rw-   0        0        0   139272 2023-01-16 16:50:11.000000 snort_web_master-0.2.1.1/data/favicon.ico
--rw-rw-rw-   0        0        0      898 2023-01-23 08:40:15.000000 snort_web_master-0.2.1.1/data/migrate sqllite to postgresql
--rw-rw-rw-   0        0        0      402 2022-11-14 09:05:52.000000 snort_web_master-0.2.1.1/data/my-snort-rule.tmp
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:28.901394 snort_web_master-0.2.1.1/data/nginx/
--rw-rw-rw-   0        0        0       96 2023-01-23 09:09:18.000000 snort_web_master-0.2.1.1/data/nginx/nginx
--rw-rw-rw-   0        0        0      296 2023-01-23 09:04:00.000000 snort_web_master-0.2.1.1/data/nginx/nginx.conf
--rw-rw-rw-   0        0        0      162 2023-01-23 08:44:15.000000 snort_web_master-0.2.1.1/data/requirements.txt
--rw-rw-rw-   0        0        0      793 2023-01-23 08:53:39.000000 snort_web_master-0.2.1.1/data/snortFile
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:28.698347 snort_web_master-0.2.1.1/data/templates/
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:28.917017 snort_web_master-0.2.1.1/data/templates/html/
--rw-rw-rw-   0        0        0     5526 2023-03-15 08:25:40.000000 snort_web_master-0.2.1.1/data/templates/html/full_rule.html
--rw-rw-rw-   0        0        0      420 2023-01-23 09:19:00.000000 snort_web_master-0.2.1.1/data/templates/html/import.html
--rw-rw-rw-   0        0        0    26013 2023-03-15 08:51:55.000000 snort_web_master-0.2.1.1/data/templates/html/snortBuilder.html
--rw-rw-rw-   0        0        0      140 2023-03-15 09:11:29.385730 snort_web_master-0.2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-03-15 09:11:20.000000 snort_web_master-0.2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:28.698347 snort_web_master-0.2.1.1/snort_web_master/
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:28.963891 snort_web_master-0.2.1.1/snort_web_master/pcaps/
--rw-rw-rw-   0        0        0        0 2022-10-31 09:04:45.000000 snort_web_master-0.2.1.1/snort_web_master/pcaps/__init__.py
--rw-rw-rw-   0        0        0     2689 2023-01-08 17:50:03.000000 snort_web_master-0.2.1.1/snort_web_master/pcaps/admin.py
--rw-rw-rw-   0        0        0      148 2022-10-31 09:04:45.000000 snort_web_master-0.2.1.1/snort_web_master/pcaps/apps.py
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:29.041993 snort_web_master-0.2.1.1/snort_web_master/pcaps/migrations/
--rw-rw-rw-   0        0        0     1385 2022-12-19 18:20:00.000000 snort_web_master-0.2.1.1/snort_web_master/pcaps/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      813 2022-12-19 18:20:00.000000 snort_web_master-0.2.1.1/snort_web_master/pcaps/migrations/0002_initial.py
--rw-rw-rw-   0        0        0      555 2022-12-19 18:24:58.000000 snort_web_master-0.2.1.1/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py
--rw-rw-rw-   0        0        0      603 2022-12-19 18:25:24.000000 snort_web_master-0.2.1.1/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.1.1/snort_web_master/pcaps/migrations/__init__.py
--rw-rw-rw-   0        0        0     1060 2022-12-19 18:25:20.000000 snort_web_master-0.2.1.1/snort_web_master/pcaps/models.py
--rw-rw-rw-   0        0        0       63 2022-10-31 09:04:45.000000 snort_web_master-0.2.1.1/snort_web_master/pcaps/tests.py
--rw-rw-rw-   0        0        0       66 2022-10-31 09:04:45.000000 snort_web_master-0.2.1.1/snort_web_master/pcaps/views.py
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:29.073473 snort_web_master-0.2.1.1/snort_web_master/settings/
--rw-rw-rw-   0        0        0        0 2022-12-19 07:00:41.000000 snort_web_master-0.2.1.1/snort_web_master/settings/__init__.py
--rw-rw-rw-   0        0        0      535 2023-01-10 16:23:06.000000 snort_web_master-0.2.1.1/snort_web_master/settings/admin.py
--rw-rw-rw-   0        0        0      154 2022-12-19 07:00:41.000000 snort_web_master-0.2.1.1/snort_web_master/settings/apps.py
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:29.151381 snort_web_master-0.2.1.1/snort_web_master/settings/migrations/
--rw-rw-rw-   0        0        0     1595 2022-12-19 18:20:00.000000 snort_web_master-0.2.1.1/snort_web_master/settings/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1350 2022-12-26 06:21:16.000000 snort_web_master-0.2.1.1/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py
--rw-rw-rw-   0        0        0      530 2022-12-26 06:23:11.000000 snort_web_master-0.2.1.1/snort_web_master/settings/migrations/0003_keywords_avalable.py
--rw-rw-rw-   0        0        0      349 2023-01-08 18:38:56.000000 snort_web_master-0.2.1.1/snort_web_master/settings/migrations/0004_remove_keywords_negation.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.1.1/snort_web_master/settings/migrations/__init__.py
--rw-rw-rw-   0        0        0     1716 2023-01-08 18:38:54.000000 snort_web_master-0.2.1.1/snort_web_master/settings/models.py
--rw-rw-rw-   0        0        0       63 2022-12-19 07:00:41.000000 snort_web_master-0.2.1.1/snort_web_master/settings/tests.py
--rw-rw-rw-   0        0        0       66 2022-12-19 07:00:41.000000 snort_web_master-0.2.1.1/snort_web_master/settings/views.py
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:29.229508 snort_web_master-0.2.1.1/snort_web_master/snort/
--rw-rw-rw-   0        0        0        0 2022-10-31 09:04:41.000000 snort_web_master-0.2.1.1/snort_web_master/snort/__init__.py
--rw-rw-rw-   0        0        0    27398 2023-03-15 07:54:27.000000 snort_web_master-0.2.1.1/snort_web_master/snort/admin.py
--rw-rw-rw-   0        0        0      148 2022-10-31 09:04:41.000000 snort_web_master-0.2.1.1/snort_web_master/snort/apps.py
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:29.292062 snort_web_master-0.2.1.1/snort_web_master/snort/migrations/
--rw-rw-rw-   0        0        0     1974 2022-12-19 18:20:00.000000 snort_web_master-0.2.1.1/snort_web_master/snort/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      870 2023-01-05 14:35:56.000000 snort_web_master-0.2.1.1/snort_web_master/snort/migrations/0002_snortruleviewarray.py
--rw-rw-rw-   0        0        0      610 2023-01-06 06:03:56.000000 snort_web_master-0.2.1.1/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py
--rw-rw-rw-   0        0        0      423 2023-01-06 13:23:29.000000 snort_web_master-0.2.1.1/snort_web_master/snort/migrations/0004_snortrule_deleted.py
--rw-rw-rw-   0        0        0      522 2023-01-08 17:24:52.000000 snort_web_master-0.2.1.1/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py
--rw-rw-rw-   0        0        0      759 2023-02-21 08:33:21.000000 snort_web_master-0.2.1.1/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.1.1/snort_web_master/snort/migrations/__init__.py
--rw-rw-rw-   0        0        0     2092 2023-03-01 09:37:23.000000 snort_web_master-0.2.1.1/snort_web_master/snort/models.py
--rw-rw-rw-   0        0        0    19362 2023-01-12 18:25:18.000000 snort_web_master-0.2.1.1/snort_web_master/snort/parser.py
--rw-rw-rw-   0        0        0     2271 2022-12-19 09:13:39.000000 snort_web_master-0.2.1.1/snort_web_master/snort/snort_templates.py
--rw-rw-rw-   0        0        0     4016 2023-02-21 08:27:30.000000 snort_web_master-0.2.1.1/snort_web_master/snort/tests.py
--rw-rw-rw-   0        0        0     5584 2023-03-15 09:02:25.000000 snort_web_master-0.2.1.1/snort_web_master/snort/views.py
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:29.354536 snort_web_master-0.2.1.1/snort_web_master/snort_web_master/
--rw-rw-rw-   0        0        0        0 2022-11-21 06:23:37.000000 snort_web_master-0.2.1.1/snort_web_master/snort_web_master/__init__.py
--rw-rw-rw-   0        0        0      425 2022-10-31 09:02:02.000000 snort_web_master-0.2.1.1/snort_web_master/snort_web_master/asgi.py
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:29.370146 snort_web_master-0.2.1.1/snort_web_master/snort_web_master/middleware/
--rw-rw-rw-   0        0        0        0 2023-01-09 07:35:12.000000 snort_web_master-0.2.1.1/snort_web_master/snort_web_master/middleware/__init__.py
--rw-rw-rw-   0        0        0      537 2023-01-09 14:10:56.000000 snort_web_master-0.2.1.1/snort_web_master/snort_web_master/middleware/no_cache.py
--rw-rw-rw-   0        0        0     5515 2023-02-21 08:38:39.000000 snort_web_master-0.2.1.1/snort_web_master/snort_web_master/settings.py
--rw-rw-rw-   0        0        0     1843 2023-02-21 09:52:10.000000 snort_web_master-0.2.1.1/snort_web_master/snort_web_master/urls.py
--rw-rw-rw-   0        0        0      425 2022-10-31 09:02:02.000000 snort_web_master-0.2.1.1/snort_web_master/snort_web_master/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-03-15 09:11:29.370146 snort_web_master-0.2.1.1/snort_web_master/snort_web_master.egg-info/
--rw-rw-rw-   0        0        0      251 2023-03-15 09:11:28.000000 snort_web_master-0.2.1.1/snort_web_master/snort_web_master.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2822 2023-03-15 09:11:28.000000 snort_web_master-0.2.1.1/snort_web_master/snort_web_master.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 09:11:28.000000 snort_web_master-0.2.1.1/snort_web_master/snort_web_master.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-03-15 09:11:28.000000 snort_web_master-0.2.1.1/snort_web_master/snort_web_master.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-03-15 09:11:28.000000 snort_web_master-0.2.1.1/snort_web_master/snort_web_master.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.483942 snort_web_master-0.2.1.2/
+-rw-rw-rw-   0        0        0       54 2022-11-21 06:29:02.000000 snort_web_master-0.2.1.2/LICENSE.rst
+-rw-rw-rw-   0        0        0       24 2022-11-24 17:54:23.000000 snort_web_master-0.2.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      251 2023-04-19 11:29:37.483942 snort_web_master-0.2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      716 2022-11-21 06:20:44.000000 snort_web_master-0.2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.374573 snort_web_master-0.2.1.2/data/
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.374573 snort_web_master-0.2.1.2/data/admin/
+-rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-0.2.1.2/data/admin/0004_keyword_delete_keywords.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.390170 snort_web_master-0.2.1.2/data/admin/image/
+-rw-rw-rw-   0        0        0     7972 2023-01-16 16:49:34.000000 snort_web_master-0.2.1.2/data/admin/image/images.png
+-rw-rw-rw-   0        0        0   241664 2023-01-07 17:05:37.000000 snort_web_master-0.2.1.2/data/db.sqlite3
+-rw-rw-rw-   0        0        0    39363 2022-10-13 12:31:39.000000 snort_web_master-0.2.1.2/data/dicts.py
+-rw-rw-rw-   0        0        0      690 2023-01-23 09:10:03.000000 snort_web_master-0.2.1.2/data/dockercompose
+-rw-rw-rw-   0        0        0   139272 2023-01-16 16:50:11.000000 snort_web_master-0.2.1.2/data/favicon.ico
+-rw-rw-rw-   0        0        0      898 2023-01-23 08:40:15.000000 snort_web_master-0.2.1.2/data/migrate sqllite to postgresql
+-rw-rw-rw-   0        0        0      402 2022-11-14 09:05:52.000000 snort_web_master-0.2.1.2/data/my-snort-rule.tmp
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.405796 snort_web_master-0.2.1.2/data/nginx/
+-rw-rw-rw-   0        0        0       96 2023-01-23 09:09:18.000000 snort_web_master-0.2.1.2/data/nginx/nginx
+-rw-rw-rw-   0        0        0      296 2023-01-23 09:04:00.000000 snort_web_master-0.2.1.2/data/nginx/nginx.conf
+-rw-rw-rw-   0        0        0      162 2023-01-23 08:44:15.000000 snort_web_master-0.2.1.2/data/requirements.txt
+-rw-rw-rw-   0        0        0      793 2023-01-23 08:53:39.000000 snort_web_master-0.2.1.2/data/snortFile
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.249571 snort_web_master-0.2.1.2/data/templates/
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.405796 snort_web_master-0.2.1.2/data/templates/html/
+-rw-rw-rw-   0        0        0     5678 2023-04-19 10:42:31.000000 snort_web_master-0.2.1.2/data/templates/html/full_rule.html
+-rw-rw-rw-   0        0        0      420 2023-01-23 09:19:00.000000 snort_web_master-0.2.1.2/data/templates/html/import.html
+-rw-rw-rw-   0        0        0    26921 2023-04-19 11:11:07.000000 snort_web_master-0.2.1.2/data/templates/html/snortBuilder.html
+-rw-rw-rw-   0        0        0      140 2023-04-19 11:29:37.499545 snort_web_master-0.2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      862 2023-04-19 11:28:23.000000 snort_web_master-0.2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.265170 snort_web_master-0.2.1.2/snort_web_master/
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.421420 snort_web_master-0.2.1.2/snort_web_master/pcaps/
+-rw-rw-rw-   0        0        0        0 2022-10-31 09:04:45.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/__init__.py
+-rw-rw-rw-   0        0        0     2689 2023-01-08 17:50:03.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/admin.py
+-rw-rw-rw-   0        0        0      148 2022-10-31 09:04:45.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.421420 snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/
+-rw-rw-rw-   0        0        0     1385 2022-12-19 18:20:00.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      813 2022-12-19 18:20:00.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0002_initial.py
+-rw-rw-rw-   0        0        0      555 2022-12-19 18:24:58.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py
+-rw-rw-rw-   0        0        0      603 2022-12-19 18:25:24.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1060 2022-12-19 18:25:20.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/models.py
+-rw-rw-rw-   0        0        0       63 2022-10-31 09:04:45.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/tests.py
+-rw-rw-rw-   0        0        0       66 2022-10-31 09:04:45.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/views.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.421420 snort_web_master-0.2.1.2/snort_web_master/settings/
+-rw-rw-rw-   0        0        0        0 2022-12-19 07:00:41.000000 snort_web_master-0.2.1.2/snort_web_master/settings/__init__.py
+-rw-rw-rw-   0        0        0      546 2023-04-19 09:25:30.000000 snort_web_master-0.2.1.2/snort_web_master/settings/admin.py
+-rw-rw-rw-   0        0        0      154 2022-12-19 07:00:41.000000 snort_web_master-0.2.1.2/snort_web_master/settings/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.437046 snort_web_master-0.2.1.2/snort_web_master/settings/migrations/
+-rw-rw-rw-   0        0        0     1595 2022-12-19 18:20:00.000000 snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1350 2022-12-26 06:21:16.000000 snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py
+-rw-rw-rw-   0        0        0      530 2022-12-26 06:23:11.000000 snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0003_keywords_avalable.py
+-rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py
+-rw-rw-rw-   0        0        0     1268 2023-04-19 09:28:30.000000 snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.1.2/snort_web_master/settings/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1444 2023-04-19 07:32:10.000000 snort_web_master-0.2.1.2/snort_web_master/settings/models.py
+-rw-rw-rw-   0        0        0       63 2022-12-19 07:00:41.000000 snort_web_master-0.2.1.2/snort_web_master/settings/tests.py
+-rw-rw-rw-   0        0        0       66 2022-12-19 07:00:41.000000 snort_web_master-0.2.1.2/snort_web_master/settings/views.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.437046 snort_web_master-0.2.1.2/snort_web_master/snort/
+-rw-rw-rw-   0        0        0        0 2022-10-31 09:04:41.000000 snort_web_master-0.2.1.2/snort_web_master/snort/__init__.py
+-rw-rw-rw-   0        0        0    28285 2023-04-19 11:26:51.000000 snort_web_master-0.2.1.2/snort_web_master/snort/admin.py
+-rw-rw-rw-   0        0        0      148 2022-10-31 09:04:41.000000 snort_web_master-0.2.1.2/snort_web_master/snort/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.452670 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/
+-rw-rw-rw-   0        0        0     1974 2022-12-19 18:20:00.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      870 2023-01-05 14:35:56.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0002_snortruleviewarray.py
+-rw-rw-rw-   0        0        0      610 2023-01-06 06:03:56.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py
+-rw-rw-rw-   0        0        0      423 2023-01-06 13:23:29.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0004_snortrule_deleted.py
+-rw-rw-rw-   0        0        0      522 2023-01-08 17:24:52.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py
+-rw-rw-rw-   0        0        0      759 2023-02-21 08:33:21.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py
+-rw-rw-rw-   0        0        0      477 2023-04-19 09:28:30.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0007_snortrule_tag.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-04-19 09:28:26.000000 snort_web_master-0.2.1.2/snort_web_master/snort/models.py
+-rw-rw-rw-   0        0        0    19362 2023-01-12 18:25:18.000000 snort_web_master-0.2.1.2/snort_web_master/snort/parser.py
+-rw-rw-rw-   0        0        0     2271 2022-12-19 09:13:39.000000 snort_web_master-0.2.1.2/snort_web_master/snort/snort_templates.py
+-rw-rw-rw-   0        0        0     4016 2023-02-21 08:27:30.000000 snort_web_master-0.2.1.2/snort_web_master/snort/tests.py
+-rw-rw-rw-   0        0        0     5584 2023-03-15 09:02:25.000000 snort_web_master-0.2.1.2/snort_web_master/snort/views.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.452670 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/
+-rw-rw-rw-   0        0        0        0 2022-11-21 06:23:37.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/__init__.py
+-rw-rw-rw-   0        0        0      425 2022-10-31 09:02:02.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/asgi.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.483942 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/middleware/
+-rw-rw-rw-   0        0        0        0 2023-01-09 07:35:12.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/middleware/__init__.py
+-rw-rw-rw-   0        0        0      537 2023-01-09 14:10:56.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/middleware/no_cache.py
+-rw-rw-rw-   0        0        0     5515 2023-04-19 09:26:16.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/settings.py
+-rw-rw-rw-   0        0        0     1959 2023-04-19 08:14:20.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/urls.py
+-rw-rw-rw-   0        0        0      425 2023-04-19 08:13:33.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.483942 snort_web_master-0.2.1.2/snort_web_master/snort_web_master.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-04-19 11:29:37.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3024 2023-04-19 11:29:37.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 11:29:37.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-04-19 11:29:37.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-04-19 11:29:37.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master.egg-info/top_level.txt
```

### Comparing `snort_web_master-0.2.1.1/README.md` & `snort_web_master-0.2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/data/admin/image/images.png` & `snort_web_master-0.2.1.2/data/admin/image/images.png`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/data/db.sqlite3` & `snort_web_master-0.2.1.2/data/db.sqlite3`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/data/dicts.py` & `snort_web_master-0.2.1.2/data/dicts.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/data/dockercompose` & `snort_web_master-0.2.1.2/data/dockercompose`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/data/favicon.ico` & `snort_web_master-0.2.1.2/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/data/migrate sqllite to postgresql` & `snort_web_master-0.2.1.2/data/migrate sqllite to postgresql`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/data/snortFile` & `snort_web_master-0.2.1.2/data/snortFile`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/data/templates/html/full_rule.html` & `snort_web_master-0.2.1.2/data/templates/html/full_rule.html`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   var id_content = document.getElementById("id_content");
   id_content.style.width = '98%';
   id_content.style.wordWrap  = "normal";
   id_content.style.wordBreak = "normal";
   function build_rule() {
   var sigid = document.getElementsByClassName("form-row field-id")[0].innerText.split("\n")[1];
   try{
-        var user_name = document.getElementsByClassName("form-row field-user")[0].innerText.split("\n")[1];
+        var user_name = document.getElementsByClassName("form-row field-user")[0].innerText.trim().split(":")[1].trim();
    }
    catch (e){
         setTimeout(() => { build_rule();}, 1000)
         return;
    }
   var action = document.getElementById("action").value;
   var protocol = document.getElementById("protocol").value;
@@ -40,14 +40,18 @@
   var dstportallow = document.getElementById("dstportallow").value;
   dstportallow = (dstportallow==="-----")? "" : dstportallow
   var group = document.getElementById("id_group")[document.getElementById("id_group").value];
   var name = document.getElementById("id_name").value;
   var id_document  = document.getElementById("id_document").value;
   var id_treatment = document.getElementById("id_treatment").value;
   var id_description = document.getElementById("id_description").value;
+  var id_tag = ""
+  if (document.getElementById("id_tag").checked === true) {
+  var id_tag = " tag:session,10,packets;"
+  }
   content = "";
   current_content = "";
   prev = null;
   for (let elem of document.getElementById("ruleform").childNodes) {
         if (elem.nodeType === 3||elem.tagName === "BR" ||elem.tagName === "IMG") // text node
         {
             continue;
@@ -120,10 +124,10 @@
   group = "";
   }
 
     id_content.value = id_content.textContent=action + " " + protocol + " " + srcipallow + srcip +" " +srcportallow+
     srcport + " " + direction + " " + dstipallow + dstip + " " + dstportallow + dstport
      + "(msg:" + group + " " + name+ ";" + content+ "sid:" +sigid +"; metadata: employee '"+
      user_name + "', group '" + group + "', name '" + name + "', treatment '" + id_treatment +
-      "', keywords 'None', date '"+date_now+"', document '" + id_document + "',description '"+id_description+"';)";
+      "', keywords 'None', date '"+date_now+"', document '" + id_document + "',description '"+id_description+"'; "+id_tag+")";
 };
 </script>
```

### Comparing `snort_web_master-0.2.1.1/data/templates/html/snortBuilder.html` & `snort_web_master-0.2.1.2/data/templates/html/snortBuilder.html`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 };
 
 </script>
 
 <script>
     function load_protocol(){
-const url_protocol="/settings/keywords/?stage=protocol&avalable=True";
+const url_protocol="/settings/keyword/?stage=protocol&available=True";
   const Http = new XMLHttpRequest();
 Http.open("GET", url_protocol);
 Http.responseType = "document";
 Http.send();
 Http.onreadystatechange = (e) => {
     var selection = document.getElementById("protocol");
     if (Http.responseXML!==null){
@@ -107,15 +107,15 @@
     else
     {
         Array.prototype.forEach.call(plus_dict[input_id], function(elem) {
             elem.remove()
         });
         plus_dict[input_id] = []
     }
-    const url_content_modifiers="/settings/keywords/?name=" + selection;
+    const url_content_modifiers="/settings/keyword/?name=" + selection;
     const Http = new XMLHttpRequest();
     selected_keyword = document.getElementById("keyword_selection" + current_index_i)
     selected_keyword_text = selected_keyword.options[selected_keyword.selectedIndex].text
     Http.open("GET", url_content_modifiers);
     Http.responseType = "document";
     Http.send();
     Http.onreadystatechange = (e) => {
@@ -125,19 +125,26 @@
             var els = Http.responseXML.getElementsByClassName("field-options")[0].textContent
             Array.prototype.forEach.call(els.split(","), function(splited) {
                 if (splited==="string"||splited==="int"){
                     var newElem = document.createElement("input");
                     newElem.onchange = function(){setTimeout(() => { build_rule();}, 50);};
                     newElem.oninput = function(){setTimeout(() => { build_rule();}, 50);};
                     newElem.name = newElem.id = input_id + "-data"
+                    if ((splited.toLowerCase() === "int")||(splited.toLowerCase() === "integer")){
+                            newElem.type = "number"
+                            newElem.step = 1
+                        }
+                        if (splited.toLowerCase() === "number"){
+                            newElem.type = "number"
+                        }
                     input.insertAdjacentElement("afterend", newElem);
                     if (plus_dict[input_id] === undefined){
                         plus_dict[current_index_i].push(newElem);
                         plus_dict[current_index_i][0].style.visibility = "visible";
-                        if (splited === "string"){
+                        if (splited.toLowerCase() === "string"){
                             input.style.visibility = "visible";
                         }
                         else
                         {
                         input.style.width = "0px"
                         input.style.padding = "0px 0px"
                         }
@@ -217,15 +224,15 @@
                 }
             });
         }else{
             manual=false;
         }
     }
     j[my_i] = 0
-    const url_modifiers="/settings/keywords/?stage={selected_keyword_text} Modifiers&avalable=True";
+    const url_modifiers="/settings/keyword/?stage={selected_keyword_text} Modifiers&available=True";
 
     var input_id3 = "keyword";
     var rule_form = document.getElementById("ruleform");
     var current_i = my_i;
     if (!manual)
     {
         var plus = document.createElement("img");
@@ -246,15 +253,15 @@
     let opt = document.createElement('option');
     opt.value = "-----";
     opt.textContent = "-----"
     input.onchange = function(){add_text_box_if_needed(input_id, input.options[input.selectedIndex].text, current_i, 0)};
     input.onblur= function(){setTimeout(() => { build_rule();}, 50);};
     input.appendChild(opt);
     //get option values
-    const url_options="/settings/keywords/?stage=options&avalable=True";
+    const url_options="/settings/keyword/?stage=options&available=True";
 
     // add not operation
     add_options_new_keyword(url_options, input_id, null, null, null)
     // add option to form
     rule_form.insertBefore(input, plus);
     if (!manual)
     {
@@ -510,14 +517,20 @@
         };
     document.getElementById("id_group").onchange = function(e){
             set_build_rule(e)
         };
     document.getElementById("id_group").onblur = function(e){
             set_build_rule(e)
         };
+    document.getElementById("id_tag").onchange = function(e){
+            set_build_rule(e)
+        };
+    document.getElementById("id_tag").onblur = function(e){
+            set_build_rule(e)
+        };
     document.getElementById("id_treatment").oninput = function(e){
             set_build_rule(e)
         };
     document.getElementById("id_treatment").onblur = function(e){
             set_build_rule(e)
         };
     document.getElementById("id_document").oninput = function(e){
@@ -630,9 +643,16 @@
 
 id_content.onblur = function(e){
   set_content_change(e)
 };
 id_content.oninput = function(e){
   set_content_change(e)
 };
+setTimeout(() => {
+    var field_user = document.getElementsByClassName("form-row field-user")[0];
+    field_user.style.display = "None";
+
+    if (document.getElementsByClassName("errorlist").length > 0){
+        document.getElementsByClassName("errorlist")[0].parentElement.scrollIntoView()
+    };}, 200)
 
 </script>
```

### Comparing `snort_web_master-0.2.1.1/snort_web_master/pcaps/admin.py` & `snort_web_master-0.2.1.2/snort_web_master/pcaps/admin.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/pcaps/migrations/0001_initial.py` & `snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/pcaps/migrations/0002_initial.py` & `snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py` & `snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py` & `snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/pcaps/models.py` & `snort_web_master-0.2.1.2/snort_web_master/pcaps/models.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/settings/admin.py` & `snort_web_master-0.2.1.2/snort_web_master/settings/admin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from django.contrib import admin
 from settings.models import Setting
 from settings.models import attackGroup
-from settings.models import keywords
+from settings.models import keyword
 # Register your models here.
 
 @admin.register(Setting)
 class SettingAdmin(admin.ModelAdmin):
     list_display = ['name', 'value']
 
 @admin.register(attackGroup)
 class attack_groupAdmin(admin.ModelAdmin):
     list_display = ['name', 'description']
 
 
-@admin.register(keywords)
+@admin.register(keyword)
 class keywords(admin.ModelAdmin):
-    list_display = ['name', 'stage', "options", "description"]
+    list_display = ['name', 'stage', "options", "description", "available"]
```

### Comparing `snort_web_master-0.2.1.1/snort_web_master/settings/migrations/0001_initial.py` & `snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py` & `snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/settings/migrations/0003_keywords_avalable.py` & `snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0003_keywords_avalable.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/settings/models.py` & `snort_web_master-0.2.1.2/snort_web_master/settings/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,22 +17,20 @@
     description = models.TextField(max_length=256)
     objects = models.Manager()
 
     def __str__(self):
         return self.name
 
 # Create your models here.
-class keywords(models.Model):
+class keyword(models.Model):
     """
     Model for site-wide settings.
     """
-    name = models.CharField(max_length=200, help_text="Name of site-wide variable")
-    stage = models.CharField(null=True, blank=True, max_length=100, help_text="Value of site-wide variable that scripts can reference")
-    description = models.CharField(null=True, blank=True, max_length=100, help_text="Value of site-wide variable that scripts can reference")
-    # negation = models.CharField(null=True, blank=True, max_length=100,
-    #                                help_text="Value of site-wide variable that scripts can reference")
+    name = models.CharField(max_length=200, help_text="keyword name")
+    stage = models.CharField(null=True, blank=True, max_length=100, help_text="where will the keyword element will appeare in snort builder")
+    description = models.CharField(null=True, blank=True, max_length=100, help_text="just a description")
     options = models.CharField(null=True, blank=True, max_length=100,
-                                help_text="Value of site-wide variable that scripts can reference")
-    avalable = models.CharField(null=True, blank=True, max_length=10,
-                                help_text="Value of site-wide variable that scripts can reference")
+                                help_text="what type of field is it, does it has sub fields")
+    available = models.BooleanField(default=False,
+                                help_text="is it available in snort builder")
     def __unicode__(self):
         return self.name
```

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort/admin.py` & `snort_web_master-0.2.1.2/snort_web_master/snort/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from django.db import transaction
 import suricataparser
 from snort.views import build_keyword_dict
 # Register your models here.
 from django.contrib import admin
 from django_object_actions import DjangoObjectActions
 import subprocess
-from settings.models import Setting, keywords, attackGroup
+from settings.models import Setting, keyword, attackGroup
 from django.shortcuts import render
 from pcaps.admin import verify_legal_pcap
 from advanced_filters.admin import AdminAdvancedFiltersMixin
 from django.core.files.storage import default_storage
 from django.core.files.base import ContentFile
 from django.conf import settings
 from datetime import datetime
@@ -53,16 +53,16 @@
 
 BASE_FIELDS = [
     "id", "active", "is_template", "deleted", "admin_locked", 'name', "document", "treatment", "description",
     "extra", "user"]
 FILTER_FIELDS = ("active", "is_template", "deleted", "admin_locked")
 ADVANCE_FILTER_FIELDS = tuple(i for i in BASE_FIELDS + ["content", ("pcap_sanity_check__name", "pcap_sanity_check_name"), ("pcap_legal_check__name", "pcap_legal_check_name"),("group_name", "group_name")])
 FIELDS = [
-    "id", "content", "active", "is_template", "deleted", "admin_locked", 'name', "document", "treatment", "snort_builder", "description",
-    "group", "extra", "user", "rule_validation_section",'pcap_sanity_check', "pcap_legal_check", ]
+    "id", "content", "active", "is_template", "deleted", "admin_locked", "tag",'name', "document", "treatment", "snort_builder", "description",
+    "extra", "user", 'pcap_sanity_check', "pcap_legal_check"]
 SEARCH_FIELDS = tuple(i for i in BASE_FIELDS + ["content", "pcap_sanity_check__name", "pcap_legal_check__name", "group__name"])
 BASE_BUILDER_KEY = ("action", "protocol", "srcipallow", "srcip", "srcportallow", "srcport", "direction", "dstipallow",
                     "dstportallow", "dstport")
 
 INPUT_TYPE = ("srcip" , "srcport", "dstip", "dstport")
 from django.core.cache import cache
 # todo: upload unmanaged rule file
@@ -82,15 +82,15 @@
     def clean_content(self):
         try:
             parser = Parser(self.data["content"])
             parser.parse_header()
             options = parser.parse_options()
             for option in options:
                 try:
-                    if keywords.objects.get(name=options[option][0]):
+                    if keyword.objects.get(name=options[option][0]):
                         break
                 except:
                     pass
             else:
                 raise Exception("no content; please add at least one keyword")
         except Exception as e:
             raise forms.ValidationError(e)
@@ -151,15 +151,14 @@
             else:
                 raise forms.ValidationError(
                     f"bad configuration setting (FORCE_LEGAL_CHECK), pleas edit setting(FORCE_LEGAL_CHECK) must be True or False")
 
         cur_rule = SnortRule()
         cur_rule.content = self.data.get("content")
         cur_rule.location = self.data.get("location")
-        cur_rule.group = self.data.get("group")
         cur_rule.id = self.data.get("id")
         cur_rule.treatment = self.data.get("treatment")
         cur_rule.name = self.data.get("name")
         cur_rule.type = self.data.get("type")
         cur_rule.user = getattr(self.current_user, self.current_user.USERNAME_FIELD)
         cur_rule.document = self.data.get("document")
 
@@ -289,29 +288,34 @@
                                .lower())
 
     with open(rule.location + ".tmp", "w") as rule_file:
         rule_file.write(rule.content)
     failed = True
     for pcap in pcaps:
         try:
-            if not verify_legal_pcap("/app/{pcap.pcap_file}"):
+            base = "/app/"
+            if os.name =="nt":
+                from django.conf import settings as s
+                base = str(s.BASE_DIR) + "/"
+
+            if not verify_legal_pcap(f"{base}{pcap.pcap_file}"):
                 raise Exception(f"illegal pcap file")
-            if not os.path.exists(f"/app/{pcap.pcap_file}"):
-                raise Exception(f"cant find file /app/{pcap.pcap_file}")
+            if not os.path.exists(f"{base}{pcap.pcap_file}"):
+                raise Exception(f"cant find file {base}{pcap.pcap_file}")
             stdout, stderr = subprocess.Popen(
-                ["/home/snorty/snort3/bin/snort", "-R", rule.location + ".tmp", "-r", f"/app/{pcap.pcap_file}", "-A",
+                ["/home/snorty/snort3/bin/snort", "-R", rule.location + ".tmp", "-r", f"{base}{pcap.pcap_file}", "-A",
                  "fast"], stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE).communicate()
             if stdout and not stderr:
                 if b"total_alerts: " in stdout:
                     return stdout.split(b"total_alerts: ")[1].split(b"\n")[0]
                 else:
                     return 0
         except Exception as e:
-            raise forms.ValidationError(f"could not validate rule on {pcap.pcap_file}: {e}", code=405)
+            raise forms.ValidationError(f"could not validate rule on {base}{pcap.pcap_file}: {e}", code=405)
     if failed:
         raise Exception("no rules was chosen")
     return stdout
 
 
 
 
@@ -321,25 +325,32 @@
     list_filter = FILTER_FIELDS  # simple list filters
 
     # specify which fields can be selected in the advanced filter
     # creation form
     advanced_filter_fields = ADVANCE_FILTER_FIELDS
     change_actions = ('clone_rule',)
     # changelist_actions = ('load_template',)
-    fields = FIELDS
+
+    FIELDS_GROUP = FIELDS
+    rule_validation_fields = ("pcap_sanity_check", "pcap_legal_check")
+    for field in rule_validation_fields:
+        if field in FIELDS_GROUP:
+            FIELDS_GROUP.remove(field)
+    fieldsets = (
+        (None, {"fields": FIELDS_GROUP}),
+        ("attackers", {"fields": ("group",)}),
+        ("Rule validation", {"fields": rule_validation_fields}),
+    )
     filter_horizontal = ('pcap_sanity_check', "pcap_legal_check")
     list_display_links = ("id", "user", "name", "content", "description")
     list_display = ("id", "user", "active", "name", "group", "description", "content", "date", "is_template", "deleted")
     search_fields = SEARCH_FIELDS
     form = SnortRuleAdminForm
     actions = ['make_published', "make_delete", "make_clone"]
 
-    def rule_validation_section(self, request):
-        return mark_safe('<hr style="height:3px;width:100%;border-width:100%;color:green;background-color:green"/>')
-
     def export_action(self, request):
         return self.export_data(SnortRule.objects.all())
 
     @transaction.atomic
     def import_action(self, request):
         errors = False
         if request.method == 'POST':
@@ -533,16 +544,16 @@
         if not set_rule:
             set_rule = SnortRuleViewArray.objects.filter(snortId=obj.id)
             cache.set(obj.id, set_rule)
         else:
             cache.set(obj.id, [])
         context = {}
         context["build_items"] = set_rule
-        context["actions"] = keywords.objects.filter(stage="action", avalable="True")
-        context["protocols"] = keywords.objects.filter(stage="protocol", avalable="True")
+        context["actions"] = keyword.objects.filter(stage="action", available="True")
+        context["protocols"] = keyword.objects.filter(stage="protocol", available="True")
 
         tmp_context = copy.deepcopy(self.request.session.get("cloned_rule", {}))
         self.request.session["cloned_rule"] = {}
         tmp_context.update(context)
 
 
         snort_buider_section = render(self.request, "html/snortBuilder.html", tmp_context).content.decode("utf-8")
@@ -551,14 +562,19 @@
 
     def get_form(self, request, *args, **kwargs):
         form = super(SnortRuleAdmin, self).get_form(request, **kwargs)
         form.current_user = request.user
         self.request = request
         form.base_fields["pcap_sanity_check"].help_text = "Hold down “Control” to select more than one."
         form.base_fields["pcap_legal_check"].help_text = "Hold down “Control” to select more than one."
+        atkgroup = form.base_fields["group"]
+        atkgroup.widget.can_add_related = Setting.objects.get_or_create(**{"name": "atkgroup_can_add_related"})[0].value == "True"
+        atkgroup.widget.can_change_related = Setting.objects.get_or_create(**{"name": "atkgroup_can_change_related"})[0].value == "True"
+        atkgroup.widget.can_delete_related = Setting.objects.get_or_create(**{"name": "atkgroup_can_delete_related"})[0].value == "True"
+        atkgroup.widget.can_view_related = Setting.objects.get_or_create(**{"name": "atkgroup_can_view_related"})[0].value == "True"
         return form
 
     @transaction.atomic
     def clone_rule(self, request, obj: SnortRule):
         return HttpResponseRedirect(f"/snort/snortrule/add/")
 
     clone_rule.label = "clone_rule"  # optional
@@ -569,9 +585,8 @@
             "id", "active", "user", "admin_locked", "snort_builder", "deleted", "rule_validation_section",)
         else:
             read_only_fields = ("id", "user", "admin_locked", "snort_builder", "deleted", "rule_validation_section")
 
         return read_only_fields
 
     # readonly_fields = ("id", "user", "admin_locked", "full_rule", "snort_builder", "deleted")
-    clone_rule.short_description = "clone rule to a new rule"  # optional
-
+    clone_rule.short_description = "clone rule to a new rule"  # optional
```

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort/migrations/0001_initial.py` & `snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort/migrations/0002_snortruleviewarray.py` & `snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0002_snortruleviewarray.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py` & `snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py` & `snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py` & `snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort/models.py` & `snort_web_master-0.2.1.2/snort_web_master/snort/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     treatment = models.CharField(max_length=12, blank=True)
     date = models.DateTimeField(auto_now=True)
     is_template = models.BooleanField(default=False)
     pcap_sanity_check = models.ManyToManyField("pcaps.Pcap", related_name='pcap_sanity_check', blank=True)
     pcap_legal_check = models.ManyToManyField("pcaps.white_Pcap", related_name='pcap_legal_check', blank=True)
     objects = models.Manager()
     deleted = models.BooleanField(default=False)
+    tag = models.BooleanField(default=True, help_text="add 'tag:session,10,packets' to rule")
 
     def delete(self):
         self.active = False
         self.deleted = True
         self.save()
     class Meta:
         ordering = ("name", "type", "date")
```

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort/parser.py` & `snort_web_master-0.2.1.2/snort_web_master/snort/parser.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort/snort_templates.py` & `snort_web_master-0.2.1.2/snort_web_master/snort/snort_templates.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort/tests.py` & `snort_web_master-0.2.1.2/snort_web_master/snort/tests.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort/views.py` & `snort_web_master-0.2.1.2/snort_web_master/snort/views.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort_web_master/middleware/no_cache.py` & `snort_web_master-0.2.1.2/snort_web_master/snort_web_master/middleware/no_cache.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort_web_master/settings.py` & `snort_web_master-0.2.1.2/snort_web_master/snort_web_master/settings.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort_web_master/urls.py` & `snort_web_master-0.2.1.2/snort_web_master/snort_web_master/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 """
 from django.contrib import admin
 from django.urls import path, include
 from django.shortcuts import redirect
 from snort.views import get_rule, get_rule_keys, build_rule_keyword_to_rule, build_rule_rule_to_keywords, favico,get_current_user_name
 from django.conf import settings
 from django.conf.urls.static import static
-
+import django.contrib.auth.admin
+django.contrib.auth.admin.UserAdmin.readonly_fields= ("last_login", 'date_joined')
 admin.site.site_header = 'snort web master'
 app_name = "snort_web_master"
 urlpatterns = [
     path("favicon.ico", favico),
     path("get_rule_update/<int:rule_id>/", get_rule, name="get_rule_update"),
     path("get_rule_keywords/<int:rule_id>/", get_rule_keys,name="get_rule_keywords"),
     path('advanced_filters/', include("advanced_filters.urls"), name="advance_filter"),
```

### Comparing `snort_web_master-0.2.1.1/snort_web_master/snort_web_master.egg-info/SOURCES.txt` & `snort_web_master-0.2.1.2/snort_web_master/snort_web_master.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 data/dicts.py
 data/dockercompose
 data/favicon.ico
 data/migrate sqllite to postgresql
 data/my-snort-rule.tmp
 data/requirements.txt
 data/snortFile
+data/admin/0004_keyword_delete_keywords.py
 data/admin/image/images.png
 data/nginx/nginx
 data/nginx/nginx.conf
 data/templates/html/full_rule.html
 data/templates/html/import.html
 data/templates/html/snortBuilder.html
 snort_web_master/pcaps/__init__.py
@@ -33,15 +34,16 @@
 snort_web_master/settings/apps.py
 snort_web_master/settings/models.py
 snort_web_master/settings/tests.py
 snort_web_master/settings/views.py
 snort_web_master/settings/migrations/0001_initial.py
 snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py
 snort_web_master/settings/migrations/0003_keywords_avalable.py
-snort_web_master/settings/migrations/0004_remove_keywords_negation.py
+snort_web_master/settings/migrations/0004_keyword_delete_keywords.py
+snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py
 snort_web_master/settings/migrations/__init__.py
 snort_web_master/snort/__init__.py
 snort_web_master/snort/admin.py
 snort_web_master/snort/apps.py
 snort_web_master/snort/models.py
 snort_web_master/snort/parser.py
 snort_web_master/snort/snort_templates.py
@@ -49,14 +51,15 @@
 snort_web_master/snort/views.py
 snort_web_master/snort/migrations/0001_initial.py
 snort_web_master/snort/migrations/0002_snortruleviewarray.py
 snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py
 snort_web_master/snort/migrations/0004_snortrule_deleted.py
 snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py
 snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py
+snort_web_master/snort/migrations/0007_snortrule_tag.py
 snort_web_master/snort/migrations/__init__.py
 snort_web_master/snort_web_master/__init__.py
 snort_web_master/snort_web_master/asgi.py
 snort_web_master/snort_web_master/settings.py
 snort_web_master/snort_web_master/urls.py
 snort_web_master/snort_web_master/wsgi.py
 snort_web_master/snort_web_master.egg-info/PKG-INFO
```

