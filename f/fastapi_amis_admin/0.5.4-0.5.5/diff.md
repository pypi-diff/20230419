# Comparing `tmp/fastapi_amis_admin-0.5.4.tar.gz` & `tmp/fastapi_amis_admin-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_amis_admin-0.5.4.tar", last modified: Sun Apr  9 15:26:23 2023, max compression
+gzip compressed data, was "fastapi_amis_admin-0.5.5.tar", last modified: Wed Apr 19 07:00:07 2023, max compression
```

## Comparing `fastapi_amis_admin-0.5.4.tar` & `fastapi_amis_admin-0.5.5.tar`

### file list

```diff
@@ -1,164 +1,163 @@
--rw-r--r--   0        0        0      131 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/.flake8
--rw-r--r--   0        0        0      717 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/.github/dependabot.yml
--rw-r--r--   0        0        0      781 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/.github/workflows/build-docs.yml
--rw-r--r--   0        0        0     1450 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      978 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2111 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/.gitignore
--rw-r--r--   0        0        0      326 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/LICENSE
--rw-r--r--   0        0        0     8705 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/README.md
--rw-r--r--   0        0        0     8597 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/README.zh.md
--rw-r--r--   0        0        0     1509 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/demo/demo-form.py
--rw-r--r--   0        0        0     1179 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/demo/demo-model.py
--rw-r--r--   0        0        0      420 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/demo/demo-simple.py
--rw-r--r--   0        0        0       17 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/CNAME
--rw-r--r--   0        0        0     2245 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/about.md
--rw-r--r--   0        0        0     1702 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/amis/types.md
--rw-r--r--   0        0        0     2631 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/AdminApp.md
--rw-r--r--   0        0        0     1101 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/AdminGroup.md
--rw-r--r--   0        0        0     1100 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/AdminSite.md
--rw-r--r--   0        0        0     2780 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/BaseAdmin.md
--rw-r--r--   0        0        0     1681 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/FormAdmin.md
--rw-r--r--   0        0        0     1473 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/ModelAction.md
--rw-r--r--   0        0        0     7898 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/ModelAdmin.md
--rw-r--r--   0        0        0     1237 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/PageAdmin.md
--rw-r--r--   0        0        0     1280 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/PageSchemaAdmin.md
--rw-r--r--   0        0        0      353 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/RouterAdmin.md
--rw-r--r--   0        0        0     1745 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/Settings.md
--rw-r--r--   0        0        0      732 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/TemplateAdmin.md
--rw-r--r--   0        0        0     3601 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/crud/BaseCrud.md
--rw-r--r--   0        0        0      465 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/crud/RouterMixin.md
--rw-r--r--   0        0        0     2618 2023-04-09 15:26:19.528692 fastapi_amis_admin-0.5.4/docs/en/docs/crud/SQLModelCrud.md
--rw-r--r--   0        0        0       94 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/extended/SQLModel.md
--rw-r--r--   0        0        0      683 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/extended/about.md
--rw-r--r--   0        0        0     1351 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/extended/alembic.md
--rw-r--r--   0        0        0     9217 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/index.md
--rw-r--r--   0        0        0       83 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/js/chat.js
--rw-r--r--   0        0        0    19360 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/js/sidecar-1.5.0.js
--rw-r--r--   0        0        0    29223 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/static/Docs.png
--rw-r--r--   0        0        0    80404 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/static/ModelAdmin.png
--rw-r--r--   0        0        0    21317 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/static/logo.png
--rw-r--r--   0        0        0     3017 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/AdminApp.md
--rw-r--r--   0        0        0       21 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/_more.md
--rw-r--r--   0        0        0      580 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/cli.md
--rw-r--r--   0        0        0     2030 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/debug.md
--rw-r--r--   0        0        0     5125 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/permission.md
--rw-r--r--   0        0        0     2163 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/scheduler.md
--rw-r--r--   0        0        0     1944 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/structure.md
--rw-r--r--   0        0        0     7186 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/user-auth.md
--rw-r--r--   0        0        0     2464 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/FormAdmin.md
--rw-r--r--   0        0        0     3974 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/Inheritance.md
--rw-r--r--   0        0        0     5233 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/ModelAction.md
--rw-r--r--   0        0        0     8076 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/ModelAdmin.md
--rw-r--r--   0        0        0     5341 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/PageAdmin.md
--rw-r--r--   0        0        0     3829 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/Settings.md
--rw-r--r--   0        0        0     1088 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/TemplateAdmin.md
--rw-r--r--   0        0        0       21 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/_more.md
--rw-r--r--   0        0        0     1274 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/i18n.md
--rw-r--r--   0        0        0     1852 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/quickstart.md
--rw-r--r--   0        0        0     2020 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/docs/utils/database.md
--rw-r--r--   0        0        0     3320 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/en/mkdocs.yml
--rw-r--r--   0        0        0       17 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/CNAME
--rw-r--r--   0        0        0     2075 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/about.md
--rw-r--r--   0        0        0     1596 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/amis/types.md
--rw-r--r--   0        0        0     2302 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/AdminApp.md
--rw-r--r--   0        0        0      960 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/AdminGroup.md
--rw-r--r--   0        0        0      932 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/AdminSite.md
--rw-r--r--   0        0        0     2669 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/BaseAdmin.md
--rw-r--r--   0        0        0     1572 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/FormAdmin.md
--rw-r--r--   0        0        0     1473 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/ModelAction.md
--rw-r--r--   0        0        0     7270 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/ModelAdmin.md
--rw-r--r--   0        0        0     1124 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/PageAdmin.md
--rw-r--r--   0        0        0     1163 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/PageSchemaAdmin.md
--rw-r--r--   0        0        0      316 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/RouterAdmin.md
--rw-r--r--   0        0        0     1534 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/Settings.md
--rw-r--r--   0        0        0      670 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/TemplateAdmin.md
--rw-r--r--   0        0        0     3328 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/crud/BaseCrud.md
--rw-r--r--   0        0        0      441 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/crud/RouterMixin.md
--rw-r--r--   0        0        0     2370 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/crud/SQLModelCrud.md
--rw-r--r--   0        0        0       76 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/extended/SQLModel.md
--rw-r--r--   0        0        0      610 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/extended/about.md
--rw-r--r--   0        0        0     1210 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/extended/alembic.md
--rw-r--r--   0        0        0     8443 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/index.md
--rw-r--r--   0        0        0       83 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/js/chat.js
--rw-r--r--   0        0        0    19360 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/js/sidecar-1.5.0.js
--rw-r--r--   0        0        0    29223 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/static/Docs.png
--rw-r--r--   0        0        0    80404 2023-04-09 15:26:19.532692 fastapi_amis_admin-0.5.4/docs/zh/docs/static/ModelAdmin.png
--rw-r--r--   0        0        0    21317 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/static/logo.png
--rw-r--r--   0        0        0     2660 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/AdminApp.md
--rw-r--r--   0        0        0       20 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/_more.md
--rw-r--r--   0        0        0      548 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/cli.md
--rw-r--r--   0        0        0     1805 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/debug.md
--rw-r--r--   0        0        0     4648 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/permission.md
--rw-r--r--   0        0        0     2016 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/scheduler.md
--rw-r--r--   0        0        0     1930 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/structure.md
--rw-r--r--   0        0        0     6532 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/user-auth.md
--rw-r--r--   0        0        0     2194 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/FormAdmin.md
--rw-r--r--   0        0        0     3747 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/Inheritance.md
--rw-r--r--   0        0        0     5233 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/ModelAction.md
--rw-r--r--   0        0        0     9483 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/ModelAdmin.md
--rw-r--r--   0        0        0     4756 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/PageAdmin.md
--rw-r--r--   0        0        0     3325 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/Settings.md
--rw-r--r--   0        0        0     1004 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/TemplateAdmin.md
--rw-r--r--   0        0        0       20 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/_more.md
--rw-r--r--   0        0        0     1137 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/i18n.md
--rw-r--r--   0        0        0     1763 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/quickstart.md
--rw-r--r--   0        0        0     1989 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/docs/utils/database.md
--rw-r--r--   0        0        0     3326 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/docs/zh/mkdocs.yml
--rw-r--r--   0        0        0      577 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/__init__.py
--rw-r--r--   0        0        0      411 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/admin/__init__.py
--rw-r--r--   0        0        0    57478 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/admin/admin.py
--rw-r--r--   0        0        0     3693 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/admin/handlers.py
--rw-r--r--   0        0        0    13103 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/admin/parser.py
--rw-r--r--   0        0        0     1719 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/admin/settings.py
--rw-r--r--   0        0        0     5368 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/admin/site.py
--rw-r--r--   0        0        0     4007 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/amis/README.md
--rw-r--r--   0        0        0      447 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/amis/__init__.py
--rw-r--r--   0        0        0   144473 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/amis/components.py
--rw-r--r--   0        0        0     2266 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/amis/constants.py
--rw-r--r--   0        0        0     6673 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/amis/templates/app.html
--rw-r--r--   0        0        0     1240 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/amis/templates/page.html
--rw-r--r--   0        0        0     4987 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/amis/types.py
--rw-r--r--   0        0        0      256 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/amis/utils.py
--rw-r--r--   0        0        0     1663 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/crud/README.md
--rw-r--r--   0        0        0      200 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/crud/__init__.py
--rw-r--r--   0        0        0    22650 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/crud/_sqlmodel.py
--rw-r--r--   0        0        0     7855 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/crud/base.py
--rw-r--r--   0        0        0     8437 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/crud/parser.py
--rw-r--r--   0        0        0     1878 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/crud/schema.py
--rw-r--r--   0        0        0     3348 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/crud/utils.py
--rw-r--r--   0        0        0     1719 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2551 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1563 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2598 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       73 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/models/__init__.py
--rw-r--r--   0        0        0     2825 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/models/enums.py
--rw-r--r--   0        0        0     2891 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/models/fields.py
--rw-r--r--   0        0        0        0 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/utils/__init__.py
--rw-r--r--   0        0        0     2097 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/utils/functools.py
--rw-r--r--   0        0        0     1848 2023-04-09 15:26:19.536692 fastapi_amis_admin-0.5.4/fastapi_amis_admin/utils/translation.py
--rw-r--r--   0        0        0   152180 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/pdm.lock
--rw-r--r--   0        0        0     2311 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/__init__.py
--rw-r--r--   0        0        0     1357 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/conftest.py
--rw-r--r--   0        0        0     3010 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/models.py
--rw-r--r--   0        0        0      682 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_admin/conftest.py
--rw-r--r--   0        0        0     1256 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_admin/test_AdminApp.py
--rw-r--r--   0        0        0     1989 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_admin/test_AdminGroup.py
--rw-r--r--   0        0        0     2527 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_admin/test_FormAdmin.py
--rw-r--r--   0        0        0     4583 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_admin/test_ModelAdmin.py
--rw-r--r--   0        0        0     4533 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_admin/test_admin.py
--rw-r--r--   0        0        0    11443 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_admin/test_parser.py
--rw-r--r--   0        0        0      879 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_admin/test_settings.py
--rw-r--r--   0        0        0        0 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_amis/__init__.py
--rw-r--r--   0        0        0      591 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_amis/test_amis.py
--rw-r--r--   0        0        0        0 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_crud/__init__.py
--rw-r--r--   0        0        0     2811 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_crud/conftest.py
--rw-r--r--   0        0        0     3152 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_crud/test_Mapper_Events.py
--rw-r--r--   0        0        0    13075 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_crud/test_SQLModelCrud_fields.py
--rw-r--r--   0        0        0     5896 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_crud/test_SQLModelCrud_routes_async.py
--rw-r--r--   0        0        0     5868 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_crud/test_SQLModelCrud_routes_sync.py
--rw-r--r--   0        0        0     7537 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_crud/test_SQLModelCrud_schemas.py
--rw-r--r--   0        0        0     1360 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/test_crud/test_SQLModelSelector.py
--rw-r--r--   0        0        0        0 2023-04-09 15:26:19.540692 fastapi_amis_admin-0.5.4/tests/todo.md
--rw-r--r--   0        0        0    10937 1970-01-01 00:00:00.000000 fastapi_amis_admin-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      717 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      781 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/.github/workflows/build-docs.yml
+-rw-r--r--   0        0        0     1450 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      978 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2111 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/.gitignore
+-rw-r--r--   0        0        0      266 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/LICENSE
+-rw-r--r--   0        0        0     8705 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/README.md
+-rw-r--r--   0        0        0     8597 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/README.zh.md
+-rw-r--r--   0        0        0     1509 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/demo/demo-form.py
+-rw-r--r--   0        0        0     1179 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/demo/demo-model.py
+-rw-r--r--   0        0        0      420 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/demo/demo-simple.py
+-rw-r--r--   0        0        0       17 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/CNAME
+-rw-r--r--   0        0        0     2245 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/about.md
+-rw-r--r--   0        0        0     1702 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/amis/types.md
+-rw-r--r--   0        0        0     2631 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/AdminApp.md
+-rw-r--r--   0        0        0     1101 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/AdminGroup.md
+-rw-r--r--   0        0        0     1100 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/AdminSite.md
+-rw-r--r--   0        0        0     2780 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/BaseAdmin.md
+-rw-r--r--   0        0        0     1681 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/FormAdmin.md
+-rw-r--r--   0        0        0     1473 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/ModelAction.md
+-rw-r--r--   0        0        0     7898 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/ModelAdmin.md
+-rw-r--r--   0        0        0     1237 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/PageAdmin.md
+-rw-r--r--   0        0        0     1280 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/PageSchemaAdmin.md
+-rw-r--r--   0        0        0      353 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/RouterAdmin.md
+-rw-r--r--   0        0        0     1745 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/Settings.md
+-rw-r--r--   0        0        0      732 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/TemplateAdmin.md
+-rw-r--r--   0        0        0     3601 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/crud/BaseCrud.md
+-rw-r--r--   0        0        0      465 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/crud/RouterMixin.md
+-rw-r--r--   0        0        0     2618 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/crud/SQLModelCrud.md
+-rw-r--r--   0        0        0       94 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/extended/SQLModel.md
+-rw-r--r--   0        0        0      683 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/extended/about.md
+-rw-r--r--   0        0        0     1351 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/extended/alembic.md
+-rw-r--r--   0        0        0     9217 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/index.md
+-rw-r--r--   0        0        0       83 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/js/chat.js
+-rw-r--r--   0        0        0    19360 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/js/sidecar-1.5.0.js
+-rw-r--r--   0        0        0    29223 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/static/Docs.png
+-rw-r--r--   0        0        0    80404 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/static/ModelAdmin.png
+-rw-r--r--   0        0        0    21317 2023-04-19 07:00:03.450487 fastapi_amis_admin-0.5.5/docs/en/docs/static/logo.png
+-rw-r--r--   0        0        0     3017 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/AdminApp.md
+-rw-r--r--   0        0        0       21 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/_more.md
+-rw-r--r--   0        0        0      580 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/cli.md
+-rw-r--r--   0        0        0     2030 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/debug.md
+-rw-r--r--   0        0        0     5125 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/permission.md
+-rw-r--r--   0        0        0     2163 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/scheduler.md
+-rw-r--r--   0        0        0     1944 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/structure.md
+-rw-r--r--   0        0        0     7186 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/user-auth.md
+-rw-r--r--   0        0        0     2464 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/FormAdmin.md
+-rw-r--r--   0        0        0     3974 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/Inheritance.md
+-rw-r--r--   0        0        0     5233 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/ModelAction.md
+-rw-r--r--   0        0        0     8076 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/ModelAdmin.md
+-rw-r--r--   0        0        0     5341 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/PageAdmin.md
+-rw-r--r--   0        0        0     3829 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/Settings.md
+-rw-r--r--   0        0        0     1088 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/TemplateAdmin.md
+-rw-r--r--   0        0        0       21 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/_more.md
+-rw-r--r--   0        0        0     1274 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/i18n.md
+-rw-r--r--   0        0        0     1852 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/quickstart.md
+-rw-r--r--   0        0        0     2020 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/docs/utils/database.md
+-rw-r--r--   0        0        0     3320 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/en/mkdocs.yml
+-rw-r--r--   0        0        0       17 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/CNAME
+-rw-r--r--   0        0        0     2075 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/about.md
+-rw-r--r--   0        0        0     1596 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/amis/types.md
+-rw-r--r--   0        0        0     2302 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/AdminApp.md
+-rw-r--r--   0        0        0      960 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/AdminGroup.md
+-rw-r--r--   0        0        0      932 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/AdminSite.md
+-rw-r--r--   0        0        0     2669 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/BaseAdmin.md
+-rw-r--r--   0        0        0     1572 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/FormAdmin.md
+-rw-r--r--   0        0        0     1473 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/ModelAction.md
+-rw-r--r--   0        0        0     7270 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/ModelAdmin.md
+-rw-r--r--   0        0        0     1124 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/PageAdmin.md
+-rw-r--r--   0        0        0     1163 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/PageSchemaAdmin.md
+-rw-r--r--   0        0        0      316 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/RouterAdmin.md
+-rw-r--r--   0        0        0     1534 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/Settings.md
+-rw-r--r--   0        0        0      670 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/TemplateAdmin.md
+-rw-r--r--   0        0        0     3328 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/crud/BaseCrud.md
+-rw-r--r--   0        0        0      441 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/crud/RouterMixin.md
+-rw-r--r--   0        0        0     2370 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/crud/SQLModelCrud.md
+-rw-r--r--   0        0        0       76 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/extended/SQLModel.md
+-rw-r--r--   0        0        0      610 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/extended/about.md
+-rw-r--r--   0        0        0     1210 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/extended/alembic.md
+-rw-r--r--   0        0        0     8443 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/index.md
+-rw-r--r--   0        0        0       83 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/js/chat.js
+-rw-r--r--   0        0        0    19360 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/js/sidecar-1.5.0.js
+-rw-r--r--   0        0        0    29223 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/static/Docs.png
+-rw-r--r--   0        0        0    80404 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/static/ModelAdmin.png
+-rw-r--r--   0        0        0    21317 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/static/logo.png
+-rw-r--r--   0        0        0     2660 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/AdminApp.md
+-rw-r--r--   0        0        0       20 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/_more.md
+-rw-r--r--   0        0        0      548 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/cli.md
+-rw-r--r--   0        0        0     1805 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/debug.md
+-rw-r--r--   0        0        0     4648 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/permission.md
+-rw-r--r--   0        0        0     2016 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/scheduler.md
+-rw-r--r--   0        0        0     1930 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/structure.md
+-rw-r--r--   0        0        0     6532 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/user-auth.md
+-rw-r--r--   0        0        0     2194 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/FormAdmin.md
+-rw-r--r--   0        0        0     3747 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/Inheritance.md
+-rw-r--r--   0        0        0     5233 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/ModelAction.md
+-rw-r--r--   0        0        0     9483 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/ModelAdmin.md
+-rw-r--r--   0        0        0     4756 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/PageAdmin.md
+-rw-r--r--   0        0        0     3325 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/Settings.md
+-rw-r--r--   0        0        0     1004 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/TemplateAdmin.md
+-rw-r--r--   0        0        0       20 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/_more.md
+-rw-r--r--   0        0        0     1137 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/i18n.md
+-rw-r--r--   0        0        0     1763 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/quickstart.md
+-rw-r--r--   0        0        0     1989 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/docs/utils/database.md
+-rw-r--r--   0        0        0     3326 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/docs/zh/mkdocs.yml
+-rw-r--r--   0        0        0      577 2023-04-19 07:00:03.454487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/__init__.py
+-rw-r--r--   0        0        0      411 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/admin/__init__.py
+-rw-r--r--   0        0        0    57295 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/admin/admin.py
+-rw-r--r--   0        0        0     3717 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/admin/handlers.py
+-rw-r--r--   0        0        0    13214 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/admin/parser.py
+-rw-r--r--   0        0        0     1719 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/admin/settings.py
+-rw-r--r--   0        0        0     5368 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/admin/site.py
+-rw-r--r--   0        0        0     4007 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/amis/README.md
+-rw-r--r--   0        0        0      466 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/amis/__init__.py
+-rw-r--r--   0        0        0   145260 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/amis/components.py
+-rw-r--r--   0        0        0     2353 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/amis/constants.py
+-rw-r--r--   0        0        0     6673 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/amis/templates/app.html
+-rw-r--r--   0        0        0     1240 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/amis/templates/page.html
+-rw-r--r--   0        0        0     4987 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/amis/types.py
+-rw-r--r--   0        0        0      256 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/amis/utils.py
+-rw-r--r--   0        0        0     1663 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/crud/README.md
+-rw-r--r--   0        0        0      200 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/crud/__init__.py
+-rw-r--r--   0        0        0    22650 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/crud/_sqlmodel.py
+-rw-r--r--   0        0        0     7855 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/crud/base.py
+-rw-r--r--   0        0        0     8545 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/crud/parser.py
+-rw-r--r--   0        0        0     1878 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/crud/schema.py
+-rw-r--r--   0        0        0     3348 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/crud/utils.py
+-rw-r--r--   0        0        0     1719 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2551 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1563 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2598 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       73 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/models/__init__.py
+-rw-r--r--   0        0        0     2825 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/models/enums.py
+-rw-r--r--   0        0        0     2891 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/models/fields.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/utils/__init__.py
+-rw-r--r--   0        0        0     2097 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/utils/functools.py
+-rw-r--r--   0        0        0     1848 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/fastapi_amis_admin/utils/translation.py
+-rw-r--r--   0        0        0   152180 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/pdm.lock
+-rw-r--r--   0        0        0     2652 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/__init__.py
+-rw-r--r--   0        0        0     1357 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/conftest.py
+-rw-r--r--   0        0        0     3010 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/models.py
+-rw-r--r--   0        0        0      682 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_admin/conftest.py
+-rw-r--r--   0        0        0     1256 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_admin/test_AdminApp.py
+-rw-r--r--   0        0        0     1989 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_admin/test_AdminGroup.py
+-rw-r--r--   0        0        0     2527 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_admin/test_FormAdmin.py
+-rw-r--r--   0        0        0     4583 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_admin/test_ModelAdmin.py
+-rw-r--r--   0        0        0     4533 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_admin/test_admin.py
+-rw-r--r--   0        0        0    11490 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_admin/test_parser.py
+-rw-r--r--   0        0        0      879 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_admin/test_settings.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_amis/__init__.py
+-rw-r--r--   0        0        0      591 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_amis/test_amis.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_crud/__init__.py
+-rw-r--r--   0        0        0     2894 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_crud/conftest.py
+-rw-r--r--   0        0        0     3152 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_crud/test_Mapper_Events.py
+-rw-r--r--   0        0        0    13075 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_crud/test_SQLModelCrud_fields.py
+-rw-r--r--   0        0        0     6008 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_crud/test_SQLModelCrud_routes_async.py
+-rw-r--r--   0        0        0     5868 2023-04-19 07:00:03.458487 fastapi_amis_admin-0.5.5/tests/test_crud/test_SQLModelCrud_routes_sync.py
+-rw-r--r--   0        0        0     7546 2023-04-19 07:00:03.462487 fastapi_amis_admin-0.5.5/tests/test_crud/test_SQLModelCrud_schemas.py
+-rw-r--r--   0        0        0     1360 2023-04-19 07:00:03.462487 fastapi_amis_admin-0.5.5/tests/test_crud/test_SQLModelSelector.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:00:03.462487 fastapi_amis_admin-0.5.5/tests/todo.md
+-rw-r--r--   0        0        0    10983 1970-01-01 00:00:00.000000 fastapi_amis_admin-0.5.5/PKG-INFO
```

### Comparing `fastapi_amis_admin-0.5.4/.github/dependabot.yml` & `fastapi_amis_admin-0.5.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/.github/workflows/build-docs.yml` & `fastapi_amis_admin-0.5.5/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/.github/workflows/pytest.yml` & `fastapi_amis_admin-0.5.5/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/.github/workflows/python-publish.yml` & `fastapi_amis_admin-0.5.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/.gitignore` & `fastapi_amis_admin-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/LICENSE` & `fastapi_amis_admin-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/README.md` & `fastapi_amis_admin-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/README.zh.md` & `fastapi_amis_admin-0.5.5/README.zh.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/demo/demo-form.py` & `fastapi_amis_admin-0.5.5/demo/demo-form.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/demo/demo-model.py` & `fastapi_amis_admin-0.5.5/demo/demo-model.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/about.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/about.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/amis/types.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/amis/types.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/AdminApp.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/AdminApp.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/AdminGroup.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/AdminGroup.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/AdminSite.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/AdminSite.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/BaseAdmin.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/BaseAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/FormAdmin.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/FormAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/ModelAction.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/ModelAction.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/ModelAdmin.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/ModelAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/PageAdmin.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/PageAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/PageSchemaAdmin.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/PageSchemaAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/Settings.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/Settings.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/amis_admin/TemplateAdmin.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/amis_admin/TemplateAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/crud/BaseCrud.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/crud/BaseCrud.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/crud/SQLModelCrud.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/crud/SQLModelCrud.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/extended/about.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/extended/about.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/extended/alembic.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/extended/alembic.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/index.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/js/sidecar-1.5.0.js` & `fastapi_amis_admin-0.5.5/docs/en/docs/js/sidecar-1.5.0.js`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/static/Docs.png` & `fastapi_amis_admin-0.5.5/docs/en/docs/static/Docs.png`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/static/ModelAdmin.png` & `fastapi_amis_admin-0.5.5/docs/en/docs/static/ModelAdmin.png`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/static/logo.png` & `fastapi_amis_admin-0.5.5/docs/en/docs/static/logo.png`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/AdminApp.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/AdminApp.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/cli.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/cli.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/debug.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/debug.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/permission.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/permission.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/scheduler.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/scheduler.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/structure.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/structure.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/advanced/user-auth.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/advanced/user-auth.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/FormAdmin.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/FormAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/Inheritance.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/Inheritance.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/ModelAction.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/ModelAction.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/ModelAdmin.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/ModelAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/PageAdmin.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/PageAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/Settings.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/Settings.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/TemplateAdmin.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/TemplateAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/basic/i18n.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/basic/i18n.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/tutorials/quickstart.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/tutorials/quickstart.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/docs/utils/database.md` & `fastapi_amis_admin-0.5.5/docs/en/docs/utils/database.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/en/mkdocs.yml` & `fastapi_amis_admin-0.5.5/docs/en/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/about.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/about.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/amis/types.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/amis/types.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/AdminApp.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/AdminApp.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/AdminGroup.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/AdminGroup.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/AdminSite.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/AdminSite.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/BaseAdmin.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/BaseAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/FormAdmin.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/FormAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/ModelAction.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/ModelAction.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/ModelAdmin.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/ModelAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/PageAdmin.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/PageAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/PageSchemaAdmin.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/PageSchemaAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/Settings.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/Settings.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/amis_admin/TemplateAdmin.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/amis_admin/TemplateAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/crud/BaseCrud.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/crud/BaseCrud.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/crud/SQLModelCrud.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/crud/SQLModelCrud.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/extended/about.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/extended/about.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/extended/alembic.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/extended/alembic.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/index.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/js/sidecar-1.5.0.js` & `fastapi_amis_admin-0.5.5/docs/zh/docs/js/sidecar-1.5.0.js`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/static/Docs.png` & `fastapi_amis_admin-0.5.5/docs/zh/docs/static/Docs.png`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/static/ModelAdmin.png` & `fastapi_amis_admin-0.5.5/docs/zh/docs/static/ModelAdmin.png`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/static/logo.png` & `fastapi_amis_admin-0.5.5/docs/zh/docs/static/logo.png`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/AdminApp.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/AdminApp.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/cli.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/cli.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/debug.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/debug.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/permission.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/permission.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/scheduler.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/scheduler.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/structure.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/structure.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/advanced/user-auth.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/advanced/user-auth.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/FormAdmin.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/FormAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/Inheritance.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/Inheritance.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/ModelAction.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/ModelAction.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/ModelAdmin.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/ModelAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/PageAdmin.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/PageAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/Settings.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/Settings.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/TemplateAdmin.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/TemplateAdmin.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/basic/i18n.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/basic/i18n.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/tutorials/quickstart.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/tutorials/quickstart.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/docs/utils/database.md` & `fastapi_amis_admin-0.5.5/docs/zh/docs/utils/database.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/docs/zh/mkdocs.yml` & `fastapi_amis_admin-0.5.5/docs/zh/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/__init__.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.4"
+__version__ = "0.5.5"
 __url__ = "https://github.com/amisadmin/fastapi_amis_admin"
 
 import gettext
 import os
 
 from .utils.translation import i18n
