# Comparing `tmp/oking_oz-3.2.28.tar.gz` & `tmp/oking_oz-3.2.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oking_oz-3.2.28.tar", last modified: Mon Apr 10 19:00:32 2023, max compression
+gzip compressed data, was "oking_oz-3.2.30.tar", last modified: Wed Apr 19 16:47:58 2023, max compression
```

## Comparing `oking_oz-3.2.28.tar` & `oking_oz-3.2.30.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 19:00:32.646843 oking_oz-3.2.28/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.28/LICENSE
--rw-rw-rw-   0        0        0       29 2022-06-03 11:48:57.000000 oking_oz-3.2.28/MANIFEST.in
--rw-rw-rw-   0        0        0      935 2023-04-10 19:00:32.646843 oking_oz-3.2.28/PKG-INFO
--rw-rw-rw-   0        0        0     1187 2022-06-03 12:55:44.000000 oking_oz-3.2.28/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 19:00:32.596725 oking_oz-3.2.28/oking_oz.egg-info/
--rw-rw-rw-   0        0        0      935 2023-04-10 19:00:32.000000 oking_oz-3.2.28/oking_oz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1551 2023-04-10 19:00:32.000000 oking_oz-3.2.28/oking_oz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 19:00:32.000000 oking_oz-3.2.28/oking_oz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-10 19:00:32.000000 oking_oz-3.2.28/oking_oz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-04-10 19:00:32.000000 oking_oz-3.2.28/oking_oz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-10 19:00:32.000000 oking_oz-3.2.28/oking_oz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-06-03 11:48:57.000000 oking_oz-3.2.28/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 19:00:32.646843 oking_oz-3.2.28/setup.cfg
--rw-rw-rw-   0        0        0     1833 2023-04-10 19:00:09.000000 oking_oz-3.2.28/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 19:00:32.596725 oking_oz-3.2.28/src/
--rw-rw-rw-   0        0        0     2979 2022-08-23 11:22:25.000000 oking_oz-3.2.28/src/__init__.py
--rw-rw-rw-   0        0        0    25475 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 19:00:32.607008 oking_oz-3.2.28/src/api/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.28/src/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 19:00:32.616798 oking_oz-3.2.28/src/api/entities/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.28/src/api/entities/__init__.py
--rw-rw-rw-   0        0        0     5097 2022-12-16 19:21:16.000000 oking_oz-3.2.28/src/api/entities/cliente.py
--rw-rw-rw-   0        0        0     4496 2022-12-23 14:47:52.000000 oking_oz-3.2.28/src/api/entities/cliente_aprovado.py
--rw-rw-rw-   0        0        0      249 2022-12-19 18:06:20.000000 oking_oz-3.2.28/src/api/entities/cliente_erp_code.py
--rw-rw-rw-   0        0        0      932 2022-10-03 17:41:50.000000 oking_oz-3.2.28/src/api/entities/imposto_produto.py
--rw-rw-rw-   0        0        0     1171 2022-10-03 17:41:50.000000 oking_oz-3.2.28/src/api/entities/lista_preco.py
--rw-rw-rw-   0        0        0      390 2022-12-16 19:21:16.000000 oking_oz-3.2.28/src/api/entities/plano_pagamento_cliente.py
--rw-rw-rw-   0        0        0      934 2022-12-16 19:21:16.000000 oking_oz-3.2.28/src/api/entities/representante.py
--rw-rw-rw-   0        0        0      739 2022-06-03 11:48:57.000000 oking_oz-3.2.28/src/api/oking.py
--rw-rw-rw-   0        0        0    20636 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/api/okvendas.py
--rw-rw-rw-   0        0        0      886 2022-06-03 11:48:57.000000 oking_oz-3.2.28/src/api/slack.py
-drwxrwxrwx   0        0        0        0 2023-04-10 19:00:32.616798 oking_oz-3.2.28/src/database/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.28/src/database/__init__.py
--rw-rw-rw-   0        0        0     2488 2022-08-23 11:22:25.000000 oking_oz-3.2.28/src/database/connection.py
-drwxrwxrwx   0        0        0        0 2023-04-10 19:00:32.627666 oking_oz-3.2.28/src/database/entities/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.28/src/database/entities/__init__.py
--rw-rw-rw-   0        0        0     1616 2022-12-16 19:21:16.000000 oking_oz-3.2.28/src/database/entities/client.py
--rw-rw-rw-   0        0        0      253 2022-12-16 19:21:16.000000 oking_oz-3.2.28/src/database/entities/client_payment_plan.py
--rw-rw-rw-   0        0        0     1077 2022-10-03 17:41:50.000000 oking_oz-3.2.28/src/database/entities/price_list.py
--rw-rw-rw-   0        0        0      801 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/database/entities/product_tax.py
--rw-rw-rw-   0        0        0      639 2022-12-16 19:21:16.000000 oking_oz-3.2.28/src/database/entities/representative.py
--rw-rw-rw-   0        0        0    49069 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/database/queries.py
--rw-rw-rw-   0        0        0      327 2022-07-04 16:40:47.000000 oking_oz-3.2.28/src/database/sqlserver_db.py
--rw-rw-rw-   0        0        0     1106 2022-07-04 16:40:47.000000 oking_oz-3.2.28/src/database/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 19:00:32.636890 oking_oz-3.2.28/src/entities/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.28/src/entities/__init__.py
--rw-rw-rw-   0        0        0      628 2022-07-29 17:49:42.000000 oking_oz-3.2.28/src/entities/invoice.py
--rw-rw-rw-   0        0        0      288 2022-06-03 11:48:57.000000 oking_oz-3.2.28/src/entities/log.py
--rw-rw-rw-   0        0        0     6798 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/entities/order.py
--rw-rw-rw-   0        0        0    16869 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/entities/orderb2b.py
--rw-rw-rw-   0        0        0     6583 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/entities/orderb2c.py
--rw-rw-rw-   0        0        0     3014 2022-06-03 11:48:57.000000 oking_oz-3.2.28/src/entities/pagamento.py
--rw-rw-rw-   0        0        0      351 2022-06-03 11:48:57.000000 oking_oz-3.2.28/src/entities/photos_sku.py
--rw-rw-rw-   0        0        0      407 2022-06-03 11:48:57.000000 oking_oz-3.2.28/src/entities/price.py
--rw-rw-rw-   0        0        0    10790 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/entities/product.py
--rw-rw-rw-   0        0        0     1959 2022-12-16 19:21:16.000000 oking_oz-3.2.28/src/entities/response.py
--rw-rw-rw-   0        0        0      940 2022-06-03 11:48:57.000000 oking_oz-3.2.28/src/entities/tracking.py
-drwxrwxrwx   0        0        0        0 2023-04-10 19:00:32.646843 oking_oz-3.2.28/src/jobs/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.28/src/jobs/__init__.py
--rw-rw-rw-   0        0        0    18254 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/jobs/client_jobs.py
--rw-rw-rw-   0        0        0     8965 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/jobs/client_payment_plan_jobs.py
--rw-rw-rw-   0        0        0     2937 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/jobs/client_payment_plan_semaphore_jobs.py
--rw-rw-rw-   0        0        0    83787 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/jobs/order_jobs.py
--rw-rw-rw-   0        0        0    19666 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/jobs/price_jobs.py
--rw-rw-rw-   0        0        0    25107 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/jobs/products_jobs.py
--rw-rw-rw-   0        0        0     6841 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/jobs/representative_jobs.py
--rw-rw-rw-   0        0        0    12784 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/jobs/stock_jobs.py
--rw-rw-rw-   0        0        0     2003 2023-04-10 18:55:42.000000 oking_oz-3.2.28/src/jobs/system_jobs.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:47:58.715412 oking_oz-3.2.30/
+-rw-rw-rw-   0        0        0        0 2022-05-12 13:12:05.000000 oking_oz-3.2.30/LICENSE
+-rw-rw-rw-   0        0        0       29 2022-05-12 13:12:05.000000 oking_oz-3.2.30/MANIFEST.in
+-rw-rw-rw-   0        0        0      935 2023-04-19 16:47:58.713412 oking_oz-3.2.30/PKG-INFO
+-rw-rw-rw-   0        0        0     1187 2022-06-07 17:54:09.000000 oking_oz-3.2.30/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 16:47:58.530420 oking_oz-3.2.30/oking_oz.egg-info/
+-rw-rw-rw-   0        0        0      935 2023-04-19 16:47:58.000000 oking_oz-3.2.30/oking_oz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1551 2023-04-19 16:47:58.000000 oking_oz-3.2.30/oking_oz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 16:47:58.000000 oking_oz-3.2.30/oking_oz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-19 16:47:58.000000 oking_oz-3.2.30/oking_oz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       96 2023-04-19 16:47:58.000000 oking_oz-3.2.30/oking_oz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-19 16:47:58.000000 oking_oz-3.2.30/oking_oz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-05-12 13:12:05.000000 oking_oz-3.2.30/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 16:47:58.715412 oking_oz-3.2.30/setup.cfg
+-rw-rw-rw-   0        0        0     1833 2023-04-19 16:47:55.000000 oking_oz-3.2.30/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:47:58.537412 oking_oz-3.2.30/src/
+-rw-rw-rw-   0        0        0     2979 2022-10-11 18:25:34.000000 oking_oz-3.2.30/src/__init__.py
+-rw-rw-rw-   0        0        0    25475 2023-03-30 19:14:59.000000 oking_oz-3.2.30/src/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:47:58.553413 oking_oz-3.2.30/src/api/
+-rw-rw-rw-   0        0        0        0 2022-05-12 13:12:05.000000 oking_oz-3.2.30/src/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:47:58.588409 oking_oz-3.2.30/src/api/entities/
+-rw-rw-rw-   0        0        0        0 2022-06-07 17:53:11.000000 oking_oz-3.2.30/src/api/entities/__init__.py
+-rw-rw-rw-   0        0        0     5097 2022-11-10 17:25:47.000000 oking_oz-3.2.30/src/api/entities/cliente.py
+-rw-rw-rw-   0        0        0     4496 2023-01-18 12:21:21.000000 oking_oz-3.2.30/src/api/entities/cliente_aprovado.py
+-rw-rw-rw-   0        0        0      249 2022-12-09 13:49:41.000000 oking_oz-3.2.30/src/api/entities/cliente_erp_code.py
+-rw-rw-rw-   0        0        0      932 2023-03-24 18:51:35.000000 oking_oz-3.2.30/src/api/entities/imposto_produto.py
+-rw-rw-rw-   0        0        0     1171 2022-10-11 18:41:22.000000 oking_oz-3.2.30/src/api/entities/lista_preco.py
+-rw-rw-rw-   0        0        0      390 2022-11-10 17:25:47.000000 oking_oz-3.2.30/src/api/entities/plano_pagamento_cliente.py
+-rw-rw-rw-   0        0        0      934 2022-10-11 18:41:22.000000 oking_oz-3.2.30/src/api/entities/representante.py
+-rw-rw-rw-   0        0        0      739 2022-08-04 16:50:16.000000 oking_oz-3.2.30/src/api/oking.py
+-rw-rw-rw-   0        0        0    20636 2023-03-30 19:04:33.000000 oking_oz-3.2.30/src/api/okvendas.py
+-rw-rw-rw-   0        0        0      886 2022-06-07 17:54:09.000000 oking_oz-3.2.30/src/api/slack.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:47:58.621411 oking_oz-3.2.30/src/database/
+-rw-rw-rw-   0        0        0        0 2022-05-12 13:12:05.000000 oking_oz-3.2.30/src/database/__init__.py
+-rw-rw-rw-   0        0        0     2488 2022-10-11 18:25:34.000000 oking_oz-3.2.30/src/database/connection.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:47:58.646414 oking_oz-3.2.30/src/database/entities/
+-rw-rw-rw-   0        0        0        0 2022-06-07 17:53:11.000000 oking_oz-3.2.30/src/database/entities/__init__.py
+-rw-rw-rw-   0        0        0     1616 2022-11-10 17:25:47.000000 oking_oz-3.2.30/src/database/entities/client.py
+-rw-rw-rw-   0        0        0      253 2022-11-10 17:25:47.000000 oking_oz-3.2.30/src/database/entities/client_payment_plan.py
+-rw-rw-rw-   0        0        0     1077 2022-10-11 18:41:22.000000 oking_oz-3.2.30/src/database/entities/price_list.py
+-rw-rw-rw-   0        0        0      801 2023-03-24 18:55:10.000000 oking_oz-3.2.30/src/database/entities/product_tax.py
+-rw-rw-rw-   0        0        0      639 2022-10-11 18:41:22.000000 oking_oz-3.2.30/src/database/entities/representative.py
+-rw-rw-rw-   0        0        0    49121 2023-04-19 16:46:53.000000 oking_oz-3.2.30/src/database/queries.py
+-rw-rw-rw-   0        0        0      327 2022-05-12 13:12:05.000000 oking_oz-3.2.30/src/database/sqlserver_db.py
+-rw-rw-rw-   0        0        0     1106 2022-06-07 17:54:09.000000 oking_oz-3.2.30/src/database/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:47:58.681414 oking_oz-3.2.30/src/entities/
+-rw-rw-rw-   0        0        0        0 2022-05-12 13:12:05.000000 oking_oz-3.2.30/src/entities/__init__.py
+-rw-rw-rw-   0        0        0      628 2022-05-12 13:12:05.000000 oking_oz-3.2.30/src/entities/invoice.py
+-rw-rw-rw-   0        0        0      288 2022-06-07 17:53:11.000000 oking_oz-3.2.30/src/entities/log.py
+-rw-rw-rw-   0        0        0     6798 2023-02-23 19:03:05.000000 oking_oz-3.2.30/src/entities/order.py
+-rw-rw-rw-   0        0        0    16869 2023-03-03 18:46:53.000000 oking_oz-3.2.30/src/entities/orderb2b.py
+-rw-rw-rw-   0        0        0     6583 2023-02-23 19:03:05.000000 oking_oz-3.2.30/src/entities/orderb2c.py
+-rw-rw-rw-   0        0        0     3014 2022-05-12 13:12:05.000000 oking_oz-3.2.30/src/entities/pagamento.py
+-rw-rw-rw-   0        0        0      351 2022-06-07 17:54:09.000000 oking_oz-3.2.30/src/entities/photos_sku.py
+-rw-rw-rw-   0        0        0      407 2022-06-07 17:53:11.000000 oking_oz-3.2.30/src/entities/price.py
+-rw-rw-rw-   0        0        0    10790 2023-02-23 18:59:53.000000 oking_oz-3.2.30/src/entities/product.py
+-rw-rw-rw-   0        0        0     1959 2022-11-10 17:25:47.000000 oking_oz-3.2.30/src/entities/response.py
+-rw-rw-rw-   0        0        0      940 2022-05-12 13:12:05.000000 oking_oz-3.2.30/src/entities/tracking.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:47:58.710415 oking_oz-3.2.30/src/jobs/
+-rw-rw-rw-   0        0        0        0 2022-05-12 13:12:05.000000 oking_oz-3.2.30/src/jobs/__init__.py
+-rw-rw-rw-   0        0        0    18254 2023-03-24 13:37:59.000000 oking_oz-3.2.30/src/jobs/client_jobs.py
+-rw-rw-rw-   0        0        0     8965 2023-03-22 17:12:58.000000 oking_oz-3.2.30/src/jobs/client_payment_plan_jobs.py
+-rw-rw-rw-   0        0        0     2937 2023-03-22 17:11:32.000000 oking_oz-3.2.30/src/jobs/client_payment_plan_semaphore_jobs.py
+-rw-rw-rw-   0        0        0    83964 2023-04-19 16:46:53.000000 oking_oz-3.2.30/src/jobs/order_jobs.py
+-rw-rw-rw-   0        0        0    19666 2023-03-20 19:07:16.000000 oking_oz-3.2.30/src/jobs/price_jobs.py
+-rw-rw-rw-   0        0        0    25107 2023-03-30 19:02:54.000000 oking_oz-3.2.30/src/jobs/products_jobs.py
+-rw-rw-rw-   0        0        0     6841 2023-03-24 13:58:57.000000 oking_oz-3.2.30/src/jobs/representative_jobs.py
+-rw-rw-rw-   0        0        0    12784 2023-03-20 19:07:16.000000 oking_oz-3.2.30/src/jobs/stock_jobs.py
+-rw-rw-rw-   0        0        0     2003 2023-03-20 19:07:16.000000 oking_oz-3.2.30/src/jobs/system_jobs.py
```

### Comparing `oking_oz-3.2.28/PKG-INFO` & `oking_oz-3.2.30/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oking_oz
-Version: 3.2.28
+Version: 3.2.30
 Summary: Pacote de integração de produtos, preço, estoque e pedidos com o sistema OkVendas da Openk
 Home-page: UNKNOWN
 Author: Openk Tecnologia
 Author-email: <suporte.b2c@openk.com.br>
 License: UNKNOWN
 Keywords: python,oking,openk,okvendas,ok
 Platform: UNKNOWN
