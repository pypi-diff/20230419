# Comparing `tmp/design.plone.contenttypes-6.0.3.tar.gz` & `tmp/design.plone.contenttypes-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.contenttypes-6.0.3.tar", last modified: Tue Apr 18 07:12:23 2023, max compression
+gzip compressed data, was "design.plone.contenttypes-6.0.4.tar", last modified: Wed Apr 19 07:57:21 2023, max compression
```

## Comparing `design.plone.contenttypes-6.0.3.tar` & `design.plone.contenttypes-6.0.4.tar`

### file list

```diff
@@ -1,362 +1,359 @@
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.618737 design.plone.contenttypes-6.0.3/
--rw-r--r--   0 lucabel    (501) staff       (20)    16110 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/CHANGES.rst
--rw-r--r--   0 lucabel    (501) staff       (20)       67 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/CONTRIBUTORS.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      585 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/DEVELOP.rst
--rw-r--r--   0 lucabel    (501) staff       (20)    18092 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/LICENSE.GPL
--rw-r--r--   0 lucabel    (501) staff       (20)      665 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/LICENSE.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      158 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/MANIFEST.in
--rw-r--r--   0 lucabel    (501) staff       (20)    32900 2023-04-18 07:12:23.618901 design.plone.contenttypes-6.0.3/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)    15519 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/README.md
--rw-r--r--   0 lucabel    (501) staff       (20)       27 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/constraints.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      105 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/constraints_plone60.txt
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.526284 design.plone.contenttypes-6.0.3/docs/
--rw-r--r--   0 lucabel    (501) staff       (20)     7993 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/docs/conf.py
--rw-r--r--   0 lucabel    (501) staff       (20)       98 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/docs/index.rst
--rw-r--r--   0 lucabel    (501) staff       (20)       50 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/requirements.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      383 2023-04-18 07:12:23.619466 design.plone.contenttypes-6.0.3/setup.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     3002 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/setup.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.514696 design.plone.contenttypes-6.0.3/src/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.526572 design.plone.contenttypes-6.0.3/src/design/
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.529976 design.plone.contenttypes-6.0.3/src/design/plone/
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.532703 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/
--rw-r--r--   0 lucabel    (501) staff       (20)      668 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.534620 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/adapters/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/adapters/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      828 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/adapters/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      421 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/adapters/interfaces.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1755 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/adapters/searchabletext_indexers.py
--rw-r--r--   0 lucabel    (501) staff       (20)      231 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/adapters/servizi_correlati.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.540471 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1354 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/additional_help_infos.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2403 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/address.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7942 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/argomenti.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11450 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     6669 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/contatti.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1629 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/dataset_correlati.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2679 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/descrizione_estesa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6334 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/evento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1657 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/geolocation.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2388 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/info_testata.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2733 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/luoghi_correlati.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6580 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1606 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/multi_file.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4559 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/news_additional_fields.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1827 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/servizi_correlati.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1357 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/show_modified.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1688 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/strutture_correlate.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10532 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/trasparenza.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1164 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/update_note.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.541349 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1342 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.542984 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3813 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/change_news_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5162 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/check_servizi.py
--rw-r--r--   0 lucabel    (501) staff       (20)      787 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2796 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/move_news_items.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.544005 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/templates/
--rw-r--r--   0 lucabel    (501) staff       (20)     3360 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     6876 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/templates/check_servizi.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     4760 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.544569 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/overrides/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/overrides/.gitkeep
--rw-r--r--   0 lucabel    (501) staff       (20)      993 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.516421 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/static/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.544875 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/static/js/
--rw-r--r--   0 lucabel    (501) staff       (20)      262 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/static/js/move_content.js
--rw-r--r--   0 lucabel    (501) staff       (20)      469 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/trasparenza.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2464 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.550375 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      315 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)      238 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/dataset.py
--rw-r--r--   0 lucabel    (501) staff       (20)      246 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      283 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/documento_personale.py
--rw-r--r--   0 lucabel    (501) staff       (20)      210 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/evento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      242 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/incarico.py
--rw-r--r--   0 lucabel    (501) staff       (20)      215 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)      275 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/messaggio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      229 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)      271 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      238 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)      238 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)      272 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)      279 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/ricevuta_pagamento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      242 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      283 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/content/unita_organizzativa.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.551540 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/controlpanels/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/controlpanels/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      737 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/controlpanels/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1382 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3441 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/controlpanels/settings.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.555709 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      540 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)      276 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/common.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3259 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      618 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/document.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1265 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3024 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/evento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1660 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/incarico.py
--rw-r--r--   0 lucabel    (501) staff       (20)      848 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1268 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/notizie_e_comunicati_stampa.py
--rw-r--r--   0 lucabel    (501) staff       (20)      969 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1886 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)      631 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1842 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1078 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/unita_organizzativa.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.558771 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      458 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)      989 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/common.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1605 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      411 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/events.py
--rw-r--r--   0 lucabel    (501) staff       (20)      921 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/news.py
--rw-r--r--   0 lucabel    (501) staff       (20)      621 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      829 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)      741 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)      327 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      445 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/uo.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.563555 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/
--rw-r--r--   0 lucabel    (501) staff       (20)      419 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6263 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)      699 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)      857 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/dataset.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8681 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4702 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/documento_personale.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5442 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/incarico.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1483 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/messaggio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      205 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2600 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4773 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1781 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2522 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1838 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py
--rw-r--r--   0 lucabel    (501) staff       (20)    18282 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8198 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/unita_organizzativa.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.565625 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/
--rw-r--r--   0 lucabel    (501) staff       (20)      611 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/README.rst
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.517746 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/__pycache__/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.565968 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)    83688 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po
--rw-r--r--   0 lucabel    (501) staff       (20)    83643 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.518038 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/en/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.566402 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/en/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)    83808 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.518333 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/it/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.567539 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/it/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)     1243 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po
--rw-r--r--   0 lucabel    (501) staff       (20)    84783 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po
--rw-r--r--   0 lucabel    (501) staff       (20)     7287 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/plone.pot
--rw-r--r--   0 lucabel    (501) staff       (20)     1597 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/update.py
--rwxr-xr-x   0 lucabel    (501) staff       (20)      512 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/update.sh
--rw-r--r--   0 lucabel    (501) staff       (20)      712 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/overrides.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.568652 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/patches/
--rw-r--r--   0 lucabel    (501) staff       (20)      516 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/patches/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3700 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/patches/baseserializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)      483 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/patches/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      319 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/patches/patches.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2751 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/permissions.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.519781 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.518927 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.576707 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/
--rw-r--r--   0 lucabel    (501) staff       (20)      314 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     3401 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      331 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     4370 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      286 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2870 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      372 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     8078 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      300 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2156 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      313 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)    13733 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      398 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     5133 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      292 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     1042 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      303 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2196 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      265 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)    15346 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      322 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     1015 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      355 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     3138 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      342 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2275 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      344 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2275 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.579222 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/
--rw-r--r--   0 lucabel    (501) staff       (20)      193 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2681 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/catalog.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1040 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/controlpanel.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1219 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/diff_tool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      519 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/metadata.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.579992 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/registry/
--rw-r--r--   0 lucabel    (501) staff       (20)    19192 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/registry/criteria.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      618 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/registry/settings.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1139 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/repositorytool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     4491 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/rolemap.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.586094 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/
--rw-r--r--   0 lucabel    (501) staff       (20)     1155 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Bando.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      503 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Bando_Folder_Deepening.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3563 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3327 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Dataset.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      921 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Document.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3747 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Documento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3321 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2500 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Event.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3427 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Incarico.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      432 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Link.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3199 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2855 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Modulo.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1007 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/News_Item.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3456 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3430 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Persona.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3178 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Pratica.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3342 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3149 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     4084 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Servizio.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3775 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2212 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Venue.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1194 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.586685 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/to_3000/
--rw-r--r--   0 lucabel    (501) staff       (20)      377 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/to_3000/controlpanel.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      275 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/to_3000/registry.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.586946 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/uninstall/
--rw-r--r--   0 lucabel    (501) staff       (20)      128 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.588060 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      663 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      504 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/converters.py
--rw-r--r--   0 lucabel    (501) staff       (20)      702 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/correlati.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.591100 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      760 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     5795 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6300 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/dxfields.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5743 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/news.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1658 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5844 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5999 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6016 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/venue.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.596104 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1254 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2086 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1858 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2102 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3377 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/dxcontent.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5307 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/dxfields.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1452 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2190 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3771 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1763 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2401 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/relationfield.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1705 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)    13976 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/summary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5523 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3814 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/venue.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.597152 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      685 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.598215 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/content/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/content/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      664 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/content/add.py
--rw-r--r--   0 lucabel    (501) staff       (20)      368 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/content/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      653 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/controlpanel.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.599154 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/modulistica_items/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/modulistica_items/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      605 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2915 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.600257 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/prenotazioni_folders_list/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/prenotazioni_folders_list/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      556 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/prenotazioni_folders_list/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      834 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/prenotazioni_folders_list/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.601046 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/scadenziario/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/scadenziario/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1200 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)    10380 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/scadenziario/post.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.601855 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/trasparenza/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/trasparenza/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      884 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     3351 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/trasparenza/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.602650 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/types/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/types/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      404 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/types/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)    10630 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/types/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.603458 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/types/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/types/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3804 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/types/adapters.py
--rw-r--r--   0 lucabel    (501) staff       (20)      394 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/types/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1628 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/schema_overrides.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2315 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/setuphandlers.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4341 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/testing.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.613945 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11218 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/example.pdf
--rw-r--r--   0 lucabel    (501) staff       (20)     1997 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_argomenti.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2330 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_base_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1564 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3169 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_behavior_luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2563 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_behavior_show_modified.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1755 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_behavior_update_note.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1893 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_change_news_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1679 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1462 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1342 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_document.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6365 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1294 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_documento_personale.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4924 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_event.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7744 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)      982 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8019 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_news.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1296 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5271 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11188 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10788 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2164 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_filefield_view_mode_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2526 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_move_news_items_view.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6638 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2063 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_service_prenotazioni_folders_list.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1381 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3533 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_setup.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11257 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_summary_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1234 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6351 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_vocabularies.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.615656 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/upgrades/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/upgrades/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)    21651 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/upgrades/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     5033 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/upgrades/draftjs_converter.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11792 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/upgrades/to_7001.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5975 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/upgrades/to_7002.py
--rw-r--r--   0 lucabel    (501) staff       (20)    48753 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/upgrades/upgrades.py
--rw-r--r--   0 lucabel    (501) staff       (20)      862 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/utils.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.618499 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1308 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1573 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1824 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1466 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1895 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1704 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/mockup.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2223 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/people_vocabulary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1533 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5199 2023-04-18 07:12:22.000000 design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-18 07:12:23.529346 design.plone.contenttypes-6.0.3/src/design.plone.contenttypes.egg-info/
--rw-r--r--   0 lucabel    (501) staff       (20)    32900 2023-04-18 07:12:23.000000 design.plone.contenttypes-6.0.3/src/design.plone.contenttypes.egg-info/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)    18661 2023-04-18 07:12:23.000000 design.plone.contenttypes-6.0.3/src/design.plone.contenttypes.egg-info/SOURCES.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-04-18 07:12:23.000000 design.plone.contenttypes-6.0.3/src/design.plone.contenttypes.egg-info/dependency_links.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      130 2023-04-18 07:12:23.000000 design.plone.contenttypes-6.0.3/src/design.plone.contenttypes.egg-info/entry_points.txt
--rw-r--r--   0 lucabel    (501) staff       (20)       20 2023-04-18 07:12:23.000000 design.plone.contenttypes-6.0.3/src/design.plone.contenttypes.egg-info/namespace_packages.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-04-18 07:12:23.000000 design.plone.contenttypes-6.0.3/src/design.plone.contenttypes.egg-info/not-zip-safe
--rw-r--r--   0 lucabel    (501) staff       (20)      470 2023-04-18 07:12:23.000000 design.plone.contenttypes-6.0.3/src/design.plone.contenttypes.egg-info/requires.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        7 2023-04-18 07:12:23.000000 design.plone.contenttypes-6.0.3/src/design.plone.contenttypes.egg-info/top_level.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.078411 design.plone.contenttypes-6.0.4/
+-rw-r--r--   0 lucabel    (501) staff       (20)    16236 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/CHANGES.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       67 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/CONTRIBUTORS.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      585 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/DEVELOP.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)    18092 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/LICENSE.GPL
+-rw-r--r--   0 lucabel    (501) staff       (20)      665 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/LICENSE.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      158 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/MANIFEST.in
+-rw-r--r--   0 lucabel    (501) staff       (20)    33000 2023-04-19 07:57:21.078566 design.plone.contenttypes-6.0.4/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)    15519 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/README.md
+-rw-r--r--   0 lucabel    (501) staff       (20)       27 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/constraints.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      105 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/constraints_plone60.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.992127 design.plone.contenttypes-6.0.4/docs/
+-rw-r--r--   0 lucabel    (501) staff       (20)     7993 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/docs/conf.py
+-rw-r--r--   0 lucabel    (501) staff       (20)       98 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/docs/index.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       50 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/requirements.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      383 2023-04-19 07:57:21.079037 design.plone.contenttypes-6.0.4/setup.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2892 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/setup.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.979909 design.plone.contenttypes-6.0.4/src/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.992431 design.plone.contenttypes-6.0.4/src/design/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.995357 design.plone.contenttypes-6.0.4/src/design/plone/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.997654 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/
+-rw-r--r--   0 lucabel    (501) staff       (20)      668 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.999035 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/adapters/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/adapters/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      828 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/adapters/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      421 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/adapters/interfaces.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1755 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/adapters/searchabletext_indexers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      231 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/adapters/servizi_correlati.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.004760 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1354 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/additional_help_infos.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2403 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/address.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7942 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/argomenti.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11450 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     6669 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/contatti.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1629 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/dataset_correlati.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2679 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/descrizione_estesa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6334 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/evento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1657 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/geolocation.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2388 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/info_testata.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2733 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/luoghi_correlati.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6580 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1606 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/multi_file.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4559 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/news_additional_fields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1827 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/servizi_correlati.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1357 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/show_modified.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1688 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/strutture_correlate.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    10532 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/trasparenza.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1164 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/update_note.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.005561 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1342 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.007010 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3813 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/change_news_type.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5162 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/check_servizi.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      787 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2796 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/move_news_items.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.007892 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/templates/
+-rw-r--r--   0 lucabel    (501) staff       (20)     3360 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     6876 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/templates/check_servizi.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     4760 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.008410 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/overrides/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/overrides/.gitkeep
+-rw-r--r--   0 lucabel    (501) staff       (20)      993 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.981554 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/static/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.008703 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/static/js/
+-rw-r--r--   0 lucabel    (501) staff       (20)      262 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/static/js/move_content.js
+-rw-r--r--   0 lucabel    (501) staff       (20)      469 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/trasparenza.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2770 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.013968 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      315 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      238 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/dataset.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      246 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      283 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/documento_personale.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      210 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/evento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      242 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/incarico.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      215 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      275 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/messaggio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      229 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      271 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      238 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      238 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      272 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      279 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/ricevuta_pagamento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      242 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      283 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/content/unita_organizzativa.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.015115 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/controlpanels/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/controlpanels/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      737 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/controlpanels/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1382 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3441 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/controlpanels/settings.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.019404 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      540 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      276 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/common.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2964 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      618 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/document.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1265 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3024 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/evento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1660 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/incarico.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      848 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1268 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/notizie_e_comunicati_stampa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      969 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1886 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      631 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1053 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1078 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/unita_organizzativa.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.022566 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      458 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      989 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/common.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1605 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      411 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/events.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      921 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/news.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      621 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      829 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      741 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      327 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      445 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/uo.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.027325 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/
+-rw-r--r--   0 lucabel    (501) staff       (20)      419 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6263 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      699 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      857 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/dataset.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8681 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4702 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/documento_personale.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5442 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/incarico.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1483 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/messaggio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      205 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2600 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4773 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1781 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2522 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1838 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    18282 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8198 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/unita_organizzativa.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.029032 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/
+-rw-r--r--   0 lucabel    (501) staff       (20)      611 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/README.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.982853 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/__pycache__/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.029318 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)    83688 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po
+-rw-r--r--   0 lucabel    (501) staff       (20)    83643 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.983150 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/en/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.029735 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/en/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)    83808 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.983452 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/it/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.030791 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/it/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1243 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po
+-rw-r--r--   0 lucabel    (501) staff       (20)    84783 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po
+-rw-r--r--   0 lucabel    (501) staff       (20)     7287 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/plone.pot
+-rw-r--r--   0 lucabel    (501) staff       (20)     1597 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/update.py
+-rwxr-xr-x   0 lucabel    (501) staff       (20)      512 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/update.sh
+-rw-r--r--   0 lucabel    (501) staff       (20)      712 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/overrides.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.031871 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/patches/
+-rw-r--r--   0 lucabel    (501) staff       (20)      516 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/patches/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3700 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/patches/baseserializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      483 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/patches/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      319 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/patches/patches.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2751 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/permissions.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.985060 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.984037 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.040009 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/
+-rw-r--r--   0 lucabel    (501) staff       (20)      314 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     3401 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      331 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     4370 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      286 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2870 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      372 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     8078 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      300 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2156 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      313 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)    13733 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      398 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     5133 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      292 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     1042 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      303 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2196 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      265 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)    15346 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      322 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     1015 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      355 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     3138 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      342 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2275 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      344 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2275 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.042663 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/
+-rw-r--r--   0 lucabel    (501) staff       (20)      193 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2681 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/catalog.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1040 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/controlpanel.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1219 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/diff_tool.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      519 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/metadata.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.043190 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/registry/
+-rw-r--r--   0 lucabel    (501) staff       (20)    19192 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/registry/criteria.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      618 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/registry/settings.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1139 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/repositorytool.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     4491 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/rolemap.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.048341 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1155 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Bando.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      503 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Bando_Folder_Deepening.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3563 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3327 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Dataset.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      921 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Document.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3747 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Documento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3321 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2500 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Event.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3427 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Incarico.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      432 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Link.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3199 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2855 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Modulo.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1007 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/News_Item.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3456 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3430 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Persona.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3178 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Pratica.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3342 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3149 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3784 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Servizio.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3775 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2212 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Venue.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1194 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.048578 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/fix_syndication/
+-rw-r--r--   0 lucabel    (501) staff       (20)      524 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.049077 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/to_3000/
+-rw-r--r--   0 lucabel    (501) staff       (20)      377 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/to_3000/controlpanel.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      275 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/to_3000/registry.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.049317 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/uninstall/
+-rw-r--r--   0 lucabel    (501) staff       (20)      128 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.050217 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      663 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      504 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/converters.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      702 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/correlati.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.052512 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      760 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     5795 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6300 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/dxfields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5743 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/news.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1658 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5844 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5999 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6016 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/venue.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.056815 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1254 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2086 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1858 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2102 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3377 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/dxcontent.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5307 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/dxfields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1452 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2190 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3771 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1763 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2401 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/relationfield.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1705 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    13976 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/summary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5523 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3814 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/venue.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.057632 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      564 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.058342 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/content/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/content/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      664 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/content/add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      368 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/content/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      653 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/controlpanel.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.059279 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/modulistica_items/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/modulistica_items/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      605 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2915 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.059980 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/scadenziario/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/scadenziario/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1200 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)    10380 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/scadenziario/post.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.061598 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/trasparenza/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/trasparenza/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      884 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3351 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/trasparenza/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.062714 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/types/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      404 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/types/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)    10630 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/types/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.063706 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/types/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3804 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/types/adapters.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      394 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/types/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1628 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/schema_overrides.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2315 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/setuphandlers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3857 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/testing.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.073383 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11218 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/example.pdf
+-rw-r--r--   0 lucabel    (501) staff       (20)     1997 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_argomenti.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2330 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_base_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1564 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3169 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_behavior_luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2563 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_behavior_show_modified.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1755 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_behavior_update_note.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1893 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_change_news_type.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1679 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1462 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1342 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_document.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6365 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1294 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_documento_personale.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4924 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_event.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7744 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      982 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8019 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_news.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1296 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5271 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11188 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    10788 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2164 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_filefield_view_mode_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2526 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_move_news_items_view.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6638 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1381 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3533 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_setup.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11257 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_summary_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1234 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6351 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_vocabularies.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.075676 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/upgrades/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/upgrades/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    21941 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/upgrades/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     5033 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/upgrades/draftjs_converter.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11792 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/upgrades/to_7001.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5975 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/upgrades/to_7002.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    50684 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/upgrades/upgrades.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      862 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/utils.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:21.078212 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1308 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1573 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1824 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1466 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1895 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1704 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/mockup.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2223 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/people_vocabulary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1533 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5199 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-19 07:57:20.995073 design.plone.contenttypes-6.0.4/src/design.plone.contenttypes.egg-info/
+-rw-r--r--   0 lucabel    (501) staff       (20)    33000 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design.plone.contenttypes.egg-info/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)    18398 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design.plone.contenttypes.egg-info/SOURCES.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design.plone.contenttypes.egg-info/dependency_links.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      130 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design.plone.contenttypes.egg-info/entry_points.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       20 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design.plone.contenttypes.egg-info/namespace_packages.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design.plone.contenttypes.egg-info/not-zip-safe
+-rw-r--r--   0 lucabel    (501) staff       (20)      411 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design.plone.contenttypes.egg-info/requires.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        7 2023-04-19 07:57:20.000000 design.plone.contenttypes-6.0.4/src/design.plone.contenttypes.egg-info/top_level.txt
```

### Comparing `design.plone.contenttypes-6.0.3/CHANGES.rst` & `design.plone.contenttypes-6.0.4/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 Changelog
 =========
 
 