```

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/admin/admin.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/admin/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,20 +54,15 @@
     Picker,
     Remark,
     Service,
     TableColumn,
     TableCRUD,
     Tpl,
 )
-from fastapi_amis_admin.amis.constants import (
-    DisplayModeEnum,
-    LevelEnum,
-    SizeEnum,
-    TabsModeEnum,
-)
+from fastapi_amis_admin.amis.constants import DisplayModeEnum, LevelEnum, SizeEnum
 from fastapi_amis_admin.amis.types import (
     AmisAPI,
     AmisNode,
     BaseAmisApiOut,
     BaseAmisModel,
     SchemaNode,
 )
@@ -279,15 +274,15 @@
             )
         return Service(
             schemaApi=AmisAPI(
                 method="post",
                 url=url,
                 data={},
                 cache=300000,
-                responseData=dict(controls=[picker]),
+                responseData={"controls": [picker]},
                 qsOptions={"id": f"${self.pk_admin.pk_name}"},
                 adaptor=adaptor,
             )
         )
 
     def register_router(self):
         self.pk_admin.router.add_api_route(
@@ -699,36 +694,36 @@
                 modelfields = [self.parser.get_modelfield(ins) for ins in ins_list]
                 columns.extend([await self.get_list_column(request, modelfield) for modelfield in modelfields])
             else:
                 modelfield = self.parser.get_modelfield(field)
                 if modelfield:
                     columns.append(await self.get_list_column(request, modelfield))
         # Append operation column
-        actions = await self.get_actions(request, flag="column")
-        if actions:
+        actions = await self.get_actions(request, flag="column") or []
+        for action in actions:
             columns.append(
                 ColumnOperation(
-                    width=160,
-                    label=_("Operation"),
+                    label=getattr(action, "label", _("Operation")),
                     breakpoint="*",
-                    buttons=actions,
+                    buttons=[action],
                 )
             )
         # Append inline link model column
         for link_form in self.link_model_forms:
             form = await link_form.get_form_item(request)
-            if form:
-                columns.append(
-                    ColumnOperation(
-                        width=160,
-                        label=link_form.display_admin.page_schema.label,
-                        breakpoint="*",
-                        buttons=[form],
-                    )
+            if not form:
+                continue
+            columns.append(
+                ColumnOperation(
+                    width=160,
+                    label=link_form.display_admin.page_schema.label,
+                    breakpoint="*",
+                    buttons=[form],
                 )
+            )
         return columns
 
     async def get_list_table_api(self, request: Request) -> AmisAPI:
         data = {"&": "$$"}
         for field in self.search_fields:
             alias = self.parser.get_alias(field)
             if alias:
@@ -822,15 +817,15 @@
         return Service(
             name=modelfield.alias,
             schemaApi=AmisAPI(
                 method="post",
                 url=url,
                 data={},
                 cache=300000,
-                responseData=dict(controls=[picker]),
+                responseData={"controls": [picker]},
             ),
         )
 
     async def get_form_item(
         self, request: Request, modelfield: ModelField, action: CrudEnum
     ) -> Union[FormItem, SchemaNode, None]:
         is_filter = action == CrudEnum.list
@@ -1289,15 +1284,14 @@
 
 
 class AdminApp(PageAdmin, AdminGroup):
     """Manage applications"""
 
     engine: SqlalchemyDatabase = None
     page_path = "/"
-    tabs_mode: TabsModeEnum = None  # Deprecated. Use the tabsMode attribute in the page_schema.
 
     def __init__(self, app: "AdminApp"):
         PageAdmin.__init__(self, app)
         AdminGroup.__init__(self, app)
         self.engine = self.engine or self.app.engine
         self.db = get_engine_db(self.engine)
         self._registered: Dict[Type[BaseAdminT], Optional[BaseAdminT]] = {}
@@ -1357,15 +1351,14 @@
         return admin_cls[0]
 
     def unregister_admin(self, *admin_cls: Type[BaseAdmin]):
         [self._registered.pop(cls) for cls in admin_cls if cls]
 
     def get_page_schema(self) -> Optional[PageSchema]:
         if super().get_page_schema():
-            self.page_schema.tabsMode = self.tabs_mode
             if self.page_schema.tabsMode is None:
                 self.page_schema.schemaApi = None
         return self.page_schema
 
     async def get_page(self, request: Request) -> Union[Page, App]:
         if self.page_schema.tabsMode is None:
             return await self._get_page_as_app(request)
@@ -1394,15 +1387,15 @@
         children = await self.get_page_schema_children(request)
         app.pages = [{"children": children}] if children else []
         return app
 
     async def _get_page_as_tabs(self, request: Request) -> Page:
         page = await super(AdminApp, self).get_page(request)
         children = await self.get_page_schema_children(request)
-        page.body = PageSchema(children=children, tabsMode=self.page_schema.tabsMode).as_tabs_item().tab
+        page.body = PageSchema(children=children, tabsMode=self.page_schema.tabsMode).as_page_body()
         return page
 
 
 class BaseAdminSite(AdminApp):
     def __init__(
         self,
         settings: Settings,
```

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/admin/handlers.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/admin/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,16 +78,16 @@
 
 
 async def http_exception_handler(request: Request, exc: HTTPException):
     """http exception"""
     headers = getattr(exc, "headers", None)
     if not is_body_allowed_for_status_code(exc.status_code):
         return Response(status_code=exc.status_code, headers=headers)