```

### Comparing `oking_oz-3.2.28/README.md` & `oking_oz-3.2.30/README.md`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/oking_oz.egg-info/PKG-INFO` & `oking_oz-3.2.30/oking_oz.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oking-oz
-Version: 3.2.28
+Version: 3.2.30
 Summary: Pacote de integração de produtos, preço, estoque e pedidos com o sistema OkVendas da Openk
 Home-page: UNKNOWN
 Author: Openk Tecnologia
 Author-email: <suporte.b2c@openk.com.br>
 License: UNKNOWN
 Keywords: python,oking,openk,okvendas,ok
 Platform: UNKNOWN
```

### Comparing `oking_oz-3.2.28/oking_oz.egg-info/SOURCES.txt` & `oking_oz-3.2.30/oking_oz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/setup.py` & `oking_oz-3.2.30/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #     f = open('version.txt', 'w')
 #     f.write(f'\tOking {v} - Openk Tecnologia')
 #     f.close()
 
 
 # Utilizar o padrão x.x.x.xxxx para caso precise subir versão de testes para o respositorio test-pypi
 # Utilizar o padrão x.x.x para subir em produção
-version = '3.2.28'
+version = '3.2.30'
 package_name = "oking_oz" if len([c for c in version if c == '.']) < 3 else 'okingtest'
 # save_version(version)
 setup(
     name=package_name,
     version=version,
     author="Openk Tecnologia",
     author_email="<suporte.b2c@openk.com.br>",
```

### Comparing `oking_oz-3.2.28/src/__init__.py` & `oking_oz-3.2.30/src/__init__.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/__main__.py` & `oking_oz-3.2.30/src/__main__.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/api/entities/cliente.py` & `oking_oz-3.2.30/src/api/entities/cliente.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/api/entities/cliente_aprovado.py` & `oking_oz-3.2.30/src/api/entities/cliente_aprovado.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/api/entities/imposto_produto.py` & `oking_oz-3.2.30/src/api/entities/imposto_produto.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/api/entities/lista_preco.py` & `oking_oz-3.2.30/src/api/entities/lista_preco.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/api/entities/representante.py` & `oking_oz-3.2.30/src/api/entities/representante.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/api/oking.py` & `oking_oz-3.2.30/src/api/oking.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/api/okvendas.py` & `oking_oz-3.2.30/src/api/okvendas.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/api/slack.py` & `oking_oz-3.2.30/src/api/slack.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/database/connection.py` & `oking_oz-3.2.30/src/database/connection.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/database/entities/client.py` & `oking_oz-3.2.30/src/database/entities/client.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/database/entities/price_list.py` & `oking_oz-3.2.30/src/database/entities/price_list.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/database/entities/product_tax.py` & `oking_oz-3.2.30/src/database/entities/product_tax.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/database/entities/representative.py` & `oking_oz-3.2.30/src/database/entities/representative.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/database/queries.py` & `oking_oz-3.2.30/src/database/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,24 +56,24 @@
 														tipo_logradouro, logradouro, numero, complemento, bairro, cidade, estado, referencia, direcao, codigo_ibge)
 					values (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?) '''
 
 
 def get_insert_b2b_client_command(connection_type: str):
     if connection_type.lower() == 'mysql':
         return '''insert into openk_semaforo.cliente (nome, razao_social, cpf, cnpj, email, telefone_residencial, telefone_celular, cep, 
-														tipo_logradouro, logradouro, numero, complemento, bairro, cidade, estado, referencia, direcao, inscricao_estadual, codigo_ibge)
-					values (%s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s %s) '''
+														tipo_logradouro, logradouro, numero, complemento, bairro, cidade, estado, referencia, direcao, inscricao_estadual, codigo_ibge, cliente_erp)
+					values (%s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s) '''
     elif connection_type.lower() == 'oracle':
         return '''INSERT INTO OPENK_SEMAFORO.CLIENTE (NOME, RAZAO_SOCIAL, CPF, CNPJ, EMAIL, TELEFONE_RESIDENCIAL, TELEFONE_CELULAR, CEP, 
-														TIPO_LOGRADOURO, LOGRADOURO,NUMERO, COMPLEMENTO, BAIRRO, CIDADE, ESTADO, REFERENCIA, DIRECAO, INSCRICAO_ESTADUAL, CODIGO_IBGE) 
-				VALUES (:1, :2, :3, :4, :5, :6, :7, :8, :9, :10, :11, :12, :13, :14, :15, :16, :17, :18, :19) '''
+														TIPO_LOGRADOURO, LOGRADOURO,NUMERO, COMPLEMENTO, BAIRRO, CIDADE, ESTADO, REFERENCIA, DIRECAO, INSCRICAO_ESTADUAL, CODIGO_IBGE, CLIENTE_ERP) 
+				VALUES (:1, :2, :3, :4, :5, :6, :7, :8, :9, :10, :11, :12, :13, :14, :15, :16, :17, :18, :19, :20) '''
     elif connection_type.lower() == 'sql':
         return '''insert into openk_semaforo.cliente (nome, razao_social, cpf, cnpj, email, telefone_residencial, telefone_celular, cep, 
-														tipo_logradouro, logradouro, numero, complemento, bairro, cidade, estado, referencia, direcao, inscricao_estadual, codigo_ibge)
-					values (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?) '''
+														tipo_logradouro, logradouro, numero, complemento, bairro, cidade, estado, referencia, direcao, inscricao_estadual, codigo_ibge, cliente_erp)
+					values (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?) '''
 
 
 def get_insert_b2c_client_command(connection_type: str):
     if connection_type.lower() == 'mysql':
         return '''insert into openk_semaforo.cliente (nome, razao_social, cpf, cnpj, email, telefone_residencial, telefone_celular, cep, 
 														tipo_logradouro, logradouro, numero, complemento, bairro, cidade, estado, referencia, direcao)
 					values (%s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s) '''
