# Comparing `tmp/netbox-slm-1.2.tar.gz` & `tmp/netbox-slm-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/netbox-slm-1.2.tar", last modified: Thu May 19 09:09:13 2022, max compression
+gzip compressed data, was "netbox-slm-1.3.tar", last modified: Wed Apr 19 08:25:32 2023, max compression
```

## Comparing `netbox-slm-1.2.tar` & `netbox-slm-1.3.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 heddevanderheide   (501) staff       (20)        0 2022-05-19 09:09:13.000000 netbox-slm-1.2/
--rw-r--r--   0 heddevanderheide   (501) staff       (20)      904 2022-05-19 09:09:13.000000 netbox-slm-1.2/PKG-INFO
-drwxr-xr-x   0 heddevanderheide   (501) staff       (20)        0 2022-05-19 09:09:13.000000 netbox-slm-1.2/netbox_slm/
-drwxr-xr-x   0 heddevanderheide   (501) staff       (20)        0 2022-05-19 09:09:13.000000 netbox-slm-1.2/netbox_slm/templatetags/
--rw-r--r--   0 heddevanderheide   (501) staff       (20)        0 2021-12-23 10:53:39.000000 netbox-slm-1.2/netbox_slm/templatetags/__init__.py
-drwxr-xr-x   0 heddevanderheide   (501) staff       (20)        0 2022-05-19 09:09:13.000000 netbox-slm-1.2/netbox_slm/migrations/
--rw-r--r--   0 heddevanderheide   (501) staff       (20)      576 2022-01-24 08:05:57.000000 netbox-slm-1.2/netbox_slm/migrations/0002_alter_softwareproduct_manufacturer.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)        0 2021-12-23 10:53:39.000000 netbox-slm-1.2/netbox_slm/migrations/__init__.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     1876 2022-04-15 07:05:04.000000 netbox-slm-1.2/netbox_slm/migrations/0004_auto_20220415_0705.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     1436 2022-04-07 12:09:55.000000 netbox-slm-1.2/netbox_slm/migrations/0003_auto_20220407_1209.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     3752 2021-12-23 10:53:39.000000 netbox-slm-1.2/netbox_slm/migrations/0001_initial.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     2871 2022-04-22 11:25:11.000000 netbox-slm-1.2/netbox_slm/models.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     1848 2022-05-19 08:41:33.000000 netbox-slm-1.2/netbox_slm/filtersets.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)      429 2022-05-19 09:08:48.000000 netbox-slm-1.2/netbox_slm/__init__.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     5280 2022-05-19 08:43:56.000000 netbox-slm-1.2/netbox_slm/forms.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)        0 2022-05-03 13:18:38.000000 netbox-slm-1.2/netbox_slm/admin.py
-drwxr-xr-x   0 heddevanderheide   (501) staff       (20)        0 2022-05-19 09:09:13.000000 netbox-slm-1.2/netbox_slm/api/
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     1772 2022-04-07 13:54:44.000000 netbox-slm-1.2/netbox_slm/api/serializers.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)        0 2021-12-23 10:53:39.000000 netbox-slm-1.2/netbox_slm/api/__init__.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)      515 2022-04-07 13:50:44.000000 netbox-slm-1.2/netbox_slm/api/urls.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     1289 2022-05-19 08:42:02.000000 netbox-slm-1.2/netbox_slm/api/views.py
-drwxr-xr-x   0 heddevanderheide   (501) staff       (20)        0 2022-05-19 09:09:13.000000 netbox-slm-1.2/netbox_slm/templates/
-drwxr-xr-x   0 heddevanderheide   (501) staff       (20)        0 2022-05-19 09:09:13.000000 netbox-slm-1.2/netbox_slm/templates/netbox_slm/
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     1570 2022-04-08 07:06:03.000000 netbox-slm-1.2/netbox_slm/templates/netbox_slm/softwareproductinstallation.html
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     1182 2022-04-08 07:06:03.000000 netbox-slm-1.2/netbox_slm/templates/netbox_slm/softwareproductversion.html
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     1549 2022-04-15 06:59:26.000000 netbox-slm-1.2/netbox_slm/templates/netbox_slm/softwareproduct.html
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     4754 2022-04-15 06:56:58.000000 netbox-slm-1.2/netbox_slm/tables.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     2283 2022-04-22 11:25:11.000000 netbox-slm-1.2/netbox_slm/navigation.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     3938 2022-04-22 11:20:07.000000 netbox-slm-1.2/netbox_slm/urls.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     5327 2022-04-22 11:15:46.000000 netbox-slm-1.2/netbox_slm/views.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)      544 2022-05-03 13:19:55.000000 netbox-slm-1.2/LICENSE
-drwxr-xr-x   0 heddevanderheide   (501) staff       (20)        0 2022-05-19 09:09:13.000000 netbox-slm-1.2/netbox_slm.egg-info/
--rw-r--r--   0 heddevanderheide   (501) staff       (20)      904 2022-05-19 09:09:13.000000 netbox-slm-1.2/netbox_slm.egg-info/PKG-INFO
--rw-r--r--   0 heddevanderheide   (501) staff       (20)      931 2022-05-19 09:09:13.000000 netbox-slm-1.2/netbox_slm.egg-info/SOURCES.txt
--rw-r--r--   0 heddevanderheide   (501) staff       (20)       11 2022-05-19 09:09:13.000000 netbox-slm-1.2/netbox_slm.egg-info/top_level.txt
--rw-r--r--   0 heddevanderheide   (501) staff       (20)        1 2022-05-19 09:09:13.000000 netbox-slm-1.2/netbox_slm.egg-info/dependency_links.txt
--rw-r--r--   0 heddevanderheide   (501) staff       (20)       81 2022-01-24 07:52:12.000000 netbox-slm-1.2/MANIFEST.in
--rw-r--r--   0 heddevanderheide   (501) staff       (20)     7932 2022-05-19 09:08:48.000000 netbox-slm-1.2/README.md
--rw-r--r--   0 heddevanderheide   (501) staff       (20)       48 2022-01-24 07:52:12.000000 netbox-slm-1.2/setup.py
--rw-r--r--   0 heddevanderheide   (501) staff       (20)      813 2022-05-19 09:09:13.000000 netbox-slm-1.2/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:32.056067 netbox-slm-1.3/
+-rwxrwxrwx   0 user      (1000) user      (1000)      557 2022-09-12 10:32:39.000000 netbox-slm-1.3/LICENSE
+-rwxrwxrwx   0 user      (1000) user      (1000)      108 2023-04-19 08:14:46.000000 netbox-slm-1.3/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)      858 2023-04-19 08:25:32.058042 netbox-slm-1.3/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)     8170 2023-03-31 08:03:01.000000 netbox-slm-1.3/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:31.117380 netbox-slm-1.3/netbox_slm/
+-rwxrwxrwx   0 user      (1000) user      (1000)      451 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/__init__.py
+-rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/admin.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:31.440583 netbox-slm-1.3/netbox_slm/api/
+-rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/api/__init__.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1811 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/api/serializers.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      531 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/api/urls.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1317 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/api/views.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1951 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/filtersets.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     5405 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/forms.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:31.687302 netbox-slm-1.3/netbox_slm/migrations/
+-rwxrwxrwx   0 user      (1000) user      (1000)     3820 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/migrations/0001_initial.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      596 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/migrations/0002_alter_softwareproduct_manufacturer.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1479 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/migrations/0003_auto_20220407_1209.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1922 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/migrations/0004_auto_20220415_0705.py
+-rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/migrations/__init__.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2954 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/models.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2347 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/navigation.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     4902 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/tables.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:30.672999 netbox-slm-1.3/netbox_slm/templates/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:31.875513 netbox-slm-1.3/netbox_slm/templates/netbox_slm/
+-rwxrwxrwx   0 user      (1000) user      (1000)     1595 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/templates/netbox_slm/softwareproduct.html
+-rwxrwxrwx   0 user      (1000) user      (1000)     1619 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/templates/netbox_slm/softwareproductinstallation.html
+-rwxrwxrwx   0 user      (1000) user      (1000)     1222 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/templates/netbox_slm/softwareproductversion.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:31.925514 netbox-slm-1.3/netbox_slm/templatetags/
+-rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/templatetags/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:32.016329 netbox-slm-1.3/netbox_slm/tests/
+-rwxrwxrwx   0 user      (1000) user      (1000)        0 2023-03-29 20:01:01.000000 netbox-slm-1.3/netbox_slm/tests/__init__.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1914 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/tests/test_models.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     4006 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/urls.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     5425 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/views.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:31.253863 netbox-slm-1.3/netbox_slm.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      858 2023-04-19 08:25:30.000000 netbox-slm-1.3/netbox_slm.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      992 2023-04-19 08:25:30.000000 netbox-slm-1.3/netbox_slm.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-19 08:25:30.000000 netbox-slm-1.3/netbox_slm.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       11 2023-04-19 08:25:30.000000 netbox-slm-1.3/netbox_slm.egg-info/top_level.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)      803 2023-04-19 08:25:32.068239 netbox-slm-1.3/setup.cfg
+-rwxrwxrwx   0 user      (1000) user      (1000)       41 2023-04-19 08:14:46.000000 netbox-slm-1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `netbox-slm-1.2/netbox_slm/migrations/0004_auto_20220415_0705.py` & `netbox-slm-1.3/netbox_slm/migrations/0004_auto_20220415_0705.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# Generated by Django 3.2.9 on 2022-04-15 07:05
-
-from django.db import migrations, models
-import django.db.models.deletion
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('dcim', '0153_created_datetimefield'),
-        ('virtualization', '0029_created_datetimefield'),
-        ('netbox_slm', '0003_auto_20220407_1209'),
-    ]
-
-    operations = [
-        migrations.AlterField(
-            model_name='softwareproduct',
-            name='manufacturer',
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.PROTECT, to='dcim.manufacturer'),
-        ),
-        migrations.AlterField(
-            model_name='softwareproductinstallation',
-            name='device',
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.PROTECT, to='dcim.device'),
-        ),
-        migrations.AlterField(
-            model_name='softwareproductinstallation',
-            name='software_product',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, to='netbox_slm.softwareproduct'),
-        ),
-        migrations.AlterField(
-            model_name='softwareproductinstallation',
-            name='version',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, to='netbox_slm.softwareproductversion'),
-        ),
-        migrations.AlterField(
-            model_name='softwareproductinstallation',
-            name='virtualmachine',
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.PROTECT, to='virtualization.virtualmachine'),
-        ),
-        migrations.AlterField(
-            model_name='softwareproductversion',
-            name='software_product',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, to='netbox_slm.softwareproduct'),
-        ),
-    ]
+# Generated by Django 3.2.9 on 2022-04-15 07:05
+
+from django.db import migrations, models
+import django.db.models.deletion
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('dcim', '0153_created_datetimefield'),
+        ('virtualization', '0029_created_datetimefield'),
+        ('netbox_slm', '0003_auto_20220407_1209'),
+    ]
+
+    operations = [
+        migrations.AlterField(
+            model_name='softwareproduct',
+            name='manufacturer',
+            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.PROTECT, to='dcim.manufacturer'),
+        ),
+        migrations.AlterField(
+            model_name='softwareproductinstallation',
+            name='device',
+            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.PROTECT, to='dcim.device'),
+        ),
+        migrations.AlterField(
+            model_name='softwareproductinstallation',
+            name='software_product',
+            field=models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, to='netbox_slm.softwareproduct'),
+        ),
+        migrations.AlterField(
+            model_name='softwareproductinstallation',
+            name='version',
+            field=models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, to='netbox_slm.softwareproductversion'),
+        ),
+        migrations.AlterField(
+            model_name='softwareproductinstallation',
+            name='virtualmachine',
+            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.PROTECT, to='virtualization.virtualmachine'),
+        ),
+        migrations.AlterField(
+            model_name='softwareproductversion',
+            name='software_product',
+            field=models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, to='netbox_slm.softwareproduct'),
+        ),
+    ]
```