-    result = BaseApiOut(status=exc.status_code, msg=exc.detail).dict()
-    return JSONResponse(result, status_code=exc.status_code, headers=headers)
+    content = getattr(exc, "content", {"status": exc.status_code, "msg": exc.detail})
+    return JSONResponse(content=content, status_code=exc.status_code, headers=headers)
 
 
 async def request_validation_exception_handler(request: Request, exc: RequestValidationError):
     """Request parameter validation exception"""
     return make_error_response(
         status=HTTP_422_UNPROCESSABLE_ENTITY,
         body=exc.body,
```

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/admin/parser.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/admin/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,19 @@
             self.as_form_item(modelfield, set_default=set_default, is_filter=is_filter)
             for modelfield in model.__fields__.values()
         ]
         # InputSubForm
         return form
 
     def update_common_attrs(
-        self, modelfield: ModelField, item: Union[FormItem, TableColumn], set_default: bool = False, is_filter: bool = False
+        self,
+        modelfield: ModelField,
+        item: Union[FormItem, TableColumn],
+        set_default: bool = False,
+        is_filter: bool = False,
     ):
         """Set common attributes for FormItem and TableColumn."""
         if not is_filter:
             if modelfield.field_info.max_length:
                 item.maxLength = modelfield.field_info.max_length
             if modelfield.field_info.min_length:
                 item.minLength = modelfield.field_info.min_length
@@ -191,34 +195,38 @@
         elif issubclass(type_, datetime.time):
             kwargs["type"] = "time"
         elif issubclass(type_, Enum):
             items = type_.choices if issubclass(type_, Choices) else [(m.value, m.value) for m in type_]
             kwargs["type"] = "mapping"
             kwargs["filterable"] = {"options": [{"label": v, "value": k} for k, v in items]}
             kwargs["map"] = {
-                k: f"<span class='label label-{l.value}'>{v}</span>" for (k, v), l in zip(items, cyclic_generator(LabelEnum))
+                k: f"<span class='label label-{label.value}'>{v}</span>"
+                for (k, v), label in zip(items, cyclic_generator(LabelEnum))
             }
         elif issubclass(type_, (dict, Json)):
             kwargs["type"] = "json"
         elif issubclass(type_, (list, set)):
             kwargs["type"] = "each"
-            kwargs["items"] = {"type": "tpl", "tpl": "<span class='label label-info m-l-sm'><%= this.item %></span>"}
+            kwargs["items"] = {
+                "type": "tpl",
+                "tpl": "<span class='label label-info m-l-sm'><%= this.item %></span>",
+            }
         return kwargs
 
     def get_field_amis_form_item_type(self, type_: Any, is_filter: bool, required: bool = False) -> dict:
         """Get amis form item type from pydantic model field type."""
         kwargs = {}
         if type_ in {str, Any}:
             kwargs["type"] = "input-text"
         elif issubclass(type_, Enum):
             items = type_.choices if issubclass(type_, Choices) else [(m.value, m.value) for m in type_]
             kwargs.update(
                 {
                     "type": "select",
-                    "options": [{"label": l, "value": v} for v, l in items],
+                    "options": [{"label": label, "value": v} for v, label in items],
                     "extractValue": True,
                     "joinValues": False,
                 }
             )
             if not required or is_filter:
                 kwargs["clearable"] = True
         elif issubclass(type_, bool):
@@ -279,15 +287,15 @@
             return {}
         if callable(extra):
             return extra()
         extra = smart_deepcopy(extra)
         if isinstance(extra, (AmisNode, dict)):
             pass
         elif isinstance(extra, str):
-            extra = dict(type=extra)
+            extra = {"type": extra}
         else:
             extra = {}
         return extra
 
 
 def cyclic_generator(iterable: Iterable[_T]) -> Generator[_T, None, None]:
     while True:
```

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/admin/settings.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/admin/settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/admin/site.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/admin/site.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/amis/README.md` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/amis/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/amis/components.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/amis/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,39 +388,54 @@
     # because only the first one will be useful.
     visible: Union[str, bool] = None  # Some pages may not want to appear in the menu, you can configure it to false, and the
     # route with parameters does not need to be configured, it is directly invisible.
     className: str = None  # Menu class name.
     children: List["PageSchema"] = None  # Submenu
     sort: int = None  # Unofficial attribute. sort
     tabsMode: TabsModeEnum = None  # Unofficial attribute. Display mode, the value can be line, card, radio, vertical,
+    # chrome, simple, strong, tiled, sidebar, collapse
 
-    # chrome, simple, strong, tiled, sidebar
-
-    def as_tabs_item(self, tabs_extra: Dict[str, Any] = None, item_extra: Dict[str, Any] = None):
+    def as_page_body(self, group_extra: Dict[str, Any] = None, item_extra: Dict[str, Any] = None):
         if self.children:
-            tab = Tabs(
-                tabsMode=self.tabsMode,
-                mountOnEnter=True,
-                tabs=[item.as_tabs_item(tabs_extra, item_extra) for item in self.children],
-            ).update_from_dict(tabs_extra or {})
+            if self.tabsMode is None:
+                body = App(pages=[PageSchema(children=self.children)])
+            elif self.tabsMode == TabsModeEnum.collapse:
+                body = CollapseGroup(
+                    body=[
+                        CollapseGroup.CollapseItem(
+                            header=item.label,
+                            body=item.as_page_body(group_extra, item_extra),
+                        ).update_from_dict(item_extra or {})
+                        for item in self.children
+                    ],
+                ).update_from_dict(group_extra or {})
+            else:
+                body = Tabs(
+                    tabsMode=self.tabsMode,
+                    mountOnEnter=True,
+                    tabs=[
+                        Tabs.Item(
+                            title=item.label,
+                            icon=item.icon,
+                            tab=item.as_page_body(group_extra, item_extra),
+                        ).update_from_dict(item_extra or {})
+                        for item in self.children
+                    ],
+                ).update_from_dict(group_extra or {})
         elif self.schema_:
-            tab = self.schema_
-            if isinstance(tab, Iframe):
-                tab.height = 1080
+            body = self.schema_
+            if isinstance(body, Iframe):
+                body.height = 1080
         elif self.schemaApi:
-            tab = Service(schemaApi=self.schemaApi)
+            body = Service(schemaApi=self.schemaApi)
         elif self.link:
-            tab = Page(body=Link(href=self.link, body=self.label, blank=True))
+            body = Page(body=Link(href=self.link, body=self.label, blank=True))
         else:
-            tab = None
-        return Tabs.Item(
-            title=self.label,
-            icon=self.icon,
-            tab=tab,
-        ).update_from_dict(item_extra or {})
+            body = None
+        return body
 
 
 class App(Page):
     """Multi-page application"""
 
     __default_template_path__: str = f"{BASE_DIR}/templates/app.html"
     type: str = "app"
```

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/amis/constants.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/amis/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,7 +120,8 @@
     radio = "radio"
     vertical = "vertical"
     chrome = "chrome"
     simple = "simple"
     strong = "strong"
     tiled = "tiled"
     sidebar = "sidebar"
+    collapse = "collapse"  # collapse 容器, 用于将多个页面展示为折叠器.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/amis/templates/app.html` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/amis/templates/app.html`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/amis/templates/page.html` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/amis/templates/page.html`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/amis/types.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/amis/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/crud/README.md` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/crud/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/crud/_sqlmodel.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/crud/_sqlmodel.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/crud/base.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/crud/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/crud/parser.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/crud/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -178,15 +178,20 @@
 def _get_label_modelfield(label: Label) -> ModelField:
     modelfield = getattr(label, "__ModelField__", None)
     if modelfield is None:
         try:
             python_type = label.expression.type.python_type
         except NotImplementedError:
             python_type = str
-        modelfield = ModelField(name=label.key, type_=python_type, class_validators={}, model_config=BaseConfig)
+        modelfield = ModelField(
+            name=label.key,
+            type_=python_type,
+            class_validators={},
+            model_config=BaseConfig,
+        )
         label.__ModelField__ = modelfield
     return modelfield
 
 
 def LabelField(label: Label, field: FieldInfo) -> Label:
     """Use for adding FieldInfo to sqlalchemy Label type"""
     modelfield = _get_label_modelfield(label)
@@ -196,12 +201,18 @@
     return label
 
 
 class PropertyField(ModelField):
     """Use this to quickly initialize a ModelField, mainly used in schema_read and schema_update"""
 
     def __init__(
-        self, *, name: str, type_: Type[Any], required: bool = False, field_info: Optional[FieldInfo] = None, **kwargs: Any
+        self,
+        *,
+        name: str,
+        type_: Type[Any],
+        required: bool = False,
+        field_info: Optional[FieldInfo] = None,
+        **kwargs: Any,
     ) -> None:
         kwargs.setdefault("class_validators", {})
         kwargs.setdefault("model_config", BaseConfig)
         super().__init__(name=name, type_=type_, required=required, field_info=field_info, **kwargs)
```

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/crud/schema.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/crud/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/crud/utils.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/crud/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/models/enums.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/models/enums.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/models/fields.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/models/fields.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/utils/functools.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/utils/functools.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/fastapi_amis_admin/utils/translation.py` & `fastapi_amis_admin-0.5.5/fastapi_amis_admin/utils/translation.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/pdm.lock` & `fastapi_amis_admin-0.5.5/pdm.lock`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/pyproject.toml` & `fastapi_amis_admin-0.5.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     "jinja2 >=2.11.2,<4.0.0",
     "ujson>=4.0.1",
     "requests>=2.28.1",
 ]
 dev = [
     "fastapi-amis-admin[test]",
     "pre-commit>=2.20.0",
+    "ruff>=0.0.261",
 ]
 cli = [
     "fastapi-amis-admin-cli>=0.1.0,<0.2.0",
 ]
 all = [
     "fastapi-amis-admin[dev]",
 ]