```

### Comparing `oking_oz-3.2.28/src/database/utils.py` & `oking_oz-3.2.30/src/database/utils.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/entities/invoice.py` & `oking_oz-3.2.30/src/entities/invoice.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/entities/order.py` & `oking_oz-3.2.30/src/entities/order.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/entities/orderb2b.py` & `oking_oz-3.2.30/src/entities/orderb2b.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/entities/orderb2c.py` & `oking_oz-3.2.30/src/entities/orderb2c.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/entities/pagamento.py` & `oking_oz-3.2.30/src/entities/pagamento.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/entities/product.py` & `oking_oz-3.2.30/src/entities/product.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/entities/response.py` & `oking_oz-3.2.30/src/entities/response.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/entities/tracking.py` & `oking_oz-3.2.30/src/entities/tracking.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/jobs/client_jobs.py` & `oking_oz-3.2.30/src/jobs/client_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/jobs/client_payment_plan_jobs.py` & `oking_oz-3.2.30/src/jobs/client_payment_plan_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/jobs/client_payment_plan_semaphore_jobs.py` & `oking_oz-3.2.30/src/jobs/client_payment_plan_semaphore_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/jobs/order_jobs.py` & `oking_oz-3.2.30/src/jobs/order_jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -940,14 +940,17 @@
 
         if existent_client is None:
             # insere cliente
             step = 'insere cliente'
             logger.info(f'')
             send_log(job_config.get('job_name'), job_config.get('enviar_logs'), False,
                      f'\tPedido {order.order_id}: Inserindo cliente', 'info', 'PEDIDO')