+6.0.4 (2023-04-19)
+------------------
+
+- Remove redturtle.prenotazioni integration.
+  [cekk]
+- Fix syndication.
+  [lucabel]
+
+
 6.0.3 (2023-04-18)
 ------------------
 
 - Change check_servizi making optional the check for
   field "condizioni_di_servizio" and removing the check for
   the "contact_info" field.
   Import a fontawesome cdn in this view to show the "V" icon.
```

### Comparing `design.plone.contenttypes-6.0.3/DEVELOP.rst` & `design.plone.contenttypes-6.0.4/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/LICENSE.GPL` & `design.plone.contenttypes-6.0.4/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/LICENSE.rst` & `design.plone.contenttypes-6.0.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/PKG-INFO` & `design.plone.contenttypes-6.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.contenttypes
-Version: 6.0.3
+Version: 6.0.4
 Summary: DesignItalia contenty types
 Home-page: https://github.com/collective/design.plone.contenttypes
 Author: RedTurtle
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.contenttypes
 Project-URL: Source, https://github.com/RedTurtle/design.plone.contenttypes
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
-Provides-Extra: ioprenoto
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 [![Latest Version](https://img.shields.io/pypi/v/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Supported - Python Versions](https://img.shields.io/pypi/pyversions/design.plone.contenttypes.svg?style=plastic)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![License](https://img.shields.io/pypi/l/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
@@ -486,14 +485,23 @@
 - RedTurtle, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
 
+6.0.4 (2023-04-19)
+------------------
+
+- Remove redturtle.prenotazioni integration.
+  [cekk]
+- Fix syndication.
+  [lucabel]
+
+
 6.0.3 (2023-04-18)
 ------------------
 
 - Change check_servizi making optional the check for
   field "condizioni_di_servizio" and removing the check for
   the "contact_info" field.
   Import a fontawesome cdn in this view to show the "V" icon.
```

### Comparing `design.plone.contenttypes-6.0.3/README.md` & `design.plone.contenttypes-6.0.4/README.md`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/docs/conf.py` & `design.plone.contenttypes-6.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/setup.py` & `design.plone.contenttypes-6.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.contenttypes",
-    version="6.0.3",
+    version="6.0.4",
     description="DesignItalia contenty types",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
@@ -72,18 +72,14 @@
             # Remove if your package shall be part of coredev.
             # plone_coredev tests as of 2016-04-01.
             "collective.volto.blocksfield",
             "plone.testing>=5.0.0",
             "plone.app.contenttypes",
             "plone.app.robotframework[debug]",
             "collective.MockMailHost",
-            "redturtle.prenotazioni",
-        ],
-        "ioprenoto": [
-            "redturtle.prenotazioni",
         ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     [console_scripts]
     update_locale = design.plone.contenttypes.locales.update:update_locale
```

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/__init__.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/adapters/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/adapters/searchabletext_indexers.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/adapters/searchabletext_indexers.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/additional_help_infos.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/additional_help_infos.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/address.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/address.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/argomenti.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/argomenti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/contatti.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/contatti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/dataset_correlati.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/dataset_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/descrizione_estesa.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/descrizione_estesa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/evento.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/evento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/geolocation.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/geolocation.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/info_testata.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/info_testata.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/luoghi_correlati.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/luoghi_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/luogo.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/multi_file.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/multi_file.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/news_additional_fields.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/news_additional_fields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/servizi_correlati.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/servizi_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/show_modified.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/show_modified.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/strutture_correlate.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/strutture_correlate.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/trasparenza.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/trasparenza.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/behaviors/update_note.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/behaviors/update_note.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/change_news_type.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/change_news_type.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/check_servizi.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/check_servizi.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/move_news_items.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/move_news_items.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/templates/check_servizi.pt` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/templates/check_servizi.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/configure.zcml`

 * *Files 10% similar despite different names*

```diff
@@ -53,14 +53,22 @@
       name="to_3000"
       title="Design Plone: Content-types to 3000"
       description="Fix control panel of design.plone.contenttypes add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
       directory="profiles/to_3000"
       />
 
+  <genericsetup:registerProfile
+      name="fix_syndication"
+      title="Design Plone: Fix Syndication after Plone6 Migration"
+      description="After Plone6 migration syndication is broken"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/fix_syndication"
+      />
+
   <utility
       factory=".setuphandlers.HiddenProfiles"
       name="design.plone.contenttypes-hiddenprofiles"
       />
 
   <!-- schema customizations -->
   <adapter
```

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/controlpanels/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/controlpanels/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/controlpanels/settings.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/controlpanels/settings.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/bando.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/configure.zcml`

 * *Files 12% similar despite different names*

```diff
@@ -73,17 +73,8 @@
   <!-- common -->
   <subscriber
       for="plone.dexterity.interfaces.IDexterityContent
            zope.lifecycleevent.interfaces.IObjectModifiedEvent"
       handler=".common.onModify"
       />
 
-  <configure zcml:condition="installed redturtle.prenotazioni">
-    <subscriber
-        for="design.plone.contenttypes.interfaces.servizio.IServizio
-             zope.lifecycleevent.interfaces.IObjectAddedEvent"
-        handler=".servizio.prenotazioni_folder_create"
-        />
-  </configure>
-
-
 </configure>
```

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/document.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/document.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/documento.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/evento.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/evento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/incarico.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/incarico.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/luogo.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/notizie_e_comunicati_stampa.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/notizie_e_comunicati_stampa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/pagina_argomento.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/persona.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/pratica.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/events/unita_organizzativa.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/events/unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/common.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/common.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/news.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/news.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/pagina_argomento.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/persona.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/indexers/punto_di_contatto.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/indexers/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/bando.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/cartella_modulistica.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/dataset.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/dataset.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/documento.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/documento_personale.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/documento_personale.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/incarico.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/incarico.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/messaggio.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/messaggio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/pagina_argomento.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/persona.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/pratica.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/punto_di_contatto.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/servizio.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/interfaces/unita_organizzativa.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/interfaces/unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/README.rst` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/update.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/locales/update.sh` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/locales/update.sh`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/overrides.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/overrides.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/patches/__init__.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/patches/baseserializer.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/patches/baseserializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/permissions.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/permissions.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/catalog.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/controlpanel.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/diff_tool.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/diff_tool.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/metadata.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/metadata.xml`

 * *Files 1% similar despite different names*

#### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/metadata.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/metadata.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <metadata>
-  <version>7009</version>
+  <version>7010</version>
   <dependencies>
     <dependency>profile-redturtle.bandi:default</dependency>
     <dependency>profile-collective.venue:default</dependency>
     <dependency>profile-redturtle.volto:default</dependency>
     <dependency>profile-eea.api.taxonomy:default</dependency>
     <dependency>profile-collective.z3cform.datagridfield:default</dependency>
     <dependency>profile-design.plone.contenttypes:taxonomy</dependency>
```

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/registry/criteria.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/registry/criteria.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/registry/settings.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/registry/settings.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/repositorytool.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/repositorytool.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/rolemap.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Bando.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Bando.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Dataset.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Dataset.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Document.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Document.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Documento.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Documento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Event.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Event.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Incarico.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Incarico.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Modulo.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Modulo.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/News_Item.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/News_Item.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Persona.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Persona.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Pratica.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Pratica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Servizio.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Servizio.xml`

 * *Files 3% similar despite different names*

#### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Servizio.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Servizio.xml`

```diff
@@ -11,20 +11,14 @@
   <property name="global_allow">True</property>
   <property name="filter_content_types">True</property>
   <property name="allowed_content_types" purge="False">
     <element value="CartellaModulistica"/>
     <element value="Document"/>
     <element value="Image"/>
     <element value="File"/>
-    <!-- 
-      * integration btw design.plone.contenttypes and redturtle.prenotazioni
-        TODO: rivalutare se è necessario, o se i folder e i folder delle prenotazioni
-              vanno creati manualmente al di fuori del servizio
-    -->
-    <element value="PrenotazioniFolderContainer"/>
   </property>
   <!-- Schema, class and security -->
   <property name="add_permission">design.plone.contenttypes.AddServizio</property>
   <property name="klass">design.plone.contenttypes.content.servizio.Servizio</property>
   <property name="model_file"/>
   <property name="model_source"/>
   <property name="schema">design.plone.contenttypes.interfaces.servizio.IServizio</property>
```

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types/Venue.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types/Venue.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/profiles/default/types.xml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/correlati.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/documento.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/dxfields.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/dxfields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/news.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/news.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/persona.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/servizio.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/deserializers/venue.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/deserializers/venue.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/bando.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/documento.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/dxcontent.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/dxcontent.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/dxfields.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/dxfields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/modulo.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/modulo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/persona.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/relationfield.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/relationfield.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/servizio.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/summary.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/summary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/serializers/venue.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/serializers/venue.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/configure.zcml`

 * *Files 23% similar despite different names*

```diff
@@ -6,20 +6,14 @@
 
   <include package=".content" />
   <include package=".modulistica_items" />
   <include package=".types" />
   <include package=".scadenziario" />
   <include package=".trasparenza" />
 
-  <include
-      package=".prenotazioni_folders_list"
-      zcml:condition="installed redturtle.prenotazioni"
-      />
-
-
   <adapter
       factory=".controlpanel.DesignPloneSettings"
       provides="design.plone.contenttypes.controlpanels.settings.IDesignPloneSettingsControlpanel"
       name="design-plone-settings"
       />
 
 </configure>
```

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/content/add.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/content/add.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/controlpanel.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/controlpanel.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/scadenziario/post.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/scadenziario/post.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/trasparenza/get.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/trasparenza/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/services/types/get.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/services/types/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/restapi/types/adapters.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/restapi/types/adapters.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/schema_overrides.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/schema_overrides.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/setuphandlers.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/testing.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,27 @@
 from plone.app.testing import IntegrationTesting
 from plone.testing import z2
 from redturtle.volto.testing import RedturtleVoltoLayer
 from redturtle.volto.testing import RedturtleVoltoRestApiLayer
 from zope.configuration import xmlconfig
 
 import collective.address
-import collective.contentrules.mailfromfield
 import collective.taxonomy
 
 # import collective.folderishtypes
 import collective.venue
 import collective.volto.blocksfield
 import collective.volto.cookieconsent
 import collective.z3cform.datagridfield
 import design.plone.contenttypes
 import eea.api.taxonomy
 import kitconcept.seo
 import plone.app.caching
 import plone.formwidget.geolocation
 import redturtle.bandi
-import redturtle.prenotazioni
 import redturtle.volto
 
 
 class DesignPloneContenttypesLayer(RedturtleVoltoLayer):
     def setUpZope(self, app, configurationContext):
         # Load any other ZCML that is required for your tests.
         # The z3c.autoinclude feature is disabled in the Plone fixture base
@@ -81,26 +79,19 @@
             "configure.zcml",
             design.plone.contenttypes,
             context=configurationContext,
         )
         self.loadZCML(package=redturtle.bandi)
         self.loadZCML(package=kitconcept.seo)
 
-        # TODO: valutare un layer a parte per i test di redturtle.prenotazioni
-        self.loadZCML(package=redturtle.prenotazioni)
-        self.loadZCML(package=collective.z3cform.datagridfield)
-        self.loadZCML(package=collective.contentrules.mailfromfield)
-
         self.loadZCML(name="overrides.zcml", package=design.plone.contenttypes)
 
     def setUpPloneSite(self, portal):
         super().setUpPloneSite(portal)
         applyProfile(portal, "design.plone.contenttypes:default")
-        # TODO: valutare un layer a parte per i test di redturtle.prenotazioni
-        applyProfile(portal, "redturtle.prenotazioni:default")
 
 
 DESIGN_PLONE_CONTENTTYPES_API_FIXTURE = DesignPloneContenttypesRestApiLayer()
 DESIGN_PLONE_CONTENTTYPES_API_INTEGRATION_TESTING = IntegrationTesting(
     bases=(DESIGN_PLONE_CONTENTTYPES_API_FIXTURE,),
     name="DesignPloneContenttypesRestApiLayer:Integration",
 )
```

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/example.pdf` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/example.pdf`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_argomenti.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_argomenti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_base_serializer.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_base_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_behavior_luogo.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_behavior_luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_behavior_show_modified.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_behavior_show_modified.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_behavior_update_note.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_behavior_update_note.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_change_news_type.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_change_news_type.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_bando.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_document.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_document.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_documento.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_documento_personale.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_documento_personale.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_event.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_event.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_luogo.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_modulo.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_modulo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_news.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_news.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_persona.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_servizio.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_filefield_view_mode_serializer.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_filefield_view_mode_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_move_news_items_view.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_move_news_items_view.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_service_prenotazioni_folders_list.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,38 @@
 # -*- coding: utf-8 -*-
-# TODO: skip se redturtle.prenotazioni non è presente
 from design.plone.contenttypes.testing import (
     DESIGN_PLONE_CONTENTTYPES_API_FUNCTIONAL_TESTING,
 )
-from plone import api
 from plone.app.testing import setRoles
 from plone.app.testing import SITE_OWNER_NAME
 from plone.app.testing import SITE_OWNER_PASSWORD
 from plone.app.testing import TEST_USER_ID
 from plone.restapi.testing import RelativeSession
 
-import transaction
 import unittest
 
 
-class TestServicePrnotazioniFoldersList(unittest.TestCase):
+class SettingsControlpanelTest(unittest.TestCase):
     layer = DESIGN_PLONE_CONTENTTYPES_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.portal_url = self.portal.absolute_url()
-        self.testing_view_name = "@prenotazioni_folders-list"
 
         self.api_session = RelativeSession(self.portal_url)
         self.api_session.headers.update({"Accept": "application/json"})
-
         self.api_session.auth = (SITE_OWNER_NAME, SITE_OWNER_PASSWORD)
 
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
 
-        self.servizio = api.content.create(
-            type="Servizio", title="servizio", container=self.portal
-        )
-        self.prenotazioni_folders_folder = api.content.create(
-            type="Folder", title="PrenotazioniFolders", container=self.servizio
-        )
-
-        transaction.commit()
-
-    def test_no_prenotazioni_folders(self):
-        res = self.api_session.get(
-            self.servizio.absolute_url() + "/" + self.testing_view_name
-        ).json()
-
-        self.assertFalse(res)
-
-    def test_prenotazioni_folders(self):
-        prenotazione_folder = api.content.create(
-            type="PrenotazioniFolder",
-            title="prenotazioni_folder",
-            container=self.prenotazioni_folders_folder,
-        )
-        transaction.commit()
-
-        res = self.api_session.get(
-            self.servizio.absolute_url() + "/" + self.testing_view_name
-        ).json()
+    def test_controlpanel_exists(self):
+        response = self.api_session.get("/@controlpanels/design-plone-settings")
+
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(response.headers.get("Content-Type"), "application/json")
+
+    def test_controlpanel_listed(self):
+        response = self.api_session.get("/@controlpanels")
 
-        self.assertIn(prenotazione_folder.absolute_url(), [item["@id"] for item in res])
+        titles = [x.get("title") for x in response.json()]
+        self.assertIn("Impostazioni Design Plone", titles)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 # -*- coding: utf-8 -*-
 from design.plone.contenttypes.testing import (
     DESIGN_PLONE_CONTENTTYPES_API_FUNCTIONAL_TESTING,
 )
+from plone import api
 from plone.app.testing import setRoles
-from plone.app.testing import SITE_OWNER_NAME
-from plone.app.testing import SITE_OWNER_PASSWORD
 from plone.app.testing import TEST_USER_ID
-from plone.restapi.testing import RelativeSession
+from plone.formwidget.geolocation import Geolocation
+from plone.restapi.interfaces import ISerializeToJsonSummary
+from zope.component import getMultiAdapter
 
 import unittest
 
 
-class SettingsControlpanelTest(unittest.TestCase):
+class UOSummarySerializerTest(unittest.TestCase):
     layer = DESIGN_PLONE_CONTENTTYPES_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
-        self.portal_url = self.portal.absolute_url()
-
-        self.api_session = RelativeSession(self.portal_url)
-        self.api_session.headers.update({"Accept": "application/json"})
-        self.api_session.auth = (SITE_OWNER_NAME, SITE_OWNER_PASSWORD)
 
+    def test_geolocation_injected(self):
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
 
-    def test_controlpanel_exists(self):
-        response = self.api_session.get("/@controlpanels/design-plone-settings")
-
-        self.assertEqual(response.status_code, 200)
-        self.assertEqual(response.headers.get("Content-Type"), "application/json")
-
-    def test_controlpanel_listed(self):
-        response = self.api_session.get("/@controlpanels")
-
-        titles = [x.get("title") for x in response.json()]
-        self.assertIn("Impostazioni Design Plone", titles)
+        uo = api.content.create(
+            container=self.portal,
+            type="UnitaOrganizzativa",
+            title="UO",
+            geolocation=Geolocation(25, 25),
+        )
+
+        summary = getMultiAdapter(
+            (uo, self.layer["request"]), ISerializeToJsonSummary
+        )()
+
+        self.assertDictEqual(
+            {
+                "longitude": uo.geolocation.longitude,
+                "latitude": uo.geolocation.latitude,
+            },
+            summary["geolocation"],
+        )
```

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_setup.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_summary_serializer.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_summary_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/tests/test_vocabularies.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/upgrades/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/upgrades/configure.zcml`

 * *Files 1% similar despite different names*

```diff
@@ -740,8 +740,19 @@
       destination="7009"
       >
     <genericsetup:upgradeStep
         title="Add plone.excludefromnavigation to Venue"
         handler=".upgrades.to_7009"
         />
   </genericsetup:upgradeSteps>
+  <genericsetup:upgradeSteps
+      profile="design.plone.contenttypes:default"
+      source="7009"
+      destination="7010"
+      >
+    <genericsetup:upgradeStep
+        title="Upgrade for CMFPlone syndication"
+        handler=".upgrades.to_7010"
+        />
+  </genericsetup:upgradeSteps>
+
 </configure>
```

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/upgrades/draftjs_converter.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/upgrades/draftjs_converter.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/upgrades/to_7001.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/upgrades/to_7001.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/upgrades/to_7002.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/upgrades/to_7002.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/upgrades/upgrades.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/upgrades/upgrades.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from design.plone.contenttypes.controlpanels.settings import IDesignPloneSettings
 from design.plone.contenttypes.setuphandlers import remove_blocks_behavior
 from design.plone.contenttypes.upgrades.draftjs_converter import to_draftjs
 from design.plone.contenttypes.utils import create_default_blocks
 from plone import api
 from plone.app.textfield.value import RichTextValue
 from plone.app.upgrade.utils import installOrReinstallProduct
+from plone.base.interfaces.syndication import ISiteSyndicationSettings
 from plone.dexterity.utils import iterSchemata
+from plone.registry.interfaces import IRegistry
 from Products.CMFPlone.interfaces import ISelectableConstrainTypes
 from redturtle.bandi.interfaces.settings import IBandoSettings
 from transaction import commit
 from z3c.relationfield import RelationValue
 from zope.component import getUtility
 from zope.event import notify
 from zope.intid.interfaces import IIntIds
@@ -1205,37 +1207,14 @@
     GREEN = "\033[92m"
     ENDC = "\033[0m"
     RED = "\033[91m"
     DARKCYAN = "\033[36m"
     YELLOW = "\033[93m"
 
 
-# XXX: le prenotazioni non sono necessariamente all'interno del servizio
-# def add_ioprenoto_folder(context):
-#     """Adds PrenotazioniFoldersContainer object to Servizio c.t. object"""
-#     catalog = api.portal.get_tool("portal_catalog")
-#     for servizio in catalog(portal_type="Servizio"):
-#         if not catalog(
-#             portal_type="PrenotazioniFolderContainer", path=servizio.getPath()
-#         ):
-#             container = servizio.getObject()
-#             if "PrenotazioniFolderContainer" in getattr(
-#                 context, "allowedContentTypes", None
-#             ):
-#                 api.content.create(
-#                     type="PrenotazioniFolderContainer",
-#                     title="Cartella delle prenotazioni",
-#                     container=container,
-#                 )
-#             else:
-#                 raise Exception(
-#                     "Can not mirgate so as PrenotazioniFolderContainer is not allowed"
-#                 )
-
-
 def update_uo_contact_info(context):
     brains = api.portal.get_tool("portal_catalog")(portal_type="UnitaOrganizzativa")
     logger.info(
         f"{colors.DARKCYAN} Inizio la pulzia delle {len(brains)} UO campo contact_info {colors.ENDC}"  # noqa
     )
     for brain in brains:
         obj = brain.getObject()
@@ -1422,7 +1401,87 @@
         i += 1
         if i % 100 == 0:
             logger.info("Progress: {}/{}".format(i, tot))
         venue = brain.getObject()
         if not getattr(venue, "exclude_from_nav", None):
             setattr(venue, "exclude_from_nav", False)
             venue.reindexObject(idxs=["exclude_from_nav"])
+
+
+def to_7010(context):
+    registry = getUtility(IRegistry)
+    prefix = "Products.CMFPlone.interfaces.syndication.ISiteSyndicationSettings"
+
+    # get the old values
+    old_attributes = [
+        attribute for attribute in registry.records if attribute.startswith(prefix)
+    ]
+    if not old_attributes:
+        logger.info(
+            f"{colors.GREEN} We already have the correct interface. Nothing to do here! {colors.ENDC}"
+        )
+        return
+    old_values = {
+        attribute.split(".")[-1]: registry.records[attribute].value
+        for attribute in old_attributes
+    }
+    logger.info(
+        f"{colors.DARKCYAN} Deleting old ISiteSyndicationSettings Records {colors.ENDC}"
+    )
+    # delete the old records
+    for attribute in old_attributes:
+        del registry.records[attribute]
+
+    # import the new interface
+    logger.info(f"{colors.DARKCYAN} Setup new interface in the registry {colors.ENDC}")
+    context.runImportStepFromProfile(
+        "profile-design.plone.contenttypes:fix_syndication", "plone.app.registry", False
+    )
+    logger.info(
+        f"{colors.DARKCYAN} Set the old values into the new registry records{colors.ENDC}"
+    )
+    # set the old values into the new records
+    default_values = {
+        "allowed": True,
+        "allowed_feed_types": (
+            "RSS|RSS 1.0",
+            "rss.xml|RSS 2.0",
+            "atom.xml|Atom",
+            "itunes.xml|iTunes",
+        ),
+        "default_enabled": False,
+        "max_items": 15,
+        "render_body": False,
+        "search_rss_enabled": True,
+        "show_author_info": True,
+        "show_syndication_button": False,
+        "show_syndication_link": False,
+        "site_rss_items": tuple(),
+    }
+
+    for attribute in old_values:
+        # we could have None value and we can't set None with set_registry_record
+        # so we can set the value to the default.
+        if old_values[attribute] == None:  # noqa
+            old_values[attribute] = default_values[attribute]
+            logger.info(
+                f"{colors.RED } Fix {attribute} to default: {old_values[attribute]} {colors.ENDC}"
+            )
+
+        if attribute == "site_rss_items" and old_values[attribute]:
+            logger.info(
+                f"{colors.RED} Please manually fix {attribute} with old value"
+                f" {old_values[attribute]} {colors.ENDC}"
+            )
+            continue
+
+        logger.info(
+            f"{colors.DARKCYAN} Set {attribute} to  {old_values[attribute]} {colors.ENDC}"
+        )
+        api.portal.set_registry_record(
+            name=attribute,
+            value=old_values[attribute],
+            interface=ISiteSyndicationSettings,
+        )
+    logger.info(
+        f"{colors.GREEN}ISiteSyndicationSettings interface fixed! {colors.ENDC}"
+    )
```

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/utils.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/utils.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/configure.zcml` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/mockup.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/mockup.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/people_vocabulary.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/people_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py` & `design.plone.contenttypes-6.0.4/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.3/src/design.plone.contenttypes.egg-info/PKG-INFO` & `design.plone.contenttypes-6.0.4/src/design.plone.contenttypes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.contenttypes
-Version: 6.0.3
+Version: 6.0.4
 Summary: DesignItalia contenty types
 Home-page: https://github.com/collective/design.plone.contenttypes
 Author: RedTurtle
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.contenttypes
 Project-URL: Source, https://github.com/RedTurtle/design.plone.contenttypes
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
-Provides-Extra: ioprenoto
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 [![Latest Version](https://img.shields.io/pypi/v/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Supported - Python Versions](https://img.shields.io/pypi/pyversions/design.plone.contenttypes.svg?style=plastic)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![License](https://img.shields.io/pypi/l/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
@@ -486,14 +485,23 @@
 - RedTurtle, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
 
+6.0.4 (2023-04-19)
+------------------
+
+- Remove redturtle.prenotazioni integration.
+  [cekk]
+- Fix syndication.
+  [lucabel]
+
+
 6.0.3 (2023-04-18)
 ------------------
 
 - Change check_servizi making optional the check for
   field "condizioni_di_servizio" and removing the check for
   the "contact_info" field.
   Import a fontawesome cdn in this view to show the "V" icon.
```

### Comparing `design.plone.contenttypes-6.0.3/src/design.plone.contenttypes.egg-info/SOURCES.txt` & `design.plone.contenttypes-6.0.4/src/design.plone.contenttypes.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,15 @@
 src/design/plone/contenttypes/profiles/default/types/Persona.xml
 src/design/plone/contenttypes/profiles/default/types/Pratica.xml
 src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
 src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
 src/design/plone/contenttypes/profiles/default/types/Servizio.xml
 src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
 src/design/plone/contenttypes/profiles/default/types/Venue.xml
+src/design/plone/contenttypes/profiles/fix_syndication/registry.xml
 src/design/plone/contenttypes/profiles/to_3000/controlpanel.xml
 src/design/plone/contenttypes/profiles/to_3000/registry.xml
 src/design/plone/contenttypes/profiles/uninstall/browserlayer.xml
 src/design/plone/contenttypes/restapi/__init__.py
 src/design/plone/contenttypes/restapi/configure.zcml
 src/design/plone/contenttypes/restapi/converters.py
 src/design/plone/contenttypes/restapi/correlati.py
@@ -243,17 +244,14 @@
 src/design/plone/contenttypes/restapi/services/controlpanel.py
 src/design/plone/contenttypes/restapi/services/content/__init__.py
 src/design/plone/contenttypes/restapi/services/content/add.py
 src/design/plone/contenttypes/restapi/services/content/configure.zcml
 src/design/plone/contenttypes/restapi/services/modulistica_items/__init__.py
 src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml
 src/design/plone/contenttypes/restapi/services/modulistica_items/get.py
-src/design/plone/contenttypes/restapi/services/prenotazioni_folders_list/__init__.py
-src/design/plone/contenttypes/restapi/services/prenotazioni_folders_list/configure.zcml
-src/design/plone/contenttypes/restapi/services/prenotazioni_folders_list/get.py
 src/design/plone/contenttypes/restapi/services/scadenziario/__init__.py
 src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml
 src/design/plone/contenttypes/restapi/services/scadenziario/post.py
 src/design/plone/contenttypes/restapi/services/trasparenza/__init__.py
 src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml
 src/design/plone/contenttypes/restapi/services/trasparenza/get.py
 src/design/plone/contenttypes/restapi/services/types/__init__.py
@@ -283,15 +281,14 @@
 src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py
 src/design/plone/contenttypes/tests/test_ct_persona.py
 src/design/plone/contenttypes/tests/test_ct_servizio.py
 src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py
 src/design/plone/contenttypes/tests/test_filefield_view_mode_serializer.py
 src/design/plone/contenttypes/tests/test_move_news_items_view.py
 src/design/plone/contenttypes/tests/test_relateditems_with_dates.py
-src/design/plone/contenttypes/tests/test_service_prenotazioni_folders_list.py
 src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py
 src/design/plone/contenttypes/tests/test_setup.py
 src/design/plone/contenttypes/tests/test_summary_serializer.py
 src/design/plone/contenttypes/tests/test_uo_summary_serializer.py
 src/design/plone/contenttypes/tests/test_vocabularies.py
 src/design/plone/contenttypes/upgrades/__init__.py
 src/design/plone/contenttypes/upgrades/configure.zcml
```