@@ -79,21 +80,35 @@
 minversion = "6.0"
 testpaths = [
     "tests",
 ]
 # pytest-asyncio
 asyncio_mode = "auto"
 
-[tool.isort]
-profile = "black"
-atomic = true
-filter_files = true
-
 [tool.black]
 line-length = 130
 include = '\.pyi?$'
 
+[tool.ruff]
+select = [
+    "E",  # pycodestyle errors
+    "W",  # pycodestyle warnings
+    "F",  # pyflakes
+    "I",  # isort
+    "C",  # flake8-comprehensions
+    "B",  # flake8-bugbear
+]
+ignore = [
+    "B008",  # do not perform function calls in argument defaults
+    "C901",  # too complex
+]
+# Same as Black.
+line-length = 130
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]
+
 [tool.pdm]
 [tool.pdm.dev-dependencies]
 [tool.pdm.scripts]
 lint = "pre-commit run --all-files"
 test= "pytest"
```

### Comparing `fastapi_amis_admin-0.5.4/tests/conftest.py` & `fastapi_amis_admin-0.5.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/tests/models.py` & `fastapi_amis_admin-0.5.5/tests/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/tests/test_admin/conftest.py` & `fastapi_amis_admin-0.5.5/tests/test_admin/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/tests/test_admin/test_AdminApp.py` & `fastapi_amis_admin-0.5.5/tests/test_admin/test_AdminApp.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/tests/test_admin/test_AdminGroup.py` & `fastapi_amis_admin-0.5.5/tests/test_admin/test_AdminGroup.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/tests/test_admin/test_FormAdmin.py` & `fastapi_amis_admin-0.5.5/tests/test_admin/test_FormAdmin.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/tests/test_admin/test_ModelAdmin.py` & `fastapi_amis_admin-0.5.5/tests/test_admin/test_ModelAdmin.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/tests/test_admin/test_admin.py` & `fastapi_amis_admin-0.5.5/tests/test_admin/test_admin.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/tests/test_admin/test_parser.py` & `fastapi_amis_admin-0.5.5/tests/test_admin/test_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,19 @@
     assert column.type == "datetime"
     assert column.label == "创建时间"
 
 
 def test_field_list():
     class User(BaseModel):
         tags: List[str] = Field([], title="标签")
