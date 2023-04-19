# Comparing `tmp/rapidpro-dash-1.9.2.tar.gz` & `tmp/rapidpro-dash-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpro-dash-1.9.2.tar", max compression
+gzip compressed data, was "rapidpro-dash-1.9.3.tar", max compression
```

## Comparing `rapidpro-dash-1.9.2.tar` & `rapidpro-dash-1.9.3.tar`

### file list

```diff
@@ -1,145 +1,145 @@
--rw-r--r--   0        0        0     1476 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/LICENSE
--rw-r--r--   0        0        0       22 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/__init__.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/__init__.py
--rw-r--r--   0        0        0      163 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/fields.py
--rw-r--r--   0        0        0     2515 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/migrations/0001_initial.py
--rw-r--r--   0        0        0     1030 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/migrations/0002_auto_20140820_1415.py
--rw-r--r--   0        0        0     2273 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/migrations/0003_categoryimage.py
--rw-r--r--   0        0        0      831 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/migrations/0004_auto_20140904_0927.py
--rw-r--r--   0        0        0     2103 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/migrations/0005_auto_20140922_1514.py
--rw-r--r--   0        0        0      511 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/migrations/0006_auto_20141008_1955.py
--rw-r--r--   0        0        0     1567 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/migrations/0007_auto_20170301_0914.py
--rw-r--r--   0        0        0      387 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/migrations/0008_alter_category_options.py
--rw-r--r--   0        0        0      977 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/migrations/0009_auto_20210910_1450.py
--rw-r--r--   0        0        0     1999 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/migrations/0010_alter_category_created_by_alter_category_modified_by_and_more.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/migrations/__init__.py
--rw-r--r--   0        0        0     2021 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/models.py
--rw-r--r--   0        0        0      862 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/templates/categories/categoryimage_list.haml
--rw-r--r--   0        0        0      133 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/urls.py
--rw-r--r--   0        0        0     3142 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/categories/views.py
--rw-r--r--   0        0        0      413 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/context_processors.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/dashblocks/__init__.py
--rw-r--r--   0        0        0    11152 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/dashblocks/migrations/0001_initial.py
--rw-r--r--   0        0        0     1908 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/dashblocks/migrations/0002_auto_20140802_2112.py
--rw-r--r--   0        0        0     1012 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/dashblocks/migrations/0003_auto_20140804_0236.py
--rw-r--r--   0        0        0     1448 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/dashblocks/migrations/0004_auto_20140902_1200.py
--rw-r--r--   0        0        0     1014 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/dashblocks/migrations/0005_auto_20140904_0957.py
--rw-r--r--   0        0        0     2771 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/dashblocks/migrations/0006_auto_20140922_1514.py
--rw-r--r--   0        0        0     2259 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/dashblocks/migrations/0007_auto_20170301_0914.py
--rw-r--r--   0        0        0      497 2022-01-14 20:40:35.774517 rapidpro-dash-1.9.2/dash/dashblocks/migrations/0008_auto_20210902_1125.py
--rw-r--r--   0        0        0     1026 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/migrations/0009_auto_20210910_1450.py
--rw-r--r--   0        0        0     2823 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/migrations/0010_alter_dashblock_created_by_and_more.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/migrations/__init__.py
--rw-r--r--   0        0        0     5922 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/models.py
--rwxr-xr-x   0        0        0    16746 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/static/css/font/summernote.eot
--rwxr-xr-x   0        0        0    16560 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/static/css/font/summernote.ttf
--rwxr-xr-x   0        0        0    10324 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/static/css/font/summernote.woff
--rwxr-xr-x   0        0        0    18395 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/static/css/summernote.css
--rwxr-xr-x   0        0        0   122966 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/static/js/summernote.min.js
--rw-r--r--   0        0        0       43 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/templates/dashblocks/dashblock_create.haml
--rw-r--r--   0        0        0     1525 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/templates/dashblocks/dashblock_form.haml
--rw-r--r--   0        0        0     1554 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/templates/dashblocks/dashblock_list.haml
--rw-r--r--   0        0        0       43 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/templates/dashblocks/dashblock_update.haml
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/templatetags/__init__.py
--rw-r--r--   0        0        0     2121 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/templatetags/dashblocks.py
--rw-r--r--   0        0        0      194 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/urls.py
--rw-r--r--   0        0        0     8627 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/dashblocks/views.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/__init__.py
--rw-r--r--   0        0        0     2453 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/context_processors.py
--rw-r--r--   0        0        0     2038 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/forms.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/management/__init__.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/management/commands/__init__.py
--rw-r--r--   0        0        0     3800 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/management/commands/orgtasks.py
--rw-r--r--   0        0        0     5863 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/middleware.py
--rw-r--r--   0        0        0     6623 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0001_initial.py
--rw-r--r--   0        0        0      580 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0002_auto_20140802_2104.py
--rw-r--r--   0        0        0      543 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0003_org_logo.py
--rw-r--r--   0        0        0     1082 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0004_auto_20140804_1453.py
--rw-r--r--   0        0        0     2771 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0005_orgbackground.py
--rw-r--r--   0        0        0      601 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0006_auto_20140919_2056.py
--rw-r--r--   0        0        0     4336 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0007_auto_20140922_1514.py
--rw-r--r--   0        0        0      416 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0008_org_timezone.py
--rw-r--r--   0        0        0      672 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0009_auto_20150331_1452.py
--rw-r--r--   0        0        0      685 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0010_auto_20150618_1042.py
--rw-r--r--   0        0        0      678 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0011_auto_20150710_1612.py
--rw-r--r--   0        0        0      503 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0012_auto_20150715_1816.py
--rw-r--r--   0        0        0      543 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0013_auto_20150715_1831.py
--rw-r--r--   0        0        0     1417 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0014_auto_20150722_1419.py
--rw-r--r--   0        0        0     1036 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0015_auto_20160209_0926.py
--rw-r--r--   0        0        0      306 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0016_taskstate_is_disabled.py
--rw-r--r--   0        0        0      542 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0017_auto_20161026_1513.py
--rw-r--r--   0        0        0     2308 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0018_auto_20170301_0914.py
--rw-r--r--   0        0        0     1007 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0019_restructure_org_config.py
--rw-r--r--   0        0        0      291 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0020_remove_org_api_token.py
--rw-r--r--   0        0        0      602 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0021_auto_20180315_0823.py
--rw-r--r--   0        0        0     1180 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0022_populate_rapidpro_specific_config.py
--rw-r--r--   0        0        0     2975 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0023_orgbackend.py
--rw-r--r--   0        0        0     1607 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0024_populate_org_backend.py
--rw-r--r--   0        0        0     1012 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0025_auto_20180322_1415.py
--rw-r--r--   0        0        0      983 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0026_fix_org_config_rapidpro.py
--rw-r--r--   0        0        0      344 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0027_alter_org_options.py
--rw-r--r--   0        0        0      522 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0028_alter_org_config.py
--rw-r--r--   0        0        0      945 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0029_auto_20211025_1504.py
--rw-r--r--   0        0        0     3611 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/0030_alter_invitation_created_by_and_more.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/migrations/__init__.py
--rw-r--r--   0        0        0    12313 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/models.py
--rw-r--r--   0        0        0     4170 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/tasks.py
--rw-r--r--   0        0        0     2528 2022-01-14 20:40:35.778518 rapidpro-dash-1.9.2/dash/orgs/templates/email_base.html
--rw-r--r--   0        0        0      388 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/orgs/templates/orgs/email/invitation_email.html
--rw-r--r--   0        0        0      181 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/orgs/templates/orgs/email/invitation_email.txt
--rw-r--r--   0        0        0      137 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/orgs/templates/orgs/org_chooser.haml
--rw-r--r--   0        0        0      763 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/orgs/templates/orgs/org_home.haml
--rw-r--r--   0        0        0     3408 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/orgs/templates/orgs/org_manage_accounts.haml
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/orgs/templatetags/__init__.py
--rw-r--r--   0        0        0      894 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/orgs/templatetags/dashorgs.py
--rw-r--r--   0        0        0      234 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/orgs/urls.py
--rw-r--r--   0        0        0    27848 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/orgs/views.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/__init__.py
--rw-r--r--   0        0        0     3246 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0001_initial.py
--rw-r--r--   0        0        0      507 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0002_auto_20140805_1158.py
--rw-r--r--   0        0        0      427 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0003_story_summary.py
--rw-r--r--   0        0        0      424 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0004_auto_20140806_1540.py
--rw-r--r--   0        0        0      621 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0005_story_category.py
--rw-r--r--   0        0        0      594 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0006_auto_20140821_0859.py
--rw-r--r--   0        0        0     2200 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0007_storyimage.py
--rw-r--r--   0        0        0      692 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0008_auto_20140912_0524.py
--rw-r--r--   0        0        0      246 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0009_remove_story_image.py
--rw-r--r--   0        0        0     2473 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0010_auto_20140922_1514.py
--rw-r--r--   0        0        0      461 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0011_story_audio_link.py
--rw-r--r--   0        0        0      407 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0012_story_written_by.py
--rw-r--r--   0        0        0     1625 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0013_auto_20170301_0914.py
--rw-r--r--   0        0        0      575 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0014_alter_storyimage_image.py
--rw-r--r--   0        0        0      745 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0015_story_attachment.py
--rw-r--r--   0        0        0     1982 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/0016_alter_story_created_by_alter_story_modified_by_and_more.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/migrations/__init__.py
--rw-r--r--   0        0        0     4910 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/models.py
--rw-r--r--   0        0        0      541 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/templates/stories/story_create.haml
--rw-r--r--   0        0        0      116 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/templates/stories/story_list.haml
--rw-r--r--   0        0        0      542 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/templates/stories/story_update.haml
--rw-r--r--   0        0        0       71 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/urls.py
--rw-r--r--   0        0        0     5955 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/stories/views.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/tags/__init__.py
--rw-r--r--   0        0        0     2774 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/tags/migrations/0001_initial.py
--rw-r--r--   0        0        0     1152 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/tags/migrations/0002_alter_tag_created_by_alter_tag_modified_by.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/tags/migrations/__init__.py
--rw-r--r--   0        0        0      438 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/tags/models.py
--rw-r--r--   0        0        0       69 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/tags/urls.py
--rw-r--r--   0        0        0     1349 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/tags/views.py
--rw-r--r--   0        0        0     4341 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/test.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/users/__init__.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/users/models.py
--rw-r--r--   0        0        0      591 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/users/urls.py
--rw-r--r--   0        0        0     1096 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/users/views.py
--rw-r--r--   0        0        0     5013 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/utils/__init__.py
--rw-r--r--   0        0        0      642 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/utils/email.py
--rw-r--r--   0        0        0     1941 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/utils/haml.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/utils/management/__init__.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/utils/management/commands/__init__.py
--rw-r--r--   0        0        0      300 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/utils/management/commands/hamlcompress.py
--rw-r--r--   0        0        0     8670 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/utils/sync.py
--rw-r--r--   0        0        0        0 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/utils/templatetags/__init__.py
--rw-r--r--   0        0        0      346 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/utils/templatetags/utils.py
--rw-r--r--   0        0        0     4861 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/dash/utils/tests.py
--rw-r--r--   0        0        0     1162 2022-01-14 20:40:35.782518 rapidpro-dash-1.9.2/pyproject.toml
--rw-r--r--   0        0        0     1782 2022-01-14 20:40:51.618448 rapidpro-dash-1.9.2/setup.py
--rw-r--r--   0        0        0     1344 2022-01-14 20:40:51.618795 rapidpro-dash-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1476 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/LICENSE
+-rw-r--r--   0        0        0       22 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/__init__.py
+-rw-r--r--   0        0        0      163 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/fields.py
+-rw-r--r--   0        0        0     2515 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1030 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/migrations/0002_auto_20140820_1415.py
+-rw-r--r--   0        0        0     2273 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/migrations/0003_categoryimage.py
+-rw-r--r--   0        0        0      831 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/migrations/0004_auto_20140904_0927.py
+-rw-r--r--   0        0        0     2103 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/migrations/0005_auto_20140922_1514.py
+-rw-r--r--   0        0        0      511 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/migrations/0006_auto_20141008_1955.py
+-rw-r--r--   0        0        0     1567 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/migrations/0007_auto_20170301_0914.py
+-rw-r--r--   0        0        0      387 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/migrations/0008_alter_category_options.py
+-rw-r--r--   0        0        0      977 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/migrations/0009_auto_20210910_1450.py
+-rw-r--r--   0        0        0     1999 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/migrations/0010_alter_category_created_by_alter_category_modified_by_and_more.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/migrations/__init__.py
+-rw-r--r--   0        0        0     2021 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/models.py
+-rw-r--r--   0        0        0      862 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/templates/categories/categoryimage_list.haml
+-rw-r--r--   0        0        0      133 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/urls.py
+-rw-r--r--   0        0        0     3142 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/categories/views.py
+-rw-r--r--   0        0        0      413 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/context_processors.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/__init__.py
+-rw-r--r--   0        0        0    11152 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1908 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/migrations/0002_auto_20140802_2112.py
+-rw-r--r--   0        0        0     1012 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/migrations/0003_auto_20140804_0236.py
+-rw-r--r--   0        0        0     1448 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/migrations/0004_auto_20140902_1200.py
+-rw-r--r--   0        0        0     1014 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/migrations/0005_auto_20140904_0957.py
+-rw-r--r--   0        0        0     2771 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/migrations/0006_auto_20140922_1514.py
+-rw-r--r--   0        0        0     2259 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/migrations/0007_auto_20170301_0914.py
+-rw-r--r--   0        0        0      497 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/migrations/0008_auto_20210902_1125.py
+-rw-r--r--   0        0        0     1026 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/migrations/0009_auto_20210910_1450.py
+-rw-r--r--   0        0        0     2823 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/migrations/0010_alter_dashblock_created_by_and_more.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/migrations/__init__.py
+-rw-r--r--   0        0        0     5922 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/models.py
+-rwxr-xr-x   0        0        0    16746 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/static/css/font/summernote.eot
+-rwxr-xr-x   0        0        0    16560 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/static/css/font/summernote.ttf
+-rwxr-xr-x   0        0        0    10324 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/static/css/font/summernote.woff
+-rwxr-xr-x   0        0        0    18395 2022-04-05 09:42:58.745822 rapidpro-dash-1.9.3/dash/dashblocks/static/css/summernote.css
+-rwxr-xr-x   0        0        0   122966 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/dashblocks/static/js/summernote.min.js
+-rw-r--r--   0        0        0       43 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/dashblocks/templates/dashblocks/dashblock_create.haml
+-rw-r--r--   0        0        0     1525 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/dashblocks/templates/dashblocks/dashblock_form.haml
+-rw-r--r--   0        0        0     1554 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/dashblocks/templates/dashblocks/dashblock_list.haml
+-rw-r--r--   0        0        0       43 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/dashblocks/templates/dashblocks/dashblock_update.haml
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/dashblocks/templatetags/__init__.py
+-rw-r--r--   0        0        0     2366 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/dashblocks/templatetags/dashblocks.py
+-rw-r--r--   0        0        0      194 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/dashblocks/urls.py
+-rw-r--r--   0        0        0     8627 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/dashblocks/views.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/__init__.py
+-rw-r--r--   0        0        0     2138 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/context_processors.py
+-rw-r--r--   0        0        0     2038 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/forms.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/management/commands/__init__.py
+-rw-r--r--   0        0        0     3800 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/management/commands/orgtasks.py
+-rw-r--r--   0        0        0     5863 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/middleware.py
+-rw-r--r--   0        0        0     6623 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0001_initial.py
+-rw-r--r--   0        0        0      580 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0002_auto_20140802_2104.py
+-rw-r--r--   0        0        0      543 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0003_org_logo.py
+-rw-r--r--   0        0        0     1082 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0004_auto_20140804_1453.py
+-rw-r--r--   0        0        0     2771 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0005_orgbackground.py
+-rw-r--r--   0        0        0      601 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0006_auto_20140919_2056.py
+-rw-r--r--   0        0        0     4336 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0007_auto_20140922_1514.py
+-rw-r--r--   0        0        0      416 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0008_org_timezone.py
+-rw-r--r--   0        0        0      672 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0009_auto_20150331_1452.py
+-rw-r--r--   0        0        0      685 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0010_auto_20150618_1042.py
+-rw-r--r--   0        0        0      678 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0011_auto_20150710_1612.py
+-rw-r--r--   0        0        0      503 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0012_auto_20150715_1816.py
+-rw-r--r--   0        0        0      543 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0013_auto_20150715_1831.py
+-rw-r--r--   0        0        0     1417 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0014_auto_20150722_1419.py
+-rw-r--r--   0        0        0     1036 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0015_auto_20160209_0926.py
+-rw-r--r--   0        0        0      306 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0016_taskstate_is_disabled.py
+-rw-r--r--   0        0        0      542 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0017_auto_20161026_1513.py
+-rw-r--r--   0        0        0     2308 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0018_auto_20170301_0914.py
+-rw-r--r--   0        0        0     1007 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0019_restructure_org_config.py
+-rw-r--r--   0        0        0      291 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0020_remove_org_api_token.py
+-rw-r--r--   0        0        0      602 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0021_auto_20180315_0823.py
+-rw-r--r--   0        0        0     1180 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0022_populate_rapidpro_specific_config.py
+-rw-r--r--   0        0        0     2975 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0023_orgbackend.py
+-rw-r--r--   0        0        0     1607 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0024_populate_org_backend.py
+-rw-r--r--   0        0        0     1012 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0025_auto_20180322_1415.py
+-rw-r--r--   0        0        0      983 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0026_fix_org_config_rapidpro.py
+-rw-r--r--   0        0        0      344 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0027_alter_org_options.py
+-rw-r--r--   0        0        0      522 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0028_alter_org_config.py
+-rw-r--r--   0        0        0      945 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0029_auto_20211025_1504.py
+-rw-r--r--   0        0        0     3611 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/0030_alter_invitation_created_by_and_more.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/migrations/__init__.py
+-rw-r--r--   0        0        0    12313 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/models.py
+-rw-r--r--   0        0        0     4170 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/tasks.py
+-rw-r--r--   0        0        0     2528 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/templates/email_base.html
+-rw-r--r--   0        0        0      388 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/templates/orgs/email/invitation_email.html
+-rw-r--r--   0        0        0      181 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/templates/orgs/email/invitation_email.txt
+-rw-r--r--   0        0        0      137 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/templates/orgs/org_chooser.haml
+-rw-r--r--   0        0        0      763 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/templates/orgs/org_home.haml
+-rw-r--r--   0        0        0     3408 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/templates/orgs/org_manage_accounts.haml
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/templatetags/__init__.py
+-rw-r--r--   0        0        0      894 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/templatetags/dashorgs.py
+-rw-r--r--   0        0        0      234 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/urls.py
+-rw-r--r--   0        0        0    27848 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/orgs/views.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/__init__.py
+-rw-r--r--   0        0        0     3246 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0001_initial.py
+-rw-r--r--   0        0        0      507 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0002_auto_20140805_1158.py
+-rw-r--r--   0        0        0      427 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0003_story_summary.py
+-rw-r--r--   0        0        0      424 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0004_auto_20140806_1540.py
+-rw-r--r--   0        0        0      621 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0005_story_category.py
+-rw-r--r--   0        0        0      594 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0006_auto_20140821_0859.py
+-rw-r--r--   0        0        0     2200 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0007_storyimage.py
+-rw-r--r--   0        0        0      692 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0008_auto_20140912_0524.py
+-rw-r--r--   0        0        0      246 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0009_remove_story_image.py
+-rw-r--r--   0        0        0     2473 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0010_auto_20140922_1514.py
+-rw-r--r--   0        0        0      461 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0011_story_audio_link.py
+-rw-r--r--   0        0        0      407 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0012_story_written_by.py
+-rw-r--r--   0        0        0     1625 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0013_auto_20170301_0914.py
+-rw-r--r--   0        0        0      575 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0014_alter_storyimage_image.py
+-rw-r--r--   0        0        0      745 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0015_story_attachment.py
+-rw-r--r--   0        0        0     1982 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/0016_alter_story_created_by_alter_story_modified_by_and_more.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/migrations/__init__.py
+-rw-r--r--   0        0        0     5642 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/models.py
+-rw-r--r--   0        0        0      541 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/templates/stories/story_create.haml
+-rw-r--r--   0        0        0      116 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/templates/stories/story_list.haml
+-rw-r--r--   0        0        0      542 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/templates/stories/story_update.haml
+-rw-r--r--   0        0        0       71 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/urls.py
+-rw-r--r--   0        0        0     5955 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/stories/views.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/tags/__init__.py
+-rw-r--r--   0        0        0     2774 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/tags/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1152 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/tags/migrations/0002_alter_tag_created_by_alter_tag_modified_by.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/tags/migrations/__init__.py
+-rw-r--r--   0        0        0      438 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/tags/models.py
+-rw-r--r--   0        0        0       69 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/tags/urls.py
+-rw-r--r--   0        0        0     1349 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/tags/views.py
+-rw-r--r--   0        0        0     4341 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/test.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/users/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/users/models.py
+-rw-r--r--   0        0        0      591 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/users/urls.py
+-rw-r--r--   0        0        0     1096 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/users/views.py
+-rw-r--r--   0        0        0     5013 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/utils/__init__.py
+-rw-r--r--   0        0        0      642 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/utils/email.py
+-rw-r--r--   0        0        0     1941 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/utils/haml.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/utils/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/utils/management/commands/__init__.py
+-rw-r--r--   0        0        0      300 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/utils/management/commands/hamlcompress.py
+-rw-r--r--   0        0        0     8670 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/utils/sync.py
+-rw-r--r--   0        0        0        0 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/utils/templatetags/__init__.py
+-rw-r--r--   0        0        0      346 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/utils/templatetags/utils.py
+-rw-r--r--   0        0        0     4861 2022-04-05 09:42:58.749822 rapidpro-dash-1.9.3/dash/utils/tests.py
+-rw-r--r--   0        0        0     1162 2022-04-05 09:42:58.753822 rapidpro-dash-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0     1782 2022-04-05 09:43:07.343271 rapidpro-dash-1.9.3/setup.py
+-rw-r--r--   0        0        0     1344 2022-04-05 09:43:07.343580 rapidpro-dash-1.9.3/PKG-INFO
```

### Comparing `rapidpro-dash-1.9.2/LICENSE` & `rapidpro-dash-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/categories/migrations/0001_initial.py` & `rapidpro-dash-1.9.3/dash/categories/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/categories/migrations/0002_auto_20140820_1415.py` & `rapidpro-dash-1.9.3/dash/categories/migrations/0002_auto_20140820_1415.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/categories/migrations/0003_categoryimage.py` & `rapidpro-dash-1.9.3/dash/categories/migrations/0003_categoryimage.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/categories/migrations/0004_auto_20140904_0927.py` & `rapidpro-dash-1.9.3/dash/categories/migrations/0004_auto_20140904_0927.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/categories/migrations/0005_auto_20140922_1514.py` & `rapidpro-dash-1.9.3/dash/categories/migrations/0005_auto_20140922_1514.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/categories/migrations/0007_auto_20170301_0914.py` & `rapidpro-dash-1.9.3/dash/categories/migrations/0007_auto_20170301_0914.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/categories/migrations/0009_auto_20210910_1450.py` & `rapidpro-dash-1.9.3/dash/categories/migrations/0009_auto_20210910_1450.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/categories/migrations/0010_alter_category_created_by_alter_category_modified_by_and_more.py` & `rapidpro-dash-1.9.3/dash/categories/migrations/0010_alter_category_created_by_alter_category_modified_by_and_more.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/categories/models.py` & `rapidpro-dash-1.9.3/dash/categories/models.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/categories/templates/categories/categoryimage_list.haml` & `rapidpro-dash-1.9.3/dash/categories/templates/categories/categoryimage_list.haml`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/categories/views.py` & `rapidpro-dash-1.9.3/dash/categories/views.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/migrations/0001_initial.py` & `rapidpro-dash-1.9.3/dash/dashblocks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/migrations/0002_auto_20140802_2112.py` & `rapidpro-dash-1.9.3/dash/dashblocks/migrations/0002_auto_20140802_2112.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/migrations/0003_auto_20140804_0236.py` & `rapidpro-dash-1.9.3/dash/dashblocks/migrations/0003_auto_20140804_0236.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/migrations/0004_auto_20140902_1200.py` & `rapidpro-dash-1.9.3/dash/dashblocks/migrations/0004_auto_20140902_1200.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/migrations/0005_auto_20140904_0957.py` & `rapidpro-dash-1.9.3/dash/dashblocks/migrations/0005_auto_20140904_0957.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/migrations/0006_auto_20140922_1514.py` & `rapidpro-dash-1.9.3/dash/dashblocks/migrations/0006_auto_20140922_1514.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/migrations/0007_auto_20170301_0914.py` & `rapidpro-dash-1.9.3/dash/dashblocks/migrations/0007_auto_20170301_0914.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/migrations/0009_auto_20210910_1450.py` & `rapidpro-dash-1.9.3/dash/dashblocks/migrations/0009_auto_20210910_1450.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/migrations/0010_alter_dashblock_created_by_and_more.py` & `rapidpro-dash-1.9.3/dash/dashblocks/migrations/0010_alter_dashblock_created_by_and_more.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/models.py` & `rapidpro-dash-1.9.3/dash/dashblocks/models.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/static/css/font/summernote.eot` & `rapidpro-dash-1.9.3/dash/dashblocks/static/css/font/summernote.eot`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/static/css/font/summernote.ttf` & `rapidpro-dash-1.9.3/dash/dashblocks/static/css/font/summernote.ttf`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/static/css/font/summernote.woff` & `rapidpro-dash-1.9.3/dash/dashblocks/static/css/font/summernote.woff`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/static/css/summernote.css` & `rapidpro-dash-1.9.3/dash/dashblocks/static/css/summernote.css`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/static/js/summernote.min.js` & `rapidpro-dash-1.9.3/dash/dashblocks/static/js/summernote.min.js`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/templates/dashblocks/dashblock_form.haml` & `rapidpro-dash-1.9.3/dash/dashblocks/templates/dashblocks/dashblock_form.haml`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/templates/dashblocks/dashblock_list.haml` & `rapidpro-dash-1.9.3/dash/dashblocks/templates/dashblocks/dashblock_list.haml`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/templatetags/dashblocks.py` & `rapidpro-dash-1.9.3/dash/dashblocks/templatetags/dashblocks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django import template
 from django.conf import settings