### Comparing `netbox-slm-1.2/netbox_slm/migrations/0001_initial.py` & `netbox-slm-1.3/netbox_slm/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-# Generated by Django 3.2.8 on 2021-12-17 10:11
-
-import django.core.serializers.json
-from django.db import migrations, models
-import django.db.models.deletion
-import taggit.managers
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-        ('virtualization', '0023_virtualmachine_natural_ordering'),
-        ('extras', '0062_clear_secrets_changelog'),
-        ('dcim', '0133_port_colors'),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='SoftwareProduct',
-            fields=[
-                ('created', models.DateField(auto_now_add=True, null=True)),
-                ('last_updated', models.DateTimeField(auto_now=True, null=True)),
-                ('custom_field_data', models.JSONField(blank=True, default=dict, encoder=django.core.serializers.json.DjangoJSONEncoder)),
-                ('id', models.BigAutoField(primary_key=True, serialize=False)),
-                ('name', models.CharField(max_length=128)),
-                ('description', models.CharField(blank=True, max_length=255, null=True)),
-                ('manufacturer', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='software_products', to='dcim.manufacturer')),
-                ('tags', taggit.managers.TaggableManager(through='extras.TaggedItem', to='extras.Tag')),
-            ],
-            options={
-                'abstract': False,
-            },
-        ),
-        migrations.CreateModel(
-            name='SoftwareProductVersion',
-            fields=[
-                ('created', models.DateField(auto_now_add=True, null=True)),
-                ('last_updated', models.DateTimeField(auto_now=True, null=True)),
-                ('custom_field_data', models.JSONField(blank=True, default=dict, encoder=django.core.serializers.json.DjangoJSONEncoder)),
-                ('id', models.BigAutoField(primary_key=True, serialize=False)),
-                ('name', models.CharField(max_length=64)),
-                ('software_product', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='softwareproduct_versions', to='netbox_slm.softwareproduct')),
-                ('tags', taggit.managers.TaggableManager(through='extras.TaggedItem', to='extras.Tag')),
-            ],
-            options={
-                'abstract': False,
-            },
-        ),
-        migrations.CreateModel(
-            name='SoftwareProductInstallation',
-            fields=[
-                ('created', models.DateField(auto_now_add=True, null=True)),
-                ('last_updated', models.DateTimeField(auto_now=True, null=True)),
-                ('custom_field_data', models.JSONField(blank=True, default=dict, encoder=django.core.serializers.json.DjangoJSONEncoder)),
-                ('id', models.BigAutoField(primary_key=True, serialize=False)),
-                ('device', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.PROTECT, related_name='softwareproduct_installations', to='dcim.device')),
-                ('software_product', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='software_products', to='netbox_slm.softwareproduct')),
-                ('tags', taggit.managers.TaggableManager(through='extras.TaggedItem', to='extras.Tag')),
-                ('version', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='softwareproduct_versions', to='netbox_slm.softwareproductversion')),
-                ('virtualmachine', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.PROTECT, related_name='softwareproduct_installations', to='virtualization.virtualmachine')),
-            ],
-            options={
-                'abstract': False,
-            },
-        ),
-    ]
+# Generated by Django 3.2.8 on 2021-12-17 10:11
+
+import django.core.serializers.json
+from django.db import migrations, models
+import django.db.models.deletion
+import taggit.managers
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+        ('virtualization', '0023_virtualmachine_natural_ordering'),
+        ('extras', '0062_clear_secrets_changelog'),
+        ('dcim', '0133_port_colors'),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='SoftwareProduct',
+            fields=[
+                ('created', models.DateField(auto_now_add=True, null=True)),
+                ('last_updated', models.DateTimeField(auto_now=True, null=True)),
+                ('custom_field_data', models.JSONField(blank=True, default=dict, encoder=django.core.serializers.json.DjangoJSONEncoder)),
+                ('id', models.BigAutoField(primary_key=True, serialize=False)),
+                ('name', models.CharField(max_length=128)),
+                ('description', models.CharField(blank=True, max_length=255, null=True)),
+                ('manufacturer', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='software_products', to='dcim.manufacturer')),
+                ('tags', taggit.managers.TaggableManager(through='extras.TaggedItem', to='extras.Tag')),
+            ],
+            options={
+                'abstract': False,
+            },
+        ),
+        migrations.CreateModel(
+            name='SoftwareProductVersion',
+            fields=[
+                ('created', models.DateField(auto_now_add=True, null=True)),
+                ('last_updated', models.DateTimeField(auto_now=True, null=True)),
+                ('custom_field_data', models.JSONField(blank=True, default=dict, encoder=django.core.serializers.json.DjangoJSONEncoder)),
+                ('id', models.BigAutoField(primary_key=True, serialize=False)),
+                ('name', models.CharField(max_length=64)),
+                ('software_product', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='softwareproduct_versions', to='netbox_slm.softwareproduct')),
+                ('tags', taggit.managers.TaggableManager(through='extras.TaggedItem', to='extras.Tag')),
+            ],
+            options={
+                'abstract': False,
+            },
+        ),
+        migrations.CreateModel(
+            name='SoftwareProductInstallation',
+            fields=[
+                ('created', models.DateField(auto_now_add=True, null=True)),
+                ('last_updated', models.DateTimeField(auto_now=True, null=True)),
+                ('custom_field_data', models.JSONField(blank=True, default=dict, encoder=django.core.serializers.json.DjangoJSONEncoder)),
+                ('id', models.BigAutoField(primary_key=True, serialize=False)),
+                ('device', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.PROTECT, related_name='softwareproduct_installations', to='dcim.device')),
+                ('software_product', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='software_products', to='netbox_slm.softwareproduct')),
+                ('tags', taggit.managers.TaggableManager(through='extras.TaggedItem', to='extras.Tag')),
+                ('version', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='softwareproduct_versions', to='netbox_slm.softwareproductversion')),
+                ('virtualmachine', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.PROTECT, related_name='softwareproduct_installations', to='virtualization.virtualmachine')),
+            ],
+            options={
+                'abstract': False,
+            },
+        ),
+    ]
```

### Comparing `netbox-slm-1.2/netbox_slm/models.py` & `netbox-slm-1.3/netbox_slm/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,180 +1,185 @@
 00000000: 6672 6f6d 2064 6a61 6e67 6f2e 6462 2069  from django.db i