-        email: List[str] = Field([], title="邮箱列表", amis_form_item=amis.InputArray(items=amis.InputText(type="input-email")))
+        email: List[str] = Field(
+            [],
+            title="邮箱列表",
+            amis_form_item=amis.InputArray(items=amis.InputText(type="input-email")),
+        )
         names: list = Field([], title="姓名列表")
 
     # test tags
     modelfield = User.__fields__["tags"]
     assert modelfield.type_ == str
     assert get_origin(modelfield.outer_type_) is list
     # formitem
```

### Comparing `fastapi_amis_admin-0.5.4/tests/test_admin/test_settings.py` & `fastapi_amis_admin-0.5.5/tests/test_admin/test_settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/tests/test_amis/test_amis.py` & `fastapi_amis_admin-0.5.5/tests/test_amis/test_amis.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/tests/test_crud/conftest.py` & `fastapi_amis_admin-0.5.5/tests/test_crud/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,22 @@
     await async_session.commit()
     return data
 
 
 @pytest.fixture
 async def fake_articles(async_session, fake_users, fake_categorys, fake_article_contents) -> List[Article]:
     data = [
-        Article(id=i, title=f"Article_{i}", description=f"Description_{i}", user_id=i, category_id=i, content_id=i)
+        Article(
+            id=i,
+            title=f"Article_{i}",
+            description=f"Description_{i}",
+            user_id=i,
+            category_id=i,
+            content_id=i,
+        )
         for i in range(1, 6)
     ]
     async_session.add_all(data)
     await async_session.commit()
     return data