+from django.db.models import Prefetch
 
 from dash.dashblocks.models import DashBlock, DashBlockType
 
 """
 This module offers one templatetag called ``load_dashblocks``.
 
 ``load_dashblocks`` does a query for all active DashBlock objects
@@ -51,26 +52,36 @@
 
 
 @register.simple_tag(takes_context=True)
 def load_dashblocks(context, org, slug, tag=None):
     if not org:
         return ""
 
-    try:
-        dashblock_type = DashBlockType.objects.get(slug=slug)
-    except DashBlockType.DoesNotExist:
+    dashblocks_qs = DashBlock.objects.filter(org=org, is_active=True).order_by("-priority")
+    # filter by our tag if one was specified
+    if tag is not None:
+        dashblocks_qs = dashblocks_qs.filter(tags__icontains=tag)
+
+    dashblock_type = (
+        DashBlockType.objects.filter(slug=slug)
+        .prefetch_related(
+            Prefetch(
+                "dashblock_set",
+                queryset=dashblocks_qs,
+                to_attr="prefetch_dashblocks",
+            )
+        )
+        .first()
+    )
+
+    if not dashblock_type:
         default_invalid = '<b><font color="red">DashBlockType with slug: %s not found</font></b>'
         return getattr(settings, "DASHBLOCK_STRING_IF_INVALID", default_invalid) % slug
 
-    dashblocks = DashBlock.objects.filter(dashblock_type=dashblock_type, org=org, is_active=True)
-    dashblocks = dashblocks.order_by("-priority")
-
-    # filter by our tag if one was specified
-    if tag is not None:
-        dashblocks = dashblocks.filter(tags__icontains=tag)
+    dashblocks = dashblock_type.prefetch_dashblocks
 
     context[slug] = dashblocks
 
     return ""
 
 
 @register.simple_tag(takes_context=True)
```

### Comparing `rapidpro-dash-1.9.2/dash/dashblocks/views.py` & `rapidpro-dash-1.9.3/dash/dashblocks/views.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/context_processors.py` & `rapidpro-dash-1.9.3/dash/orgs/context_processors.py`

 * *Files 22% similar despite different names*

```diff
@@ -68,15 +68,11 @@
 def set_org_processor(request):
     """
     Simple context processor that automatically sets 'org' on the context if it
     is present in the request.
     """
     if getattr(request, "org", None):
         org = request.org
-        pattern_bg = org.backgrounds.filter(is_active=True, background_type="P")
-        pattern_bg = pattern_bg.order_by("-pk").first()
-        banner_bg = org.backgrounds.filter(is_active=True, background_type="B")
-        banner_bg = banner_bg.order_by("-pk").first()
 
-        return dict(org=org, pattern_bg=pattern_bg, banner_bg=banner_bg)
+        return dict(org=org)
     else:
         return dict()
```

### Comparing `rapidpro-dash-1.9.2/dash/orgs/forms.py` & `rapidpro-dash-1.9.3/dash/orgs/forms.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/management/commands/orgtasks.py` & `rapidpro-dash-1.9.3/dash/orgs/management/commands/orgtasks.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/middleware.py` & `rapidpro-dash-1.9.3/dash/orgs/middleware.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0001_initial.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0002_auto_20140802_2104.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0002_auto_20140802_2104.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0003_org_logo.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0003_org_logo.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0004_auto_20140804_1453.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0004_auto_20140804_1453.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0005_orgbackground.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0005_orgbackground.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0006_auto_20140919_2056.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0006_auto_20140919_2056.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0007_auto_20140922_1514.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0007_auto_20140922_1514.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0009_auto_20150331_1452.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0009_auto_20150331_1452.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0010_auto_20150618_1042.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0010_auto_20150618_1042.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0011_auto_20150710_1612.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0011_auto_20150710_1612.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0013_auto_20150715_1831.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0013_auto_20150715_1831.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0014_auto_20150722_1419.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0014_auto_20150722_1419.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0015_auto_20160209_0926.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0015_auto_20160209_0926.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0017_auto_20161026_1513.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0017_auto_20161026_1513.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0018_auto_20170301_0914.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0018_auto_20170301_0914.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0019_restructure_org_config.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0019_restructure_org_config.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0021_auto_20180315_0823.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0021_auto_20180315_0823.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0022_populate_rapidpro_specific_config.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0022_populate_rapidpro_specific_config.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0023_orgbackend.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0023_orgbackend.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0024_populate_org_backend.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0024_populate_org_backend.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0025_auto_20180322_1415.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0025_auto_20180322_1415.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0026_fix_org_config_rapidpro.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0026_fix_org_config_rapidpro.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0028_alter_org_config.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0028_alter_org_config.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0029_auto_20211025_1504.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0029_auto_20211025_1504.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/migrations/0030_alter_invitation_created_by_and_more.py` & `rapidpro-dash-1.9.3/dash/orgs/migrations/0030_alter_invitation_created_by_and_more.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/models.py` & `rapidpro-dash-1.9.3/dash/orgs/models.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/tasks.py` & `rapidpro-dash-1.9.3/dash/orgs/tasks.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/templates/email_base.html` & `rapidpro-dash-1.9.3/dash/orgs/templates/email_base.html`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/templates/orgs/org_home.haml` & `rapidpro-dash-1.9.3/dash/orgs/templates/orgs/org_home.haml`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/templates/orgs/org_manage_accounts.haml` & `rapidpro-dash-1.9.3/dash/orgs/templates/orgs/org_manage_accounts.haml`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/templatetags/dashorgs.py` & `rapidpro-dash-1.9.3/dash/orgs/templatetags/dashorgs.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/orgs/views.py` & `rapidpro-dash-1.9.3/dash/orgs/views.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/stories/migrations/0001_initial.py` & `rapidpro-dash-1.9.3/dash/stories/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/stories/migrations/0005_story_category.py` & `rapidpro-dash-1.9.3/dash/stories/migrations/0005_story_category.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/stories/migrations/0006_auto_20140821_0859.py` & `rapidpro-dash-1.9.3/dash/stories/migrations/0006_auto_20140821_0859.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/stories/migrations/0007_storyimage.py` & `rapidpro-dash-1.9.3/dash/stories/migrations/0007_storyimage.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/stories/migrations/0008_auto_20140912_0524.py` & `rapidpro-dash-1.9.3/dash/stories/migrations/0008_auto_20140912_0524.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/stories/migrations/0010_auto_20140922_1514.py` & `rapidpro-dash-1.9.3/dash/stories/migrations/0010_auto_20140922_1514.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/stories/migrations/0013_auto_20170301_0914.py` & `rapidpro-dash-1.9.3/dash/stories/migrations/0013_auto_20170301_0914.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/stories/migrations/0014_alter_storyimage_image.py` & `rapidpro-dash-1.9.3/dash/stories/migrations/0014_alter_storyimage_image.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/stories/migrations/0015_story_attachment.py` & `rapidpro-dash-1.9.3/dash/stories/migrations/0015_story_attachment.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/stories/migrations/0016_alter_story_created_by_alter_story_modified_by_and_more.py` & `rapidpro-dash-1.9.3/dash/stories/migrations/0016_alter_story_created_by_alter_story_modified_by_and_more.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/stories/models.py` & `rapidpro-dash-1.9.3/dash/stories/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from functools import partial
 
 from smartmin.models import SmartModel
 
 from django.core.exceptions import ValidationError
 from django.db import models
+from django.db.models import Prefetch, Q
 from django.utils.translation import gettext_lazy as _
 
 from dash.categories.models import Category
 from dash.orgs.models import Org
 from dash.utils import generate_file_path
 
 
@@ -114,15 +115,19 @@
             return self.written_by
 
         if self.created_by.first_name or self.created_by.last_name:
             full_name = self.created_by.first_name + " " + self.created_by.last_name
             return full_name.strip()
 
     def get_featured_images(self):
-        return self.images.filter(is_active=True).exclude(image="")
+        return (
+            self.prefetched_images
+            if hasattr(self, "prefetched_images")
+            else self.images.filter(is_active=True).exclude(image="")
+        )
 
     def get_category_image(self):
         cat_image = None
         if self.category and self.category.is_active:
             cat_image = self.category.get_first_image()
 
         if not cat_image:
@@ -138,14 +143,31 @@
 
         if not cat_image:
             if self.category and self.category.is_active:
                 cat_image = self.category.get_first_image()
 
         return cat_image
 
+    @classmethod
+    def get_main_stories(cls, org, limit=None):
+        stories = (
+            Story.objects.filter(org=org, featured=True, is_active=True)
+            .filter(Q(attachment="") | Q(attachment=None))
+            .prefetch_related(
+                Prefetch(
+                    "images",
+                    queryset=StoryImage.objects.filter(is_active=True).exclude(image=""),
+                    to_attr="prefetched_images",
+                )
+            )
+            .order_by("-created_on")
+        )
+
+        return stories[:limit] if limit else stories
+
     class Meta:
         verbose_name_plural = _("Stories")
 
 
 class StoryImage(SmartModel):
     name = models.CharField(max_length=64, help_text=_("The name to describe this image"))
```

### Comparing `rapidpro-dash-1.9.2/dash/stories/templates/stories/story_create.haml` & `rapidpro-dash-1.9.3/dash/stories/templates/stories/story_create.haml`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/stories/templates/stories/story_update.haml` & `rapidpro-dash-1.9.3/dash/stories/templates/stories/story_update.haml`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/stories/views.py` & `rapidpro-dash-1.9.3/dash/stories/views.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/tags/migrations/0001_initial.py` & `rapidpro-dash-1.9.3/dash/tags/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/tags/migrations/0002_alter_tag_created_by_alter_tag_modified_by.py` & `rapidpro-dash-1.9.3/dash/tags/migrations/0002_alter_tag_created_by_alter_tag_modified_by.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/tags/views.py` & `rapidpro-dash-1.9.3/dash/tags/views.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/test.py` & `rapidpro-dash-1.9.3/dash/test.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/users/urls.py` & `rapidpro-dash-1.9.3/dash/users/urls.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/users/views.py` & `rapidpro-dash-1.9.3/dash/users/views.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/utils/__init__.py` & `rapidpro-dash-1.9.3/dash/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/utils/email.py` & `rapidpro-dash-1.9.3/dash/utils/email.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/utils/haml.py` & `rapidpro-dash-1.9.3/dash/utils/haml.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/utils/sync.py` & `rapidpro-dash-1.9.3/dash/utils/sync.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/dash/utils/tests.py` & `rapidpro-dash-1.9.3/dash/utils/tests.py`

 * *Files identical despite different names*

### Comparing `rapidpro-dash-1.9.2/pyproject.toml` & `rapidpro-dash-1.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rapidpro-dash"
-version = "1.9.2"
+version = "1.9.3"
 description = "Support library for RapidPro dashboards"
 authors = ["Nyaruka Ltd <code@nyaruka.com>"]
 license = "BSD"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
```

### Comparing `rapidpro-dash-1.9.2/setup.py` & `rapidpro-dash-1.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
  'python-dateutil>=2.8.1,<3.0.0',
  'rapidpro-python>=2.8.3,<3.0.0',
  'smartmin>=4.1.0,<5.0.0',
  'sorl-thumbnail>=12.7.0,<13.0.0']
 
 setup_kwargs = {
     'name': 'rapidpro-dash',
-    'version': '1.9.2',
+    'version': '1.9.3',
     'description': 'Support library for RapidPro dashboards',
     'long_description': None,
     'author': 'Nyaruka Ltd',
     'author_email': 'code@nyaruka.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `rapidpro-dash-1.9.2/PKG-INFO` & `rapidpro-dash-1.9.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpro-dash
-Version: 1.9.2
+Version: 1.9.3
 Summary: Support library for RapidPro dashboards
 License: BSD
 Author: Nyaruka Ltd
 Author-email: code@nyaruka.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