-00000010: 6d70 6f72 7420 6d6f 6465 6c73 0a66 726f  mport models.fro
-00000020: 6d20 646a 616e 676f 2e75 726c 7320 696d  m django.urls im
-00000030: 706f 7274 2072 6576 6572 7365 2c20 7265  port reverse, re
-00000040: 7665 7273 655f 6c61 7a79 0a66 726f 6d20  verse_lazy.from 
-00000050: 646a 616e 676f 2e75 7469 6c73 2069 6d70  django.utils imp
-00000060: 6f72 7420 7361 6665 7374 7269 6e67 0a0a  ort safestring..
-00000070: 6672 6f6d 206e 6574 626f 782e 6d6f 6465  from netbox.mode
-00000080: 6c73 2069 6d70 6f72 7420 4e65 7442 6f78  ls import NetBox
-00000090: 4d6f 6465 6c0a 6672 6f6d 2075 7469 6c69  Model.from utili
-000000a0: 7469 6573 2e71 7565 7279 7365 7473 2069  ties.querysets i
-000000b0: 6d70 6f72 7420 5265 7374 7269 6374 6564  mport Restricted
-000000c0: 5175 6572 7953 6574 0a0a 0a63 6c61 7373  QuerySet...class
-000000d0: 2053 6f66 7477 6172 6550 726f 6475 6374   SoftwareProduct
-000000e0: 284e 6574 426f 784d 6f64 656c 293a 0a20  (NetBoxModel):. 
-000000f0: 2020 206e 616d 6520 3d20 6d6f 6465 6c73     name = models
-00000100: 2e43 6861 7246 6965 6c64 286d 6178 5f6c  .CharField(max_l
-00000110: 656e 6774 683d 3132 3829 0a20 2020 2064  ength=128).    d
-00000120: 6573 6372 6970 7469 6f6e 203d 206d 6f64  escription = mod
-00000130: 656c 732e 4368 6172 4669 656c 6428 6d61  els.CharField(ma
-00000140: 785f 6c65 6e67 7468 3d32 3535 2c20 6e75  x_length=255, nu
-00000150: 6c6c 3d54 7275 652c 2062 6c61 6e6b 3d54  ll=True, blank=T
-00000160: 7275 6529 0a20 2020 200a 2020 2020 6d61  rue).    .    ma
-00000170: 6e75 6661 6374 7572 6572 203d 206d 6f64  nufacturer = mod
-00000180: 656c 732e 466f 7265 6967 6e4b 6579 280a  els.ForeignKey(.
-00000190: 2020 2020 2020 2020 746f 3d27 6463 696d          to='dcim
-000001a0: 2e4d 616e 7566 6163 7475 7265 7227 2c0a  .Manufacturer',.
-000001b0: 2020 2020 2020 2020 6f6e 5f64 656c 6574          on_delet
-000001c0: 653d 6d6f 6465 6c73 2e50 524f 5445 4354  e=models.PROTECT
-000001d0: 2c0a 2020 2020 2020 2020 6e75 6c6c 3d54  ,.        null=T
-000001e0: 7275 652c 2062 6c61 6e6b 3d54 7275 650a  rue, blank=True.
-000001f0: 2020 2020 290a 0a20 2020 206f 626a 6563      )..    objec
-00000200: 7473 203d 2052 6573 7472 6963 7465 6451  ts = RestrictedQ
-00000210: 7565 7279 5365 742e 6173 5f6d 616e 6167  uerySet.as_manag
-00000220: 6572 2829 0a0a 2020 2020 6465 6620 5f5f  er()..    def __
-00000230: 7374 725f 5f28 7365 6c66 293a 0a20 2020  str__(self):.   
-00000240: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00000250: 2e6e 616d 650a 0a20 2020 2064 6566 2067  .name..    def g
-00000260: 6574 5f61 6273 6f6c 7574 655f 7572 6c28  et_absolute_url(
-00000270: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
-00000280: 6574 7572 6e20 7265 7665 7273 6528 2270  eturn reverse("p
-00000290: 6c75 6769 6e73 3a6e 6574 626f 785f 736c  lugins:netbox_sl
-000002a0: 6d3a 736f 6674 7761 7265 7072 6f64 7563  m:softwareproduc
-000002b0: 7422 2c20 6b77 6172 6773 3d7b 2270 6b22  t", kwargs={"pk"
-000002c0: 3a20 7365 6c66 2e70 6b7d 290a 0a20 2020  : self.pk})..   
-000002d0: 2064 6566 2067 6574 5f69 6e73 7461 6c6c   def get_install
-000002e0: 6174 696f 6e5f 636f 756e 7428 7365 6c66  ation_count(self
-000002f0: 293a 0a20 2020 2020 2020 2063 6f75 6e74  ):.        count
-00000300: 203d 2053 6f66 7477 6172 6550 726f 6475   = SoftwareProdu
-00000310: 6374 496e 7374 616c 6c61 7469 6f6e 2e6f  ctInstallation.o
-00000320: 626a 6563 7473 2e66 696c 7465 7228 736f  bjects.filter(so
-00000330: 6674 7761 7265 5f70 726f 6475 6374 5f69  ftware_product_i
-00000340: 643d 7365 6c66 2e70 6b29 2e63 6f75 6e74  d=self.pk).count
-00000350: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-00000360: 6e20 7361 6665 7374 7269 6e67 2e6d 6172  n safestring.mar
-00000370: 6b5f 7361 6665 2822 3c61 2068 7265 663d  k_safe("<a href=
-00000380: 5c22 7b75 726c 7d5c 223e 7b63 6f75 6e74  \"{url}\">{count
-00000390: 7d3c 2f61 3e22 2e66 6f72 6d61 7428 0a20  }</a>".format(. 
-000003a0: 2020 2020 2020 2020 2020 2075 726c 3d72             url=r
-000003b0: 6576 6572 7365 5f6c 617a 7928 2270 6c75  everse_lazy("plu
-000003c0: 6769 6e73 3a6e 6574 626f 785f 736c 6d3a  gins:netbox_slm:
-000003d0: 736f 6674 7761 7265 7072 6f64 7563 7469  softwareproducti
-000003e0: 6e73 7461 6c6c 6174 696f 6e5f 6c69 7374  nstallation_list
-000003f0: 2229 202b 2066 223f 713d 7b73 656c 662e  ") + f"?q={self.
-00000400: 6e61 6d65 7d22 2c0a 2020 2020 2020 2020  name}",.        
-00000410: 2020 2020 636f 756e 743d 636f 756e 740a      count=count.
-00000420: 2020 2020 2020 2020 2929 2069 6620 636f          )) if co
-00000430: 756e 7420 656c 7365 2022 3022 0a0a 0a63  unt else "0"...c
-00000440: 6c61 7373 2053 6f66 7477 6172 6550 726f  lass SoftwarePro
-00000450: 6475 6374 5665 7273 696f 6e28 4e65 7442  ductVersion(NetB
-00000460: 6f78 4d6f 6465 6c29 3a0a 2020 2020 736f  oxModel):.    so
-00000470: 6674 7761 7265 5f70 726f 6475 6374 203d  ftware_product =
-00000480: 206d 6f64 656c 732e 466f 7265 6967 6e4b   models.ForeignK
-00000490: 6579 280a 2020 2020 2020 2020 746f 3d27  ey(.        to='
-000004a0: 6e65 7462 6f78 5f73 6c6d 2e53 6f66 7477  netbox_slm.Softw
-000004b0: 6172 6550 726f 6475 6374 272c 0a20 2020  areProduct',.   
-000004c0: 2020 2020 206f 6e5f 6465 6c65 7465 3d6d       on_delete=m
-000004d0: 6f64 656c 732e 5052 4f54 4543 542c 0a20  odels.PROTECT,. 
-000004e0: 2020 2029 0a20 2020 206e 616d 6520 3d20     ).    name = 
-000004f0: 6d6f 6465 6c73 2e43 6861 7246 6965 6c64  models.CharField
-00000500: 286d 6178 5f6c 656e 6774 683d 3634 290a  (max_length=64).
-00000510: 0a20 2020 206f 626a 6563 7473 203d 2052  .    objects = R
-00000520: 6573 7472 6963 7465 6451 7565 7279 5365  estrictedQuerySe
-00000530: 742e 6173 5f6d 616e 6167 6572 2829 0a0a  t.as_manager()..
-00000540: 2020 2020 6465 6620 5f5f 7374 725f 5f28      def __str__(
-00000550: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
-00000560: 6574 7572 6e20 7365 6c66 2e6e 616d 650a  eturn self.name.
-00000570: 0a20 2020 2064 6566 2067 6574 5f61 6273  .    def get_abs
-00000580: 6f6c 7574 655f 7572 6c28 7365 6c66 293a  olute_url(self):
-00000590: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000005a0: 7265 7665 7273 6528 2270 6c75 6769 6e73  reverse("plugins
-000005b0: 3a6e 6574 626f 785f 736c 6d3a 736f 6674  :netbox_slm:soft
-000005c0: 7761 7265 7072 6f64 7563 7476 6572 7369  wareproductversi
-000005d0: 6f6e 222c 206b 7761 7267 733d 7b22 706b  on", kwargs={"pk
-000005e0: 223a 2073 656c 662e 706b 7d29 0a0a 2020  ": self.pk})..  
-000005f0: 2020 6465 6620 6765 745f 696e 7374 616c    def get_instal
-00000600: 6c61 7469 6f6e 5f63 6f75 6e74 2873 656c  lation_count(sel
-00000610: 6629 3a0a 2020 2020 2020 2020 636f 756e  f):.        coun
-00000620: 7420 3d20 536f 6674 7761 7265 5072 6f64  t = SoftwareProd
-00000630: 7563 7449 6e73 7461 6c6c 6174 696f 6e2e  uctInstallation.
-00000640: 6f62 6a65 6374 732e 6669 6c74 6572 2876  objects.filter(v
-00000650: 6572 7369 6f6e 5f69 643d 7365 6c66 2e70  ersion_id=self.p
-00000660: 6b29 2e63 6f75 6e74 2829 0a20 2020 2020  k).count().     
-00000670: 2020 2072 6574 7572 6e20 7361 6665 7374     return safest
-00000680: 7269 6e67 2e6d 6172 6b5f 7361 6665 2822  ring.mark_safe("
-00000690: 3c61 2068 7265 663d 5c22 7b75 726c 7d5c  <a href=\"{url}\
-000006a0: 223e 7b63 6f75 6e74 7d3c 2f61 3e22 2e66  ">{count}</a>".f
-000006b0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-000006c0: 2020 2075 726c 3d72 6576 6572 7365 5f6c     url=reverse_l
-000006d0: 617a 7928 2270 6c75 6769 6e73 3a6e 6574  azy("plugins:net
-000006e0: 626f 785f 736c 6d3a 736f 6674 7761 7265  box_slm:software
-000006f0: 7072 6f64 7563 7469 6e73 7461 6c6c 6174  productinstallat
-00000700: 696f 6e5f 6c69 7374 2229 202b 2066 223f  ion_list") + f"?
-00000710: 713d 7b73 656c 662e 6e61 6d65 7d22 2c0a  q={self.name}",.
-00000720: 2020 2020 2020 2020 2020 2020 636f 756e              coun
-00000730: 743d 636f 756e 740a 2020 2020 2020 2020  t=count.        
-00000740: 2929 2069 6620 636f 756e 7420 656c 7365  )) if count else
-00000750: 2022 3022 0a0a 0a63 6c61 7373 2053 6f66   "0"...class Sof
-00000760: 7477 6172 6550 726f 6475 6374 496e 7374  twareProductInst
-00000770: 616c 6c61 7469 6f6e 284e 6574 426f 784d  allation(NetBoxM
-00000780: 6f64 656c 293a 0a20 2020 2064 6576 6963  odel):.    devic
-00000790: 6520 3d20 6d6f 6465 6c73 2e46 6f72 6569  e = models.Forei
-000007a0: 676e 4b65 7928 0a20 2020 2020 2020 2074  gnKey(.        t
-000007b0: 6f3d 2764 6369 6d2e 4465 7669 6365 272c  o='dcim.Device',
-000007c0: 0a20 2020 2020 2020 206f 6e5f 6465 6c65  .        on_dele
-000007d0: 7465 3d6d 6f64 656c 732e 5052 4f54 4543  te=models.PROTEC
-000007e0: 542c 0a20 2020 2020 2020 206e 756c 6c3d  T,.        null=
-000007f0: 5472 7565 2c0a 2020 2020 2020 2020 626c  True,.        bl
-00000800: 616e 6b3d 5472 7565 0a20 2020 2029 0a20  ank=True.    ). 
-00000810: 2020 2076 6972 7475 616c 6d61 6368 696e     virtualmachin
-00000820: 6520 3d20 6d6f 6465 6c73 2e46 6f72 6569  e = models.Forei
-00000830: 676e 4b65 7928 0a20 2020 2020 2020 2074  gnKey(.        t
-00000840: 6f3d 2776 6972 7475 616c 697a 6174 696f  o='virtualizatio
-00000850: 6e2e 5669 7274 7561 6c4d 6163 6869 6e65  n.VirtualMachine
-00000860: 272c 0a20 2020 2020 2020 206f 6e5f 6465  ',.        on_de
-00000870: 6c65 7465 3d6d 6f64 656c 732e 5052 4f54  lete=models.PROT
-00000880: 4543 542c 0a20 2020 2020 2020 206e 756c  ECT,.        nul
-00000890: 6c3d 5472 7565 2c0a 2020 2020 2020 2020  l=True,.        
-000008a0: 626c 616e 6b3d 5472 7565 0a20 2020 2029  blank=True.    )
-000008b0: 0a20 2020 2073 6f66 7477 6172 655f 7072  .    software_pr
-000008c0: 6f64 7563 7420 3d20 6d6f 6465 6c73 2e46  oduct = models.F
-000008d0: 6f72 6569 676e 4b65 7928 0a20 2020 2020  oreignKey(.     
-000008e0: 2020 2074 6f3d 276e 6574 626f 785f 736c     to='netbox_sl
-000008f0: 6d2e 536f 6674 7761 7265 5072 6f64 7563  m.SoftwareProduc
-00000900: 7427 2c0a 2020 2020 2020 2020 6f6e 5f64  t',.        on_d
-00000910: 656c 6574 653d 6d6f 6465 6c73 2e50 524f  elete=models.PRO
-00000920: 5445 4354 2c0a 2020 2020 290a 2020 2020  TECT,.    ).    
-00000930: 7665 7273 696f 6e20 3d20 6d6f 6465 6c73  version = models
-00000940: 2e46 6f72 6569 676e 4b65 7928 0a20 2020  .ForeignKey(.   
-00000950: 2020 2020 2074 6f3d 276e 6574 626f 785f       to='netbox_
-00000960: 736c 6d2e 536f 6674 7761 7265 5072 6f64  slm.SoftwareProd
-00000970: 7563 7456 6572 7369 6f6e 272c 0a20 2020  uctVersion',.   
-00000980: 2020 2020 206f 6e5f 6465 6c65 7465 3d6d       on_delete=m
-00000990: 6f64 656c 732e 5052 4f54 4543 542c 0a20  odels.PROTECT,. 
-000009a0: 2020 2029 0a0a 2020 2020 6f62 6a65 6374     )..    object
-000009b0: 7320 3d20 5265 7374 7269 6374 6564 5175  s = RestrictedQu
-000009c0: 6572 7953 6574 2e61 735f 6d61 6e61 6765  erySet.as_manage
-000009d0: 7228 290a 0a20 2020 2064 6566 205f 5f73  r()..    def __s
-000009e0: 7472 5f5f 2873 656c 6629 3a0a 2020 2020  tr__(self):.    
-000009f0: 2020 2020 7265 7475 726e 2066 227b 7365      return f"{se
-00000a00: 6c66 2e70 6b7d 220a 0a20 2020 2064 6566  lf.pk}"..    def
-00000a10: 2067 6574 5f61 6273 6f6c 7574 655f 7572   get_absolute_ur
-00000a20: 6c28 7365 6c66 293a 0a20 2020 2020 2020  l(self):.       
-00000a30: 2072 6574 7572 6e20 7265 7665 7273 6528   return reverse(
-00000a40: 2270 6c75 6769 6e73 3a6e 6574 626f 785f  "plugins:netbox_
-00000a50: 736c 6d3a 736f 6674 7761 7265 7072 6f64  slm:softwareprod
-00000a60: 7563 7469 6e73 7461 6c6c 6174 696f 6e22  uctinstallation"
-00000a70: 2c20 6b77 6172 6773 3d7b 2270 6b22 3a20  , kwargs={"pk": 
-00000a80: 7365 6c66 2e70 6b7d 290a 0a20 2020 2064  self.pk})..    d
-00000a90: 6566 2067 6574 5f70 6c61 7466 6f72 6d28  ef get_platform(
-00000aa0: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
-00000ab0: 6574 7572 6e20 7365 6c66 2e64 6576 6963  eturn self.devic
-00000ac0: 6520 6f72 2073 656c 662e 7669 7274 7561  e or self.virtua
-00000ad0: 6c6d 6163 6869 6e65 0a0a 2020 2020 6465  lmachine..    de
-00000ae0: 6620 7265 6e64 6572 5f74 7970 6528 7365  f render_type(se
-00000af0: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-00000b00: 7572 6e20 6622 7b27 6465 7669 6365 2720  urn f"{'device' 
-00000b10: 6966 2073 656c 662e 6465 7669 6365 2065  if self.device e
-00000b20: 6c73 6520 2776 6972 7475 616c 6d61 6368  lse 'virtualmach
-00000b30: 696e 6527 7d22 0a                        ine'}".
+00000010: 6d70 6f72 7420 6d6f 6465 6c73 0d0a 6672  mport models..fr
+00000020: 6f6d 2064 6a61 6e67 6f2e 7572 6c73 2069  om django.urls i
+00000030: 6d70 6f72 7420 7265 7665 7273 652c 2072  mport reverse, r
+00000040: 6576 6572 7365 5f6c 617a 790d 0a66 726f  everse_lazy..fro
+00000050: 6d20 646a 616e 676f 2e75 7469 6c73 2069  m django.utils i
+00000060: 6d70 6f72 7420 7361 6665 7374 7269 6e67  mport safestring
+00000070: 0d0a 0d0a 6672 6f6d 206e 6574 626f 782e  ....from netbox.
+00000080: 6d6f 6465 6c73 2069 6d70 6f72 7420 4e65  models import Ne
+00000090: 7442 6f78 4d6f 6465 6c0d 0a66 726f 6d20  tBoxModel..from 
+000000a0: 7574 696c 6974 6965 732e 7175 6572 7973  utilities.querys
+000000b0: 6574 7320 696d 706f 7274 2052 6573 7472  ets import Restr
+000000c0: 6963 7465 6451 7565 7279 5365 740d 0a0d  ictedQuerySet...
+000000d0: 0a0d 0a63 6c61 7373 2053 6f66 7477 6172  ...class Softwar
+000000e0: 6550 726f 6475 6374 284e 6574 426f 784d  eProduct(NetBoxM
+000000f0: 6f64 656c 293a 0d0a 2020 2020 6e61 6d65  odel):..    name
+00000100: 203d 206d 6f64 656c 732e 4368 6172 4669   = models.CharFi
+00000110: 656c 6428 6d61 785f 6c65 6e67 7468 3d31  eld(max_length=1
+00000120: 3238 290d 0a20 2020 2064 6573 6372 6970  28)..    descrip
+00000130: 7469 6f6e 203d 206d 6f64 656c 732e 4368  tion = models.Ch
+00000140: 6172 4669 656c 6428 6d61 785f 6c65 6e67  arField(max_leng
+00000150: 7468 3d32 3535 2c20 6e75 6c6c 3d54 7275  th=255, null=Tru
+00000160: 652c 2062 6c61 6e6b 3d54 7275 6529 0d0a  e, blank=True)..
+00000170: 0d0a 2020 2020 6d61 6e75 6661 6374 7572  ..    manufactur
+00000180: 6572 203d 206d 6f64 656c 732e 466f 7265  er = models.Fore
+00000190: 6967 6e4b 6579 280d 0a20 2020 2020 2020  ignKey(..       
+000001a0: 2074 6f3d 2764 6369 6d2e 4d61 6e75 6661   to='dcim.Manufa
+000001b0: 6374 7572 6572 272c 0d0a 2020 2020 2020  cturer',..      
+000001c0: 2020 6f6e 5f64 656c 6574 653d 6d6f 6465    on_delete=mode
+000001d0: 6c73 2e50 524f 5445 4354 2c0d 0a20 2020  ls.PROTECT,..   
+000001e0: 2020 2020 206e 756c 6c3d 5472 7565 2c20       null=True, 
+000001f0: 626c 616e 6b3d 5472 7565 0d0a 2020 2020  blank=True..    
+00000200: 290d 0a0d 0a20 2020 206f 626a 6563 7473  )....    objects
+00000210: 203d 2052 6573 7472 6963 7465 6451 7565   = RestrictedQue
+00000220: 7279 5365 742e 6173 5f6d 616e 6167 6572  rySet.as_manager
+00000230: 2829 0d0a 0d0a 2020 2020 6465 6620 5f5f  ()....    def __
+00000240: 7374 725f 5f28 7365 6c66 293a 0d0a 2020  str__(self):..  
+00000250: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00000260: 662e 6e61 6d65 0d0a 0d0a 2020 2020 6465  f.name....    de
+00000270: 6620 6765 745f 6162 736f 6c75 7465 5f75  f get_absolute_u
+00000280: 726c 2873 656c 6629 3a0d 0a20 2020 2020  rl(self):..     
+00000290: 2020 2072 6574 7572 6e20 7265 7665 7273     return revers
+000002a0: 6528 2270 6c75 6769 6e73 3a6e 6574 626f  e("plugins:netbo
+000002b0: 785f 736c 6d3a 736f 6674 7761 7265 7072  x_slm:softwarepr
+000002c0: 6f64 7563 7422 2c20 6b77 6172 6773 3d7b  oduct", kwargs={
+000002d0: 2270 6b22 3a20 7365 6c66 2e70 6b7d 290d  "pk": self.pk}).
+000002e0: 0a0d 0a20 2020 2064 6566 2067 6574 5f69  ...    def get_i
+000002f0: 6e73 7461 6c6c 6174 696f 6e5f 636f 756e  nstallation_coun
+00000300: 7428 7365 6c66 293a 0d0a 2020 2020 2020  t(self):..      
+00000310: 2020 636f 756e 7420 3d20 536f 6674 7761    count = Softwa
+00000320: 7265 5072 6f64 7563 7449 6e73 7461 6c6c  reProductInstall
+00000330: 6174 696f 6e2e 6f62 6a65 6374 732e 6669  ation.objects.fi
+00000340: 6c74 6572 2873 6f66 7477 6172 655f 7072  lter(software_pr
+00000350: 6f64 7563 745f 6964 3d73 656c 662e 706b  oduct_id=self.pk
+00000360: 292e 636f 756e 7428 290d 0a20 2020 2020  ).count()..     
+00000370: 2020 2072 6574 7572 6e20 7361 6665 7374     return safest
+00000380: 7269 6e67 2e6d 6172 6b5f 7361 6665 2822  ring.mark_safe("
+00000390: 3c61 2068 7265 663d 5c22 7b75 726c 7d5c  <a href=\"{url}\
+000003a0: 223e 7b63 6f75 6e74 7d3c 2f61 3e22 2e66  ">{count}</a>".f
+000003b0: 6f72 6d61 7428 0d0a 2020 2020 2020 2020  ormat(..        
+000003c0: 2020 2020 7572 6c3d 7265 7665 7273 655f      url=reverse_
+000003d0: 6c61 7a79 2822 706c 7567 696e 733a 6e65  lazy("plugins:ne
+000003e0: 7462 6f78 5f73 6c6d 3a73 6f66 7477 6172  tbox_slm:softwar
+000003f0: 6570 726f 6475 6374 696e 7374 616c 6c61  eproductinstalla
+00000400: 7469 6f6e 5f6c 6973 7422 2920 2b20 6622  tion_list") + f"
+00000410: 3f71 3d7b 7365 6c66 2e6e 616d 657d 222c  ?q={self.name}",
+00000420: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+00000430: 756e 743d 636f 756e 740d 0a20 2020 2020  unt=count..     
+00000440: 2020 2029 2920 6966 2063 6f75 6e74 2065     )) if count e
+00000450: 6c73 6520 2230 220d 0a0d 0a0d 0a63 6c61  lse "0"......cla
+00000460: 7373 2053 6f66 7477 6172 6550 726f 6475  ss SoftwareProdu
+00000470: 6374 5665 7273 696f 6e28 4e65 7442 6f78  ctVersion(NetBox
+00000480: 4d6f 6465 6c29 3a0d 0a20 2020 2073 6f66  Model):..    sof
+00000490: 7477 6172 655f 7072 6f64 7563 7420 3d20  tware_product = 
+000004a0: 6d6f 6465 6c73 2e46 6f72 6569 676e 4b65  models.ForeignKe
+000004b0: 7928 0d0a 2020 2020 2020 2020 746f 3d27  y(..        to='
+000004c0: 6e65 7462 6f78 5f73 6c6d 2e53 6f66 7477  netbox_slm.Softw
+000004d0: 6172 6550 726f 6475 6374 272c 0d0a 2020  areProduct',..  
+000004e0: 2020 2020 2020 6f6e 5f64 656c 6574 653d        on_delete=
+000004f0: 6d6f 6465 6c73 2e50 524f 5445 4354 2c0d  models.PROTECT,.
+00000500: 0a20 2020 2029 0d0a 2020 2020 6e61 6d65  .    )..    name
+00000510: 203d 206d 6f64 656c 732e 4368 6172 4669   = models.CharFi
+00000520: 656c 6428 6d61 785f 6c65 6e67 7468 3d36  eld(max_length=6
+00000530: 3429 0d0a 0d0a 2020 2020 6f62 6a65 6374  4)....    object
+00000540: 7320 3d20 5265 7374 7269 6374 6564 5175  s = RestrictedQu
+00000550: 6572 7953 6574 2e61 735f 6d61 6e61 6765  erySet.as_manage
+00000560: 7228 290d 0a0d 0a20 2020 2064 6566 205f  r()....    def _
+00000570: 5f73 7472 5f5f 2873 656c 6629 3a0d 0a20  _str__(self):.. 
+00000580: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00000590: 6c66 2e6e 616d 650d 0a0d 0a20 2020 2064  lf.name....    d
+000005a0: 6566 2067 6574 5f61 6273 6f6c 7574 655f  ef get_absolute_
+000005b0: 7572 6c28 7365 6c66 293a 0d0a 2020 2020  url(self):..    
+000005c0: 2020 2020 7265 7475 726e 2072 6576 6572      return rever
+000005d0: 7365 2822 706c 7567 696e 733a 6e65 7462  se("plugins:netb
+000005e0: 6f78 5f73 6c6d 3a73 6f66 7477 6172 6570  ox_slm:softwarep
+000005f0: 726f 6475 6374 7665 7273 696f 6e22 2c20  roductversion", 
+00000600: 6b77 6172 6773 3d7b 2270 6b22 3a20 7365  kwargs={"pk": se
+00000610: 6c66 2e70 6b7d 290d 0a0d 0a20 2020 2064  lf.pk})....    d
+00000620: 6566 2067 6574 5f69 6e73 7461 6c6c 6174  ef get_installat
+00000630: 696f 6e5f 636f 756e 7428 7365 6c66 293a  ion_count(self):
+00000640: 0d0a 2020 2020 2020 2020 636f 756e 7420  ..        count 
+00000650: 3d20 536f 6674 7761 7265 5072 6f64 7563  = SoftwareProduc
+00000660: 7449 6e73 7461 6c6c 6174 696f 6e2e 6f62  tInstallation.ob
+00000670: 6a65 6374 732e 6669 6c74 6572 2876 6572  jects.filter(ver
+00000680: 7369 6f6e 5f69 643d 7365 6c66 2e70 6b29  sion_id=self.pk)
+00000690: 2e63 6f75 6e74 2829 0d0a 2020 2020 2020  .count()..      
+000006a0: 2020 7265 7475 726e 2073 6166 6573 7472    return safestr
+000006b0: 696e 672e 6d61 726b 5f73 6166 6528 223c  ing.mark_safe("<
+000006c0: 6120 6872 6566 3d5c 227b 7572 6c7d 5c22  a href=\"{url}\"
+000006d0: 3e7b 636f 756e 747d 3c2f 613e 222e 666f  >{count}</a>".fo
+000006e0: 726d 6174 280d 0a20 2020 2020 2020 2020  rmat(..         
+000006f0: 2020 2075 726c 3d72 6576 6572 7365 5f6c     url=reverse_l
+00000700: 617a 7928 2270 6c75 6769 6e73 3a6e 6574  azy("plugins:net
+00000710: 626f 785f 736c 6d3a 736f 6674 7761 7265  box_slm:software
+00000720: 7072 6f64 7563 7469 6e73 7461 6c6c 6174  productinstallat
+00000730: 696f 6e5f 6c69 7374 2229 202b 2066 223f  ion_list") + f"?
+00000740: 713d 7b73 656c 662e 6e61 6d65 7d22 2c0d  q={self.name}",.
+00000750: 0a20 2020 2020 2020 2020 2020 2063 6f75  .            cou
+00000760: 6e74 3d63 6f75 6e74 0d0a 2020 2020 2020  nt=count..      
+00000770: 2020 2929 2069 6620 636f 756e 7420 656c    )) if count el
+00000780: 7365 2022 3022 0d0a 0d0a 0d0a 636c 6173  se "0"......clas
+00000790: 7320 536f 6674 7761 7265 5072 6f64 7563  s SoftwareProduc
+000007a0: 7449 6e73 7461 6c6c 6174 696f 6e28 4e65  tInstallation(Ne
+000007b0: 7442 6f78 4d6f 6465 6c29 3a0d 0a20 2020  tBoxModel):..   
+000007c0: 2064 6576 6963 6520 3d20 6d6f 6465 6c73   device = models
+000007d0: 2e46 6f72 6569 676e 4b65 7928 0d0a 2020  .ForeignKey(..  
+000007e0: 2020 2020 2020 746f 3d27 6463 696d 2e44        to='dcim.D
+000007f0: 6576 6963 6527 2c0d 0a20 2020 2020 2020  evice',..       
+00000800: 206f 6e5f 6465 6c65 7465 3d6d 6f64 656c   on_delete=model
+00000810: 732e 5052 4f54 4543 542c 0d0a 2020 2020  s.PROTECT,..    
+00000820: 2020 2020 6e75 6c6c 3d54 7275 652c 0d0a      null=True,..
+00000830: 2020 2020 2020 2020 626c 616e 6b3d 5472          blank=Tr
+00000840: 7565 0d0a 2020 2020 290d 0a20 2020 2076  ue..    )..    v
+00000850: 6972 7475 616c 6d61 6368 696e 6520 3d20  irtualmachine = 
+00000860: 6d6f 6465 6c73 2e46 6f72 6569 676e 4b65  models.ForeignKe
+00000870: 7928 0d0a 2020 2020 2020 2020 746f 3d27  y(..        to='
+00000880: 7669 7274 7561 6c69 7a61 7469 6f6e 2e56  virtualization.V
+00000890: 6972 7475 616c 4d61 6368 696e 6527 2c0d  irtualMachine',.
+000008a0: 0a20 2020 2020 2020 206f 6e5f 6465 6c65  .        on_dele
+000008b0: 7465 3d6d 6f64 656c 732e 5052 4f54 4543  te=models.PROTEC
+000008c0: 542c 0d0a 2020 2020 2020 2020 6e75 6c6c  T,..        null
+000008d0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+000008e0: 626c 616e 6b3d 5472 7565 0d0a 2020 2020  blank=True..    
+000008f0: 290d 0a20 2020 2073 6f66 7477 6172 655f  )..    software_
+00000900: 7072 6f64 7563 7420 3d20 6d6f 6465 6c73  product = models
+00000910: 2e46 6f72 6569 676e 4b65 7928 0d0a 2020  .ForeignKey(..  
+00000920: 2020 2020 2020 746f 3d27 6e65 7462 6f78        to='netbox
+00000930: 5f73 6c6d 2e53 6f66 7477 6172 6550 726f  _slm.SoftwarePro
+00000940: 6475 6374 272c 0d0a 2020 2020 2020 2020  duct',..        
+00000950: 6f6e 5f64 656c 6574 653d 6d6f 6465 6c73  on_delete=models
+00000960: 2e50 524f 5445 4354 2c0d 0a20 2020 2029  .PROTECT,..    )
+00000970: 0d0a 2020 2020 7665 7273 696f 6e20 3d20  ..    version = 
+00000980: 6d6f 6465 6c73 2e46 6f72 6569 676e 4b65  models.ForeignKe
+00000990: 7928 0d0a 2020 2020 2020 2020 746f 3d27  y(..        to='
+000009a0: 6e65 7462 6f78 5f73 6c6d 2e53 6f66 7477  netbox_slm.Softw
+000009b0: 6172 6550 726f 6475 6374 5665 7273 696f  areProductVersio
+000009c0: 6e27 2c0d 0a20 2020 2020 2020 206f 6e5f  n',..        on_
+000009d0: 6465 6c65 7465 3d6d 6f64 656c 732e 5052  delete=models.PR
+000009e0: 4f54 4543 542c 0d0a 2020 2020 290d 0a0d  OTECT,..    )...
+000009f0: 0a20 2020 206f 626a 6563 7473 203d 2052  .    objects = R
+00000a00: 6573 7472 6963 7465 6451 7565 7279 5365  estrictedQuerySe
+00000a10: 742e 6173 5f6d 616e 6167 6572 2829 0d0a  t.as_manager()..
+00000a20: 0d0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
+00000a30: 5f28 7365 6c66 293a 0d0a 2020 2020 2020  _(self):..      
+00000a40: 2020 7265 7475 726e 2066 227b 7365 6c66    return f"{self
+00000a50: 2e70 6b7d 220d 0a0d 0a20 2020 2064 6566  .pk}"....    def
+00000a60: 2067 6574 5f61 6273 6f6c 7574 655f 7572   get_absolute_ur
+00000a70: 6c28 7365 6c66 293a 0d0a 2020 2020 2020  l(self):..      
+00000a80: 2020 7265 7475 726e 2072 6576 6572 7365    return reverse
+00000a90: 2822 706c 7567 696e 733a 6e65 7462 6f78  ("plugins:netbox
+00000aa0: 5f73 6c6d 3a73 6f66 7477 6172 6570 726f  _slm:softwarepro
+00000ab0: 6475 6374 696e 7374 616c 6c61 7469 6f6e  ductinstallation
+00000ac0: 222c 206b 7761 7267 733d 7b22 706b 223a  ", kwargs={"pk":
+00000ad0: 2073 656c 662e 706b 7d29 0d0a 0d0a 2020   self.pk})....  
+00000ae0: 2020 6465 6620 6765 745f 706c 6174 666f    def get_platfo
+00000af0: 726d 2873 656c 6629 3a0d 0a20 2020 2020  rm(self):..     
+00000b00: 2020 2072 6574 7572 6e20 7365 6c66 2e64     return self.d
+00000b10: 6576 6963 6520 6f72 2073 656c 662e 7669  evice or self.vi
+00000b20: 7274 7561 6c6d 6163 6869 6e65 0d0a 0d0a  rtualmachine....
+00000b30: 2020 2020 6465 6620 7265 6e64 6572 5f74      def render_t
+00000b40: 7970 6528 7365 6c66 293a 0d0a 2020 2020  ype(self):..    
+00000b50: 2020 2020 7265 7475 726e 2027 6465 7669      return 'devi
+00000b60: 6365 2720 6966 2073 656c 662e 6465 7669  ce' if self.devi
+00000b70: 6365 2065 6c73 6520 2776 6972 7475 616c  ce else 'virtual
+00000b80: 6d61 6368 696e 6527 0d0a                 machine'..
```

### Comparing `netbox-slm-1.2/netbox_slm/filtersets.py` & `netbox-slm-1.3/netbox_slm/filtersets.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,55 @@
-from django.db.models import Q
-
-from netbox.filtersets import NetBoxModelFilterSet
-from netbox_slm.models import *
-
-
-class SoftwareProductFilterSet(NetBoxModelFilterSet):
-    """Filter capabilities for SoftwareProduct instances."""
-    class Meta:
-        model = SoftwareProduct
-        fields = tuple()
-
-    def search(self, queryset, name, value):
-        """Perform the filtered search."""
-        if not value.strip():
-            return queryset
-        qs_filter = Q(name__icontains=value) | \
-                    Q(manufacturer__name__icontains=value)
-        return queryset.filter(qs_filter)
-
-
-class SoftwareProductVersionFilterSet(NetBoxModelFilterSet):
-    """Filter capabilities for SoftwareProductVersion instances."""
-    class Meta:
-        model = SoftwareProductVersion
-        fields = (
-            "software_product",
-        )
-
-    def search(self, queryset, name, value):
-        """Perform the filtered search."""
-        if not value.strip():
-            return queryset
-        qs_filter = Q(name__icontains=value) | \
-                    Q(software_product__name__icontains=value) | \
-                    Q(software_product__manufacturer__name__icontains=value)
-        return queryset.filter(qs_filter)
-
-
-class SoftwareProductInstallationFilterSet(NetBoxModelFilterSet):
-    """Filter capabilities for SoftwareProductInstallation instances."""
-    class Meta:
-        model = SoftwareProductInstallation
-        fields = tuple()
-
-    def search(self, queryset, name, value):
-        """Perform the filtered search."""
-        if not value.strip():
-            return queryset
-        qs_filter = Q(software_product__name__icontains=value) | \
-                    Q(software_product__manufacturer__name__icontains=value) | \
-                    Q(version__name__icontains=value)
-        return queryset.filter(qs_filter)
+from django.db.models import Q
+
+from netbox.filtersets import NetBoxModelFilterSet
+from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation
+
+
+class SoftwareProductFilterSet(NetBoxModelFilterSet):
+    """Filter capabilities for SoftwareProduct instances."""
+
+    class Meta:
+        model = SoftwareProduct
+        fields = tuple()
+
+    def search(self, queryset, name, value):
+        """Perform the filtered search."""
+        if not value.strip():
+            return queryset
+        qs_filter = Q(name__icontains=value) | Q(manufacturer__name__icontains=value)
+        return queryset.filter(qs_filter)
+
+
+class SoftwareProductVersionFilterSet(NetBoxModelFilterSet):
+    """Filter capabilities for SoftwareProductVersion instances."""
+
+    class Meta:
+        model = SoftwareProductVersion
+        fields = (
+            "software_product",
+        )
+
+    def search(self, queryset, name, value):
+        """Perform the filtered search."""
+        if not value.strip():
+            return queryset
+        qs_filter = Q(name__icontains=value) | \
+                    Q(software_product__name__icontains=value) | \
+                    Q(software_product__manufacturer__name__icontains=value)
+        return queryset.filter(qs_filter)
+
+
+class SoftwareProductInstallationFilterSet(NetBoxModelFilterSet):
+    """Filter capabilities for SoftwareProductInstallation instances."""
+
+    class Meta:
+        model = SoftwareProductInstallation
+        fields = tuple()
+
+    def search(self, queryset, name, value):
+        """Perform the filtered search."""
+        if not value.strip():
+            return queryset
+        qs_filter = Q(software_product__name__icontains=value) | \
+                    Q(software_product__manufacturer__name__icontains=value) | \
+                    Q(version__name__icontains=value)
+        return queryset.filter(qs_filter)
```

### Comparing `netbox-slm-1.2/netbox_slm/forms.py` & `netbox-slm-1.3/netbox_slm/tables.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,174 +1,167 @@
-from django import forms
-from django.urls import reverse_lazy
-from django.utils.translation import gettext as _
-
-from dcim.models import Manufacturer, Device
-from netbox.forms import (
-    NetBoxModelForm,
-    NetBoxModelCSVForm,
-    NetBoxModelBulkEditForm,
-    NetBoxModelFilterSetForm,
-)
-from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation
-from utilities.forms import (
-    DynamicModelChoiceField, APISelect, TagFilterField, ChoiceField
-)
-from virtualization.models import VirtualMachine
-
-
-class SoftwareProductForm(NetBoxModelForm):
-    """Form for creating a new SoftwareProduct object."""
-
-    manufacturer = DynamicModelChoiceField(
-        queryset=Manufacturer.objects.all(),
-        required=True,
-    )
-
-    class Meta:
-        model = SoftwareProduct
-        fields = ("name", "manufacturer", "description", "tags")
-
-
-class SoftwareProductFilterForm(NetBoxModelFilterSetForm):
-    model = SoftwareProduct
-    fieldsets = (
-        (None, ('q', 'tag')),
-    )
-
-    tag = TagFilterField(model)
-
-
-class SoftwareProductCSVForm(NetBoxModelCSVForm):
-    class Meta:
-        model = SoftwareProduct
-        fields = ("name", "manufacturer",)
-
-
-class SoftwareProductBulkEditForm(NetBoxModelBulkEditForm):
-    pk = forms.ModelMultipleChoiceField(
-        queryset=SoftwareProduct.objects.all(),
-        widget=forms.MultipleHiddenInput(),
-    )
-
-    class Meta:
-        model = SoftwareProduct
-        nullable_fields = []
-
-
-class SoftwareProductVersionForm(NetBoxModelForm):
-    """Form for creating a new SoftwareProductVersion object."""
-    name = forms.CharField(label=_("Version"))
-
-    software_product = DynamicModelChoiceField(
-        queryset=SoftwareProduct.objects.all(),
-        widget=APISelect(
-            attrs={"data-url": reverse_lazy("plugins-api:netbox_slm-api:softwareproduct-list")}
-        ),
-    )
-
-    class Meta:
-        model = SoftwareProductVersion
-        fields = ("name", "software_product", "tags")
-
-
-class SoftwareProductVersionFilterForm(NetBoxModelFilterSetForm):
-    model = SoftwareProductVersion
-    fieldsets = (
-        (None, ('q', 'tag')),
-    )
-
-    tag = TagFilterField(model)
-
-
-class SoftwareProductVersionCSVForm(NetBoxModelCSVForm):
-    class Meta:
-        model = SoftwareProductVersion
-        fields = ("name",)
-
-
-class SoftwareProductVersionBulkEditForm(NetBoxModelBulkEditForm):
-    pk = forms.ModelMultipleChoiceField(
-        queryset=SoftwareProduct.objects.all(),
-        widget=forms.MultipleHiddenInput(),
-    )
-
-    class Meta:
-        model = SoftwareProductVersion
-        nullable_fields = []
-
-
-class SoftwareProductInstallationForm(NetBoxModelForm):
-    """Form for creating a new SoftwareProductInstallation object."""
-
-    device = DynamicModelChoiceField(
-        queryset=Device.objects.all(),
-        required=False,
-    )
-    virtualmachine = DynamicModelChoiceField(
-        queryset=VirtualMachine.objects.all(),
-        required=False,
-    )
-    software_product = DynamicModelChoiceField(
-        queryset=SoftwareProduct.objects.all(),
-        required=True,
-        widget=APISelect(
-            attrs={"data-url": reverse_lazy("plugins-api:netbox_slm-api:softwareproduct-list")}
-        ),
-    )
-    version = DynamicModelChoiceField(
-        queryset=SoftwareProductVersion.objects.all(),
-        required=True,
-        widget=APISelect(
-            attrs={"data-url": reverse_lazy("plugins-api:netbox_slm-api:softwareproductversion-list")}
-        ),
-        query_params={
-            'software_product': '$software_product',
-        }
-    )
-
-    class Meta:
-        model = SoftwareProductInstallation
-        fields = ("device", "virtualmachine", "software_product", "version", "tags")
-
-    def clean_version(self):
-        version = self.cleaned_data['version']
-        software_product = self.cleaned_data['software_product']
-        if version not in software_product.softwareproductversion_set.all():
-            raise forms.ValidationError(_(f"Version `{version}` doesn't exist on {software_product}, make sure you've "
-                                          f"selected a compatible version or first select the software product."))
-        return version
-
-    def clean(self):
-        if not any([self.cleaned_data['device'], self.cleaned_data['virtualmachine']]):
-            raise forms.ValidationError(_("Installation requires atleast one virtualmachine or device destination."))
-        return super(SoftwareProductInstallationForm, self).clean()
-
-
-class SoftwareProductInstallationFilterForm(NetBoxModelFilterSetForm):
-    model = SoftwareProductInstallation
-    fieldsets = (
-        (None, ('q', 'tag',)),
-    )
-
-    tag = TagFilterField(model)
-
-
-class SoftwareProductInstallationCSVForm(NetBoxModelCSVForm):
-    class Meta:
-        model = SoftwareProductInstallation
-        fields = tuple()
-
-
-class SoftwareProductInstallationBulkEditForm(NetBoxModelBulkEditForm):
-    software_product = DynamicModelChoiceField(
-        queryset=SoftwareProduct.objects.all(),
-        required=False
-    )
-    version = DynamicModelChoiceField(
-        queryset=SoftwareProductVersion.objects.all(),
-        required=False
-    )
-    model = SoftwareProductInstallation
-    fieldsets = (
-        (None, ('software_product', 'version',)),
-    )
+import django_tables2 as tables
+from django.db.models import Count
+from django_tables2.utils import Accessor
+
+from netbox.tables import NetBoxTable, ToggleColumn, columns
+from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation
+
+
+class SoftwareProductTable(NetBoxTable):
+    """Table for displaying SoftwareProduct objects."""
+
+    pk = ToggleColumn()
+    name = tables.LinkColumn()
+    manufacturer = tables.Column(
+        accessor=Accessor('manufacturer'),
+        linkify=True
+    )
+    installations = tables.Column(accessor='get_installation_count', verbose_name='Installations')
+
+    tags = columns.TagColumn(
+        url_name="plugins:netbox_slm:softwareproduct_list",
+    )
+
+    class Meta(NetBoxTable.Meta):
+        model = SoftwareProduct
+        fields = (
+            "pk",
+            "name",
+            "manufacturer",
+            "description",
+            "installations",
+            "tags",
+        )
+        default_columns = (
+            "pk",
+            "name",
+            "manufacturer",
+            "description",
+            "installations",
+            "tags",
+        )
+        sequence = (
+            "manufacturer",
+            "name",
+            "description",
+            "installations",
+        )
+
+    def order_installations(self, queryset, is_descending):
+        queryset = queryset.annotate(
+            count=Count('softwareproductinstallation__id')
+        ).order_by(("-" if is_descending else "") + "count")
+        return queryset, True
+
+
+class SoftwareProductVersionTable(NetBoxTable):
+    """Table for displaying SoftwareProductVersion objects."""
+
+    pk = ToggleColumn()
+    name = tables.LinkColumn(verbose_name='Version')
+    software_product = tables.Column(
+        accessor=Accessor('software_product'),
+        linkify=True
+    )
+    manufacturer = tables.Column(
+        accessor=Accessor('software_product__manufacturer'),
+        linkify=True
+    )
+    installations = tables.Column(accessor='get_installation_count', verbose_name='Installations')
+
+    tags = columns.TagColumn(
+        url_name="plugins:netbox_slm:softwareproductversion_list",
+    )
+
+    class Meta(NetBoxTable.Meta):
+        model = SoftwareProductVersion
+        fields = (
+            "pk",
+            "name",
+            "software_product",
+            "manufacturer",
+            "installations",
+            "tags",
+        )
+        default_columns = (
+            "pk",
+            "name",
+            "software_product",
+            "manufacturer",
+            "installations",
+            "tags",
+        )
+        sequence = (
+            "manufacturer",
+            "software_product",
+            "name",
+            "installations",
+        )
+
+    def order_installations(self, queryset, is_descending):
+        queryset = queryset.annotate(
+            count=Count('softwareproductinstallation__id')
+        ).order_by(("-" if is_descending else "") + "count")
+        return queryset, True
+
+
+class SoftwareProductInstallationTable(NetBoxTable):
+    """Table for displaying SoftwareProductInstallation objects."""
+
+    pk = ToggleColumn()
+    name = tables.LinkColumn()
+    device = tables.Column(
+        accessor=Accessor('device'),
+        linkify=True
+    )
+    virtualmachine = tables.Column(
+        accessor=Accessor('virtualmachine'),
+        linkify=True
+    )
+    platform = tables.Column(
+        accessor='get_platform',
+        linkify=True
+    )
+    type = tables.Column(accessor='render_type')
+    software_product = tables.Column(
+        accessor=Accessor('software_product'),
+        linkify=True
+    )
+    version = tables.Column(
+        accessor=Accessor('version'),
+        linkify=True
+    )
+
+    tags = columns.TagColumn(
+        url_name="plugins:netbox_slm:softwareproductinstallation_list",
+    )
+
+    class Meta(NetBoxTable.Meta):
+        model = SoftwareProductInstallation
+        fields = (
+            "pk",
+            "name",
+            "platform",
+            "type",
+            "software_product",
+            "version",
+            "tags",
+        )
+        default_columns = (
+            "pk",
+            "platform",
+            "type",
+            "software_product",
+            "version",
+            "tags",
+        )
+
+    def order_platform(self, queryset, is_descending):
+        queryset = queryset.order_by(("device" if is_descending else "virtualmachine"))
+        return queryset, True
+
+    def order_type(self, queryset, is_descending):
+        queryset = queryset.order_by(("device" if is_descending else "virtualmachine"))
+        return queryset, True
+
+    def render_software_product(self, value, **kwargs):
+        return f"{kwargs['record'].software_product.manufacturer.name} - {value}"
```

### Comparing `netbox-slm-1.2/netbox_slm/api/urls.py` & `netbox-slm-1.3/netbox_slm/api/urls.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from netbox.api.routers import NetBoxRouter
-from netbox_slm.api.views import (
-    NetboxSLMRootView,
-    SoftwareProductViewSet,
-    SoftwareProductVersionViewSet,
-    SoftwareProductInstallationViewSet,
-)
-
-router = NetBoxRouter()
-router.APIRootView = NetboxSLMRootView
-
-router.register("softwareproducts", SoftwareProductViewSet)
-router.register("softwareproductversions", SoftwareProductVersionViewSet)
-router.register("softwareproductinstallations", SoftwareProductInstallationViewSet)
-urlpatterns = router.urls
+from netbox.api.routers import NetBoxRouter
+from netbox_slm.api.views import (
+    NetboxSLMRootView,
+    SoftwareProductViewSet,
+    SoftwareProductVersionViewSet,
+    SoftwareProductInstallationViewSet,
+)
+
+router = NetBoxRouter()
+router.APIRootView = NetboxSLMRootView
+
+router.register("softwareproducts", SoftwareProductViewSet)
+router.register("softwareproductversions", SoftwareProductVersionViewSet)
+router.register("softwareproductinstallations", SoftwareProductInstallationViewSet)
+urlpatterns = router.urls
```

### Comparing `netbox-slm-1.2/netbox_slm/templates/netbox_slm/softwareproductinstallation.html` & `netbox-slm-1.3/netbox_slm/templates/netbox_slm/softwareproductinstallation.html`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-{% extends 'generic/object.html' %}
-{% load buttons %}
-{% load static %}
-{% load helpers %}
-{% load plugins %}
-
-{% block content %}
-<div class="row my-3">
-	<div class="col col-md-6">
-        <div class="card">
-            <h5 class="card-header">
-                Software Product Installation
-            </h5>
-            <div class="card-body">
-                <table class="table table-hover attr-table">
-                    {% if object.device %}
-                    <tr>
-                        <th scope="row">Device</th>
-                        <td>{{ object.device }}</td>
-                    </tr>
-                    {% else %}
-                    <tr>
-                        <th scope="row">Virtualmachine</th>
-                        <td>{{ object.virtualmachine }}</td>
-                    </tr>
-                    {% endif %}
-                    <tr>
-                        <th scope="row">Software Product</th>
-                        <td>{{ object.software_product }}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Version</th>
-                        <td>{{ object.version }}</td>
-                    </tr>
-                </table>
-            </div>
-        </div>
-        {% include 'inc/panels/custom_fields.html' %}
-        {% include 'inc/panels/tags.html' %}
-{#        {% include 'inc/panels/comments.html' %}#}
-        {% plugin_left_page object %}
-    </div>
-</div>
-<div class="row">
-    <div class="col col-md-12">
-        {% plugin_full_width_page object %}
-    </div>
-</div>
-{% endblock %}
+{% extends 'generic/object.html' %}
+{% load buttons %}
+{% load static %}
+{% load helpers %}
+{% load plugins %}
+
+{% block content %}
+<div class="row my-3">
+	<div class="col col-md-6">
+        <div class="card">
+            <h5 class="card-header">
+                Software Product Installation
+            </h5>
+            <div class="card-body">
+                <table class="table table-hover attr-table">
+                    {% if object.device %}
+                    <tr>
+                        <th scope="row">Device</th>
+                        <td>{{ object.device }}</td>
+                    </tr>
+                    {% else %}
+                    <tr>
+                        <th scope="row">Virtualmachine</th>
+                        <td>{{ object.virtualmachine }}</td>
+                    </tr>
+                    {% endif %}
+                    <tr>
+                        <th scope="row">Software Product</th>
+                        <td>{{ object.software_product }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Version</th>
+                        <td>{{ object.version }}</td>
+                    </tr>
+                </table>
+            </div>
+        </div>
+        {% include 'inc/panels/custom_fields.html' %}
+        {% include 'inc/panels/tags.html' %}
+{#        {% include 'inc/panels/comments.html' %}#}
+        {% plugin_left_page object %}
+    </div>
+</div>
+<div class="row">
+    <div class="col col-md-12">
+        {% plugin_full_width_page object %}
+    </div>
+</div>
+{% endblock %}
```

### Comparing `netbox-slm-1.2/netbox_slm/templates/netbox_slm/softwareproductversion.html` & `netbox-slm-1.3/netbox_slm/templates/netbox_slm/softwareproductversion.html`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-{% extends 'generic/object.html' %}
-{% load buttons %}
-{% load static %}
-{% load helpers %}
-{% load plugins %}
-
-{% block content %}
-<div class="row my-3">
-	<div class="col col-md-6">
-        <div class="card">
-            <h5 class="card-header">
-                Software Product Version
-            </h5>
-            <div class="card-body">
-                <table class="table table-hover attr-table">
-                    <tr>
-                        <th scope="row">Name</th>
-                        <td>{{ object.name }}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Installations</th>
-                        <td>
-                            {{ object.get_installation_count }}
-                        </td>
-                    </tr>
-                </table>
-            </div>
-        </div>
-        {% include 'inc/panels/custom_fields.html' %}
-        {% include 'inc/panels/tags.html' %}
-{#        {% include 'inc/panels/comments.html' %}#}
-        {% plugin_left_page object %}
-    </div>
-</div>
-<div class="row">
-    <div class="col col-md-12">
-        {% plugin_full_width_page object %}
-    </div>
-</div>
-{% endblock %}
+{% extends 'generic/object.html' %}
+{% load buttons %}
+{% load static %}
+{% load helpers %}
+{% load plugins %}
+
+{% block content %}
+<div class="row my-3">
+	<div class="col col-md-6">
+        <div class="card">
+            <h5 class="card-header">
+                Software Product Version
+            </h5>
+            <div class="card-body">
+                <table class="table table-hover attr-table">
+                    <tr>
+                        <th scope="row">Name</th>
+                        <td>{{ object.name }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Installations</th>
+                        <td>
+                            {{ object.get_installation_count }}
+                        </td>
+                    </tr>
+                </table>
+            </div>
+        </div>
+        {% include 'inc/panels/custom_fields.html' %}
+        {% include 'inc/panels/tags.html' %}
+{#        {% include 'inc/panels/comments.html' %}#}
+        {% plugin_left_page object %}
+    </div>
+</div>
+<div class="row">
+    <div class="col col-md-12">
+        {% plugin_full_width_page object %}
+    </div>
+</div>
+{% endblock %}
```

### Comparing `netbox-slm-1.2/netbox_slm/templates/netbox_slm/softwareproduct.html` & `netbox-slm-1.3/netbox_slm/templates/netbox_slm/softwareproduct.html`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-{% extends 'generic/object.html' %}
-{% load buttons %}
-{% load static %}
-{% load helpers %}
-{% load plugins %}
-
-{% block content %}
-<div class="row my-3">
-	<div class="col col-md-6">
-        <div class="card">
-            <h5 class="card-header">
-                Software Product
-            </h5>
-            <div class="card-body">
-                <table class="table table-hover attr-table">
-                    <tr>
-                        <th scope="row">Name</th>
-                        <td>{{ object }}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Versions</th>
-                        <td>
-                        {% for version in object.softwareproduct_versions.all %}
-                            <a href="{% url 'plugins:netbox_slm:softwareproductversion' pk=version.pk %}">
-                                <span class="badge" style="color: #ffffff; background-color: #9e9e9e">{{ version }}</span>
-                            </a>
-                        {% empty %}
-                            n/a
-                        {% endfor %}
-                        </td>
-                    </tr>
-                </table>
-            </div>
-        </div>
-        {% include 'inc/panels/custom_fields.html' %}
-        {% include 'inc/panels/tags.html' %}
-{#        {% include 'inc/panels/comments.html' %}#}
-        {% plugin_left_page object %}
-    </div>
-</div>
-<div class="row">
-    <div class="col col-md-12">
-        {% plugin_full_width_page object %}
-    </div>
-</div>
-{% endblock %}
+{% extends 'generic/object.html' %}
+{% load buttons %}
+{% load static %}
+{% load helpers %}
+{% load plugins %}
+
+{% block content %}
+<div class="row my-3">
+	<div class="col col-md-6">
+        <div class="card">
+            <h5 class="card-header">
+                Software Product
+            </h5>
+            <div class="card-body">
+                <table class="table table-hover attr-table">
+                    <tr>
+                        <th scope="row">Name</th>
+                        <td>{{ object }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Versions</th>
+                        <td>
+                        {% for version in object.softwareproduct_versions.all %}
+                            <a href="{% url 'plugins:netbox_slm:softwareproductversion' pk=version.pk %}">
+                                <span class="badge" style="color: #ffffff; background-color: #9e9e9e">{{ version }}</span>
+                            </a>
+                        {% empty %}
+                            n/a
+                        {% endfor %}
+                        </td>
+                    </tr>
+                </table>
+            </div>
+        </div>
+        {% include 'inc/panels/custom_fields.html' %}
+        {% include 'inc/panels/tags.html' %}
+{#        {% include 'inc/panels/comments.html' %}#}
+        {% plugin_left_page object %}
+    </div>
+</div>
+<div class="row">
+    <div class="col col-md-12">
+        {% plugin_full_width_page object %}
+    </div>
+</div>
+{% endblock %}
```

### Comparing `netbox-slm-1.2/netbox_slm/navigation.py` & `netbox-slm-1.3/netbox_slm/navigation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,65 @@
-from extras.plugins import PluginMenuButton, PluginMenuItem
-from utilities.choices import ButtonColorChoices
-
-
-menu_items = (
-    PluginMenuItem(
-        link='plugins:netbox_slm:softwareproduct_list',
-        link_text='Software Products',
-        buttons=(
-            PluginMenuButton(
-                "plugins:netbox_slm:softwareproduct_add",
-                "Add",
-                "mdi mdi-plus-thick",
-                ButtonColorChoices.GREEN,
-                permissions=["netbox_slm.add_softwareproduct"],
-            ),
-            PluginMenuButton(
-                "plugins:netbox_slm:softwareproduct_import",
-                "Import",
-                "mdi mdi-upload",
-                ButtonColorChoices.CYAN,
-                permissions=["netbox_slm.add_softwareproduct"],
-            ),
-        )
-    ),
-    PluginMenuItem(
-        link='plugins:netbox_slm:softwareproductversion_list',
-        link_text='Versions',
-        buttons=(
-            PluginMenuButton(
-                "plugins:netbox_slm:softwareproductversion_add",
-                "Add",
-                "mdi mdi-plus-thick",
-                ButtonColorChoices.GREEN,
-                permissions=["netbox_slm.add_softwareproductversion"],
-            ),
-            PluginMenuButton(
-                "plugins:netbox_slm:softwareproductversion_import",
-                "Import",
-                "mdi mdi-upload",
-                ButtonColorChoices.CYAN,
-                permissions=["netbox_slm.add_softwareproductversion"],
-            ),
-        )
-    ),
-    PluginMenuItem(
-        link='plugins:netbox_slm:softwareproductinstallation_list',
-        link_text='Installations',
-        buttons=(
-            PluginMenuButton(
-                "plugins:netbox_slm:softwareproductinstallation_add",
-                "Add",
-                "mdi mdi-plus-thick",
-                ButtonColorChoices.GREEN,
-                permissions=["netbox_slm.add_softwareproductinstallation"],
-            ),
-            PluginMenuButton(
-                "plugins:netbox_slm:softwareproductinstallation_import",
-                "Import",
-                "mdi mdi-upload",
-                ButtonColorChoices.CYAN,
-                permissions=["netbox_slm.add_softwareproductinstallation"],
-            ),
-        )
-    ),
-)
+from extras.plugins import PluginMenuButton, PluginMenuItem
+from utilities.choices import ButtonColorChoices
+
+menu_items = (
+    PluginMenuItem(
+        link='plugins:netbox_slm:softwareproduct_list',
+        link_text='Software Products',
+        buttons=(
+            PluginMenuButton(
+                "plugins:netbox_slm:softwareproduct_add",
+                "Add",
+                "mdi mdi-plus-thick",
+                ButtonColorChoices.GREEN,
+                permissions=["netbox_slm.add_softwareproduct"],
+            ),
+            PluginMenuButton(
+                "plugins:netbox_slm:softwareproduct_import",
+                "Import",
+                "mdi mdi-upload",
+                ButtonColorChoices.CYAN,
+                permissions=["netbox_slm.add_softwareproduct"],
+            ),
+        )
+    ),
+    PluginMenuItem(
+        link='plugins:netbox_slm:softwareproductversion_list',
+        link_text='Versions',
+        buttons=(
+            PluginMenuButton(
+                "plugins:netbox_slm:softwareproductversion_add",
+                "Add",
+                "mdi mdi-plus-thick",
+                ButtonColorChoices.GREEN,
+                permissions=["netbox_slm.add_softwareproductversion"],
+            ),
+            PluginMenuButton(
+                "plugins:netbox_slm:softwareproductversion_import",
+                "Import",
+                "mdi mdi-upload",
+                ButtonColorChoices.CYAN,
+                permissions=["netbox_slm.add_softwareproductversion"],
+            ),
+        )
+    ),
+    PluginMenuItem(
+        link='plugins:netbox_slm:softwareproductinstallation_list',
+        link_text='Installations',
+        buttons=(
+            PluginMenuButton(
+                "plugins:netbox_slm:softwareproductinstallation_add",
+                "Add",
+                "mdi mdi-plus-thick",
+                ButtonColorChoices.GREEN,
+                permissions=["netbox_slm.add_softwareproductinstallation"],
+            ),
+            PluginMenuButton(
+                "plugins:netbox_slm:softwareproductinstallation_import",
+                "Import",
+                "mdi mdi-upload",
+                ButtonColorChoices.CYAN,
+                permissions=["netbox_slm.add_softwareproductinstallation"],
+            ),
+        )
+    ),
+)
```

### Comparing `netbox-slm-1.2/LICENSE` & `netbox-slm-1.3/LICENSE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Copyright 2022 ICTU
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-   http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
+Copyright 2022 ICTU
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+   http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `netbox-slm-1.2/netbox_slm.egg-info/SOURCES.txt` & `netbox-slm-1.3/netbox_slm.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,8 +24,10 @@
 netbox_slm/migrations/0002_alter_softwareproduct_manufacturer.py
 netbox_slm/migrations/0003_auto_20220407_1209.py
 netbox_slm/migrations/0004_auto_20220415_0705.py
 netbox_slm/migrations/__init__.py
 netbox_slm/templates/netbox_slm/softwareproduct.html
 netbox_slm/templates/netbox_slm/softwareproductinstallation.html
 netbox_slm/templates/netbox_slm/softwareproductversion.html
-netbox_slm/templatetags/__init__.py
+netbox_slm/templatetags/__init__.py
+netbox_slm/tests/__init__.py
+netbox_slm/tests/test_models.py
```

### Comparing `netbox-slm-1.2/README.md` & `netbox-slm-1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-<h1 align="center">NetBox SLM</h1>
-
-<p align="center"><i>Netbox SLM is a plugin for lifecycle management of software components, including versions and installations.</i></p>
-
-<div align="center">
-<a href="https://pypi.org/project/netbox_slm/"><img src="https://img.shields.io/pypi/v/netbox_slm" alt="PyPi"/></a>
-<a href="https://github.com/ICTU/netbox_slm/stargazers"><img src="https://img.shields.io/github/stars/ICTU/netbox_slm" alt="Stars Badge"/></a>
-<a href="https://github.com/ICTU/netbox_slm/network/members"><img src="https://img.shields.io/github/forks/ICTU/netbox_slm" alt="Forks Badge"/></a>
-<a href="https://github.com/ICTU/netbox_slm/pulls"><img src="https://img.shields.io/github/issues-pr/ICTU/netbox_slm" alt="Pull Requests Badge"/></a>
-<a href="https://github.com/ICTU/netbox_slm/issues"><img src="https://img.shields.io/github/issues/ICTU/netbox_slm" alt="Issues Badge"/></a>
-<a href="https://github.com/ICTU/netbox_slm/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/ICTU/netbox_slm?color=2b9348"></a>
-<a href="https://github.com/ICTU/netbox_slm/blob/master/LICENSE"><img src="https://img.shields.io/github/license/ICTU/netbox_slm?color=2b9348" alt="License Badge"/></a>
-</div>
-
-
-## Known Issues
-
-- WARNING: This plugin is only tested with Netbox 3.2 at this time.
-- CSV/Bulk imports for SoftwareProduct, Version and Installation are currently broken (WIP)
-
-## Installation Guide
-
-When using the Docker version of Netbox, first follow the netbox-docker [quickstart](https://github.com/netbox-community/netbox-docker#quickstart) instructions to clone the netbox-docker repo and set up the ``docker-compose.override.yml``.
-
-Next, follow these instructions (based on the Netbox docker variant
-[instructions](https://github.com/netbox-community/netbox-docker/wiki/Configuration#custom-configuration-files))
-to install the Netbox SLM plugin:
-
-1. Add ``netbox_slm`` to the ``PLUGINS`` list in
-   ``configuration/extra.py``.
-2. Create a ``plugin_requirements.txt`` with ``netbox-slm==1.2`` as
-   contents.
-3. Create a ``Dockerfile-SLM`` with contents:
-
-   ```
-   FROM netboxcommunity/netbox:v3.2.X
-
-   COPY ./plugin_requirements.txt /
-   RUN /opt/netbox/venv/bin/pip install --no-warn-script-location -r /plugin_requirements.txt
-   ```
-
-4. Create a ``docker-compose.override.yml`` with contents:
-
-   ```
-   version: '3.4'
-   services:
-     netbox:
-       ports:
-         - 8000:8080
-       build:
-         context: .
-         dockerfile: Dockerfile-SLM
-       image: netbox:slm
-     netbox-worker:
-       image: netbox:slm
-     netbox-housekeeping:
-       image: netbox:slm
-   ```
-
-Now, build the image: ``docker compose build --no-cache``
-
-And finally, run Netbox with the SLM plugin: ``docker compose up``
-
-## Releasing Guide
-
-To draft a release;
-
-update the setup.py file to reflect the new version, then from the *src*
-directory run
-
-   ```
-   # make sure to update the version in netbox_slm/__init__.py
-   $ python setup.py sdist
-   $ twine upload dist/*
-   ```
-
-On Github.com create a similar tag and version. These steps could be
-automated with a github workflow.
-
-n.b. Currently the plugin is configured to use a personal pypi account,
-this should be changed.
-
-## Developer Guide (local installation)
-
-*Follow the steps below on your local system to run netbox and the
-netbox_slm plugin in developer mode*
-
-### Setup
-
-The goal below is to run all Netbox components in Docker and run a local
-Netbox Django copy with auto-reload to develop the plugin pointing to
-the Dockerized postgres and redis instances, basically ignoring the
-netbox docker runtime server.
-
-### Steps
-
-   from your projects directory clone the netbox repository
-
-   ```
-   $ git clone https://github.com/netbox-community/netbox
-   $ cd netbox
-   ```
-   
-   install the virtual environment
-   
-   ```
-   $ pipenv shell
-   $ pipenv install
-   ```
-
-   create and edit netbox/configuration.py (based on the template file) add these lines at the end of the file;
-   
-   ```
-   DEBUG = True
-   SECRET_KEY = 'dummy'
-   DEVELOPER = True
-   PLUGINS = [
-       'netbox_slm',
-   ]
-   ```
-
-The Netbox installation above will be used to run Django management
-commands like runserver, makemigrations and migrate, which will be
-explained in the next steps below;
-
-   from your projects directory clone the netbox-slm repository
-
-   ```
-   $ git clone https://github.com/ICTU/netbox_slm
-   $ cd netbox_slm
-   $ ./start-netbox.sh
-   ```
-   
-This will start Netbox locally (requires Docker) and forward the redis
-and postgres ports to the localhost (make sure there’s no processes
-using these ports or change the dockerfiles accordingly)
-
-Note, you can also start and stop netbox by hand:
-
-   ```
-   $ cd netbox-docker
-   $ docker-compose up -d
-   ```
-   
-   or stop the stack with
-
-   ```
-   $ docker-compose down
-   ```
-   
-   # to start fresh:
-
-   ```
-   $ docker-compose down
-   $ docker volume rm netbox-docker_netbox-postgres-data  # et cetera
-   $ docker-compose up -d --force-recreate
-   ```
-   
-   this will require you to re-run the migrate commando's for netbox-slm, see further down below
-
-Go back to the netbox configuration.py file and update the postgres and
-redis connection strings (username, password) to the ones the netbox
-docker backend is using, for example (using default user and passwords
-from the netbox docker example):
-
-   ```
-   <<collapsed>>
-
-   # PostgreSQL database configuration. See the Django documentation for a complete list of available parameters:
-   #   https://docs.djangoproject.com/en/stable/ref/settings/#databases
-   DATABASE = {
-       'NAME': 'netbox',               # Database name
-       'USER': 'netbox',               # PostgreSQL username
-       'PASSWORD': 'J5brHrAXFLQSif0K', # PostgreSQL password
-       'HOST': 'localhost',            # Database server
-       'PORT': '',                     # Database port (leave blank for default)
-       'CONN_MAX_AGE': 300,            # Max database connection age
-   }
-
-   # Redis database settings. Redis is used for caching and for queuing background tasks such as webhook events. A separate
-   # configuration exists for each. Full connection details are required in both sections, and it is strongly recommended
-   # to use two separate database IDs.
-   REDIS = {
-       'tasks': {
-           'HOST': 'localhost',
-           'PORT': 6379,
-           # Comment out `HOST` and `PORT` lines and uncomment the following if using Redis Sentinel
-           # 'SENTINELS': [('mysentinel.redis.example.com', 6379)],
-           # 'SENTINEL_SERVICE': 'netbox',
-           'PASSWORD': 'H733Kdjndks81',
-           'DATABASE': 0,
-           'SSL': False,
-           # Set this to True to skip TLS certificate verification
-           # This can expose the connection to attacks, be careful
-           # 'INSECURE_SKIP_TLS_VERIFY': False,
-       },
-       'caching': {
-           'HOST': 'localhost',
-           'PORT': 6379,
-           # Comment out `HOST` and `PORT` lines and uncomment the following if using Redis Sentinel
-           # 'SENTINELS': [('mysentinel.redis.example.com', 6379)],
-           # 'SENTINEL_SERVICE': 'netbox',
-           'PASSWORD': 'H733Kdjndks81',
-           'DATABASE': 1,
-           'SSL': False,
-           # Set this to True to skip TLS certificate verification
-           # This can expose the connection to attacks, be careful
-           # 'INSECURE_SKIP_TLS_VERIFY': False,
-       }
-   }
-
-   <<collapsed>>
-   ```
-   
-Now you can run commands from the netbox repository like this;
-
-   ```
-   $ cd netbox/netbox
-   $ export PYTHONPATH=../../netbox_slm/netbox_slm/  # or with the pipenv activated run `python3 setup.py develop` from the netbox_slm directory
-   $ python3 manage.py migrate netbox_slm
-   $ python3 manage.py runserver 8001
-   ```
-
-Visit http://127.0.0.1:8001 in the browser to see the auto reloading
-version of the netbox UI. Port 8000 is taken by the docker ran variant.
+<h1 align="center">NetBox SLM</h1>
+
+<p align="center"><i>Netbox SLM is a plugin for lifecycle management of software components, including versions and installations.</i></p>
+
+<div align="center">
+<a href="https://pypi.org/project/netbox_slm/"><img src="https://img.shields.io/pypi/v/netbox_slm" alt="PyPi"/></a>
+<a href="https://github.com/ICTU/netbox_slm/stargazers"><img src="https://img.shields.io/github/stars/ICTU/netbox_slm" alt="Stars Badge"/></a>
+<a href="https://github.com/ICTU/netbox_slm/network/members"><img src="https://img.shields.io/github/forks/ICTU/netbox_slm" alt="Forks Badge"/></a>
+<a href="https://github.com/ICTU/netbox_slm/pulls"><img src="https://img.shields.io/github/issues-pr/ICTU/netbox_slm" alt="Pull Requests Badge"/></a>
+<a href="https://github.com/ICTU/netbox_slm/issues"><img src="https://img.shields.io/github/issues/ICTU/netbox_slm" alt="Issues Badge"/></a>
+<a href="https://github.com/ICTU/netbox_slm/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/ICTU/netbox_slm?color=2b9348"></a>
+<a href="https://github.com/ICTU/netbox_slm/blob/master/LICENSE"><img src="https://img.shields.io/github/license/ICTU/netbox_slm?color=2b9348" alt="License Badge"/></a>
+</div>
+
+
+## Known Issues
+
+- WARNING: This plugin is only tested with a single Netbox version at this time.
+- CSV/Bulk imports for SoftwareProduct, Version and Installation are currently broken (WIP)
+
+## Installation Guide
+
+When using the Docker version of Netbox, first follow the netbox-docker [quickstart](https://github.com/netbox-community/netbox-docker#quickstart) instructions to clone the netbox-docker repo and set up the ``docker-compose.override.yml``.
+
+Next, follow these instructions (based on the Netbox docker variant
+[instructions](https://github.com/netbox-community/netbox-docker/wiki/Configuration#custom-configuration-files))
+to install the Netbox SLM plugin:
+
+1. Add ``netbox_slm`` to the ``PLUGINS`` list in
+   ``configuration/extra.py``.
+2. Create a ``plugin_requirements.txt`` with ``netbox-slm==1.2`` as
+   contents.
+3. Create a ``Dockerfile-SLM`` with contents:
+
+   ```
+   FROM netboxcommunity/netbox:vX.Y.Z
+
+   COPY ./plugin_requirements.txt /
+   RUN /opt/netbox/venv/bin/pip install --no-warn-script-location -r /plugin_requirements.txt
+   ```
+
+4. Create a ``docker-compose.override.yml`` with contents:
+
+   ```
+   version: '3.7'
+   services:
+     netbox:
+       ports:
+         - 8000:8080
+       build:
+         context: .
+         dockerfile: Dockerfile-SLM
+       image: netbox:slm
+     netbox-worker:
+       image: netbox:slm
+     netbox-housekeeping:
+       image: netbox:slm
+   ```
+
+Now, build the image: ``docker compose build --no-cache``
+
+And finally, run Netbox with the SLM plugin: ``docker compose up``
+
+## Releasing Guide
+
+To draft a release;
+
+update the setup.py file to reflect the new version, then from the *src*
+directory run
+
+   ```
+   # make sure to update the version in netbox_slm/__init__.py
+   $ python setup.py sdist
+   $ twine upload dist/*
+   ```
+
+On Github.com create a similar tag and version. These steps could be
+automated with a github workflow.
+
+n.b. Currently the plugin is configured to use a personal pypi account,
+this should be changed.
+
+## Developer Guide (local installation)
+
+*Follow the steps below on your local system to run netbox and the
+netbox_slm plugin in developer mode*
+
+### Setup
+
+The goal below is to run all Netbox components in Docker and run a local
+Netbox Django copy with auto-reload to develop the plugin pointing to
+the Dockerized postgres and redis instances, basically ignoring the
+netbox docker runtime server.
+
+### Steps
+
+   from your projects directory clone the netbox repository
+
+   ```
+   $ git clone https://github.com/netbox-community/netbox
+   $ cd netbox
+   ```
+   
+   install the virtual environment
+   
+   ```
+   $ pipenv shell
+   $ pipenv install
+   ```
+
+   create and edit netbox/configuration.py (based on the template file) add these lines at the end of the file;
+   
+   ```
+   DEBUG = True
+   SECRET_KEY = 'dummy'
+   DEVELOPER = True
+   PLUGINS = [
+       'netbox_slm',
+   ]
+   ```
+
+The Netbox installation above will be used to run Django management
+commands like runserver, makemigrations and migrate, which will be
+explained in the next steps below;
+
+   from your projects directory clone the netbox-slm repository
+
+   ```
+   $ git clone https://github.com/ICTU/netbox_slm
+   $ cd netbox_slm
+   $ ./start-netbox.sh
+   ```
+   
+This will start Netbox locally (requires Docker) and forward the redis
+and postgres ports to the localhost (make sure there’s no processes
+using these ports or change the dockerfiles accordingly)
+
+Note, you can also start and stop netbox by hand:
+
+   ```
+   $ cd netbox-docker
+   $ docker-compose up -d
+   ```
+   
+   or stop the stack with
+
+   ```
+   $ docker-compose down
+   ```
+   
+   # to start fresh:
+
+   ```
+   $ docker-compose down
+   $ docker volume rm netbox-docker_netbox-postgres-data  # et cetera
+   $ docker-compose up -d --force-recreate
+   ```
+   
+   this will require you to re-run the migrate commando's for netbox-slm, see further down below
+
+Go back to the netbox configuration.py file and update the postgres and
+redis connection strings (username, password) to the ones the netbox
+docker backend is using, for example (using default user and passwords
+from the netbox docker example):
+
+   ```
+   <<collapsed>>
+
+   # PostgreSQL database configuration. See the Django documentation for a complete list of available parameters:
+   #   https://docs.djangoproject.com/en/stable/ref/settings/#databases
+   DATABASE = {
+       'NAME': 'netbox',               # Database name
+       'USER': 'netbox',               # PostgreSQL username
+       'PASSWORD': 'J5brHrAXFLQSif0K', # PostgreSQL password
+       'HOST': 'localhost',            # Database server
+       'PORT': '',                     # Database port (leave blank for default)
+       'CONN_MAX_AGE': 300,            # Max database connection age
+   }
+
+   # Redis database settings. Redis is used for caching and for queuing background tasks such as webhook events. A separate
+   # configuration exists for each. Full connection details are required in both sections, and it is strongly recommended
+   # to use two separate database IDs.
+   REDIS = {
+       'tasks': {
+           'HOST': 'localhost',
+           'PORT': 6379,
+           # Comment out `HOST` and `PORT` lines and uncomment the following if using Redis Sentinel
+           # 'SENTINELS': [('mysentinel.redis.example.com', 6379)],
+           # 'SENTINEL_SERVICE': 'netbox',
+           'PASSWORD': 'H733Kdjndks81',
+           'DATABASE': 0,
+           'SSL': False,
+           # Set this to True to skip TLS certificate verification
+           # This can expose the connection to attacks, be careful
+           # 'INSECURE_SKIP_TLS_VERIFY': False,
+       },
+       'caching': {
+           'HOST': 'localhost',
+           'PORT': 6379,
+           # Comment out `HOST` and `PORT` lines and uncomment the following if using Redis Sentinel
+           # 'SENTINELS': [('mysentinel.redis.example.com', 6379)],
+           # 'SENTINEL_SERVICE': 'netbox',
+           'PASSWORD': 'H733Kdjndks81',
+           'DATABASE': 1,
+           'SSL': False,
+           # Set this to True to skip TLS certificate verification
+           # This can expose the connection to attacks, be careful
+           # 'INSECURE_SKIP_TLS_VERIFY': False,
+       }
+   }
+
+   <<collapsed>>
+   ```
+   
+Now you can run commands from the netbox repository like this;
+
+   ```
+   $ cd netbox/netbox
+   $ export PYTHONPATH=../../netbox_slm/netbox_slm/  # or with the pipenv activated run `python3 setup.py develop` from the netbox_slm directory
+   $ python3 manage.py migrate netbox_slm
+   $ python3 manage.py runserver 8001
+   ```
+
+Visit http://127.0.0.1:8001 in the browser to see the auto reloading
+version of the netbox UI. Port 8000 is taken by the docker ran variant.
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
                            ****** NetBox SLM ******
     Netbox SLM is a plugin for lifecycle management of software components,
                      including versions and installations.
 [PyPi] [Stars_Badge] [Forks_Badge] [Pull_Requests_Badge] [Issues_Badge] [GitHub
                          contributors] [License_Badge]
-## Known Issues - WARNING: This plugin is only tested with Netbox 3.2 at this
-time. - CSV/Bulk imports for SoftwareProduct, Version and Installation are
-currently broken (WIP) ## Installation Guide When using the Docker version of
-Netbox, first follow the netbox-docker [quickstart](https://github.com/netbox-
-community/netbox-docker#quickstart) instructions to clone the netbox-docker
-repo and set up the ``docker-compose.override.yml``. Next, follow these
-instructions (based on the Netbox docker variant [instructions](https://
+## Known Issues - WARNING: This plugin is only tested with a single Netbox
+version at this time. - CSV/Bulk imports for SoftwareProduct, Version and
+Installation are currently broken (WIP) ## Installation Guide When using the
+Docker version of Netbox, first follow the netbox-docker [quickstart](https://
+github.com/netbox-community/netbox-docker#quickstart) instructions to clone the
+netbox-docker repo and set up the ``docker-compose.override.yml``. Next, follow
+these instructions (based on the Netbox docker variant [instructions](https://
 github.com/netbox-community/netbox-docker/wiki/Configuration#custom-
 configuration-files)) to install the Netbox SLM plugin: 1. Add ``netbox_slm``
 to the ``PLUGINS`` list in ``configuration/extra.py``. 2. Create a
 ``plugin_requirements.txt`` with ``netbox-slm==1.2`` as contents. 3. Create a
-``Dockerfile-SLM`` with contents: ``` FROM netboxcommunity/netbox:v3.2.X COPY
+``Dockerfile-SLM`` with contents: ``` FROM netboxcommunity/netbox:vX.Y.Z COPY
 ./plugin_requirements.txt / RUN /opt/netbox/venv/bin/pip install --no-warn-
 script-location -r /plugin_requirements.txt ``` 4. Create a ``docker-
-compose.override.yml`` with contents: ``` version: '3.4' services: netbox:
+compose.override.yml`` with contents: ``` version: '3.7' services: netbox:
 ports: - 8000:8080 build: context: . dockerfile: Dockerfile-SLM image: netbox:
 slm netbox-worker: image: netbox:slm netbox-housekeeping: image: netbox:slm ```
 Now, build the image: ``docker compose build --no-cache`` And finally, run
 Netbox with the SLM plugin: ``docker compose up`` ## Releasing Guide To draft a
 release; update the setup.py file to reflect the new version, then from the
 *src* directory run ``` # make sure to update the version in netbox_slm/
 __init__.py $ python setup.py sdist $ twine upload dist/* ``` On Github.com
```