```

### Comparing `fastapi_amis_admin-0.5.4/tests/test_crud/test_Mapper_Events.py` & `fastapi_amis_admin-0.5.5/tests/test_crud/test_Mapper_Events.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/tests/test_crud/test_SQLModelCrud_fields.py` & `fastapi_amis_admin-0.5.5/tests/test_crud/test_SQLModelCrud_fields.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/tests/test_crud/test_SQLModelCrud_routes_async.py` & `fastapi_amis_admin-0.5.5/tests/test_crud/test_SQLModelCrud_routes_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,25 +92,35 @@
     assert users[0]["address"] == ["address_1", "address_2"]
     assert users[2]["address"] == ["address_1", "address_2"]
 
 
 async def test_route_update(async_client: AsyncClient, fake_users):
     # update one
     res = await async_client.put(
-        "/User/item/1", json={"username": "new_name", "address": ["address_3"], "attach": {"attach_3": "attach_3"}}
+        "/User/item/1",
+        json={
+            "username": "new_name",
+            "address": ["address_3"],
+            "attach": {"attach_3": "attach_3"},
+        },
     )
     count = res.json()["data"]
     assert count == 1
     user = await db.session.get(User, 1)
     assert user.username == "new_name"
     assert user.address == ["address_3"]
     assert user.attach == {"attach_3": "attach_3"}
     # update bulk
     res = await async_client.put(
-        "/User/item/1,2,4", json={"password": "new_password", "address": ["address_3"], "attach": {"attach_3": "attach_3"}}
+        "/User/item/1,2,4",
+        json={
+            "password": "new_password",
+            "address": ["address_3"],
+            "attach": {"attach_3": "attach_3"},
+        },
     )
     count = res.json()["data"]
     assert count == 3
     db.session.expire_all()
     for user in await db.session.scalars(select(User).where(User.id.in_([1, 2, 4]))):
         assert user.password == "new_password"
         assert user.address == ["address_3"]