+
+            erp_code = order.user.erp_code if order.user.erp_code is not None and order.user.erp_code not in ['', '0'] else None
+
             cursor.execute(queries.get_insert_b2b_client_command(db_config.db_type),
                            queries.get_command_parameter(db_config.db_type, [
                                order.user.name or order.user.company_name,
                                order.user.company_name or order.user.name,
                                order.user.cpf,
                                order.user.cnpj,
                                order.user.email,
@@ -960,15 +963,16 @@
                                order.user.address.complement,
                                order.user.address.neighbourhood or " ",
                                order.user.address.city,
                                order.user.address.state,
                                order.user.address.reference,
                                'IN',
                                order.user.state_registry,
-                               order.user.address.ibge_code
+                               order.user.address.ibge_code,
+                               erp_code,
                            ]))
         else:
             # update no cliente existente
             step = 'update cliente'
             send_log(job_config.get('job_name'), job_config.get('enviar_logs'), False,
                      f'\tPedido {order.order_id}: Atualizando cliente existente', 'info', 'PEDIDO')
             cursor.execute(queries.get_update_b2b_client_sql(db_config.db_type),
```

### Comparing `oking_oz-3.2.28/src/jobs/price_jobs.py` & `oking_oz-3.2.30/src/jobs/price_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/jobs/products_jobs.py` & `oking_oz-3.2.30/src/jobs/products_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/jobs/representative_jobs.py` & `oking_oz-3.2.30/src/jobs/representative_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/jobs/stock_jobs.py` & `oking_oz-3.2.30/src/jobs/stock_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.28/src/jobs/system_jobs.py` & `oking_oz-3.2.30/src/jobs/system_jobs.py`

 * *Files identical despite different names*