```

### Comparing `fastapi_amis_admin-0.5.4/tests/test_crud/test_SQLModelCrud_routes_sync.py` & `fastapi_amis_admin-0.5.5/tests/test_crud/test_SQLModelCrud_routes_sync.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/tests/test_crud/test_SQLModelCrud_schemas.py` & `fastapi_amis_admin-0.5.5/tests/test_crud/test_SQLModelCrud_schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,12 +217,13 @@
     # test api
     res = await async_client.put("/article/item/1", json={"title": "new_title"})
     assert res.json()["data"] == 1
     article = await async_session.get(Article, 1, with_for_update=True)
     assert article.title == "new_title"
 
     res = await async_client.put(
-        "/article/item/1", json={"content": {"id": 2, "content": "new_content"}}  # will be ignored by `update_exclude`
+        "/article/item/1",
+        json={"content": {"id": 2, "content": "new_content"}},  # will be ignored by `update_exclude`
     )
     assert res.json()["data"] == 1
     content = await async_session.get(ArticleContent, 1, with_for_update=True)
     assert content.content == "new_content"
```

### Comparing `fastapi_amis_admin-0.5.4/tests/test_crud/test_SQLModelSelector.py` & `fastapi_amis_admin-0.5.5/tests/test_crud/test_SQLModelSelector.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.4/PKG-INFO` & `fastapi_amis_admin-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_amis_admin
-Version: 0.5.4
+Version: 0.5.5
 Summary: FastAPI-Amis-Admin is a high-performance, efficient and easily extensible FastAPI admin framework. Inspired by Django-admin, and has as many powerful functions as Django-admin. 
 Keywords: fastapi,fastapi-admin,fastapi-amis-admin,django-admin,sqlmodel,sqlalchemy
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
@@ -23,14 +23,15 @@
 Requires-Dist: python-multipart>=0.0.5
 Requires-Dist: sqlalchemy-database>=0.1.0,<0.2.0
 Requires-Dist: aiofiles>=0.17.0
 Requires-Dist: fastapi-amis-admin[dev] ; extra == "all"
 Requires-Dist: fastapi-amis-admin-cli>=0.1.0,<0.2.0 ; extra == "cli"
 Requires-Dist: fastapi-amis-admin[test] ; extra == "dev"
 Requires-Dist: pre-commit>=2.20.0 ; extra == "dev"
+Requires-Dist: ruff>=0.0.261 ; extra == "dev"
 Requires-Dist: uvicorn[standard] >=0.19.0,<1.0 ; extra == "standard"
 Requires-Dist: fastapi-amis-admin-cli>=0.1.0,<0.2.0 ; extra == "standard"
 Requires-Dist: fastapi-amis-admin[standard] ; extra == "test"
 Requires-Dist: pytest >=6.2.4,<7.0.0 ; extra == "test"
 Requires-Dist: aiosqlite>=0.15.0 ; extra == "test"
 Requires-Dist: pytest-asyncio>=0.17 ; extra == "test"
 Requires-Dist: httpx>=0.23.0,<1.0 ; extra == "test"
```

